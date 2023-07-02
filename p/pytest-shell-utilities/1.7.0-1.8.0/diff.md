# Comparing `tmp/pytest-shell-utilities-1.7.0.tar.gz` & `tmp/pytest-shell-utilities-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Sep 23 08:10:11 2022, max compression
+gzip compressed data, last modified: Sun Jul  2 20:32:04 2023, max compression
```

## Comparing `pytest-shell-utilities-1.7.0.tar` & `pytest-shell-utilities-1.8.0.tar`

### file list

```diff
@@ -1,122 +1,113 @@
--rw-r--r--   0 root         (0) root         (0)     4958 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.codecov.yml
--rw-r--r--   0 root         (0) root         (0)     1222 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.github/
--rw-r--r--   0 root         (0) root         (0)      430 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.github/CODEOWNERS
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      638 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)    21772 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.github/workflows/testing.yml
--rw-r--r--   0 root         (0) root         (0)     1963 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     5660 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4622 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     3549 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)      579 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      690 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)    13551 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      735 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)     7353 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2479 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4900 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3452 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/changelog/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/css/
--rw-r--r--   0 root         (0) root         (0)      425 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/css/inline-include.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/img/
--rw-r--r--   0 root         (0) root         (0)    10359 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/img/SaltProject_Logomark_teal.png
--rw-r--r--   0 root         (0) root         (0)     9591 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/_static/img/SaltProject_altlogo_teal.png
--rw-r--r--   0 root         (0) root         (0)      164 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6197 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      222 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       85 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)     1060 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/ref/pytestshellutils.rst
--rw-r--r--   0 root         (0) root         (0)      883 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/ref/pytestshellutils.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    18907 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1326 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      348 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      105 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      144 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      202 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/lint.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     2868 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      186 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4900 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2994 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      457 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/
--rw-r--r--   0 root         (0) root         (0)     3070 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1969 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/customtypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1919 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/customtypes.py
--rw-r--r--   0 root         (0) root         (0)     2466 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      652 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/plugin.py
--rw-r--r--   0 root         (0) root         (0)    44596 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/
--rw-r--r--   0 root         (0) root         (0)     3955 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2227 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/ports.py
--rw-r--r--   0 root         (0) root         (0)    11977 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/processes.py
--rw-r--r--   0 root         (0) root         (0)      550 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/socket.py
--rw-r--r--   0 root         (0) root         (0)      542 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/time.py
--rw-r--r--   0 root         (0) root         (0)     2415 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      615 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/plugin.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/py.typed
--rw-r--r--   0 root         (0) root         (0)    48941 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/
--rw-r--r--   0 root         (0) root         (0)     4105 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2185 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/ports.py
--rw-r--r--   0 root         (0) root         (0)    15303 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/processes.py
--rw-r--r--   0 root         (0) root         (0)      512 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/socket.py
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/socket.pyi
--rw-r--r--   0 root         (0) root         (0)      504 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/time.py
--rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/time.pyi
--rw-r--r--   0 root         (0) root         (0)       43 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/src/pytestshellutils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2724 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25101 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/test_daemon.py
--rw-r--r--   0 root         (0) root         (0)     1389 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/test_fixture.py
--rw-r--r--   0 root         (0) root         (0)     6634 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/test_script_subprocess.py
--rw-r--r--   0 root         (0) root         (0)     6399 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/shell/test_subprocess.py
--rw-r--r--   0 root         (0) root         (0)     5213 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/functional/test_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/support/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/support/coverage/
--rw-r--r--   0 root         (0) root         (0)      161 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/support/coverage/sitecustomize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/customtypes/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/customtypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1187 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/customtypes/test_callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/processes/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/processes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5508 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/processes/test_processresult.py
--rw-r--r--   0 root         (0) root         (0)     1215 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/processes/test_processresult_matcher.py
--rw-r--r--   0 root         (0) root         (0)     1148 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/test_format_callback_to_string.py
--rw-r--r--   0 root         (0) root         (0)     2978 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/test_ports.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-09-23 08:10:11.000000 pytest-shell-utilities-1.7.0/tests/unit/utils/test_time.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.codecov.yml
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      430 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.github/CODEOWNERS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     9765 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.github/workflows/testing.yml
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     5500 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      735 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2479 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/changelog/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/css/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/css/inline-include.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/img/
+-rw-r--r--   0 root         (0) root         (0)    10359 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/img/SaltProject_Logomark_teal.png
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/_static/img/SaltProject_altlogo_teal.png
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6197 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/ref/pytestshellutils.rst
+-rw-r--r--   0 root         (0) root         (0)      883 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/ref/pytestshellutils.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    18931 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/lint.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/customtypes.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/plugin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/py.typed
+-rw-r--r--   0 root         (0) root         (0)    48340 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/
+-rw-r--r--   0 root         (0) root         (0)     4125 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/ports.py
+-rw-r--r--   0 root         (0) root         (0)    15403 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/processes.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/socket.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/socket.pyi
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/time.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/time.pyi
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/src/pytestshellutils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25101 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/test_daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/test_fixture.py
+-rw-r--r--   0 root         (0) root         (0)     6634 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/test_script_subprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6404 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/shell/test_subprocess.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/functional/test_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/support/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/support/coverage/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/support/coverage/sitecustomize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/customtypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/customtypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/customtypes/test_callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/processes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/processes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/processes/test_processresult.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/processes/test_processresult_matcher.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/test_format_callback_to_string.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/test_ports.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tests/unit/utils/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tools/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-02 20:32:04.000000 pytest-shell-utilities-1.8.0/tools/pre_commit.py
```

### Comparing `pytest-shell-utilities-1.7.0/.codecov.yml` & `pytest-shell-utilities-1.8.0/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/.coveragerc` & `pytest-shell-utilities-1.8.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/.github/workflows/release.yml` & `pytest-shell-utilities-1.8.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
   release:
     types: [created]
 
 jobs:
   Publish:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.9
     - name: Install Nox
       run: |
         python -m pip install nox
     - name: Build a binary wheel and a source tarball
       run: |
```

### Comparing `pytest-shell-utilities-1.7.0/.gitignore` & `pytest-shell-utilities-1.8.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -132,7 +132,10 @@
 .vim/
 
 # Ignore the setuptools_scm auto-generated version module
 src/pytestshellutils/version.py
 
 # Ignore CI generated artifacts
 artifacts/
+
+# neovim backup files
+*~
```

### Comparing `pytest-shell-utilities-1.7.0/.pre-commit-config.yaml` & `pytest-shell-utilities-1.8.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 minimum_pre_commit_version: 2.9.2
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-merge-conflict  # Check for files that contain merge conflict strings.
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
         exclude: ^src/pytestshellutils/downgraded/.*\.py$
       - id: mixed-line-ending     # Replaces or checks mixed line ending.
         args: [--fix=lf]
@@ -41,114 +41,127 @@
   # ----- Formatting ------------------------------------------------------------------------------------------------>
   - repo: https://github.com/saltstack/pre-commit-remove-import-headers
     rev: 1.1.0
     hooks:
       - id: remove-import-headers
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         name: Rewrite Code to be Py3.5+
         args: [
           --py3-plus
         ]
         files: ^((setup|noxfile|tests/.*|src/pytestshellutils/__init__)\.py)$
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         name: Rewrite Code to be Py3.7+
         args: [
           --py37-plus
         ]
         files: ^(src/.*\.py)$
-        exclude: ^src/pytestshellutils/(__init__|version|downgraded/.*)\.py$
+        exclude: ^src/pytestshellutils/(__init__|version)\.py$
 
   - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.8.2
+    rev: v3.9.0
     hooks:
       - id: reorder-python-imports
         args:
           - --py37-plus
           - --application-directories=.:src
-        exclude: ^src/pytestshellutils/(version.py|downgraded/.*)$
+        exclude: ^src/pytestshellutils/version\.py$
 
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 22.12.0
     hooks:
       - id: black
         args: [-l 100]
-        exclude: ^src/pytestshellutils/(version.py|downgraded/.*)$
+        exclude: ^src/pytestshellutils/version\.py$
 
   - repo: https://github.com/asottile/blacken-docs
     rev: v1.12.1
     hooks:
       - id: blacken-docs
         args: [--skip-errors]
         files: ^(.*\.rst|docs/.*\.rst|src/pytestshellutils/.*\.py)$
-        exclude: ^src/pytestshellutils/downgraded/.*$
         additional_dependencies: [black==22.8.0]
-  # <---- Formatting -------------------------------------------------------------------------------------------------
 
-  # ----- Remove Typing - Py3.5 Support  ---------------------------------------------------------------------------->
-  - repo: https://github.com/s0undt3ch/downgrade-source
-    rev: v3.0.0
-    hooks:
-      - id: downgrade-source
-        name: Downgrade source code into a separate package to support Py3.5
-        files: ^src/.*\.py$
-        exclude: ^src/pytestshellutils/((__init__|version)\.py|downgraded/.*\.py)$
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.4.1
+    hooks:
+      - id: mypy
+        alias: mypy-tools
+        name: Run mypy against tools
+        files: ^tools/.*\.py$
+        #args: [--strict]
+        additional_dependencies:
+          - attrs
+          - rich
+          - types-attrs
+          - types-requests
+
+  - repo: https://github.com/s0undt3ch/python-tools-scripts
+    rev: "0.15.0"
+    hooks:
+      - id: tools
+        alias: actionlint
+        name: Lint GitHub Actions Workflows
+        files: "^.github/workflows/"
+        types:
+          - yaml
         args:
-          - --target-version=3.5
-          - --pkg-path=src/pytestshellutils
-          - --skip-checker=nounusableimports
-          - --skip-checker=nostarimports
-  # <---- Remove Typing - Py3.5 Support  -----------------------------------------------------------------------------
+          - pre-commit
+          - actionlint
+        additional_dependencies:
+          - packaging==23.0
+  # <---- Formatting -------------------------------------------------------------------------------------------------
 
   # ----- Security -------------------------------------------------------------------------------------------------->
   - repo: https://github.com/PyCQA/bandit
     rev: "1.7.4"
     hooks:
       - id: bandit
         alias: bandit-salt
         name: Run bandit against the code base
         args: [--silent, -lll, --skip, B701]
         files: ^(?!tests/).*\.py$
-        exclude: ^src/pytestshellutils/(version|downgraded/shell)\.py$
+        exclude: ^src/pytestshellutils/version\.py$
   - repo: https://github.com/PyCQA/bandit
     rev: "1.7.4"
     hooks:
       - id: bandit
         alias: bandit-tests
         name: Run bandit against the test suite
         args: [--silent, -lll, --skip, B701]
         files: ^tests/.*
   # <---- Security ---------------------------------------------------------------------------------------------------
 
   # ----- Code Analysis --------------------------------------------------------------------------------------------->
   - repo: https://github.com/pycqa/flake8
-    rev: '5.0.4'
+    rev: '6.0.0'
     hooks:
       - id: flake8
-        exclude: ^(src/pytestshellutils/(downgraded/.*|version\.py)|\.pre-commit-hooks/.*\.py)$
+        exclude: ^(src/pytestshellutils/version\.py|\.pre-commit-hooks/.*\.py)$
         additional_dependencies:
         - flake8-mypy-fork
         - pydocstyle>=4.0.0
         - flake8-docstrings
         - flake8-rst
         - flake8-typing-imports
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v0.991
     hooks:
       - id: mypy
         files: ^((src|tests)/.*\.py)$
-        exclude: ^(src/pytestshellutils/(downgraded/.*|utils/(socket|time)\.py))$
+        exclude: ^(src/pytestshellutils/(utils/(socket|time)\.py))$
         args: [--strict]
         additional_dependencies:
           - attrs
           - types-attrs
           - types-setuptools
           - pydantic
           - pytest
```

### Comparing `pytest-shell-utilities-1.7.0/.pre-commit-hooks/check-changelog-entries.py` & `pytest-shell-utilities-1.8.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: disable=invalid-name,missing-module-docstring,missing-function-docstring
 import argparse
 import pathlib
 import re
 import sys
```

### Comparing `pytest-shell-utilities-1.7.0/.pre-commit-hooks/copyright-headers.py` & `pytest-shell-utilities-1.8.0/.pre-commit-hooks/copyright-headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: disable=invalid-name,missing-module-docstring,missing-function-docstring
 import argparse
 import pathlib
 import re
 import sys
```

### Comparing `pytest-shell-utilities-1.7.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `pytest-shell-utilities-1.8.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 # pylint: skip-file
 import pathlib
 
 REPO_ROOT = pathlib.Path(__name__).resolve().parent
 PYLINT_SPELLING_WORDS = REPO_ROOT / ".pylint-spelling-words"
```

### Comparing `pytest-shell-utilities-1.7.0/.pylint-spelling-words` & `pytest-shell-utilities-1.8.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/.pylintrc` & `pytest-shell-utilities-1.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/.readthedocs.yaml` & `pytest-shell-utilities-1.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/CHANGELOG.rst` & `pytest-shell-utilities-1.8.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,47 @@
 Backward incompatible (breaking) changes will only be introduced in major versions with advance notice in the
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
+shell-utilities 1.8.0 (2023-07-02)
+==================================
+
+Breaking Changes
+----------------
+
+- Drop support for python versions older than 3.7 (`#38 <https://github.com/saltstack/pytest-shell-utilities/issues/38>`_)
+
+
+Improvements
+------------
+
+- Support Python 3.11 (`#40 <https://github.com/saltstack/pytest-shell-utilities/issues/40>`_)
+
+
+Bug Fixes
+---------
+
+- Set minimal attrs version to 22.1.0 (`#28 <https://github.com/saltstack/pytest-shell-utilities/issues/28>`_)
+
+
+Trivial/Internal Changes
+------------------------
+
+- Update the GitHub actions versions and stop using `::set-output` (`#38 <https://github.com/saltstack/pytest-shell-utilities/issues/38>`_)
+- Several project internal changes
+
+  * Start running tests against Py3.11 and Pytest `7.3.x` and `7.4.x`
+  * Update copyright headers
+  * Upgrade to `coverage==7.2.7`
+  * Switch to `codecov/codecov-action` (`#39 <https://github.com/saltstack/pytest-shell-utilities/issues/39>`_)
+
+
 shell-utilities 1.7.0 (2022-09-23)
 ==================================
 
 Bug Fixes
 ---------
 
 - ``Subprocess.run()`` now accepts ``shell`` keyword argument like ``subprocess.Popen``. (`#32 <https://github.com/saltstack/pytest-shell-utilities/issues/32>`_)
```

### Comparing `pytest-shell-utilities-1.7.0/CODE_OF_CONDUCT.md` & `pytest-shell-utilities-1.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/CONTRIBUTING.md` & `pytest-shell-utilities-1.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/LICENSE` & `pytest-shell-utilities-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/PKG-INFO` & `pytest-shell-utilities-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-shell-utilities
-Version: 1.7.0
+Version: 1.8.0
 Summary: Pytest plugin to simplify running shell commands against the system
 Home-page: https://github.com/saltstack/pytest-shell-utilities
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-shell-utilities
 Project-URL: Tracker, https://github.com/saltstack/pytest-shell-utilities/issues
@@ -14,25 +14,24 @@
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5.2
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: tests
 Provides-Extra: changelog
 License-File: LICENSE
```

### Comparing `pytest-shell-utilities-1.7.0/README.rst` & `pytest-shell-utilities-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/Makefile` & `pytest-shell-utilities-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/_static/img/SaltProject_Logomark_teal.png` & `pytest-shell-utilities-1.8.0/docs/_static/img/SaltProject_Logomark_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/_static/img/SaltProject_altlogo_teal.png` & `pytest-shell-utilities-1.8.0/docs/_static/img/SaltProject_altlogo_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/conf.py` & `pytest-shell-utilities-1.8.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
```

### Comparing `pytest-shell-utilities-1.7.0/docs/index.rst` & `pytest-shell-utilities-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/make.bat` & `pytest-shell-utilities-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/ref/pytestshellutils.rst` & `pytest-shell-utilities-1.8.0/docs/ref/pytestshellutils.rst`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/docs/ref/pytestshellutils.utils.rst` & `pytest-shell-utilities-1.8.0/docs/ref/pytestshellutils.utils.rst`

 * *Files identical despite different names*

### Comparing `pytest-shell-utilities-1.7.0/noxfile.py` & `pytest-shell-utilities-1.8.0/noxfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: disable=import-error,protected-access,line-too-long
 import datetime
 import gzip
 import json
 import os
@@ -12,15 +12,15 @@
 import tarfile
 import tempfile
 
 import nox
 from nox.command import CommandFailed
 
 
-COVERAGE_VERSION_REQUIREMENT = "coverage==6.2"
+COVERAGE_VERSION_REQUIREMENT = "coverage==7.2.7"
 PYTEST_VERSION_REQUIREMENT = os.environ.get("PYTEST_VERSION_REQUIREMENT") or None
 IS_WINDOWS = sys.platform.lower().startswith("win")
 IS_DARWIN = sys.platform.lower().startswith("darwin")
 
 if IS_WINDOWS:
     COVERAGE_FAIL_UNDER_PERCENT = 87
 elif IS_DARWIN:
@@ -107,41 +107,41 @@
             #   https://github.com/theacodes/nox/pull/181
             session._runner.global_config.install_only = False
             return session.run(*command, **kwargs)
         finally:
             session._runner.global_config.install_only = old_install_only_value
 
 
-@nox.session(python=("3", "3.5", "3.6", "3.7", "3.8", "3.9"))
+@nox.session(python=("3", "3.7", "3.8", "3.9", "3.10", "3.11"))
 def tests(session):
     """
     Run tests.
     """
     env = {}
     install_arguments = ["--progress-bar=off"]
     if SKIP_REQUIREMENTS_INSTALL is False:
-        # Always have the wheel package installed
-        if python_version(session) < (3, 6):
-            install_arguments.append("--no-python-version-warning")
-            session.install(*install_arguments, "-U", "pip<21.0", silent=PIP_INSTALL_SILENT)
-            coverage_requirements = ["coverage==5.2"]
-        else:
-            env["COVERAGE_PLUGINS_LIST"] = "coverage_conditional_plugin"
-            coverage_requirements = [COVERAGE_VERSION_REQUIREMENT, "coverage-conditional-plugin"]
+        env["COVERAGE_PLUGINS_LIST"] = "coverage_conditional_plugin"
+        coverage_requirements = [COVERAGE_VERSION_REQUIREMENT, "coverage-conditional-plugin"]
         session.install(*install_arguments, "wheel", silent=PIP_INSTALL_SILENT)
         session.install(
             *install_arguments,
             *coverage_requirements,
             silent=PIP_INSTALL_SILENT,
         )
 
         pytest_version_requirement = PYTEST_VERSION_REQUIREMENT
         if pytest_version_requirement:
             if not pytest_version_requirement.startswith("pytest"):
-                pytest_version_requirement = "pytest{}".format(pytest_version_requirement)
+                if (
+                    not pytest_version_requirement.startswith(("==", "~="))
+                    and pytest_version_requirement.endswith(".0")
+                    and not pytest_version_requirement.startswith("~=")
+                ):
+                    pytest_version_requirement = f"~={pytest_version_requirement}"
+                pytest_version_requirement = f"pytest{pytest_version_requirement}"
             session.install(pytest_version_requirement, silent=PIP_INSTALL_SILENT)
         session.install(*install_arguments, "-e", ".[tests]", silent=PIP_INSTALL_SILENT)
 
         if EXTRA_REQUIREMENTS_INSTALL:
             session.log(
                 "Installing the following extra requirements because the EXTRA_REQUIREMENTS_INSTALL "
                 "environment variable was set: EXTRA_REQUIREMENTS_INSTALL='%s'",
@@ -195,15 +195,15 @@
     else:
         for arg in session.posargs:
             if arg.startswith("--color") and session._runner.global_config.forcecolor:
                 args.remove("--color=yes")
             args.append(arg)
 
     try:
-        session.run("coverage", "run", "-m", "pytest", *args, env=env)
+        session.run("python", "-bb", "-m", "coverage", "run", "-m", "pytest", *args, env=env)
     finally:
         # Always combine and generate the XML coverage report
         try:
             session.run("coverage", "combine")
         except CommandFailed:
             # Sometimes some of the coverage files are corrupt which would
             # trigger a CommandFailed exception
```

### Comparing `pytest-shell-utilities-1.7.0/pyproject.toml` & `pytest-shell-utilities-1.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -43,12 +43,7 @@
   name = "Improved Documentation"
   showcontent = true
 
   [[tool.towncrier.type]]
   directory = "trivial"
   name = "Trivial/Internal Changes"
   showcontent = true
-
-[tool.bandit]
-exclude = [
-  "src/pytestshellutils/downgraded/shell.py"
-]
```

### Comparing `pytest-shell-utilities-1.7.0/setup.cfg` & `pytest-shell-utilities-1.8.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 	Documentation=https://pytest-shell-utilities.readthedocs.io
 license = Apache Software License 2.0
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Typing :: Typed
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 platforms = unix, linux, osx, cygwin, win32
 
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
-python_requires = >= 3.5.2
+python_requires = >= 3.7
 setup_requires = 
 	setuptools>=50.3.2
 	setuptools_scm[toml]>=3.4
 	setuptools-declarative-requirements
 
 [options.packages.find]
 where = src
@@ -114,11 +113,14 @@
 
 [mypy-pytestshellutils.utils.socket]
 no_implicit_reexport = False
 
 [mypy-pytestshellutils.utils.time]
 no_implicit_reexport = False
 
+[mypy.tools]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytest_shell_utilities.egg-info/PKG-INFO` & `pytest-shell-utilities-1.8.0/src/pytest_shell_utilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-shell-utilities
-Version: 1.7.0
+Version: 1.8.0
 Summary: Pytest plugin to simplify running shell commands against the system
 Home-page: https://github.com/saltstack/pytest-shell-utilities
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-shell-utilities
 Project-URL: Tracker, https://github.com/saltstack/pytest-shell-utilities/issues
@@ -14,25 +14,24 @@
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5.2
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: tests
 Provides-Extra: changelog
 License-File: LICENSE
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/customtypes.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/customtypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Custom Types.
 """
 import copy
 import logging
 from typing import Any
@@ -24,15 +24,15 @@
 
 
 class EnvironDict(Dict[str, str]):
     """
     Environ dictionary type.
     """
 
-    def __str__(self) -> str:
+    def __str__(self) -> str:  # pragma: no cover
         """
         String representation of the class.
         """
         return f"EnvironDict({super().__str__()})"
 
 
 class GenericCallback(Protocol):
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/exceptions.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Pytest Shell Utilities related exceptions.
 """
-from __future__ import generator_stop
 from typing import Optional
+
 from pytestshellutils.utils.processes import ProcessResult
 
 
 class ShellUtilsException(Exception):
     """
     Base pytest shell utilities exception.
     """
@@ -29,29 +29,27 @@
             The exception message
 
     Keyword Arguments:
         process_result:
             The ``ProcessResult`` instance when the exception occurred
     """
 
-    def __init__(
-        self, message: str, process_result: Optional[ProcessResult] = None
-    ) -> None:
+    def __init__(self, message: str, process_result: Optional[ProcessResult] = None) -> None:
         super().__init__()
         self.message = message
         self.process_result = process_result
 
     def __str__(self) -> str:
         """
         Return a printable representation of the exception.
         """
         message = self.message
         if self.process_result:
-            if not message.endswith('\n'):
-                message += '\n'
+            if not message.endswith("\n"):
+                message += "\n"
             message += str(self.process_result)
         return message
 
 
 class FactoryFailure(ProcessFailed):
     """
     Exception raised when a sub-process fails on one of the factories.
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/plugin.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Pytest shell utilities plugin.
 """
-from __future__ import generator_stop
 import pytest
+
 from pytestshellutils.shell import Subprocess
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def shell() -> Subprocess:
     """
     Shell fixture.
 
     Example:
         .. code-block:: python
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/shell.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/shell.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Shelling class implementations.
 """
-from __future__ import generator_stop
 import atexit
 import contextlib
 import json
 import locale
 import logging
 import os
 import pathlib
@@ -21,17 +20,19 @@
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import TYPE_CHECKING
 from typing import Union
+
 import attr
 import psutil
 from pytestskipmarkers.utils import platform
+
 from pytestshellutils.customtypes import Callback
 from pytestshellutils.customtypes import EnvironDict
 from pytestshellutils.exceptions import CallbackException
 from pytestshellutils.exceptions import FactoryNotRunning
 from pytestshellutils.exceptions import FactoryNotStarted
 from pytestshellutils.exceptions import FactoryTimeout
 from pytestshellutils.exceptions import ShellUtilsException
@@ -42,14 +43,15 @@
 from pytestshellutils.utils.processes import ProcessResult
 from pytestshellutils.utils.processes import terminate_process
 from pytestshellutils.utils.processes import terminate_process_list
 
 if TYPE_CHECKING:
     from typing import Type
     from pytestsysstats.plugin import StatsProcesses
+
 log = logging.getLogger(__name__)
 
 
 @attr.s(slots=True, kw_only=True)
 class BaseFactory:
     """
     Base factory class.
@@ -57,16 +59,16 @@
     Keyword Arguments:
         cwd:
             The path to the desired working directory
         environ:
             A dictionary of ``key``, ``value`` pairs to add to the environment.
     """
 
-    cwd = attr.ib(converter=resolved_pathlib_path)
-    environ = attr.ib(repr=False)
+    cwd: pathlib.Path = attr.ib(converter=resolved_pathlib_path)
+    environ: EnvironDict = attr.ib(repr=False)
 
     @cwd.default
     def _default_cwd(self) -> pathlib.Path:
         """
         Return the default cwd to use.
         """
         return pathlib.Path.cwd()
@@ -86,21 +88,26 @@
 
     Arguments:
         factory:
             The factory instance, either :py:class:`~pytestshellutils.shell.Subprocess` or
             a sub-class of it.
     """
 
-    factory = attr.ib()
-    _terminal = attr.ib(repr=False, init=False, default=None)
-    _terminal_stdout = attr.ib(repr=False, init=False, default=None)
-    _terminal_stderr = attr.ib(repr=False, init=False, default=None)
-    _terminal_result = attr.ib(repr=False, init=False, default=None)
-    _terminal_timeout = attr.ib(repr=False, init=False, default=None)
-    _children = attr.ib(repr=False, init=False, factory=list)
+    factory: "Union[Factory, Subprocess, ScriptSubprocess]" = attr.ib()
+
+    _terminal: "Optional[subprocess.Popen[Any]]" = attr.ib(repr=False, init=False, default=None)
+    _terminal_stdout: "Optional[SpooledTemporaryFile[bytes]]" = attr.ib(
+        repr=False, init=False, default=None
+    )
+    _terminal_stderr: "Optional[SpooledTemporaryFile[bytes]]" = attr.ib(
+        repr=False, init=False, default=None
+    )
+    _terminal_result: Optional[ProcessResult] = attr.ib(repr=False, init=False, default=None)
+    _terminal_timeout: Union[int, float] = attr.ib(repr=False, init=False, default=None)
+    _children: List[psutil.Process] = attr.ib(repr=False, init=False, factory=list)
 
     def cmdline(self, *args: str, **kwargs: Any) -> List[str]:
         """
         Construct a list of arguments to use when starting the subprocess.
 
         Arguments:
             args:
@@ -113,15 +120,15 @@
 
     def init_terminal(
         self,
         cmdline: List[str],
         shell: bool = False,
         env: Optional[EnvironDict] = None,
         cwd: Optional[Union[str, pathlib.Path]] = None,
-    ) -> 'subprocess.Popen[Any]':
+    ) -> "subprocess.Popen[Any]":
         """
         Instantiate a terminal with the passed command line(``cmdline``) and return it.
 
         Additionally, it sets a reference to it in ``self._terminal`` and also collects
         an initial listing of child processes which will be used when terminating the
         terminal
 
@@ -142,40 +149,48 @@
             A :py:class:`~subprocess.Popen` instance.
         """
         environ = self.factory.environ.copy()
         if env is not None:
             environ.update(env)
         self._terminal_stdout = SpooledTemporaryFile(512000, buffering=0)
         self._terminal_stderr = SpooledTemporaryFile(512000, buffering=0)
-        close_fds = None
-        if platform.is_windows():
+        close_fds: bool
+        if platform.is_windows():  # pragma: is-windows
+            # Windows does not support closing FDs
             close_fds = False
-        elif platform.is_freebsd() and sys.version_info < (3, 9):
+        elif platform.is_freebsd() and sys.version_info < (3, 9):  # pragma: is-bsd-lt-py39
+            # Closing FDs in FreeBSD before Py3.9 can be slow
+            #   https://bugs.python.org/issue38061
             close_fds = False
         else:
             close_fds = True
         self._terminal = subprocess.Popen(
             cmdline,
             stdout=self._terminal_stdout,
             stderr=self._terminal_stderr,
-            shell=shell,
+            shell=shell,  # nosec B602
             cwd=str(cwd or self.factory.cwd),
             universal_newlines=True,
             close_fds=close_fds,
             env=environ,
             bufsize=0,
         )
+        # Reset the previous _terminal_result if set
         self._terminal_result = None
         try:
+            # Check if the process starts properly
             self._terminal.wait(timeout=0.05)
+            # If TimeoutExpired is not raised, it means the process failed to start
         except subprocess.TimeoutExpired:
+            # We're good
+            # Collect any child processes, though, this early there likely is none
             with contextlib.suppress(psutil.NoSuchProcess):
                 for child in psutil.Process(self._terminal.pid).children(
                     recursive=True
-                ):
+                ):  # pragma: no cover
                     if child not in self._children:
                         self._children.append(child)
             atexit.register(self.terminate)
         return self._terminal
 
     def is_running(self) -> bool:
         """
@@ -196,103 +211,113 @@
 
     def _terminate(self) -> ProcessResult:
         """
         This method actually terminates the started subprocess.
         """
         if self._terminal is None:
             if TYPE_CHECKING:
+                # Make mypy happy
                 assert self._terminal_result
             return self._terminal_result
         atexit.unregister(self.terminate)
-        log.info('Stopping %s', self.factory)
+        log.info("Stopping %s", self.factory)
+        # Collect any child processes information before terminating the process
         with contextlib.suppress(psutil.NoSuchProcess):
             for child in psutil.Process(self._terminal.pid).children(recursive=True):
                 if child not in self._children:
                     self._children.append(child)
+
         with self._terminal:
             try:
                 if self.factory.slow_stop:
                     self._terminal.terminate()
                 else:
                     self._terminal.kill()
                 try:
+                    # Allow the process to exit by itself in case slow_stop is True
                     self._terminal.wait(10)
-                except subprocess.TimeoutExpired:
+                except subprocess.TimeoutExpired:  # pragma: no cover
+                    # The process failed to stop, no worries, we'll make sure it exit along with it's
+                    # child processes bellow
                     pass
             except ProcessLookupError:
+                # The process is already gone
                 pass
+            # Lets log and kill any child processes left behind, including the main subprocess
+            # If it failed to properly stop
             terminate_process(
                 pid=self._terminal.pid,
                 kill_children=True,
                 children=self._children,
                 slow_stop=self.factory.slow_stop,
             )
+            # Wait for the process to terminate, to avoid zombies.
             self._terminal.wait()
+            # poll the terminal so the right returncode is set on the popen object
             self._terminal.poll()
+            # This call shouldn't really be necessary
             self._terminal.communicate()
+
             if TYPE_CHECKING:
+                # Make mypy happy
                 assert self._terminal_stdout
             self._terminal_stdout.flush()
             self._terminal_stdout.seek(0)
             _read_stdout = self._terminal_stdout.read()
-            try:
-                stdout = self._terminal._translate_newlines(
-                    _read_stdout, self.factory.system_encoding, sys.stdout.errors
-                )
-            except TypeError:
-                stdout = self._terminal._translate_newlines(
-                    _read_stdout, self.factory.system_encoding
-                )
+            stdout = self._terminal._translate_newlines(  # type: ignore[attr-defined]
+                _read_stdout,
+                self.factory.system_encoding,
+                sys.stdout.errors,
+            )
             self._terminal_stdout.close()
+
             if TYPE_CHECKING:
+                # Make mypy happy
                 assert self._terminal_stderr
             self._terminal_stderr.flush()
             self._terminal_stderr.seek(0)
             _read_stderr = self._terminal_stderr.read()
-            try:
-                stderr = self._terminal._translate_newlines(
-                    _read_stderr, self.factory.system_encoding, sys.stderr.errors
-                )
-            except TypeError:
-                stderr = self._terminal._translate_newlines(
-                    _read_stderr, self.factory.system_encoding
-                )
+            stderr = self._terminal._translate_newlines(  # type: ignore[attr-defined]
+                _read_stderr,
+                self.factory.system_encoding,
+                sys.stderr.errors,
+            )
             self._terminal_stderr.close()
         try:
             self._terminal_result = ProcessResult(
                 returncode=self._terminal.returncode,
                 stdout=stdout,
                 stderr=stderr,
                 cmdline=cast(List[str], self._terminal.args),
             )
-            log.info('%s %s', self.factory.__class__.__name__, self._terminal_result)
+            log.info("%s %s", self.factory.__class__.__name__, self._terminal_result)
             return self._terminal_result
         finally:
             self._terminal = None
             self._terminal_stdout = None
             self._terminal_stderr = None
             self._children = []
 
     @property
     def pid(self) -> Optional[int]:
         """
         The pid of the running process. None if not running.
         """
-        if not self._terminal:
+        if not self._terminal:  # pragma: no cover
             return None
         return self._terminal.pid
 
     def run(
         self,
         *args: str,
         shell: bool = False,
         env: Optional[EnvironDict] = None,
         cwd: Optional[Union[str, pathlib.Path]] = None,
-        **kwargs: Any
-    ) -> 'subprocess.Popen[Any]':
+        **kwargs: Any,
+    ) -> "subprocess.Popen[Any]":
         """
         Run the given command synchronously.
 
         Arguments:
             args:
                 The command to run.
 
@@ -306,20 +331,15 @@
             cwd:
                 A path for the CWD when running the process.
 
         Returns:
             A :py:class:`~subprocess.Popen` instance.
         """
         cmdline = self.cmdline(*args, **kwargs)
-        log.info(
-            '%s is running %r in CWD: %s ...',
-            self.factory,
-            cmdline,
-            cwd or self.factory.cwd,
-        )
+        log.info("%s is running %r in CWD: %s ...", self.factory, cmdline, cwd or self.factory.cwd)
         return self.init_terminal(cmdline, shell=shell, env=env, cwd=cwd)
 
 
 @attr.s(slots=True, kw_only=True)
 class Factory(BaseFactory):
     """
     Base shell factory class.
@@ -335,54 +355,78 @@
         timeout:
             The default maximum amount of seconds that a script should run.
             This value can be overridden when calling :py:meth:`~pytestshellutils.shell.Process.run` through
             the ``_timeout`` keyword argument, and, in that case, the timeout value applied would be that
             of ``_timeout`` instead of ``self.timeout``.
     """
 
-    slow_stop = attr.ib(default=True)
-    system_encoding = attr.ib(repr=False)
-    timeout = attr.ib()
-    impl = attr.ib(repr=False, init=False)
-    _cmdline = attr.ib(repr=False, init=False, default=None)
+    slow_stop: bool = attr.ib(default=True)
+    system_encoding: str = attr.ib(repr=False)
+    timeout: Union[int, float] = attr.ib()
+
+    impl: SubprocessImpl = attr.ib(repr=False, init=False)
+
+    # Internal attributes
+    _cmdline: List[Any] = attr.ib(repr=False, init=False, default=None)
 
     @system_encoding.default
     def _default_system_encoding(self) -> str:
         return self._get_default_system_encoding()
 
     @timeout.default
     def _set_timeout(self) -> Optional[int]:
         return self._get_default_timeout()
 
     def _get_default_system_encoding(self) -> str:
-        encoding = None
+        encoding: Optional[str] = None
+
         if not platform.is_windows() and sys.stdin is not None:
+            # On Linux we can rely on sys.stdin for the encoding since it
+            # most commonly matches the file-system encoding. This however
+            # does not apply to windows
             encoding = sys.stdin.encoding
+
         if not encoding:
+            # If the system is properly configured this should return a valid
+            # encoding. MS Windows has problems with this and reports the wrong
+            # encoding
+
             try:
-                encoding = locale.getdefaultlocale()[-1]
-            except ValueError:
-                pass
+                encoding = locale.getencoding()  # type: ignore[attr-defined]
+            except AttributeError:
+                # Python < 3.11
+                encoding = locale.getpreferredencoding(do_setlocale=True)
+
             if not encoding:
+                # This is most likely ascii which is not the best but we were
+                # unable to find a better encoding. If this fails, we fall all
+                # the way back to ascii
                 encoding = sys.getdefaultencoding()
             if not encoding:
                 if platform.is_darwin():
-                    encoding = 'utf-8'
+                    # Mac OS X uses UTF-8
+                    encoding = "utf-8"
                 elif platform.is_windows():
-                    encoding = 'mbcs'
+                    # Windows uses a configurable encoding; on Windows, Python uses the name “mbcs”
+                    # to refer to whatever the currently configured encoding is.
+                    encoding = "mbcs"
                 else:
-                    encoding = 'ascii'
+                    # On linux default to ascii as a last resort
+                    encoding = "ascii"
+
         if not encoding:
-            encoding = 'utf-8'
+            # If we still didn't detect the encoding, default to utf-8
+            encoding = "utf-8"
+
         return encoding
 
     def _get_default_timeout(self) -> Optional[int]:
         return None
 
-    def _get_impl_class(self) -> 'Type[SubprocessImpl]':
+    def _get_impl_class(self) -> "Type[SubprocessImpl]":
         """
         Return the ``impl`` class to use.
         """
         return SubprocessImpl
 
     def __attrs_post_init__(self) -> None:
         """
@@ -398,15 +442,15 @@
         self._cmdline = list(args)
         return self._cmdline
 
     def get_display_name(self) -> str:
         """
         Returns a human readable name for the factory.
         """
-        return '{}({})'.format(self.__class__.__name__, self._cmdline or '')
+        return "{}({})".format(self.__class__.__name__, self._cmdline or "")
 
     def is_running(self) -> bool:
         """
         Returns true if the sub-process is alive.
         """
         return self.impl.is_running()
 
@@ -431,15 +475,15 @@
     """
 
     def run(
         self,
         *args: str,
         env: Optional[EnvironDict] = None,
         _timeout: Optional[Union[int, float]] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> ProcessResult:
         """
         Run the given command synchronously.
 
         Keyword Arguments:
             args:
                 The list of arguments to pass to :py:meth:`~pytestshellutils.shell.Subprocess.cmdline`
@@ -448,49 +492,50 @@
                 Pass a dictionary of environment key, value pairs to inject into the subprocess.
             _timeout:
                 The timeout value for this particular ``run()`` call. If this value is not ``None``,
                 it will be used instead of :py:attr:`~pytestshellutils.shell.Subprocess.timeout`,
                 the default timeout.
         """
         start_time = time.time()
+        # Build the cmdline to pass to the terminal
+        # We set the _terminal_timeout attribute while calling cmdline in case it needs
+        # access to that information to build the command line
         self.impl._terminal_timeout = _timeout or self.timeout
         timmed_out = False
         try:
             self.impl.run(*args, env=env, **kwargs)
             if TYPE_CHECKING:
+                # Make mypy happy
                 assert self.impl._terminal
             self.impl._terminal.communicate(timeout=self.impl._terminal_timeout)
         except subprocess.TimeoutExpired:
             timmed_out = True
+
         result = self.terminate()
         cmdline = result.cmdline
         returncode = result.returncode
         if timmed_out:
             raise FactoryTimeout(
-                '{} Failed to run: {}; Error: Timed out after {:.2f} seconds!'.format(
+                "{} Failed to run: {}; Error: Timed out after {:.2f} seconds!".format(
                     self, cmdline, time.time() - start_time
                 ),
                 process_result=result,
             )
         stdout, stderr, json_out = self.process_output(
             result.stdout, result.stderr, cmdline=cmdline
         )
         log.info(
-            '%s completed %r in CWD: %s after %.2f seconds',
+            "%s completed %r in CWD: %s after %.2f seconds",
             self,
             cmdline,
             self.cwd,
             time.time() - start_time,
         )
         return ProcessResult(
-            returncode=returncode,
-            stdout=stdout,
-            stderr=stderr,
-            data=json_out,
-            cmdline=cmdline,
+            returncode=returncode, stdout=stdout, stderr=stderr, data=json_out, cmdline=cmdline
         )
 
     def process_output(
         self, stdout: str, stderr: str, cmdline: Optional[List[str]] = None
     ) -> Tuple[str, str, Optional[Dict[Any, Any]]]:
         """
         Process the output. When possible JSON is loaded from the output.
@@ -498,19 +543,15 @@
         Returns:
             Returns a tuple in the form of ``(stdout, stderr, loaded_json)``
         """
         if stdout:
             try:
                 json_out = json.loads(stdout)
             except ValueError:
-                log.debug(
-                    '%s failed to load JSON from the following output:\n%r',
-                    self,
-                    stdout,
-                )
+                log.debug("%s failed to load JSON from the following output:\n%r", self, stdout)
                 json_out = None
         else:
             json_out = None
         return stdout, stderr, json_out
 
 
 @attr.s(slots=True, kw_only=True)
@@ -527,49 +568,46 @@
             An list or tuple iterable of the base arguments to use when building the command line to
             launch the process
 
     Please look at :py:class:`~pytestshellutils.shell.Factory` for the additional supported keyword
     arguments documentation.
     """
 
-    script_name = attr.ib()
-    base_script_args = attr.ib(factory=list)
+    script_name: str = attr.ib()
+    base_script_args: List[str] = attr.ib(factory=list)
 
     def get_display_name(self) -> str:
         """
         Returns a human readable name for the factory.
         """
-        return '{0}({1})'.format(
-            self.__class__.__name__, pathlib.Path(self.script_name).name
-        )
+        return f"{self.__class__.__name__}({pathlib.Path(self.script_name).name})"
 
     def get_script_path(self) -> str:
         """
         Returns the path to the script to run.
         """
-        script_path = None
+        script_path: Optional[str]
         if os.path.isabs(self.script_name):
             script_path = self.script_name
         else:
             script_path = shutil.which(self.script_name)
         if not script_path or not os.path.exists(script_path):
-            raise FileNotFoundError(
-                "The CLI script '{0}' does not exist".format(self.script_name)
-            )
+            raise FileNotFoundError(f"The CLI script '{self.script_name}' does not exist")
         if TYPE_CHECKING:
+            # Make mypy happy
             assert script_path
         return script_path
 
     def get_base_script_args(self) -> List[str]:
         """
         Returns any additional arguments to pass to the CLI script.
         """
         return list(self.base_script_args)
 
-    def get_script_args(self) -> List[str]:
+    def get_script_args(self) -> List[str]:  # pylint: disable=no-self-use
         """
         Returns any additional arguments to pass to the CLI script.
         """
         return []
 
     def cmdline(self, *args: str) -> List[str]:
         """
@@ -597,37 +635,38 @@
     Keyword Arguments:
         args:
             List of arguments
         kwargs:
             Dictionary of keyword arguments
     """
 
-    args = attr.ib()
-    kwargs = attr.ib()
+    args: Tuple[str, ...] = attr.ib()
+    kwargs: Dict[str, Any] = attr.ib()
 
 
 @attr.s(slots=True, kw_only=True)
 class DaemonImpl(SubprocessImpl):
     """
     Daemon subprocess interaction implementation.
 
     Please look at :py:class:`~pytestshellutils.shell.SubprocessImpl` for the additional supported keyword
     arguments documentation.
     """
 
-    factory = attr.ib()
-    _before_start_callbacks = attr.ib(repr=False, hash=False, factory=list)
-    _after_start_callbacks = attr.ib(repr=False, hash=False, factory=list)
-    _before_terminate_callbacks = attr.ib(repr=False, hash=False, factory=list)
-    _after_terminate_callbacks = attr.ib(repr=False, hash=False, factory=list)
-    _start_args_and_kwargs = attr.ib(init=False, repr=False, hash=False, default=None)
-
-    def before_start(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    factory: "Daemon" = attr.ib()
+
+    _before_start_callbacks: List[Callback] = attr.ib(repr=False, hash=False, factory=list)
+    _after_start_callbacks: List[Callback] = attr.ib(repr=False, hash=False, factory=list)
+    _before_terminate_callbacks: List[Callback] = attr.ib(repr=False, hash=False, factory=list)
+    _after_terminate_callbacks: List[Callback] = attr.ib(repr=False, hash=False, factory=list)
+    _start_args_and_kwargs: StartDaemonCallArguments = attr.ib(
+        init=False, repr=False, hash=False, default=None
+    )
+
+    def before_start(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run before the daemon starts.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -636,21 +675,17 @@
                 The arguments to pass to the callback
             kwargs:
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
-        self._before_start_callbacks.append(
-            Callback(func=callback, args=args, kwargs=kwargs)
-        )
+        self._before_start_callbacks.append(Callback(func=callback, args=args, kwargs=kwargs))
 
-    def after_start(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def after_start(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run after the daemon starts.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -659,21 +694,17 @@
                 The arguments to pass to the callback
             kwargs:
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
-        self._after_start_callbacks.append(
-            Callback(func=callback, args=args, kwargs=kwargs)
-        )
+        self._after_start_callbacks.append(Callback(func=callback, args=args, kwargs=kwargs))
 
-    def before_terminate(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def before_terminate(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run before the daemon terminates.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -682,21 +713,17 @@
                 The arguments to pass to the callback
             kwargs:
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
-        self._before_terminate_callbacks.append(
-            Callback(func=callback, args=args, kwargs=kwargs)
-        )
+        self._before_terminate_callbacks.append(Callback(func=callback, args=args, kwargs=kwargs))
 
-    def after_terminate(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def after_terminate(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run after the daemon terminates.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -705,23 +732,21 @@
                 The arguments to pass to the callback
             kwargs:
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
-        self._after_terminate_callbacks.append(
-            Callback(func=callback, args=args, kwargs=kwargs)
-        )
+        self._after_terminate_callbacks.append(Callback(func=callback, args=args, kwargs=kwargs))
 
     def start(
         self,
         *extra_cli_arguments: str,
         max_start_attempts: Optional[int] = None,
-        start_timeout: Optional[Union[int, float]] = None
+        start_timeout: Optional[Union[int, float]] = None,
     ) -> bool:
         """
         Start the daemon.
 
         Keyword Arguments:
             extra_cli_arguments:
                 Extra arguments to pass to the CLI that starts the daemon
@@ -729,134 +754,132 @@
                 Maximum number of attempts to try and start the daemon in case of failures
             start_timeout:
                 The maximum number of seconds to wait before considering that the daemon did not start
 
         Returns:
             bool: A boolean indicating if the start was successful or not.
         """
-        if self.is_running():
-            log.warning('%s is already running.', self)
+        if self.is_running():  # pragma: no cover
+            log.warning("%s is already running.", self)
             return True
         self._start_args_and_kwargs = StartDaemonCallArguments(
             args=extra_cli_arguments,
-            kwargs={
-                'max_start_attempts': max_start_attempts,
-                'start_timeout': start_timeout,
-            },
+            kwargs={"max_start_attempts": max_start_attempts, "start_timeout": start_timeout},
         )
         process_running = False
         start_time = time.time()
         start_attempts = max_start_attempts or self.factory.max_start_attempts
         current_attempt = 0
         run_arguments = list(extra_cli_arguments)
         while True:
             if process_running:
                 break
             current_attempt += 1
             if current_attempt > start_attempts:
                 break
             log.info(
-                'Starting %s. Attempt: %d of %d',
-                self.factory,
-                current_attempt,
-                start_attempts,
+                "Starting %s. Attempt: %d of %d", self.factory, current_attempt, start_attempts
             )
-            for callback in self._before_start_callbacks:
+            for callback in self._before_start_callbacks:  # pylint: disable=not-an-iterable
                 try:
                     callback()
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.info(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         callback,
                         exc,
                         exc_info=True,
                     )
             current_start_time = time.time()
             start_running_timeout = current_start_time + (
                 start_timeout or self.factory.start_timeout
             )
-            if (
-                current_attempt > 1
-                and self.factory.extra_cli_arguments_after_first_start_failure
-            ):
+            if current_attempt > 1 and self.factory.extra_cli_arguments_after_first_start_failure:
                 run_arguments = list(extra_cli_arguments) + list(
                     self.factory.extra_cli_arguments_after_first_start_failure
                 )
             self.run(*run_arguments)
-            if not self.is_running():
+            if not self.is_running():  # pragma: no cover
+                # A little breathe time to allow the process to start if not started already
                 time.sleep(0.5)
             while time.time() <= start_running_timeout:
                 if not self.is_running():
-                    log.warning('%s is no longer running', self.factory)
+                    log.warning("%s is no longer running", self.factory)
                     self.terminate()
                     break
                 try:
                     if (
-                        self.factory.run_start_checks(
-                            current_start_time, start_running_timeout
-                        )
+                        self.factory.run_start_checks(current_start_time, start_running_timeout)
                         is False
                     ):
                         time.sleep(1)
                         continue
                 except FactoryNotStarted:
                     self.terminate()
                     break
                 log.info(
-                    'The %s factory is running after %d attempts. Took %1.2f seconds',
+                    "The %s factory is running after %d attempts. Took %1.2f seconds",
                     self.factory,
                     current_attempt,
                     time.time() - start_time,
                 )
                 process_running = True
                 break
             else:
+                # The factory failed to confirm it's running status
                 self.terminate()
         if process_running:
-            for callback in self._after_start_callbacks:
+            for callback in self._after_start_callbacks:  # pylint: disable=not-an-iterable
                 try:
                     callback()
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.info(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         callback,
                         exc,
                         exc_info=True,
                     )
             return process_running
         result = self.terminate()
         raise FactoryNotStarted(
-            'The {} factory has failed to confirm running status after {} attempts, which took {:.2f} seconds'.format(
-                self.factory, current_attempt - 1, time.time() - start_time
+            "The {} factory has failed to confirm running status after {} attempts, which "
+            "took {:.2f} seconds".format(
+                self.factory,
+                current_attempt - 1,
+                time.time() - start_time,
             ),
             process_result=result,
         )
 
     def terminate(self) -> ProcessResult:
         """
         Terminate the daemon.
         """
         if self._terminal_result is not None:
+            # This factory has already been terminated
             return self._terminal_result
-        for callback in self._before_terminate_callbacks:
+        for callback in self._before_terminate_callbacks:  # pylint: disable=not-an-iterable
             try:
                 callback()
-            except CallbackException as exc:
+            except CallbackException as exc:  # pragma: no cover
                 log.info(
-                    'Exception raised when running %s: %s', callback, exc, exc_info=True
+                    "Exception raised when running %s: %s",
+                    callback,
+                    exc,
+                    exc_info=True,
                 )
         try:
             return super().terminate()
         finally:
-            for callback in self._after_terminate_callbacks:
+            for callback in self._after_terminate_callbacks:  # pylint: disable=not-an-iterable
                 try:
                     callback()
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.warning(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         callback,
                         exc,
                         exc_info=True,
                     )
 
     def get_start_arguments(self) -> StartDaemonCallArguments:
         """
@@ -880,48 +903,48 @@
         start_timeout:
             The maximum number of seconds to wait before considering that the daemon did not start
 
     Please look at :py:class:`~pytestshellutils.shell.Subprocess` for the additional supported keyword
     arguments documentation.
     """
 
-    impl = attr.ib(repr=False, init=False)
-    script_name = attr.ib()
-    base_script_args = attr.ib(factory=list)
-    check_ports = attr.ib(factory=list)
-    stats_processes = attr.ib(repr=False, hash=False, default=None)
-    start_timeout = attr.ib(repr=False)
-    max_start_attempts = attr.ib(repr=False, default=3)
-    extra_cli_arguments_after_first_start_failure = attr.ib(hash=False, factory=list)
-    listen_ports = attr.ib(init=False, repr=False, hash=False, factory=list)
-    _start_checks_callbacks = attr.ib(repr=False, hash=False, factory=list)
+    impl: DaemonImpl = attr.ib(repr=False, init=False)
+
+    script_name: str = attr.ib()
+    base_script_args: List[str] = attr.ib(factory=list)
+    check_ports: List[int] = attr.ib(factory=list)
+    stats_processes: "StatsProcesses" = attr.ib(repr=False, hash=False, default=None)
+    start_timeout: Union[int, float] = attr.ib(repr=False)
+    max_start_attempts: int = attr.ib(repr=False, default=3)
+    extra_cli_arguments_after_first_start_failure: List[str] = attr.ib(hash=False, factory=list)
+    listen_ports: List[int] = attr.ib(init=False, repr=False, hash=False, factory=list)
+    _start_checks_callbacks: List[Callback] = attr.ib(repr=False, hash=False, factory=list)
 
-    def _get_impl_class(self) -> 'Type[DaemonImpl]':
+    def _get_impl_class(self) -> "Type[DaemonImpl]":
         """
         Return the ``impl`` class to use.
         """
         return DaemonImpl
 
     def __attrs_post_init__(self) -> None:
         """
         Post ``attrs`` class initialization routines.
         """
         super().__attrs_post_init__()
         if self.check_ports and not isinstance(self.check_ports, (list, tuple)):
             self.check_ports = [self.check_ports]
         if self.check_ports:
             self.listen_ports.extend(self.check_ports)
+
         self.after_start(self._add_factory_to_stats_processes)
         self.after_terminate(self._terminate_processes_matching_listen_ports)
         self.after_terminate(self._remove_factory_from_stats_processes)
         self.start_check(self._check_listening_ports)
 
-    def before_start(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def before_start(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run before the daemon starts.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -932,17 +955,15 @@
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
         self.impl.before_start(callback, *args, **kwargs)
 
-    def after_start(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def after_start(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run after the daemon starts.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -953,17 +974,15 @@
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
         self.impl.after_start(callback, *args, **kwargs)
 
-    def before_terminate(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def before_terminate(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run before the daemon terminates.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -974,17 +993,15 @@
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
         self.impl.before_terminate(callback, *args, **kwargs)
 
-    def after_terminate(
-        self, callback: Callable[[], None], *args: Any, **kwargs: Any
-    ) -> None:
+    def after_terminate(self, callback: Callable[[], None], *args: Any, **kwargs: Any) -> None:
         """
         Register a function callback to run after the daemon terminates.
 
         Arguments:
             callback:
                 The function to call back
 
@@ -995,17 +1012,15 @@
                 The keyword arguments to pass to the callback
 
         Returns:
             Nothing.
         """
         self.impl.after_terminate(callback, *args, **kwargs)
 
-    def start_check(
-        self, callback: Callable[..., bool], *args: Any, **kwargs: Any
-    ) -> None:
+    def start_check(self, callback: Callable[..., bool], *args: Any, **kwargs: Any) -> None:
         """
         Register a function to run after the daemon starts to confirm readiness for work.
 
         The callback must accept as the first argument ``timeout_at`` which is a float.
         The callback must stop trying to confirm running behavior once ``time.time() > timeout_at``.
         The callback should return ``True`` to confirm that the daemon is ready for work.
 
@@ -1031,17 +1046,15 @@
                         ...
                         # if all is good
                         break
                     else:
                         return False
                     return True
         """
-        self._start_checks_callbacks.append(
-            Callback(func=callback, args=args, kwargs=kwargs)
-        )
+        self._start_checks_callbacks.append(Callback(func=callback, args=args, kwargs=kwargs))
 
     def get_check_ports(self) -> List[int]:
         """
         Return a list of ports to check against to ensure the daemon is running.
         """
         return self.check_ports or []
 
@@ -1051,32 +1064,30 @@
         """
         return self._start_checks_callbacks or []
 
     def start(
         self,
         *extra_cli_arguments: str,
         max_start_attempts: Optional[int] = None,
-        start_timeout: Optional[Union[int, float]] = None
+        start_timeout: Optional[Union[int, float]] = None,
     ) -> bool:
         """
         Start the daemon.
         """
         return self.impl.start(
-            *extra_cli_arguments,
-            max_start_attempts=max_start_attempts,
-            start_timeout=start_timeout,
+            *extra_cli_arguments, max_start_attempts=max_start_attempts, start_timeout=start_timeout
         )
 
     @contextlib.contextmanager
     def started(
         self,
         *extra_cli_arguments: str,
         max_start_attempts: Optional[int] = None,
-        start_timeout: Optional[Union[int, float]] = None
-    ) -> Generator['Daemon', None, None]:
+        start_timeout: Optional[Union[int, float]] = None,
+    ) -> Generator["Daemon", None, None]:
         """
         Start the daemon and return it's instance so it can be used as a context manager.
         """
         try:
             self.start(
                 *extra_cli_arguments,
                 max_start_attempts=max_start_attempts,
@@ -1085,19 +1096,19 @@
             yield self
         finally:
             self.terminate()
 
     @contextlib.contextmanager
     def stopped(
         self,
-        before_stop_callback: Optional[Callable[['Daemon'], None]] = None,
-        after_stop_callback: Optional[Callable[['Daemon'], None]] = None,
-        before_start_callback: Optional[Callable[['Daemon'], None]] = None,
-        after_start_callback: Optional[Callable[['Daemon'], None]] = None,
-    ) -> Generator['Daemon', None, None]:
+        before_stop_callback: Optional[Callable[["Daemon"], None]] = None,
+        after_stop_callback: Optional[Callable[["Daemon"], None]] = None,
+        before_start_callback: Optional[Callable[["Daemon"], None]] = None,
+        after_start_callback: Optional[Callable[["Daemon"], None]] = None,
+    ) -> Generator["Daemon", None, None]:
         """
         Stop the daemon and return it's instance so it can be used as a context manager.
 
         Keyword Arguments:
             before_stop_callback:
                 A callable to run before stopping the daemon. The callback must accept one argument,
                 the daemon instance.
@@ -1121,138 +1132,138 @@
 
                 with factory.stopped():
                     assert factory.is_running() is False
 
                 assert factory.is_running() is True
         """
         if not self.is_running():
-            raise FactoryNotRunning('{0} is not running '.format(self))
+            raise FactoryNotRunning(f"{self} is not running ")
         start_arguments = self.impl.get_start_arguments()
         try:
             if before_stop_callback:
                 try:
                     before_stop_callback(self)
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.info(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         format_callback_to_string(before_stop_callback),
                         exc,
                         exc_info=True,
                     )
             self.terminate()
             if after_stop_callback:
                 try:
                     after_stop_callback(self)
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.info(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         format_callback_to_string(after_stop_callback),
                         exc,
                         exc_info=True,
                     )
             yield self
-        except ShellUtilsException:
+        except ShellUtilsException:  # pragma: no cover pylint: disable=try-except-raise
             raise
         else:
             if before_start_callback:
                 try:
                     before_start_callback(self)
-                except CallbackException as exc:
+                except CallbackException as exc:  # pragma: no cover
                     log.info(
-                        'Exception raised when running %s: %s',
+                        "Exception raised when running %s: %s",
                         format_callback_to_string(before_start_callback),
                         exc,
                         exc_info=True,
                     )
-            _started = self.start(*start_arguments.args, **start_arguments.kwargs)
+            _started = self.start(
+                *start_arguments.args,  # pylint: disable=not-an-iterable
+                **start_arguments.kwargs,  # pylint: disable=not-a-mapping
+            )
             if _started:
                 if after_start_callback:
                     try:
                         after_start_callback(self)
-                    except CallbackException as exc:
+                    except CallbackException as exc:  # pragma: no cover
                         log.info(
-                            'Exception raised when running %s: %s',
+                            "Exception raised when running %s: %s",
                             format_callback_to_string(after_start_callback),
                             exc,
                             exc_info=True,
                         )
 
     def run_start_checks(self, started_at: float, timeout_at: float) -> bool:
         """
         Run checks to confirm that the daemon has started.
         """
         start_check_callbacks = list(self.get_start_check_callbacks())
         if not start_check_callbacks:
-            log.debug('No start check callbacks to run for %s', self)
+            log.debug("No start check callbacks to run for %s", self)
             return True
         checks_start_time = time.time()
-        log.debug('%s is running start checks', self)
+        log.debug("%s is running start checks", self)
         while time.time() <= timeout_at:
             if not self.is_running():
-                raise FactoryNotStarted('{0} is no longer running'.format(self))
+                raise FactoryNotStarted(f"{self} is no longer running")
             if not start_check_callbacks:
                 break
             start_check = start_check_callbacks[0]
             try:
                 ret = start_check(timeout_at)
                 if ret is True:
                     start_check_callbacks.pop(0)
-            except Exception as exc:
+            except Exception as exc:  # pylint: disable=broad-except
                 log.info(
-                    'Exception raised when running %s: %s',
+                    "Exception raised when running %s: %s",
                     start_check,
                     exc,
                     exc_info=True,
                 )
         if start_check_callbacks:
             log.error(
-                'Failed to run start check callbacks after %1.2f seconds for %s. Remaining start check callbacks: %s',
+                "Failed to run start check callbacks after %1.2f seconds for %s. "
+                "Remaining start check callbacks: %s",
                 time.time() - checks_start_time,
                 self,
                 start_check_callbacks,
             )
             return False
-        log.debug('All start check callbacks executed for %s', self)
+        log.debug("All start check callbacks executed for %s", self)
         return True
 
     def _check_listening_ports(self, timeout_at: float) -> bool:
         """
         Check if the defined ports are in a listening state.
 
         This callback will run when trying to assess if the daemon is ready
         to accept work by trying to connect to each of the ports it's supposed
         to be listening.
         """
         check_ports = set(self.get_check_ports())
         if not check_ports:
-            log.debug('No ports to check connection to for %s', self)
+            log.debug("No ports to check connection to for %s", self)
             return True
-        log.debug(
-            'Listening ports to check for %s: %s', self, set(self.get_check_ports())
-        )
+        log.debug("Listening ports to check for %s: %s", self, set(self.get_check_ports()))
         checks_start_time = time.time()
         while time.time() <= timeout_at:
             if not self.is_running():
-                raise FactoryNotStarted('{0} is no longer running'.format(self))
+                raise FactoryNotStarted(f"{self} is no longer running")
             if not check_ports:
                 break
             check_ports -= ports.get_connectable_ports(check_ports)
             if check_ports:
                 time.sleep(1.5)
         else:
             log.error(
-                'Failed to check ports after %1.2f seconds for %s. Remaining ports to check: %s',
+                "Failed to check ports after %1.2f seconds for %s. Remaining ports to check: %s",
                 time.time() - checks_start_time,
                 self,
                 check_ports,
             )
             return False
-        log.debug(
-            'All listening ports checked for %s: %s', self, set(self.get_check_ports())
-        )
+        log.debug("All listening ports checked for %s: %s", self, set(self.get_check_ports()))
         return True
 
     def _add_factory_to_stats_processes(self) -> None:
         if self.stats_processes is not None:
             display_name = self.get_display_name()
             self.stats_processes.add(display_name, self.pid)
 
@@ -1260,52 +1271,58 @@
         if self.stats_processes is not None:
             display_name = self.get_display_name()
             self.stats_processes.remove(display_name)
 
     def _terminate_processes_matching_listen_ports(self) -> None:
         if not self.listen_ports:
             return
+        # If any processes were not terminated and are listening on the ports
+        # we have set on listen_ports, terminate those processes.
         found_processes = []
-        for process in psutil.process_iter(['connections']):
+        for process in psutil.process_iter(["connections"]):
             try:
                 for connection in process.connections():
                     if connection.status != psutil.CONN_LISTEN:
+                        # We only care about listening services
                         continue
                     if connection.laddr.port in self.check_ports:
                         found_processes.append(process)
+                        # We already found one connection, no need to check the others
                         break
-            except psutil.AccessDenied:
+            except psutil.AccessDenied:  # pragma: no cover
+                # We've been denied access to this process connections. Carry on.
                 continue
             except psutil.ZombieProcess:
                 continue
         if found_processes:
             log.debug(
-                'The following processes were found listening on ports %s: %s',
-                ', '.join([str(port) for port in self.listen_ports]),
+                "The following processes were found listening on ports %s: %s",
+                ", ".join(
+                    [str(port) for port in self.listen_ports],  # pylint: disable=not-an-iterable
+                ),
                 found_processes,
             )
             terminate_process_list(found_processes, kill=True, slow_stop=False)
         else:
             log.debug(
-                'No astray processes were found listening on ports: %s',
-                ', '.join([str(port) for port in self.listen_ports]),
+                "No astray processes were found listening on ports: %s",
+                ", ".join(
+                    [str(port) for port in self.listen_ports],  # pylint: disable=not-an-iterable
+                ),
             )
 
-    def __enter__(self) -> 'Daemon':
+    def __enter__(self) -> "Daemon":
         """
         Use class as a context manager.
         """
         if not self.is_running():
             raise RuntimeError(
-                """Factory not yet started. Perhaps you're after something like:
-
-with {}.started() as factory:
-    yield factory""".format(
-                    self.__class__.__name__
-                )
+                "Factory not yet started. Perhaps you're after something like:\n\n"
+                "with {}.started() as factory:\n"
+                "    yield factory".format(self.__class__.__name__)
             )
         return self
 
     def __exit__(self, *_: Any) -> None:
         """
         Exit the class context manager.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/__init__.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
-from __future__ import generator_stop
 import inspect
 import pathlib
 import sys
 import warnings
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import Union
+
 import packaging.version
+
 import pytestshellutils
 
 if TYPE_CHECKING:
     from packaging.version import Version
 
 
 def resolved_pathlib_path(path: Union[str, pathlib.Path]) -> pathlib.Path:
@@ -47,33 +48,33 @@
             The callback arguments
         kwargs:
             The callback keyword arguments
 
     Returns:
         str: The formatted callback string
     """
-    callback_str = None
+    callback_str: str
     if not isinstance(callback, str):
         try:
-            callback_str = '{0}('.format(callback.__qualname__)
-        except AttributeError:
-            callback_str = '{0}('.format(callback.__name__)
+            callback_str = f"{callback.__qualname__}("
+        except AttributeError:  # pragma: no cover
+            callback_str = f"{callback.__name__}("
     else:
-        callback_str = '{0}('.format(callback)
+        callback_str = f"{callback}("
     if args:
-        callback_str += ', '.join([repr(arg) for arg in args])
+        callback_str += ", ".join([repr(arg) for arg in args])
     if kwargs:
         if args:
-            callback_str += ', '
-        callback_str += ', '.join(['{0}={1}'.format(k, v) for k, v in kwargs.items()])
-    callback_str += ')'
+            callback_str += ", "
+        callback_str += ", ".join([f"{k}={v!r}" for (k, v) in kwargs.items()])
+    callback_str += ")"
     return callback_str
 
 
-def warn_until(
+def warn_until(  # pragma: no cover
     version: str,
     message: str,
     category: Type[Warning] = DeprecationWarning,
     stacklevel: Optional[int] = None,
     _dont_call_warnings: bool = False,
     _pkg_version_: Optional[str] = None,
 ) -> None:
@@ -103,23 +104,34 @@
             raise a ``RuntimeError``.
 
     Returns:
         Nothing.
     """
     _version = packaging.version.parse(version)
     if _pkg_version_ is None:
-        _pkg_version_ = pytestshellutils.__version__
+        _pkg_version_ = pytestshellutils.__version__  # type: ignore[attr-defined]
     _pkg_version = packaging.version.parse(_pkg_version_)
+
     if stacklevel is None:
+        # Attribute the warning to the calling function, not to warn_until()
         stacklevel = 3
+
     if _pkg_version >= _version:
         caller = inspect.getframeinfo(sys._getframe(stacklevel - 1))
         raise RuntimeError(
-            "The warning triggered on filename '{filename}', line number {lineno}, is supposed to be shown until version {until_version} is released. Current version is now {version}. Please remove the warning.".format(
+            "The warning triggered on filename '{filename}', line number "
+            "{lineno}, is supposed to be shown until version "
+            "{until_version} is released. Current version is now "
+            "{version}. Please remove the warning.".format(
                 filename=caller.filename,
                 lineno=caller.lineno,
                 until_version=_pkg_version_,
                 version=version,
-            )
+            ),
         )
+
     if _dont_call_warnings is False:
-        warnings.warn(message.format(version=version), category, stacklevel=stacklevel)
+        warnings.warn(
+            message.format(version=version),
+            category,
+            stacklevel=stacklevel,
+        )
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/ports.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/ports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Ports related utility functions.
 """
-from __future__ import generator_stop
 import contextlib
 import logging
 from typing import Iterable
 from typing import Set
+
 import pytest
+
 import pytestshellutils.utils.socket as socket
 
 log = logging.getLogger(__name__)
 
 
 def get_unused_localhost_port(use_cache: bool = False) -> int:
     """
     Return a random unused port on localhost.
 
     Keyword Arguments:
         use_cache:
             If ``use_cache`` is ``True``, consecutive calls to this function will never return the cached port.
     """
-    if not isinstance(use_cache, bool):
+    if not isinstance(use_cache, bool):  # pragma: no cover
         raise pytest.UsageError(
-            "The value of 'use_cache' needs to be an boolean, not {0}".format(
-                type(use_cache)
-            )
+            f"The value of 'use_cache' needs to be an boolean, not {type(use_cache)}"
         )
-    with contextlib.closing(
-        socket.socket(family=socket.AF_INET, type=socket.SOCK_STREAM)
-    ) as usock:
-        usock.bind(('127.0.0.1', 0))
-        port = usock.getsockname()[1]
+
+    with contextlib.closing(socket.socket(family=socket.AF_INET, type=socket.SOCK_STREAM)) as usock:
+        usock.bind(("127.0.0.1", 0))
+        port: int = usock.getsockname()[1]
+
     if use_cache:
         try:
-            cached_ports = get_unused_localhost_port.__cached_ports__
+            cached_ports = get_unused_localhost_port.__cached_ports__  # type: ignore[attr-defined]
         except AttributeError:
-            cached_ports = get_unused_localhost_port.__cached_ports__ = set()
+            cached_ports = get_unused_localhost_port.__cached_ports__ = set()  # type: ignore[attr-defined]
         if port in cached_ports:
             return get_unused_localhost_port(use_cache=use_cache)
         cached_ports.add(port)
+
     return port
 
 
 def get_connectable_ports(ports: Iterable[int]) -> Set[int]:
     """
     Given a list of ports, returns those that we can connect to.
 
@@ -52,20 +52,19 @@
         ports: An iterable of ports to try and connect to
 
     Returns:
         set: Returns a set of the ports where connection was successful
     """
     connectable_ports = set()
     check_ports = set(ports)
+
     for port in set(check_ports):
-        with contextlib.closing(
-            socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        ) as sock:
-            conn = sock.connect_ex(('localhost', port))
+        with contextlib.closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
+            conn = sock.connect_ex(("localhost", port))
             try:
                 if conn == 0:
-                    log.debug('Port %s is connectable!', port)
+                    log.debug("Port %s is connectable!", port)
                     connectable_ports.add(port)
                     sock.shutdown(socket.SHUT_RDWR)
-            except OSError:
+            except OSError:  # pragma: no cover
                 continue
     return connectable_ports
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/downgraded/utils/socket.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/socket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: disable=wildcard-import,unused-wildcard-import
 """
 Namespace the standard library :py:mod:`socket` module.
 
 This module's sole purpose is to have the standard library :py:mod:`socket` module functions under a different
 namespace to be used in pytest-shell-utilities so that projects using it, which need to mock :py:mod:`socket` functions,
 don't influence the pytest-shell-utilities run time behavior.
 """
-from __future__ import generator_stop
 from socket import *
```

### Comparing `pytest-shell-utilities-1.7.0/src/pytestshellutils/utils/processes.py` & `pytest-shell-utilities-1.8.0/src/pytestshellutils/utils/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Process related utilities.
 """
 import errno
 import json
 import logging
@@ -15,15 +15,15 @@
 from typing import Optional
 
 import attr
 import psutil
 
 try:
     from pytest import LineMatcher
-except ImportError:
+except ImportError:  # pragma: no cover
     # Older pytest
     from _pytest.pytester import LineMatcher
 
 from pytestshellutils.utils import warn_until
 
 
 log = logging.getLogger(__name__)
@@ -109,15 +109,15 @@
                     data = data[self.data_key]
                 return data
             except ValueError:
                 pass
         return None
 
     @property
-    def exitcode(self) -> int:
+    def exitcode(self) -> int:  # pragma: no cover
         """
         Return the process returncode.
 
         This property is deprecated and should not be used.
         It only exists to support projects that are migrating from
         pytest-salt-factories versions. Use ``.returncode`` instead.
         """
@@ -125,15 +125,15 @@
             "2.0.0",
             "The '.exitcode' property is deprecated and will cease to exist after "
             "pytest-shell-utilities {version}. Please use '.returncode' instead.",
         )
         return self.returncode
 
     @property
-    def json(self) -> Optional[Dict[Any, Any]]:
+    def json(self) -> Optional[Dict[Any, Any]]:  # pragma: no cover
         """
         Return the process output parsed as JSON, if possible.
 
         This property is deprecated and should not be used.
         It only exists to support projects that are migrating from
         pytest-salt-factories versions. Use ``.data`` instead.
         """
@@ -191,15 +191,15 @@
     try:
         return proc._cmdline
     except AttributeError:
         # Cache the cmdline since that will be inaccessible once the process is terminated
         # and we use it in log calls
         try:
             cmdline = proc.cmdline()
-        except (psutil.NoSuchProcess, psutil.AccessDenied):
+        except (psutil.NoSuchProcess, psutil.AccessDenied):  # pragma: no cover
             # OSX is more restrictive about the above information
             cmdline = None
         except OSError:  # pragma: no cover
             # On Windows we've seen something like:
             #   File " c: ... \lib\site-packages\pytestsalt\utils\__init__.py", line 182, in terminate_process
             #     terminate_process_list(process_list, kill=slow_stop is False, slow_stop=slow_stop)
             #   File " c: ... \lib\site-packages\pytestsalt\utils\__init__.py", line 130, in terminate_process_list
@@ -233,15 +233,15 @@
             #         basic_mem = self.memory_info()
             # >       uss = cext.proc_memory_uss(self.pid)
             # E       RuntimeError: NtQueryVirtualMemory failed
             #
             # c: ... \lib\site-packages\psutil\_pswindows.py:806: RuntimeError
             cmdline = None
 
-        if not cmdline:
+        if not cmdline:  # pragma: no cover
             try:
                 cmdline = proc.as_dict()
             except psutil.NoSuchProcess:
                 cmdline = f"<could not be retrived; dead process: {proc}>"
             except (psutil.AccessDenied, OSError):  # pragma: no cover
                 cmdline = weakref.proxy(proc)
         proc._cmdline = cmdline
```

### Comparing `pytest-shell-utilities-1.7.0/tests/conftest.py` & `pytest-shell-utilities-1.8.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import functools
 import logging
 import os
 import stat
 import tempfile
```

### Comparing `pytest-shell-utilities-1.7.0/tests/functional/shell/test_daemon.py` & `pytest-shell-utilities-1.8.0/tests/functional/shell/test_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import functools
 import logging
 import pprint
 import re
 import sys
```

### Comparing `pytest-shell-utilities-1.7.0/tests/functional/shell/test_fixture.py` & `pytest-shell-utilities-1.8.0/tests/functional/shell/test_fixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 VMware, Inc.
+# Copyright 2022-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import pathlib
 import sys
 import tempfile
 
 import pytest
```

### Comparing `pytest-shell-utilities-1.7.0/tests/functional/shell/test_script_subprocess.py` & `pytest-shell-utilities-1.8.0/tests/functional/shell/test_script_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import os
 import pathlib
 import sys
 from typing import Any
 from typing import cast
```

### Comparing `pytest-shell-utilities-1.7.0/tests/functional/shell/test_subprocess.py` & `pytest-shell-utilities-1.8.0/tests/functional/shell/test_subprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 VMware, Inc.
+# Copyright 2022-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import os
 import pathlib
 import sys
 import tempfile
 from typing import Any
```

### Comparing `pytest-shell-utilities-1.7.0/tests/functional/test_exceptions.py` & `pytest-shell-utilities-1.8.0/tests/functional/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 VMware, Inc.
+# Copyright 2022-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import textwrap
 
 import pytest
 
 import pytestshellutils.exceptions as exceptions
 from pytestshellutils.utils.processes import ProcessResult
```

### Comparing `pytest-shell-utilities-1.7.0/tests/unit/customtypes/test_callback.py` & `pytest-shell-utilities-1.8.0/tests/unit/customtypes/test_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from typing import Any
 from typing import Dict
 
 import pytest
```

### Comparing `pytest-shell-utilities-1.7.0/tests/unit/utils/processes/test_processresult.py` & `pytest-shell-utilities-1.8.0/tests/unit/utils/processes/test_processresult.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Test ``pytestshellutils.utils.processes.ProcessResult``.
 """
 import json as jsonlib
 import textwrap
```

### Comparing `pytest-shell-utilities-1.7.0/tests/unit/utils/processes/test_processresult_matcher.py` & `pytest-shell-utilities-1.8.0/tests/unit/utils/processes/test_processresult_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Test ``pytestshellutils.utils.processes.ProcessResult``.
 """
 import pytest
 
 from pytestshellutils.utils.processes import ProcessResult
```

### Comparing `pytest-shell-utilities-1.7.0/tests/unit/utils/test_format_callback_to_string.py` & `pytest-shell-utilities-1.8.0/tests/unit/utils/test_format_callback_to_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from pytestshellutils.utils import format_callback_to_string
 
 
 def test_format_from_string() -> None:
     func = "the_function"
```

### Comparing `pytest-shell-utilities-1.7.0/tests/unit/utils/test_ports.py` & `pytest-shell-utilities-1.8.0/tests/unit/utils/test_ports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Test the port related utilities.
 """
 import functools
 from typing import Any
 from typing import List
```

