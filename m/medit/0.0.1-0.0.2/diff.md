# Comparing `tmp/medit-0.0.1.tar.gz` & `tmp/medit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.1.tar", max compression
+gzip compressed data, was "medit-0.0.2.tar", max compression
```

## Comparing `medit-0.0.1.tar` & `medit-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      698 2023-06-16 08:02:50.686048 medit-0.0.1/Readme.md
--rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.1/medit/__init__.py
--rwxr-xr-x   0        0        0     2291 2023-06-16 07:50:49.465277 medit-0.0.1/medit/cli.py
--rw-r--r--   0        0        0     3293 2023-06-16 08:00:45.597915 medit-0.0.1/medit/meditor.py
--rw-r--r--   0        0        0     2389 2023-06-16 07:34:35.088205 medit-0.0.1/medit/misc.py
--rwxr-xr-x   0        0        0     3702 2023-06-16 08:00:59.101929 medit-0.0.1/medit/ui.py
--rwxr-xr-x   0        0        0     7256 2023-06-16 07:26:02.815585 medit-0.0.1/medit/yatl.py
--rw-r--r--   0        0        0     2087 2023-06-16 08:00:14.485882 medit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 medit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1837 2023-07-02 11:33:38.540816 medit-0.0.2/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.2/medit/__init__.py
+-rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.2/medit/cli.py
+-rw-r--r--   0        0        0     4619 2023-07-02 15:32:07.351200 medit-0.0.2/medit/meditor.py
+-rw-r--r--   0        0        0     7055 2023-07-02 14:04:10.012757 medit-0.0.2/medit/mview.py
+-rwxr-xr-x   0        0        0     6984 2023-07-02 15:29:24.360828 medit-0.0.2/medit/ui.py
+-rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.2/medit/utils.py
+-rw-r--r--   0        0        0     2232 2023-07-02 15:34:15.036636 medit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 medit-0.0.2/PKG-INFO
```

### Comparing `medit-0.0.1/medit/cli.py` & `medit-0.0.2/medit/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import sys
 from argparse import ArgumentParser
 from argparse import Namespace as Args
 from collections.abc import Sequence
 from contextlib import suppress
 from pathlib import Path
 
-from medit.misc import setup_logging
 from medit.ui import main as ui_main
+from medit.utils import setup_logging
 
 
 def parse_args(argv: Sequence[str] | None = None) -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser(__doc__)
     parser.add_argument("--verbose", "-v", action="store_true")
 
@@ -26,14 +26,15 @@
     subparsers = parser.add_subparsers(help="available commands", metavar="CMD")
 
     parser_help = subparsers.add_parser("help")
     parser_help.set_defaults(func=lambda *_: parser.print_help())
 
     parser_ui = subparsers.add_parser("ui")
     parser_ui.set_defaults(func=fn_ui)
+    parser_ui.add_argument("path", type=Path, nargs="?")
 
     return parser.parse_args(argv)
 
 
 def logger() -> logging.Logger:
     """Named logger"""
     return logging.getLogger("medit.cli")
@@ -68,16 +69,16 @@
     print(f"Version: {__version__} (at {shorten_home(Path(__file__).parent)})")
     print(
         f"Python: {'.'.join(map(str, sys.version_info[:3]))}"
         f" (at {shorten_home(sys.executable)})"
     )
 
 
-def fn_ui(_args: Args) -> None:
-    ui_main()
+def fn_ui(args: Args) -> None:
+    ui_main(args.path if hasattr(args, "path") else None)
 
 
 def main() -> int:
     """Entry point for everything else"""
     (args := parse_args()).func(args)
     return 0
```

### Comparing `medit-0.0.1/medit/misc.py` & `medit-0.0.2/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.1/pyproject.toml` & `medit-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.1"
+version = "0.0.2"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"}
 ]
 
 [tool.poetry.scripts]
 medit = 'medit.cli:main'
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 asyncinotify = "^4.0.1"
 toml = "^0.10.2"
 pyqt6 = "^6.5.1"
 pyqt6-qscintilla = "^2.14.0"
+pyqt6-webengine = "^6.5.0"
+markdown = "^3.4.3"
+markdown-checklist = "^0.4.4"
+# pygments-solarized-style = "^0.1"
+pyqtdarktheme = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

