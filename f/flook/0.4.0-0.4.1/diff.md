# Comparing `tmp/flook-0.4.0.tar.gz` & `tmp/flook-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.4.0.tar", last modified: Sat Jul  1 21:05:32 2023, max compression
+gzip compressed data, was "flook-0.4.1.tar", last modified: Sat Jul  1 21:58:54 2023, max compression
```

## Comparing `flook-0.4.0.tar` & `flook-0.4.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-01 21:05:10.000000 flook-0.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 21:05:10.000000 flook-0.4.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-01 21:05:10.000000 flook-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-01 21:05:10.000000 flook-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-01 21:05:10.000000 flook-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-01 21:05:10.000000 flook-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-01 21:05:10.000000 flook-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 21:05:10.000000 flook-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-01 21:05:10.000000 flook-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-01 21:05:10.000000 flook-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 21:05:10.000000 flook-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 21:05:10.000000 flook-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-01 21:05:10.000000 flook-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:05:32.233853 flook-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-01 21:05:10.000000 flook-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 21:05:10.000000 flook-0.4.0/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-01 21:05:10.000000 flook-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:05:10.000000 flook-0.4.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-01 21:05:32.237853 flook-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-01 21:05:10.000000 flook-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:05:31.000000 flook-0.4.0/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:10.000000 flook-0.4.0/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 21:05:10.000000 flook-0.4.0/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-01 21:05:10.000000 flook-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.688341 flook-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-01 21:58:30.000000 flook-0.4.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 21:58:30.000000 flook-0.4.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-01 21:58:30.000000 flook-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-01 21:58:30.000000 flook-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-01 21:58:30.000000 flook-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-01 21:58:30.000000 flook-0.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-01 21:58:30.000000 flook-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 21:58:30.000000 flook-0.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-01 21:58:30.000000 flook-0.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-01 21:58:30.000000 flook-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 21:58:30.000000 flook-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 21:58:30.000000 flook-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-01 21:58:30.000000 flook-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:58:54.696340 flook-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-01 21:58:30.000000 flook-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 21:58:30.000000 flook-0.4.1/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-01 21:58:30.000000 flook-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.684341 flook-0.4.1/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 21:58:30.000000 flook-0.4.1/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 21:58:30.000000 flook-0.4.1/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-01 21:58:30.000000 flook-0.4.1/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.692340 flook-0.4.1/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-01 21:58:30.000000 flook-0.4.1/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:58:30.000000 flook-0.4.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-01 21:58:54.700340 flook-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-01 21:58:30.000000 flook-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.684341 flook-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-01 21:58:30.000000 flook-0.4.1/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 21:58:54.000000 flook-0.4.1/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:58:30.000000 flook-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:54.696340 flook-0.4.1/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:58:30.000000 flook-0.4.1/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 21:58:30.000000 flook-0.4.1/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-01 21:58:30.000000 flook-0.4.1/tox.ini
```

### Comparing `flook-0.4.0/.github/workflows/release.yml` & `flook-0.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/.gitignore` & `flook-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/CHANGELOG.rst` & `flook-0.4.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/CODE_OF_CONDUCT.md` & `flook-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/CONTRIBUTING.rst` & `flook-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/LICENSE.txt` & `flook-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/Makefile` & `flook-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/PKG-INFO` & `flook-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.4.0/README.rst` & `flook-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/recipe/motd/recipe.yml` & `flook-0.4.1/recipe/motd/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/recipe/nginx/recipe.yml` & `flook-0.4.1/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/recipe/ping/recipe.yml` & `flook-0.4.1/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/setup.cfg` & `flook-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/setup.py` & `flook-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/__init__.py` & `flook-0.4.1/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/cli.py` & `flook-0.4.1/src/flook/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import uuid
 import click
 import logging, json, sys
+
 from flook import __version__
-from flook.command.configs import Configs
+from flook.model.host import Host
 from flook.command.hosts import Hosts
+from flook.command.configs import Configs
 from flook.command.recipes import Recipes
-from flook.model.host import Host
 
 
 @click.group(help="🐺 A Lightweight and Flexible Ansible Command Line Tool")
 @click.version_option(version=__version__, help="Show the current version")
 def main():
     pass
```

### Comparing `flook-0.4.0/src/flook/command/__init__.py` & `flook-0.4.1/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/command/configs.py` & `flook-0.4.1/src/flook/command/configs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import yaml
 import click
 
-from flook.module.database import Database
 from flook.module.logger import Logger
 from flook.module.output import Output
+from flook.module.database import Database
 from flook.module.file_system import FileSystem
 
 
 class Configs:
     """Configs Class"""
 
     FILE = ".flook.yml"
```

### Comparing `flook-0.4.0/src/flook/command/hosts.py` & `flook-0.4.1/src/flook/command/hosts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # SOFTWARE.
 
 import click
 import subprocess
 
 from flook.model.host import Host
 from flook.module.logger import Logger
-from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
+from flook.module.database import Database
 from flook.module.file_system import FileSystem
 
 
 class Hosts:
     """Hosts Class"""
 
     def __init__(self):
```

### Comparing `flook-0.4.0/src/flook/command/recipes.py` & `flook-0.4.1/src/flook/command/recipes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import uuid
-import click
 import yaml
+import click
 
 from flook.model.recipe import Recipe
 from flook.module.logger import Logger
-from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
-from flook.module.file_system import FileSystem
+from flook.module.database import Database
 from flook.module.playbook import Playbook
+from flook.module.file_system import FileSystem
 
 
 class Recipes:
     """Recipes Class"""
 
     def __init__(self):
         self.output = Output()
```

### Comparing `flook-0.4.0/src/flook/exception/__init__.py` & `flook-0.4.1/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/model/__init__.py` & `flook-0.4.1/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/model/host.py` & `flook-0.4.1/src/flook/model/host.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/model/recipe.py` & `flook-0.4.1/src/flook/model/recipe.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/model/task.py` & `flook-0.4.1/src/flook/model/task.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/__init__.py` & `flook-0.4.1/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/config.py` & `flook-0.4.1/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/database.py` & `flook-0.4.1/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/file_system.py` & `flook-0.4.1/src/flook/module/file_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import shutil
+
 from os.path import exists as file_exists
 
 
 class FileSystem:
     """FileSystem Class"""
 
     def read_file(self, file_path):
```

### Comparing `flook-0.4.0/src/flook/module/logger.py` & `flook-0.4.1/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/output.py` & `flook-0.4.1/src/flook/module/output.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook/module/playbook.py` & `flook-0.4.1/src/flook/module/playbook.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/src/flook.egg-info/PKG-INFO` & `flook-0.4.1/src/flook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.4.0/src/flook.egg-info/SOURCES.txt` & `flook-0.4.1/src/flook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/tests/__init__.py` & `flook-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/tests/module/test_logger.py` & `flook-0.4.1/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.4.0/tox.ini` & `flook-0.4.1/tox.ini`

 * *Files identical despite different names*

