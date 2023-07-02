# Comparing `tmp/libdnf5_shim-0.0.1.tar.gz` & `tmp/libdnf5_shim-0.1.0.tar.gz`

## Comparing `libdnf5_shim-0.0.1.tar` & `libdnf5_shim-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/NEWS.md
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/noxfile.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/ruff.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/.builds/f38.yml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/.builds/main.yml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/src/_libdnf5_shim/__init__.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/src/_libdnf5_shim/_impl.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/src/_libdnf5_shim/initialize.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/src/libdnf5/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/tests/test_libdnf5_shim.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/.gitignore
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/README.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 libdnf5_shim-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/NEWS.md
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/noxfile.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/ruff.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/.builds/f38.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/.builds/main.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/libdnf5.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/libdnf5_cli.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/_libdnf5_shim/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/_libdnf5_shim/_impl.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/_libdnf5_shim/initialize.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/src/_libdnf5_shim/initialize_cli.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/tests/test_libdnf5_shim.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/.gitignore
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/README.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 libdnf5_shim-0.1.0/PKG-INFO
```

### Comparing `libdnf5_shim-0.0.1/CONTRIBUTING.md` & `libdnf5_shim-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libdnf5_shim-0.0.1/noxfile.py` & `libdnf5_shim-0.1.0/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 ALLOW_EDITABLE = os.environ.get("ALLOW_EDITABLE", str(not IN_CI)).lower() in (
     "1",
     "true",
 )
 
 PROJECT = "libdnf5_shim"
 LINT_SESSIONS = ("formatters", "codeqa", "typing")
-LINT_FILES = ("src/_libdnf5_shim", "src/libdnf5/", "tests/", "noxfile.py")
+LINT_FILES = (
+    "src/_libdnf5_shim",
+    "src/libdnf5.py",
+    "src/libdnf5_cli.py",
+    "tests/",
+    "noxfile.py",
+)
 RELEASERR = "releaserr[all] @ git+https://git.sr.ht/~gotmax23/releaserr"
 # RELEASERR = "-e../releaserr[all]"
 
 nox.options.sessions = (*LINT_SESSIONS, "test")
 
 
 # Helpers
@@ -35,15 +41,15 @@
 def git(session: nox.Session, *args, **kwargs):
     return session.run("git", *args, **kwargs, external=True)
 
 
 # General
 
 
-@nox.session
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"])
 def test(session: nox.Session):
     install(session, ".[test]", editable=True)
     session.run("pytest", "--forked", *session.posargs)
 
 
 @nox.session(venv_backend="none")
 def lint(session: nox.Session):
```

### Comparing `libdnf5_shim-0.0.1/ruff.toml` & `libdnf5_shim-0.1.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `libdnf5_shim-0.0.1/src/_libdnf5_shim/_impl.py` & `libdnf5_shim-0.1.0/src/_libdnf5_shim/_impl.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,23 +17,22 @@
 import logging
 import subprocess
 import sys
 from collections.abc import Iterator
 from pathlib import Path
 
 PROJECT_NAME = "libdnf5-shim"
-MODULE_NAME = "libdnf5"
 
 INTERPRETERS: tuple[str, ...] = (
     "/usr/libexec/platform-python",
     f"/usr/bin/python{sys.version_info.major}",
     f"/usr/bin/python{sys.version_info.major}.{sys.version_info.minor}",
 )
 FAILURE_MSG = (
-    "Failed to import system libdnf5 module. "
+    "Failed to import system {} module. "
     "Make sure libdnf5 Python bindings installed on your system."
 )
 
 LOG = logging.getLogger(PROJECT_NAME)
 
 
 def query_interp_sitepackages(interpreter) -> list[str]:
@@ -58,38 +57,38 @@
         if not Path(interpreter).is_file():
             continue
         sitepackages = query_interp_sitepackages(interpreter)
         LOG.debug("Collected sitepackages for %s:\n%s", interpreter, sitepackages)
         yield from sitepackages
 
 
-def try_path(path: str) -> bool:
+def try_path(path: str, module_name: str) -> bool:
     """
     Tries to load system libdnf5 module from the specified path.
 
     Returns:
         True if successful, False otherwise.
     """
-    if not (Path(path) / MODULE_NAME).is_dir():
+    if not (Path(path) / module_name).is_dir():
         return False
     sys.path.insert(0, path)
     try:
-        importlib.reload(sys.modules[MODULE_NAME])
+        importlib.reload(sys.modules[module_name])
     except Exception as exc:  # pragma: no cover
         LOG.debug("Exception:", exc_info=exc)
         return False
     else:
         return True
     finally:
         del sys.path[0]
 
 
-def initialize() -> None:
+def initialize(module_name: str) -> None:
     """
     Initializes the shim. Tries to load system libdnf5 module.
     """
     for path in get_system_sitepackages():
         LOG.debug(f"Trying {path}")
-        if try_path(path):
+        if try_path(path, module_name):
             LOG.debug("Import successful")
             return
-    raise ImportError(FAILURE_MSG)
+    raise ImportError(FAILURE_MSG.format(module_name))
```

### Comparing `libdnf5_shim-0.0.1/tests/test_libdnf5_shim.py` & `libdnf5_shim-0.1.0/tests/test_libdnf5_shim.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,113 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import importlib
 import sys
+from collections.abc import Callable
 from types import ModuleType
 
 import pytest
 from pytest_mock import MockerFixture
 
 
 def basic(mod: ModuleType):
     assert mod.__name__ == "libdnf5"
     base = mod.base.Base()
     base.load_config_from_file()
     base.get_config()
     base.setup()
 
 
-def test_libdnf5_import(mocker: MockerFixture):
+def basic_libdnf5_cli(mod: ModuleType):
+    assert mod.__name__ == "libdnf5_cli"
+    mod.progressbar.DownloadProgressBar(500, "abcdefgh")
+
+
+PARAM = pytest.mark.parametrize(
+    "module_name,checker,init",
+    [
+        pytest.param("libdnf5", basic, "_libdnf5_shim.initialize", id="libdnf5"),
+        pytest.param(
+            "libdnf5_cli",
+            basic_libdnf5_cli,
+            "_libdnf5_shim.initialize_cli",
+            id="libdnf5_cli",
+        ),
+    ],
+)
+
+
+@PARAM
+def test_libdnf5_import(
+    mocker: MockerFixture,
+    module_name: str,
+    checker: Callable[[ModuleType], None],
+    init: str,
+):
     import _libdnf5_shim._impl
 
     initializes = mocker.spy(_libdnf5_shim._impl, "initialize")
 
     # Import libdnf5 for the first time
-    import libdnf5
+    mod = importlib.import_module(module_name)
 
     # Check that the shim was used
     initializes.assert_called_once()
-    assert "libdnf5" in sys.modules
-    assert "_libdnf5_shim.initialize" in sys.modules
+    assert module_name in sys.modules
+    assert init in sys.modules
 
     # Run basic tests to make sure the imported libdnf5 works
-    basic(libdnf5)
+    checker(mod)
 
     # Import again
-    import libdnf5
+    mod = importlib.import_module(module_name)
 
-    basic(libdnf5)
+    checker(mod)
 
     # Ensure that initialize was only called once
     initializes.assert_called_once()
 
 
-def test_libdnf5_import_fail(mocker: MockerFixture):
+@PARAM
+def test_libdnf5_import_fail(
+    mocker: MockerFixture,
+    module_name: str,
+    checker: Callable[[ModuleType], None],
+    init: str,
+):
     import _libdnf5_shim._impl
 
     initializes = mocker.spy(_libdnf5_shim._impl, "initialize")
 
     # Set the INTERPRETERS to an empty tuple to cause a failure
     inters = _libdnf5_shim._impl.INTERPRETERS
     _libdnf5_shim._impl.INTERPRETERS = ()
 
     # Check failure
     try:
-        with pytest.raises(ImportError, match=_libdnf5_shim._impl.FAILURE_MSG):
-            import libdnf5
+        with pytest.raises(
+            ImportError, match=_libdnf5_shim._impl.FAILURE_MSG.format(module_name)
+        ):
+            importlib.import_module(module_name)
     finally:
         _libdnf5_shim._impl.INTERPRETERS = inters
 
     # Check that shim was used
     initializes.assert_called_once()
 
     # Try to import libdnf5
-    import libdnf5  # noqa: F811
+    mod = importlib.import_module(module_name)  # noqa: F811
 
     # Check that it works now
-    basic(libdnf5)
+    checker(mod)
     assert initializes.call_count == 2
+
+
+def test_both_import():
+    import libdnf5
+    import libdnf5_cli
+
+    basic(libdnf5)
+    basic_libdnf5_cli(libdnf5_cli)
```

### Comparing `libdnf5_shim-0.0.1/README.md` & `libdnf5_shim-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `libdnf5_shim-0.0.1/pyproject.toml` & `libdnf5_shim-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -48,31 +48,37 @@
 ]
 test = [
     "pytest",
     "pytest-mock",
     "pytest-forked",
 ]
 dev = [
+    "libdnf5-shim[codeqa]",
     "libdnf5-shim[formatters]",
     "libdnf5-shim[test]",
     "libdnf5-shim[typing]",
     "nox",
 ]
 
 [project.urls]
+Homepage = "https://sr.ht/~gotmax23/libdnf5-shim"
 Source = "https://git.sr.ht/~gotmax23/libdnf5-shim"
 "Mailing List" = "https://lists.sr.ht/~gotmax23/libdnf5-shim"
 Changelog = "https://git.sr.ht/~gotmax23/libdnf5-shim/tree/main/item/NEWS.md"
 
 
 [tool.hatch.version]
 path = "src/_libdnf5_shim/__init__.py"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/libdnf5", "src/_libdnf5_shim"]
+packages = [
+    "src/libdnf5.py",
+    "src/libdnf5_cli.py",
+    "src/_libdnf5_shim"
+]
 
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `libdnf5_shim-0.0.1/LICENSES/MIT.txt` & `libdnf5_shim-0.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `libdnf5_shim-0.0.1/PKG-INFO` & `libdnf5_shim-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: libdnf5-shim
-Version: 0.0.1
+Version: 0.1.0
 Summary: libdnf5 shim module for usage in virtualenvs
+Project-URL: Homepage, https://sr.ht/~gotmax23/libdnf5-shim
 Project-URL: Source, https://git.sr.ht/~gotmax23/libdnf5-shim
 Project-URL: Mailing List, https://lists.sr.ht/~gotmax23/libdnf5-shim
 Project-URL: Changelog, https://git.sr.ht/~gotmax23/libdnf5-shim/tree/main/item/NEWS.md
 Author-email: Maxwell G <maxwell@gtmx.me>
 License-Expression: MIT
 License-File: LICENSES/MIT.txt
 Classifier: Development Status :: 3 - Alpha
@@ -19,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Provides-Extra: codeqa
 Requires-Dist: reuse; extra == 'codeqa'
 Requires-Dist: ruff; extra == 'codeqa'
 Provides-Extra: dev
+Requires-Dist: libdnf5-shim[codeqa]; extra == 'dev'
 Requires-Dist: libdnf5-shim[formatters]; extra == 'dev'
 Requires-Dist: libdnf5-shim[test]; extra == 'dev'
 Requires-Dist: libdnf5-shim[typing]; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Provides-Extra: formatters
 Requires-Dist: black; extra == 'formatters'
 Requires-Dist: isort; extra == 'formatters'
```

