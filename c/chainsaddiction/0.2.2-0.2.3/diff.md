# Comparing `tmp/chainsaddiction-0.2.2.tar.gz` & `tmp/chainsaddiction-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsaddiction-0.2.2.tar", last modified: Sun Jul  2 20:04:07 2023, max compression
+gzip compressed data, was "chainsaddiction-0.2.3.tar", last modified: Sun Jul  2 20:07:13 2023, max compression
```

## Comparing `chainsaddiction-0.2.2.tar` & `chainsaddiction-0.2.3.tar`

### file list

```diff
@@ -1,273 +1,272 @@
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.111814 chainsaddiction-0.2.2/
--rw-r--r--   0 pmind      (502) staff       (20)      235 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/.gitignore
--rw-r--r--   0 pmind      (502) staff       (20)       96 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/.gitmodules
--rw-r--r--   0 pmind      (502) staff       (20)      547 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/.readthedocs.yml
--rw-r--r--   0 pmind      (502) staff       (20)      121 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/CHANGELOG.md
--rw-r--r--   0 pmind      (502) staff       (20)     1487 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/LICENSE
--rw-r--r--   0 pmind      (502) staff       (20)      260 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/MANIFEST.in
--rw-r--r--   0 pmind      (502) staff       (20)     2018 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     3839 2023-07-02 20:04:07.110536 chainsaddiction-0.2.2/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     1211 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/README.md
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.721869 chainsaddiction-0.2.2/docs/
--rw-r--r--   0 pmind      (502) staff       (20)      584 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      791 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/make.bat
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.725517 chainsaddiction-0.2.2/docs/source/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.727913 chainsaddiction-0.2.2/docs/source/api/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.733788 chainsaddiction-0.2.2/docs/source/api/c/
--rw-r--r--   0 pmind      (502) staff       (20)      483 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/basics.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1792 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/dataset.rst
--rw-r--r--   0 pmind      (502) staff       (20)      279 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)      116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/internal.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.738460 chainsaddiction-0.2.2/docs/source/api/c/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)      200 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/poishmm/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     5120 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-hmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)     4161 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-params.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1952 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-probs.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2260 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/docs/source/api/c/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)      337 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.746968 chainsaddiction-0.2.2/docs/source/api/python/
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/python/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2123 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/docs/source/api/python/poishmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)      805 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/api/python/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1897 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/conf.py
--rw-r--r--   0 pmind      (502) staff       (20)     2229 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/docs/source/getting-started.rst
--rw-r--r--   0 pmind      (502) staff       (20)      526 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/docs/source/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.748875 chainsaddiction-0.2.2/docs/source/usrguide/
--rw-r--r--   0 pmind      (502) staff       (20)     1442 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/usrguide/examples.rst
--rw-r--r--   0 pmind      (502) staff       (20)      198 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/docs/source/usrguide/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.756395 chainsaddiction-0.2.2/include/
--rw-r--r--   0 pmind      (502) staff       (20)      464 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/include/chainsaddiction.h
--rw-r--r--   0 pmind      (502) staff       (20)      159 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/include/libvmath.h
--rw-r--r--   0 pmind      (502) staff       (20)     1079 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/pyproject.toml
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/requirements-dev.txt
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-07-02 20:04:07.112337 chainsaddiction-0.2.2/setup.cfg
--rw-r--r--   0 pmind      (502) staff       (20)     1458 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/setup.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.689206 chainsaddiction-0.2.2/src/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.786683 chainsaddiction-0.2.2/src/chainsaddiction/
--rw-r--r--   0 pmind      (502) staff       (20)      249 2023-07-02 14:18:19.000000 chainsaddiction-0.2.2/src/chainsaddiction/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     2025 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)     1953 2023-07-02 14:48:22.000000 chainsaddiction-0.2.2/src/chainsaddiction/dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)      301 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/err.h
--rw-r--r--   0 pmind      (502) staff       (20)      861 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/libma.c
--rw-r--r--   0 pmind      (502) staff       (20)     1831 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/libma.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.818089 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)     1240 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      294 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/__init__.pyi
--rw-r--r--   0 pmind      (502) staff       (20)     4383 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)     2212 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     1844 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-fwbw.c
--rw-r--r--   0 pmind      (502) staff       (20)     2153 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-fwbw.h
--rw-r--r--   0 pmind      (502) staff       (20)     4864 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)     2099 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     4540 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)     2116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      964 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)     1130 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)     9619 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-module.c
--rw-r--r--   0 pmind      (502) staff       (20)     1109 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     2263 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-object.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.831735 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1594 2023-07-02 11:49:32.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/Makefile
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.846773 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)      222 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/params-3s
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/ppr1
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/ppr2
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/ppr3
--rw-r--r--   0 pmind      (502) staff       (20)      119 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/ppr4
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/ppr5
--rw-r--r--   0 pmind      (502) staff       (20)      135 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
--rw-r--r--   0 pmind      (502) staff       (20)      874 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     4808 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)      290 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     6676 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)      542 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     1222 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)      216 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      699 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)      210 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/src/chainsaddiction/py.typed
--rw-r--r--   0 pmind      (502) staff       (20)     3293 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/read.c
--rw-r--r--   0 pmind      (502) staff       (20)     1556 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/read.h
--rw-r--r--   0 pmind      (502) staff       (20)      196 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/restrict.h
--rw-r--r--   0 pmind      (502) staff       (20)      335 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/scalar.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.853056 chainsaddiction-0.2.2/src/chainsaddiction/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      822 2023-07-02 14:18:30.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      593 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2464 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/test-dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)      626 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/test-dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/test-read.c
--rw-r--r--   0 pmind      (502) staff       (20)      397 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/tests/test-read.h
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/src/chainsaddiction/typing.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.864138 chainsaddiction-0.2.2/src/chainsaddiction/utils/
--rw-r--r--   0 pmind      (502) staff       (20)      430 2023-07-02 11:08:18.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      207 2023-06-30 09:02:51.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/__init__.pyi
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.869391 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1116 2023-07-02 14:25:01.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/log.txt
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-07-02 13:06:36.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2264 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/test-utils.c
--rw-r--r--   0 pmind      (502) staff       (20)      244 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/test-utils.h
--rw-r--r--   0 pmind      (502) staff       (20)     4798 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/utils-module.c
--rw-r--r--   0 pmind      (502) staff       (20)      795 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/utils-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     3119 2023-07-01 19:30:23.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/utils.c
--rw-r--r--   0 pmind      (502) staff       (20)     1467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/chainsaddiction/utils/utils.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.795729 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/
--rw-r--r--   0 pmind      (502) staff       (20)     3839 2023-07-02 20:04:06.000000 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     8013 2023-07-02 20:04:06.000000 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/SOURCES.txt
--rw-r--r--   0 pmind      (502) staff       (20)        1 2023-07-02 20:04:06.000000 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/dependency_links.txt
--rw-r--r--   0 pmind      (502) staff       (20)        6 2023-07-02 20:04:06.000000 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/requires.txt
--rw-r--r--   0 pmind      (502) staff       (20)       22 2023-07-02 20:04:06.000000 chainsaddiction-0.2.2/src/chainsaddiction.egg-info/top_level.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.884788 chainsaddiction-0.2.2/src/vmath/
--rw-r--r--   0 pmind      (502) staff       (20)      659 2023-07-02 10:49:38.000000 chainsaddiction-0.2.2/src/vmath/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      773 2023-07-02 10:49:20.000000 chainsaddiction-0.2.2/src/vmath/alloc.h
--rw-r--r--   0 pmind      (502) staff       (20)      440 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/config.h
--rw-r--r--   0 pmind      (502) staff       (20)     1473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/core.c
--rw-r--r--   0 pmind      (502) staff       (20)      932 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/core.h
--rw-r--r--   0 pmind      (502) staff       (20)     4047 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/print.h
--rw-r--r--   0 pmind      (502) staff       (20)     1349 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)     2907 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)      682 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/stats.c
--rw-r--r--   0 pmind      (502) staff       (20)     1008 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/stats.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.893609 chainsaddiction-0.2.2/src/vmath/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      807 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     1294 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2507 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)      301 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)     1086 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_stats.c
--rw-r--r--   0 pmind      (502) staff       (20)      248 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_stats.h
--rw-r--r--   0 pmind      (502) staff       (20)    23272 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)     1137 2023-07-02 20:03:27.000000 chainsaddiction-0.2.2/src/vmath/tests/test_vmath.h
--rw-r--r--   0 pmind      (502) staff       (20)    13402 2023-07-02 19:08:05.000000 chainsaddiction-0.2.2/src/vmath/vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)    18516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/src/vmath/vmath.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.900683 chainsaddiction-0.2.2/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      179 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/README
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.945737 chainsaddiction-0.2.2/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)     1299 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/S4_N100
--rw-r--r--   0 pmind      (502) staff       (20)     6535 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/S4_N500
--rw-r--r--   0 pmind      (502) staff       (20)      967 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/S4_N50_MID
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.947024 chainsaddiction-0.2.2/tests/data/centroids/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.972894 chainsaddiction-0.2.2/tests/data/centroids/2s/
--rw-r--r--   0 pmind      (502) staff       (20)        8 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       43 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68421 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    72888 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.991819 chainsaddiction-0.2.2/tests/data/centroids/3s/
--rw-r--r--   0 pmind      (502) staff       (20)       12 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      187 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102650 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       64 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102555 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   105803 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.015449 chainsaddiction-0.2.2/tests/data/centroids/4s/
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      356 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135537 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135631 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   141473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.039608 chainsaddiction-0.2.2/tests/data/centroids/5s/
--rw-r--r--   0 pmind      (502) staff       (20)       44 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      553 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170825 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)      107 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170730 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   176569 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)     6164 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/centroids/centroids
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.041764 chainsaddiction-0.2.2/tests/data/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.058850 chainsaddiction-0.2.2/tests/data/earthquakes/2s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4872 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4826 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     5138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       27 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       42 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.075532 chainsaddiction-0.2.2/tests/data/earthquakes/3s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7304 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7249 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       50 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      210 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.087715 chainsaddiction-0.2.2/tests/data/earthquakes/4s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9724 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9672 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9894 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       71 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      368 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       88 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.100505 chainsaddiction-0.2.2/tests/data/earthquakes/5s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12048 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12274 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       76 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      571 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      315 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/earthquakes/earthquakes
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/empty
--rw-r--r--   0 pmind      (502) staff       (20)       31 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/params_2s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/params_3s
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/params_4s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/params_4s_MID
--rw-r--r--   0 pmind      (502) staff       (20)      206 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/test_15_100_50
--rw-r--r--   0 pmind      (502) staff       (20)       10 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/data/wrong_format
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.101292 chainsaddiction-0.2.2/tests/params/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:06.699523 chainsaddiction-0.2.2/tests/params/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.104518 chainsaddiction-0.2.2/tests/params/earthquakes/3/
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/3/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/3/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/3/random.p
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:04:07.108925 chainsaddiction-0.2.2/tests/params/earthquakes/4/
--rw-r--r--   0 pmind      (502) staff       (20)      250 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/4/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      228 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/4/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      232 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/earthquakes/4/random.p
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/params/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      862 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/test-ext-earthquakes.py
--rw-r--r--   0 pmind      (502) staff       (20)     1069 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/test-utils.py
--rw-r--r--   0 pmind      (502) staff       (20)     1084 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tests/utils.py
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.2/tox.ini
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:13.002029 chainsaddiction-0.2.3/
+-rw-r--r--   0 pmind      (502) staff       (20)      235 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/.gitignore
+-rw-r--r--   0 pmind      (502) staff       (20)       96 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/.gitmodules
+-rw-r--r--   0 pmind      (502) staff       (20)      336 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 pmind      (502) staff       (20)      335 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/CHANGELOG.md
+-rw-r--r--   0 pmind      (502) staff       (20)     1487 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/LICENSE
+-rw-r--r--   0 pmind      (502) staff       (20)       58 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/MANIFEST.in
+-rw-r--r--   0 pmind      (502) staff       (20)     1938 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-02 20:07:12.999961 chainsaddiction-0.2.3/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)     1223 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/README.md
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.778272 chainsaddiction-0.2.3/docs/
+-rw-r--r--   0 pmind      (502) staff       (20)      584 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      791 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/make.bat
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.781376 chainsaddiction-0.2.3/docs/source/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.782178 chainsaddiction-0.2.3/docs/source/api/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.787760 chainsaddiction-0.2.3/docs/source/api/c/
+-rw-r--r--   0 pmind      (502) staff       (20)      483 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/basics.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1792 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/dataset.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      279 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/internal.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.792087 chainsaddiction-0.2.3/docs/source/api/c/poishmm/
+-rw-r--r--   0 pmind      (502) staff       (20)      200 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     5120 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-hmm.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     4161 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-params.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1952 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-probs.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     2260 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/api/c/utils.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      337 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.794834 chainsaddiction-0.2.3/docs/source/api/python/
+-rw-r--r--   0 pmind      (502) staff       (20)      169 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/python/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     2123 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/api/python/poishmm.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      805 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/python/utils.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1897 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/conf.py
+-rw-r--r--   0 pmind      (502) staff       (20)     2229 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/docs/source/getting-started.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      526 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.796251 chainsaddiction-0.2.3/docs/source/usrguide/
+-rw-r--r--   0 pmind      (502) staff       (20)     1442 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/usrguide/examples.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      198 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/usrguide/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.798458 chainsaddiction-0.2.3/include/
+-rw-r--r--   0 pmind      (502) staff       (20)      464 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/include/chainsaddiction.h
+-rw-r--r--   0 pmind      (502) staff       (20)      159 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/include/libvmath.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1079 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/pyproject.toml
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/requirements-dev.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       38 2023-07-02 20:07:13.002449 chainsaddiction-0.2.3/setup.cfg
+-rw-r--r--   0 pmind      (502) staff       (20)     1458 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/setup.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.759240 chainsaddiction-0.2.3/src/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.809973 chainsaddiction-0.2.3/src/chainsaddiction/
+-rw-r--r--   0 pmind      (502) staff       (20)      249 2023-07-02 14:18:19.000000 chainsaddiction-0.2.3/src/chainsaddiction/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)     2026 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/dataset.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1953 2023-07-02 14:48:22.000000 chainsaddiction-0.2.3/src/chainsaddiction/dataset.h
+-rw-r--r--   0 pmind      (502) staff       (20)      301 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/err.h
+-rw-r--r--   0 pmind      (502) staff       (20)      861 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/libma.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1831 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/libma.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.828990 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/
+-rw-r--r--   0 pmind      (502) staff       (20)     1240 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      294 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/__init__.pyi
+-rw-r--r--   0 pmind      (502) staff       (20)     4383 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2212 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1844 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2153 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4864 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2099 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4534 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.h
+-rw-r--r--   0 pmind      (502) staff       (20)      964 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1130 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.h
+-rw-r--r--   0 pmind      (502) staff       (20)     9619 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1109 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.h
+-rw-r--r--   0 pmind      (502) staff       (20)     2263 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-object.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.841528 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)     1594 2023-07-02 11:49:32.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/Makefile
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.847042 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/
+-rw-r--r--   0 pmind      (502) staff       (20)      222 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
+-rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/params-3s
+-rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/params-4s
+-rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr1
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr2
+-rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr3
+-rw-r--r--   0 pmind      (502) staff       (20)      119 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr4
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr5
+-rw-r--r--   0 pmind      (502) staff       (20)      135 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
+-rw-r--r--   0 pmind      (502) staff       (20)      896 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     4808 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.c
+-rw-r--r--   0 pmind      (502) staff       (20)      294 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.h
+-rw-r--r--   0 pmind      (502) staff       (20)     6676 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
+-rw-r--r--   0 pmind      (502) staff       (20)      546 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1239 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.c
+-rw-r--r--   0 pmind      (502) staff       (20)      220 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.h
+-rw-r--r--   0 pmind      (502) staff       (20)      699 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.c
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.h
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/py.typed
+-rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/read.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1556 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/read.h
+-rw-r--r--   0 pmind      (502) staff       (20)      196 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/restrict.h
+-rw-r--r--   0 pmind      (502) staff       (20)      335 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/scalar.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.850698 chainsaddiction-0.2.3/src/chainsaddiction/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      822 2023-07-02 14:18:30.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      593 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2464 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.c
+-rw-r--r--   0 pmind      (502) staff       (20)      626 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.h
+-rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.c
+-rw-r--r--   0 pmind      (502) staff       (20)      397 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.h
+-rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/typing.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.855020 chainsaddiction-0.2.3/src/chainsaddiction/utils/
+-rw-r--r--   0 pmind      (502) staff       (20)      430 2023-07-02 11:08:18.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      207 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/__init__.pyi
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.859702 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)     1116 2023-07-02 14:25:01.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      169 2023-07-02 13:06:36.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2280 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.c
+-rw-r--r--   0 pmind      (502) staff       (20)      248 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4882 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.c
+-rw-r--r--   0 pmind      (502) staff       (20)      795 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.h
+-rw-r--r--   0 pmind      (502) staff       (20)     3119 2023-07-01 19:30:23.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.813672 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/
+-rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)     7974 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/SOURCES.txt
+-rw-r--r--   0 pmind      (502) staff       (20)        1 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/dependency_links.txt
+-rw-r--r--   0 pmind      (502) staff       (20)        6 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/requires.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       22 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/top_level.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.872678 chainsaddiction-0.2.3/src/vmath/
+-rw-r--r--   0 pmind      (502) staff       (20)      659 2023-07-02 10:49:38.000000 chainsaddiction-0.2.3/src/vmath/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      773 2023-07-02 10:49:20.000000 chainsaddiction-0.2.3/src/vmath/alloc.h
+-rw-r--r--   0 pmind      (502) staff       (20)      440 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/config.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/core.c
+-rw-r--r--   0 pmind      (502) staff       (20)      932 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/core.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4047 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/print.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1349 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/rnd.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2907 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/rnd.h
+-rw-r--r--   0 pmind      (502) staff       (20)      682 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/stats.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1008 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/stats.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.884006 chainsaddiction-0.2.3/src/vmath/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      807 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)     1294 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2573 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_rnd.c
+-rw-r--r--   0 pmind      (502) staff       (20)      344 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_rnd.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_stats.c
+-rw-r--r--   0 pmind      (502) staff       (20)      273 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_stats.h
+-rw-r--r--   0 pmind      (502) staff       (20)    23250 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_vmath.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1182 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_vmath.h
+-rw-r--r--   0 pmind      (502) staff       (20)    13402 2023-07-02 19:08:05.000000 chainsaddiction-0.2.3/src/vmath/vmath.c
+-rw-r--r--   0 pmind      (502) staff       (20)    18516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/vmath.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.891368 chainsaddiction-0.2.3/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      179 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/README
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.898804 chainsaddiction-0.2.3/tests/data/
+-rw-r--r--   0 pmind      (502) staff       (20)     1299 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N100
+-rw-r--r--   0 pmind      (502) staff       (20)     6535 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N500
+-rw-r--r--   0 pmind      (502) staff       (20)      967 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N50_MID
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.900416 chainsaddiction-0.2.3/tests/data/centroids/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.909180 chainsaddiction-0.2.3/tests/data/centroids/2s/
+-rw-r--r--   0 pmind      (502) staff       (20)        8 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    68467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       43 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    68421 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    72888 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.919295 chainsaddiction-0.2.3/tests/data/centroids/3s/
+-rw-r--r--   0 pmind      (502) staff       (20)       12 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      187 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   102650 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       64 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   102555 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   105803 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.931388 chainsaddiction-0.2.3/tests/data/centroids/4s/
+-rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      356 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   135537 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   135631 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   141473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.946299 chainsaddiction-0.2.3/tests/data/centroids/5s/
+-rw-r--r--   0 pmind      (502) staff       (20)       44 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      553 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   170825 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      107 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   170730 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   176569 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/local-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     6164 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/centroids
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.947080 chainsaddiction-0.2.3/tests/data/earthquakes/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.958894 chainsaddiction-0.2.3/tests/data/earthquakes/2s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     4872 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     4826 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     5138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       27 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       42 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.968229 chainsaddiction-0.2.3/tests/data/earthquakes/3s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7304 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7249 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       50 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      210 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.980755 chainsaddiction-0.2.3/tests/data/earthquakes/4s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9724 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9672 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9894 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       71 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      368 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       88 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.991639 chainsaddiction-0.2.3/tests/data/earthquakes/5s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12048 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12274 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       76 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      571 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/local-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      315 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/earthquakes
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/empty
+-rw-r--r--   0 pmind      (502) staff       (20)       31 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_2s
+-rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_3s
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_4s
+-rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_4s_MID
+-rw-r--r--   0 pmind      (502) staff       (20)      206 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/test_15_100_50
+-rw-r--r--   0 pmind      (502) staff       (20)       10 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/wrong_format
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.992372 chainsaddiction-0.2.3/tests/params/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.766045 chainsaddiction-0.2.3/tests/params/earthquakes/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.994610 chainsaddiction-0.2.3/tests/params/earthquakes/3/
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/linear.p
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/quantile.p
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/random.p
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.998175 chainsaddiction-0.2.3/tests/params/earthquakes/4/
+-rw-r--r--   0 pmind      (502) staff       (20)      250 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/linear.p
+-rw-r--r--   0 pmind      (502) staff       (20)      228 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/quantile.p
+-rw-r--r--   0 pmind      (502) staff       (20)      232 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/random.p
+-rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/params-4s
+-rw-r--r--   0 pmind      (502) staff       (20)      862 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/test-ext-earthquakes.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1069 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/test-utils.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1084 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/utils.py
+-rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tox.ini
```

### Comparing `chainsaddiction-0.2.2/LICENSE` & `chainsaddiction-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/Makefile` & `chainsaddiction-0.2.3/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -37,21 +37,18 @@
 	@echo '    pkg        Build the package under build/.'
 	@echo '    ext        Recompile the extension module.'
 	@echo '    check      Run extension module tests.'
 	@echo '    vmath      Rebuild vmath.'
 
 
 install:
-	python3 setup.py install 
+	pip3 install .
 
-pkg:
-	python3 setup.py --quiet build --force
-
-ext:
-	python3 setup.py --quiet build_ext --force
+build:
+	python3 -m build
 
 check:
 	make check -C tests
 
 vmath:
 	make clean -C src/vmath
 	make -C src/vmath
@@ -74,8 +71,8 @@
 	@echo 'BUILD_DIR:      $(build_dir)'
 	@echo 'BIN_DIR:        $(bin_dir)'
 	@echo 'OBJ_DIR:        $(obj_dir)'
 	@echo 'OBJS:           $(objs)'
 	@echo 'TEST_ROOT_DIR:  $(test_root_dir)'
 	@echo 'TEST_SRC_DIR:   $(test_src_dir)'
 
-.PHONY: check test clean distclean
+.PHONY: build check clean distclean
```

### Comparing `chainsaddiction-0.2.2/PKG-INFO` & `chainsaddiction-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.2
+Version: 0.2.3
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -55,16 +55,16 @@
 
 ## Installation
 ### Prerequisites
 
 The installation of ChainsAddiction requires to following tools to be installed
 on your system:
 
-- Python >= 3.7
-- pip
+- Python >= 3.9
+- pip, setuptools
 - C compiler
 
 
 ### Install from PyPi
 
 You can install chainsaddiction from PyPi with:
```

### Comparing `chainsaddiction-0.2.2/README.md` & `chainsaddiction-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 ## Installation
 ### Prerequisites
 
 The installation of ChainsAddiction requires to following tools to be installed
 on your system:
 
-- Python >= 3.7
-- pip
+- Python >= 3.9
+- pip, setuptools
 - C compiler
 
 
 ### Install from PyPi
 
 You can install chainsaddiction from PyPi with:
```

### Comparing `chainsaddiction-0.2.2/docs/Makefile` & `chainsaddiction-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/make.bat` & `chainsaddiction-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/c/dataset.rst` & `chainsaddiction-0.2.3/docs/source/api/c/dataset.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-hmm.rst` & `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-hmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-params.rst` & `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-params.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/c/poishmm/pois-probs.rst` & `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-probs.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/c/utils.rst` & `chainsaddiction-0.2.3/docs/source/api/c/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/python/poishmm.rst` & `chainsaddiction-0.2.3/docs/source/api/python/poishmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/api/python/utils.rst` & `chainsaddiction-0.2.3/docs/source/api/python/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/conf.py` & `chainsaddiction-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/getting-started.rst` & `chainsaddiction-0.2.3/docs/source/getting-started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 Prerequisites
 ===============================================================================
 
 ChainsAddiction provides a Python extension module that needs to be compiled
 before you can use it. Therefore, your system has to meet the following
 requirements:
 
-* Python >= 3.7
+* Python >= 3.9
 * pip and setuptools installed
 * C compiler (Windows and GNU/Linux only)
 
 No matter which operating system you use, the first step is to check the
 currently installed Python version. To do so, open a terminal and execute the
 following command:
 
 .. code-block:: sh
 
     python --version
 
 .. note::
 
    The Python interpreter may be available under different names, such as ``python3``, or
-   ``python3.7``, etc, depending on your operating system and virtual
+   ``python3.9``, etc, depending on your operating system and virtual
    environment setup.
 
 
 Installation
 ===============================================================================
 
 ChainsAddiction is available on `PyPi`_. That means you can download and
```

### Comparing `chainsaddiction-0.2.2/docs/source/index.rst` & `chainsaddiction-0.2.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/docs/source/usrguide/examples.rst` & `chainsaddiction-0.2.3/docs/source/usrguide/examples.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/pyproject.toml` & `chainsaddiction-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chainsaddiction"
-version = "0.2.2"
+version = "0.2.3"
 authors = [{name = "Michael Blaß", email = "mblass@posteo.net"}]
 description = "HMM with Poisson-distributed latent variables."
 keywords = ["hmm", "poisson", "hidden-markov model"]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: BSD License",
```

### Comparing `chainsaddiction-0.2.2/setup.py` & `chainsaddiction-0.2.3/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 from pathlib import Path
-from setuptools import setup, Extension
 from typing import Generator
 
 import numpy as np
+from setuptools import setup, Extension
 
 
 def cglob(path: str) -> Generator[str, None, None]:
     """Generate all .c files in ``path``."""
     return (f'{src!s}' for src in Path(path).glob('*.c'))
 
 def list_source_files (paths: tuple[str, ...]) -> list[str]:
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/dataset.c` & `chainsaddiction-0.2.3/src/chainsaddiction/dataset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #include "dataset.h"
 
 
 DataSet *
 DataSet_NewEmpty (void)
 {
-    DataSet *this = malloc (sizeof this);
+    DataSet *this = malloc (sizeof *this);
     if (this == NULL)
     {
         Ca_ErrMsg ("Could not allocate data set.");
     }
     else
     {
         this->data = NULL;
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/dataset.h` & `chainsaddiction-0.2.3/src/chainsaddiction/dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/libma.c` & `chainsaddiction-0.2.3/src/chainsaddiction/libma.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/libma.h` & `chainsaddiction-0.2.3/src/chainsaddiction/libma.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/Makefile` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-em.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-em.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-fwbw.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-fwbw.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-hmm.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-hmm.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-params.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.c`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 PoisParams *
 PoisParams_NewFromFile (
     const char *fpath)
 {
     int err = 0;
-    unsigned int n_lines = 0;
+    size_t n_lines = 0;
     scalar mbuff = 0l;
     PoisParams *out = NULL;
     FILE *dfd = Ca_OpenFile (fpath, "r");
     Ca_CountLines (dfd, &n_lines);
     if (n_lines == 0)
     {
         fprintf (stderr, "Empty file: %s\n", fpath);
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-params.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-probs.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/pois-probs.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-module.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-module.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/poishmm-object.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-object.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/Makefile` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/runtest.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/runtest.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "test-pois-probs.h"
 #include "test-pois-params.h"
 #include "test-pois-hmm.h"
 #include "test-pois-em.h"
+#include "unittest.h"
 
 int
 main (void)
 {
     SETUP;
 
     RUN_TEST (test__PoisParams_New);
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-em.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-hmm.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-hmm.h` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #ifndef test_pois_hmm_h
 #define test_pois_hmm_h
 
 #include <math.h>
 #include <string.h>
-#include "unittest.h"
+#include "assertations.h"
 #include "../pois-hmm.h"
 
 bool test__PoisHmm_New (void);
 bool test__PoisHmm_Init (void);
 bool test__PoisHmm_InitRandom (void);
 bool test__PoisHmm_InitRandom_sorted_lambda (void);
 bool test__PoisHmm_LogLikelihood (void);
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-params.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.c`

 * *Files 26% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     PoisParams *params = PoisParams_New (m_states);
 
     for (size_t i=0; i<m_states; i++) {
         if (fpclassify (params->lambda[i]) != FP_ZERO ||
             fpclassify (params->delta[i]) != FP_ZERO)
         {
             PoisParams_Delete (params);
-            return true;
+            return UT_FAILURE;
         }
     }
 
     for (size_t i=0; i<m_states*m_states; i++) {
         if (fpclassify (params->gamma[i]) != FP_ZERO)
         {
             PoisParams_Delete (params);
-            return true;
+            return UT_FAILURE;
         }
     }
 
     PoisParams_Delete (params);
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__PoisParams_NewFromFile (void)
 {
     enum { FNAME_LEN_MAX = 100, N_FILES = 5};
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/poishmm/tests/test-pois-probs.c` & `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/read.c` & `chainsaddiction-0.2.3/src/chainsaddiction/read.c`

 * *Files 2% similar despite different names*

```diff
@@ -54,36 +54,28 @@
 
 
 void
 Ca_CountLines (FILE *stream, size_t *line_cnt)
 {
     int fp_err = 1;
     int chr = 0;
-    fpos_t fp_start = 0;
-    fpos_t fp_current = 0;
+    fpos_t fp_current;
 
     if (stream == NULL)
     {
         PERISH ("File pointer points to NULL");
     }
 
     fp_err = fgetpos (stream, &fp_current);
     if (fp_err)
     {
         PERISH ("Could not get file position");
     }
 
-    if (fp_current != fp_start)
-    {
-        fp_err = fsetpos (stream, &fp_start);
-        if (fp_err)
-        {
-            PERISH ("Could not set file position");
-        }
-    }
+    rewind (stream);
 
     while (true)
     {
         chr = getc (stream);
         if (chr == EOF) break;
 
         if (chr == '\n')
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/read.h` & `chainsaddiction-0.2.3/src/chainsaddiction/read.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/tests/Makefile` & `chainsaddiction-0.2.3/src/chainsaddiction/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/tests/runtest.c` & `chainsaddiction-0.2.3/src/chainsaddiction/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/tests/test-dataset.c` & `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/tests/test-dataset.h` & `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/tests/test-read.c` & `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/Makefile` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/tests/test-utils.c` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+#include <stdio.h>
 #include "test-utils.h"
 
-
 bool test__local_decoding (void)
 {
 #ifdef datapath
 #undef datapath
 #endif
 #define datapath "../../../../tests/data/earthquakes/3s/"
     enum {
@@ -23,15 +23,14 @@
     if (lcsp == NULL || xpct == NULL || dec == NULL)
     {
         DataSet_Delete (lcsp);
         DataSet_Delete (xpct);
         FREE (dec);
         return UT_FAILURE;
     }
-
     local_decoding (n_obs, m_states, lcsp->data, dec);
 
     for (size_t i = 0; i < n_obs; i++)
     {
         err = ((size_t)xpct->data[i] != dec[i]) ? true : false;
         if (err) break;
     }
@@ -50,15 +49,14 @@
 #endif
 #define datapath "../../../../tests/data/earthquakes/3s/"
 
     enum {
         m_states = 3,
         n_obs    = 107
     };
-
     bool    err     = false;
     size_t  *dec    = NULL;
     DataSet *lcsp   = NULL;
     DataSet *lgamma = NULL;
     DataSet *ldelta = NULL;
     DataSet *xpct   = NULL;
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/utils-module.c` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.c`

 * *Files 3% similar despite different names*

```diff
@@ -68,19 +68,20 @@
 {
     UNUSED (self);
 
     npy_intp *shape_lcsp = NULL;
     PyObject *pyo_lgamma  = NULL;
     PyObject *pyo_ldelta  = NULL;
     PyObject *pyo_lcsp   = NULL;
-    PyObject *arr_states  = NULL;
+    PyObject *pyo_states  = NULL;
 
     PyArrayObject *arr_lgamma  = NULL;
     PyArrayObject *arr_ldelta  = NULL;
     PyArrayObject *arr_lcsp   = NULL;
+    PyArrayObject *arr_states = NULL;
 
     if (!PyArg_ParseTuple (args, "OOO", &pyo_lgamma, &pyo_ldelta, &pyo_lcsp))
     {
         const char msg[] = "global_decoding: Could not parse args.";
         PyErr_SetString (PyExc_TypeError, msg);
         goto fail;
     }
@@ -118,33 +119,34 @@
     {
         const char msg[] = "lcsp has dimension != 2.";
         PyErr_SetString (PyExc_TypeError, msg);
         goto fail;
     }
 
     shape_lcsp = PyArray_SHAPE (arr_lcsp);
-    arr_states  = PyArray_SimpleNew (PyCh_VECTOR, shape_lcsp, NPY_ULONG);
-    if (arr_states == NULL)
+    pyo_states = PyArray_SimpleNew (PyCh_VECTOR, shape_lcsp, NPY_ULONG);
+    if (pyo_states == NULL)
     {
         const char msg[] = "global_decoding: Could not allocate states object.";
         PyErr_SetString (PyExc_TypeError, msg);
         goto fail;
     }
+    arr_states = (PyArrayObject *) pyo_states;
 
     global_decoding ((size_t) shape_lcsp[0], (size_t) shape_lcsp[1],
             (long double *) PyArray_DATA (arr_lgamma),
             (long double *) PyArray_DATA (arr_ldelta),
             (long double *) PyArray_DATA (arr_lcsp),
             (size_t *) PyArray_DATA (arr_states));
 
     Py_DECREF (arr_lgamma);
     Py_DECREF (arr_ldelta);
     Py_DECREF (arr_lcsp);
     Py_INCREF (arr_states);
-    return arr_states;
+    return pyo_states;
 
 fail:
     Py_XDECREF (arr_lgamma);
     Py_XDECREF (arr_ldelta);
     Py_XDECREF (arr_lcsp);
     Py_XDECREF (arr_states);
     return NULL;
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/utils-module.h` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/utils.c` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction/utils/utils.h` & `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction.egg-info/PKG-INFO` & `chainsaddiction-0.2.3/src/chainsaddiction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.2
+Version: 0.2.3
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -55,16 +55,16 @@
 
 ## Installation
 ### Prerequisites
 
 The installation of ChainsAddiction requires to following tools to be installed
 on your system:
 
-- Python >= 3.7
-- pip
+- Python >= 3.9
+- pip, setuptools
 - C compiler
 
 
 ### Install from PyPi
 
 You can install chainsaddiction from PyPi with:
```

### Comparing `chainsaddiction-0.2.2/src/chainsaddiction.egg-info/SOURCES.txt` & `chainsaddiction-0.2.3/src/chainsaddiction.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .gitignore
 .gitmodules
-.readthedocs.yml
+.readthedocs.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements-dev.txt
@@ -93,15 +93,14 @@
 src/chainsaddiction/utils/Makefile
 src/chainsaddiction/utils/__init__.pyi
 src/chainsaddiction/utils/utils-module.c
 src/chainsaddiction/utils/utils-module.h
 src/chainsaddiction/utils/utils.c
 src/chainsaddiction/utils/utils.h
 src/chainsaddiction/utils/tests/Makefile
-src/chainsaddiction/utils/tests/log.txt
 src/chainsaddiction/utils/tests/runtest.c
 src/chainsaddiction/utils/tests/test-utils.c
 src/chainsaddiction/utils/tests/test-utils.h
 src/vmath/Makefile
 src/vmath/alloc.h
 src/vmath/config.h
 src/vmath/core.c
```

### Comparing `chainsaddiction-0.2.2/src/vmath/Makefile` & `chainsaddiction-0.2.3/src/vmath/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/alloc.h` & `chainsaddiction-0.2.3/src/vmath/alloc.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/core.c` & `chainsaddiction-0.2.3/src/vmath/core.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/core.h` & `chainsaddiction-0.2.3/src/vmath/core.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/print.h` & `chainsaddiction-0.2.3/src/vmath/print.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/rnd.c` & `chainsaddiction-0.2.3/src/vmath/rnd.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/rnd.h` & `chainsaddiction-0.2.3/src/vmath/rnd.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/stats.c` & `chainsaddiction-0.2.3/src/vmath/stats.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/stats.h` & `chainsaddiction-0.2.3/src/vmath/stats.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/Makefile` & `chainsaddiction-0.2.3/src/vmath/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/runtest.c` & `chainsaddiction-0.2.3/src/vmath/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/test_rnd.c` & `chainsaddiction-0.2.3/src/vmath/tests/test_rnd.c`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         SR_UB  =  100,
     };
 
     for (size_t i = 0; i < N_ITER; i++)
     {
         if (!ASSERT_IN_RANGE (rnd_int (SR_LB, SR_UB), SR_LB, SR_UB))
         {
-            return true;
+            return UT_FAILURE;
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__v_rnd_int (void)
 {
     enum setup {
@@ -37,37 +37,37 @@
         int arr[N_ELEM] = { IVAL };
         v_rnd_int (N_ELEM, SR_LB, SR_UB, arr);
 
         for (size_t i = 0; i < N_ELEM; i++)
         {
             if (!ASSERT_IN_RANGE (arr[i], SR_LB, SR_UB) || !isfinite (arr[i]))
             {
-                return true;
+                return UT_FAILURE;
             }
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__rnd_scalar (void)
 {
     enum setup { N_ITER = 200u };
     const scalar SR_LB = -100.0L;
     const scalar SR_UB =  100.0L;
 
     for (size_t i = 0; i < N_ITER; i++)
     {
         if (!ASSERT_IN_RANGE (rnd_scalar (SR_LB, SR_UB), SR_LB, SR_UB))
         {
-            return true;
+            return UT_FAILURE;
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__v_rnd_scalar (void)
 {
     enum setup { N_ELEM = 200u };
@@ -78,18 +78,18 @@
     scalar arr[N_ELEM] = { IVAL };
     v_rnd_scalar (N_ELEM, SR_LB, SR_UB, arr);
 
     for (size_t i = 0; i < N_ELEM; i++)
     {
         if (!ASSERT_IN_RANGE (arr[i], SR_LB, SR_UB) || !isfinite (arr[i]))
         {
-            return true;
+            return UT_FAILURE;
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__sample (void)
 {
     enum setup { N_ELEM = 200u };
@@ -97,18 +97,18 @@
     const scalar SR_UB = 1.0L;
 
     for (size_t i = 0; i < N_ELEM; i++)
     {
         scalar val = rnd_sample ();
         if (!ASSERT_IN_RANGE (val, SR_LB, SR_UB) || !isfinite (val))
         {
-            return true;
+            return UT_FAILURE;
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test__v_sample (void)
 {
     enum setup { N_ELEM = 200u, N_ITER =  10u, };
@@ -121,13 +121,13 @@
         scalar arr[N_ELEM] = { IVAL };
         v_rnd_sample (N_ELEM, arr);
 
         for (size_t i = 0; i < N_ELEM; i++)
         {
             if (!ASSERT_IN_RANGE (arr[i], SR_LB, SR_UB) || !isfinite (arr[i]))
             {
-                return true;
+                return UT_FAILURE;
             }
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
```

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/test_stats.c` & `chainsaddiction-0.2.3/src/vmath/tests/test_stats.c`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         for (size_t i = 0; i < OOM; i++)
         {
             long variate = (long) pow (10.0, i);
             scalar res = poisson_pmf (lambda, variate);
             /*printf ("Lambda: %10.Lf\t variate: %10.ld\t pmf: %20.15Lg\n", lambda, variate, res);*/
             if (isinf (res) || isnan (res))
             {
-                return true;
+                return UT_FAILURE;
             }
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
 
 
 bool
 test_poisson_logpmf (void)
 {
     for (size_t oom = 0; oom < OOM; oom++)
@@ -31,13 +31,13 @@
         for (size_t i = 0; i < OOM; i++)
         {
             long variate = (long) pow (10.0, i);
             scalar res = poisson_logpmf (lambda, variate);
             /*printf ("Lambda: %10.Lf\t variate: %10.ld\t log_pmf: %20.15Lf\n", lambda, variate, res);*/
             if (isinf (res) || isnan (res))
             {
-                return true;
+                return UT_FAILURE;
             }
         }
     }
-    return false;
+    return UT_SUCCESS;
 }
```

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/test_vmath.c` & `chainsaddiction-0.2.3/src/vmath/tests/test_vmath.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#include "unittest.h"
 #include "test_vmath.h"
 
 
 bool
 test__v_sum (void)
 {
     enum setup {
```

### Comparing `chainsaddiction-0.2.2/src/vmath/tests/test_vmath.h` & `chainsaddiction-0.2.3/src/vmath/tests/test_vmath.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #ifndef test_vmath_h
 #define test_vmath_h
 
+#include <assert.h>
+#include <stdbool.h>
 #include "config.h"
-#include "unittest.h"
+#include "assertations.h"
 #include "rnd.h"
 #include "vmath.h"
 
 
 bool test__strided_max (void);
 
 bool test__v_sum (void);
```

### Comparing `chainsaddiction-0.2.2/src/vmath/vmath.c` & `chainsaddiction-0.2.3/src/vmath/vmath.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/src/vmath/vmath.h` & `chainsaddiction-0.2.3/src/vmath/vmath.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/S4_N100` & `chainsaddiction-0.2.3/tests/data/S4_N100`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/S4_N500` & `chainsaddiction-0.2.3/tests/data/S4_N500`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/S4_N50_MID` & `chainsaddiction-0.2.3/tests/data/S4_N50_MID`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/2s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/centroids/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/2s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/centroids/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/2s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/centroids/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/3s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/centroids/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/3s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/centroids/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/3s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/centroids/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/4s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/centroids/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/4s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/centroids/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/4s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/centroids/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/gamma.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/gamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/global-decoding.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/global-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/5s/local-decoding.txt` & `chainsaddiction-0.2.3/tests/data/centroids/5s/local-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/centroids/centroids` & `chainsaddiction-0.2.3/tests/data/centroids/centroids`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/2s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/2s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/2s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/3s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/3s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/3s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/4s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/4s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/4s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/5s/lalpha.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/5s/lbeta.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/5s/lcsp.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/data/earthquakes/5s/lgamma.txt` & `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lgamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/test-ext-earthquakes.py` & `chainsaddiction-0.2.3/tests/test-ext-earthquakes.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/test-utils.py` & `chainsaddiction-0.2.3/tests/test-utils.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.2/tests/utils.py` & `chainsaddiction-0.2.3/tests/utils.py`

 * *Files identical despite different names*

