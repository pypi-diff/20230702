# Comparing `tmp/funfluid-202307021904.tar.gz` & `tmp/funfluid-202307021923.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202307021904.tar", last modified: Sun Jul  2 11:04:56 2023, max compression
+gzip compressed data, was "funfluid-202307021923.tar", last modified: Sun Jul  2 11:23:07 2023, max compression
```

## Comparing `funfluid-202307021904.tar` & `funfluid-202307021923.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307021904/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 11:04:56.727875 funfluid-202307021904/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202307021904/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.711874 funfluid-202307021904/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307021904/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.719874 funfluid-202307021904/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.719874 funfluid-202307021904/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.719874 funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.719874 funfluid-202307021904/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.719874 funfluid-202307021904/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307021904/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307021904/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/simulate/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307021904/funfluid/simulate/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/simulate/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/simulate/ellipse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307021904/funfluid/simulate/ellipse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/simulate/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/simulate/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307021904/funfluid/simulate/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/simulate/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/simulate/ellipse/project/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.723875 funfluid-202307021904/funfluid/simulate/ellipse/project/models/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/models/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/models/flow.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:57.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/project.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/simulate/ellipse/project/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:36:34.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6457 2023-07-02 11:04:34.000000 funfluid-202307021904/funfluid/simulate/ellipse/project/track/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/simulate/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/simulate/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/simulate/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307021904/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.727875 funfluid-202307021904/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021904/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307021904/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307021904/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:04:56.715874 funfluid-202307021904/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 11:04:56.000000 funfluid-202307021904/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2625 2023-07-02 11:04:56.000000 funfluid-202307021904/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-02 11:04:56.000000 funfluid-202307021904/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-07-02 11:04:56.000000 funfluid-202307021904/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-02 11:04:56.000000 funfluid-202307021904/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-02 11:04:56.727875 funfluid-202307021904/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202307021904/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.547033 funfluid-202307021923/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307021923/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 11:23:07.547033 funfluid-202307021923/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202307021923/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.487032 funfluid-202307021923/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.495032 funfluid-202307021923/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.495032 funfluid-202307021923/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307021923/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.495032 funfluid-202307021923/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.495032 funfluid-202307021923/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.499032 funfluid-202307021923/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.499032 funfluid-202307021923/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.503032 funfluid-202307021923/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.507032 funfluid-202307021923/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.511032 funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.515032 funfluid-202307021923/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.515032 funfluid-202307021923/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307021923/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.519033 funfluid-202307021923/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.523033 funfluid-202307021923/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307021923/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.527033 funfluid-202307021923/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.527033 funfluid-202307021923/funfluid/simulate/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307021923/funfluid/simulate/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.531033 funfluid-202307021923/funfluid/simulate/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/simulate/ellipse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307021923/funfluid/simulate/ellipse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.531033 funfluid-202307021923/funfluid/simulate/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/simulate/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307021923/funfluid/simulate/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/simulate/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.531033 funfluid-202307021923/funfluid/simulate/ellipse/project/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.535033 funfluid-202307021923/funfluid/simulate/ellipse/project/models/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/models/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/models/flow.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:36:57.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/project.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.535033 funfluid-202307021923/funfluid/simulate/ellipse/project/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:36:34.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6648 2023-07-02 11:23:05.000000 funfluid-202307021923/funfluid/simulate/ellipse/project/track/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.539033 funfluid-202307021923/funfluid/simulate/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/simulate/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/simulate/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.539033 funfluid-202307021923/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.539033 funfluid-202307021923/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307021923/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.543033 funfluid-202307021923/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.543033 funfluid-202307021923/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.547033 funfluid-202307021923/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307021923/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307021923/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307021923/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:23:07.491032 funfluid-202307021923/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 11:23:07.000000 funfluid-202307021923/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2625 2023-07-02 11:23:07.000000 funfluid-202307021923/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-02 11:23:07.000000 funfluid-202307021923/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       12 2023-07-02 11:23:07.000000 funfluid-202307021923/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-02 11:23:07.000000 funfluid-202307021923/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-02 11:23:07.547033 funfluid-202307021923/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      399 2023-06-30 08:49:30.000000 funfluid-202307021923/setup.py
```

### Comparing `funfluid-202307021904/LICENSE` & `funfluid-202307021923/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/common/base/cache.py` & `funfluid-202307021923/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202307021923/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/core/buff.py` & `funfluid-202307021923/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/core/lattice.py` & `funfluid-202307021923/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/core/shape.py` & `funfluid-202307021923/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/core/speed_nb.py` & `funfluid-202307021923/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/example/example_cavity1.py` & `funfluid-202307021923/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/example/example_cavity3.py` & `funfluid-202307021923/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/example/example_obstacle.py` & `funfluid-202307021923/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202307021923/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/example/example_turek.py` & `funfluid-202307021923/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/obs_array.py` & `funfluid-202307021923/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/lbm/params.py` & `funfluid-202307021923/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/simulate/ellipse/example/largs_plot_example.py` & `funfluid-202307021923/funfluid/simulate/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/simulate/ellipse/plot.py` & `funfluid-202307021923/funfluid/simulate/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/simulate/ellipse/project/track/plot.py` & `funfluid-202307021923/funfluid/simulate/ellipse/project/track/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import math
+from functools import partial
 from typing import List
 
 import matplotlib.animation as animation
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
@@ -37,15 +38,15 @@
         ax.set_ylim(self.y_start, self.y_start + self.height)
         ax.set_aspect(1)
 
 
 class EllipseTrack:
     def __init__(self, df, a=10, b=5, color=None, marker=None, *args, **kwargs):
         if isinstance(df, str):
-            self.df = _load(path=df)
+            self.df = _load(df)
         else:
             self.df = df
 
         self.a = a
         self.b = b
         self.color = color
         self.marker = marker
@@ -172,21 +173,22 @@
         self.ellipses.append(ellipse)
 
     def plot_ref(self, ax):
         self.flow.figure(ax)
         for ellipse in self.ellipses:
             self.lns.extend(ellipse.plot_ref())
 
-    def plot_update(self, step=10):
+    def plot_update(self, step=10, title='', *args, **kwargs):
         for ellipse in self.ellipses:
             ellipse.plot_update(step=step)
-        self.lns[-1].set_text(f'step={step}')
+        # self.lns[-1].set_text(f'step={step}')
+        self.lns[-1].set_text(title.replace("{step}", str(step)))
         return self.lns
 
-    def plot(self, min_step=2, max_step=None, step=10, gif_path='./trak.gif'):
+    def plot(self, min_step=2, max_step=None, step=10, title='', gif_path='./trak.gif'):
         max_step = max_step or self.max_step
 
         fig, ax = plt.subplots()
 
         plt.grid(ls='--')
         plt.xlabel(r'$x/L$')
         plt.ylabel(r'$y/L$')
@@ -194,19 +196,19 @@
         ax.set_ylim(0, 1200)
         ax.set_aspect(1)
         plt.tick_params(labelsize=11)
         labels = ax.get_xticklabels() + ax.get_yticklabels()
         [label.set_fontname('Times New Roman') for label in labels]
 
         self.plot_ref(ax)
-        print(self.lns)
         self.lns.append(plt.title('', fontsize=12))
+
         ani = animation.FuncAnimation(fig=fig,
-                                      func=self.plot_update,
+                                      # func=self.plot_update,
+                                      func=partial(self.plot_update, title=title),
                                       frames=[i for i in range(min_step, max_step, step)],
                                       interval=100,
                                       blit=False,
                                       repeat=False
                                       )
-
         plt.show()
         ani.save(gif_path, writer='imagemagick')
```

### Comparing `funfluid-202307021904/funfluid/simulate/ellipse/utils/largs_plot.py` & `funfluid-202307021923/funfluid/simulate/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/tecplot/templates/templates1.py` & `funfluid-202307021923/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/temp/data_fit.py` & `funfluid-202307021923/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid/utils/timer.py` & `funfluid-202307021923/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307021904/funfluid.egg-info/SOURCES.txt` & `funfluid-202307021923/funfluid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

