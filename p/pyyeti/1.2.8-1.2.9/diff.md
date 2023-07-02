# Comparing `tmp/pyyeti-1.2.8.tar.gz` & `tmp/pyyeti-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyeti-1.2.8.tar", last modified: Mon Jun 19 22:33:01 2023, max compression
+gzip compressed data, was "pyyeti-1.2.9.tar", last modified: Sun Jul  2 17:11:44 2023, max compression
```

## Comparing `pyyeti-1.2.8.tar` & `pyyeti-1.2.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-19 22:32:39.000000 pyyeti-1.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-19 22:32:39.000000 pyyeti-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 22:33:01.885629 pyyeti-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-19 22:32:39.000000 pyyeti-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/pyyeti/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106717 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/cla/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_magpct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rptext1.py
--rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rptpct1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rpttab1.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    50944 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_def.py
--rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_event.py
--rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_results_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/rel_disp_dtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/column_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cyclecount.py
--rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/datacursor.py
--rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    69230 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/era.py
--rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/expmint.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/fdepsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/frclim.py
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/guitools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/locate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/nastran/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131608 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)   136601 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/n2p.py
--rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/op2.py
--rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/op4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/ode/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/_base_ode_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/freqdirect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/frf_mode_participation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solvecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveexp1.py
--rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveexp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solvenewmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    69302 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/pp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42978 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/rainflow/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/c_rain.c
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/py_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/srs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ssmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56785 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/pyyeti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-06-19 22:32:39.000000 pyyeti-1.2.8/scripts/lsop2
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 22:32:39.000000 pyyeti-1.2.8/scripts/lsop4
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-19 22:33:01.889629 pyyeti-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-19 22:32:39.000000 pyyeti-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/tests/nas2cam_csuper/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.asm
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.op4
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.pch
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/tests/nastran_drm12/
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/drm12.op2
--rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/drm12.op4
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-02 17:11:24.000000 pyyeti-1.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-02 17:11:24.000000 pyyeti-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-02 17:11:44.418480 pyyeti-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-02 17:11:24.000000 pyyeti-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.414480 pyyeti-1.2.9/pyyeti/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106717 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.414480 pyyeti-1.2.9/pyyeti/cla/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/_magpct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/_rptext1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/_rptpct1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/_rpttab1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50944 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/dr_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/dr_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/dr_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/dr_results_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cla/rel_disp_dtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/column_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/cyclecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/datacursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70785 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/era.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/expmint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/fdepsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/frclim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/guitools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/locate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/pyyeti/nastran/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/nastran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131608 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/nastran/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136601 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/nastran/n2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/nastran/op2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/nastran/op4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/pyyeti/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/_base_ode_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/freqdirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/frf_mode_participation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/solvecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/solveexp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/solveexp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/solvenewmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69302 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ode/solveunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43744 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/pyyeti/rainflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/rainflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/rainflow/c_rain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/rainflow/py_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/srs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ssmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57514 2023-07-02 17:11:24.000000 pyyeti-1.2.9/pyyeti/ytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.414480 pyyeti-1.2.9/pyyeti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-02 17:11:44.000000 pyyeti-1.2.9/pyyeti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-02 17:11:44.000000 pyyeti-1.2.9/pyyeti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:11:44.000000 pyyeti-1.2.9/pyyeti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 17:11:44.000000 pyyeti-1.2.9/pyyeti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 17:11:44.000000 pyyeti-1.2.9/pyyeti.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-07-02 17:11:24.000000 pyyeti-1.2.9/scripts/lsop2
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-02 17:11:24.000000 pyyeti-1.2.9/scripts/lsop4
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 17:11:44.422480 pyyeti-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-02 17:11:24.000000 pyyeti-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.410480 pyyeti-1.2.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/tests/nas2cam_csuper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nas2cam_csuper/inboard.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nas2cam_csuper/inboard.op4
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nas2cam_csuper/inboard.pch
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nas2cam_csuper/nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nas2cam_csuper/nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:11:44.418480 pyyeti-1.2.9/tests/nastran_drm12/
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nastran_drm12/drm12.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nastran_drm12/drm12.op4
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nastran_drm12/inboard_nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-07-02 17:11:24.000000 pyyeti-1.2.9/tests/nastran_drm12/inboard_nas2cam.op4
```

### Comparing `pyyeti-1.2.8/LICENSE.txt` & `pyyeti-1.2.9/LICENSE.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2022, pyYeti Developers.
+Copyright (c) 2015-2023, pyYeti Developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
     * Redistributions of source code must retain the above copyright
```

### Comparing `pyyeti-1.2.8/PKG-INFO` & `pyyeti-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.8
+Version: 1.2.9
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.8 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.9 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.8/README.md` & `pyyeti-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/__init__.py` & `pyyeti-1.2.9/pyyeti/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cb.py` & `pyyeti-1.2.9/pyyeti/cb.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/_magpct.py` & `pyyeti-1.2.9/pyyeti/cla/_magpct.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/_rptext1.py` & `pyyeti-1.2.9/pyyeti/cla/_rptext1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/_rptpct1.py` & `pyyeti-1.2.9/pyyeti/cla/_rptpct1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/_rpttab1.py` & `pyyeti-1.2.9/pyyeti/cla/_rpttab1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/_utilities.py` & `pyyeti-1.2.9/pyyeti/cla/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/dr_def.py` & `pyyeti-1.2.9/pyyeti/cla/dr_def.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/dr_event.py` & `pyyeti-1.2.9/pyyeti/cla/dr_event.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/dr_results.py` & `pyyeti-1.2.9/pyyeti/cla/dr_results.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/dr_results_plots.py` & `pyyeti-1.2.9/pyyeti/cla/dr_results_plots.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cla/rel_disp_dtm.py` & `pyyeti-1.2.9/pyyeti/cla/rel_disp_dtm.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/column_plotter.py` & `pyyeti-1.2.9/pyyeti/column_plotter.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/cyclecount.py` & `pyyeti-1.2.9/pyyeti/cyclecount.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/datacursor.py` & `pyyeti-1.2.9/pyyeti/datacursor.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/dsp.py` & `pyyeti-1.2.9/pyyeti/dsp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/era.py` & `pyyeti-1.2.9/pyyeti/era.py`

 * *Files 2% similar despite different names*

```diff
@@ -1386,27 +1386,28 @@
     resp,
     sr,
     *,
     ref_channels="all",
     lag_start=1,
     lag_stop,
     domain="time",
+    unbiased=True,
+    demean=True,
     nperseg=None,
     window="hann",
-    nfft=None,
     noverlap=None,
 ):
     """
     Use NExT method to prepare measurement data for :class:`ERA`
 
     **BETA**
 
     This routine uses the "Natural Excitation Technique" to process
-    response measurements into free-decay-like signals using
-    cross-correlations. This can be done in either the time-domain or
+    response measurements into free-decay-like signals using auto and
+    cross correlations. This can be done in either the time-domain or
     the frequency-domain. The resulting signals can then be input to
     ERA (the Eigensystem Realization Algorithm) for system
     identification. See references [#nxt1]_ and [#nxt2]_.
 
     Parameters
     ----------
     resp : 1d or 2d ndarray
@@ -1436,45 +1437,53 @@
         frequency you are interested in for the current run. For
         example, an initial value for `lag_stop` might be computed
         such that the decay will have time for one full cycle of the
         estimated lowest frequency (in Hz)::
 
             lag_stop = lag_start + sr / lowest_est_freq
 
-        .. note::
-
-            `lag_stop` must be less than ``nperseg / 2`` if `domain`
-            is "frequency". This is due to the symmetric nature of the
-            cross-correlations. This shouldn't be much of a
-            restriction however, as the `lag_stop` value will
-            typically be considerably less than this for good results.
-
     domain : string
         Either "time" or "frequency" to specify how this routine is to
         compute the cross-correlations. If "time",
         :func:`scipy.signal.correlate` is used to compute the
         correlations using the entire time history for each
         cross-correlation. If "frequency", :func:`scipy.fft.ifft` and
         :func:`scipy.signal.csd` are used together to compute the
         correlations, along with looping and windowing and
         averaging. If `domain` is "frequency", see the inputs
-        `nperseg`, `window`, `nfft`, and `noverlap`.
+        `nperseg`, `window`, and `noverlap`.
+
+        .. note::
+           To get the frequency domain method to give identical
+           results to the time domain method, set `nperseg` to the
+           entire signal and `window` to "boxcar".
+
+    unbiased : bool; optional
+        If True, use unbiased estimates for the correlations. This
+        should be True for ERA.
+    demean : bool; optional
+        If True (the default), subtract the mean from each signal
+        prior to any other processing. Auto and cross correlations
+        computed with demeaned signals are often called auto and cross
+        covariances.
     nperseg : integer
         Required if `domain` is "frequency". Specifies the window size
-        to pass to :func:`scipy.signal.csd`. If `nperseg` is too
-        small, the damping for the lower frequency modes will likely
-        be inflated. In order to get any benefit that might come from
+        to pass to :func:`scipy.signal.csd`. Generally, using higher
+        values for `nperseg` will result in higher quality
+        correlations. In order to get any benefit that might come from
         averaging multiple windows, a reasonable initial setting for
         this value might be to choose the first power-of-2 less than N
         / 2 where N is the number of time-steps. That would result in
         the largest power-of-2 size window size (for fast processing)
         while still giving you 3 windows to average.
-    window, nfft, noverlap : optional
+    window, noverlap : optional
         These inputs are only used if `domain` is "frequency". The are
-        all passed to :func:`scipy.signal.csd`.
+        all passed to :func:`scipy.signal.csd`. Note that the ``nfft``
+        input is supplied by this routine and is set to ``2 *
+        nperseg``.
 
     Returns
     -------
     3d ndarray
         Decay-like responses shaped as expected by :class:`ERA`:
         ``n_channels x n_decay_tsteps x n_ref_channels``. :class:`ERA`
         will interpret the number of reference channels as the number
@@ -1554,14 +1563,42 @@
         >>> n = len(t)
         >>> sr = 1 / dt
         >>> np.random.seed(1)  # for repeatability
         >>> F = np.random.randn(3, len(t))
         >>> ts = ode.SolveUnc(M, D, K, dt)
         >>> sol = ts.tsolve(force=F)
 
+        Before calling ERA, we'll plot some auto and cross
+        correlations directly from NExT. These should have the same
+        properties as impulse response functions:
+
+        >>> lag_stop = 200
+        >>> t_irf = t[1 : lag_stop + 1]
+        >>> irf = era.NExT(sol.a, sr, lag_stop=lag_stop)
+        >>>
+        >>> fig = plt.figure("corr comp", clear=True, figsize=(6.4, 6.4))
+        >>> ax = fig.subplots(4, 1)
+        >>>
+        >>> _ = ax[0].plot(t, sol.a.T)
+        >>> _ = ax[0].set_title("Original data")
+        >>> _ = ax[0].set_ylabel("Acce")
+        >>>
+        >>> # loop over all 3 ref channels:
+        >>> for ref in range(irf.shape[2]):
+        ...     # loop over all 3 output channels:
+        ...     for out in range(irf.shape[0]):
+        ...         _ = ax[ref + 1].plot(t_irf, irf[out, :, ref])
+        ...     _ = ax[ref + 1].set_title(f"IRFs with reference channel {ref}")
+        ...     _ = ax[ref + 1].set_ylabel("X-corr IRFs")
+        >>> _ = ax[3].set_xlabel("Time (s)")
+        >>> fig.tight_layout()
+
+    .. plot::
+        :context: close-figs
+
         Use the time-domain method of NExT and call :class:`ERA` to
         get estimates of frequency, damping, and mode-shapes. We'll
         use a `lag_stop` of 75 (from sr / lowest_freq = 100 / 1.33 ~=
         75).
 
         >>> era_fit = era.ERA(
         ...     era.NExT(sol.a, sr, lag_stop=75),
@@ -1570,24 +1607,24 @@
         ...     input_labels=["x", "y", "z"],
         ...     figure_label="Time Domain ERA Fit",
         ... )
         <BLANKLINE>
         Current fit includes all modes:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-        *    1     1.3258    2.4155  *0.676  *0.996  *0.998  *1.000  *0.998  *1.000
-        *    2     7.5586    7.0610  *0.656  *0.715  *0.844  *1.000  *0.843  *1.000
-        *    3    13.8643    4.6710  *1.000  *0.721  *0.852  *1.000  *0.852  *1.000
+        *    1     1.3258    2.2962  *0.676  *0.994  *0.999  *1.000  *0.999  *1.000
+        *    2     7.5588    7.0415  *0.656  *0.714  *0.859  *1.000  *0.859  *0.999
+        *    3    13.8644    4.6586  *1.000  *0.722  *0.845  *1.000  *0.845  *1.000
         <BLANKLINE>
         Auto-selected modes fit:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-             1     1.3258    2.4155   0.676   0.996   0.998   1.000   0.998   1.000
-             2     7.5586    7.0610   0.656   0.715   0.844   1.000   0.843   1.000
-             3    13.8643    4.6710   1.000   0.721   0.852   1.000   0.852   1.000
+             1     1.3258    2.2962   0.676   0.994   0.999   1.000   0.999   1.000
+             2     7.5588    7.0415   0.656   0.714   0.859   1.000   0.859   0.999
+             3    13.8644    4.6586   1.000   0.722   0.845   1.000   0.845   1.000
 
     .. plot::
         :context: close-figs
 
         That seemed to work out pretty well! Now we'll try the
         frequency-domain method of NExT (the increased `svd_tol` gave
         slightly better results in this case):
@@ -1606,24 +1643,24 @@
         ...     input_labels=["x", "y", "z"],
         ...     figure_label="Frequency Domain ERA Fit",
         ... )
         <BLANKLINE>
         Current fit includes all modes:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-        *    1     1.3231    2.1499  *0.691  *0.993  *0.997  *1.000  *0.997  *1.000
-        *    2     7.5231    7.1348  *0.626  *0.640  *0.801  *0.997  *0.798  *0.999
-        *    3    13.9075    4.2107  *1.000  *0.684  *0.813  *1.000  *0.813  *0.999
+        *    1     1.3231    1.8534  *0.691  *0.993  *0.997  *1.000  *0.997  *1.000
+        *    2     7.5233    7.0859  *0.626  *0.642  *0.802  *0.997  *0.800  *0.999
+        *    3    13.9076    4.1781  *1.000  *0.686  *0.814  *1.000  *0.814  *0.999
         <BLANKLINE>
         Auto-selected modes fit:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-             1     1.3231    2.1499   0.691   0.993   0.997   1.000   0.997   1.000
-             2     7.5231    7.1348   0.626   0.640   0.801   0.997   0.798   0.999
-             3    13.9075    4.2107   1.000   0.684   0.813   1.000   0.813   0.999
+             1     1.3231    1.8534   0.691   0.993   0.997   1.000   0.997   1.000
+             2     7.5233    7.0859   0.626   0.642   0.802   0.997   0.800   0.999
+             3    13.9076    4.1781   1.000   0.686   0.814   1.000   0.814   0.999
 
     .. plot::
         :context: close-figs
 
         Both of the above examples used all channels as reference
         channels. The next example uses just the first measurement as
         the reference channel (which also means that the only
@@ -1637,70 +1674,81 @@
         ...     input_labels=["x", "y", "z"],
         ...     figure_label="Time Domain ERA Fit",
         ... )
         <BLANKLINE>
         Current fit includes all modes:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-        *    1     1.3455    1.8899  *0.881  *0.992  *0.992  *1.000  *0.992  *1.000
-             2     7.4679    4.5610   0.238  *0.785  *0.873  *0.978  *0.854  *0.998
-        *    3    13.8546    4.9336  *1.000  *0.893  *0.924  *0.999  *0.923  *1.000
-             4    14.5075   -3.7478   0.246  *0.440  *0.604   0.226   0.137  *0.982
+        *    1     1.3259    2.2077  *0.888  *0.989  *0.989  *1.000  *0.989  *1.000
+        *    2    13.8740    4.6136  *1.000  *0.688  *0.827  *0.999  *0.826  *1.000
         <BLANKLINE>
         Auto-selected modes fit:
           Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
           ----  ---------  --------  ------  ------  ------  ------  ------  ------
-             1     1.3455    1.8899   0.881   0.992   0.992   1.000   0.992   1.000
-             2    13.8546    4.9336   1.000   0.893   0.924   0.999   0.923   1.000
+             1     1.3259    2.2077   0.888   0.989   0.989   1.000   0.989   1.000
+             2    13.8740    4.6136   1.000   0.688   0.827   0.999   0.826   1.000
 
-        All three modes were identified, but the 7.4 Hz mode was not
-        auto-selected because the MSV indicator was too low. To
-        successfully auto-select it, we could either lower the MSV
-        value, use a different reference channel, or add more
-        reference channels.
+    In that case, the 7.4 Hz mode was not identified. From the plot, a
+    decent fit was found without it since the 7.x Hz content is not
+    visibly prominent. To successfully identify that mode, it would be
+    best to add more reference channels.
     """
     resp = np.atleast_2d(resp)
+    if demean:
+        resp = resp - resp.mean(axis=1, keepdims=True)
     n = resp.shape[1]
 
     if ref_channels == "all":
         ref_channels = np.arange(0, resp.shape[0])
     else:
         ref_channels = np.atleast_1d(ref_channels)
 
+    lags = slice(lag_start, lag_stop + 1)
+
     # compute cross-correlation functions
     xc = []
     if domain == "time":
         for ref in resp[ref_channels]:
             xc_ref = []
             for sig in resp:
-                corr = signal.correlate(ref, sig, mode="same")[n // 2 :]
-                xc_ref.append(corr[lag_start : lag_stop + 1])
+                corr = signal.correlate(sig, ref, mode="full")[n - 1 :]
+                xc_ref.append(corr[lags])
             xc.append(xc_ref)
+
+        if unbiased:
+            scale = np.arange(n, 0, -1)[lags]
+            xc = np.array(xc) / scale
+
     elif domain == "frequency":
         # csd will scale values down by window.sum() ** 2 ... we don't
         # need or necessarily want that, so scaling up by nperseg ** 2
-        # is reasonable
+        # is reasonable (as if window == "boxcar"):
         sc = nperseg**2
         for ref in resp[ref_channels]:
             xc_ref = []
             for sig in resp:
                 f, csd = signal.csd(
                     ref,
                     sig,
                     fs=sr,
                     window=window,
                     nperseg=nperseg,
-                    nfft=nfft,
+                    nfft=nperseg * 2,
                     noverlap=noverlap,
                     scaling="spectrum",
                     return_onesided=False,
                 )
-                corr = fft.ifft(csd).real * sc
-                xc_ref.append(corr[lag_start : lag_stop + 1])
+                corr = fft.ifft(csd).real
+                xc_ref.append(corr[lags] * sc)
             xc.append(xc_ref)
+
+        if unbiased:
+            scale = np.arange(nperseg, 0, -1)[lags]
+            xc = np.array(xc) / scale
+
     else:
         raise ValueError(
             "invalid value for `domain`; must be either 'time' or 'frequency'"
         )
 
     # put reference channels last instead of first for ERA:
     return np.moveaxis(xc, 0, -1)
```

### Comparing `pyyeti-1.2.8/pyyeti/expmint.py` & `pyyeti-1.2.9/pyyeti/expmint.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/fdepsd.py` & `pyyeti-1.2.9/pyyeti/fdepsd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/frclim.py` & `pyyeti-1.2.9/pyyeti/frclim.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/guitools.py` & `pyyeti-1.2.9/pyyeti/guitools.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,48 @@
 
 def get_file_name(f, read):
     """
     Utility function to get the file name using guitools if needed.
 
     Parameters
     ----------
-    f : string or None
-        File name or directory name or None. If `f` is not None or is
-        not a directory name, this routine just returns it as is. If
-        it is a directory name, it is used as the `initialdir` option
-        to :func:`askopenfilename` or :func:`asksaveasfilename`.
+    f : :class:`pathlib.Path` object or string or None
+        File name or directory name (something that :func:`os.fspath`
+        accepts) or None. If `f` is not None or is not a directory
+        name, this routine just returns it as is. If it is a directory
+        name, it is used as the `initialdir` option to
+        :func:`askopenfilename` or :func:`asksaveasfilename`.
     read : bool
         If True, calls :func:`askopenfilename` to get file name.
         Otherwise, :func:`asksaveasfilename` is called.
 
     Returns
     -------
     filename : string
         The selected filename.
     """
-    if isinstance(f, str) and os.path.isdir(f):  # pragma: no cover
-        initialdir = f
-        f = None
-    else:
+    try:
+        fs = os.fspath(f)
+    except TypeError:
+        fs = f
         initialdir = None
-    if f is None:  # pragma: no cover
+    else:
+        if os.path.isdir(fs):  # pragma: no cover
+            initialdir = fs
+            fs = None
+        else:
+            initialdir = None
+
+    if fs is None:  # pragma: no cover
         if read:
             return askopenfilename(initialdir=initialdir)
         else:
             return asksaveasfilename(initialdir=initialdir)
-    return f
+
+    return fs
 
 
 def askopenfilename(title=None, filetypes=None, initialdir=None):  # pragma: no cover
     """
     Use GUI to select file for reading
 
     Parameters
```

### Comparing `pyyeti-1.2.8/pyyeti/locate.py` & `pyyeti-1.2.9/pyyeti/locate.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/nastran/bulk.py` & `pyyeti-1.2.9/pyyeti/nastran/bulk.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/nastran/n2p.py` & `pyyeti-1.2.9/pyyeti/nastran/n2p.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/nastran/op2.py` & `pyyeti-1.2.9/pyyeti/nastran/op2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/nastran/op4.py` & `pyyeti-1.2.9/pyyeti/nastran/op4.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/__init__.py` & `pyyeti-1.2.9/pyyeti/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/_base_ode_class.py` & `pyyeti-1.2.9/pyyeti/ode/_base_ode_class.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/_utilities.py` & `pyyeti-1.2.9/pyyeti/ode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/freqdirect.py` & `pyyeti-1.2.9/pyyeti/ode/freqdirect.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/frf_mode_participation.py` & `pyyeti-1.2.9/pyyeti/ode/frf_mode_participation.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/solvecdf.py` & `pyyeti-1.2.9/pyyeti/ode/solvecdf.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/solveexp1.py` & `pyyeti-1.2.9/pyyeti/ode/solveexp1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/solveexp2.py` & `pyyeti-1.2.9/pyyeti/ode/solveexp2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/solvenewmark.py` & `pyyeti-1.2.9/pyyeti/ode/solvenewmark.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ode/solveunc.py` & `pyyeti-1.2.9/pyyeti/ode/solveunc.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/pp.py` & `pyyeti-1.2.9/pyyeti/pp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/psd.py` & `pyyeti-1.2.9/pyyeti/psd.py`

 * *Files 2% similar despite different names*

```diff
@@ -823,28 +823,29 @@
     if fs != 0:
         _, F, _, P = rescale(P, F, n_oct=fs, frange=(s, e), extendends=extendends)
     else:
         P = P * F[1]
         pv = (F >= s) & (F <= e)
         F = F[pv]
         P = P[pv]
-    v = P / pref ** 2
+    v = P / pref**2
     return F, 10 * np.log10(v), 10 * np.log10(np.sum(v))
 
 
 def psd2time(
     spec,
     fstart,
     fstop,
     *,
     ppc=10,
     df=None,
     winends=None,
     gettime=False,
     expand_method="interp",
+    rng=None,
 ):
     r"""
     Generate a 'random' time domain signal given a PSD specification.
 
     Parameters
     ----------
     spec : 2d ndarray or 2-element tuple/list
@@ -889,14 +890,25 @@
     expand_method : str; optional
         Either 'interp' or 'rescale', referring to which function in
         this module will be used to expand input `spec` to all needed
         frequencies. Use 'interp' if `spec` is a specification with
         constant dB/octave slopes. Use 'rescale' if `spec` provides
         the PSD levels on a center-band scale. See :func:`interp` and
         :func:`rescale` for more information.
+    rng : :class:`numpy.random.Generator` object or None; optional
+        If not None, uniform deviates are generated via
+        :func:`rng.random`. If None, the singleton generator
+        :func:`numpy.random.rand` is used. Supplying your own `rng`
+        can be handy for parallel applications, for example, when you
+        need repeatability. For illustration, the following creates a
+        Mersenne Twister generator::
+
+            from numpy.random import Generator, MT19937
+            seed = 1
+            rng = Generator(MT19937(seed))
 
     Returns
     -------
     sig : 1d ndarray
         The time domain signal with properties set to match input PSD
         spectrum. Duration of signal: ``1 / df``.
     sr : scalar
@@ -982,21 +994,25 @@
 
     Examples
     --------
     .. plot::
         :context: close-figs
 
         >>> import numpy as np
+        >>> from numpy.random import Generator, MT19937
         >>> from pyyeti import psd
         >>> spec = np.array([[20,  .0768],
         ...                  [50,  .48],
         ...                  [100, .48]])
-        >>> sig, sr = psd.psd2time(spec, ppc=10, fstart=35,
-        ...                        fstop=70, df=.01,
-        ...                        winends=dict(portion=.01))
+        >>> we = dict(portion=0.01)
+        >>> seed = 1
+        >>> rng = Generator(MT19937(seed))
+        >>> sig, sr = psd.psd2time(
+        ...     spec, 35, 70, ppc=10, df=.01, winends=we, rng=rng,
+        ... )
         >>> sr  # the sample rate should be 70*10 = 700
         700.0
 
         Compare the resulting psd to the spec from 37 to 68:
 
         >>> import matplotlib.pyplot as plt
         >>> import scipy.signal as signal
@@ -1079,15 +1095,19 @@
     nbot = m - ntop - len(amp)
     if nbot > 0:
         amp = np.hstack((np.zeros(ntop), amp, np.zeros(nbot)))
     else:
         amp = np.hstack((np.zeros(ntop), amp))
 
     # generate F(t)
-    phi = np.random.rand(m) * np.pi * 2  # random phase angle
+    # - use uniformly distributed random phase angle:
+    if rng is None:
+        phi = np.random.rand(m) * np.pi * 2
+    else:
+        phi = rng.random(m) * np.pi * 2
 
     # force these terms to be pure cosine
     phi[0] = 0.0
     if not odd:
         phi[m - 1] = 0
 
     # coefficients:
```

### Comparing `pyyeti-1.2.8/pyyeti/rainflow/c_rain.c` & `pyyeti-1.2.9/pyyeti/rainflow/c_rain.c`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/rainflow/py_rain.py` & `pyyeti-1.2.9/pyyeti/rainflow/py_rain.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/srs.py` & `pyyeti-1.2.9/pyyeti/srs.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ssmodel.py` & `pyyeti-1.2.9/pyyeti/ssmodel.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/stats.py` & `pyyeti-1.2.9/pyyeti/stats.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/writer.py` & `pyyeti-1.2.9/pyyeti/writer.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/pyyeti/ytools.py` & `pyyeti-1.2.9/pyyeti/ytools.py`

 * *Files 1% similar despite different names*

```diff
@@ -950,28 +950,39 @@
             if tmp <= 0:
                 c += 1
         count[i] = c
     return count
 
 
 def eig_si(
-    K, M, Xk=None, f=None, p=10, mu=0, tol=1e-6, pmax=None, maxiter=50, verbose=True
+    K,
+    M,
+    *,
+    Xk=None,
+    f=None,
+    p=10,
+    mu=0,
+    tol=1e-6,
+    pmax=None,
+    maxiter=50,
+    verbose=True,
+    rng=None,
 ):
     r"""
     Perform subspace iteration to calculate eigenvalues and eigenvectors.
 
     Parameters
     ----------
     K : ndarray
         The stiffness (assumed symmetric).
     M : ndarray
         The mass (assumed positive-definite).
     Xk : ndarray or None
         Initial guess @ eigenvectors; # columns > `p`. If None,
-        random vectors are used from ``np.random.rand()-.5``.
+        random vectors are generated internally; see `rng` below.
     f : scalar or None
         Desired cutoff frequency in Hz. `pmax` will override this if
         set. Takes precedence over `p` if both are input.
     p : scalar or None
         Number of desired eigenpairs (eigenvalues and eigenvectors).
         `pmax` will limit this if set. If `f` is input, `p` is
         calculated internally (from :func:`sturm`).
@@ -981,14 +992,26 @@
         Eigenvalue convergence tolerance.
     pmax : scalar or None
         Maximum number of eigenpairs; no limit if None.
     maxiter : scalar
         Maximum number of iterations.
     verbose : bool
         If True, print status message for each iteration.
+    rng : :class:`numpy.random.Generator` object or None; optional
+        If not None, uniform deviates are generated via
+        :func:`rng.random`. If None, the singleton generator
+        :func:`numpy.random.rand` is used. The deviates range from
+        ``[-0.5, 0.5)``. Supplying your own `rng` can be handy for
+        parallel applications, for example, when you need
+        repeatability. For illustration, the following creates a
+        Mersenne Twister generator::
+
+            from numpy.random import Generator, MT19937
+            seed = 1
+            rng = Generator(MT19937(seed))
 
     Returns
     -------
     lam : ndarray
         Ideally, `p` converged eigenvalues.
     phi : ndarray
         Ideally, p converged eigenvectors.
@@ -1052,19 +1075,21 @@
     [  0.   5.  15.]
     >>> import scipy.linalg as linalg
     >>> k = np.random.randn(40, 40)
     >>> m = np.random.randn(40, 40)
     >>> k = np.dot(k.T, k) * 1000
     >>> m = np.dot(m.T, m) * 10
     >>> w1, phi1 = linalg.eigh(k, m, subset_by_index=(0, 14))
-    >>> w2, phi2, phiv2 = ytools.eig_si(k, m, p=15, mu=-1, tol=1e-12,
-    ...                                 verbose=False)
+    >>> w2, phi2, phiv2 = ytools.eig_si(
+    ...     k, m, p=15, mu=-1, tol=1e-12, verbose=False
+    ... )
     >>> fcut = np.sqrt(w2.max())/2/np.pi * 1.001
-    >>> w3, phi3, phiv3 = ytools.eig_si(k, m, f=fcut, tol=1e-12,
-    ...                                 verbose=False)
+    >>> w3, phi3, phiv3 = ytools.eig_si(
+    ...     k, m, f=fcut, tol=1e-12, verbose=False
+    ... )
     >>> print(np.allclose(w1, w2))
     True
     >>> print(np.allclose(np.abs(phi1), np.abs(phi2)))
     True
     >>> print(np.allclose(w1, w3))
     True
     >>> print(np.allclose(np.abs(phi1), np.abs(phi3)))
@@ -1092,18 +1117,22 @@
     if q > n:
         q = n
     if Xk is not None:
         c = np.size(Xk, 1)
     else:
         c = 0
     if c < q:
+        if rng is None:
+            deviates = np.random.rand(n, q - c) - 0.5
+        else:
+            deviates = rng.random((n, q - c)) - 0.5
         if Xk is None:
-            Xk = np.random.rand(n, q) - 0.5
+            Xk = deviates
         else:
-            Xk = np.hstack((Xk, np.random.rand(n, q - c) - 0.5))
+            Xk = np.hstack((Xk, deviates))
     elif c > q:
         Xk = Xk[:, :q]
 
     lamk = np.ones(q)
     nconv = 0
     loops = 0
     tolc = 1
```

### Comparing `pyyeti-1.2.8/pyyeti.egg-info/PKG-INFO` & `pyyeti-1.2.9/pyyeti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.8
+Version: 1.2.9
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.8 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.9 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.8/pyyeti.egg-info/SOURCES.txt` & `pyyeti-1.2.9/pyyeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/scripts/lsop2` & `pyyeti-1.2.9/scripts/lsop2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/setup.py` & `pyyeti-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
     else:
         kw = {}
 
     install_requires = check_dependencies()
     setup(
         name="pyyeti",
-        version="1.2.8",
+        version="1.2.9",
         url="http://github.com/twmacro/pyyeti/",
         license="BSD",
         author="Tim Widrick",
         install_requires=install_requires,
         author_email="twmacro@gmail.com",
         description=("Tools mostly related to structural dynamics"),
         long_description=long_description,
```

### Comparing `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.asm` & `pyyeti-1.2.9/tests/nas2cam_csuper/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.op4` & `pyyeti-1.2.9/tests/nas2cam_csuper/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.pch` & `pyyeti-1.2.9/tests/nas2cam_csuper/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op2` & `pyyeti-1.2.9/tests/nas2cam_csuper/nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op4` & `pyyeti-1.2.9/tests/nas2cam_csuper/nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nastran_drm12/drm12.op2` & `pyyeti-1.2.9/tests/nastran_drm12/drm12.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nastran_drm12/drm12.op4` & `pyyeti-1.2.9/tests/nastran_drm12/drm12.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op2` & `pyyeti-1.2.9/tests/nastran_drm12/inboard_nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op4` & `pyyeti-1.2.9/tests/nastran_drm12/inboard_nas2cam.op4`

 * *Files identical despite different names*

