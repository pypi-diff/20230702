# Comparing `tmp/ez-a-sync-0.3.0.tar.gz` & `tmp/ez-a-sync-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.3.0.tar", last modified: Sun Jul  2 06:45:57 2023, max compression
+gzip compressed data, was "ez-a-sync-0.3.1.tar", last modified: Sun Jul  2 06:56:17 2023, max compression
```

## Comparing `ez-a-sync-0.3.0.tar` & `ez-a-sync-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.119997 ez-a-sync-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.123997 ez-a-sync-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.127997 ez-a-sync-0.3.1/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.131997 ez-a-sync-0.3.1/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 06:56:17.000000 ez-a-sync-0.3.1/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:17.135997 ez-a-sync-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 06:56:02.000000 ez-a-sync-0.3.1/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.3.0/.github/workflows/codeql.yaml` & `ez-a-sync-0.3.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/.github/workflows/mypy.yaml` & `ez-a-sync-0.3.1/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/.github/workflows/pytest.yaml` & `ez-a-sync-0.3.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/.github/workflows/release.yaml` & `ez-a-sync-0.3.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/LICENSE.txt` & `ez-a-sync-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/README.md` & `ez-a-sync-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/__init__.py` & `ez-a-sync-0.3.1/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_bound.py` & `ez-a-sync-0.3.1/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_flags.py` & `ez-a-sync-0.3.1/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_helpers.py` & `ez-a-sync-0.3.1/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_kwargs.py` & `ez-a-sync-0.3.1/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_meta.py` & `ez-a-sync-0.3.1/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/_typing.py` & `ez-a-sync-0.3.1/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/abstract.py` & `ez-a-sync-0.3.1/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/base.py` & `ez-a-sync-0.3.1/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/config.py` & `ez-a-sync-0.3.1/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/decorator.py` & `ez-a-sync-0.3.1/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/exceptions.py` & `ez-a-sync-0.3.1/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modified.py` & `ez-a-sync-0.3.1/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/__init__.py` & `ez-a-sync-0.3.1/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.3.1/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.3.1/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/limiter.py` & `ez-a-sync-0.3.1/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/manager.py` & `ez-a-sync-0.3.1/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.3.1/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/primitives/executor.py` & `ez-a-sync-0.3.1/a_sync/primitives/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# NOTE: Will be deprecated soon in lieu of dank_mids.helpers.executor
 
 import asyncio
+import concurrent.futures as cf
 import queue
 import threading
 import weakref
-import  concurrent.futures as cf
 from concurrent.futures import _base, thread
 from functools import cached_property
-from typing import Any, Awaitable, Callable, TypeVar
+from typing import Callable, TypeVar
 
 from typing_extensions import ParamSpec
 
 TEN_MINUTES = 60 * 10
 
 T = TypeVar('T')
 P = ParamSpec('P')
```

### Comparing `ez-a-sync-0.3.0/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.3.1/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/primitives/locks/event.py` & `ez-a-sync-0.3.1/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/a_sync/property.py` & `ez-a-sync-0.3.1/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.3.1/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/setup.py` & `ez-a-sync-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/fixtures.py` & `ez-a-sync-0.3.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/test_base.py` & `ez-a-sync-0.3.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/test_cache.py` & `ez-a-sync-0.3.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/test_decorator.py` & `ez-a-sync-0.3.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/test_meta.py` & `ez-a-sync-0.3.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.3.0/tests/test_semaphore.py` & `ez-a-sync-0.3.1/tests/test_semaphore.py`

 * *Files identical despite different names*

