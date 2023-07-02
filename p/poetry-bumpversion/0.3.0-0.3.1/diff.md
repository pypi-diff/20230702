# Comparing `tmp/poetry-bumpversion-0.3.0.tar.gz` & `tmp/poetry_bumpversion-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-bumpversion-0.3.0.tar", max compression
+gzip compressed data, was "poetry_bumpversion-0.3.1.tar", max compression
```

## Comparing `poetry-bumpversion-0.3.0.tar` & `poetry_bumpversion-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1068 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/LICENSE
--rw-r--r--   0        0        0     3577 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/README.rst
--rw-r--r--   0        0        0     2696 2022-10-04 07:10:40.428354 poetry-bumpversion-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       83 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/src/poetry_bumpversion/__init__.py
--rw-r--r--   0        0        0     1140 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/src/poetry_bumpversion/models.py
--rw-r--r--   0        0        0     5474 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/src/poetry_bumpversion/plugin.py
--rw-r--r--   0        0        0        0 2022-10-04 07:10:32.544211 poetry-bumpversion-0.3.0/src/poetry_bumpversion/py.typed
--rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 poetry-bumpversion-0.3.0/setup.py
--rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 poetry-bumpversion-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-02 18:57:26.949288 poetry_bumpversion-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4043 2023-07-02 18:57:26.949288 poetry_bumpversion-0.3.1/README.rst
+-rw-r--r--   0        0        0     2564 2023-07-02 18:57:44.473440 poetry_bumpversion-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-07-02 18:57:44.501440 poetry_bumpversion-0.3.1/src/poetry_bumpversion/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-02 18:57:26.949288 poetry_bumpversion-0.3.1/src/poetry_bumpversion/models.py
+-rw-r--r--   0        0        0     5550 2023-07-02 18:57:26.949288 poetry_bumpversion-0.3.1/src/poetry_bumpversion/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:57:26.949288 poetry_bumpversion-0.3.1/src/poetry_bumpversion/py.typed
+-rw-r--r--   0        0        0     5012 1970-01-01 00:00:00.000000 poetry_bumpversion-0.3.1/PKG-INFO
```

### Comparing `poetry-bumpversion-0.3.0/LICENSE` & `poetry_bumpversion-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-bumpversion-0.3.0/README.rst` & `poetry_bumpversion-0.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,23 @@
     replace = '__version__ = "{new_version}"'
 
     [[tool.poetry_bumpversion.replacements]]
     files = ["README.md"]
     search = 'version: {current_version}'
     replace = 'version: {new_version}'
 
+******************************
+Usage with Github Workflow
+******************************
+
+This plugin uses itself in it's "Deploy to PyPI" workflow. When a release tag is created on
+GitHub, the workflow updates package version using the release tag name and deploys it to PyPI.
+You can copy the `deploy workflow code`_ to your repository to set it up.
+
+.. _deploy workflow code: https://github.com/monim67/poetry-bumpversion/blob/master/.github/workflows/deploy.yml
 
 ********************
 License
 ********************
 
 This project is licensed under MIT License - see the
 `LICENSE <https://github.com/monim67/poetry-bumpversion/blob/master/LICENSE>`_ file for details.
```

### Comparing `poetry-bumpversion-0.3.0/pyproject.toml` & `poetry_bumpversion-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "poetry-bumpversion"
-version = "0.3.0"
+version = "0.3.1"
 description = "Poetry plugin to update __version__ in __init__ file and other files containing version strings"
 authors = ["Munim Munna <6266677+monim67@users.noreply.github.com>"]
 readme = "README.rst"
-packages = [{ include = "*", from = "src" }]
+packages = [{ include = "poetry_bumpversion", from = "src" }]
 repository = "https://github.com/monim67/poetry-bumpversion"
 license = "MIT"
 keywords = ["poetry", "bump", "version", "plugin"]
 classifiers = ["Typing :: Typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 poetry = "^1.2.0a2"
 typing-extensions = "*"
-pydantic = "*"
+pydantic = "<2"
 
 [tool.poetry.group.build.dependencies]
 black = "^22.3.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 pydocstyle = {extras = ["toml"], version = "^6.1.1"}
 pytest = "^7.1.3"
 rstcheck = "^6.0.0.post1"
-poethepoet = "^0.15.0"
+poethepoet = "^0.16.3"
 coverage = { extras = ["toml"], version = "^6.4.4" }
 pre-commit = "^2.20.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^3.24.5"
 docutils = "^0.18.1" # RST Preview
 Pygments = "^2.12.0" # RST Preview
@@ -41,14 +41,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 target_version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.isort]
+py_version = "37"
 profile = "black"
 
 [tool.mypy]
 python_version = "3.7"
 namespace_packages = true
 strict = true
 
@@ -100,11 +101,7 @@
 ]
 test-cov = [
     { cmd = "coverage run" },
     { cmd = "coverage combine" },
     { cmd = "coverage lcov -o coverage/lcov.info" },
     { cmd = "coverage report" },
 ]
-
-[tool.poe.tasks.check-lock]
-shell = "poetry lock --check | grep -v 'not consistent'"
-help = "poetry lock workaround for https://github.com/nat-n/poethepoet/issues/91"
```

### Comparing `poetry-bumpversion-0.3.0/src/poetry_bumpversion/models.py` & `poetry_bumpversion-0.3.1/src/poetry_bumpversion/models.py`

 * *Files identical despite different names*

### Comparing `poetry-bumpversion-0.3.0/src/poetry_bumpversion/plugin.py` & `poetry_bumpversion-0.3.1/src/poetry_bumpversion/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Plugins provided by the package."""
 
 from pathlib import Path
 from typing import Iterator, cast
 
 from cleo.events.console_events import TERMINATE
 from cleo.events.console_terminate_event import ConsoleTerminateEvent
+from cleo.events.event import Event
 from cleo.events.event_dispatcher import EventDispatcher
 from poetry.console.application import Application
 from poetry.console.commands.version import VersionCommand
 from poetry.core.pyproject.toml import PyProjectTOML
 from poetry.plugins.application_plugin import ApplicationPlugin
 from pydantic import ValidationError
 
@@ -37,23 +38,24 @@
         Args:
             application (Application): The poetry application hook/argument.
         """
         if application.event_dispatcher:
             application.event_dispatcher.add_listener(TERMINATE, self.on_terminate)
 
     def on_terminate(
-        self, event: ConsoleTerminateEvent, event_name: str, dispatcher: EventDispatcher
+        self, event: Event, event_name: str, dispatcher: EventDispatcher
     ) -> None:
         """Plugin on terminate hook/function.
 
         Args:
             event: Console event hook.
             event_name (str): Event name.
             dispatcher (EventDispatcher): Event dispatcher.
         """
+        assert isinstance(event, ConsoleTerminateEvent)
         try:
             command = event.command
             if command.name == "version" and command.argument("version"):
                 handle_version_update(cast(VersionCommand, command))
         except (PluginException, ValidationError) as exc:
             command.line(_(str(exc)), "warning")
         except Exception:  # pragma: no cover
```

### Comparing `poetry-bumpversion-0.3.0/PKG-INFO` & `poetry_bumpversion-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: poetry-bumpversion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Poetry plugin to update __version__ in __init__ file and other files containing version strings
 Home-page: https://github.com/monim67/poetry-bumpversion
 License: MIT
 Keywords: poetry,bump,version,plugin
 Author: Munim Munna
 Author-email: 6266677+monim67@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: poetry (>=1.2.0a2,<2.0.0)
-Requires-Dist: pydantic
+Requires-Dist: pydantic (<2)
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/monim67/poetry-bumpversion
 Description-Content-Type: text/x-rst
 
 ####################
 poetry-bumpversion
 ####################
@@ -105,14 +106,23 @@
     replace = '__version__ = "{new_version}"'
 
     [[tool.poetry_bumpversion.replacements]]
     files = ["README.md"]
     search = 'version: {current_version}'
     replace = 'version: {new_version}'
 
+******************************
+Usage with Github Workflow
+******************************
+
+This plugin uses itself in it's "Deploy to PyPI" workflow. When a release tag is created on
+GitHub, the workflow updates package version using the release tag name and deploys it to PyPI.
+You can copy the `deploy workflow code`_ to your repository to set it up.
+
+.. _deploy workflow code: https://github.com/monim67/poetry-bumpversion/blob/master/.github/workflows/deploy.yml
 
 ********************
 License
 ********************
 
 This project is licensed under MIT License - see the
 `LICENSE <https://github.com/monim67/poetry-bumpversion/blob/master/LICENSE>`_ file for details.
```

