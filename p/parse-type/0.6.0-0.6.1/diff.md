# Comparing `tmp/parse_type-0.6.0.tar.gz` & `tmp/parse_type-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parse_type-0.6.0.tar", last modified: Tue Jan 18 22:04:38 2022, max compression
+gzip compressed data, was "parse_type-0.6.1.tar", last modified: Sun Jul  2 18:17:41 2023, max compression
```

## Comparing `parse_type-0.6.0.tar` & `parse_type-0.6.1.tar`

### file list

```diff
@@ -1,73 +1,65 @@
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/py.requirements/
--rw-r--r--   0 jens       (502) staff       (20)      450 2018-10-29 20:24:10.000000 parse_type-0.6.0/py.requirements/all.txt
--rw-r--r--   0 jens       (502) staff       (20)      415 2022-01-18 21:46:14.000000 parse_type-0.6.0/py.requirements/testing.txt
--rw-r--r--   0 jens       (502) staff       (20)      429 2022-01-18 21:46:14.000000 parse_type-0.6.0/py.requirements/ci.travis.txt
--rw-r--r--   0 jens       (502) staff       (20)      437 2022-01-18 21:46:14.000000 parse_type-0.6.0/py.requirements/basic.txt
--rw-r--r--   0 jens       (502) staff       (20)       38 2018-10-29 20:24:10.000000 parse_type-0.6.0/py.requirements/py26_more.txt
--rw-r--r--   0 jens       (502) staff       (20)      381 2022-01-18 21:46:14.000000 parse_type-0.6.0/py.requirements/optional.txt
--rw-r--r--   0 jens       (502) staff       (20)      805 2022-01-18 21:46:14.000000 parse_type-0.6.0/py.requirements/develop.txt
--rw-r--r--   0 jens       (502) staff       (20)      267 2018-10-29 20:24:10.000000 parse_type-0.6.0/py.requirements/docs.txt
--rw-r--r--   0 jens       (502) staff       (20)    12914 2022-01-18 22:04:38.000000 parse_type-0.6.0/PKG-INFO
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/tasks/
--rw-r--r--   0 jens       (502) staff       (20)     1157 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/_dry_run.py
--rw-r--r--   0 jens       (502) staff       (20)     7381 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/release.py
--rw-r--r--   0 jens       (502) staff       (20)      546 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/py.requirements.txt
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/tasks/_vendor/
--rw-r--r--   0 jens       (502) staff       (20)    30098 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/_vendor/six.py
--rw-r--r--   0 jens       (502) staff       (20)     1117 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/_vendor/README.rst
--rw-r--r--   0 jens       (502) staff       (20)    41481 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/_vendor/pathlib.py
--rw-r--r--   0 jens       (502) staff       (20)    55818 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/_vendor/path.py
--rw-r--r--   0 jens       (502) staff       (20)   172281 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/_vendor/invoke.zip
--rw-r--r--   0 jens       (502) staff       (20)     2294 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/__init__.py
--rw-r--r--   0 jens       (502) staff       (20)     7183 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/docs.py
--rw-r--r--   0 jens       (502) staff       (20)     6940 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/test.py
--rw-r--r--   0 jens       (502) staff       (20)      220 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/_compat_shutil.py
--rw-r--r--   0 jens       (502) staff       (20)    10896 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/_tasklet_cleanup.py
--rw-r--r--   0 jens       (502) staff       (20)     1898 2018-10-29 20:24:10.000000 parse_type-0.6.0/tasks/__main__.py
--rw-r--r--   0 jens       (502) staff       (20)     4775 2022-01-18 21:46:14.000000 parse_type-0.6.0/tasks/_setup.py
--rw-r--r--   0 jens       (502) staff       (20)     1152 2022-01-18 21:57:02.000000 parse_type-0.6.0/pytest.ini
--rw-r--r--   0 jens       (502) staff       (20)     1488 2022-01-18 21:46:14.000000 parse_type-0.6.0/LICENSE
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/bin/
--rwxr-xr-x   0 jens       (502) staff       (20)      171 2018-10-29 20:24:10.000000 parse_type-0.6.0/bin/invoke
--rw-r--r--   0 jens       (502) staff       (20)      207 2018-10-29 20:24:10.000000 parse_type-0.6.0/bin/invoke.cmd
--rwx--x--x   0 jens       (502) staff       (20)     7693 2018-10-29 20:24:10.000000 parse_type-0.6.0/bin/make_localpi.py
--rwx--x--x   0 jens       (502) staff       (20)     8762 2018-10-29 20:24:10.000000 parse_type-0.6.0/bin/toxcmd.py
--rwx--x--x   0 jens       (502) staff       (20)      672 2018-10-29 20:24:10.000000 parse_type-0.6.0/bin/project_bootstrap.sh
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type/
--rw-r--r--   0 jens       (502) staff       (20)     8560 2022-01-18 21:46:14.000000 parse_type-0.6.0/parse_type/cardinality.py
--rw-r--r--   0 jens       (502) staff       (20)     6176 2018-10-29 20:24:10.000000 parse_type-0.6.0/parse_type/parse_util.py
--rw-r--r--   0 jens       (502) staff       (20)     6830 2022-01-18 21:46:14.000000 parse_type-0.6.0/parse_type/cardinality_field.py
--rw-r--r--   0 jens       (502) staff       (20)     1576 2022-01-18 21:57:02.000000 parse_type-0.6.0/parse_type/__init__.py
--rw-r--r--   0 jens       (502) staff       (20)    12159 2022-01-18 21:46:14.000000 parse_type-0.6.0/parse_type/builder.py
--rw-r--r--   0 jens       (502) staff       (20)     3773 2022-01-18 21:46:14.000000 parse_type-0.6.0/parse_type/cfparse.py
--rw-r--r--   0 jens       (502) staff       (20)    52208 2022-01-18 21:46:14.000000 parse_type-0.6.0/parse_type/parse.py
--rw-r--r--   0 jens       (502) staff       (20)      152 2022-01-18 21:57:02.000000 parse_type-0.6.0/.bumpversion.cfg
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/tests/
--rw-r--r--   0 jens       (502) staff       (20)     1779 2022-01-18 21:46:14.000000 parse_type-0.6.0/tests/test_parse_number.py
--rw-r--r--   0 jens       (502) staff       (20)    42935 2022-01-18 21:51:20.000000 parse_type-0.6.0/tests/test_parse.py
--rw-------   0 jens       (502) staff       (20)        0 2018-10-29 20:24:10.000000 parse_type-0.6.0/tests/__init__.py
--rwxr-xr-x   0 jens       (502) staff       (20)    23905 2022-01-18 21:46:14.000000 parse_type-0.6.0/tests/test_cardinality.py
--rw-r--r--   0 jens       (502) staff       (20)    18227 2018-10-29 20:24:10.000000 parse_type-0.6.0/tests/test_parse_util.py
--rwxr-xr-x   0 jens       (502) staff       (20)     5688 2022-01-18 21:46:14.000000 parse_type-0.6.0/tests/test_parse_decorator.py
--rwxr-xr-x   0 jens       (502) staff       (20)    23498 2022-01-18 21:46:14.000000 parse_type-0.6.0/tests/test_builder.py
--rw-r--r--   0 jens       (502) staff       (20)     8549 2022-01-18 21:46:14.000000 parse_type-0.6.0/tests/test_cfparse.py
--rwx--x--x   0 jens       (502) staff       (20)    16286 2018-10-29 20:24:10.000000 parse_type-0.6.0/tests/test_cardinality_field.py
--rwxr-xr-x   0 jens       (502) staff       (20)     5248 2018-10-29 20:24:10.000000 parse_type-0.6.0/tests/parse_type_test.py
--rwx--x--x   0 jens       (502) staff       (20)     7058 2018-10-29 20:24:10.000000 parse_type-0.6.0/tests/test_cardinality_field0.py
--rw-r--r--   0 jens       (502) staff       (20)      452 2018-10-29 20:24:10.000000 parse_type-0.6.0/MANIFEST.in
--rw-r--r--   0 jens       (502) staff       (20)     1148 2018-10-29 20:24:09.000000 parse_type-0.6.0/.coveragerc
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/
--rw-r--r--   0 jens       (502) staff       (20)    12914 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/PKG-INFO
--rw-r--r--   0 jens       (502) staff       (20)        1 2018-10-29 20:24:10.000000 parse_type-0.6.0/parse_type.egg-info/zip-safe
--rw-r--r--   0 jens       (502) staff       (20)     1397 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (502) staff       (20)      344 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/requires.txt
--rw-r--r--   0 jens       (502) staff       (20)       11 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/top_level.txt
--rw-r--r--   0 jens       (502) staff       (20)        1 2022-01-18 22:04:38.000000 parse_type-0.6.0/parse_type.egg-info/dependency_links.txt
--rw-------   0 jens       (502) staff       (20)      564 2018-10-29 20:24:09.000000 parse_type-0.6.0/.editorconfig
--rw-r--r--   0 jens       (502) staff       (20)      509 2022-01-18 21:46:14.000000 parse_type-0.6.0/CHANGES.txt
--rw-r--r--   0 jens       (502) staff       (20)     4029 2022-01-18 21:57:02.000000 parse_type-0.6.0/setup.py
--rw-r--r--   0 jens       (502) staff       (20)     2398 2022-01-18 21:50:13.000000 parse_type-0.6.0/tox.ini
--rw-r--r--   0 jens       (502) staff       (20)      262 2022-01-18 22:04:38.000000 parse_type-0.6.0/setup.cfg
--rw-r--r--   0 jens       (502) staff       (20)     9530 2022-01-18 21:46:14.000000 parse_type-0.6.0/README.rst
--rw-r--r--   0 jens       (502) staff       (20)      635 2022-01-18 21:46:14.000000 parse_type-0.6.0/invoke.yaml
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.937255 parse_type-0.6.1/
+-rw-r--r--   0 jens       (502) staff       (20)      141 2023-07-02 06:59:36.000000 parse_type-0.6.1/.bumpversion.cfg
+-rw-r--r--   0 jens       (502) staff       (20)     1148 2022-03-19 08:12:41.000000 parse_type-0.6.1/.coveragerc
+-rw-------   0 jens       (502) staff       (20)      564 2018-10-29 20:24:09.000000 parse_type-0.6.1/.editorconfig
+-rw-r--r--   0 jens       (502) staff       (20)     2953 2023-07-02 07:24:28.000000 parse_type-0.6.1/CHANGES.txt
+-rw-r--r--   0 jens       (502) staff       (20)     1069 2023-07-02 07:01:28.000000 parse_type-0.6.1/LICENSE
+-rw-r--r--   0 jens       (502) staff       (20)      487 2023-07-02 06:59:36.000000 parse_type-0.6.1/MANIFEST.in
+-rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-02 18:17:41.937515 parse_type-0.6.1/PKG-INFO
+-rw-r--r--   0 jens       (502) staff       (20)     9562 2022-03-11 22:21:42.000000 parse_type-0.6.1/README.rst
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.897128 parse_type-0.6.1/bin/
+-rwxr-xr-x   0 jens       (502) staff       (20)      171 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/invoke
+-rw-r--r--   0 jens       (502) staff       (20)      207 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/invoke.cmd
+-rwx--x--x   0 jens       (502) staff       (20)     7693 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/make_localpi.py
+-rwx--x--x   0 jens       (502) staff       (20)      672 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/project_bootstrap.sh
+-rwx--x--x   0 jens       (502) staff       (20)     8762 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/toxcmd.py
+-rw-r--r--   0 jens       (502) staff       (20)      694 2023-07-01 20:43:17.000000 parse_type-0.6.1/invoke.yaml
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.904209 parse_type-0.6.1/parse_type/
+-rw-r--r--   0 jens       (502) staff       (20)      434 2023-07-02 06:59:36.000000 parse_type-0.6.1/parse_type/__init__.py
+-rw-r--r--   0 jens       (502) staff       (20)    12159 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/builder.py
+-rw-r--r--   0 jens       (502) staff       (20)     8560 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cardinality.py
+-rw-r--r--   0 jens       (502) staff       (20)     6830 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cardinality_field.py
+-rw-r--r--   0 jens       (502) staff       (20)     3773 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cfparse.py
+-rw-r--r--   0 jens       (502) staff       (20)    34449 2023-07-01 20:47:57.000000 parse_type-0.6.1/parse_type/parse.py
+-rw-r--r--   0 jens       (502) staff       (20)     6176 2018-10-29 20:24:10.000000 parse_type-0.6.1/parse_type/parse_util.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.909774 parse_type-0.6.1/parse_type.egg-info/
+-rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (502) staff       (20)     1236 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (502) staff       (20)      644 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/requires.txt
+-rw-r--r--   0 jens       (502) staff       (20)       11 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/top_level.txt
+-rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-02 06:43:08.000000 parse_type-0.6.1/parse_type.egg-info/zip-safe
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.918114 parse_type-0.6.1/py.requirements/
+-rw-r--r--   0 jens       (502) staff       (20)      433 2023-07-01 19:28:19.000000 parse_type-0.6.1/py.requirements/all.txt
+-rw-r--r--   0 jens       (502) staff       (20)      526 2023-07-01 19:28:34.000000 parse_type-0.6.1/py.requirements/basic.txt
+-rw-r--r--   0 jens       (502) staff       (20)      394 2023-07-01 19:29:19.000000 parse_type-0.6.1/py.requirements/ci.github.testing.txt
+-rw-r--r--   0 jens       (502) staff       (20)      907 2023-07-02 06:59:36.000000 parse_type-0.6.1/py.requirements/develop.txt
+-rw-r--r--   0 jens       (502) staff       (20)      275 2023-07-02 06:59:36.000000 parse_type-0.6.1/py.requirements/docs.txt
+-rw-r--r--   0 jens       (502) staff       (20)      381 2022-01-18 21:46:14.000000 parse_type-0.6.1/py.requirements/optional.txt
+-rw-r--r--   0 jens       (502) staff       (20)      325 2023-07-01 19:52:23.000000 parse_type-0.6.1/py.requirements/testing.txt
+-rw-r--r--   0 jens       (502) staff       (20)     4119 2023-07-02 18:13:10.000000 parse_type-0.6.1/pyproject.toml
+-rw-r--r--   0 jens       (502) staff       (20)     1115 2023-07-02 06:59:36.000000 parse_type-0.6.1/pytest.ini
+-rw-r--r--   0 jens       (502) staff       (20)      111 2023-07-02 18:17:41.938852 parse_type-0.6.1/setup.cfg
+-rw-r--r--   0 jens       (502) staff       (20)     4343 2023-07-02 18:13:26.000000 parse_type-0.6.1/setup.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.925697 parse_type-0.6.1/tasks/
+-rw-r--r--   0 jens       (502) staff       (20)     1879 2023-07-01 20:05:14.000000 parse_type-0.6.1/tasks/__init__.py
+-rw-r--r--   0 jens       (502) staff       (20)      728 2023-07-01 20:04:08.000000 parse_type-0.6.1/tasks/__main__.py
+-rw-r--r--   0 jens       (502) staff       (20)      220 2022-01-18 21:46:14.000000 parse_type-0.6.1/tasks/_compat_shutil.py
+-rw-r--r--   0 jens       (502) staff       (20)     7183 2022-01-18 21:46:14.000000 parse_type-0.6.1/tasks/docs.py
+-rw-r--r--   0 jens       (502) staff       (20)     1722 2023-07-01 20:09:28.000000 parse_type-0.6.1/tasks/invoke_dry_run.py
+-rw-r--r--   0 jens       (502) staff       (20)      840 2023-07-01 20:01:21.000000 parse_type-0.6.1/tasks/py.requirements.txt
+-rw-r--r--   0 jens       (502) staff       (20)     7384 2023-07-01 20:09:51.000000 parse_type-0.6.1/tasks/release.py
+-rw-r--r--   0 jens       (502) staff       (20)     6937 2023-07-01 20:05:50.000000 parse_type-0.6.1/tasks/test.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.936680 parse_type-0.6.1/tests/
+-rw-------   0 jens       (502) staff       (20)        0 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/__init__.py
+-rwxr-xr-x   0 jens       (502) staff       (20)     5248 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/parse_type_test.py
+-rwxr-xr-x   0 jens       (502) staff       (20)    23498 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_builder.py
+-rwxr-xr-x   0 jens       (502) staff       (20)    23905 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_cardinality.py
+-rwx--x--x   0 jens       (502) staff       (20)    16286 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_cardinality_field.py
+-rwx--x--x   0 jens       (502) staff       (20)     7058 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_cardinality_field0.py
+-rw-r--r--   0 jens       (502) staff       (20)     8549 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_cfparse.py
+-rw-r--r--   0 jens       (502) staff       (20)    44199 2023-07-01 19:15:46.000000 parse_type-0.6.1/tests/test_parse.py
+-rwxr-xr-x   0 jens       (502) staff       (20)     5688 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_parse_decorator.py
+-rw-r--r--   0 jens       (502) staff       (20)     1834 2023-07-01 20:54:29.000000 parse_type-0.6.1/tests/test_parse_number.py
+-rw-r--r--   0 jens       (502) staff       (20)    18227 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_parse_util.py
+-rw-r--r--   0 jens       (502) staff       (20)     3483 2023-07-01 20:28:52.000000 parse_type-0.6.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `parse_type-0.6.0/PKG-INFO` & `parse_type-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,306 +1,320 @@
 Metadata-Version: 2.1
 Name: parse_type
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simplifies to build parse types based on the parse module
 Home-page: https://github.com/jenisys/parse_type
-Author: Jens Engel
-Author-email: jenisys@noreply.github.com
-License: BSD
 Download-URL: http://pypi.python.org/pypi/parse_type
-Description: .. image:: https://img.shields.io/travis/jenisys/parse_type/master.svg
-            :target: https://travis-ci.org/jenisys/parse_type
-            :alt: Travis CI Build Status
-        
-        .. image:: https://img.shields.io/pypi/v/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type
-            :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/dm/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/l/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type/
-            :alt: License
-        
-        
-        `parse_type`_ extends the `parse`_ module (opposite of `string.format()`_)
-        with the following features:
-        
-        * build type converters for common use cases (enum/mapping, choice)
-        * build a type converter with a cardinality constraint (0..1, 0..*, 1..*)
-            from the type converter with cardinality=1.
-        * compose a type converter from other type converters
-        * an extended parser that supports the CardinalityField naming schema
-            and creates missing type variants (0..1, 0..*, 1..*) from the
-            primary type converter
-        
-        .. _parse_type: http://pypi.python.org/pypi/parse_type
-        .. _parse:      http://pypi.python.org/pypi/parse
-        .. _`string.format()`: http://docs.python.org/library/string.html#format-string-syntax
-        
-        
-        Definitions
-        -------------------------------------------------------------------------------
-        
-        *type converter*
-            A type converter function that converts a textual representation
-            of a value type into instance of this value type.
-            In addition, a type converter function is often annotated with attributes
-            that allows the `parse`_ module to use it in a generic way.
-            A type converter is also called a *parse_type* (a definition used here).
-        
-        *cardinality field*
-            A naming convention for related types that differ in cardinality.
-            A cardinality field is a type name suffix in the format of a field.
-            It allows parse format expression, ala::
-        
-                "{person:Person}"     #< Cardinality: 1    (one; the normal case)
-                "{person:Person?}"    #< Cardinality: 0..1 (zero or one  = optional)
-                "{persons:Person*}"   #< Cardinality: 0..* (zero or more = many0)
-                "{persons:Person+}"   #< Cardinality: 1..* (one  or more = many)
-        
-            This naming convention mimics the relationship descriptions in UML diagrams.
-        
-        
-        Basic Example
-        -------------------------------------------------------------------------------
-        
-        Define an own type converter for numbers (integers):
-        
-        .. code-block:: python
-        
-            # -- USE CASE:
-            def parse_number(text):
-                return int(text)
-            parse_number.pattern = r"\d+"  # -- REGULAR EXPRESSION pattern for type.
-        
-        This is equivalent to:
-        
-        .. code-block:: python
-        
-            import parse
-        
-            @parse.with_pattern(r"\d+")
-            def parse_number(text):
-                 return int(text)
-            assert hasattr(parse_number, "pattern")
-            assert parse_number.pattern == r"\d+"
-        
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Use the type converter with the parse module.
-            schema = "Hello {number:Number}"
-            parser = parse.Parser(schema, dict(Number=parse_number))
-            result = parser.parse("Hello 42")
-            assert result is not None, "REQUIRE: text matches the schema."
-            assert result["number"] == 42
-        
-            result = parser.parse("Hello XXX")
-            assert result is None, "MISMATCH: text does not match the schema."
-        
-        .. hint::
-        
-            The described functionality above is standard functionality
-            of the `parse`_ module. It serves as introduction for the remaining cases.
-        
-        
-        Cardinality
-        -------------------------------------------------------------------------------
-        
-        Create an type converter for "ManyNumbers" (List, separated with commas)
-        with cardinality "1..* = 1+" (many) from the type converter for a "Number".
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create new type converter with a cardinality constraint.
-            # CARDINALITY: many := one or more (1..*)
-            from parse import Parser
-            from parse_type import TypeBuilder
-            parse_numbers = TypeBuilder.with_many(parse_number, listsep=",")
-        
-            schema = "List: {numbers:ManyNumbers}"
-            parser = Parser(schema, dict(ManyNumbers=parse_numbers))
-            result = parser.parse("List: 1, 2, 3")
-            assert result["numbers"] == [1, 2, 3]
-        
-        
-        Create an type converter for an "OptionalNumbers" with cardinality "0..1 = ?"
-        (optional) from the type converter for a "Number".
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create new type converter with cardinality constraint.
-            # CARDINALITY: optional := zero or one (0..1)
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_optional_number = TypeBuilder.with_optional(parse_number)
-            schema = "Optional: {number:OptionalNumber}"
-            parser = Parser(schema, dict(OptionalNumber=parse_optional_number))
-            result = parser.parse("Optional: 42")
-            assert result["number"] == 42
-            result = parser.parse("Optional: ")
-            assert result["number"] == None
-        
-        
-        Enumeration (Name-to-Value Mapping)
-        -------------------------------------------------------------------------------
-        
-        Create an type converter for an "Enumeration" from the description of
-        the mapping as dictionary.
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create a type converter for an enumeration.
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_enum_yesno = TypeBuilder.make_enum({"yes": True, "no": False})
-            parser = Parser("Answer: {answer:YesNo}", dict(YesNo=parse_enum_yesno))
-            result = parser.parse("Answer: yes")
-            assert result["answer"] == True
-        
-        
-        Create an type converter for an "Enumeration" from the description of
-        the mapping as an enumeration class (`Python 3.4 enum`_ or the `enum34`_
-        backport; see also: `PEP-0435`_).
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create a type converter for enum34 enumeration class.
-            # NOTE: Use Python 3.4 or enum34 backport.
-            from parse import Parser
-            from parse_type import TypeBuilder
-            from enum import Enum
-        
-            class Color(Enum):
-                red   = 1
-                green = 2
-                blue  = 3
-        
-            parse_enum_color = TypeBuilder.make_enum(Color)
-            parser = Parser("Select: {color:Color}", dict(Color=parse_enum_color))
-            result = parser.parse("Select: red")
-            assert result["color"] is Color.red
-        
-        .. _`Python 3.4 enum`: http://docs.python.org/3.4/library/enum.html#module-enum
-        .. _enum34:   http://pypi.python.org/pypi/enum34
-        .. _PEP-0435: http://www.python.org/dev/peps/pep-0435
-        
-        
-        Choice (Name Enumeration)
-        -------------------------------------------------------------------------------
-        
-        A Choice data type allows to select one of several strings.
-        
-        Create an type converter for an "Choice" list, a list of unique names
-        (as string).
-        
-        .. code-block:: python
-        
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_choice_yesno = TypeBuilder.make_choice(["yes", "no"])
-            schema = "Answer: {answer:ChoiceYesNo}"
-            parser = Parser(schema, dict(ChoiceYesNo=parse_choice_yesno))
-            result = parser.parse("Answer: yes")
-            assert result["answer"] == "yes"
-        
-        
-        Variant (Type Alternatives)
-        -------------------------------------------------------------------------------
-        
-        Sometimes you need a type converter that can accept text for multiple
-        type converter alternatives. This is normally called a "variant" (or: union).
-        
-        Create an type converter for an "Variant" type that accepts:
-        
-        * Numbers (positive numbers, as integer)
-        * Color enum values (by name)
-        
-        .. code-block:: python
-        
-            from parse import Parser, with_pattern
-            from parse_type import TypeBuilder
-            from enum import Enum
-        
-            class Color(Enum):
-                red   = 1
-                green = 2
-                blue  = 3
-        
-            @with_pattern(r"\d+")
-            def parse_number(text):
-                return int(text)
-        
-            # -- MAKE VARIANT: Alternatives of different type converters.
-            parse_color = TypeBuilder.make_enum(Color)
-            parse_variant = TypeBuilder.make_variant([parse_number, parse_color])
-            schema = "Variant: {variant:Number_or_Color}"
-            parser = Parser(schema, dict(Number_or_Color=parse_variant))
-        
-            # -- TEST VARIANT: With number, color and mismatch.
-            result = parser.parse("Variant: 42")
-            assert result["variant"] == 42
-            result = parser.parse("Variant: blue")
-            assert result["variant"] is Color.blue
-            result = parser.parse("Variant: __MISMATCH__")
-            assert not result
-        
-        
-        
-        Extended Parser with CardinalityField support
-        -------------------------------------------------------------------------------
-        
-        The parser extends the ``parse.Parser`` and adds the following functionality:
-        
-        * supports the CardinalityField naming scheme
-        * automatically creates missing type variants for types with
-          a CardinalityField by using the primary type converter for cardinality=1
-        * extends the provide type converter dictionary with new type variants.
-        
-        Example:
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Parser with CardinalityField support.
-            # NOTE: Automatically adds missing type variants with CardinalityField part.
-            # USE:  parse_number() type converter from above.
-            from parse_type.cfparse import Parser
-        
-            # -- PREPARE: parser, adds missing type variant for cardinality 1..* (many)
-            type_dict = dict(Number=parse_number)
-            schema = "List: {numbers:Number+}"
-            parser = Parser(schema, type_dict)
-            assert "Number+" in type_dict, "Created missing type variant based on: Number"
-        
-            # -- USE: parser.
-            result = parser.parse("List: 1, 2, 3")
-            assert result["numbers"] == [1, 2, 3]
-        
+Author: Jens Engel
+Author-email: Jens Engel <jenisys@noreply.github.com>
+License: MIT
+Project-URL: Homepage, https://github.com/jenisys/parse_type
+Project-URL: Download, http://pypi.python.org/pypi/parse_type
+Project-URL: Source Code, https://github.com/jenisys/parse_type
+Project-URL: Issue Tracker, https://github.com/jenisys/parse_type/issues/
 Keywords: parse,parsing
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
+Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: develop
+Provides-Extra: testing
+License-File: LICENSE
+
+===============================================================================
+parse_type
+===============================================================================
+
+.. image:: https://github.com/jenisys/parse_type/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jenisys/parse_type/actions/workflows/test.yml
+    :alt: CI Build Status
+
+.. image:: https://img.shields.io/pypi/v/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type
+    :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/dm/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/l/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type/
+    :alt: License
+
+
+`parse_type`_ extends the `parse`_ module (opposite of `string.format()`_)
+with the following features:
+
+* build type converters for common use cases (enum/mapping, choice)
+* build a type converter with a cardinality constraint (0..1, 0..*, 1..*)
+    from the type converter with cardinality=1.
+* compose a type converter from other type converters
+* an extended parser that supports the CardinalityField naming schema
+    and creates missing type variants (0..1, 0..*, 1..*) from the
+    primary type converter
+
+.. _parse_type: http://pypi.python.org/pypi/parse_type
+.. _parse:      http://pypi.python.org/pypi/parse
+.. _`string.format()`: http://docs.python.org/library/string.html#format-string-syntax
+
+
+Definitions
+-------------------------------------------------------------------------------
+
+*type converter*
+    A type converter function that converts a textual representation
+    of a value type into instance of this value type.
+    In addition, a type converter function is often annotated with attributes
+    that allows the `parse`_ module to use it in a generic way.
+    A type converter is also called a *parse_type* (a definition used here).
+
+*cardinality field*
+    A naming convention for related types that differ in cardinality.
+    A cardinality field is a type name suffix in the format of a field.
+    It allows parse format expression, ala::
+
+        "{person:Person}"     #< Cardinality: 1    (one; the normal case)
+        "{person:Person?}"    #< Cardinality: 0..1 (zero or one  = optional)
+        "{persons:Person*}"   #< Cardinality: 0..* (zero or more = many0)
+        "{persons:Person+}"   #< Cardinality: 1..* (one  or more = many)
+
+    This naming convention mimics the relationship descriptions in UML diagrams.
+
+
+Basic Example
+-------------------------------------------------------------------------------
+
+Define an own type converter for numbers (integers):
+
+.. code-block:: python
+
+    # -- USE CASE:
+    def parse_number(text):
+        return int(text)
+    parse_number.pattern = r"\d+"  # -- REGULAR EXPRESSION pattern for type.
+
+This is equivalent to:
+
+.. code-block:: python
+
+    import parse
+
+    @parse.with_pattern(r"\d+")
+    def parse_number(text):
+         return int(text)
+    assert hasattr(parse_number, "pattern")
+    assert parse_number.pattern == r"\d+"
+
+
+.. code-block:: python
+
+    # -- USE CASE: Use the type converter with the parse module.
+    schema = "Hello {number:Number}"
+    parser = parse.Parser(schema, dict(Number=parse_number))
+    result = parser.parse("Hello 42")
+    assert result is not None, "REQUIRE: text matches the schema."
+    assert result["number"] == 42
+
+    result = parser.parse("Hello XXX")
+    assert result is None, "MISMATCH: text does not match the schema."
+
+.. hint::
+
+    The described functionality above is standard functionality
+    of the `parse`_ module. It serves as introduction for the remaining cases.
+
+
+Cardinality
+-------------------------------------------------------------------------------
+
+Create an type converter for "ManyNumbers" (List, separated with commas)
+with cardinality "1..* = 1+" (many) from the type converter for a "Number".
+
+.. code-block:: python
+
+    # -- USE CASE: Create new type converter with a cardinality constraint.
+    # CARDINALITY: many := one or more (1..*)
+    from parse import Parser
+    from parse_type import TypeBuilder
+    parse_numbers = TypeBuilder.with_many(parse_number, listsep=",")
+
+    schema = "List: {numbers:ManyNumbers}"
+    parser = Parser(schema, dict(ManyNumbers=parse_numbers))
+    result = parser.parse("List: 1, 2, 3")
+    assert result["numbers"] == [1, 2, 3]
+
+
+Create an type converter for an "OptionalNumbers" with cardinality "0..1 = ?"
+(optional) from the type converter for a "Number".
+
+.. code-block:: python
+
+    # -- USE CASE: Create new type converter with cardinality constraint.
+    # CARDINALITY: optional := zero or one (0..1)
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_optional_number = TypeBuilder.with_optional(parse_number)
+    schema = "Optional: {number:OptionalNumber}"
+    parser = Parser(schema, dict(OptionalNumber=parse_optional_number))
+    result = parser.parse("Optional: 42")
+    assert result["number"] == 42
+    result = parser.parse("Optional: ")
+    assert result["number"] == None
+
+
+Enumeration (Name-to-Value Mapping)
+-------------------------------------------------------------------------------
+
+Create an type converter for an "Enumeration" from the description of
+the mapping as dictionary.
+
+.. code-block:: python
+
+    # -- USE CASE: Create a type converter for an enumeration.
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_enum_yesno = TypeBuilder.make_enum({"yes": True, "no": False})
+    parser = Parser("Answer: {answer:YesNo}", dict(YesNo=parse_enum_yesno))
+    result = parser.parse("Answer: yes")
+    assert result["answer"] == True
+
+
+Create an type converter for an "Enumeration" from the description of
+the mapping as an enumeration class (`Python 3.4 enum`_ or the `enum34`_
+backport; see also: `PEP-0435`_).
+
+.. code-block:: python
+
+    # -- USE CASE: Create a type converter for enum34 enumeration class.
+    # NOTE: Use Python 3.4 or enum34 backport.
+    from parse import Parser
+    from parse_type import TypeBuilder
+    from enum import Enum
+
+    class Color(Enum):
+        red   = 1
+        green = 2
+        blue  = 3
+
+    parse_enum_color = TypeBuilder.make_enum(Color)
+    parser = Parser("Select: {color:Color}", dict(Color=parse_enum_color))
+    result = parser.parse("Select: red")
+    assert result["color"] is Color.red
+
+.. _`Python 3.4 enum`: http://docs.python.org/3.4/library/enum.html#module-enum
+.. _enum34:   http://pypi.python.org/pypi/enum34
+.. _PEP-0435: http://www.python.org/dev/peps/pep-0435
+
+
+Choice (Name Enumeration)
+-------------------------------------------------------------------------------
+
+A Choice data type allows to select one of several strings.
+
+Create an type converter for an "Choice" list, a list of unique names
+(as string).
+
+.. code-block:: python
+
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_choice_yesno = TypeBuilder.make_choice(["yes", "no"])
+    schema = "Answer: {answer:ChoiceYesNo}"
+    parser = Parser(schema, dict(ChoiceYesNo=parse_choice_yesno))
+    result = parser.parse("Answer: yes")
+    assert result["answer"] == "yes"
+
+
+Variant (Type Alternatives)
+-------------------------------------------------------------------------------
+
+Sometimes you need a type converter that can accept text for multiple
+type converter alternatives. This is normally called a "variant" (or: union).
+
+Create an type converter for an "Variant" type that accepts:
+
+* Numbers (positive numbers, as integer)
+* Color enum values (by name)
+
+.. code-block:: python
+
+    from parse import Parser, with_pattern
+    from parse_type import TypeBuilder
+    from enum import Enum
+
+    class Color(Enum):
+        red   = 1
+        green = 2
+        blue  = 3
+
+    @with_pattern(r"\d+")
+    def parse_number(text):
+        return int(text)
+
+    # -- MAKE VARIANT: Alternatives of different type converters.
+    parse_color = TypeBuilder.make_enum(Color)
+    parse_variant = TypeBuilder.make_variant([parse_number, parse_color])
+    schema = "Variant: {variant:Number_or_Color}"
+    parser = Parser(schema, dict(Number_or_Color=parse_variant))
+
+    # -- TEST VARIANT: With number, color and mismatch.
+    result = parser.parse("Variant: 42")
+    assert result["variant"] == 42
+    result = parser.parse("Variant: blue")
+    assert result["variant"] is Color.blue
+    result = parser.parse("Variant: __MISMATCH__")
+    assert not result
+
+
+
+Extended Parser with CardinalityField support
+-------------------------------------------------------------------------------
+
+The parser extends the ``parse.Parser`` and adds the following functionality:
+
+* supports the CardinalityField naming scheme
+* automatically creates missing type variants for types with
+  a CardinalityField by using the primary type converter for cardinality=1
+* extends the provide type converter dictionary with new type variants.
+
+Example:
+
+.. code-block:: python
+
+    # -- USE CASE: Parser with CardinalityField support.
+    # NOTE: Automatically adds missing type variants with CardinalityField part.
+    # USE:  parse_number() type converter from above.
+    from parse_type.cfparse import Parser
+
+    # -- PREPARE: parser, adds missing type variant for cardinality 1..* (many)
+    type_dict = dict(Number=parse_number)
+    schema = "List: {numbers:Number+}"
+    parser = Parser(schema, type_dict)
+    assert "Number+" in type_dict, "Created missing type variant based on: Number"
+
+    # -- USE: parser.
+    result = parser.parse("List: 1, 2, 3")
+    assert result["numbers"] == [1, 2, 3]
```

### Comparing `parse_type-0.6.0/tasks/release.py` & `parse_type-0.6.1/tasks/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     * https://packaging.python.org/
     * https://packaging.python.org/guides/
     * https://packaging.python.org/tutorials/distributing-packages/
 """
 
 from __future__ import absolute_import, print_function
 from invoke import Collection, task
-from ._tasklet_cleanup import path_glob
-from ._dry_run import DryRunContext
+from invoke_cleanup import path_glob
+from .invoke_dry_run import DryRunContext
 
 
 # -----------------------------------------------------------------------------
 # TASKS:
 # -----------------------------------------------------------------------------
 @task
 def checklist(ctx=None):    # pylint: disable=unused-argument
```

### Comparing `parse_type-0.6.0/tasks/__init__.py` & `parse_type-0.6.1/tasks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,24 @@
 
 .. seealso::
 
     * http://pyinvoke.org
     * https://github.com/pyinvoke/invoke
 """
 
-from __future__ import absolute_import
-
-# -----------------------------------------------------------------------------
-# BOOTSTRAP PATH: Use provided vendor bundle if "invoke" is not installed
-# -----------------------------------------------------------------------------
-from . import _setup    # pylint: disable=wrong-import-order
-import os.path
-import sys
-INVOKE_MINVERSION = "1.2.0"
-_setup.setup_path()
-_setup.require_invoke_minversion(INVOKE_MINVERSION)
+from __future__ import absolute_import, print_function
 
 # -----------------------------------------------------------------------------
 # IMPORTS:
 # -----------------------------------------------------------------------------
 import sys
 from invoke import Collection
 
 # -- TASK-LIBRARY:
-from . import _tasklet_cleanup as cleanup
+import invoke_cleanup as cleanup
 from . import test
 from . import release
 # DISABLED: from . import docs
 
 # -----------------------------------------------------------------------------
 # TASKS:
 # -----------------------------------------------------------------------------
```

### Comparing `parse_type-0.6.0/tasks/docs.py` & `parse_type-0.6.1/tasks/docs.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tasks/test.py` & `parse_type-0.6.1/tasks/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from __future__ import print_function
 import os.path
 import sys
 from invoke import task, Collection
 
 # -- TASK-LIBRARY:
-from ._tasklet_cleanup import cleanup_tasks, cleanup_dirs, cleanup_files
+from invoke_cleanup import cleanup_tasks, cleanup_dirs, cleanup_files
 
 
 # ---------------------------------------------------------------------------
 # CONSTANTS:
 # ---------------------------------------------------------------------------
 USE_BEHAVE = False
```

### Comparing `parse_type-0.6.0/pytest.ini` & `parse_type-0.6.1/pytest.ini`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 [pytest]
 minversion    = 4.2
 testpaths     = tests
 python_files  = test_*.py
 junit_family = xunit2
 addopts = --metadata PACKAGE_UNDER_TEST parse_type
-    --metadata PACKAGE_VERSION 0.6.0
     --html=build/testing/report.html --self-contained-html
     --junit-xml=build/testing/report.xml
 # markers =
 #    smoke
 #    slow
 
 # -- PREPARED:
```

### Comparing `parse_type-0.6.0/bin/make_localpi.py` & `parse_type-0.6.1/bin/make_localpi.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/bin/toxcmd.py` & `parse_type-0.6.1/bin/toxcmd.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/bin/project_bootstrap.sh` & `parse_type-0.6.1/bin/project_bootstrap.sh`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type/cardinality.py` & `parse_type-0.6.1/parse_type/cardinality.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type/parse_util.py` & `parse_type-0.6.1/parse_type/parse_util.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type/cardinality_field.py` & `parse_type-0.6.1/parse_type/cardinality_field.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type/builder.py` & `parse_type-0.6.1/parse_type/builder.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type/cfparse.py` & `parse_type-0.6.1/parse_type/cfparse.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_parse_number.py` & `parse_type-0.6.1/tests/test_parse_number.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 Additional unit tests for the :mod`parse` module.
 Related to auto-detection of number base (base=10, 2, 8, 16).
 """
 
 from __future__ import absolute_import, print_function
 import pytest
 import parse
+
 parse_version = parse.__version__
 print("USING: parse-%s" % parse_version)
 if parse_version in ("1.17.0", "1.16.0"):
+    # -- REQUIRES: parse >= 1.18.0 -- WORKAROUND HERE
     print("USING: parse_type.parse (INSTEAD)")
     from parse_type import parse
 
 def assert_parse_number_with_format_d(text, expected):
     parser = parse.Parser("{value:d}")
     result = parser.parse(text)
     assert result.named == dict(value=expected)
```

### Comparing `parse_type-0.6.0/tests/test_parse.py` & `parse_type-0.6.1/tests/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- encoding: utf8 -*-
 # -- BASED-ON: https://github.com/r1chardj0n3s/parse/test_parse.py
-# VERSION:  parse 1.17.0_POST_JE_FIX-ISSUE_121_PULL-REQUEST_122
+# VERSION:  parse v1.19.1
 # Same as original file but uses bundled :mod:`parse_type.parse` module
 # instead of :mod:`parse` module
 #
 # NOTE: Part of the tests are/were providd by jenisys.
 # -- ORIGINAL-CODE STARTS-HERE ------------------------------------------------
 '''Test suite for parse.py
 
@@ -55,14 +55,19 @@
         self._test_expression('{name} {other}', r'(?P<name>.+?) (?P<other>.+?)')
 
     def test_named_typed(self):
         # pull a named string out of another string
         self._test_expression('{name:w}', r'(?P<name>\w+)')
         self._test_expression('{name:w} {other:w}', r'(?P<name>\w+) (?P<other>\w+)')
 
+    def test_numbered(self):
+        self._test_expression('{0}', r'(.+?)')
+        self._test_expression('{0} {1}', r'(.+?) (.+?)')
+        self._test_expression('{0:f} {1:f}', r'([-+ ]?\d*\.\d+) ([-+ ]?\d*\.\d+)')
+
     def test_bird(self):
         # skip some trailing whitespace
         self._test_expression('{:>}', r' *(.+?)')
 
     def test_format_variety(self):
         def _(fmt, matches):
             d = parse.extract_format(fmt, {'spam': 'spam'})
@@ -123,14 +128,22 @@
     def test_fixed_access(self):
         r = parse.Result((1, 2), {}, None)
         self.assertEqual(r[0], 1)
         self.assertEqual(r[1], 2)
         self.assertRaises(IndexError, r.__getitem__, 2)
         self.assertRaises(KeyError, r.__getitem__, 'spam')
 
+    def test_slice_access(self):
+        r = parse.Result((1, 2, 3, 4), {}, None)
+        self.assertEqual(r[1:3], (2, 3))
+        self.assertEqual(r[-5:5], (1, 2, 3, 4))
+        self.assertEqual(r[:4:2], (1, 3))
+        self.assertEqual(r[::-2], (4, 2))
+        self.assertEqual(r[5:10], tuple())
+
     def test_named_access(self):
         r = parse.Result((), {'spam': 'ham'}, None)
         self.assertEqual(r['spam'], 'ham')
         self.assertRaises(KeyError, r.__getitem__, 'ham')
         self.assertRaises(IndexError, r.__getitem__, 0)
 
     def test_contains(self):
@@ -210,14 +223,25 @@
     def test_typed(self):
         # pull a named, typed values out of string
         r = parse.parse('hello {:d} {:w}', 'hello 12 people')
         self.assertEqual(r.fixed, (12, 'people'))
         r = parse.parse('hello {:w} {:w}', 'hello 12 people')
         self.assertEqual(r.fixed, ('12', 'people'))
 
+    def test_sign(self):
+        # sign is ignored
+        r = parse.parse('Pi = {:.7f}', 'Pi = 3.1415926')
+        self.assertEqual(r.fixed, (3.1415926,))
+        r = parse.parse('Pi = {:+.7f}', 'Pi = 3.1415926')
+        self.assertEqual(r.fixed, (3.1415926,))
+        r = parse.parse('Pi = {:-.7f}', 'Pi = 3.1415926')
+        self.assertEqual(r.fixed, (3.1415926,))
+        r = parse.parse('Pi = {: .7f}', 'Pi = 3.1415926')
+        self.assertEqual(r.fixed, (3.1415926,))
+
     def test_precision(self):
         # pull a float out of a string
         r = parse.parse('Pi = {:.7f}', 'Pi = 3.1415926')
         self.assertEqual(r.fixed, (3.1415926,))
         r = parse.parse('Pi/10 = {:8.5f}', 'Pi/10 =  0.31415')
         self.assertEqual(r.fixed, (0.31415,))
         # float may have not leading zero
@@ -870,25 +894,35 @@
         self.assertIsNone(r)
 
     def test_pickling_bug_110(self):
         p = parse.compile('{a:d}')
         # prior to the fix, this would raise an AttributeError
         pickle.dumps(p)
 
-    def test_search_centered_bug_112(self):
-        r = parse.parse("{:^},{:^}", " 12 , 34 ")
-        self.assertEqual(r[1], "34")
-        r = parse.search("{:^},{:^}", " 12 , 34 ")
-        self.assertEqual(r[1], "34")
-
-    def test_search_left_align_bug_112(self):
-        r = parse.parse("{:<},{:<}", "12 ,34 ")
-        self.assertEqual(r[1], "34")
-        r = parse.search("{:<},{:<}", "12 ,34 ")
-        self.assertEqual(r[1], "34")
+
+    def test_unused_centered_alignment_bug(self):
+        r = parse.parse("{:^2S}", "foo")
+        self.assertEqual(r[0], "foo")
+        r = parse.search("{:^2S}", "foo")
+        self.assertEqual(r[0], "foo")
+
+        # specifically test for the case in issue #118 as well
+        r = parse.parse("Column {:d}:{:^}", "Column 1: Timestep")
+        self.assertEqual(r[0], 1)
+        self.assertEqual(r[1], "Timestep")
+
+    def test_unused_left_alignment_bug(self):
+        r = parse.parse("{:<2S}", "foo")
+        self.assertEqual(r[0], "foo")
+        r = parse.search("{:<2S}", "foo")
+        self.assertEqual(r[0], "foo")
+
+    def test_match_trailing_newline(self):
+        r = parse.parse('{}', 'test\n')
+        self.assertEqual(r[0], 'test\n')
 
 
 # -----------------------------------------------------------------------------
 # TEST SUPPORT FOR: TestParseType
 # -----------------------------------------------------------------------------
 class TestParseType(unittest.TestCase):
     def assert_match(self, parser, text, param_name, expected):
```

### Comparing `parse_type-0.6.0/tests/test_cardinality.py` & `parse_type-0.6.1/tests/test_cardinality.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_parse_util.py` & `parse_type-0.6.1/tests/test_parse_util.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_parse_decorator.py` & `parse_type-0.6.1/tests/test_parse_decorator.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_builder.py` & `parse_type-0.6.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_cfparse.py` & `parse_type-0.6.1/tests/test_cfparse.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_cardinality_field.py` & `parse_type-0.6.1/tests/test_cardinality_field.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/parse_type_test.py` & `parse_type-0.6.1/tests/parse_type_test.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/tests/test_cardinality_field0.py` & `parse_type-0.6.1/tests/test_cardinality_field0.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/.coveragerc` & `parse_type-0.6.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/parse_type.egg-info/PKG-INFO` & `parse_type-0.6.1/parse_type.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,306 +1,320 @@
 Metadata-Version: 2.1
 Name: parse-type
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simplifies to build parse types based on the parse module
 Home-page: https://github.com/jenisys/parse_type
-Author: Jens Engel
-Author-email: jenisys@noreply.github.com
-License: BSD
 Download-URL: http://pypi.python.org/pypi/parse_type
-Description: .. image:: https://img.shields.io/travis/jenisys/parse_type/master.svg
-            :target: https://travis-ci.org/jenisys/parse_type
-            :alt: Travis CI Build Status
-        
-        .. image:: https://img.shields.io/pypi/v/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type
-            :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/dm/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/l/parse_type.svg
-            :target: https://pypi.python.org/pypi/parse_type/
-            :alt: License
-        
-        
-        `parse_type`_ extends the `parse`_ module (opposite of `string.format()`_)
-        with the following features:
-        
-        * build type converters for common use cases (enum/mapping, choice)
-        * build a type converter with a cardinality constraint (0..1, 0..*, 1..*)
-            from the type converter with cardinality=1.
-        * compose a type converter from other type converters
-        * an extended parser that supports the CardinalityField naming schema
-            and creates missing type variants (0..1, 0..*, 1..*) from the
-            primary type converter
-        
-        .. _parse_type: http://pypi.python.org/pypi/parse_type
-        .. _parse:      http://pypi.python.org/pypi/parse
-        .. _`string.format()`: http://docs.python.org/library/string.html#format-string-syntax
-        
-        
-        Definitions
-        -------------------------------------------------------------------------------
-        
-        *type converter*
-            A type converter function that converts a textual representation
-            of a value type into instance of this value type.
-            In addition, a type converter function is often annotated with attributes
-            that allows the `parse`_ module to use it in a generic way.
-            A type converter is also called a *parse_type* (a definition used here).
-        
-        *cardinality field*
-            A naming convention for related types that differ in cardinality.
-            A cardinality field is a type name suffix in the format of a field.
-            It allows parse format expression, ala::
-        
-                "{person:Person}"     #< Cardinality: 1    (one; the normal case)
-                "{person:Person?}"    #< Cardinality: 0..1 (zero or one  = optional)
-                "{persons:Person*}"   #< Cardinality: 0..* (zero or more = many0)
-                "{persons:Person+}"   #< Cardinality: 1..* (one  or more = many)
-        
-            This naming convention mimics the relationship descriptions in UML diagrams.
-        
-        
-        Basic Example
-        -------------------------------------------------------------------------------
-        
-        Define an own type converter for numbers (integers):
-        
-        .. code-block:: python
-        
-            # -- USE CASE:
-            def parse_number(text):
-                return int(text)
-            parse_number.pattern = r"\d+"  # -- REGULAR EXPRESSION pattern for type.
-        
-        This is equivalent to:
-        
-        .. code-block:: python
-        
-            import parse
-        
-            @parse.with_pattern(r"\d+")
-            def parse_number(text):
-                 return int(text)
-            assert hasattr(parse_number, "pattern")
-            assert parse_number.pattern == r"\d+"
-        
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Use the type converter with the parse module.
-            schema = "Hello {number:Number}"
-            parser = parse.Parser(schema, dict(Number=parse_number))
-            result = parser.parse("Hello 42")
-            assert result is not None, "REQUIRE: text matches the schema."
-            assert result["number"] == 42
-        
-            result = parser.parse("Hello XXX")
-            assert result is None, "MISMATCH: text does not match the schema."
-        
-        .. hint::
-        
-            The described functionality above is standard functionality
-            of the `parse`_ module. It serves as introduction for the remaining cases.
-        
-        
-        Cardinality
-        -------------------------------------------------------------------------------
-        
-        Create an type converter for "ManyNumbers" (List, separated with commas)
-        with cardinality "1..* = 1+" (many) from the type converter for a "Number".
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create new type converter with a cardinality constraint.
-            # CARDINALITY: many := one or more (1..*)
-            from parse import Parser
-            from parse_type import TypeBuilder
-            parse_numbers = TypeBuilder.with_many(parse_number, listsep=",")
-        
-            schema = "List: {numbers:ManyNumbers}"
-            parser = Parser(schema, dict(ManyNumbers=parse_numbers))
-            result = parser.parse("List: 1, 2, 3")
-            assert result["numbers"] == [1, 2, 3]
-        
-        
-        Create an type converter for an "OptionalNumbers" with cardinality "0..1 = ?"
-        (optional) from the type converter for a "Number".
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create new type converter with cardinality constraint.
-            # CARDINALITY: optional := zero or one (0..1)
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_optional_number = TypeBuilder.with_optional(parse_number)
-            schema = "Optional: {number:OptionalNumber}"
-            parser = Parser(schema, dict(OptionalNumber=parse_optional_number))
-            result = parser.parse("Optional: 42")
-            assert result["number"] == 42
-            result = parser.parse("Optional: ")
-            assert result["number"] == None
-        
-        
-        Enumeration (Name-to-Value Mapping)
-        -------------------------------------------------------------------------------
-        
-        Create an type converter for an "Enumeration" from the description of
-        the mapping as dictionary.
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create a type converter for an enumeration.
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_enum_yesno = TypeBuilder.make_enum({"yes": True, "no": False})
-            parser = Parser("Answer: {answer:YesNo}", dict(YesNo=parse_enum_yesno))
-            result = parser.parse("Answer: yes")
-            assert result["answer"] == True
-        
-        
-        Create an type converter for an "Enumeration" from the description of
-        the mapping as an enumeration class (`Python 3.4 enum`_ or the `enum34`_
-        backport; see also: `PEP-0435`_).
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Create a type converter for enum34 enumeration class.
-            # NOTE: Use Python 3.4 or enum34 backport.
-            from parse import Parser
-            from parse_type import TypeBuilder
-            from enum import Enum
-        
-            class Color(Enum):
-                red   = 1
-                green = 2
-                blue  = 3
-        
-            parse_enum_color = TypeBuilder.make_enum(Color)
-            parser = Parser("Select: {color:Color}", dict(Color=parse_enum_color))
-            result = parser.parse("Select: red")
-            assert result["color"] is Color.red
-        
-        .. _`Python 3.4 enum`: http://docs.python.org/3.4/library/enum.html#module-enum
-        .. _enum34:   http://pypi.python.org/pypi/enum34
-        .. _PEP-0435: http://www.python.org/dev/peps/pep-0435
-        
-        
-        Choice (Name Enumeration)
-        -------------------------------------------------------------------------------
-        
-        A Choice data type allows to select one of several strings.
-        
-        Create an type converter for an "Choice" list, a list of unique names
-        (as string).
-        
-        .. code-block:: python
-        
-            from parse import Parser
-            from parse_type import TypeBuilder
-        
-            parse_choice_yesno = TypeBuilder.make_choice(["yes", "no"])
-            schema = "Answer: {answer:ChoiceYesNo}"
-            parser = Parser(schema, dict(ChoiceYesNo=parse_choice_yesno))
-            result = parser.parse("Answer: yes")
-            assert result["answer"] == "yes"
-        
-        
-        Variant (Type Alternatives)
-        -------------------------------------------------------------------------------
-        
-        Sometimes you need a type converter that can accept text for multiple
-        type converter alternatives. This is normally called a "variant" (or: union).
-        
-        Create an type converter for an "Variant" type that accepts:
-        
-        * Numbers (positive numbers, as integer)
-        * Color enum values (by name)
-        
-        .. code-block:: python
-        
-            from parse import Parser, with_pattern
-            from parse_type import TypeBuilder
-            from enum import Enum
-        
-            class Color(Enum):
-                red   = 1
-                green = 2
-                blue  = 3
-        
-            @with_pattern(r"\d+")
-            def parse_number(text):
-                return int(text)
-        
-            # -- MAKE VARIANT: Alternatives of different type converters.
-            parse_color = TypeBuilder.make_enum(Color)
-            parse_variant = TypeBuilder.make_variant([parse_number, parse_color])
-            schema = "Variant: {variant:Number_or_Color}"
-            parser = Parser(schema, dict(Number_or_Color=parse_variant))
-        
-            # -- TEST VARIANT: With number, color and mismatch.
-            result = parser.parse("Variant: 42")
-            assert result["variant"] == 42
-            result = parser.parse("Variant: blue")
-            assert result["variant"] is Color.blue
-            result = parser.parse("Variant: __MISMATCH__")
-            assert not result
-        
-        
-        
-        Extended Parser with CardinalityField support
-        -------------------------------------------------------------------------------
-        
-        The parser extends the ``parse.Parser`` and adds the following functionality:
-        
-        * supports the CardinalityField naming scheme
-        * automatically creates missing type variants for types with
-          a CardinalityField by using the primary type converter for cardinality=1
-        * extends the provide type converter dictionary with new type variants.
-        
-        Example:
-        
-        .. code-block:: python
-        
-            # -- USE CASE: Parser with CardinalityField support.
-            # NOTE: Automatically adds missing type variants with CardinalityField part.
-            # USE:  parse_number() type converter from above.
-            from parse_type.cfparse import Parser
-        
-            # -- PREPARE: parser, adds missing type variant for cardinality 1..* (many)
-            type_dict = dict(Number=parse_number)
-            schema = "List: {numbers:Number+}"
-            parser = Parser(schema, type_dict)
-            assert "Number+" in type_dict, "Created missing type variant based on: Number"
-        
-            # -- USE: parser.
-            result = parser.parse("List: 1, 2, 3")
-            assert result["numbers"] == [1, 2, 3]
-        
+Author: Jens Engel
+Author-email: Jens Engel <jenisys@noreply.github.com>
+License: MIT
+Project-URL: Homepage, https://github.com/jenisys/parse_type
+Project-URL: Download, http://pypi.python.org/pypi/parse_type
+Project-URL: Source Code, https://github.com/jenisys/parse_type
+Project-URL: Issue Tracker, https://github.com/jenisys/parse_type/issues/
 Keywords: parse,parsing
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
+Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: develop
+Provides-Extra: testing
+License-File: LICENSE
+
+===============================================================================
+parse_type
+===============================================================================
+
+.. image:: https://github.com/jenisys/parse_type/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jenisys/parse_type/actions/workflows/test.yml
+    :alt: CI Build Status
+
+.. image:: https://img.shields.io/pypi/v/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type
+    :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/dm/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/l/parse_type.svg
+    :target: https://pypi.python.org/pypi/parse_type/
+    :alt: License
+
+
+`parse_type`_ extends the `parse`_ module (opposite of `string.format()`_)
+with the following features:
+
+* build type converters for common use cases (enum/mapping, choice)
+* build a type converter with a cardinality constraint (0..1, 0..*, 1..*)
+    from the type converter with cardinality=1.
+* compose a type converter from other type converters
+* an extended parser that supports the CardinalityField naming schema
+    and creates missing type variants (0..1, 0..*, 1..*) from the
+    primary type converter
+
+.. _parse_type: http://pypi.python.org/pypi/parse_type
+.. _parse:      http://pypi.python.org/pypi/parse
+.. _`string.format()`: http://docs.python.org/library/string.html#format-string-syntax
+
+
+Definitions
+-------------------------------------------------------------------------------
+
+*type converter*
+    A type converter function that converts a textual representation
+    of a value type into instance of this value type.
+    In addition, a type converter function is often annotated with attributes
+    that allows the `parse`_ module to use it in a generic way.
+    A type converter is also called a *parse_type* (a definition used here).
+
+*cardinality field*
+    A naming convention for related types that differ in cardinality.
+    A cardinality field is a type name suffix in the format of a field.
+    It allows parse format expression, ala::
+
+        "{person:Person}"     #< Cardinality: 1    (one; the normal case)
+        "{person:Person?}"    #< Cardinality: 0..1 (zero or one  = optional)
+        "{persons:Person*}"   #< Cardinality: 0..* (zero or more = many0)
+        "{persons:Person+}"   #< Cardinality: 1..* (one  or more = many)
+
+    This naming convention mimics the relationship descriptions in UML diagrams.
+
+
+Basic Example
+-------------------------------------------------------------------------------
+
+Define an own type converter for numbers (integers):
+
+.. code-block:: python
+
+    # -- USE CASE:
+    def parse_number(text):
+        return int(text)
+    parse_number.pattern = r"\d+"  # -- REGULAR EXPRESSION pattern for type.
+
+This is equivalent to:
+
+.. code-block:: python
+
+    import parse
+
+    @parse.with_pattern(r"\d+")
+    def parse_number(text):
+         return int(text)
+    assert hasattr(parse_number, "pattern")
+    assert parse_number.pattern == r"\d+"
+
+
+.. code-block:: python
+
+    # -- USE CASE: Use the type converter with the parse module.
+    schema = "Hello {number:Number}"
+    parser = parse.Parser(schema, dict(Number=parse_number))
+    result = parser.parse("Hello 42")
+    assert result is not None, "REQUIRE: text matches the schema."
+    assert result["number"] == 42
+
+    result = parser.parse("Hello XXX")
+    assert result is None, "MISMATCH: text does not match the schema."
+
+.. hint::
+
+    The described functionality above is standard functionality
+    of the `parse`_ module. It serves as introduction for the remaining cases.
+
+
+Cardinality
+-------------------------------------------------------------------------------
+
+Create an type converter for "ManyNumbers" (List, separated with commas)
+with cardinality "1..* = 1+" (many) from the type converter for a "Number".
+
+.. code-block:: python
+
+    # -- USE CASE: Create new type converter with a cardinality constraint.
+    # CARDINALITY: many := one or more (1..*)
+    from parse import Parser
+    from parse_type import TypeBuilder
+    parse_numbers = TypeBuilder.with_many(parse_number, listsep=",")
+
+    schema = "List: {numbers:ManyNumbers}"
+    parser = Parser(schema, dict(ManyNumbers=parse_numbers))
+    result = parser.parse("List: 1, 2, 3")
+    assert result["numbers"] == [1, 2, 3]
+
+
+Create an type converter for an "OptionalNumbers" with cardinality "0..1 = ?"
+(optional) from the type converter for a "Number".
+
+.. code-block:: python
+
+    # -- USE CASE: Create new type converter with cardinality constraint.
+    # CARDINALITY: optional := zero or one (0..1)
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_optional_number = TypeBuilder.with_optional(parse_number)
+    schema = "Optional: {number:OptionalNumber}"
+    parser = Parser(schema, dict(OptionalNumber=parse_optional_number))
+    result = parser.parse("Optional: 42")
+    assert result["number"] == 42
+    result = parser.parse("Optional: ")
+    assert result["number"] == None
+
+
+Enumeration (Name-to-Value Mapping)
+-------------------------------------------------------------------------------
+
+Create an type converter for an "Enumeration" from the description of
+the mapping as dictionary.
+
+.. code-block:: python
+
+    # -- USE CASE: Create a type converter for an enumeration.
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_enum_yesno = TypeBuilder.make_enum({"yes": True, "no": False})
+    parser = Parser("Answer: {answer:YesNo}", dict(YesNo=parse_enum_yesno))
+    result = parser.parse("Answer: yes")
+    assert result["answer"] == True
+
+
+Create an type converter for an "Enumeration" from the description of
+the mapping as an enumeration class (`Python 3.4 enum`_ or the `enum34`_
+backport; see also: `PEP-0435`_).
+
+.. code-block:: python
+
+    # -- USE CASE: Create a type converter for enum34 enumeration class.
+    # NOTE: Use Python 3.4 or enum34 backport.
+    from parse import Parser
+    from parse_type import TypeBuilder
+    from enum import Enum
+
+    class Color(Enum):
+        red   = 1
+        green = 2
+        blue  = 3
+
+    parse_enum_color = TypeBuilder.make_enum(Color)
+    parser = Parser("Select: {color:Color}", dict(Color=parse_enum_color))
+    result = parser.parse("Select: red")
+    assert result["color"] is Color.red
+
+.. _`Python 3.4 enum`: http://docs.python.org/3.4/library/enum.html#module-enum
+.. _enum34:   http://pypi.python.org/pypi/enum34
+.. _PEP-0435: http://www.python.org/dev/peps/pep-0435
+
+
+Choice (Name Enumeration)
+-------------------------------------------------------------------------------
+
+A Choice data type allows to select one of several strings.
+
+Create an type converter for an "Choice" list, a list of unique names
+(as string).
+
+.. code-block:: python
+
+    from parse import Parser
+    from parse_type import TypeBuilder
+
+    parse_choice_yesno = TypeBuilder.make_choice(["yes", "no"])
+    schema = "Answer: {answer:ChoiceYesNo}"
+    parser = Parser(schema, dict(ChoiceYesNo=parse_choice_yesno))
+    result = parser.parse("Answer: yes")
+    assert result["answer"] == "yes"
+
+
+Variant (Type Alternatives)
+-------------------------------------------------------------------------------
+
+Sometimes you need a type converter that can accept text for multiple
+type converter alternatives. This is normally called a "variant" (or: union).
+
+Create an type converter for an "Variant" type that accepts:
+
+* Numbers (positive numbers, as integer)
+* Color enum values (by name)
+
+.. code-block:: python
+
+    from parse import Parser, with_pattern
+    from parse_type import TypeBuilder
+    from enum import Enum
+
+    class Color(Enum):
+        red   = 1
+        green = 2
+        blue  = 3
+
+    @with_pattern(r"\d+")
+    def parse_number(text):
+        return int(text)
+
+    # -- MAKE VARIANT: Alternatives of different type converters.
+    parse_color = TypeBuilder.make_enum(Color)
+    parse_variant = TypeBuilder.make_variant([parse_number, parse_color])
+    schema = "Variant: {variant:Number_or_Color}"
+    parser = Parser(schema, dict(Number_or_Color=parse_variant))
+
+    # -- TEST VARIANT: With number, color and mismatch.
+    result = parser.parse("Variant: 42")
+    assert result["variant"] == 42
+    result = parser.parse("Variant: blue")
+    assert result["variant"] is Color.blue
+    result = parser.parse("Variant: __MISMATCH__")
+    assert not result
+
+
+
+Extended Parser with CardinalityField support
+-------------------------------------------------------------------------------
+
+The parser extends the ``parse.Parser`` and adds the following functionality:
+
+* supports the CardinalityField naming scheme
+* automatically creates missing type variants for types with
+  a CardinalityField by using the primary type converter for cardinality=1
+* extends the provide type converter dictionary with new type variants.
+
+Example:
+
+.. code-block:: python
+
+    # -- USE CASE: Parser with CardinalityField support.
+    # NOTE: Automatically adds missing type variants with CardinalityField part.
+    # USE:  parse_number() type converter from above.
+    from parse_type.cfparse import Parser
+
+    # -- PREPARE: parser, adds missing type variant for cardinality 1..* (many)
+    type_dict = dict(Number=parse_number)
+    schema = "List: {numbers:Number+}"
+    parser = Parser(schema, type_dict)
+    assert "Number+" in type_dict, "Created missing type variant based on: Number"
+
+    # -- USE: parser.
+    result = parser.parse("List: 1, 2, 3")
+    assert result["numbers"] == [1, 2, 3]
```

### Comparing `parse_type-0.6.0/parse_type.egg-info/SOURCES.txt` & `parse_type-0.6.1/parse_type.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .coveragerc
 .editorconfig
 CHANGES.txt
 LICENSE
 MANIFEST.in
 README.rst
 invoke.yaml
+pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
 bin/invoke
 bin/invoke.cmd
 bin/make_localpi.py
@@ -26,35 +27,27 @@
 parse_type.egg-info/SOURCES.txt
 parse_type.egg-info/dependency_links.txt
 parse_type.egg-info/requires.txt
 parse_type.egg-info/top_level.txt
 parse_type.egg-info/zip-safe
 py.requirements/all.txt
 py.requirements/basic.txt
-py.requirements/ci.travis.txt
+py.requirements/ci.github.testing.txt
 py.requirements/develop.txt
 py.requirements/docs.txt
 py.requirements/optional.txt
-py.requirements/py26_more.txt
 py.requirements/testing.txt
 tasks/__init__.py
 tasks/__main__.py
 tasks/_compat_shutil.py
-tasks/_dry_run.py
-tasks/_setup.py
-tasks/_tasklet_cleanup.py
 tasks/docs.py
+tasks/invoke_dry_run.py
 tasks/py.requirements.txt
 tasks/release.py
 tasks/test.py
-tasks/_vendor/README.rst
-tasks/_vendor/invoke.zip
-tasks/_vendor/path.py
-tasks/_vendor/pathlib.py
-tasks/_vendor/six.py
 tests/__init__.py
 tests/parse_type_test.py
 tests/test_builder.py
 tests/test_cardinality.py
 tests/test_cardinality_field.py
 tests/test_cardinality_field0.py
 tests/test_cfparse.py
```

### Comparing `parse_type-0.6.0/.editorconfig` & `parse_type-0.6.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.0/setup.py` & `parse_type-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,75 +49,82 @@
 
 
 # -----------------------------------------------------------------------------
 # SETUP:
 # -----------------------------------------------------------------------------
 setup(
     name = "parse_type",
-    version = "0.6.0",
+    version = "0.6.1",
     author = "Jens Engel",
     author_email = "jenisys@noreply.github.com",
     url = "https://github.com/jenisys/parse_type",
     download_url= "http://pypi.python.org/pypi/parse_type",
     description = "Simplifies to build parse types based on the parse module",
     long_description = long_description,
     keywords= "parse, parsing",
-    license = "BSD",
+    license = "MIT",
     packages = find_packages_by_root_package("parse_type"),
     include_package_data = True,
 
     # -- REQUIREMENTS:
     python_requires=">=2.7, !=3.0.*, !=3.1.*",
     install_requires=[
         "parse >= 1.18.0; python_version >= '3.0'",
         "parse >= 1.13.1; python_version <= '2.7'",
-        # -- MAYBE, related to issue #15:
-        # "parse == 1.13.1; python_version <= '2.7'",
         "enum34; python_version < '3.4'",
-        "six >= 1.11",
-        "ordereddict; python_version < '2.7'",
+        "six >= 1.15",
     ],
     tests_require=[
         "pytest <  5.0; python_version <  '3.0'", # >= 4.2
         "pytest >= 5.0; python_version >= '3.0'",
         "pytest-html >= 1.19.0",
-        # -- PYTHON 2.6 SUPPORT:
-        "unittest2; python_version < '2.7'",
     ],
     extras_require={
-        'docs': ["sphinx>=1.2"],
+        'docs': [
+            "Sphinx >=1.6",
+            "sphinx_bootstrap_theme >= 0.6.0"
+        ],
         'develop': [
+            "build >= 0.5.1",
+            "twine >= 1.13.0",
             "coverage >= 4.4",
-            "pytest <  5.0; python_version <  '3.0'", # >= 4.2
+            "pytest <  5.0; python_version <  '3.0'",  # >= 4.2
             "pytest >= 5.0; python_version >= '3.0'",
             "pytest-html >= 1.19.0",
             "pytest-cov",
-            "tox >= 2.8",
+            "tox >=2.8,<4.0",
+            "virtualenv <  20.22.0; python_version <= '3.6'",  # -- SUPPORT FOR: Python 2.7, Python <= 3.6
+            "virtualenv >= 20.0.0;  python_version >  '3.6'",
+            "ruff; python_version >=  '3.7'",
+            "pylint",
         ],
     },
 
     test_suite = "tests",
     test_loader = "setuptools.command.test:ScanningLoader",
     zip_safe = True,
 
     classifiers = [
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Code Generators",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "License :: OSI Approved :: BSD License",
     ],
     platforms = ['any'],
 )
```

### Comparing `parse_type-0.6.0/README.rst` & `parse_type-0.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ===============================================================================
 parse_type
 ===============================================================================
 
-.. image:: https://img.shields.io/travis/jenisys/parse_type/master.svg
-    :target: https://travis-ci.org/jenisys/parse_type
-    :alt: Travis CI Build Status
+.. image:: https://github.com/jenisys/parse_type/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jenisys/parse_type/actions/workflows/test.yml
+    :alt: CI Build Status
 
 .. image:: https://img.shields.io/pypi/v/parse_type.svg
     :target: https://pypi.python.org/pypi/parse_type
     :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/dm/parse_type.svg
     :target: https://pypi.python.org/pypi/parse_type
```

