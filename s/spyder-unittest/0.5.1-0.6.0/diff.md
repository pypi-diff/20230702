# Comparing `tmp/spyder_unittest-0.5.1.tar.gz` & `tmp/spyder_unittest-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_unittest-0.5.1.tar", last modified: Sat Sep  3 20:30:03 2022, max compression
+gzip compressed data, was "spyder_unittest-0.6.0.tar", last modified: Sun Jul  2 14:57:15 2023, max compression
```

## Comparing `spyder_unittest-0.5.1.tar` & `spyder_unittest-0.6.0.tar`

### file list

```diff
@@ -1,88 +1,93 @@
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      311 2018-06-06 18:45:39.000000 spyder_unittest-0.5.1/AUTHORS
--rw-r--r--   0 jitse     (1000) jitse     (1000)    17850 2022-09-03 20:28:01.000000 spyder_unittest-0.5.1/CHANGELOG.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1093 2017-02-11 17:35:04.000000 spyder_unittest-0.5.1/LICENSE.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)      144 2022-01-20 09:27:13.000000 spyder_unittest-0.5.1/MANIFEST.in
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1079 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/PKG-INFO
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5762 2022-01-18 15:35:18.000000 spyder_unittest-0.5.1/README.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)       71 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/setup.cfg
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2684 2022-07-02 21:35:20.000000 spyder_unittest-0.5.1/setup.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.793950 spyder_unittest-0.5.1/spyder_unittest/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      293 2022-09-03 20:29:10.000000 spyder_unittest-0.5.1/spyder_unittest/__init__.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.793950 spyder_unittest-0.5.1/spyder_unittest/backend/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      220 2017-02-11 17:35:04.000000 spyder_unittest-0.5.1/spyder_unittest/backend/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2997 2022-01-18 15:35:18.000000 spyder_unittest-0.5.1/spyder_unittest/backend/abbreviator.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2069 2018-01-07 17:11:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/frameworkregistry.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3239 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/noserunner.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7121 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/pytestrunner.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7363 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/runnerbase.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/backend/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      194 2017-04-14 14:36:00.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2495 2022-01-18 15:35:18.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_abbreviator.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      829 2018-01-07 17:11:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_frameworkregistry.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3127 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_noserunner.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    12263 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_pytestrunner.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3235 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_runnerbase.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5221 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_unittestrunner.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      592 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_zmqstream.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5107 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/unittestrunner.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/backend/workers/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      539 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2535 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/print_versions.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5446 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/pytestworker.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/backend/workers/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2777 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/tests/test_print_versions.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    11052 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/tests/test_pytestworker.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1486 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/workers/zmqwriter.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2770 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/backend/zmqreader.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.785950 spyder_unittest-0.5.1/spyder_unittest/locale/de/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/de/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2519 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/de/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.785950 spyder_unittest-0.5.1/spyder_unittest/locale/es/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/es/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      558 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/es/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.785950 spyder_unittest-0.5.1/spyder_unittest/locale/fr/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2382 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/fr/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.785950 spyder_unittest-0.5.1/spyder_unittest/locale/hr/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/hr/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      630 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/hr/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/hu/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/hu/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      557 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/hu/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/ja/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/ja/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      549 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/ja/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/pl/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      700 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/pl/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/pt_BR/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2337 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/pt_BR/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/ru/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.797950 spyder_unittest-0.5.1/spyder_unittest/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      720 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/ru/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.789950 spyder_unittest-0.5.1/spyder_unittest/locale/zh_CN/
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/spyder_unittest/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      562 2022-09-03 20:17:37.000000 spyder_unittest-0.5.1/spyder_unittest/locale/zh_CN/LC_MESSAGES/spyder_unittest.mo
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/spyder_unittest/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4983 2022-07-24 12:46:05.000000 spyder_unittest-0.5.1/spyder_unittest/tests/test_unittestplugin.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10262 2022-08-10 16:42:52.000000 spyder_unittest-0.5.1/spyder_unittest/unittestplugin.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/spyder_unittest/widgets/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      187 2017-02-11 17:35:04.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     7116 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/configdialog.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    16307 2022-07-29 20:34:29.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/datatree.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.801950 spyder_unittest-0.5.1/spyder_unittest/widgets/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      194 2017-04-14 14:36:00.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/tests/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4675 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_configdialog.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    10164 2022-07-24 12:46:05.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_datatree.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    12624 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_unittestgui.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    18515 2022-08-29 16:00:19.000000 spyder_unittest-0.5.1/spyder_unittest/widgets/unittestgui.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-09-03 20:30:03.793950 spyder_unittest-0.5.1/spyder_unittest.egg-info/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1079 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/PKG-INFO
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2353 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/SOURCES.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/dependency_links.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       75 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/entry_points.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       28 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/requires.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       16 2022-09-03 20:30:03.000000 spyder_unittest-0.5.1/spyder_unittest.egg-info/top_level.txt
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.328519 spyder_unittest-0.6.0/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      311 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/AUTHORS
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    20748 2023-07-02 14:51:58.000000 spyder_unittest-0.6.0/CHANGELOG.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1093 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/LICENSE.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      144 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/MANIFEST.in
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1060 2023-07-02 14:57:15.328519 spyder_unittest-0.6.0/PKG-INFO
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5600 2023-05-26 19:42:30.000000 spyder_unittest-0.6.0/README.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       71 2023-07-02 14:57:15.328519 spyder_unittest-0.6.0/setup.cfg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2685 2023-07-02 12:49:34.000000 spyder_unittest-0.6.0/setup.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      294 2023-07-02 14:55:05.000000 spyder_unittest-0.6.0/spyder_unittest/__init__.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/backend/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      220 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/backend/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3501 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/abbreviator.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2423 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/frameworkregistry.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3769 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/nose2runner.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     9171 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/pytestrunner.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8244 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/runnerbase.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/backend/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      194 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2495 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_abbreviator.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      829 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_frameworkregistry.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1416 2023-04-25 08:39:52.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_nose2runner.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13334 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_pytestrunner.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3252 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_runnerbase.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6497 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_unittestrunner.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      592 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_zmqstream.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3598 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/unittestrunner.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/backend/workers/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      540 2023-04-25 08:39:52.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2365 2023-04-25 08:39:52.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/print_versions.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4919 2023-06-15 20:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/pytestworker.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1900 2023-04-25 08:39:52.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/test_print_versions.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11854 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/test_pytestworker.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6934 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/test_unittestworker.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4428 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/unittestworker.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1980 2023-04-25 08:39:52.000000 spyder_unittest-0.6.0/spyder_unittest/backend/workers/zmqwriter.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2794 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/backend/zmqreader.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/de/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3423 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/de/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/es/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      558 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/es/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/fr/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2386 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/fr/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/hr/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      630 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/hr/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/hu/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      557 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/hu/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/ja/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      549 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/ja/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/pl/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      700 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/pl/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/pt_BR/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2341 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/pt_BR/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/ru/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      720 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/ru/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.320519 spyder_unittest-0.6.0/spyder_unittest/locale/zh_CN/
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      562 2023-07-02 12:46:42.000000 spyder_unittest-0.6.0/spyder_unittest/locale/zh_CN/LC_MESSAGES/spyder_unittest.mo
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1315 2023-07-02 12:49:34.000000 spyder_unittest-0.6.0/spyder_unittest/tests/conftest.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5399 2023-07-02 12:49:34.000000 spyder_unittest-0.6.0/spyder_unittest/tests/test_unittestplugin.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    13054 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/unittestplugin.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest/widgets/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      187 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     8529 2023-05-26 19:42:30.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/configdialog.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1155 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/confpage.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    16958 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/datatree.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.328519 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      194 2022-12-17 18:45:31.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     5055 2023-05-26 19:42:30.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_configdialog.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     6188 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_confpage.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    11180 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_datatree.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    14743 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_unittestgui.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    18867 2023-06-23 15:39:21.000000 spyder_unittest-0.6.0/spyder_unittest/widgets/unittestgui.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-07-02 14:57:15.324519 spyder_unittest-0.6.0/spyder_unittest.egg-info/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1060 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/PKG-INFO
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2583 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/SOURCES.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/dependency_links.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       74 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/entry_points.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       28 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/requires.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       16 2023-07-02 14:57:15.000000 spyder_unittest-0.6.0/spyder_unittest.egg-info/top_level.txt
```

### Comparing `spyder_unittest-0.5.1/CHANGELOG.md` & `spyder_unittest-0.6.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,33 @@
 # History of changes
 
+## Version 0.6.0 (2023-07-02)
+
+### New Features
+
+* Support nose2 and drop support for nose ([Issue 178](https://github.com/spyder-ide/spyder-unittest/issues/178), [PR 200](https://github.com/spyder-ide/spyder-unittest/pull/200))
+* New menu item for running only a single test ([Issue 88](https://github.com/spyder-ide/spyder-unittest/issues/88), [PR 211](https://github.com/spyder-ide/spyder-unittest/pull/211))
+* New configuration option for adding extra command-line arguments when running tests ([Issue 199](https://github.com/spyder-ide/spyder-unittest/issues/199), [PR 204](https://github.com/spyder-ide/spyder-unittest/pull/204))
+* New configuration option to disable or enable abbreviating the test name ([Issue 122](https://github.com/spyder-ide/spyder-unittest/issues/122), [PR 208](https://github.com/spyder-ide/spyder-unittest/pull/208))
+
+### Bug Fixes
+
+* Execute `unittest` tests programmatically for robustness ([Issue 73](https://github.com/spyder-ide/spyder-unittest/issues/73), [Issue 76](https://github.com/spyder-ide/spyder-unittest/issues/76), [Issue 160](https://github.com/spyder-ide/spyder-unittest/issues/160), [PR 202](https://github.com/spyder-ide/spyder-unittest/pull/202))
+* Support changed format of `unittest` output in Python 3.11 ([Issue 193](https://github.com/spyder-ide/spyder-unittest/issues/193), [PR 190](https://github.com/spyder-ide/spyder-unittest/pull/190), [PR 194](https://github.com/spyder-ide/spyder-unittest/pull/194), by [@juliangilbey](https://github.com/juliangilbey))
+* Fix keyboard shortcut for running tests ([Issue 172](https://github.com/spyder-ide/spyder-unittest/issues/172), [PR 203](https://github.com/spyder-ide/spyder-unittest/pull/203))
+* Use colours from Spyder's standard palette to get a uniform UI ([Issue 186](https://github.com/spyder-ide/spyder-unittest/issues/186), [PR 187](https://github.com/spyder-ide/spyder-unittest/pull/187))
+
+### Maintenance
+
+* Keep plugin up-to-date with latest changes in Spyder 5 ([Issue 195](https://github.com/spyder-ide/spyder-unittest/issues/195), [Issue 206](https://github.com/spyder-ide/spyder-unittest/issues/206), [Issue 209](https://github.com/spyder-ide/spyder-unittest/issues/209), [PR 197](https://github.com/spyder-ide/spyder-unittest/pull/197), [PR 207](https://github.com/spyder-ide/spyder-unittest/pull/207), [PR 214](https://github.com/spyder-ide/spyder-unittest/pull/214))
+* Update translations ([PR 212](https://github.com/spyder-ide/spyder-unittest/pull/212))
+* Fix integration tests for the plugin ([Issue 167](https://github.com/spyder-ide/spyder-unittest/issues/167), [PR 197](https://github.com/spyder-ide/spyder-unittest/pull/197))
+* Update GitHub workflow for running tests ([PR 192](https://github.com/spyder-ide/spyder-unittest/pull/192), [PR 196](https://github.com/spyder-ide/spyder-unittest/pull/196), [PR 201](https://github.com/spyder-ide/spyder-unittest/pull/201))
+
+
 ## Version 0.5.1 (2022/09/03)
 
 ### New Features
 
 * Tests are executed using the Python interpreter set in Preferences (instead of the interpreter that Spyder runs under), by [@stevetracvc](https://github.com/stevetracvc) ([Issue 65](https://github.com/spyder-ide/spyder-unittest/issues/65), [PR 174](https://github.com/spyder-ide/spyder-unittest/pull/174))
 * You can display test coverage, though only for pytest; by [@stevetracvc](https://github.com/stevetracvc) ([Issue 33](https://github.com/spyder-ide/spyder-unittest/issues/33), [PR 175](https://github.com/spyder-ide/spyder-unittest/pull/175))
```

### Comparing `spyder_unittest-0.5.1/LICENSE.txt` & `spyder_unittest-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyder_unittest-0.5.1/PKG-INFO` & `spyder_unittest-0.6.0/spyder_unittest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
-Name: spyder_unittest
-Version: 0.5.1
+Name: spyder-unittest
+Version: 0.6.0
 Summary: Plugin to run tests from within the Spyder IDE
 Home-page: https://github.com/spyder-ide/spyder-unittest
 Author: Spyder Project Contributors
 License: MIT
 Keywords: Qt PyQt4 PyQt5 spyder plugins testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 
 This is a plugin for the Spyder IDE that integrates popular unit test
 frameworks. It allows you to run tests and view the results.
 
 The plugin supports the `unittest` framework in the Python
-standard library and the `pytest` and `nose` testing frameworks.
-
-
+standard library and the `pytest` and `nose2` testing frameworks.
```

### Comparing `spyder_unittest-0.5.1/README.md` & `spyder_unittest-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 [![OpenCollective Backers](https://opencollective.com/spyder/backers/badge.svg?color=blue)](#backers)
 [![OpenCollective Sponsors](https://opencollective.com/spyder/sponsors/badge.svg?color=blue)](#sponsors)
 
 ## Build status
 [![Windows status](https://github.com/spyder-ide/spyder-unittest/workflows/Windows%20tests/badge.svg)](https://github.com/spyder-ide/spyder-notebook/actions?query=workflow%3A%22Windows+tests%22)
 [![Linux status](https://github.com/spyder-ide/spyder-unittest/workflows/Linux%20tests/badge.svg)](https://github.com/spyder-ide/spyder-notebook/actions?query=workflow%3A%22Linux+tests%22)
 [![MacOS status](https://github.com/spyder-ide/spyder-unittest/workflows/Macos%20tests/badge.svg)](https://github.com/spyder-ide/spyder-notebook/actions?query=workflow%3A%22Macos+tests%22)
-[![codecov](https://codecov.io/gh/spyder-ide/spyder-unittest/branch/master/graph/badge.svg)](https://codecov.io/gh/spyder-ide/spyder-notebook/branch/master)
 [![Crowdin](https://badges.crowdin.net/spyder-unittest/localized.svg)](https://crowdin.com/project/spyder-unittest)
 
 *Copyright © 2014 Spyder Project Contributors*
 
-![Screenshot of spyder-unittest plugin showing test results](./screenshot.png)
+![Screenshot of spyder-unittest plugin showing test results](./doc/screenshot.png)
 
 ## Description
 
 Spyder-unittest is a plugin that integrates popular unit test frameworks
 with Spyder, allowing you to run test suites and view the results in the IDE.
 
 The plugin supports the `unittest` module in the Python standard library
-as well as the `pytest` and `nose` testing frameworks.
+as well as the `pytest` and `nose2` testing frameworks.
 Support for `pytest` is most complete at the moment.
 
 
 ## Installation
 
 The unittest plugin is available in the `spyder-ide` channel in Anaconda and in PyPI,
 so it can be installed with the following commands:
@@ -72,18 +71,18 @@
 and running `pip install .`, possibly with the `--editable` flag.
 
 The plugin has the following dependencies:
 
 * [spyder](https://github.com/spyder-ide/spyder) (obviously), at least version 4.0
 * [lxml](http://lxml.de/)
 * the testing framework that you will be using: [pytest](https://pytest.org)
-  and/or [nose](https://nose.readthedocs.io)
+  and/or [nose2](https://docs.nose2.io)
 
 In order to run the tests distributed with this plugin, you need
-[nose](https://nose.readthedocs.io), [pytest](https://pytest.org)
+[nose2](https://docs.nose2.io), [pytest](https://pytest.org)
 and [pytest-qt](https://github.com/pytest-dev/pytest-qt). If you use Python 2,
 you also need [mock](https://github.com/testing-cabal/mock).
 
 You are very welcome to submit code contributions in the form of pull
 requests to the
 [issue tracker](https://github.com/spyder-ide/spyder-unittest/issues).
 GitHub is configured to run pull requests automatically against the test suite
```

### Comparing `spyder_unittest-0.5.1/setup.py` & `spyder_unittest-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,34 +33,34 @@
         for fname in filenames:
             if not fname.startswith('.') and osp.splitext(fname)[1] in extlist:
                 flist.append(osp.join(dirpath, fname)[offset:])
     return flist
 
 
 # Requirements
-REQUIREMENTS = ['lxml', 'spyder>=5.3.1,<6', 'pyzmq']
+REQUIREMENTS = ['lxml', 'spyder>=5.4.1,<6', 'pyzmq']
 EXTLIST = ['.jpg', '.png', '.json', '.mo', '.ini']
 LIBNAME = 'spyder_unittest'
 
 
 LONG_DESCRIPTION = """
 This is a plugin for the Spyder IDE that integrates popular unit test
 frameworks. It allows you to run tests and view the results.
 
 The plugin supports the `unittest` framework in the Python
-standard library and the `pytest` and `nose` testing frameworks.
+standard library and the `pytest` and `nose2` testing frameworks.
 """
 
 setup(
     name=LIBNAME,
     version=get_version(),
     packages=find_packages(),
     package_data={LIBNAME: get_package_data(LIBNAME, EXTLIST)},
     keywords=["Qt PyQt4 PyQt5 spyder plugins testing"],
-    python_requires='>=3.5',
+    python_requires='>=3.7',
     install_requires=REQUIREMENTS,
     url='https://github.com/spyder-ide/spyder-unittest',
     license='MIT',
     author="Spyder Project Contributors",
     description='Plugin to run tests from within the Spyder IDE',
     long_description=LONG_DESCRIPTION,
     classifiers=[
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/abbreviator.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/abbreviator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © 2017 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Class for abbreviating test names."""
 
+from __future__ import annotations
+
+# Standard imports
+from dataclasses import dataclass
+
+@dataclass
+class Abbreviation:
+    """
+    Abbreviation for one component of a test name.
+
+    Abbreviations are defined recursively, so `.head` is the abbreviation
+    for the first component and `.tail` specifies the abbreviations for the
+    second and later components.
+    """
+    head: str
+    tail: Abbreviator
+
 
 class Abbreviator:
     """
     Abbreviates names so that abbreviation identifies name uniquely.
 
     First, if the name contains brackets, the part in brackets starting at
     the first bracket is removed from the name. Then, all names are split
@@ -22,28 +39,28 @@
     ----------
     dic : dict of (str, [str, Abbreviator])
         keys are the first-level components, values are a list, with the
         abbreviation as its first element and an Abbreviator for abbreviating
         the higher-level components as its second element.
     """
 
-    def __init__(self, names=[]):
+    def __init__(self, names: list[str]=[]) -> None:
         """
         Constructor.
 
         Arguments
         ---------
         names : list of str
             list of words which needs to be abbreviated.
         """
-        self.dic = {}
+        self.dic: dict[str, Abbreviation] = {}
         for name in names:
             self.add(name)
 
-    def add(self, name):
+    def add(self, name: str) -> None:
         """
         Add name to list of names to be abbreviated.
 
         Arguments
         ---------
         name : str
         """
@@ -57,32 +74,32 @@
                 if start == other:
                     break
                 while (start[:len_abbrev] == other[:len_abbrev]
                        and len_abbrev < len(start)
                        and len_abbrev < len(other)):
                     len_abbrev += 1
                 if len_abbrev == len(start):
-                    self.dic[other][0] = other[:len_abbrev + 1]
+                    self.dic[other].head = other[:len_abbrev + 1]
                 elif len_abbrev == len(other):
-                    self.dic[other][0] = other
+                    self.dic[other].head = other
                     len_abbrev += 1
                 else:
-                    if len(self.dic[other][0]) < len_abbrev:
-                        self.dic[other][0] = other[:len_abbrev]
+                    if len(self.dic[other].head) < len_abbrev:
+                        self.dic[other].head = other[:len_abbrev]
         else:
-            self.dic[start] = [start[:len_abbrev], Abbreviator()]
-        self.dic[start][1].add(rest)
+            self.dic[start] = Abbreviation(start[:len_abbrev], Abbreviator())
+        self.dic[start].tail.add(rest)
 
-    def abbreviate(self, name):
+    def abbreviate(self, name: str) -> str:
         """Return abbreviation of name."""
         if '[' in name:
             name, parameters = name.split('[', 1)
             parameters = '[' + parameters
         else:
             parameters = ''
         if '.' in name:
             start, rest = name.split('.', 1)
-            res = (self.dic[start][0]
-                   + '.' + self.dic[start][1].abbreviate(rest))
+            res = (self.dic[start].head
+                   + '.' + self.dic[start].tail.abbreviate(rest))
         else:
             res = name
         return res + parameters
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/frameworkregistry.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/frameworkregistry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © 2017 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Keep track of testing frameworks and create test runners when requested."""
 
+from __future__ import annotations
+
+# Standard imports
+from typing import Optional, TYPE_CHECKING
+
+# Local imports
+if TYPE_CHECKING:
+    from spyder_unittest.backend.runnerbase import RunnerBase
+    from spyder_unittest.widgets.unittestgui import UnitTestWidget
+
 
 class FrameworkRegistry():
     """
     Registry of testing frameworks and their associated runners.
 
     The test runner for a framework is responsible for running the tests and
     parsing the results. It should implement the interface of RunnerBase.
@@ -20,41 +30,42 @@
     Attributes
     ----------
     frameworks : dict of (str, type)
         Dictionary mapping names of testing frameworks to the types of the
         associated runners.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize self."""
-        self.frameworks = {}
+        self.frameworks: dict[str, type[RunnerBase]] = {}
 
-    def register(self, runner_class):
+    def register(self, runner_class: type[RunnerBase]) -> None:
         """Register runner class for a testing framework.
 
         Parameters
         ----------
-        runner_class : type
+        runner_class
             Class used for creating tests runners for the framework.
         """
         self.frameworks[runner_class.name] = runner_class
 
-    def create_runner(self, framework, widget, tempfilename):
+    def create_runner(self, framework: str, widget: UnitTestWidget,
+                      tempfilename: Optional[str]) -> RunnerBase:
         """Create test runner associated to some testing framework.
 
         This creates an instance of the runner class whose `name` attribute
         equals `framework`.
 
         Parameters
         ----------
-        framework : str
+        framework
             Name of testing framework.
-        widget : UnitTestWidget
+        widget
             Unit test widget which constructs the test runner.
-        resultfilename : str or None
+        resultfilename
             Name of file in which to store test results. If None, use default.
 
         Returns
         -------
         RunnerBase
             Newly created test runner
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/noserunner.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/nose2runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © 2013 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Support for Nose framework."""
 
+from __future__ import annotations
+
+# Standard library imports
+from typing import Optional, TYPE_CHECKING
+
 # Third party imports
 from lxml import etree
 from spyder.config.base import get_translation
 
 # Local imports
 from spyder_unittest.backend.runnerbase import Category, RunnerBase, TestResult
+if TYPE_CHECKING:
+    from spyder_unittest.widgets.configdialog import Config
 
 try:
     _ = get_translation('spyder_unittest')
 except KeyError:
     import gettext
     _ = gettext.gettext
 
 
-class NoseRunner(RunnerBase):
+class Nose2Runner(RunnerBase):
     """Class for running tests within Nose framework."""
 
-    module = 'nose'
-    name = 'nose'
+    module = 'nose2'
+    name = 'nose2'
 
-    def create_argument_list(self, config, cov_path):
+    def create_argument_list(self, config: Config,
+                             cov_path: Optional[str],
+                             single_test: Optional[str]) -> list[str]:
         """Create argument list for testing process."""
-        return [
-            '-m', self.module, '--with-xunit',
-            '--xunit-file={}'.format(self.resultfilename),
-            ]
+        arguments = [
+            '-m', self.module, '--plugin=nose2.plugins.junitxml',
+            '--junit-xml', '--junit-xml-path={}'.format(self.resultfilename)
+        ]
+        if single_test:
+            arguments.append(single_test)
+        arguments += config.args
+        return arguments
 
-    def finished(self):
+    def finished(self, exitcode: int) -> None:
         """Called when the unit test process has finished."""
         output = self.read_all_process_output()
         testresults = self.load_data()
         self.sig_finished.emit(testresults, output, True)
 
-    def load_data(self):
+    def load_data(self) -> list[TestResult]:
         """
         Read and parse unit test results.
 
         This function reads the unit test results from the file with name
         `self.resultfilename` and parses them. The file should contain the
         test results in JUnitXML format.
 
@@ -50,15 +63,15 @@
         -------
         list of TestResult
             Unit test results.
         """
         try:
             data = etree.parse(self.resultfilename).getroot()
         except OSError:
-            data = []
+            return []
 
         testresults = []
         for testcase in data:
             category = Category.OK
             status = 'ok'
             name = '{}.{}'.format(testcase.get('classname'),
                                   testcase.get('name'))
@@ -77,15 +90,15 @@
                     message = child.get('message', default='')
                     if type_ and message:
                         message = '{0}: {1}'.format(type_, message)
                     elif type_:
                         message = type_
                     if child.text:
                         extras.append(child.text)
-                elif child.tag in ('system-out', 'system-err'):
+                elif child.tag in ('system-out', 'system-err') and child.text:
                     if child.tag == 'system-out':
                         heading = _('Captured stdout')
                     else:
                         heading = _('Captured stderr')
                     contents = child.text.rstrip('\n')
                     extras.append('----- {} -----\n{}'.format(heading,
                                                               contents))
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/pytestrunner.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/pytestrunner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,105 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © 2013 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Support for pytest framework."""
 
+from __future__ import annotations
+
 # Standard library imports
 import os
 import os.path as osp
 import re
+from typing import Any, Optional, TYPE_CHECKING
 
 # Local imports
 from spyder.config.base import get_translation
 from spyder_unittest.backend.runnerbase import (Category, RunnerBase,
                                                 TestResult, COV_TEST_NAME)
 from spyder_unittest.backend.zmqreader import ZmqStreamReader
+if TYPE_CHECKING:
+    from spyder_unittest.widgets.configdialog import Config
 
 try:
     _ = get_translation('spyder_unittest')
 except KeyError:
     import gettext
     _ = gettext.gettext
 
 
 class PyTestRunner(RunnerBase):
     """Class for running tests within pytest framework."""
 
     module = 'pytest'
     name = 'pytest'
 
-    def create_argument_list(self, config, cov_path):
+    def create_argument_list(self, config: Config,
+                             cov_path: Optional[str],
+                             single_test: Optional[str]) -> list[str]:
         """Create argument list for testing process."""
         dirname = os.path.dirname(__file__)
         pyfile = os.path.join(dirname, 'workers', 'pytestworker.py')
         arguments = [pyfile, str(self.reader.port)]
         if config.coverage:
             arguments += [f'--cov={cov_path}', '--cov-report=term-missing']
+        if single_test:
+            arguments.append(self.convert_testname_to_nodeid(single_test))
+        arguments += config.args
         return arguments
 
-
-    def start(self, config, cov_path, executable, pythonpath):
+    def start(self, config: Config, cov_path: Optional[str],
+              executable: str, pythonpath: list[str],
+              single_test: Optional[str]) -> None:
         """Start process which will run the unit test suite."""
         self.config = config
         self.reader = ZmqStreamReader()
         self.reader.sig_received.connect(self.process_output)
-        RunnerBase.start(self, config, cov_path, executable, pythonpath)
+        super().start(config, cov_path, executable, pythonpath, single_test)
 
-    def process_output(self, output):
+    def process_output(self, output: list[dict[str, Any]]) -> None:
         """
         Process output of test process.
 
         Parameters
         ----------
-        output : list
+        output
             list of decoded Python object sent by test process.
         """
         collected_list = []
         collecterror_list = []
         starttest_list = []
         result_list = []
         for result_item in output:
             if result_item['event'] == 'config':
                 self.rootdir = result_item['rootdir']
             elif result_item['event'] == 'collected':
-                testname = convert_nodeid_to_testname(result_item['nodeid'])
-                collected_list.append(testname)
+                name = self.convert_nodeid_to_testname(result_item['nodeid'])
+                collected_list.append(name)
             elif result_item['event'] == 'collecterror':
-                tupl = logreport_collecterror_to_tuple(result_item)
+                tupl = self.logreport_collecterror_to_tuple(result_item)
                 collecterror_list.append(tupl)
             elif result_item['event'] == 'starttest':
-                starttest_list.append(logreport_starttest_to_str(result_item))
+                name = self.logreport_starttest_to_str(result_item)
+                starttest_list.append(name)
             elif result_item['event'] == 'logreport':
-                testresult = logreport_to_testresult(result_item, self.rootdir)
+                testresult = self.logreport_to_testresult(result_item)
                 result_list.append(testresult)
 
         if collected_list:
             self.sig_collected.emit(collected_list)
         if collecterror_list:
             self.sig_collecterror.emit(collecterror_list)
         if starttest_list:
             self.sig_starttest.emit(starttest_list)
         if result_list:
             self.sig_testresult.emit(result_list)
 
-    def process_coverage(self, output):
+    def process_coverage(self, output: str) -> None:
         """Search the output text for coverage details.
 
         Called by the function 'finished' at the very end.
         """
         cov_results = re.search(
             r'-*? coverage:.*?-*\nTOTAL\s.*?\s(\d*?)\%.*\n=*',
             output, flags=re.S)
@@ -103,90 +115,115 @@
             # also build a result for each file's coverage
             header = "".join(cov_results.group(0).split("\n")[1:3])
             # coverage report columns:
             # Name  Stmts   Miss  Cover   Missing
             for row in re.findall(
                     r'^((.*?\.py) .*?(\d+%).*?(\d[\d\,\-\ ]*)?)$',
                     cov_results.group(0), flags=re.M):
-                lineno = (int(re.search(r'^(\d*)', row[3]).group(1)) - 1
-                          if row[3] else None)
+                lineno: Optional[int] = None
+                if row[3]:
+                    match = re.search(r'^(\d*)', row[3])
+                    if match:
+                        lineno = int(match.group(1)) - 1
                 file_cov = TestResult(
                     Category.COVERAGE, row[2], row[1],
                     message=_('Missing: {}').format(row[3] if row[3] else _("(none)")),
                     extra_text=_('{}\n{}').format(header, row[0]), filename=row[1],
                     lineno=lineno)
                 self.sig_collected.emit([row[1]])
                 self.sig_testresult.emit([file_cov])
 
-    def finished(self, exitcode):
+    def finished(self, exitcode: int) -> None:
         """
         Called when the unit test process has finished.
 
         This function emits `sig_finished`.
 
         Parameters
         ----------
-        exitcode : int
+        exitcode
             Exit code of the test process.
         """
         self.reader.close()
         output = self.read_all_process_output()
         if self.config.coverage:
             self.process_coverage(output)
         normal_exit = exitcode in [0, 1, 2, 5]
         # Meaning of exit codes: 0 = all tests passed, 1 = test failed,
         # 2 = interrupted, 5 = no tests collected
         self.sig_finished.emit([], output, normal_exit)
 
+    def normalize_module_name(self, name: str) -> str:
+        """
+        Convert module name reported by pytest to Python conventions.
 
-def normalize_module_name(name):
-    """
-    Convert module name reported by pytest to Python conventions.
-
-    This function strips the .py suffix and replaces '/' by '.', so that
-    'ham/spam.py' becomes 'ham.spam'.
-    """
-    if name.endswith('.py'):
-        name = name[:-3]
-    return name.replace('/', '.')
-
-
-def convert_nodeid_to_testname(nodeid):
-    """Convert a nodeid to a test name."""
-    module, name = nodeid.split('::', 1)
-    module = normalize_module_name(module)
-    return '{}.{}'.format(module, name)
-
-
-def logreport_collecterror_to_tuple(report):
-    """Convert a 'collecterror' logreport to a (str, str) tuple."""
-    module = normalize_module_name(report['nodeid'])
-    return (module, report['longrepr'])
-
-
-def logreport_starttest_to_str(report):
-    """Convert a 'starttest' logreport to a str."""
-    return convert_nodeid_to_testname(report['nodeid'])
-
-
-def logreport_to_testresult(report, rootdir):
-    """Convert a logreport sent by test process to a TestResult."""
-    status = report['outcome']
-    if report['outcome'] in ('failed', 'xpassed') or report['witherror']:
-        cat = Category.FAIL
-    elif report['outcome'] in ('passed', 'xfailed'):
-        cat = Category.OK
-    else:
-        cat = Category.SKIP
-    testname = convert_nodeid_to_testname(report['nodeid'])
-    message = report.get('message', '')
-    extra_text = report.get('longrepr', '')
-    if 'sections' in report:
-        if extra_text:
-            extra_text +=  '\n'
-        for (heading, text) in report['sections']:
-            extra_text += '----- {} -----\n{}'.format(heading, text)
-    filename = osp.join(rootdir, report['filename'])
-    result = TestResult(cat, status, testname, message=message,
-                        time=report['duration'], extra_text=extra_text,
-                        filename=filename, lineno=report['lineno'])
-    return result
+        This function strips the .py suffix and replaces '/' by '.', so that
+        'ham/spam.py' becomes 'ham.spam'.
+
+        The result is relative to the directory from which tests are run and
+        not the pytest root dir.
+        """
+        wdir = osp.realpath(self.config.wdir)
+        if wdir != self.rootdir:
+            abspath = osp.join(self.rootdir, name)
+            try:
+                name = osp.relpath(abspath, start=wdir)
+            except ValueError:
+                # Happens on Windows if paths are on different drives
+                pass
+
+        if name.endswith('.py'):
+            name = name[:-3]
+        return name.replace(osp.sep, '.')
+
+    def convert_nodeid_to_testname(self, nodeid: str) -> str:
+        """Convert a nodeid to a test name."""
+        module, name = nodeid.split('::', 1)
+        module = self.normalize_module_name(module)
+        return '{}.{}'.format(module, name)
+
+    def convert_testname_to_nodeid(self, testname: str) -> str:
+        """
+        Convert a test name to a nodeid relative to wdir.
+
+        A true nodeid is relative to the pytest root dir. The return value of
+        this function is like a nodeid but relative to the wdir (i.e., the
+        directory from which test are run). This is the format that pytest
+        expects when running single tests.
+        """
+        *path_parts, last_part = testname.split('.')
+        path_parts[-1] += '.py'
+        nodeid = osp.join(*path_parts) + '::' + last_part
+        return nodeid
+
+    def logreport_collecterror_to_tuple(
+            self, report: dict[str, Any]) -> tuple[str, str]:
+        """Convert a 'collecterror' logreport to a (str, str) tuple."""
+        module = self.normalize_module_name(report['nodeid'])
+        return (module, report['longrepr'])
+
+    def logreport_starttest_to_str(self, report: dict[str, Any]) -> str:
+        """Convert a 'starttest' logreport to a str."""
+        return self.convert_nodeid_to_testname(report['nodeid'])
+
+    def logreport_to_testresult(self, report: dict[str, Any]) -> TestResult:
+        """Convert a logreport sent by test process to a TestResult."""
+        status = report['outcome']
+        if report['outcome'] in ('failed', 'xpassed') or report['witherror']:
+            cat = Category.FAIL
+        elif report['outcome'] in ('passed', 'xfailed'):
+            cat = Category.OK
+        else:
+            cat = Category.SKIP
+        testname = self.convert_nodeid_to_testname(report['nodeid'])
+        message = report.get('message', '')
+        extra_text = report.get('longrepr', '')
+        if 'sections' in report:
+            if extra_text:
+                extra_text +=  '\n'
+            for (heading, text) in report['sections']:
+                extra_text += '----- {} -----\n{}'.format(heading, text)
+        filename = osp.join(self.rootdir, report['filename'])
+        result = TestResult(cat, status, testname, message=message,
+                            time=report['duration'], extra_text=extra_text,
+                            filename=filename, lineno=report['lineno'])
+        return result
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/runnerbase.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/runnerbase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,89 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © 2013 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Classes for running tests within various frameworks."""
 
+from __future__ import annotations
+
 # Standard library imports
+from enum import IntEnum
+import logging
 import os
 import tempfile
+from typing import ClassVar, Optional, TYPE_CHECKING
 
 # Third party imports
-from importlib.util import find_spec as find_spec_or_loader
-from qtpy.QtCore import (QObject, QProcess, QProcessEnvironment, QTextCodec,
-                         Signal)
+from qtpy.QtCore import (
+    QObject, QProcess, QProcessEnvironment, QTextCodec, Signal)
+
+# Local imports
+if TYPE_CHECKING:
+    from spyder_unittest.widgets.configdialog import Config
+    from spyder_unittest.widgets.unittestgui import UnitTestWidget
 
 
+# Logging
+logger = logging.getLogger(__name__)
+
 # if generating coverage report, use this name for the TestResult
 # it's here in case we can get coverage results from unittest too
 COV_TEST_NAME = 'Total Test Coverage'
 
 
-class Category:
+class Category(IntEnum):
     """Enum type representing category of test result."""
 
     FAIL = 1
     OK = 2
     SKIP = 3
     PENDING = 4
     COVERAGE = 5
 
 
 class TestResult:
     """Class representing the result of running a single test."""
 
     __test__ = False  # this is not a pytest test class
 
-    def __init__(self, category, status, name, message='', time=None,
-                 extra_text='', filename=None, lineno=None):
+    def __init__(self, category: Category, status: str, name: str,
+                 message: str = '', time: Optional[float] = None,
+                 extra_text: str = '', filename: Optional[str] = None,
+                 lineno: Optional[int] = None):
         """
         Construct a test result.
-
-        Parameters
-        ----------
-        category : Category
-        status : str
-        name : str
-        message : str
-        time : float or None
-        extra_text : str
-        filename : str or None
-        lineno : int or None
         """
         self.category = category
         self.status = status
         self.name = name
         self.message = message
         self.time = time
         extra_text = extra_text.rstrip()
         if extra_text:
             self.extra_text = extra_text.split("\n")
         else:
             self.extra_text = []
         self.filename = filename
         self.lineno = lineno
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         """Test for equality."""
+        if not isinstance(other, TestResult):
+            return NotImplemented
         return self.__dict__ == other.__dict__
 
 
 class RunnerBase(QObject):
     """
     Base class for running tests with a framework that uses JUnit XML.
 
     This is an abstract class, meant to be subclassed before being used.
-    Concrete subclasses should define executable and create_argument_list(),
+    Concrete subclasses should define create_argument_list() and finished().
 
     All communication back to the caller is done via signals.
 
     Attributes
     ----------
     module : str
         Name of Python module for test framework. This needs to be defined
@@ -105,118 +110,132 @@
         Emitted when test process finishes. First argument contains the test
         results, second argument contains the output of the test process,
         third argument is True on normal exit, False on abnormal exit.
     sig_stop()
         Emitted when test process is being stopped.
     """
 
+    module: ClassVar[str]
+    name: ClassVar[str]
+
     sig_collected = Signal(object)
     sig_collecterror = Signal(object)
     sig_starttest = Signal(object)
     sig_testresult = Signal(object)
     sig_finished = Signal(object, str, bool)
     sig_stop = Signal()
 
-    def __init__(self, widget, resultfilename=None):
+    def __init__(self, widget: UnitTestWidget,
+                 resultfilename: Optional[str] = None):
         """
         Construct test runner.
 
         Parameters
         ----------
         widget : UnitTestWidget
             Unit test widget which constructs the test runner.
         resultfilename : str or None
             Name of file in which to store test results. If None, use default.
         """
         QObject.__init__(self, widget)
-        self.process = None
+        self.process: Optional[QProcess] = None
         if resultfilename is None:
             self.resultfilename = os.path.join(tempfile.gettempdir(),
                                                'unittest.results')
         else:
             self.resultfilename = resultfilename
 
-    def create_argument_list(self, config, cov_path):
+    def create_argument_list(self, config: Config,
+                             cov_path: Optional[str],
+                             single_test: Optional[str]) -> list[str]:
         """
         Create argument list for testing process (dummy).
 
         This function should be defined before calling self.start().
         """
         raise NotImplementedError
 
-    def _prepare_process(self, config, pythonpath):
+    def _prepare_process(self, config: Config,
+                         pythonpath: list[str]) -> QProcess:
         """
         Prepare and return process for running the unit test suite.
 
         This sets the working directory and environment.
         """
         process = QProcess(self)
         process.setProcessChannelMode(QProcess.MergedChannels)
         process.setWorkingDirectory(config.wdir)
         process.finished.connect(self.finished)
         if pythonpath:
             env = QProcessEnvironment.systemEnvironment()
-            old_python_path = env.value('PYTHONPATH', None)
+            old_python_path = env.value('PYTHONPATH', '')
             python_path_str = os.pathsep.join(pythonpath)
             if old_python_path:
                 python_path_str += os.pathsep + old_python_path
             env.insert('PYTHONPATH', python_path_str)
             process.setProcessEnvironment(env)
         return process
 
-    def start(self, config, cov_path, executable, pythonpath):
+    def start(self, config: Config, cov_path: Optional[str],
+              executable: str, pythonpath: list[str],
+              single_test: Optional[str]) -> None:
         """
         Start process which will run the unit test suite.
 
         The process is run in the working directory specified in 'config',
         with the directories in `pythonpath` added to the Python path for the
         test process. The test results are written to the file
         `self.resultfilename`. The standard output and error are also recorded.
         Once the process is finished, `self.finished()` will be called.
 
         Parameters
         ----------
-        config : TestConfig
+        config
             Unit test configuration.
-        cov_path : str or None
+        cov_path
             Path to filter source for coverage report
-        executable : str
+        executable
             Path to Python executable
-        pythonpath : list of str
+        pythonpath
             List of directories to be added to the Python path
+        single_test
+            If None, run all tests; otherwise, it is the name of the only test
+            to be run.
 
         Raises
         ------
         RuntimeError
             If process failed to start.
         """
         self.process = self._prepare_process(config, pythonpath)
-        p_args = self.create_argument_list(config, cov_path)
+        p_args = self.create_argument_list(config, cov_path, single_test)
         try:
             os.remove(self.resultfilename)
         except OSError:
             pass
+        logger.debug(f'Starting Python process with arguments {p_args}')
         self.process.start(executable, p_args)
         running = self.process.waitForStarted()
         if not running:
             raise RuntimeError
 
-    def finished(self):
+    def finished(self, exitcode: int) -> None:
         """
         Called when the unit test process has finished.
 
         This function should be implemented in derived classes. It should read
         the results (if necessary) and emit `sig_finished`.
         """
         raise NotImplementedError
 
-    def read_all_process_output(self):
+    def read_all_process_output(self) -> str:
         """Read and return all output from `self.process` as unicode."""
+        assert self.process is not None
         qbytearray = self.process.readAllStandardOutput()
         locale_codec = QTextCodec.codecForLocale()
         return locale_codec.toUnicode(qbytearray.data())
 
-    def stop_if_running(self):
+    def stop_if_running(self) -> None:
         """Stop testing process if it is running."""
         if self.process and self.process.state() == QProcess.Running:
             self.process.kill()
             self.sig_stop.emit()
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_abbreviator.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_abbreviator.py`

 * *Files identical despite different names*

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_frameworkregistry.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_frameworkregistry.py`

 * *Files identical despite different names*

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_pytestrunner.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_pytestrunner.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,102 +4,108 @@
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Tests for pytestrunner.py"""
 
 # Standard library imports
 import os.path as osp
 import sys
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 
 # Third party imports
 import pytest
 
 # Local imports
-from spyder_unittest.backend.pytestrunner import (PyTestRunner,
-                                                  logreport_to_testresult)
+from spyder_unittest.backend.pytestrunner import PyTestRunner
 from spyder_unittest.backend.runnerbase import (Category, TestResult,
                                                 COV_TEST_NAME)
 from spyder_unittest.widgets.configdialog import Config
 
 
-def test_pytestrunner_create_argument_list(monkeypatch):
-    config = Config()
+@pytest.fixture
+def runner():
+    res = PyTestRunner(None)
+    res.rootdir = 'ham'
+    res.config = Config(wdir='ham')
+    return res
+
+
+def test_pytestrunner_create_argument_list(monkeypatch, runner):
+    config = Config(args=['--extra-arg'])
     cov_path = None
     MockZMQStreamReader = Mock()
     monkeypatch.setattr(
         'spyder_unittest.backend.pytestrunner.ZmqStreamReader',
         MockZMQStreamReader)
     mock_reader = MockZMQStreamReader()
     mock_reader.port = 42
     runner = PyTestRunner(None, 'results')
     runner.reader = mock_reader
     monkeypatch.setattr('spyder_unittest.backend.pytestrunner.os.path.dirname',
                         lambda _: 'dir')
-    pyfile, port, *coverage = runner.create_argument_list(config, cov_path)
+    arg_list = runner.create_argument_list(config, cov_path, None)
+    pyfile, port, *coverage, last = arg_list
     assert pyfile == osp.join('dir', 'workers', 'pytestworker.py')
     assert port == '42'
+    assert last == '--extra-arg'
 
 
 def test_pytestrunner_start(monkeypatch):
     MockZMQStreamReader = Mock()
     monkeypatch.setattr(
         'spyder_unittest.backend.pytestrunner.ZmqStreamReader',
         MockZMQStreamReader)
     mock_reader = MockZMQStreamReader()
 
-    MockRunnerBase = Mock(name='RunnerBase')
-    monkeypatch.setattr('spyder_unittest.backend.pytestrunner.RunnerBase',
-                        MockRunnerBase)
+    mock_base_start = Mock()
+    monkeypatch.setattr('spyder_unittest.backend.unittestrunner.RunnerBase.start',
+                        mock_base_start)
 
     runner = PyTestRunner(None, 'results')
     config = Config()
     cov_path = None
-    runner.start(config, cov_path, sys.executable, ['pythondir'])
+    runner.start(config, cov_path, sys.executable, ['pythondir'], None)
     assert runner.config is config
     assert runner.reader is mock_reader
     runner.reader.sig_received.connect.assert_called_once_with(
         runner.process_output)
-    MockRunnerBase.start.assert_called_once_with(
-        runner, config, cov_path, sys.executable, ['pythondir'])
+    mock_base_start.assert_called_once_with(
+        config, cov_path, sys.executable, ['pythondir'], None)
 
 
-def test_pytestrunner_process_output_with_collected(qtbot):
-    runner = PyTestRunner(None)
+def test_pytestrunner_process_output_with_collected(qtbot, runner):
     output = [{'event': 'collected', 'nodeid': 'spam.py::ham'},
               {'event': 'collected', 'nodeid': 'eggs.py::bacon'}]
     with qtbot.waitSignal(runner.sig_collected) as blocker:
         runner.process_output(output)
     expected = ['spam.ham', 'eggs.bacon']
     assert blocker.args == [expected]
 
 
-def test_pytestrunner_process_output_with_collecterror(qtbot):
-    runner = PyTestRunner(None)
+def test_pytestrunner_process_output_with_collecterror(qtbot, runner):
     output = [{
             'event': 'collecterror',
             'nodeid': 'ham/spam.py',
             'longrepr': 'msg'
     }]
     with qtbot.waitSignal(runner.sig_collecterror) as blocker:
         runner.process_output(output)
     expected = [('ham.spam', 'msg')]
     assert blocker.args == [expected]
 
 
-def test_pytestrunner_process_output_with_starttest(qtbot):
-    runner = PyTestRunner(None)
+def test_pytestrunner_process_output_with_starttest(qtbot, runner):
     output = [{'event': 'starttest', 'nodeid': 'ham/spam.py::ham'},
               {'event': 'starttest', 'nodeid': 'ham/eggs.py::bacon'}]
     with qtbot.waitSignal(runner.sig_starttest) as blocker:
         runner.process_output(output)
     expected = ['ham.spam.ham', 'ham.eggs.bacon']
     assert blocker.args == [expected]
 
 
-@pytest.mark.parametrize('exitcode, normal_exit', 
+@pytest.mark.parametrize('exitcode, normal_exit',
                          [(0, True), (1, True), (2, True), (3, False),
                           (4, False), (5, True)])
 def test_pytestrunner_finished(qtbot, exitcode, normal_exit):
     output = '== 1 passed in 0.10s =='
     mock_reader = Mock()
     mock_reader.close = lambda: None
     runner = PyTestRunner(None)
@@ -108,28 +114,60 @@
     runner.config = Config('pytest', None, False)
     with qtbot.waitSignal(runner.sig_finished) as blocker:
         runner.finished(exitcode)
     results = []
     assert blocker.args == [results, output, normal_exit]
 
 
+@pytest.mark.parametrize('wdir, expected', [
+    ('ham', 'spam.eggs'),
+    (osp.join('ham', 'spam'), 'eggs'),
+    (osp.join('link-to-ham', 'spam'), 'eggs')])
+def test_normalize_module_name(runner, wdir, expected):
+    def new_realpath(name):
+        """Simulate link from `link-to-ham` to `ham`"""
+        if name.startswith('link-to-ham'):
+            return name[len('link-to-'):]
+        else:
+            return name
+
+    with patch('spyder_unittest.backend.pytestrunner.osp.realpath',
+               side_effect=new_realpath):
+        runner.config = Config(wdir=wdir)
+        result = runner.normalize_module_name(osp.join('spam', 'eggs.py'))
+        assert result == expected
+
+
+def test_convert_nodeid_to_testname(runner):
+    nodeid = osp.join('spam', 'eggs.py') + '::test_foo'
+    testname = 'spam.eggs.test_foo'
+    result = runner.convert_nodeid_to_testname(nodeid)
+    assert result == testname
+
+
+def test_convert_testname_to_nodeid(runner):
+    nodeid = osp.join('spam', 'eggs.py') + '::test_foo'
+    testname = 'spam.eggs.test_foo'
+    result = runner.convert_testname_to_nodeid(testname)
+    assert result == nodeid
+
+
 def standard_logreport_output():
     return {
         'event': 'logreport',
         'outcome': 'passed',
         'witherror': False,
         'nodeid': 'foo.py::bar',
         'filename': 'foo.py',
         'lineno': 24,
         'duration': 42
     }
 
-def test_pytestrunner_process_output_with_logreport_passed(qtbot):
-    runner = PyTestRunner(None)
-    runner.rootdir = 'ham'
+
+def test_pytestrunner_process_output_with_logreport_passed(qtbot, runner):
     output = [standard_logreport_output()]
     with qtbot.waitSignal(runner.sig_testresult) as blocker:
         runner.process_output(output)
     expected = [TestResult(Category.OK, 'passed', 'foo.bar', time=42,
                            filename=osp.join('ham', 'foo.py'), lineno=24)]
     assert blocker.args == [expected]
 
@@ -218,53 +256,51 @@
     ('xfailed', True, Category.FAIL),
     ('xfailed', False, Category.OK),
     ('xpassed', True, Category.FAIL),
     ('xpassed', False, Category.FAIL),
     ('---', True, Category.FAIL)
     # ('---', False, this is not possible)
 ])
-def test_logreport_to_testresult_with_outcome_and_possible_error(outcome,
-                                                                 witherror,
-                                                                 category):
+def test_logreport_to_testresult_with_outcome_and_possible_error(
+        runner, outcome, witherror, category):
     report = standard_logreport_output()
     report['outcome'] = outcome
     report['witherror'] = witherror
     expected = TestResult(category, outcome, 'foo.bar', time=42,
                           filename=osp.join('ham', 'foo.py'), lineno=24)
-    assert logreport_to_testresult(report, 'ham') == expected
+    assert runner.logreport_to_testresult(report) == expected
 
 
-def test_logreport_to_testresult_with_message():
+def test_logreport_to_testresult_with_message(runner):
     report = standard_logreport_output()
     report['message'] = 'msg'
     expected = TestResult(Category.OK, 'passed', 'foo.bar', message='msg',
                           time=42, filename=osp.join('ham', 'foo.py'),
                           lineno=24)
-    assert logreport_to_testresult(report, 'ham') == expected
+    assert runner.logreport_to_testresult(report) == expected
 
 
-def test_logreport_to_testresult_with_extratext():
+def test_logreport_to_testresult_with_extratext(runner):
     report = standard_logreport_output()
     report['longrepr'] = 'long msg'
     expected = TestResult(Category.OK, 'passed', 'foo.bar', time=42,
                           extra_text='long msg',
                           filename=osp.join('ham', 'foo.py'), lineno=24)
-    assert logreport_to_testresult(report, 'ham') == expected
+    assert runner.logreport_to_testresult(report) == expected
 
 
 @pytest.mark.parametrize('longrepr,prefix', [
     ('', ''),
     ('msg', '\n')
 ])
-def test_logreport_to_testresult_with_output(longrepr, prefix):
+def test_logreport_to_testresult_with_output(runner, longrepr, prefix):
     report = standard_logreport_output()
     report['longrepr'] = longrepr
     report['sections'] = [['Captured stdout call', 'ham\n'],
                           ['Captured stderr call', 'spam\n']]
     txt = (longrepr + prefix +
            '----- Captured stdout call -----\nham\n'
            '----- Captured stderr call -----\nspam\n')
     expected = TestResult(Category.OK, 'passed', 'foo.bar', time=42,
                           extra_text=txt, filename=osp.join('ham', 'foo.py'),
                           lineno=24)
-    assert logreport_to_testresult(report, 'ham') == expected
-
+    assert runner.logreport_to_testresult(report) == expected
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_runnerbase.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_runnerbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     class FooRunner(RunnerBase):
         module = 'nonexisiting'
 
     foo_runner = FooRunner(None)
     config = Config(foo_runner.module, 'wdir', True)
 
     with pytest.raises(NotImplementedError):
-        foo_runner.create_argument_list(config, 'cov_path')
+        foo_runner.create_argument_list(config, 'cov_path', None)
 
     with pytest.raises(NotImplementedError):
-        foo_runner.finished()
+        foo_runner.finished(0)
 
 
 @pytest.mark.parametrize('pythonpath,env_pythonpath', [
     ([], None),
     (['pythonpath'], None),
     (['pythonpath'], 'old')
 ])
@@ -77,16 +77,16 @@
 
     mock_remove = Mock(side_effect=OSError())
     monkeypatch.setattr('spyder_unittest.backend.runnerbase.os.remove',
                         mock_remove)
 
     runner = RunnerBase(None, 'results')
     runner._prepare_process = lambda c, p: mock_process
-    runner.create_argument_list = lambda c, cp: ['arg1', 'arg2']
+    runner.create_argument_list = lambda c, cp, st: ['arg1', 'arg2']
     config = Config('pytest', 'wdir', False)
     cov_path = None
     mock_process.waitForStarted = lambda: False
     with pytest.raises(RuntimeError):
-        runner.start(config, cov_path, 'python_exec', ['pythondir'])
+        runner.start(config, cov_path, 'python_exec', ['pythondir'], None)
 
     mock_process.start.assert_called_once_with('python_exec', ['arg1', 'arg2'])
     mock_remove.assert_called_once_with('results')
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/tests/test_zmqstream.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/__init__.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 This directory contains scripts and supporting modules that are supposed
 to be executed in the target environment (using the Python interpreter
 that the user specifies in the Preferences) instead of the environment that
 Spyder runs in.
 
 Dependencies should be kept to a minimum, because they need to be installed
 in each target environment.
-"""
+"""
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/print_versions.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/print_versions.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,31 +33,29 @@
                 plugins=[GetPluginVersionsPlugin()])
 
     return {'available': True,
             'version': pytest.__version__,
             'plugins': plugins}
 
 
-def get_nose_info():
-    """Return information about nose."""
-    from pkg_resources import iter_entry_points
+def get_nose2_info():
+    """
+    Return information about nose2.
+
+    This only returns the version of nose2. The function does not gather any
+    information about plugins.
+    """
     try:
-        import nose
+        import nose2
     except ImportError:
         return {'available': False}
 
-    plugins = {}
-    for entry_point, _ in (nose.plugins.manager.EntryPointPluginManager
-                           .entry_points):
-        for ep in iter_entry_points(entry_point):
-            plugins[ep.dist.project_name] = ep.dist.version
-
     return {'available': True,
-            'version': nose.__version__,
-            'plugins': plugins}
+            'version': nose2.__version__,
+            'plugins': {}}
 
 
 def get_unittest_info():
     """
     Return versions of framework and its plugins.
 
     As 'unittest' is a built-in framework, we use the python version.
@@ -71,17 +69,17 @@
 def get_all_info():
     """
     Return information about all testing frameworks.
 
     Information is returned as a dictionary like the following:
     {'pytest': {'available': True, 'version': '7.1.1',
                 'plugins': {'flaky': '3.7.0', 'pytest-mock': '3.6.1'}},
-     'nose': {'available': False},
+     'nose2': {'available': False},
      'unittest': {'available': True, 'version': '3.10.5', 'plugins': {}}}
     """
     return {'pytest': get_pytest_info(),
-            'nose': get_nose_info(),
+            'nose2': get_nose2_info(),
             'unittest': get_unittest_info()}
 
 
 if __name__ == '__main__':
     print(get_all_info())
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/pytestworker.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/pytestworker.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,37 +13,18 @@
 
 # Standard library imports
 import sys
 
 # Third party imports
 import pytest
 
-# Local imports, needs to be relative otherwise it will fail if trying
-# to execute in a different env with only spyder-kernel installed
-try:
-    # this line is needed for the tests to succeed
-    from .zmqwriter import ZmqStreamWriter
-except:
-    # this line is needed for the plugin to work
-    from zmqwriter import ZmqStreamWriter
-
-class FileStub():
-    """Stub for ZmqStreamWriter which instead writes to a file."""
-
-    def __init__(self, filename):
-        """Constructor; connect to specified filename."""
-        self.file = open(filename, 'w')
-
-    def write(self, obj):
-        """Write Python object to file."""
-        self.file.write(str(obj) + '\n')
-
-    def close(self):
-        """Close file."""
-        self.file.close()
+# Local imports
+# Note that the script can be run in an environment that does not contain
+# spyder_unittest so `from spyder_unittest.xxx import xxx` does not work.
+from zmqwriter import FileStub, ZmqStreamWriter
 
 
 class SpyderPlugin():
     """Pytest plugin which reports in format suitable for Spyder."""
 
     def __init__(self, writer):
         """Constructor."""
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/tests/test_print_versions.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/test_print_versions.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Tests for print_versions.py"""
 
 from spyder_unittest.backend.workers.print_versions import (
-    get_nose_info, get_pytest_info, get_unittest_info)
+    get_nose2_info, get_pytest_info, get_unittest_info)
 
 
 def test_get_pytest_info_without_plugins(monkeypatch):
     import pytest
     monkeypatch.setattr(pytest, '__version__', '1.2.3')
     from _pytest.config import PytestPluginManager
     monkeypatch.setattr(
@@ -33,38 +33,19 @@
         PytestPluginManager,
         'list_plugin_distinfo', lambda _: (('1', dist1), ('2', dist2)))
     expected = {'available': True, 'version': '1.2.3',
                 'plugins': {'myPlugin1': '4.5.6', 'myPlugin2': '7.8.9'}}
     assert get_pytest_info() == expected
 
 
-def test_get_nose_info_without_plugins(monkeypatch):
-    import nose
-    import pkg_resources
-    monkeypatch.setattr(nose, '__version__', '1.2.3')
-    monkeypatch.setattr(pkg_resources, 'iter_entry_points', lambda x: ())
+def test_get_nose2_info(monkeypatch):
+    import nose2
+    monkeypatch.setattr(nose2, '__version__', '1.2.3')
     expected = {'available': True, 'version': '1.2.3', 'plugins': {}}
-    assert get_nose_info() == expected
-
-
-def test_get_nose_info_with_plugins(monkeypatch):
-    import nose
-    import pkg_resources
-    monkeypatch.setattr(nose, '__version__', '1.2.3')
-    dist = pkg_resources.Distribution(project_name='myPlugin',
-                                      version='4.5.6')
-    ep = pkg_resources.EntryPoint('name', 'module_name', dist=dist)
-    monkeypatch.setattr(pkg_resources,
-                        'iter_entry_points',
-                        lambda ept: (x for x in (ep,) if ept == nose.plugins
-                                     .manager.EntryPointPluginManager
-                                     .entry_points[0][0]))
-    expected = {'available': True, 'version': '1.2.3',
-                'plugins': {'myPlugin': '4.5.6'}}
-    assert get_nose_info() == expected
+    assert get_nose2_info() == expected
 
 
 def test_get_unittest_imfo(monkeypatch):
     import platform
     monkeypatch.setattr(platform, 'python_version', lambda: '1.2.3')
     expected = {'available': True, 'version': '1.2.3', 'plugins': {}}
     assert get_unittest_info() == expected
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/tests/test_pytestworker.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/tests/test_pytestworker.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 # Copyright © 2017 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Tests for pytestworker.py"""
 
 # Standard library imports
 import os
+import os.path as osp
+import sys
 from unittest.mock import create_autospec, MagicMock, Mock
 
 # Third party imports
 import pytest
 
 # Local imports
+# Local imports
+# Modules in spyder_unittest.backend.workers assume that their directory
+# is in `sys.path`, so add that directory to the path.
+old_path = sys.path
+sys.path.insert(0, osp.join(osp.dirname(__file__), osp.pardir))
 from spyder_unittest.backend.workers.pytestworker import SpyderPlugin, main
 from spyder_unittest.backend.workers.zmqwriter import ZmqStreamWriter
+sys.path = old_path
 
 
 class EmptyClass:
     pass
 
 
 @pytest.fixture
@@ -301,53 +309,70 @@
         'filename': 'foo.py',
         'lineno': 24,
         'message': message,
         'longrepr': longrepr
     })
 
 
-def test_pytestworker_integration(monkeypatch, tmpdir):
-    os.chdir(tmpdir.strpath)
-    testfilename = tmpdir.join('test_foo.py').strpath
-    with open(testfilename, 'w') as f:
-        f.write("def test_ok(): assert 1+1 == 2\n"
-                "def test_fail(): assert 1+1 == 3\n")
+@pytest.fixture(scope='module')
+def testfile_path(tmp_path_factory):
+    tmp_path = tmp_path_factory.mktemp('pytestworker')
+    res = tmp_path / 'test_pytestworker_foo.py'
+    res.write_text('def test_ok(): assert 1+1 == 2\n'
+                   'def test_fail(): assert 1+1 == 3\n')
+    return res
+
 
+@pytest.mark.parametrize('alltests', [True, False])
+def test_pytestworker_integration(monkeypatch, testfile_path, alltests):
     mock_writer = create_autospec(ZmqStreamWriter)
     MockZmqStreamWriter = Mock(return_value=mock_writer)
     monkeypatch.setattr(
         'spyder_unittest.backend.workers.pytestworker.ZmqStreamWriter',
         MockZmqStreamWriter)
-    main(['mockscriptname', '42', testfilename])
 
-    args = mock_writer.write.call_args_list
+    os.chdir(testfile_path.parent)
+    testfilename = testfile_path.name
+    pytest_args = ['mockscriptname', '42']
+    if not alltests:
+        pytest_args.append(f'{testfilename}::test_ok')
+    main(pytest_args)
 
-    assert args[0][0][0]['event'] == 'config'
-    assert 'rootdir' in args[0][0][0]
+    args = mock_writer.write.call_args_list
+    messages = [arg[0][0] for arg in args]
+    assert len(messages) == 7 if alltests else 4
 
-    assert args[1][0][0]['event'] == 'collected'
-    assert args[1][0][0]['nodeid'] == 'test_foo.py::test_ok'
+    assert messages[0]['event'] == 'config'
+    assert 'rootdir' in messages[0]
 
-    assert args[2][0][0]['event'] == 'collected'
-    assert args[2][0][0]['nodeid'] == 'test_foo.py::test_fail'
+    assert messages[1]['event'] == 'collected'
+    assert messages[1]['nodeid'] == f'{testfilename}::test_ok'
 
-    assert args[3][0][0]['event'] == 'starttest'
-    assert args[3][0][0]['nodeid'] == 'test_foo.py::test_ok'
-
-    assert args[4][0][0]['event'] == 'logreport'
-    assert args[4][0][0]['outcome'] == 'passed'
-    assert args[4][0][0]['nodeid'] == 'test_foo.py::test_ok'
-    assert args[4][0][0]['sections'] == []
-    assert args[4][0][0]['filename'] == 'test_foo.py'
-    assert args[4][0][0]['lineno'] == 0
-    assert 'duration' in args[4][0][0]
-
-    assert args[5][0][0]['event'] == 'starttest'
-    assert args[5][0][0]['nodeid'] == 'test_foo.py::test_fail'
-
-    assert args[6][0][0]['event'] == 'logreport'
-    assert args[6][0][0]['outcome'] == 'failed'
-    assert args[6][0][0]['nodeid'] == 'test_foo.py::test_fail'
-    assert args[6][0][0]['sections'] == []
-    assert args[6][0][0]['filename'] == 'test_foo.py'
-    assert args[6][0][0]['lineno'] == 1
-    assert 'duration' in args[6][0][0]
+    if alltests:
+        n = 3
+        assert messages[2]['event'] == 'collected'
+        assert messages[2]['nodeid'] == f'{testfilename}::test_fail'
+    else:
+        n = 2
+
+    assert messages[n]['event'] == 'starttest'
+    assert messages[n]['nodeid'] == f'{testfilename}::test_ok'
+
+    assert messages[n+1]['event'] == 'logreport'
+    assert messages[n+1]['outcome'] == 'passed'
+    assert messages[n+1]['nodeid'] == f'{testfilename}::test_ok'
+    assert messages[n+1]['sections'] == []
+    assert messages[n+1]['filename'] == testfilename
+    assert messages[n+1]['lineno'] == 0
+    assert 'duration' in messages[n+1]
+
+    if alltests:
+        assert messages[n+2]['event'] == 'starttest'
+        assert messages[n+2]['nodeid'] == f'{testfilename}::test_fail'
+
+        assert messages[n+3]['event'] == 'logreport'
+        assert messages[n+3]['outcome'] == 'failed'
+        assert messages[n+3]['nodeid'] == f'{testfilename}::test_fail'
+        assert messages[n+3]['sections'] == []
+        assert messages[n+3]['filename'] == testfilename
+        assert messages[n+3]['lineno'] == 1
+        assert 'duration' in messages[n+3]
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/workers/zmqwriter.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/workers/zmqwriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,36 +18,52 @@
 # Third party imports
 import zmq
 
 
 class ZmqStreamWriter:
     """Writer for sending stream of Python object over a ZMQ stream."""
 
-    def __init__(self, port):
+    def __init__(self, port: str) -> None:
         """
         Constructor.
 
         Arguments
         ---------
-        port : int
+        port : str
             TCP port number to be used for the stream. This should equal the
             `port` attribute of the corresponding `ZmqStreamReader`.
         """
         context = zmq.Context()
         self.socket = context.socket(zmq.PAIR)
         self.socket.connect('tcp://localhost:{}'.format(port))
 
-    def write(self, obj):
+    def write(self, obj: object) -> None:
         """Write arbitrary Python object to stream."""
         self.socket.send_pyobj(obj)
 
-    def close(self):
+    def close(self) -> None:
         """Close stream."""
         self.socket.close()
 
 
+class FileStub(ZmqStreamWriter):
+    """Stub for ZmqStreamWriter which instead writes to a file."""
+
+    def __init__(self, filename: str) -> None:
+        """Constructor; connect to specified filename."""
+        self.file = open(filename, 'w')
+
+    def write(self, obj: object) -> None:
+        """Write Python object to file."""
+        self.file.write(str(obj) + '\n')
+
+    def close(self) -> None:
+        """Close file."""
+        self.file.close()
+
+
 if __name__ == '__main__':
     # Usage: python zmqwriter.py <port>
     # Construct a ZMQ stream on the given port number and send the number 42
     # over the stream (for testing)
     worker = ZmqStreamWriter(sys.argv[1])
     worker.write(42)
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/backend/zmqreader.py` & `spyder_unittest-0.6.0/spyder_unittest/backend/zmqreader.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,40 +32,40 @@
     sig_received(list)
         Emitted when objects are received; argument is list of received
         objects.
     """
 
     sig_received = Signal(object)
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Constructor; also constructs ZMQ stream."""
         super().__init__()
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.PAIR)
         self.port = self.socket.bind_to_random_port('tcp://*')
         fid = self.socket.getsockopt(zmq.FD)
         self.notifier = QSocketNotifier(fid, QSocketNotifier.Read, self)
         self.notifier.activated.connect(self.received_message)
 
-    def received_message(self):
+    def received_message(self) -> None:
         """Called when a message is received."""
         self.notifier.setEnabled(False)
         messages = []
         try:
             while 1:
                 message = self.socket.recv_pyobj(flags=zmq.NOBLOCK)
                 messages.append(message)
         except zmq.ZMQError:
             pass
         finally:
             self.notifier.setEnabled(True)
         if messages:
             self.sig_received.emit(messages)
 
-    def close(self):
+    def close(self) -> None:
         """Read any remaining messages and close stream."""
         self.received_message()  # Flush remaining messages
         self.notifier.setEnabled(False)
         self.socket.close()
         self.context.destroy()
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/de/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/de/LC_MESSAGES/spyder_unittest.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: spyder-unittest\n"
-"POT-Creation-Date: 2022-09-03 17:43+0100\n"
-"PO-Revision-Date: 2022-09-03 20:06\n"
+"POT-Creation-Date: 2023-06-23 16:41+0100\n"
+"PO-Revision-Date: 2023-06-25 20:37\n"
 "Last-Translator: \n"
 "Language-Team: German\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -28,41 +28,56 @@
 
 msgid ", {} passed"
 msgstr ", {} bestanden"
 
 msgid ", {} pending"
 msgstr ", {} ausstehend"
 
+msgid "Abbreviate test names"
+msgstr "Testnamen abkürzen"
+
+msgid "Captured stderr"
+msgstr "Erfasstes stderr"
+
+msgid "Captured stdout"
+msgstr "Erfasstes stdout"
+
 msgid "Collapse"
 msgstr "Einklappen"
 
 msgid "Collapse all"
 msgstr "Alle einklappen"
 
+msgid "Command-line arguments:"
+msgstr "Befehlszeilenargumente:"
+
 msgid "Configure ..."
 msgstr "Konfigurieren ..."
 
 msgid "Configure tests"
 msgstr "Tests konfigurieren"
 
 msgid "Dependencies"
 msgstr "Abhängigkeiten"
 
-msgid "Directory from which to run tests"
-msgstr "Verzeichnis, aus dem Tests ausgeführt werden sollen"
+msgid "Directory from which to run tests:"
+msgstr "Verzeichnis, aus dem Tests ausgeführt werden sollen:"
 
 msgid "Error"
 msgstr "Fehler"
 
 msgid "Expand"
 msgstr "Ausklappen"
 
 msgid "Expand all"
 msgstr "Alle ausklappen"
 
+msgid "Extra command-line arguments when running tests"
+msgstr "Zusätzliche Befehlszeilenargumente bei der Ausführung von Tests"
+
 msgid "Go to definition"
 msgstr "Zur Definition gehen"
 
 msgid "Include coverage report in output"
 msgstr "Abdeckungsbericht in Ausgabe einbeziehen"
 
 msgid "Message"
@@ -76,59 +91,83 @@
 
 msgid "No results to show."
 msgstr "Keine anzuzeigenden Ergebnisse."
 
 msgid "Process failed to start"
 msgstr "Prozess konnte nicht gestartet werden"
 
+msgid "Run only this test"
+msgstr "Nur diesen Test ausführen"
+
+msgid "Run test suites and view their results"
+msgstr "Testsuiten ausführen und ihre Ergebnisse ansehen"
+
 msgid "Run tests"
 msgstr "Tests ausführen"
 
 msgid "Run unit tests"
 msgstr "Unit-Tests ausführen"
 
 msgid "Running tests ..."
 msgstr "Tests laufen ..."
 
 msgid "Select directory"
 msgstr "Verzeichnis auswählen"
 
+msgid "Settings"
+msgstr "Einstellungen"
+
 msgid "Show output"
 msgstr "Ausgabe anzeigen"
 
 msgid "Status"
 msgstr "Status"
 
 msgid "Stop"
 msgstr "Stopp"
 
 msgid "Stop current test process"
 msgstr "Aktuellen Testprozess stoppen"
 
+msgid "Test framework:"
+msgstr "Test-Framework:"
+
+msgid "Test process exited abnormally"
+msgstr "Testprozess wurde abnormal beendet"
+
 msgid "Time (ms)"
 msgstr "Zeit (ms)"
 
 msgid "Unit testing"
 msgstr "Unit-Tests"
 
 msgid "Unit testing output"
 msgstr "Ausgabe der Unit-Tests"
 
+msgid "Versions of frameworks and their installed plugins:"
+msgstr "Versionen von Frameworks und deren installierte Plugins:"
+
 msgid "Works only for pytest, requires pytest-cov"
 msgstr "Funktioniert nur für pytest, erfordert pytest-cov"
 
 msgid "collected {}"
 msgstr "{} gesammelt"
 
+msgid "collection error"
+msgstr "Sammlungsfehler"
+
 msgid "failure"
 msgstr "Fehlschlag"
 
 msgid "not available"
 msgstr "nicht verfügbar"
 
+msgid "not run"
+msgstr "nicht ausgeführt"
+
 msgid "pending"
 msgstr "ausstehend"
 
 msgid "running"
 msgstr "läuft"
 
 msgid "test"
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/es/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/es/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
 00000020: 2c00 0000 0002 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
 000000b0: 616e 6775 6167 652d 5465 616d 3a20 5370  anguage-Team: Sp
 000000c0: 616e 6973 680a 4d49 4d45 2d56 6572 7369  anish.MIME-Versi
 000000d0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000000e0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000000f0: 3b20 6368 6172 7365 743d 5554 462d 380a  ; charset=UTF-8.
 00000100: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/fr/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/fr/LC_MESSAGES/spyder_unittest.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: spyder-unittest\n"
-"POT-Creation-Date: 2022-09-03 17:43+0100\n"
-"PO-Revision-Date: 2022-09-03 20:06\n"
+"POT-Creation-Date: 2023-06-23 16:41+0100\n"
+"PO-Revision-Date: 2023-06-24 20:15\n"
 "Last-Translator: \n"
 "Language-Team: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -40,16 +40,16 @@
 
 msgid "Configure ..."
 msgstr "Configurer ..."
 
 msgid "Configure tests"
 msgstr "Configurer les tests"
 
-msgid "Directory from which to run tests"
-msgstr "Répertoire depuis lequel exécuter les tests"
+msgid "Directory from which to run tests:"
+msgstr "Répertoire depuis lequel exécuter les tests:"
 
 msgid "Error"
 msgstr "Erreur"
 
 msgid "Expand"
 msgstr "Déployer"
 
@@ -91,16 +91,16 @@
 
 msgid "Stop"
 msgstr "Arrêter"
 
 msgid "Stop current test process"
 msgstr "Arrêter le processus de test en cours"
 
-msgid "Test framework"
-msgstr "Système de test"
+msgid "Test framework:"
+msgstr "Système de test:"
 
 msgid "Time (ms)"
 msgstr "Durée (ms)"
 
 msgid "Unit testing"
 msgstr "Tests unitaires"
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/hr/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/hu/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 4802 0000 2d00 0000 0050 726f  ,...H...-....Pro
+00000020: 2c00 0000 ff01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
-000000b0: 616e 6775 6167 652d 5465 616d 3a20 4372  anguage-Team: Cr
-000000c0: 6f61 7469 616e 0a4d 494d 452d 5665 7273  oatian.MIME-Vers
-000000d0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
-000000e0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
-000000f0: 6e3b 2063 6861 7273 6574 3d55 5446 2d38  n; charset=UTF-8
-00000100: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
-00000110: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
-00000120: 0a47 656e 6572 6174 6564 2d42 793a 2070  .Generated-By: p
-00000130: 7967 6574 7465 7874 2e70 7920 312e 350a  ygettext.py 1.5.
-00000140: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
-00000150: 6c75 7261 6c73 3d33 3b20 706c 7572 616c  lurals=3; plural
-00000160: 3d28 6e25 3130 3d3d 3120 2626 206e 2531  =(n%10==1 && n%1
-00000170: 3030 213d 3131 203f 2030 203a 206e 2531  00!=11 ? 0 : n%1
-00000180: 303e 3d32 2026 2620 6e25 3130 3c3d 3420  0>=2 && n%10<=4 
-00000190: 2626 2028 6e25 3130 303c 3130 207c 7c20  && (n%100<10 || 
-000001a0: 6e25 3130 303e 3d32 3029 203f 2031 203a  n%100>=20) ? 1 :
-000001b0: 2032 293b 0a58 2d43 726f 7764 696e 2d50   2);.X-Crowdin-P
-000001c0: 726f 6a65 6374 3a20 7370 7964 6572 2d75  roject: spyder-u
-000001d0: 6e69 7474 6573 740a 582d 4372 6f77 6469  nittest.X-Crowdi
-000001e0: 6e2d 5072 6f6a 6563 742d 4944 3a20 3338  n-Project-ID: 38
-000001f0: 3138 3339 0a58 2d43 726f 7764 696e 2d4c  1839.X-Crowdin-L
-00000200: 616e 6775 6167 653a 2068 720a 582d 4372  anguage: hr.X-Cr
-00000210: 6f77 6469 6e2d 4669 6c65 3a20 2f6d 6173  owdin-File: /mas
-00000220: 7465 722f 7370 7964 6572 5f75 6e69 7474  ter/spyder_unitt
-00000230: 6573 742f 6c6f 6361 6c65 2f73 7079 6465  est/locale/spyde
-00000240: 725f 756e 6974 7465 7374 2e70 6f74 0a58  r_unittest.pot.X
-00000250: 2d43 726f 7764 696e 2d46 696c 652d 4944  -Crowdin-File-ID
-00000260: 3a20 3439 0a4c 616e 6775 6167 653a 2068  : 49.Language: h
-00000270: 725f 4852 0a00                           r_HR..
+000000b0: 616e 6775 6167 652d 5465 616d 3a20 4875  anguage-Team: Hu
+000000c0: 6e67 6172 6961 6e0a 4d49 4d45 2d56 6572  ngarian.MIME-Ver
+000000d0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
+000000e0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
+000000f0: 696e 3b20 6368 6172 7365 743d 5554 462d  in; charset=UTF-
+00000100: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
+00000110: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+00000120: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
+00000130: 7079 6765 7474 6578 742e 7079 2031 2e35  pygettext.py 1.5
+00000140: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
+00000150: 706c 7572 616c 733d 323b 2070 6c75 7261  plurals=2; plura
+00000160: 6c3d 286e 2021 3d20 3129 3b0a 582d 4372  l=(n != 1);.X-Cr
+00000170: 6f77 6469 6e2d 5072 6f6a 6563 743a 2073  owdin-Project: s
+00000180: 7079 6465 722d 756e 6974 7465 7374 0a58  pyder-unittest.X
+00000190: 2d43 726f 7764 696e 2d50 726f 6a65 6374  -Crowdin-Project
+000001a0: 2d49 443a 2033 3831 3833 390a 582d 4372  -ID: 381839.X-Cr
+000001b0: 6f77 6469 6e2d 4c61 6e67 7561 6765 3a20  owdin-Language: 
+000001c0: 6875 0a58 2d43 726f 7764 696e 2d46 696c  hu.X-Crowdin-Fil
+000001d0: 653a 202f 6d61 7374 6572 2f73 7079 6465  e: /master/spyde
+000001e0: 725f 756e 6974 7465 7374 2f6c 6f63 616c  r_unittest/local
+000001f0: 652f 7370 7964 6572 5f75 6e69 7474 6573  e/spyder_unittes
+00000200: 742e 706f 740a 582d 4372 6f77 6469 6e2d  t.pot.X-Crowdin-
+00000210: 4669 6c65 2d49 443a 2034 390a 4c61 6e67  File-ID: 49.Lang
+00000220: 7561 6765 3a20 6875 5f48 550a 00         uage: hu_HU..
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/hu/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/zh_CN/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 ff01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 0402 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
-000000b0: 616e 6775 6167 652d 5465 616d 3a20 4875  anguage-Team: Hu
-000000c0: 6e67 6172 6961 6e0a 4d49 4d45 2d56 6572  ngarian.MIME-Ver
-000000d0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-000000e0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-000000f0: 696e 3b20 6368 6172 7365 743d 5554 462d  in; charset=UTF-
-00000100: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-00000110: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-00000120: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000130: 7079 6765 7474 6578 742e 7079 2031 2e35  pygettext.py 1.5
-00000140: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
-00000150: 706c 7572 616c 733d 323b 2070 6c75 7261  plurals=2; plura
-00000160: 6c3d 286e 2021 3d20 3129 3b0a 582d 4372  l=(n != 1);.X-Cr
-00000170: 6f77 6469 6e2d 5072 6f6a 6563 743a 2073  owdin-Project: s
-00000180: 7079 6465 722d 756e 6974 7465 7374 0a58  pyder-unittest.X
-00000190: 2d43 726f 7764 696e 2d50 726f 6a65 6374  -Crowdin-Project
-000001a0: 2d49 443a 2033 3831 3833 390a 582d 4372  -ID: 381839.X-Cr
-000001b0: 6f77 6469 6e2d 4c61 6e67 7561 6765 3a20  owdin-Language: 
-000001c0: 6875 0a58 2d43 726f 7764 696e 2d46 696c  hu.X-Crowdin-Fil
-000001d0: 653a 202f 6d61 7374 6572 2f73 7079 6465  e: /master/spyde
-000001e0: 725f 756e 6974 7465 7374 2f6c 6f63 616c  r_unittest/local
-000001f0: 652f 7370 7964 6572 5f75 6e69 7474 6573  e/spyder_unittes
-00000200: 742e 706f 740a 582d 4372 6f77 6469 6e2d  t.pot.X-Crowdin-
-00000210: 4669 6c65 2d49 443a 2034 390a 4c61 6e67  File-ID: 49.Lang
-00000220: 7561 6765 3a20 6875 5f48 550a 00         uage: hu_HU..
+000000b0: 616e 6775 6167 652d 5465 616d 3a20 4368  anguage-Team: Ch
+000000c0: 696e 6573 6520 5369 6d70 6c69 6669 6564  inese Simplified
+000000d0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
+000000e0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
+000000f0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
+00000100: 7273 6574 3d55 5446 2d38 0a43 6f6e 7465  rset=UTF-8.Conte
+00000110: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
+00000120: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
+00000130: 6174 6564 2d42 793a 2070 7967 6574 7465  ated-By: pygette
+00000140: 7874 2e70 7920 312e 350a 506c 7572 616c  xt.py 1.5.Plural
+00000150: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
+00000160: 3d31 3b20 706c 7572 616c 3d30 3b0a 582d  =1; plural=0;.X-
+00000170: 4372 6f77 6469 6e2d 5072 6f6a 6563 743a  Crowdin-Project:
+00000180: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
+00000190: 0a58 2d43 726f 7764 696e 2d50 726f 6a65  .X-Crowdin-Proje
+000001a0: 6374 2d49 443a 2033 3831 3833 390a 582d  ct-ID: 381839.X-
+000001b0: 4372 6f77 6469 6e2d 4c61 6e67 7561 6765  Crowdin-Language
+000001c0: 3a20 7a68 2d43 4e0a 582d 4372 6f77 6469  : zh-CN.X-Crowdi
+000001d0: 6e2d 4669 6c65 3a20 2f6d 6173 7465 722f  n-File: /master/
+000001e0: 7370 7964 6572 5f75 6e69 7474 6573 742f  spyder_unittest/
+000001f0: 6c6f 6361 6c65 2f73 7079 6465 725f 756e  locale/spyder_un
+00000200: 6974 7465 7374 2e70 6f74 0a58 2d43 726f  ittest.pot.X-Cro
+00000210: 7764 696e 2d46 696c 652d 4944 3a20 3439  wdin-File-ID: 49
+00000220: 0a4c 616e 6775 6167 653a 207a 685f 434e  .Language: zh_CN
+00000230: 0a00                                     ..
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/ja/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/ja/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
 00000020: 2c00 0000 f701 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
 000000b0: 616e 6775 6167 652d 5465 616d 3a20 4a61  anguage-Team: Ja
 000000c0: 7061 6e65 7365 0a4d 494d 452d 5665 7273  panese.MIME-Vers
 000000d0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
 000000e0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
 000000f0: 6e3b 2063 6861 7273 6574 3d55 5446 2d38  n; charset=UTF-8
 00000100: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/pl/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/pl/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
 00000020: 2c00 0000 8e02 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
 000000b0: 616e 6775 6167 652d 5465 616d 3a20 506f  anguage-Team: Po
 000000c0: 6c69 7368 0a4d 494d 452d 5665 7273 696f  lish.MIME-Versio
 000000d0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
 000000e0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
 000000f0: 2063 6861 7273 6574 3d55 5446 2d38 0a43   charset=UTF-8.C
 00000100: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/pt_BR/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/pt_BR/LC_MESSAGES/spyder_unittest.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: spyder-unittest\n"
-"POT-Creation-Date: 2022-09-03 17:43+0100\n"
-"PO-Revision-Date: 2022-09-03 20:06\n"
+"POT-Creation-Date: 2023-06-23 16:41+0100\n"
+"PO-Revision-Date: 2023-06-24 20:15\n"
 "Last-Translator: \n"
 "Language-Team: Portuguese, Brazilian\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -40,16 +40,16 @@
 
 msgid "Configure ..."
 msgstr "Configurar ..."
 
 msgid "Configure tests"
 msgstr "Configurar testes"
 
-msgid "Directory from which to run tests"
-msgstr "Diretório para execução dos testes"
+msgid "Directory from which to run tests:"
+msgstr "Diretório para execução dos testes:"
 
 msgid "Error"
 msgstr "Erro"
 
 msgid "Expand"
 msgstr "Expandir"
 
@@ -91,16 +91,16 @@
 
 msgid "Stop"
 msgstr "Parar"
 
 msgid "Stop current test process"
 msgstr "Parar processo de teste atual"
 
-msgid "Test framework"
-msgstr "Testar framework"
+msgid "Test framework:"
+msgstr "Testar framework:"
 
 msgid "Time (ms)"
 msgstr "Tempo (ms)"
 
 msgid "Unit testing"
 msgstr "Teste unitário"
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/locale/ru/LC_MESSAGES/spyder_unittest.mo` & `spyder_unittest-0.6.0/spyder_unittest/locale/ru/LC_MESSAGES/spyder_unittest.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: spyder-unittest*

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
 00000020: 2c00 0000 a202 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2073 7079 6465 722d 756e 6974 7465 7374   spyder-unittest
 00000050: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-00000060: 7465 3a20 3230 3232 2d30 392d 3033 2031  te: 2022-09-03 1
-00000070: 373a 3433 2b30 3130 300a 504f 2d52 6576  7:43+0100.PO-Rev
-00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3232  ision-Date: 2022
-00000090: 2d30 392d 3033 2032 303a 3036 0a4c 6173  -09-03 20:06.Las
+00000060: 7465 3a20 3230 3233 2d30 362d 3233 2031  te: 2023-06-23 1
+00000070: 363a 3431 2b30 3130 300a 504f 2d52 6576  6:41+0100.PO-Rev
+00000080: 6973 696f 6e2d 4461 7465 3a20 3230 3233  ision-Date: 2023
+00000090: 2d30 362d 3233 2032 303a 3137 0a4c 6173  -06-23 20:17.Las
 000000a0: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
 000000b0: 616e 6775 6167 652d 5465 616d 3a20 5275  anguage-Team: Ru
 000000c0: 7373 6961 6e0a 4d49 4d45 2d56 6572 7369  ssian.MIME-Versi
 000000d0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000000e0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000000f0: 3b20 6368 6172 7365 743d 5554 462d 380a  ; charset=UTF-8.
 00000100: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/tests/test_unittestplugin.py` & `spyder_unittest-0.6.0/spyder_unittest/tests/test_unittestplugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,155 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2017 Spyder Project Contributors
+# Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
-"""Tests for unittestplugin.py"""
+"""
+Tests for the integration of the plugin with Spyder.
+"""
+
+# Standard library imports
+from collections import OrderedDict
+import os
 
 # Third party imports
-import pytest
-from spyder.plugins.projects.api import EmptyProject
-from unittest.mock import MagicMock
+from qtpy.QtCore import Qt
+
+# Spyder imports
+from spyder.api.plugins import Plugins
 
 # Local imports
 from spyder_unittest.unittestplugin import UnitTestPlugin
 from spyder_unittest.widgets.configdialog import Config
 
 
-class PluginForTesting(UnitTestPlugin):
-    CONF_FILE = False
-
-    def __init__(self, parent):
-        UnitTestPlugin.__init__(self, parent)
-
-
-@pytest.fixture
-def plugin(qtbot):
-    """Set up the unittest plugin."""
-    res = UnitTestPlugin(None, None)
-    res._main = MagicMock()
-    res._main.get_spyder_pythonpath = MagicMock(return_value='fakepythonpath')
-    res.initialize()
-    return res
-
-
-@pytest.mark.skip('not clear how to test interactions between plugins')
-def test_plugin_initialization(plugin):
-    assert len(plugin.main.run_menu_actions) == 2
-    assert plugin.main.run_menu_actions[1].text() == 'Run unit tests'
-
-
-def test_plugin_pythonpath(plugin):
-    # Test signal/slot connection
-    plugin.get_main().sig_pythonpath_changed.connect.assert_called_with(
-        plugin.update_pythonpath)
-
-    # Test pythonpath is set to path provided by Spyder
-    assert plugin.get_widget().pythonpath == 'fakepythonpath'
-
-    # Test that change in path propagates
-    plugin.get_main().get_spyder_pythonpath = MagicMock(
-        return_value='anotherpath')
-    plugin.update_pythonpath()
-    assert plugin.get_widget().pythonpath == 'anotherpath'
-
-
-@pytest.mark.skip('not clear how to test interactions between plugins')
-def test_plugin_wdir(plugin, monkeypatch, tmpdir):
-    # Test signal/slot connections
-    plugin.main.workingdirectory.sig_current_directory_changed.connect.assert_called_with(
-        plugin.update_default_wdir)
-    plugin.main.projects.sig_project_created.connect.assert_called_with(
-        plugin.handle_project_change)
-    plugin.main.projects.sig_project_loaded.connect.assert_called_with(
-        plugin.handle_project_change)
-    plugin.main.projects.sig_project_closed.connect.assert_called_with(
-        plugin.handle_project_change)
-
-    # Test default_wdir is set to current working dir
-    monkeypatch.setattr('spyder_unittest.unittestplugin.getcwd',
-                        lambda: 'fakecwd')
-    plugin.update_default_wdir()
-    assert plugin.unittestwidget.default_wdir == 'fakecwd'
-
-    # Test after opening project, default_wdir is set to project dir
-    project = EmptyProject(str(tmpdir))
-    plugin.main.projects.get_active_project = lambda: project
-    plugin.main.projects.get_active_project_path = lambda: project.root_path
-    plugin.handle_project_change()
-    assert plugin.unittestwidget.default_wdir == str(tmpdir)
-
-    # Test after closing project, default_wdir is set back to cwd
-    plugin.main.projects.get_active_project = lambda: None
-    plugin.main.projects.get_active_project_path = lambda: None
-    plugin.handle_project_change()
-    assert plugin.unittestwidget.default_wdir == 'fakecwd'
-
+def test_menu_item(main_window):
+    """
+    Test that plugin adds item 'Run unit tests' to Run menu.
+    """
+    actions = main_window.run_menu_actions
+
+    # Filter out seperators (indicated by action is None) and convert to text
+    menu_items = [action.text() for action in actions if action]
+
+    assert 'Run unit tests' in menu_items
+
+
+def test_pythonpath_change(main_window):
+    """
+    Test that pythonpath changes in Spyder propagate to UnitTestWidget.
+    """
+    ppm = main_window.get_plugin(Plugins.PythonpathManager)
+    unittest_plugin = main_window.get_plugin(UnitTestPlugin.NAME)
+
+    new_path = '/some/path'
+    new_path_dict = OrderedDict([(new_path, True)])
+    ppm.get_container()._update_python_path(new_path_dict)
+
+    assert unittest_plugin.get_widget().pythonpath == [new_path]
+
+
+def test_default_working_dir(main_window, tmpdir):
+    """
+    Test that plugin's default working dir is current working directory.
+    After creating a project, the plugin's default working dir should be the
+    same as the project directory. When the project is closed again, the
+    plugin's default working dir should revert back to the current working
+    directory.
+    """
+    projects = main_window.get_plugin(Plugins.Projects)
+    unittest_plugin = main_window.get_plugin(UnitTestPlugin.NAME)
+    project_dir = str(tmpdir)
+
+    assert unittest_plugin.get_widget().default_wdir == os.getcwd()
+
+    projects._create_project(project_dir)
+    assert unittest_plugin.get_widget().default_wdir == project_dir
+
+    projects.close_project()
+    assert unittest_plugin.get_widget().default_wdir == os.getcwd()
+
+
+def test_plugin_config(main_window, tmpdir, qtbot):
+    """
+    Test that plugin uses the project's config file if a project is open.
+    """
+    projects = main_window.get_plugin(Plugins.Projects)
+    unittest_plugin = main_window.get_plugin(UnitTestPlugin.NAME)
+    unittest_widget = unittest_plugin.get_widget()
+    project_dir = str(tmpdir)
+    config_file_path = tmpdir.join('.spyproject', 'config', 'unittest.ini')
 
-@pytest.mark.skip('not clear how to test interactions between plugins')
-def test_plugin_config(plugin, tmpdir, qtbot):
     # Test config file does not exist and config is empty
-    config_file_path = tmpdir.join('.spyproject', 'config', 'unittest.ini')
     assert not config_file_path.check()
-    assert plugin.unittestwidget.config is None
+    assert unittest_widget.config is None
 
-    # Open project
-    project = EmptyProject(str(tmpdir))
-    plugin.main.projects.get_active_project = lambda: project
-    plugin.main.projects.get_active_project_path = lambda: project.root_path
-    plugin.handle_project_change()
+    # Create new project
+    projects._create_project(project_dir)
 
     # Test config file does exist but config is empty
     assert config_file_path.check()
     assert 'framework = ' in config_file_path.read().splitlines()
-    assert plugin.unittestwidget.config is None
+    assert unittest_widget.config is None
 
     # Set config and test that this is recorded in config file
     config = Config(framework='unittest', wdir=str(tmpdir))
-    with qtbot.waitSignal(plugin.unittestwidget.sig_newconfig):
-        plugin.unittestwidget.config = config
+    with qtbot.waitSignal(unittest_widget.sig_newconfig):
+        unittest_widget.config = config
     assert 'framework = unittest' in config_file_path.read().splitlines()
 
     # Close project and test that config is empty
-    plugin.main.projects.get_active_project = lambda: None
-    plugin.main.projects.get_active_project_path = lambda: None
-    plugin.handle_project_change()
-    assert plugin.unittestwidget.config is None
+    projects.close_project()
+    assert unittest_widget.config is None
 
     # Re-open project and test that config is correctly read
-    plugin.main.projects.get_active_project = lambda: project
-    plugin.main.projects.get_active_project_path = lambda: project.root_path
-    plugin.handle_project_change()
-    assert plugin.unittestwidget.config == config
+    projects.open_project(project_dir)
+    assert unittest_widget.config == config
+
+    # Close project before ending test, which removes the project dir
+    projects.close_project()
 
 
-@pytest.mark.skip('not clear how to test interactions between plugins')
-def test_plugin_goto_in_editor(plugin, qtbot):
-    plugin.unittestwidget.sig_edit_goto.emit('somefile', 42)
-    plugin.main.editor.load.assert_called_with('somefile', 43, '')
+def test_go_to_test_definition(main_window, tmpdir, qtbot):
+    """
+    Test that double clicking on a test result opens the file with the test
+    definition in the editor with the cursor on the test definition.
+    """
+    unittest_plugin = main_window.get_plugin(UnitTestPlugin.NAME)
+    unittest_widget = unittest_plugin.get_widget()
+    model = unittest_widget.testdatamodel
+    view = unittest_widget.testdataview
+
+    # Write test file
+    testdir_str = str(tmpdir)
+    testfile_str = tmpdir.join('test_foo.py').strpath
+    os.chdir(testdir_str)
+    with open(testfile_str, 'w') as f:
+        f.write("def test_ok(): assert 1+1 == 2\n"
+                "def test_fail(): assert 1+1 == 3\n")
+
+    # Run tests
+    config = Config(wdir=testdir_str, framework='pytest', coverage=False)
+    with qtbot.waitSignal(
+            unittest_widget.sig_finished, timeout=10000, raising=True):
+        unittest_widget.run_tests(config)
+
+    # Check that row 1 corresponds to `test_fail`
+    index = model.index(1, 1)
+    point = view.visualRect(index).center()
+    assert view.indexAt(point).data(Qt.DisplayRole).endswith('test_fail')
+
+    # Double click on `test_fail`
+    unittest_plugin.switch_to_plugin()
+    with qtbot.waitSignal(view.sig_edit_goto):
+        qtbot.mouseClick(view.viewport(), Qt.LeftButton, pos=point, delay=100)
+        qtbot.mouseDClick(view.viewport(), Qt.LeftButton, pos=point)
+
+    # Check that test file is opened in editor
+    editor = main_window.get_plugin(Plugins.Editor)
+    filename = editor.get_current_filename()
+    assert filename == testfile_str
+
+    # Check that cursor is on line defining `test_fail`
+    cursor = editor.get_current_editor().textCursor()
+    line = cursor.block().text()
+    assert line.startswith('def test_fail')
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/unittestplugin.py` & `spyder_unittest-0.6.0/spyder_unittest/unittestplugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,28 @@
 """Unit testing Plugin."""
 
 # Standard library imports
 from os import getcwd
 import os.path as osp
 
 # Third party imports
+import qtawesome
+from qtpy.QtCore import Qt
+
+# Spyder imports
 from spyder.api.plugins import Plugins, SpyderDockablePlugin
-from spyder.api.plugin_registration.decorators import on_plugin_available
+from spyder.api.plugin_registration.decorators import (
+    on_plugin_available, on_plugin_teardown)
 from spyder.config.base import get_translation
-from spyder.config.gui import is_dark_interface
 from spyder.plugins.mainmenu.api import ApplicationMenus
+from spyder.utils.palette import SpyderPalette
 
 # Local imports
 from spyder_unittest.widgets.configdialog import Config
+from spyder_unittest.widgets.confpage import UnitTestConfigPage
 from spyder_unittest.widgets.unittestgui import UnitTestWidget
 
 _ = get_translation('spyder_unittest')
 
 
 class UnitTestPluginActions:
     Run = 'Run tests'
@@ -29,25 +35,32 @@
 
 class UnitTestPlugin(SpyderDockablePlugin):
     """Spyder plugin for unit testing."""
 
     NAME = 'unittest'
     REQUIRES = []
     OPTIONAL = [Plugins.Editor, Plugins.MainMenu, Plugins.Preferences,
-                Plugins.Projects, Plugins.WorkingDirectory]
+                Plugins.Projects, Plugins.PythonpathManager,
+                Plugins.WorkingDirectory]
     TABIFY = [Plugins.VariableExplorer]
     WIDGET_CLASS = UnitTestWidget
 
     CONF_SECTION = NAME
     CONF_DEFAULTS = [(CONF_SECTION,
-                      {'framework': '', 'wdir': '', 'coverage': False})]
+                      {'framework': '',
+                       'wdir': '',
+                       'coverage': False,
+                       'abbrev_test_names': False}),
+                     ('shortcuts',
+                      {'unittest/Run tests': 'Alt+Shift+F11'})]
     CONF_NAMEMAP = {CONF_SECTION: [(CONF_SECTION,
                                     ['framework', 'wdir', 'coverage'])]}
     CONF_FILE = True
-    CONF_VERSION = '0.1.0'
+    CONF_VERSION = '0.2.0'
+    CONF_WIDGET_CLASS = UnitTestConfigPage
 
     # --- Mandatory SpyderDockablePlugin methods ------------------------------
 
     @staticmethod
     def get_name():
         """
         Return the plugin localized name.
@@ -75,32 +88,30 @@
         Return the plugin associated icon.
 
         Returns
         -------
         QIcon
             QIcon instance
         """
-        return self.create_icon('profiler')
+        return qtawesome.icon('mdi.test-tube', color=SpyderPalette.ICON_1)
 
     def on_initialize(self):
         """
         Setup the plugin.
         """
-        self.update_pythonpath()
-        self.get_main().sig_pythonpath_changed.connect(self.update_pythonpath)
         self.get_widget().sig_newconfig.connect(self.save_config)
 
         self.create_action(
             UnitTestPluginActions.Run,
             text=_('Run unit tests'),
             tip=_('Run unit tests'),
-            icon=self.create_icon('profiler'),
+            icon=self.get_icon(),
             triggered=self.maybe_configure_and_start,
+            context=Qt.ApplicationShortcut,
             register_shortcut=True)
-        #  TODO: shortcut="Shift+Alt+F11"
 
     # ----- Set up interactions with other plugins ----------------------------
 
     @on_plugin_available(plugin=Plugins.Editor)
     def on_editor_available(self):
         """
         Set up interactions when Editor plugin available.
@@ -112,70 +123,133 @@
         editor = self.get_plugin(Plugins.Editor)
         run_action = self.get_action(UnitTestPluginActions.Run)
         editor.pythonfile_dependent_actions += [run_action]
         # FIXME: Previous line does not do anything
         self.get_widget().pre_test_hook = editor.save_all
         self.get_widget().sig_edit_goto.connect(self.goto_in_editor)
 
+    @on_plugin_teardown(plugin=Plugins.Editor)
+    def on_editor_teardown(self):
+        """
+        Disconnect from Editor plugin.
+        """
+        self.get_widget().pre_test_hook = None
+        self.get_widget().sig_edit_goto.disconnect(self.goto_in_editor)
+
     @on_plugin_available(plugin=Plugins.MainMenu)
     def on_main_menu_available(self):
         """
         Add 'Run unit tests' menu item when MainMenu plugin available.
         """
         mainmenu = self.get_plugin(Plugins.MainMenu)
         run_action = self.get_action(UnitTestPluginActions.Run)
         mainmenu.add_item_to_application_menu(
             run_action, menu_id=ApplicationMenus.Run)
 
+    @on_plugin_teardown(plugin=Plugins.MainMenu)
+    def on_main_menu_teardown(self):
+        """
+        Remove 'Run unit tests; menu item from the application menu.
+        """
+        mainmenu = self.get_plugin(Plugins.MainMenu)
+        mainmenu.remove_item_from_application_menu(
+            UnitTestPluginActions.Run, menu_id=ApplicationMenus.Run)
+
     @on_plugin_available(plugin=Plugins.Preferences)
     def on_preferences_available(self):
         """
         Use config when Preferences plugin available.
 
-        Specifically, find out whether Spyder uses a dark interface and
-        communicate this to the unittest widget.
+        Specifically, register the unittest plugin preferences, and find out
+        whether Spyder uses a dark interface and communicate this to the
+        unittest widget.
+        """
+        preferences = self.get_plugin(Plugins.Preferences)
+        preferences.register_plugin_preferences(self)
+
+    @on_plugin_teardown(plugin=Plugins.Preferences)
+    def on_preferences_teardown(self):
         """
-        self.get_widget().use_dark_interface(is_dark_interface())
+        De-register unittest plugin preferences.
+        """
+        preferences = self.get_plugin(Plugins.Preferences)
+        preferences.deregister_plugin_preferences(self)
 
     @on_plugin_available(plugin=Plugins.Projects)
     def on_projects_available(self):
         """
         Connect when Projects plugin available.
 
         Connect to signals emitted when the current project changes.
         """
         projects = self.get_plugin(Plugins.Projects)
         projects.sig_project_created.connect(self.handle_project_change)
         projects.sig_project_loaded.connect(self.handle_project_change)
         projects.sig_project_closed.connect(self.handle_project_change)
 
+    @on_plugin_teardown(plugin=Plugins.Projects)
+    def on_projects_teardown(self):
+        """
+        Disconnect from Projects plugin.
+        """
+        projects = self.get_plugin(Plugins.Projects)
+        projects.sig_project_created.disconnect(self.handle_project_change)
+        projects.sig_project_loaded.disconnect(self.handle_project_change)
+        projects.sig_project_closed.disconnect(self.handle_project_change)
+
+    @on_plugin_available(plugin=Plugins.PythonpathManager)
+    def on_pythonpath_manager_available(self):
+        """
+        Connect to signal announcing that Python path changed.
+        """
+        ppm = self.get_plugin(Plugins.PythonpathManager)
+        ppm.sig_pythonpath_changed.connect(self.update_pythonpath)
+
+    @on_plugin_teardown(plugin=Plugins.PythonpathManager)
+    def on_pythonpath_manager_teardown(self):
+        """
+        Disconnect from PythonpathManager plugin.
+        """
+        ppm = self.get_plugin(Plugins.PythonpathManager)
+        ppm.sig_pythonpath_changed.disconnect(self.update_pythonpath)
+
     @on_plugin_available(plugin=Plugins.WorkingDirectory)
     def on_working_directory_available(self):
         """
         Connect when WorkingDirectory plugin available.
 
         Find out what the current working directory is and connect to the
         signal emitted when the current working directory changes.
         """
         working_directory = self.get_plugin(Plugins.WorkingDirectory)
         working_directory.sig_current_directory_changed.connect(
             self.update_default_wdir)
         self.update_default_wdir()
 
+    @on_plugin_teardown(plugin=Plugins.WorkingDirectory)
+    def on_working_directory_teardown(self):
+        """
+        Disconnect from WorkingDirectory plugin.
+        """
+        working_directory = self.get_plugin(Plugins.WorkingDirectory)
+        working_directory.sig_current_directory_changed.disconnect(
+            self.update_default_wdir)
+
     # --- UnitTestPlugin methods ----------------------------------------------
 
     def update_pythonpath(self):
         """
         Update Python path used to run unit tests.
 
         This function is called whenever the Python path set in Spyder changes.
         It synchronizes the Python path in the unittest widget with the Python
         path in Spyder.
         """
-        self.get_widget().pythonpath = self.get_main().get_spyder_pythonpath()
+        ppm = self.get_plugin(Plugins.PythonpathManager)
+        self.get_widget().pythonpath = ppm.get_spyder_pythonpath()
 
     def handle_project_change(self):
         """
         Handle the event where the current project changes.
 
         This updates the default working directory for running tests and loads
         the test configuration from the project preferences.
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/configdialog.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/configdialog.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,51 +5,63 @@
 # (see LICENSE.txt for details)
 """
 Functionality for asking the user to specify the test configuration.
 
 The main entry point is `ask_for_config()`.
 """
 
+from __future__ import annotations
+
 # Standard library imports
-from collections import namedtuple
 from os import getcwd
-from pkgutil import find_loader as find_spec_or_loader
 import os.path as osp
+import shlex
+from typing import Optional, NamedTuple
 
 # Third party imports
 from qtpy.compat import getexistingdirectory
 from qtpy.QtCore import Slot
-from qtpy.QtWidgets import (QApplication, QComboBox, QDialog, QDialogButtonBox,
-                            QHBoxLayout, QLabel, QLineEdit, QPushButton,
-                            QVBoxLayout, QCheckBox)
+from qtpy.QtWidgets import (
+    QApplication, QComboBox, QDialog, QDialogButtonBox, QGridLayout,
+    QHBoxLayout, QLabel, QLineEdit, QPushButton, QVBoxLayout, QCheckBox)
 from spyder.config.base import get_translation
 from spyder.utils import icon_manager as ima
 
 
 try:
     _ = get_translation('spyder_unittest')
 except KeyError:
     import gettext
     _ = gettext.gettext
 
-Config = namedtuple('Config', ['framework', 'wdir', 'coverage'])
-Config.__new__.__defaults__ = (None, '', False)
+class Config(NamedTuple):
+    framework: Optional[str] = None
+    wdir: str = ''
+    coverage: bool = False
+    args: list[str] = []
 
 
 class ConfigDialog(QDialog):
     """
     Dialog window for specifying test configuration.
 
     The window contains a combobox with all the frameworks, a line edit box for
     specifying the working directory, a button to use a file browser for
     selecting the directory, and OK and Cancel buttons. Initially, no framework
     is selected and the OK button is disabled. Selecting a framework enables
     the OK button.
     """
 
+    # Width of strut in the layout of the dialog window; this determines
+    # the width of the dialog
+    STRUT_WIDTH = 400
+
+    # Extra vertical space added between elements in the dialog
+    EXTRA_SPACE = 10
+
     def __init__(self, frameworks, config, versions, parent=None):
         """
         Construct a dialog window.
 
         Parameters
         ----------
         frameworks : dict of (str, type)
@@ -61,77 +73,102 @@
             Versions of testing frameworks and their plugins
         parent : QWidget
         """
         super().__init__(parent)
         self.versions = versions
         self.setWindowTitle(_('Configure tests'))
         layout = QVBoxLayout(self)
+        layout.addStrut(self.STRUT_WIDTH)
+
+        grid_layout = QGridLayout()
 
-        framework_layout = QHBoxLayout()
-        framework_label = QLabel(_('Test framework'))
-        framework_layout.addWidget(framework_label)
+        # Combo box for selecting the test framework
+
+        framework_label = QLabel(_('Test framework:'))
+        grid_layout.addWidget(framework_label, 0, 0)
 
         self.framework_combobox = QComboBox(self)
         for ix, (name, runner) in enumerate(sorted(frameworks.items())):
             installed = versions[name]['available']
             if installed:
                 label = name
             else:
                 label = '{} ({})'.format(name, _('not available'))
             self.framework_combobox.addItem(label)
             self.framework_combobox.model().item(ix).setEnabled(installed)
+        grid_layout.addWidget(self.framework_combobox, 0, 1)
+
+        # Line edit field for adding extra command-line arguments
+
+        args_label = QLabel(_('Command-line arguments:'))
+        grid_layout.addWidget(args_label, 1, 0)
+
+        self.args_lineedit = QLineEdit(self)
+        args_toolTip = _('Extra command-line arguments when running tests')
+        self.args_lineedit.setToolTip(args_toolTip)
+        grid_layout.addWidget(self.args_lineedit, 1, 1)
 
-        framework_layout.addWidget(self.framework_combobox)
-        layout.addLayout(framework_layout)
+        layout.addLayout(grid_layout)
+        spacing = grid_layout.verticalSpacing() + self.EXTRA_SPACE
+        grid_layout.setVerticalSpacing(spacing)
 
-        layout.addSpacing(10)
+        layout.addSpacing(self.EXTRA_SPACE)
+
+        # Checkbox for enabling coverage report
 
         coverage_label = _('Include coverage report in output')
         coverage_toolTip = _('Works only for pytest, requires pytest-cov')
         coverage_layout = QHBoxLayout()
         self.coverage_checkbox = QCheckBox(coverage_label, self)
         self.coverage_checkbox.setToolTip(coverage_toolTip)
         self.coverage_checkbox.setEnabled(False)
         coverage_layout.addWidget(self.coverage_checkbox)
         layout.addLayout(coverage_layout)
 
-        layout.addSpacing(10)
+        layout.addSpacing(self.EXTRA_SPACE)
+
+        # Line edit field for selecting directory
 
-        wdir_label = QLabel(_('Directory from which to run tests'))
+        wdir_label = QLabel(_('Directory from which to run tests:'))
         layout.addWidget(wdir_label)
         wdir_layout = QHBoxLayout()
         self.wdir_lineedit = QLineEdit(self)
         wdir_layout.addWidget(self.wdir_lineedit)
         self.wdir_button = QPushButton(ima.icon('DirOpenIcon'), '', self)
         self.wdir_button.setToolTip(_("Select directory"))
         self.wdir_button.clicked.connect(lambda: self.select_directory())
         wdir_layout.addWidget(self.wdir_button)
         layout.addLayout(wdir_layout)
 
-        layout.addSpacing(20)
+        layout.addSpacing(2 * self.EXTRA_SPACE)
+
+        # OK and Cancel buttons at the bottom
 
         self.buttons = QDialogButtonBox(QDialogButtonBox.Ok |
                                         QDialogButtonBox.Cancel)
         layout.addWidget(self.buttons)
         self.buttons.accepted.connect(self.accept)
         self.buttons.rejected.connect(self.reject)
 
         self.ok_button = self.buttons.button(QDialogButtonBox.Ok)
         self.ok_button.setEnabled(False)
         self.framework_combobox.currentIndexChanged.connect(
             self.framework_changed)
 
+        # Set initial values to agree with the given config
+
         self.framework_combobox.setCurrentIndex(-1)
         if config.framework:
             index = self.framework_combobox.findText(config.framework)
             if index != -1:
                 self.framework_combobox.setCurrentIndex(index)
-        self.wdir_lineedit.setText(config.wdir)
         self.coverage_checkbox.setChecked(config.coverage)
         self.enable_coverage_checkbox_if_available()
+        self.args_lineedit.setText(shlex.join(config.args))
+        self.wdir_lineedit.setText(config.wdir)
 
     @Slot(int)
     def framework_changed(self, index):
         """Called when selected framework changes."""
         if index != -1:
             self.ok_button.setEnabled(True)
             self.enable_coverage_checkbox_if_available()
@@ -169,16 +206,20 @@
         -------
         Config
             Test configuration
         """
         framework = self.framework_combobox.currentText()
         if framework == '':
             framework = None
+
+        args = self.args_lineedit.text()
+        args = shlex.split(args)
+
         return Config(framework=framework, wdir=self.wdir_lineedit.text(),
-                      coverage=self.coverage_checkbox.isChecked())
+                      coverage=self.coverage_checkbox.isChecked(), args=args)
 
 
 def ask_for_config(frameworks, config, versions, parent=None):
     """
     Ask user to specify a test configuration.
 
     This is a convenience function which displays a modal dialog window
@@ -188,10 +229,18 @@
     result = dialog.exec_()
     if result == QDialog.Accepted:
         return dialog.get_config()
 
 
 if __name__ == '__main__':
     app = QApplication([])
-    frameworks = ['nose', 'pytest', 'unittest']
-    config = Config(framework=None, wdir=getcwd(), coverage=False)
-    print(ask_for_config(frameworks, config))
+    frameworks = {
+        'nose2': object,
+        'unittest': object,
+        'pytest': object}
+    versions = {
+        'nose2': {'available': False},
+        'unittest': {'available': True},
+        'pytest': {'available': True, 'plugins': {'pytest-cov', '3.1.4'}}
+    }
+    config = Config(wdir=getcwd())
+    print(ask_for_config(frameworks, config, versions))
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/datatree.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/datatree.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,41 +10,35 @@
 from operator import attrgetter
 
 # Third party imports
 from qtpy import PYQT4
 from qtpy.QtCore import QAbstractItemModel, QModelIndex, Qt, Signal
 from qtpy.QtGui import QBrush, QColor, QFont
 from qtpy.QtWidgets import QMenu, QTreeView
+from spyder.api.config.mixins import SpyderConfigurationAccessor
 from spyder.config.base import get_translation
+from spyder.utils.palette import QStylePalette, SpyderPalette
 from spyder.utils.qthelpers import create_action
 
 # Local imports
 from spyder_unittest.backend.abbreviator import Abbreviator
 from spyder_unittest.backend.runnerbase import Category
 
 try:
     _ = get_translation('spyder_unittest')
 except KeyError:
     import gettext
     _ = gettext.gettext
 
 COLORS = {
-    Category.OK: QBrush(QColor("#C1FFBA")),
-    Category.FAIL: QBrush(QColor("#FF5050")),
-    Category.SKIP: QBrush(QColor("#C5C5C5")),
-    Category.PENDING: QBrush(QColor("#C5C5C5")),
-    Category.COVERAGE: QBrush(QColor("#89CFF0"))
-}
-
-COLORS_DARK = {
-    Category.OK: QBrush(QColor("#008000")),
-    Category.FAIL: QBrush(QColor("#C6001E")),
-    Category.SKIP: QBrush(QColor("#505050")),
-    Category.PENDING: QBrush(QColor("#505050")),
-    Category.COVERAGE: QBrush(QColor("#0047AB"))
+    Category.OK:       SpyderPalette.COLOR_SUCCESS_1,
+    Category.FAIL:     SpyderPalette.COLOR_ERROR_1,
+    Category.SKIP:     SpyderPalette.COLOR_WARN_1,
+    Category.PENDING:  QStylePalette.COLOR_BACKGROUND_1,
+    Category.COVERAGE: QStylePalette.COLOR_ACCENT_1
 }
 
 STATUS_COLUMN = 0
 NAME_COLUMN = 1
 MESSAGE_COLUMN = 2
 TIME_COLUMN = 3
 
@@ -57,17 +51,21 @@
     """
     Tree widget displaying test results.
 
     Signals
     -------
     sig_edit_goto(str, int): Emitted if editor should go to some position.
         Arguments are file name and line number (zero-based).
+    sig_single_test_run_requested(str): Emitted to request a single test
+        to be run. Argument is the name of the test.
     """
 
     sig_edit_goto = Signal(str, int)
+    sig_single_test_run_requested = Signal(str)
+
     __test__ = False  # this is not a pytest test class
 
     def __init__(self, parent=None):
         """Constructor."""
         QTreeView.__init__(self, parent)
         self.header().setDefaultAlignment(Qt.AlignCenter)
         self.setItemsExpandable(True)
@@ -122,14 +120,21 @@
         index = self.make_index_canonical(index)
         filename, lineno = self.model().data(index, Qt.UserRole)
         if filename is not None:
             if lineno is None:
                 lineno = 0
             self.sig_edit_goto.emit(filename, lineno)
 
+    def run_single_test(self, index):
+        """Ask plugin to run only the test corresponding to index."""
+        index = self.make_index_canonical(index)
+        testresult = self.model().testresults[index.row()]
+        testname = testresult.name
+        self.sig_single_test_run_requested.emit(testname)
+
     def make_index_canonical(self, index):
         """
         Convert given index to canonical index for the same test.
 
         For every test, the canonical index points to the item on the top level
         in the first column corresponding to the given position. If the given
         index is invalid, then return None.
@@ -148,20 +153,29 @@
             menuItem = create_action(self, _('Collapse'),
                                      triggered=lambda: self.collapse(index))
         else:
             menuItem = create_action(self, _('Expand'),
                                      triggered=lambda: self.expand(index))
             menuItem.setEnabled(self.model().hasChildren(index))
         contextMenu.addAction(menuItem)
+
         menuItem = create_action(
                 self, _('Go to definition'),
                 triggered=lambda: self.go_to_test_definition(index))
         test_location = self.model().data(index, Qt.UserRole)
         menuItem.setEnabled(test_location[0] is not None)
         contextMenu.addAction(menuItem)
+
+        menuItem = create_action(
+                self, _('Run only this test'),
+                triggered=lambda: self.run_single_test(index))
+        result_category = self.model().testresults[index.row()].category
+        menuItem.setEnabled(result_category != Category.COVERAGE)
+        contextMenu.addAction(menuItem)
+
         return contextMenu
 
     def resizeColumns(self):
         """Resize column to fit their contents."""
         for col in range(self.model().columnCount()):
             self.resizeColumnToContents(col)
 
@@ -182,45 +196,41 @@
         model = self.model()
         for row in range(firstRow, lastRow + 1):
             index = model.index(row, 0)
             for i in range(model.rowCount(index)):
                 self.setFirstColumnSpanned(i, index, True)
 
 
-class TestDataModel(QAbstractItemModel):
+class TestDataModel(QAbstractItemModel, SpyderConfigurationAccessor):
     """
     Model class storing test results for display.
 
     Test results are stored as a list of TestResults in the property
     `self.testresults`. Every test is exposed as a child of the root node,
     with extra information as second-level nodes.
 
     As in every model, an iteem of data is identified by its index, which is
     a tuple (row, column, id). The id is TOPLEVEL_ID for top-level items.
     For level-2 items, the id is the index of the test in `self.testresults`.
 
-    Attributes
-    ----------
-    is_dark_interface : bool
-        Whether to use colours appropriate for a dark user interface.
-
     Signals
     -------
     sig_summary(str)
        Emitted with new summary if test results change.
     """
 
+    CONF_SECTION = 'unittest'
+
     sig_summary = Signal(str)
     __test__ = False  # this is not a pytest test class
 
     def __init__(self, parent=None):
         """Constructor."""
         QAbstractItemModel.__init__(self, parent)
         self.abbreviator = Abbreviator()
-        self.is_dark_interface = False
         self.testresults = []
         try:
             self.monospace_font = parent.window().editor.get_plugin_font()
         except AttributeError:  # If run standalone for testing
             self.monospace_font = QFont("Courier New")
             self.monospace_font.setPointSize(10)
 
@@ -317,36 +327,38 @@
         id = index.internalId()
         if role == Qt.DisplayRole:
             if id != TOPLEVEL_ID:
                 return self.testresults[id].extra_text[index.row()]
             elif column == STATUS_COLUMN:
                 return self.testresults[row].status
             elif column == NAME_COLUMN:
+                name = self.testresults[row].name
                 # don't abbreviate for the code coverage filename
                 if self.testresults[row].category == Category.COVERAGE:
-                    return self.testresults[row].name
-                return self.abbreviator.abbreviate(self.testresults[row].name)
+                    return name
+                if self.get_conf('abbrev_test_names', False):
+                    return self.abbreviator.abbreviate(name)
+                else:
+                    return name
             elif column == MESSAGE_COLUMN:
                 return self.testresults[row].message
             elif column == TIME_COLUMN:
                 time = self.testresults[row].time
                 return '' if time is None else '{:.2f}'.format(time * 1e3)
         elif role == Qt.ToolTipRole:
             if id == TOPLEVEL_ID and column == NAME_COLUMN:
                 return self.testresults[row].name
         elif role == Qt.FontRole:
             if id != TOPLEVEL_ID:
                 return self.monospace_font
         elif role == Qt.BackgroundRole:
             if id == TOPLEVEL_ID:
                 testresult = self.testresults[row]
-                if self.is_dark_interface:
-                    return COLORS_DARK[testresult.category]
-                else:
-                    return COLORS[testresult.category]
+                color = COLORS[testresult.category]
+                return QBrush(QColor(color))
         elif role == Qt.TextAlignmentRole:
             if id == TOPLEVEL_ID and column == TIME_COLUMN:
                 return Qt.AlignRight
         elif role == Qt.UserRole:
             if id == TOPLEVEL_ID:
                 testresult = self.testresults[row]
                 return (testresult.filename, testresult.lineno)
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_configdialog.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_configdialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'spam': {'available': False},
     'ham': {'available': True},
     'pytest': {'available': True, 'plugins': {'pytest-cov', '3.1.4'}}
 }
 
 
 def default_config():
-    return Config(framework=None, wdir=os.getcwd(), coverage=False)
+    return Config(framework=None, wdir=os.getcwd(), coverage=False, args=[])
 
 
 def test_configdialog_uses_frameworks(qtbot):
     configdialog = ConfigDialog(
         {'ham': HamRunner}, default_config(), versions)
     assert configdialog.framework_combobox.count() == 1
     assert configdialog.framework_combobox.itemText(0) == 'ham'
@@ -72,20 +72,21 @@
     model = configdialog.framework_combobox.model()
     assert model.item(0).isEnabled()  # ham
     assert model.item(1).isEnabled()  # pytest
     assert not model.item(2).isEnabled()  # spam
 
 
 def test_configdialog_sets_initial_config(qtbot):
-    config = default_config()
+    config = Config(framework='pytest', wdir='/some/dir',
+                    coverage=True, args=['some', 'arg'])
     configdialog = ConfigDialog(frameworks, config, versions)
     assert configdialog.get_config() == config
 
 
-def test_configdialog_click_ham(qtbot):
+def test_configdialog_click_pytest(qtbot):
     configdialog = ConfigDialog(frameworks, default_config(), versions)
     qtbot.addWidget(configdialog)
     configdialog.framework_combobox.setCurrentIndex(1)
     assert configdialog.get_config().framework == 'pytest'
 
 
 def test_configdialog_ok_initially_disabled(qtbot):
@@ -121,14 +122,21 @@
     local_versions['pytest']['plugins'] = {}
     configdialog = ConfigDialog(frameworks, default_config(), local_versions)
     qtbot.addWidget(configdialog)
     configdialog.framework_combobox.setCurrentIndex(1)
     assert configdialog.coverage_checkbox.isEnabled() is False
 
 
+def test_configdialog_args_lineedit(qtbot):
+    configdialog = ConfigDialog(frameworks, default_config(), versions)
+    qtbot.addWidget(configdialog)
+    configdialog.args_lineedit.setText('-x "ham and" spam')
+    assert configdialog.get_config().args == ['-x', 'ham and', 'spam']
+
+
 def test_configdialog_wdir_lineedit(qtbot):
     configdialog = ConfigDialog(frameworks, default_config(), versions)
     qtbot.addWidget(configdialog)
     wdir = os.path.normpath(os.path.join(os.getcwd(), os.path.pardir))
     configdialog.wdir_lineedit.setText(wdir)
     assert configdialog.get_config().wdir == wdir
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_datatree.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_datatree.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # Copyright © 2017 Spyder Project Contributors
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Tests for unittestgui.py."""
 
 # Third party imports
 from qtpy.QtCore import QModelIndex, QPoint, Qt
-from qtpy.QtGui import QContextMenuEvent
+from qtpy.QtGui import QBrush, QColor, QContextMenuEvent
 from unittest.mock import Mock
 import pytest
 
 # Local imports
 from spyder_unittest.backend.runnerbase import Category, TestResult
-from spyder_unittest.widgets.datatree import (COLORS, COLORS_DARK,
-                                              TestDataModel, TestDataView)
+from spyder_unittest.widgets.datatree import (
+    COLORS, TestDataModel, TestDataView)
 
 
 @pytest.fixture
 def view_and_model(qtbot):
     view = TestDataView()
     model = TestDataModel()
     # setModel() before populating testresults because setModel() does a sort
@@ -63,14 +63,20 @@
     res = model.testresults
     res[1].lineno = None
     model.testresults = res
     with qtbot.waitSignal(view.sig_edit_goto) as blocker:
         view.go_to_test_definition(model.index(1, 0))
     assert blocker.args == ['ham.py', 0]
 
+def test_run_single_test(view_and_model, qtbot):
+    view, model = view_and_model
+    with qtbot.waitSignal(view.sig_single_test_run_requested) as blocker:
+        view.run_single_test(model.index(1, 0))
+    assert blocker.args == ['foo.bar']
+
 def test_make_index_canonical_with_index_in_column2(view_and_model):
     view, model = view_and_model
     index = model.index(1, 2)
     res = view.make_index_canonical(index)
     assert res == model.index(1, 0)
 
 def test_make_index_canonical_with_level2_index(view_and_model):
@@ -84,28 +90,41 @@
     index = QModelIndex()
     res = view.make_index_canonical(index)
     assert res is None
 
 def test_build_context_menu(view_and_model):
     view, model = view_and_model
     menu = view.build_context_menu(model.index(0, 0))
+    assert len(menu.actions()) == 3
     assert menu.actions()[0].text() == 'Expand'
     assert menu.actions()[1].text() == 'Go to definition'
+    assert menu.actions()[2].text() == 'Run only this test'
 
 def test_build_context_menu_with_disabled_entries(view_and_model):
     view, model = view_and_model
     menu = view.build_context_menu(model.index(0, 0))
     assert menu.actions()[0].isEnabled() == False
     assert menu.actions()[1].isEnabled() == False
+    assert menu.actions()[2].isEnabled() == True
 
 def test_build_context_menu_with_enabled_entries(view_and_model):
     view, model = view_and_model
     menu = view.build_context_menu(model.index(1, 0))
     assert menu.actions()[0].isEnabled() == True
     assert menu.actions()[1].isEnabled() == True
+    assert menu.actions()[2].isEnabled() == True
+
+def test_build_context_menu_with_coverage_entry(view_and_model):
+    view, model = view_and_model
+    testresult = TestResult(Category.COVERAGE, 'coverage', 'foo')
+    model.testresults.append(testresult)
+    menu = view.build_context_menu(model.index(2, 0))
+    assert menu.actions()[0].isEnabled() == False
+    assert menu.actions()[1].isEnabled() == False
+    assert menu.actions()[2].isEnabled() == False
 
 def test_build_context_menu_with_expanded_entry(view_and_model):
     view, model = view_and_model
     view.expand(model.index(1, 0))
     menu = view.build_context_menu(model.index(1, 0))
     assert menu.actions()[0].text() == 'Collapse'
     assert menu.actions()[0].isEnabled() == True
@@ -114,20 +133,25 @@
     model = TestDataModel()
     res = [TestResult(Category.OK, 'status', 'foo.bar'),
            TestResult(Category.FAIL, 'error', 'foo.bar', 'kadoom', 0,
                       'crash!\nboom!')]
     model.testresults = res
     qtmodeltester.check(model)
 
-def test_testdatamodel_shows_abbreviated_name_in_table(qtbot):
+@pytest.mark.parametrize('config, result',
+                         [(False, 'foo.bar'), (True, 'f.bar')])
+def test_testdatamodel_shows_abbreviated_name_in_table(qtbot, config, result):
     model = TestDataModel()
+    old_config = model.get_conf('abbrev_test_names')
+    model.set_conf('abbrev_test_names', config)
     res = TestResult(Category.OK, 'status', 'foo.bar', '', 0, '')
     model.testresults = [res]
     index = model.index(0, 1)
-    assert model.data(index, Qt.DisplayRole) == 'f.bar'
+    assert model.data(index, Qt.DisplayRole) == result
+    model.set_conf('abbrev_test_names', old_config)
 
 def test_testdatamodel_shows_full_name_in_tooltip(qtbot):
     model = TestDataModel()
     res = TestResult(Category.OK, 'status', 'foo.bar', '', 0, '')
     model.testresults = [res]
     index = model.index(0, 1)
     assert model.data(index, Qt.ToolTipRole) == 'foo.bar'
@@ -148,27 +172,25 @@
 
 def test_testdatamodel_shows_time_when_blank(qtmodeltester):
     model = TestDataModel()
     res = TestResult(Category.OK, 'status', 'foo.bar')
     model.testresults = [res]
     assert model.data(model.index(0, 3), Qt.DisplayRole) == ''
 
-@pytest.mark.parametrize('dark', [False, True])
-def test_testdatamodel_data_background(dark):
+def test_testdatamodel_data_background():
     model = TestDataModel()
-    if dark:
-        model.is_dark_interface = True
     res = [TestResult(Category.OK, 'status', 'foo.bar'),
            TestResult(Category.FAIL, 'error', 'foo.bar', 'kadoom')]
     model.testresults = res
     index = model.index(0, 0)
-    colors = COLORS_DARK if dark else COLORS
-    assert model.data(index, Qt.BackgroundRole) == colors[Category.OK]
+    expected = QBrush(QColor(COLORS[Category.OK]))
+    assert model.data(index, Qt.BackgroundRole) == expected
     index = model.index(1, 2)
-    assert model.data(index, Qt.BackgroundRole) == colors[Category.FAIL]
+    expected = QBrush(QColor(COLORS[Category.FAIL]))
+    assert model.data(index, Qt.BackgroundRole) == expected
 
 def test_testdatamodel_data_userrole():
     model = TestDataModel()
     res = [TestResult(Category.OK, 'status', 'foo.bar', filename='somefile',
                       lineno=42)]
     model.testresults = res
     index = model.index(0, 0)
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/tests/test_unittestgui.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/tests/test_unittestgui.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Licensed under the terms of the MIT License
 # (see LICENSE.txt for details)
 """Tests for unittestgui.py."""
 
 # Standard library imports
 import os
 import sys
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 
 # Third party imports
 from qtpy.QtCore import Qt, QProcess
 import pytest
 
 # Local imports
 from spyder_unittest.backend.runnerbase import (Category, TestResult,
@@ -147,48 +147,60 @@
     assert widget.status_label.text() == '<b>{}</b>'.format(label)
 
 def test_unittestwidget_process_finished_abnormally_status_label(widget):
     widget.process_finished([], 'output', False)
     expected_text = '<b>{}</b>'.format('Test process exited abnormally')
     assert widget.status_label.text() == expected_text
 
-@pytest.mark.parametrize('framework', ['pytest', 'nose'])
-def test_run_tests_and_display_results(qtbot, widget, tmpdir, monkeypatch, framework):
+def test_unittestwidget_handles_sig_single_test_run_requested(widget):
+    with patch.object(widget, 'run_tests') as mock_run_tests:
+        widget.testdataview.sig_single_test_run_requested.emit('testname')
+        mock_run_tests.assert_called_once_with(single_test='testname')
+
+@pytest.mark.parametrize('framework', ['pytest', 'nose2'])
+@pytest.mark.parametrize('alltests', [True, False])
+def test_run_tests_and_display_results(qtbot, widget, tmpdir, monkeypatch,
+                                       framework, alltests):
     """Basic integration test."""
     os.chdir(tmpdir.strpath)
     testfilename = tmpdir.join('test_foo.py').strpath
 
     with open(testfilename, 'w') as f:
-        f.write("def test_ok(): assert 1+1 == 2\n"
-                "def test_fail(): assert 1+1 == 3\n")
+        f.write("def test_fail(): assert 1+1 == 3\n"
+                "def test_ok(): assert 1+1 == 2\n")
 
     MockQMessageBox = Mock()
     monkeypatch.setattr('spyder_unittest.widgets.unittestgui.QMessageBox',
                         MockQMessageBox)
 
     config = Config(wdir=tmpdir.strpath, framework=framework, coverage=False)
     with qtbot.waitSignal(widget.sig_finished, timeout=10000, raising=True):
-        widget.run_tests(config)
+        if alltests:
+            widget.run_tests(config)
+        else:
+            widget.run_tests(config, single_test='test_foo.test_fail')
 
     MockQMessageBox.assert_not_called()
     model = widget.testdatamodel
-    assert model.rowCount() == 2
+    assert model.rowCount() == (2 if alltests else 1)
     assert model.index(0, 0).data(
-        Qt.DisplayRole) == 'ok' if framework == 'nose' else 'passed'
-    assert model.index(0, 1).data(Qt.DisplayRole) == 't.test_ok'
-    assert model.index(0, 1).data(Qt.ToolTipRole) == 'test_foo.test_ok'
-    assert model.index(0, 2).data(Qt.DisplayRole) == ''
-    assert model.index(1, 0).data(
-        Qt.DisplayRole) == 'failure' if framework == 'nose' else 'failed'
-    assert model.index(1, 1).data(Qt.DisplayRole) == 't.test_fail'
-    assert model.index(1, 1).data(Qt.ToolTipRole) == 'test_foo.test_fail'
+        Qt.DisplayRole) == 'failure' if framework == 'nose2' else 'failed'
+    assert model.index(0, 1).data(Qt.DisplayRole) == 'test_foo.test_fail'
+    assert model.index(0, 1).data(Qt.ToolTipRole) == 'test_foo.test_fail'
+    if alltests:
+        assert model.index(1, 0).data(
+            Qt.DisplayRole) == 'ok' if framework == 'nose2' else 'passed'
+        assert model.index(1, 1).data(Qt.DisplayRole) == 'test_foo.test_ok'
+        assert model.index(1, 1).data(Qt.ToolTipRole) == 'test_foo.test_ok'
+        assert model.index(1, 2).data(Qt.DisplayRole) == ''
 
 
+@pytest.mark.parametrize('alltests', [True, False])
 def test_run_tests_using_unittest_and_display_results(
-        qtbot, widget, tmpdir, monkeypatch):
+        qtbot, widget, tmpdir, monkeypatch, alltests):
     """Basic check."""
     os.chdir(tmpdir.strpath)
     testfilename = tmpdir.join('test_foo.py').strpath
 
     with open(testfilename, 'w') as f:
         f.write("import unittest\n"
                 "class MyTest(unittest.TestCase):\n"
@@ -197,29 +209,65 @@
 
     MockQMessageBox = Mock()
     monkeypatch.setattr('spyder_unittest.widgets.unittestgui.QMessageBox',
                         MockQMessageBox)
 
     config = Config(wdir=tmpdir.strpath, framework='unittest', coverage=False)
     with qtbot.waitSignal(widget.sig_finished, timeout=10000, raising=True):
+        if alltests:
+            widget.run_tests(config)
+        else:
+            widget.run_tests(config, single_test='test_foo.MyTest.test_fail')
+
+    MockQMessageBox.assert_not_called()
+    model = widget.testdatamodel
+    assert model.rowCount() == (2 if alltests else 1)
+    assert model.index(0, 0).data(Qt.DisplayRole) == 'failure'
+    assert model.index(0, 1).data(Qt.DisplayRole) == 'test_foo.MyTest.test_fail'
+    assert model.index(0, 1).data(Qt.ToolTipRole) == 'test_foo.MyTest.test_fail'
+    if alltests:
+        assert model.index(1, 0).data(Qt.DisplayRole) == 'success'
+        assert model.index(1, 1).data(Qt.DisplayRole) == 'test_foo.MyTest.test_ok'
+        assert model.index(1, 1).data(Qt.ToolTipRole) == 'test_foo.MyTest.test_ok'
+        assert model.index(1, 2).data(Qt.DisplayRole) == ''
+
+def test_run_tests_with_print_using_unittest_and_display_results(
+        qtbot, widget, tmpdir, monkeypatch):
+    """
+    Run a failing test which print to stderr using unittest and check
+    that it is displayed as a failing test.
+    Regression test for spyder-ide/spyder-unittest#160.
+    """
+    os.chdir(tmpdir.strpath)
+    testfilename = tmpdir.join('test_foo.py').strpath
+
+    with open(testfilename, 'w') as f:
+        f.write("import sys\n"
+                "import unittest\n"
+                "class MyTest(unittest.TestCase):\n"
+                "    def test_fail(self):\n"
+                "        print('text', file=sys.stderr)\n"
+                "        self.assertEqual(1+1, 3)\n"
+                "    def test_ok(self): self.assertEqual(1+1, 2)\n")
+
+    MockQMessageBox = Mock()
+    monkeypatch.setattr('spyder_unittest.widgets.unittestgui.QMessageBox',
+                        MockQMessageBox)
+
+    config = Config(wdir=tmpdir.strpath, framework='unittest', coverage=False)
+    with qtbot.waitSignal(widget.sig_finished, timeout=10000, raising=True):
         widget.run_tests(config)
 
     MockQMessageBox.assert_not_called()
     model = widget.testdatamodel
     assert model.rowCount() == 2
-    assert model.index(0, 0).data(Qt.DisplayRole) == 'FAIL'
-    assert model.index(0, 1).data(Qt.DisplayRole) == 't.M.test_fail'
-    assert model.index(0, 1).data(Qt.ToolTipRole) == 'test_foo.MyTest.test_fail'
-    assert model.index(0, 2).data(Qt.DisplayRole) == ''
-    assert model.index(1, 0).data(Qt.DisplayRole) == 'ok'
-    assert model.index(1, 1).data(Qt.DisplayRole) == 't.M.test_ok'
-    assert model.index(1, 1).data(Qt.ToolTipRole) == 'test_foo.MyTest.test_ok'
-    assert model.index(1, 2).data(Qt.DisplayRole) == ''
+    assert model.index(0, 0).data(Qt.DisplayRole) == 'failure'
+    assert model.index(1, 0).data(Qt.DisplayRole) == 'success'
 
-@pytest.mark.parametrize('framework', ['unittest', 'pytest', 'nose'])
+@pytest.mark.parametrize('framework', ['unittest', 'pytest', 'nose2'])
 def test_run_with_no_tests_discovered_and_display_results(
         qtbot, widget, tmpdir, monkeypatch, framework):
     """Basic integration test."""
     os.chdir(tmpdir.strpath)
 
     MockQMessageBox = Mock()
     monkeypatch.setattr('spyder_unittest.widgets.unittestgui.QMessageBox',
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest/widgets/unittestgui.py` & `spyder_unittest-0.6.0/spyder_unittest/widgets/unittestgui.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 from spyder.api.widgets.main_widget import PluginMainWidget
 from spyder.config.base import get_conf_path, get_translation
 from spyder.utils import icon_manager as ima
 from spyder.plugins.variableexplorer.widgets.texteditor import TextEditor
 
 # Local imports
 from spyder_unittest.backend.frameworkregistry import FrameworkRegistry
-from spyder_unittest.backend.noserunner import NoseRunner
+from spyder_unittest.backend.nose2runner import Nose2Runner
 from spyder_unittest.backend.pytestrunner import PyTestRunner
 from spyder_unittest.backend.runnerbase import Category, TestResult
 from spyder_unittest.backend.unittestrunner import UnittestRunner
 from spyder_unittest.widgets.configdialog import Config, ask_for_config
 from spyder_unittest.widgets.datatree import TestDataModel, TestDataView
 
 # This is needed for testing this module as a stand alone script
 try:
     _ = get_translation('spyder_unittest')
 except KeyError:
     import gettext
     _ = gettext.gettext
 
 # Supported testing frameworks
-FRAMEWORKS = {NoseRunner, PyTestRunner, UnittestRunner}
+FRAMEWORKS = {Nose2Runner, PyTestRunner, UnittestRunner}
 
 
 class UnitTestWidgetActions:
     RunTests = 'run_tests'
     Config = 'config'
     ShowLog = 'show_log'
     CollapseAll = 'collapse_all'
@@ -113,14 +113,16 @@
         self.pythonpath = None
         self.testrunner = None
 
         self.testdataview = TestDataView(self)
         self.testdatamodel = TestDataModel(self)
         self.testdataview.setModel(self.testdatamodel)
         self.testdataview.sig_edit_goto.connect(self.sig_edit_goto)
+        self.testdataview.sig_single_test_run_requested.connect(
+            self.run_single_test)
         self.testdatamodel.sig_summary.connect(self.set_status_label)
 
         self.framework_registry = FrameworkRegistry()
         for runner in FRAMEWORKS:
             self.framework_registry.register(runner)
 
         layout = QVBoxLayout()
@@ -234,18 +236,14 @@
         if self.config_is_valid():
             self.sig_newconfig.emit(new_config)
 
     def set_config_without_emit(self, new_config):
         """Set test configuration but do not emit any signal."""
         self._config = new_config
 
-    def use_dark_interface(self, flag):
-        """Set whether widget should use colours appropriate for dark UI."""
-        self.testdatamodel.is_dark_interface = flag
-
     def show_log(self):
         """Show output of testing process."""
         if self.output:
             te = TextEditor(
                 self.output,
                 title=_("Unit testing output"),
                 readonly=True,
@@ -337,31 +335,35 @@
         then ask the user to configure. Then run the tests.
         """
         if not self.config_is_valid():
             self.configure()
         if self.config_is_valid():
             self.run_tests()
 
-    def run_tests(self, config=None):
+    def run_tests(self, config=None, single_test=None):
         """
         Run unit tests.
 
         First, run `self.pre_test_hook` if it is set, and abort if its return
         value is `False`.
 
-        Then, run the unit tests.
+        Then, run the unit tests. If `single_test` is not None, then only run
+        that test.
 
         The process's output is consumed by `read_output()`.
         When the process finishes, the `finish` signal is emitted.
 
         Parameters
         ----------
         config : Config or None
             configuration for unit tests. If None, use `self.config`.
             In either case, configuration should be valid.
+        single_test : str or None
+            If None, run all tests; otherwise, it is the name of the only test
+            to be run.
         """
         if self.pre_test_hook:
             if self.pre_test_hook() is False:
                 return
 
         if config is None:
             config = self.config
@@ -380,15 +382,16 @@
 
         cov_path = self.get_conf('current_project_path', default='None',
                                  section='project_explorer')
         # config returns 'None' as a string rather than None
         cov_path = config.wdir if cov_path == 'None' else cov_path
         executable = self.get_conf('executable', section='main_interpreter')
         try:
-            self.testrunner.start(config, cov_path, executable, pythonpath)
+            self.testrunner.start(
+                config, cov_path, executable, pythonpath, single_test)
         except RuntimeError:
             QMessageBox.critical(self,
                                  _("Error"), _("Process failed to start"))
         else:
             self.set_running_state(True)
             self.set_status_label(_('Running tests ...'))
 
@@ -494,14 +497,20 @@
 
         Arguments
         ---------
         msg: str
         """
         self.status_label.setText('<b>{}</b>'.format(msg))
 
+    def run_single_test(self, test_name: str) -> None:
+        """
+        Run a single test with the given name.
+        """
+        self.run_tests(single_test=test_name)
+
 
 def test():
     """
     Run widget test.
 
     Show the unittest widgets, configured so that our own tests are run when
     the user clicks "Run tests".
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest.egg-info/PKG-INFO` & `spyder_unittest-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
-Name: spyder-unittest
-Version: 0.5.1
+Name: spyder_unittest
+Version: 0.6.0
 Summary: Plugin to run tests from within the Spyder IDE
 Home-page: https://github.com/spyder-ide/spyder-unittest
 Author: Spyder Project Contributors
 License: MIT
 Keywords: Qt PyQt4 PyQt5 spyder plugins testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 
 This is a plugin for the Spyder IDE that integrates popular unit test
 frameworks. It allows you to run tests and view the results.
 
 The plugin supports the `unittest` framework in the Python
-standard library and the `pytest` and `nose` testing frameworks.
-
-
+standard library and the `pytest` and `nose2` testing frameworks.
```

### Comparing `spyder_unittest-0.5.1/spyder_unittest.egg-info/SOURCES.txt` & `spyder_unittest-0.6.0/spyder_unittest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,45 +12,50 @@
 spyder_unittest.egg-info/dependency_links.txt
 spyder_unittest.egg-info/entry_points.txt
 spyder_unittest.egg-info/requires.txt
 spyder_unittest.egg-info/top_level.txt
 spyder_unittest/backend/__init__.py
 spyder_unittest/backend/abbreviator.py
 spyder_unittest/backend/frameworkregistry.py
-spyder_unittest/backend/noserunner.py
+spyder_unittest/backend/nose2runner.py
 spyder_unittest/backend/pytestrunner.py
 spyder_unittest/backend/runnerbase.py
 spyder_unittest/backend/unittestrunner.py
 spyder_unittest/backend/zmqreader.py
 spyder_unittest/backend/tests/__init__.py
 spyder_unittest/backend/tests/test_abbreviator.py
 spyder_unittest/backend/tests/test_frameworkregistry.py
-spyder_unittest/backend/tests/test_noserunner.py
+spyder_unittest/backend/tests/test_nose2runner.py
 spyder_unittest/backend/tests/test_pytestrunner.py
 spyder_unittest/backend/tests/test_runnerbase.py
 spyder_unittest/backend/tests/test_unittestrunner.py
 spyder_unittest/backend/tests/test_zmqstream.py
 spyder_unittest/backend/workers/__init__.py
 spyder_unittest/backend/workers/print_versions.py
 spyder_unittest/backend/workers/pytestworker.py
+spyder_unittest/backend/workers/unittestworker.py
 spyder_unittest/backend/workers/zmqwriter.py
 spyder_unittest/backend/workers/tests/test_print_versions.py
 spyder_unittest/backend/workers/tests/test_pytestworker.py
+spyder_unittest/backend/workers/tests/test_unittestworker.py
 spyder_unittest/locale/de/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/es/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/fr/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/hr/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/hu/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/ja/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/pl/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/pt_BR/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/ru/LC_MESSAGES/spyder_unittest.mo
 spyder_unittest/locale/zh_CN/LC_MESSAGES/spyder_unittest.mo
+spyder_unittest/tests/conftest.py
 spyder_unittest/tests/test_unittestplugin.py
 spyder_unittest/widgets/__init__.py
 spyder_unittest/widgets/configdialog.py
+spyder_unittest/widgets/confpage.py
 spyder_unittest/widgets/datatree.py
 spyder_unittest/widgets/unittestgui.py
 spyder_unittest/widgets/tests/__init__.py
 spyder_unittest/widgets/tests/test_configdialog.py
+spyder_unittest/widgets/tests/test_confpage.py
 spyder_unittest/widgets/tests/test_datatree.py
 spyder_unittest/widgets/tests/test_unittestgui.py
```

