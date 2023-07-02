# Comparing `tmp/ez-a-sync-0.1.9.tar.gz` & `tmp/ez-a-sync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.1.9.tar", last modified: Mon Jun 19 00:53:20 2023, max compression
+gzip compressed data, was "ez-a-sync-0.2.0.tar", last modified: Sun Jul  2 05:09:26 2023, max compression
```

## Comparing `ez-a-sync-0.1.9.tar` & `ez-a-sync-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.110393 ez-a-sync-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/_loggable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.578841 ez-a-sync-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/_loggable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.582841 ez-a-sync-0.2.0/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-02 05:09:26.000000 ez-a-sync-0.2.0/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:26.586841 ez-a-sync-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-02 05:09:08.000000 ez-a-sync-0.2.0/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.1.9/.github/workflows/codeql.yaml` & `ez-a-sync-0.2.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/.github/workflows/mypy.yaml` & `ez-a-sync-0.2.0/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/.github/workflows/pytest.yaml` & `ez-a-sync-0.2.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/.github/workflows/release.yaml` & `ez-a-sync-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/LICENSE.txt` & `ez-a-sync-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/README.md` & `ez-a-sync-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/__init__.py` & `ez-a-sync-0.2.0/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/_bound.py` & `ez-a-sync-0.2.0/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/_flags.py` & `ez-a-sync-0.2.0/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/_helpers.py` & `ez-a-sync-0.2.0/a_sync/_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from async_property.base import \
     AsyncPropertyDescriptor  # type: ignore [import]
 from async_property.cached import \
     AsyncCachedPropertyDescriptor  # type: ignore [import]
 
 from a_sync import _flags
 from a_sync._typing import *
+from a_sync.exceptions import ASyncRuntimeError, SyncModeInAsyncContextError
 
 
 def get_event_loop() -> asyncio.BaseEventLoop:
     try:
         loop = asyncio.get_event_loop()
     except RuntimeError as e: # Necessary for use with multi-threaded applications.
         if not str(e).startswith("There is no current event loop in thread"):
@@ -29,22 +30,20 @@
     if not callable(fn):
         raise TypeError(f'Input is not callable. Unable to decorate {fn}')
     fn_args = getfullargspec(fn)[0]
     for flag in _flags.VIABLE_FLAGS:
         if flag in fn_args:
             raise RuntimeError(f"{fn} must not have any arguments with the following names: {_flags.VIABLE_FLAGS}")
 
-running_event_loop_msg = f"You may want to make this an async function by setting one of the following kwargs: {_flags.VIABLE_FLAGS}"
-
 def _await(awaitable: Awaitable[T]) -> T:
     try:
         return get_event_loop().run_until_complete(awaitable)
     except RuntimeError as e:
         if str(e) == "This event loop is already running":
-            raise RuntimeError(str(e), running_event_loop_msg)
-        raise
+            raise SyncModeInAsyncContextError() from None
+        raise ASyncRuntimeError(e) from e
 
 def _asyncify(func: SyncFn[P, T], executor: Executor) -> CoroFn[P, T]:
     @functools.wraps(func)
     async def _asyncify_wrap(*args: P.args, **kwargs: P.kwargs) -> T:
         return await get_event_loop().run_in_executor(executor, func, *args, **kwargs)
     return _asyncify_wrap
```

### Comparing `ez-a-sync-0.1.9/a_sync/_kwargs.py` & `ez-a-sync-0.2.0/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/_typing.py` & `ez-a-sync-0.2.0/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/config.py` & `ez-a-sync-0.2.0/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/decorator.py` & `ez-a-sync-0.2.0/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/exceptions.py` & `ez-a-sync-0.2.0/a_sync/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,7 +44,18 @@
 
 class ImproperFunctionType(ValueError):
     pass
 
 class FunctionNotAsync(ImproperFunctionType):
     def __init__(self, fn):
         super().__init__(f"'coro_fn' must be a coroutine function defined with 'async def'. You passed {fn}.")
+
+class ASyncRuntimeError(RuntimeError):
+    def __init__(self, e: RuntimeError):
+        super().__init__(str(e))
+
+class SyncModeInAsyncContextError(ASyncRuntimeError):
+    def __init__(self):
+        from a_sync import _flags
+        err = f"The event loop is already running, which means you're trying to use an ASync function synchronously from within an async context.\n"
+        err += f"Check your traceback to determine which, then try calling asynchronously instead with one of the following kwargs:\n"
+        err += f"{_flags.VIABLE_FLAGS}"
```

### Comparing `ez-a-sync-0.1.9/a_sync/modified.py` & `ez-a-sync-0.2.0/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/__init__.py` & `ez-a-sync-0.2.0/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.2.0/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.2.0/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/limiter.py` & `ez-a-sync-0.2.0/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/manager.py` & `ez-a-sync-0.2.0/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.2.0/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.2.0/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/primitives/locks/event.py` & `ez-a-sync-0.2.0/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/a_sync/property.py` & `ez-a-sync-0.2.0/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.2.0/ez_a_sync.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/codeql.yaml
 .github/workflows/mypy.yaml
 .github/workflows/pytest.yaml
 .github/workflows/release.yaml
+a_sync/ENVIRONMENT_VARIABLES.py
 a_sync/__init__.py
 a_sync/_bound.py
 a_sync/_flags.py
 a_sync/_helpers.py
 a_sync/_kwargs.py
 a_sync/_meta.py
 a_sync/_typing.py
```

### Comparing `ez-a-sync-0.1.9/setup.py` & `ez-a-sync-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/fixtures.py` & `ez-a-sync-0.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/test_base.py` & `ez-a-sync-0.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/test_cache.py` & `ez-a-sync-0.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/test_decorator.py` & `ez-a-sync-0.2.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/test_meta.py` & `ez-a-sync-0.2.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.9/tests/test_semaphore.py` & `ez-a-sync-0.2.0/tests/test_semaphore.py`

 * *Files identical despite different names*

