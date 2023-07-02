# Comparing `tmp/ez-a-sync-0.3.1.tar.gz` & `tmp/ez-a-sync-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.3.1.tar", last modified: Sun Jul  2 06:56:17 2023, max compression
+gzip compressed data, was "ez-a-sync-0.4.0.tar", last modified: Sun Jul  2 19:03:24 2023, max compression
```

## Comparing `ez-a-sync-0.3.1.tar` & `ez-a-sync-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.119997 ez-a-sync-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.123997 ez-a-sync-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.834194 ez-a-sync-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.834194 ez-a-sync-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 19:03:24.000000 ez-a-sync-0.4.0/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-07-02 19:03:24.000000 ez-a-sync-0.4.0/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 19:03:24.000000 ez-a-sync-0.4.0/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 19:03:24.000000 ez-a-sync-0.4.0/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 19:03:24.000000 ez-a-sync-0.4.0/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:24.838194 ez-a-sync-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 19:03:12.000000 ez-a-sync-0.4.0/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.3.1/.github/workflows/codeql.yaml` & `ez-a-sync-0.4.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/.github/workflows/mypy.yaml` & `ez-a-sync-0.4.0/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/.github/workflows/pytest.yaml` & `ez-a-sync-0.4.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/.github/workflows/release.yaml` & `ez-a-sync-0.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/LICENSE.txt` & `ez-a-sync-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/README.md` & `ez-a-sync-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/_bound.py` & `ez-a-sync-0.4.0/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/_flags.py` & `ez-a-sync-0.4.0/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/_helpers.py` & `ez-a-sync-0.4.0/a_sync/_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from async_property.base import \
     AsyncPropertyDescriptor  # type: ignore [import]
 from async_property.cached import \
     AsyncCachedPropertyDescriptor  # type: ignore [import]
 
 from a_sync import _flags
 from a_sync._typing import *
-from a_sync.exceptions import ASyncRuntimeError, KwargsUnsupportedError, SyncModeInAsyncContextError
+from a_sync.exceptions import (ASyncRuntimeError, KwargsUnsupportedError,
+                               SyncModeInAsyncContextError)
 
 
 def get_event_loop() -> asyncio.AbstractEventLoop:
     try:
         loop = asyncio.get_event_loop()
     except RuntimeError as e: # Necessary for use with multi-threaded applications.
         if not str(e).startswith("There is no current event loop in thread"):
```

### Comparing `ez-a-sync-0.3.1/a_sync/_kwargs.py` & `ez-a-sync-0.4.0/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/_meta.py` & `ez-a-sync-0.4.0/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/_typing.py` & `ez-a-sync-0.4.0/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/abstract.py` & `ez-a-sync-0.4.0/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/base.py` & `ez-a-sync-0.4.0/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/config.py` & `ez-a-sync-0.4.0/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/decorator.py` & `ez-a-sync-0.4.0/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/exceptions.py` & `ez-a-sync-0.4.0/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modified.py` & `ez-a-sync-0.4.0/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/__init__.py` & `ez-a-sync-0.4.0/a_sync/modifiers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from aiolimiter import AsyncLimiter
 
 from a_sync._typing import *
+from a_sync import primitives
 from a_sync.modifiers.manager import valid_modifiers
-from a_sync.modifiers.semaphores import ThreadsafeSemaphore
 
 
 def get_modifiers_from(thing: Union[dict, type, object]) -> ModifierKwargs:
     if isinstance(thing, dict):
         apply_class_defined_modifiers(thing)
         return ModifierKwargs({modifier: thing[modifier] for modifier in valid_modifiers if modifier in thing})  # type: ignore [misc]
     return ModifierKwargs({modifier: getattr(thing, modifier) for modifier in valid_modifiers if hasattr(thing, modifier)})  # type: ignore [misc]
 
 def apply_class_defined_modifiers(attrs_from_metaclass: dict):
     if 'semaphore' in attrs_from_metaclass and isinstance(val := attrs_from_metaclass['semaphore'], int):
-        attrs_from_metaclass['semaphore'] = ThreadsafeSemaphore(val)
+        attrs_from_metaclass['semaphore'] = primitives.ThreadsafeSemaphore(val)
     if "runs_per_minute" in attrs_from_metaclass and isinstance(val := attrs_from_metaclass['runs_per_minute'], int):
         attrs_from_metaclass['runs_per_minute'] = AsyncLimiter(val)
```

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.4.0/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.4.0/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/limiter.py` & `ez-a-sync-0.4.0/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/manager.py` & `ez-a-sync-0.4.0/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.4.0/a_sync/modifiers/semaphores.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,17 @@
 # type: ignore [valid-type, misc]
 import asyncio
 import functools
-from collections import defaultdict
-from threading import Thread, current_thread
 
-from a_sync import exceptions
+from a_sync import exceptions, primitives
 from a_sync._typing import *
 
+# We keep this here for now so we don't break downstream deps. Eventually will be removed.
+from a_sync.primitives import ThreadsafeSemaphore, DummySemaphore
 
-class ThreadsafeSemaphore(asyncio.Semaphore):
-    """
-    While its a bit weird to run multiple event loops, sometimes either you or a lib you're using must do so. 
-    When in use in threaded applications, this semaphore will not work as intended but at least your program will function.
-    You may need to reduce the semaphore value for multi-threaded applications.
-    
-    # TL;DR it's a janky fix for an edge case problem and will otherwise function as a normal asyncio.Semaphore.
-    """
-
-    def __init__(self, value: Optional[int]) -> None:
-        assert isinstance(value, int), f"{value} should be an integer."
-        self._value = value
-        self.semaphores: DefaultDict[Thread, asyncio.Semaphore] = defaultdict(lambda: asyncio.Semaphore(value))  # type: ignore [arg-type]
-        self.dummy = DummySemaphore()
-    
-    def __repr__(self) -> str:
-        return f"<ThreadsafeSemaphore value={self._value}>"
-    
-    @property
-    def use_dummy(self) -> bool:
-        return self._value is None
-    
-    @property
-    def semaphore(self) -> asyncio.Semaphore:
-        if self.use_dummy:
-            return self.dummy
-        tid = current_thread()
-        if tid not in self.semaphores:
-            self.semaphores[tid] = asyncio.Semaphore(self._value)
-        return self.semaphores[tid]
-    
-    async def __aenter__(self):
-        await self.semaphore.acquire()
-    
-    async def __aexit__(self, *args):
-        self.semaphore.release()
-
-
-class DummySemaphore(asyncio.Semaphore):
-    def __init__(*args, **kwargs):
-        ...
-    def __repr__(self) -> str:
-        return "<DummySemaphore>"
-    async def __aenter__(self):
-        ...
-    async def __aexit__(self, *args):
-        ...
-
-
-Semaphore = Union[
-    asyncio.Semaphore,
-    asyncio.BoundedSemaphore,
-    ThreadsafeSemaphore,
-    DummySemaphore,
-]
 
 @overload
 async def apply_semaphore(  # type: ignore [misc]
     coro_fn: Literal[None],
     semaphore: SemaphoreSpec,
 ) -> AsyncDecorator[P, T]:...
 
@@ -94,22 +39,30 @@
         coro_fn = None
         
     elif not asyncio.iscoroutinefunction(coro_fn):
         raise exceptions.FunctionNotAsync(coro_fn)
         
     # Create the semaphore if necessary
     if isinstance(semaphore, int):
-        semaphore = ThreadsafeSemaphore(semaphore)
+        semaphore = primitives.ThreadsafeSemaphore(semaphore)
     elif not isinstance(semaphore, asyncio.Semaphore):
         raise TypeError(f"'semaphore' must either be an integer or a Semaphore object.")
-        
+    
     # Create and return the decorator
-    def semaphore_decorator(coro_fn: CoroFn[P, T]) -> CoroFn[P, T]:
-        @functools.wraps(coro_fn)
-        async def semaphore_wrap(*args, **kwargs) -> T:
-            async with semaphore:  # type: ignore [union-attr]
-                return await coro_fn(*args, **kwargs)
-        return semaphore_wrap
+    if isinstance(semaphore, primitives.Semaphore):
+        # NOTE: Our `Semaphore` primitive can be used as a decorator.
+        #       While you can use it the `async with` way like any other semaphore and we could make this code section cleaner,
+        #       applying it as a decorator adds some useful info to its debug logs so we do that here if we can.
+        semaphore_decorator = semaphore
+    
+    else:
+        def semaphore_decorator(coro_fn: CoroFn[P, T]) -> CoroFn[P, T]:
+            @functools.wraps(coro_fn)
+            async def semaphore_wrap(*args, **kwargs) -> T:
+                async with semaphore:  # type: ignore [union-attr]
+                    return await coro_fn(*args, **kwargs)
+            return semaphore_wrap
+        
     return semaphore_decorator if coro_fn is None else semaphore_decorator(coro_fn)
 
 
-dummy_semaphore = DummySemaphore()
+dummy_semaphore = primitives.DummySemaphore()
```

### Comparing `ez-a-sync-0.3.1/a_sync/primitives/executor.py` & `ez-a-sync-0.4.0/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.4.0/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/primitives/locks/event.py` & `ez-a-sync-0.4.0/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/a_sync/property.py` & `ez-a-sync-0.4.0/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.4.0/ez_a_sync.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 a_sync/modifiers/cache/memory.py
 a_sync/primitives/__init__.py
 a_sync/primitives/_loggable.py
 a_sync/primitives/executor.py
 a_sync/primitives/locks/__init__.py
 a_sync/primitives/locks/counter.py
 a_sync/primitives/locks/event.py
+a_sync/primitives/locks/semaphore.py
 ez_a_sync.egg-info/PKG-INFO
 ez_a_sync.egg-info/SOURCES.txt
 ez_a_sync.egg-info/dependency_links.txt
 ez_a_sync.egg-info/requires.txt
 ez_a_sync.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
```

### Comparing `ez-a-sync-0.3.1/setup.py` & `ez-a-sync-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/fixtures.py` & `ez-a-sync-0.4.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/test_base.py` & `ez-a-sync-0.4.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/test_cache.py` & `ez-a-sync-0.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/test_decorator.py` & `ez-a-sync-0.4.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/test_meta.py` & `ez-a-sync-0.4.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.1/tests/test_semaphore.py` & `ez-a-sync-0.4.0/tests/test_semaphore.py`

 * *Files identical despite different names*

