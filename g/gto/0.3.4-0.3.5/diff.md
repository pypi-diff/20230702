# Comparing `tmp/gto-0.3.4.tar.gz` & `tmp/gto-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gto-0.3.4.tar", last modified: Wed Jun 28 11:32:12 2023, max compression
+gzip compressed data, was "gto-0.3.5.tar", last modified: Sat Jul  1 23:26:07 2023, max compression
```

## Comparing `gto-0.3.4.tar` & `gto-0.3.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.307748 gto-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-28 11:31:48.000000 gto-0.3.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.295747 gto-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.295747 gto-0.3.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-28 11:31:48.000000 gto-0.3.4/.github/ISSUE_TEMPLATE/epic-or-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.299747 gto-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-28 11:31:48.000000 gto-0.3.4/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-28 11:31:48.000000 gto-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-28 11:31:48.000000 gto-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-06-28 11:31:48.000000 gto-0.3.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-28 11:31:48.000000 gto-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-28 11:32:12.307748 gto-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-28 11:31:48.000000 gto-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.303747 gto-0.3.4/gto/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 11:31:48.000000 gto-0.3.4/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 11:32:12.000000 gto-0.3.4/gto/_gto_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-28 11:31:48.000000 gto-0.3.4/gto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-06-28 11:31:48.000000 gto-0.3.4/gto/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-06-28 11:31:48.000000 gto-0.3.4/gto/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25318 2023-06-28 11:31:48.000000 gto-0.3.4/gto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-28 11:31:48.000000 gto-0.3.4/gto/commit_message_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-28 11:31:48.000000 gto-0.3.4/gto/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-28 11:31:48.000000 gto-0.3.4/gto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-28 11:31:48.000000 gto-0.3.4/gto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-28 11:31:48.000000 gto-0.3.4/gto/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-28 11:31:48.000000 gto-0.3.4/gto/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-28 11:31:48.000000 gto-0.3.4/gto/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-28 11:31:48.000000 gto-0.3.4/gto/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-28 11:31:48.000000 gto-0.3.4/gto/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-06-28 11:31:48.000000 gto-0.3.4/gto/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-28 11:31:48.000000 gto-0.3.4/gto/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-28 11:31:48.000000 gto-0.3.4/gto/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-28 11:31:48.000000 gto-0.3.4/gto/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.303747 gto-0.3.4/gto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 11:32:12.000000 gto-0.3.4/gto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-28 11:31:48.000000 gto-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 11:31:48.000000 gto-0.3.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-28 11:32:12.311748 gto-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-28 11:31:48.000000 gto-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.307748 gto-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:31:48.000000 gto-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-28 11:31:48.000000 gto-0.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:32:12.307748 gto-0.3.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-28 11:31:48.000000 gto-0.3.4/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-28 11:31:48.000000 gto-0.3.4/tests/resources/sample_remote_repo_expected_history_churn.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-28 11:31:48.000000 gto-0.3.4/tests/resources/sample_remote_repo_expected_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-28 11:31:48.000000 gto-0.3.4/tests/skip_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-28 11:31:48.000000 gto-0.3.4/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-28 11:31:48.000000 gto-0.3.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.867868 gto-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-01 23:25:52.000000 gto-0.3.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.855867 gto-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.859868 gto-0.3.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-01 23:25:52.000000 gto-0.3.5/.github/ISSUE_TEMPLATE/epic-or-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.859868 gto-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-01 23:25:52.000000 gto-0.3.5/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-01 23:25:52.000000 gto-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-01 23:25:52.000000 gto-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-07-01 23:25:52.000000 gto-0.3.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-01 23:25:52.000000 gto-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-01 23:26:07.867868 gto-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-01 23:25:52.000000 gto-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.859868 gto-0.3.5/gto/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 23:25:52.000000 gto-0.3.5/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 23:26:07.000000 gto-0.3.5/gto/_gto_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-01 23:25:52.000000 gto-0.3.5/gto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-07-01 23:25:52.000000 gto-0.3.5/gto/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-07-01 23:25:52.000000 gto-0.3.5/gto/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25318 2023-07-01 23:25:52.000000 gto-0.3.5/gto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-01 23:25:52.000000 gto-0.3.5/gto/commit_message_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-01 23:25:52.000000 gto-0.3.5/gto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-01 23:25:52.000000 gto-0.3.5/gto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-01 23:25:52.000000 gto-0.3.5/gto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-01 23:25:52.000000 gto-0.3.5/gto/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-01 23:25:52.000000 gto-0.3.5/gto/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-07-01 23:25:52.000000 gto-0.3.5/gto/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-01 23:25:52.000000 gto-0.3.5/gto/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-07-01 23:25:52.000000 gto-0.3.5/gto/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-07-01 23:25:52.000000 gto-0.3.5/gto/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-01 23:25:52.000000 gto-0.3.5/gto/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-01 23:25:52.000000 gto-0.3.5/gto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-01 23:25:52.000000 gto-0.3.5/gto/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.863868 gto-0.3.5/gto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 23:26:07.000000 gto-0.3.5/gto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 23:25:52.000000 gto-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 23:25:52.000000 gto-0.3.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-01 23:26:07.867868 gto-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-01 23:25:52.000000 gto-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.863868 gto-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 23:25:52.000000 gto-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-01 23:25:52.000000 gto-0.3.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:26:07.867868 gto-0.3.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-01 23:25:52.000000 gto-0.3.5/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-01 23:25:52.000000 gto-0.3.5/tests/resources/sample_remote_repo_expected_history_churn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-01 23:25:52.000000 gto-0.3.5/tests/resources/sample_remote_repo_expected_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-01 23:25:52.000000 gto-0.3.5/tests/skip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-01 23:25:52.000000 gto-0.3.5/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-01 23:25:52.000000 gto-0.3.5/tests/utils.py
```

### Comparing `gto-0.3.4/.github/ISSUE_TEMPLATE/epic-or-story.md` & `gto-0.3.5/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/.github/workflows/check-test-release.yml` & `gto-0.3.5/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/.gitignore` & `gto-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/.pre-commit-config.yaml` & `gto-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/.pylintrc` & `gto-0.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/LICENSE` & `gto-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/PKG-INFO` & `gto-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.4
+Version: 0.3.5
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.4/README.md` & `gto-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/api.py` & `gto-0.3.5/gto/api.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/base.py` & `gto-0.3.5/gto/base.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/cli.py` & `gto-0.3.5/gto/cli.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/config.py` & `gto-0.3.5/gto/config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/constants.py` & `gto-0.3.5/gto/constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/exceptions.py` & `gto-0.3.5/gto/exceptions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/ext.py` & `gto-0.3.5/gto/ext.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/git_utils.py` & `gto-0.3.5/gto/git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/index.py` & `gto-0.3.5/gto/index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/log.py` & `gto-0.3.5/gto/log.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/registry.py` & `gto-0.3.5/gto/registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/tag.py` & `gto-0.3.5/gto/tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/ui.py` & `gto-0.3.5/gto/ui.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/utils.py` & `gto-0.3.5/gto/utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto/versions.py` & `gto-0.3.5/gto/versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/gto.egg-info/PKG-INFO` & `gto-0.3.5/gto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.4
+Version: 0.3.5
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.4/gto.egg-info/SOURCES.txt` & `gto-0.3.5/gto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/setup.cfg` & `gto-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/setup.py` & `gto-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 install_requires = [
     "gitpython",
     "typer>=0.4.1",
     "rich",
-    "pydantic",
+    "pydantic>=1.9.0,<2",
     "ruamel.yaml",
     "semver>=3.0.0",
     "entrypoints",
     "tabulate>=0.8.10",
     "funcy",
 ]
```

### Comparing `gto-0.3.4/tests/conftest.py` & `gto-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/resources/__init__.py` & `gto-0.3.5/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/resources/sample_remote_repo_expected_history_churn.json` & `gto-0.3.5/tests/resources/sample_remote_repo_expected_history_churn.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/resources/sample_remote_repo_expected_registry.json` & `gto-0.3.5/tests/resources/sample_remote_repo_expected_registry.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/skip_presets.py` & `gto-0.3.5/tests/skip_presets.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_api.py` & `gto-0.3.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_cli.py` & `gto-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_config.py` & `gto-0.3.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_constants.py` & `gto-0.3.5/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_git_utils.py` & `gto-0.3.5/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_index.py` & `gto-0.3.5/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_registry.py` & `gto-0.3.5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_showcase.py` & `gto-0.3.5/tests/test_showcase.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_tag.py` & `gto-0.3.5/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/test_versions.py` & `gto-0.3.5/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.4/tests/utils.py` & `gto-0.3.5/tests/utils.py`

 * *Files identical despite different names*

