# Comparing `tmp/ez-a-sync-0.2.0.tar.gz` & `tmp/ez-a-sync-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.2.0.tar", last modified: Sun Jul  2 05:09:26 2023, max compression
+gzip compressed data, was "ez-a-sync-0.3.0.tar", last modified: Sun Jul  2 06:45:57 2023, max compression
```

## Comparing `ez-a-sync-0.2.0.tar` & `ez-a-sync-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.578841 ez-a-sync-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/_loggable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.232708 ez-a-sync-0.3.0/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 06:45:57.000000 ez-a-sync-0.3.0/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:57.236708 ez-a-sync-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 06:45:45.000000 ez-a-sync-0.3.0/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.2.0/.github/workflows/codeql.yaml` & `ez-a-sync-0.3.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/.github/workflows/mypy.yaml` & `ez-a-sync-0.3.0/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/.github/workflows/pytest.yaml` & `ez-a-sync-0.3.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/.github/workflows/release.yaml` & `ez-a-sync-0.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/LICENSE.txt` & `ez-a-sync-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/README.md` & `ez-a-sync-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/__init__.py` & `ez-a-sync-0.3.0/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/_bound.py` & `ez-a-sync-0.3.0/a_sync/_bound.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 import functools
 from inspect import isawaitable
 
 from a_sync import _helpers
 from a_sync._typing import *
 from a_sync.decorator import a_sync as unbound_a_sync
 from a_sync.modified import ASyncFunction
@@ -10,15 +10,15 @@
                              AsyncPropertyDescriptor)
 
 if TYPE_CHECKING:
     from a_sync.abstract import ASyncABC
 
 
 def _clean_default_from_modifiers(
-    coro_fn: AsyncBoundMethod[P, T],
+    coro_fn: AsyncBoundMethod[P, T],  # type: ignore [misc]
     modifiers: dict
 ):
     # NOTE: We set the default here manually because the default set by the user will be used later in the code to determine whether to await.
     force_await = None
     if not asyncio.iscoroutinefunction(coro_fn) and not isinstance(coro_fn, ASyncFunction):
         if 'default' not in modifiers or modifiers['default'] is not 'async':
             if 'default' in modifiers and modifiers['default'] == 'sync':
@@ -26,24 +26,24 @@
             modifiers['default'] = 'async'
     return modifiers, force_await
 
             
 def _wrap_bound_method(
     coro_fn: AsyncBoundMethod[P, T],
     **modifiers: Unpack[ModifierKwargs]
-) -> AsyncBoundMethod[P, T]:  # type: ignore [misc]
+) -> AsyncBoundMethod[P, T]:
     from a_sync.abstract import ASyncABC
     
     # First we unwrap the coro_fn and rewrap it so overriding flag kwargs are handled automagically.
     if isinstance(coro_fn, ASyncFunction):
         coro_fn = coro_fn._fn
     
     modifiers, _force_await = _clean_default_from_modifiers(coro_fn, modifiers)
     
-    wrapped_coro_fn: AsyncBoundMethod[P, T] = ASyncFunction(coro_fn, **modifiers)  # type: ignore [arg-type]
+    wrapped_coro_fn: AsyncBoundMethod[P, T] = ASyncFunction(coro_fn, **modifiers)  # type: ignore [arg-type, valid-type, misc]
 
     @functools.wraps(coro_fn)
     def bound_a_sync_wrap(self: ASyncABC, *args: P.args, **kwargs: P.kwargs) -> T:  # type: ignore [name-defined]
         if not isinstance(self, ASyncABC):
             raise RuntimeError(f"{self} must be an instance of a class that inherits from ASyncABC.")
         # This could either be a coroutine or a return value from an awaited coroutine,
         #   depending on if an overriding flag kwarg was passed into the function call.
```

### Comparing `ez-a-sync-0.2.0/a_sync/_flags.py` & `ez-a-sync-0.3.0/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/_helpers.py` & `ez-a-sync-0.3.0/a_sync/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
 import asyncio
 import functools
+from concurrent.futures import Executor
 from inspect import getfullargspec
 
 from async_property.base import \
     AsyncPropertyDescriptor  # type: ignore [import]
 from async_property.cached import \
     AsyncCachedPropertyDescriptor  # type: ignore [import]
 
 from a_sync import _flags
 from a_sync._typing import *
-from a_sync.exceptions import ASyncRuntimeError, SyncModeInAsyncContextError
+from a_sync.exceptions import ASyncRuntimeError, KwargsUnsupportedError, SyncModeInAsyncContextError
 
 
-def get_event_loop() -> asyncio.BaseEventLoop:
+def get_event_loop() -> asyncio.AbstractEventLoop:
     try:
         loop = asyncio.get_event_loop()
     except RuntimeError as e: # Necessary for use with multi-threaded applications.
         if not str(e).startswith("There is no current event loop in thread"):
             raise e
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
@@ -35,15 +36,17 @@
             raise RuntimeError(f"{fn} must not have any arguments with the following names: {_flags.VIABLE_FLAGS}")
 
 def _await(awaitable: Awaitable[T]) -> T:
     try:
         return get_event_loop().run_until_complete(awaitable)
     except RuntimeError as e:
         if str(e) == "This event loop is already running":
-            raise SyncModeInAsyncContextError() from None
+            raise SyncModeInAsyncContextError from None
         raise ASyncRuntimeError(e) from e
 
-def _asyncify(func: SyncFn[P, T], executor: Executor) -> CoroFn[P, T]:
+def _asyncify(func: SyncFn[P, T], executor: Executor) -> CoroFn[P, T]:  # type: ignore [misc]
     @functools.wraps(func)
     async def _asyncify_wrap(*args: P.args, **kwargs: P.kwargs) -> T:
-        return await get_event_loop().run_in_executor(executor, func, *args, **kwargs)
+        if kwargs: 
+            raise KwargsUnsupportedError
+        return await get_event_loop().run_in_executor(executor, func, *args)
     return _asyncify_wrap
```

### Comparing `ez-a-sync-0.2.0/a_sync/_kwargs.py` & `ez-a-sync-0.3.0/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/_meta.py` & `ez-a-sync-0.3.0/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/_typing.py` & `ez-a-sync-0.3.0/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/abstract.py` & `ez-a-sync-0.3.0/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/base.py` & `ez-a-sync-0.3.0/a_sync/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import inspect
 import logging
 from functools import cached_property
+from typing import Optional
 
 from a_sync import _flags, exceptions
 from a_sync.abstract import ASyncABC
 
 
 logger = logging.getLogger(__name__)
 
@@ -49,15 +50,15 @@
         flag = cls.__get_a_sync_flag_name_from_signature()
         flag_value = cls.__a_sync_flag_default_value_from_signature()
         sync = _flags.negate_if_necessary(flag, flag_value)  # type: ignore [arg-type]
         logger.debug(f"`{cls}.{flag}` indicates default mode is {'a' if sync is False else ''}synchronous")
         return sync
     
     @classmethod
-    def __get_a_sync_flag_name_from_signature(cls) -> str:
+    def __get_a_sync_flag_name_from_signature(cls) -> Optional[str]:
         logger.debug(f"Searching for flags defined on {cls}")
         if cls.__name__ == "ASyncGenericBase":
             logger.debug(f"There are no flags defined on the base class, this is expected. Skipping.")
             return None
         parameters = inspect.signature(cls.__init__).parameters
         logger.debug(f"parameters: {parameters}")
         present_flags = [flag for flag in _flags.VIABLE_FLAGS if flag in parameters]
```

### Comparing `ez-a-sync-0.2.0/a_sync/config.py` & `ez-a-sync-0.3.0/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/decorator.py` & `ez-a-sync-0.3.0/a_sync/decorator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 from a_sync import _flags, config
 from a_sync._typing import *
 from a_sync.modified import ASyncDecorator, ASyncFunction
 
 ########################
 # The a_sync decorator #
 ########################
@@ -17,22 +17,22 @@
 
 @overload
 def a_sync(
     **modifiers: Unpack[ModifierKwargs],
 ) -> AnyFn[P, T]:...
 
 @overload # async def, None default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: CoroFn[P, T],
     default: Literal[None] = None,
     **modifiers: Unpack[ModifierKwargs],
 ) -> CoroFn[P, T]:...
 
 @overload # sync def none default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: SyncFn[P, T],
     default: Literal[None] = None,
     **modifiers: Unpack[ModifierKwargs],
 ) -> SyncFn[P, T]:...
 
 # @a_sync(default='async')
 # def some_fn():
@@ -41,54 +41,54 @@
 # @a_sync(default='async')
 # async def some_fn():
 #     pass
 #
 # NOTE These should output a decorator that will be applied to 'some_fn'
 
 @overload 
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Literal[None],
     default: Literal['async'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> AllToAsyncDecorator[P, T]:...
 
 @overload # if you try to use default as the only arg
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Literal['async'],
     default: Literal[None],
     **modifiers: Unpack[ModifierKwargs],
 ) -> AllToAsyncDecorator[P, T]:...
 
 # a_sync(some_fn, default='async')
 
 @overload # async def, async default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: CoroFn[P, T],
     default: Literal['async'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> CoroFn[P, T]:...
 
 @overload # sync def async default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: SyncFn[P, T],
     default: Literal['async'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> CoroFn[P, T]:...
 
 # a_sync(some_fn, default='sync')
 
 @overload # async def, sync default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: CoroFn[P, T],
     default: Literal['sync'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> SyncFn[P, T]:...
 
 @overload # sync def sync default
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: SyncFn[P, T],
     default: Literal['sync'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> SyncFn[P, T]:...
 
 # @a_sync(default='sync')
 # def some_fn():
@@ -97,36 +97,36 @@
 # @a_sync(default='sync')
 # async def some_fn():
 #     pass
 #
 # NOTE These should output a decorator that will be applied to 'some_fn'
 
 @overload 
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Literal[None],
     default: Literal['sync'],
     **modifiers: Unpack[ModifierKwargs],
 ) -> AllToSyncDecorator[P, T]:...
 
 @overload # if you try to use default as the only arg
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Literal['sync'],
     default: Literal[None] = None,
     **modifiers: Unpack[ModifierKwargs],
 ) -> AllToSyncDecorator[P, T]:...
 
 @overload # if you try to use default as the only arg
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Literal['sync'],
     default: Literal[None],
     **modifiers: Unpack[ModifierKwargs],
 ) -> AllToSyncDecorator[P, T]:...
     
 # catchall
-def a_sync(  # type: ignore [misc]
+def a_sync(  
     coro_fn: Optional[AnyFn[P, T]] = None,
     default: DefaultMode = config.DEFAULT_MODE,
     **modifiers: Unpack[ModifierKwargs],  # default values are set by passing these kwargs into a ModifierManager object.
 ) -> Union[ASyncDecorator[P, T], ASyncFunction[P, T]]:
     f"""
     A coroutine function decorated with this decorator can be called as a sync function by passing a boolean value for any of these kwargs: {_flags.VIABLE_FLAGS}
```

### Comparing `ez-a-sync-0.2.0/a_sync/exceptions.py` & `ez-a-sync-0.3.0/a_sync/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 class ImproperFunctionType(ValueError):
     pass
 
 class FunctionNotAsync(ImproperFunctionType):
     def __init__(self, fn):
         super().__init__(f"'coro_fn' must be a coroutine function defined with 'async def'. You passed {fn}.")
 
+class KwargsUnsupportedError(ValueError):
+    def __init__(self):
+        super().__init__("`run_in_executor` does not support keyword arguments, pass them as positional args instead if you're able")
+        
 class ASyncRuntimeError(RuntimeError):
     def __init__(self, e: RuntimeError):
         super().__init__(str(e))
 
 class SyncModeInAsyncContextError(ASyncRuntimeError):
     def __init__(self):
         from a_sync import _flags
```

### Comparing `ez-a-sync-0.2.0/a_sync/modified.py` & `ez-a-sync-0.3.0/a_sync/modified.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 import functools
 import sys
 
 from a_sync import _helpers, _kwargs, exceptions
 from a_sync._typing import *
 from a_sync.modifiers.manager import ModifierManager
```

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/__init__.py` & `ez-a-sync-0.3.0/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.3.0/a_sync/modifiers/cache/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 import asyncio
 
 from a_sync import exceptions
 from a_sync._typing import *
 from a_sync.modifiers.cache.memory import apply_async_memory_cache
```

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.3.0/a_sync/modifiers/cache/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 import asyncio
 
 from async_lru import alru_cache
 
 from a_sync import exceptions
 from a_sync._typing import *
```

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/limiter.py` & `ez-a-sync-0.3.0/a_sync/modifiers/limiter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type, misc]
 import asyncio
 
 from aiolimiter import AsyncLimiter
 
 from a_sync import aliases, exceptions
 from a_sync._typing import *
```

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/manager.py` & `ez-a-sync-0.3.0/a_sync/modifiers/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# type: ignore [valid-type]
 import functools
 
 from a_sync._typing import *
 from a_sync.config import user_set_default_modifiers, null_modifiers
 from a_sync.modifiers import cache, limiter, semaphores
 
 valid_modifiers = [key for key in ModifierKwargs.__annotations__ if not key.startswith('_') and not key.endswith('_')]
```

### Comparing `ez-a-sync-0.2.0/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.3.0/a_sync/modifiers/semaphores.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore [valid-type, misc]
 import asyncio
 import functools
 from collections import defaultdict
 from threading import Thread, current_thread
 
 from a_sync import exceptions
 from a_sync._typing import *
```

### Comparing `ez-a-sync-0.2.0/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.3.0/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/primitives/locks/event.py` & `ez-a-sync-0.3.0/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/a_sync/property.py` & `ez-a-sync-0.3.0/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.3.0/ez_a_sync.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 a_sync/modifiers/limiter.py
 a_sync/modifiers/manager.py
 a_sync/modifiers/semaphores.py
 a_sync/modifiers/cache/__init__.py
 a_sync/modifiers/cache/memory.py
 a_sync/primitives/__init__.py
 a_sync/primitives/_loggable.py
+a_sync/primitives/executor.py
 a_sync/primitives/locks/__init__.py
 a_sync/primitives/locks/counter.py
 a_sync/primitives/locks/event.py
 ez_a_sync.egg-info/PKG-INFO
 ez_a_sync.egg-info/SOURCES.txt
 ez_a_sync.egg-info/dependency_links.txt
 ez_a_sync.egg-info/requires.txt
```

### Comparing `ez-a-sync-0.2.0/setup.py` & `ez-a-sync-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/fixtures.py` & `ez-a-sync-0.3.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/test_base.py` & `ez-a-sync-0.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/test_cache.py` & `ez-a-sync-0.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/test_decorator.py` & `ez-a-sync-0.3.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/test_meta.py` & `ez-a-sync-0.3.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.2.0/tests/test_semaphore.py` & `ez-a-sync-0.3.0/tests/test_semaphore.py`

 * *Files identical despite different names*

