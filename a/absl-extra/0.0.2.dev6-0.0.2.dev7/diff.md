# Comparing `tmp/absl_extra-0.0.2.dev6.tar.gz` & `tmp/absl_extra-0.0.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.2.dev7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.2.dev6.tar` & `absl_extra-0.0.2.dev7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1588 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/Readme.md
--rw-r--r--   0        0        0      646 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/__init__.py
--rw-r--r--   0        0        0       64 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/py.typed
--rw-r--r--   0        0        0        0 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/__init__.py
--rw-r--r--   0        0        0     1202 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/jax_utils.py
--rw-r--r--   0        0        0     2061 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/notifier.py
--rw-r--r--   0        0        0     4281 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/tasks.py
--rw-r--r--   0        0        0     4522 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/tf_utils.py
--rw-r--r--   0        0        0      914 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/Readme.md
+-rw-r--r--   0        0        0      682 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/py.typed
+-rw-r--r--   0        0        0        0 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/__init__.py
+-rw-r--r--   0        0        0     1202 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/jax_utils.py
+-rw-r--r--   0        0        0     2452 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/notifier.py
+-rw-r--r--   0        0        0     4281 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/tasks.py
+-rw-r--r--   0        0        0     4522 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/absl_extra/src/tf_utils.py
+-rw-r--r--   0        0        0      914 2023-07-02 11:46:35.709229 absl_extra-0.0.2.dev7/pyproject.toml
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev7/PKG-INFO
```

### Comparing `absl_extra-0.0.2.dev6/Readme.md` & `absl_extra-0.0.2.dev7/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev6/absl_extra/__init__.py` & `absl_extra-0.0.2.dev7/absl_extra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 
 from absl_extra.src.tasks import run, register_task
 from absl_extra.src.notifier import BaseNotifier
 
 if is_lib_installed("slack_sdk"):
     from absl_extra.src.notifier import SlackNotifier
-from absl_extra.src.logging_utils import log_before, log_after, setup_logging
+from absl_extra.src.logging_utils import (
+    log_before,
+    log_after,
+    setup_logging,
+    log_exception,
+)
 
 if is_lib_installed("pymongo"):
     from absl_extra.src.tasks import MongoConfig
 if is_lib_installed("tensorflow"):
     from absl_extra.src import tf_utils
 
 if is_lib_installed("jax"):
```

### Comparing `absl_extra-0.0.2.dev6/absl_extra/src/jax_utils.py` & `absl_extra-0.0.2.dev7/absl_extra/src/jax_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev6/absl_extra/src/logging_utils.py` & `absl_extra-0.0.2.dev7/absl_extra/src/logging_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 from __future__ import annotations
 
 import functools
 import inspect
 from importlib import util
-from typing import Callable, TypeVar, Literal
+from typing import Callable, TypeVar, Literal, ParamSpecArgs, ParamSpecKwargs
 
 from absl import logging
 
+A = ParamSpecArgs("A")
+K = ParamSpecKwargs("K")
 R = TypeVar("R")
 LogLevel = Literal["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"]
+Func = Callable[[A, K], R]
+Logger = Callable[[str], None]
 
 
-def log_before(
-    func: Callable[[...], R], logger: Callable[[str], None] = logging.debug
-) -> Callable[[...], R]:
-    """
-
-    Parameters
-    ----------
-    func
-    logger
+def log_exception(func: Func, logger: Logger = logging.error) -> Func:
+    """Log raised exception, and argument which caused it."""
+
+    @functools.wraps(func)
+    def wrapper(*args: A, **kwargs: K) -> R:
+        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
+        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
+
+        try:
+            return func(*args, **kwargs)
+        except Exception as ex:
+            logger(
+                f"{func.__module__}.{func.__qualname__} with args ( {func_args_str} ) raised {ex}"
+            )
+            raise ex
+
+    return wrapper
 
-    Returns
-    -------
 
-    """
+def log_before(func: Func, logger: Logger = logging.debug) -> Func:
+    """Log argument and function name."""
 
     @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> R:
+    def wrapper(*args: A, **kwargs: K) -> R:
         func_args = inspect.signature(func).bind(*args, **kwargs).arguments
         func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
         logger(
             f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
         )
         return func(*args, **kwargs)
 
     return wrapper
 
 
-def log_after(
-    func: Callable[[...], R], logger: Callable[[str], None] = logging.debug
-) -> Callable[[...], R]:
-    """
-    Log's function's return value.
-
-    Parameters
-    ----------
-    func:
-        Function exit from which must be logged.
-    logger:
-        Logger to use, default absl.logging.debug
-
-    Returns
-    -------
-
-    func:
-        Function with the same signature.
-
-    """
+def log_after(func: Func, logger: Logger = logging.debug) -> Func:
+    """Log's function's return value."""
 
     @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> R:
+    def wrapper(*args: A, **kwargs: K) -> R:
         retval = func(*args, **kwargs)
         logger(
             f"Exited {func.__module__}.{func.__qualname__}(...) with value: "
             + repr(retval)
         )
         return retval
```

### Comparing `absl_extra-0.0.2.dev6/absl_extra/src/notifier.py` & `absl_extra-0.0.2.dev7/absl_extra/src/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev6/absl_extra/src/tasks.py` & `absl_extra-0.0.2.dev7/absl_extra/src/tasks.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev6/absl_extra/src/tf_utils.py` & `absl_extra-0.0.2.dev7/absl_extra/src/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev6/pyproject.toml` & `absl_extra-0.0.2.dev7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.2dev6"
+version = "0.0.2dev7"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.2.dev6/PKG-INFO` & `absl_extra-0.0.2.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2.dev6
+Version: 0.0.2.dev7
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

