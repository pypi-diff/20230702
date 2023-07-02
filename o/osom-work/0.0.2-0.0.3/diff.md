# Comparing `tmp/osom_work-0.0.2-py3-none-any.whl.zip` & `tmp/osom_work-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 8180 bytes, number of entries: 16
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-01 04:36 osom_work/__init__.py
--rw-r--r--  2.0 unx      146 b- defN 23-Jul-01 04:36 osom_work/__main__.py
--rw-r--r--  2.0 unx     3997 b- defN 23-Jul-01 04:36 osom_work/arguments.py
--rw-r--r--  2.0 unx     2162 b- defN 23-Jul-01 04:36 osom_work/entrypoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 04:36 osom_work/apps/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 04:36 osom_work/assets/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 04:36 osom_work/logging/__init__.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Jul-01 04:36 osom_work/logging/colored_formatter.py
--rw-r--r--  2.0 unx     6012 b- defN 23-Jul-01 04:36 osom_work/logging/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 04:36 osom_work/www/__init__.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1385 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1309 b- defN 23-Jul-01 04:37 osom_work-0.0.2.dist-info/RECORD
-16 files, 17381 bytes uncompressed, 5998 bytes compressed:  65.5%
+Zip file size: 8944 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-02 13:45 osom_work/__init__.py
+-rw-r--r--  2.0 unx      146 b- defN 23-Jul-02 13:45 osom_work/__main__.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jul-02 13:45 osom_work/arguments.py
+-rw-r--r--  2.0 unx     1885 b- defN 23-Jul-02 13:45 osom_work/entrypoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 13:45 osom_work/apps/__init__.py
+-rw-r--r--  2.0 unx      493 b- defN 23-Jul-02 13:45 osom_work/apps/master/__init__.py
+-rw-r--r--  2.0 unx      272 b- defN 23-Jul-02 13:45 osom_work/apps/worker/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 13:45 osom_work/assets/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 13:45 osom_work/logging/__init__.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Jul-02 13:45 osom_work/logging/colored_formatter.py
+-rw-r--r--  2.0 unx     6012 b- defN 23-Jul-02 13:45 osom_work/logging/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 13:45 osom_work/www/__init__.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1424 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1487 b- defN 23-Jul-02 13:45 osom_work-0.0.3.dist-info/RECORD
+18 files, 18341 bytes uncompressed, 6478 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -9,14 +9,20 @@
 
 Filename: osom_work/entrypoint.py
 Comment: 
 
 Filename: osom_work/apps/__init__.py
 Comment: 
 
+Filename: osom_work/apps/master/__init__.py
+Comment: 
+
+Filename: osom_work/apps/worker/__init__.py
+Comment: 
+
 Filename: osom_work/assets/__init__.py
 Comment: 
 
 Filename: osom_work/logging/__init__.py
 Comment: 
 
 Filename: osom_work/logging/colored_formatter.py
@@ -24,26 +30,26 @@
 
 Filename: osom_work/logging/logging.py
 Comment: 
 
 Filename: osom_work/www/__init__.py
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/LICENSE
+Filename: osom_work-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/METADATA
+Filename: osom_work-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/WHEEL
+Filename: osom_work-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/entry_points.txt
+Filename: osom_work-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/top_level.txt
+Filename: osom_work-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: osom_work-0.0.2.dist-info/RECORD
+Filename: osom_work-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osom_work/__init__.py

```diff
@@ -1,3 +1,3 @@
 # -*- coding: utf-8 -*-
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## osom_work/arguments.py

```diff
@@ -1,55 +1,53 @@
 # -*- coding: utf-8 -*-
 
-from argparse import REMAINDER, ArgumentParser, Namespace, RawDescriptionHelpFormatter
+from argparse import ArgumentParser, Namespace, RawDescriptionHelpFormatter
 from functools import lru_cache
 from typing import Final, List, Optional
 
 from osom_work.logging.logging import SEVERITIES, SEVERITY_NAME_INFO
 
-CMD_CLIENT: Final[str] = "client"
-CMD_MODULES: Final[str] = "modules"
-CMD_SERVER: Final[str] = "server"
+CMD_MASTER: Final[str] = "master"
+CMD_WORKER: Final[str] = "worker"
 
-PROG: Final[str] = "osom_work"
-DESCRIPTION: Final[str] = "osom work"
+PROG: Final[str] = "osom-work"
+DESCRIPTION: Final[str] = "osom master and worker"
 EPILOG: Final[str] = ""
 
 DEFAULT_SEVERITY: Final[str] = SEVERITY_NAME_INFO
 
-CMD1 = "cmd1"
-CMD2 = "cmd2"
-CMDS = (CMD1, CMD2)
+CMDS = (CMD_MASTER, CMD_WORKER)
 
-CMD1_HELP: Final[str] = ""
-CMD1_EPILOG: Final[str] = ""
+CMD_MASTER_HELP: Final[str] = "Master node"
+CMD_MASTER_EPILOG: Final[str] = ""
 
-CMD2_HELP: Final[str] = ""
-CMD2_EPILOG: Final[str] = ""
+CMD_WORKER_HELP: Final[str] = "Worker node"
+CMD_WORKER_EPILOG: Final[str] = ""
 
 DEFAULT_BIND: Final[str] = "0.0.0.0"
 DEFAULT_PORT: Final[int] = 8080
-DEFAULT_TIMEOUT: Final[float] = 1.0
+DEFAULT_TIMEOUT: Final[float] = 8.0
+DEFAULT_BROKER: Final[str] = ""
 
 
 @lru_cache
 def version() -> str:
     # [IMPORTANT] Avoid 'circular import' issues
     from osom_work import __version__
 
     return __version__
 
 
-def add_cmd1_parser(subparsers) -> None:
+def add_cmd_master_parser(subparsers) -> None:
     # noinspection SpellCheckingInspection
     parser = subparsers.add_parser(
-        name=CMD1,
-        help=CMD1_HELP,
+        name=CMD_MASTER,
+        help=CMD_MASTER_HELP,
         formatter_class=RawDescriptionHelpFormatter,
-        epilog=CMD1_EPILOG,
+        epilog=CMD_MASTER_EPILOG,
     )
     assert isinstance(parser, ArgumentParser)
 
     parser.add_argument(
         "--bind",
         "-b",
         default=DEFAULT_BIND,
@@ -57,52 +55,55 @@
         help=f"Bind address (default: '{DEFAULT_BIND}')",
     )
     parser.add_argument(
         "--port",
         "-p",
         default=DEFAULT_PORT,
         metavar="port",
-        help=f"Port number (default: '{DEFAULT_PORT}')",
+        type=int,
+        help=f"Port number (default: {DEFAULT_PORT})",
     )
     parser.add_argument(
         "--timeout",
         "-t",
         default=DEFAULT_TIMEOUT,
+        metavar="sec",
         type=float,
         help=f"Request timeout in seconds (default: {DEFAULT_TIMEOUT})",
     )
+    parser.add_argument(
+        "--broker",
+        "-B",
+        default=DEFAULT_BROKER,
+        metavar="bind",
+        type=str,
+        help=f"URL of the default broker used (default: '{DEFAULT_BROKER}')",
+    )
 
 
-def add_cmd2_parser(subparsers) -> None:
+def add_cmd_worker_parser(subparsers) -> None:
     # noinspection SpellCheckingInspection
     parser = subparsers.add_parser(
-        name=CMD2,
-        help=CMD2_HELP,
+        name=CMD_WORKER,
+        help=CMD_WORKER_HELP,
         formatter_class=RawDescriptionHelpFormatter,
-        epilog=CMD2_EPILOG,
+        epilog=CMD_WORKER_EPILOG,
     )
     assert isinstance(parser, ArgumentParser)
 
     parser.add_argument(
-        "--config",
-        "-c",
-        default=None,
-        metavar="file",
-        help="Configuration file path",
-    )
-    parser.add_argument(
-        "module",
-        default=None,
-        nargs="?",
-        help="Module name",
+        "--timeout",
+        "-t",
+        default=DEFAULT_TIMEOUT,
+        type=float,
+        help=f"Request timeout in seconds (default: {DEFAULT_TIMEOUT})",
     )
     parser.add_argument(
-        "opts",
-        nargs=REMAINDER,
-        help="Arguments of module",
+        "broker",
+        help="URL of the default broker used",
     )
 
 
 def default_argument_parser() -> ArgumentParser:
     parser = ArgumentParser(
         prog=PROG,
         description=DESCRIPTION,
@@ -147,16 +148,16 @@
         "--version",
         "-V",
         action="version",
         version=version(),
     )
 
     subparsers = parser.add_subparsers(dest="cmd")
-    add_cmd1_parser(subparsers)
-    add_cmd2_parser(subparsers)
+    add_cmd_master_parser(subparsers)
+    add_cmd_worker_parser(subparsers)
     return parser
 
 
 def get_default_arguments(
     cmdline: Optional[List[str]] = None,
     namespace: Optional[Namespace] = None,
 ) -> Namespace:
```

## osom_work/entrypoint.py

```diff
@@ -1,49 +1,36 @@
 # -*- coding: utf-8 -*-
 
-from argparse import Namespace
 from sys import exit as sys_exit
 from typing import Callable, List, Optional
 
-from osom_work.arguments import CMD1, CMD2, CMDS, get_default_arguments
+from osom_work.apps.master import master_main
+from osom_work.apps.worker import worker_main
+from osom_work.arguments import CMD_MASTER, CMD_WORKER, CMDS, get_default_arguments
 from osom_work.logging.logging import (
     SEVERITY_NAME_DEBUG,
     logger,
     set_colored_formatter_logging_config,
     set_root_level,
     set_simple_logging_config,
 )
 
 
-def cmd1_main(args: Namespace, printer: Callable[..., None] = print) -> int:
-    assert args is not None
-    assert printer is not None
-    raise NotImplementedError
-
-
-def cmd2_main(args: Namespace, printer: Callable[..., None] = print) -> int:
-    assert args is not None
-    assert printer is not None
-    raise NotImplementedError
-
-
 def main(
     cmdline: Optional[List[str]] = None,
     printer: Callable[..., None] = print,
 ) -> int:
     args = get_default_arguments(cmdline)
 
     if not args.cmd:
         printer("The command does not exist")
         return 1
 
     if args.colored_logging and args.simple_logging:
-        printer(
-            "The 'colored_logging' flag and the 'simple_logging' flag cannot coexist"
-        )
+        printer("The 'colored_logging' and 'simple_logging' flags cannot coexist")
         return 1
 
     cmd = args.cmd
     colored_logging = args.colored_logging
     simple_logging = args.simple_logging
     severity = args.severity
     debug = args.debug
@@ -65,18 +52,18 @@
         set_root_level(SEVERITY_NAME_DEBUG)
     else:
         set_root_level(severity)
 
     logger.debug(f"Arguments: {args}")
 
     try:
-        if cmd == CMD1:
-            return cmd1_main(args, printer=printer)
-        elif cmd == CMD2:
-            return cmd2_main(args, printer=printer)
+        if cmd == CMD_MASTER:
+            return master_main(args, printer=printer)
+        elif cmd == CMD_WORKER:
+            return worker_main(args, printer=printer)
         else:
             assert False, "Inaccessible section"
     except BaseException as e:
         logger.exception(e)
         return 1
```

## Comparing `osom_work-0.0.2.dist-info/LICENSE` & `osom_work-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `osom_work-0.0.2.dist-info/METADATA` & `osom_work-0.0.3.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osom-work
-Version: 0.0.2
+Version: 0.0.3
 Summary: osom work
 Home-page: https://github.com/osom8979/osom-work
 Author: zer0
 Author-email: osom8979@gmail.com
 Maintainer: zer0
 Maintainer-email: osom8979@gmail.com
 License: MIT License
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs (>=15.0.1)
+Requires-Dist: fastapi[all] (>=0.99.0)
 
 # osom-work
 
 [![PyPI](https://img.shields.io/pypi/v/osom-work?style=flat-square)](https://pypi.org/project/osom-work/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osom-work?style=flat-square)
 [![GitHub](https://img.shields.io/github/license/osom8979/osom-work?style=flat-square)](https://github.com/osom8979/osom-work/)
```

## Comparing `osom_work-0.0.2.dist-info/RECORD` & `osom_work-0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-osom_work/__init__.py,sha256=AcHlMkGjAHXFw4aah0ZmqXNVPdqillZU3OH57EZWy78,47
+osom_work/__init__.py,sha256=zKwGQzXtKN6rpO1aKe0KDHjxNV2-lrMe8SG6P0Nk0SE,47
 osom_work/__main__.py,sha256=S8iAitJkJRMnnSxcGUL2qBFzC_L0tzEJk7Smkquk8Bg,146
-osom_work/arguments.py,sha256=wfXJBBtF5-c6fRt3ihDmrRa4OfVbC93_teJwmGyTrBU,3997
-osom_work/entrypoint.py,sha256=kHIdMu49AQQzAvhlj0fvN3P8ZX1aSQe4MHovK6DQrM8,2162
+osom_work/arguments.py,sha256=hy0It9Vwi4Z4R7Hk0uQ1otOXKVJwxPRFAOVP3d-WBoQ,4252
+osom_work/entrypoint.py,sha256=D-rLJJ47dMpSJCCILNroYObMc7JpIh2JGk4ZJtV2m78,1885
 osom_work/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+osom_work/apps/master/__init__.py,sha256=ZI28Z-PtcAVj8Kl-3gEo-NLJuFQVkgWU756ypVBdxBQ,493
+osom_work/apps/worker/__init__.py,sha256=vOn2wLMfMTN8-TuWd8mkVFyDeOiLFFr6tUBil-w98iQ,272
 osom_work/assets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 osom_work/logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 osom_work/logging/colored_formatter.py,sha256=fAedRmXIM6ttJyI8263O9uggHf8__a1SoS1lNj3I20g,1099
 osom_work/logging/logging.py,sha256=PUaps4SkBu-fwLmI5NoZ9J0l_hU57IKx8jZ8tdjQxn8,6012
 osom_work/www/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-osom_work-0.0.2.dist-info/LICENSE,sha256=W6E4CImwrifHZNTPd3mERP-Ni9XDYgU6BFAxMyccl4c,1065
-osom_work-0.0.2.dist-info/METADATA,sha256=swGP4wsK8ETNbF5qvGxj3oKk8cAokzkvT00D6XXwZtw,1385
-osom_work-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-osom_work-0.0.2.dist-info/entry_points.txt,sha256=V6NskE6nFmV8y7C3djrb7sJHRXfufTZITNXo15xzASI,57
-osom_work-0.0.2.dist-info/top_level.txt,sha256=3myYcJRndpNx3IwmlyFQInBju7h5RHalbW3omF2SLXU,10
-osom_work-0.0.2.dist-info/RECORD,,
+osom_work-0.0.3.dist-info/LICENSE,sha256=W6E4CImwrifHZNTPd3mERP-Ni9XDYgU6BFAxMyccl4c,1065
+osom_work-0.0.3.dist-info/METADATA,sha256=TEy09_d-u-SmJxjIGYzNDa-ND2TNfKmmnWpj88FAM9I,1424
+osom_work-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+osom_work-0.0.3.dist-info/entry_points.txt,sha256=V6NskE6nFmV8y7C3djrb7sJHRXfufTZITNXo15xzASI,57
+osom_work-0.0.3.dist-info/top_level.txt,sha256=3myYcJRndpNx3IwmlyFQInBju7h5RHalbW3omF2SLXU,10
+osom_work-0.0.3.dist-info/RECORD,,
```

