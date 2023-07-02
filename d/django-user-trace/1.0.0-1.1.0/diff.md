# Comparing `tmp/django_user_trace-1.0.0.tar.gz` & `tmp/django_user_trace-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_user_trace-1.0.0.tar", max compression
+gzip compressed data, was "django_user_trace-1.1.0.tar", max compression
```

## Comparing `django_user_trace-1.0.0.tar` & `django_user_trace-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,37 @@
--rw-r--r--   0        0        0     3303 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/README.md
--rw-r--r--   0        0        0     2280 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/__init__.py
--rw-r--r--   0        0        0      382 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/apps.py
--rw-r--r--   0        0        0     2749 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/conf.py
--rw-r--r--   0        0        0      527 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/context.py
--rw-r--r--   0        0        0     1250 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/log.py
--rw-r--r--   0        0        0     2742 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/middleware.py
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/py.typed
--rw-r--r--   0        0        0      658 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/signals.py
--rw-r--r--   0        0        0     2220 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/src/django_user_trace/utils.py
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/feature/__init__.py
--rw-r--r--   0        0        0     4088 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/feature/test_async_request.py
--rw-r--r--   0        0        0     4625 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/feature/test_conf.py
--rw-r--r--   0        0        0     3233 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/feature/test_sync_request.py
--rw-r--r--   0        0        0        0 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     3799 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/unit/test_conf.py
--rw-r--r--   0        0        0      393 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/unit/test_context.py
--rw-r--r--   0        0        0     1141 2023-03-28 01:34:08.376159 django_user_trace-1.0.0/tests/unit/test_middleware.py
--rw-r--r--   0        0        0     3255 2023-03-28 01:34:08.380159 django_user_trace-1.0.0/tests/unit/test_utils.py
--rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 django_user_trace-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3387 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/README.md
+-rw-r--r--   0        0        0     2712 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/__init__.py
+-rw-r--r--   0        0        0      384 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/apps.py
+-rw-r--r--   0        0        0     2871 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/conf.py
+-rw-r--r--   0        0        0      527 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/context.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/contrib/celery/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/contrib/celery/apps.py
+-rw-r--r--   0        0        0     1584 2023-07-02 12:10:54.483934 django_user_trace-1.1.0/src/django_user_trace/contrib/celery/signals.py
+-rw-r--r--   0        0        0     1250 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/src/django_user_trace/log.py
+-rw-r--r--   0        0        0     3328 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/src/django_user_trace/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/src/django_user_trace/py.typed
+-rw-r--r--   0        0        0      990 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/src/django_user_trace/signals.py
+-rw-r--r--   0        0        0     2220 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/src/django_user_trace/utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/contrib/celery/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/contrib/celery/conftest.py
+-rw-r--r--   0        0        0     2258 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/contrib/celery/test_conf.py
+-rw-r--r--   0        0        0     4808 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/contrib/celery/test_task.py
+-rw-r--r--   0        0        0     4099 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/test_async_request.py
+-rw-r--r--   0        0        0     4625 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/test_conf.py
+-rw-r--r--   0        0        0     3233 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/feature/test_sync_request.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/contrib/celery/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/contrib/celery/conftest.py
+-rw-r--r--   0        0        0     2117 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/contrib/celery/test_signals.py
+-rw-r--r--   0        0        0     3799 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/test_conf.py
+-rw-r--r--   0        0        0      393 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/test_context.py
+-rw-r--r--   0        0        0     1141 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/test_middleware.py
+-rw-r--r--   0        0        0     1048 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/test_signals.py
+-rw-r--r--   0        0        0     3255 2023-07-02 12:10:54.487934 django_user_trace-1.1.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 django_user_trace-1.1.0/PKG-INFO
```

### Comparing `django_user_trace-1.0.0/README.md` & `django_user_trace-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     django_user_trace -->> logging: `ContextVar` for user attrs
     django ->>+ django_user_trace: signal `request_finished`
     note over django, django_user_trace: Clear user attributes from the `ContextVar`
     django_user_trace ->>+ django: continue
     django -->> User: send response
 ```
 
+#### Supports
+
+* [Celery task logging][celery]
+
 #### Resources
 
 * [Django &mdash; How to configure and use logging][django:logging]
 
 #### Related Projects
 
 * [madzak/python-json-logger][python-json-logger]
@@ -72,14 +76,15 @@
 vulnerabilities.
 
 ## Licence
 
 `django-user-trace` is open-sourced software licenced under the
 [MIT licence][licence].
 
+[celery]: https://docs.celeryq.dev/
 [ci:release]: https://github.com/axieum/django-user-trace/actions/workflows/release.yml
 [ci:test]: https://github.com/axieum/django-user-trace/actions/workflows/test.yml
 [codecov]: https://app.codecov.io/gh/axieum/django-user-trace
 [contributing]: CONTRIBUTING.md
 [django]: https://djangoproject.com/
 [django:logging]: https://docs.djangoproject.com/en/stable/howto/logging/
 [django-guid]: https://github.com/snok/django-guid
```

### Comparing `django_user_trace-1.0.0/pyproject.toml` & `django_user_trace-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 [tool.poetry]
 name = "django-user-trace"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Python logging filter for Django user attributes."
 license = "MIT"
 authors = ["Jonathan Hiles <jonathan@hil.es>"]
 readme = "README.md"
 repository = "https://github.com/axieum/django-user-trace"
 documentation = "https://axieum.github.io/django-user-trace/latest/"
 keywords = ["async", "django", "logs", "logging", "middleware", "sync", "trace", "tracing", "user", "web"]
 classifiers = [
+  "Framework :: Django",
+  "Framework :: Django :: 3",
+  "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4",
+  "Framework :: Django :: 4.0",
+  "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 packages = [{ include = "django_user_trace", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
@@ -21,23 +28,29 @@
 "Funding" = "https://github.com/sponsors/axieum"
 "Issue tracker" = "https://github.com/axieum/django-user-trace/issues"
 "Release notes" = "https://axieum.github.io/django-user-trace/latest/changelog/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = "^3.0 | ^4.0"
+celery = {version = "^5.3.0", optional = true}
+
+[tool.poetry.extras]
+celery = ["celery"]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.21.0"
+pytest-celery = "^0.0.0"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
+pytest-mock = "^3.11.1"
 pytest-xdist = "^3.1.0"
 syrupy = "^3.0.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = ">=0.990"
 django-stubs = "^1.13.1"
 
@@ -63,14 +76,18 @@
 combine_as_imports = true
 
 [tool.mypy]
 files = ["src", "tests"]
 strict = true
 plugins = ["mypy_django_plugin.main"]
 
+  [[tool.mypy.overrides]]
+  module = "celery.*"
+  ignore_missing_imports = true
+
 [tool.django-stubs]
 django_settings_module = "example.settings"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 asyncio_mode = "auto"
 testpaths = ["tests"]
```

### Comparing `django_user_trace-1.0.0/src/django_user_trace/conf.py` & `django_user_trace-1.1.0/src/django_user_trace/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         #     a. To lookup nested attributes, separate them by `__` (two underscores), e.g. `profile__country__code`
         #   2. a callable that accepts (`AbstractBaseUser` | `AnonymousUser`, `HttpRequest`) and returns the result;
         #   3. an import string (prefixed with `ext://`) to a callable as seen in (2) above.
         self.USER_ATTRS: dict[str, str | Callable[[AbstractBaseUser | AnonymousUser, HttpRequest], Any]] = {
             "username": "get_username",
         }
 
+        # The name of the Celery task header used to trace user attributes
+        self.CELERY_TASK_HEADER: str = "User"
+
         # Load user defined settings
         if user_settings := getattr(django_settings, key, None):
             for setting, value in user_settings.items():
                 if not hasattr(self, setting):
                     raise ImproperlyConfigured(f"'{setting}' is not a valid django-user-trace setting.")
                 setattr(self, setting, value)
```

### Comparing `django_user_trace-1.0.0/src/django_user_trace/context.py` & `django_user_trace-1.1.0/src/django_user_trace/context.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/src/django_user_trace/log.py` & `django_user_trace-1.1.0/src/django_user_trace/log.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/src/django_user_trace/middleware.py` & `django_user_trace-1.1.0/src/django_user_trace/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 from asgiref.sync import sync_to_async
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.decorators import sync_and_async_middleware
 
 from django_user_trace.conf import settings
 from django_user_trace.context import user_attrs
+from django_user_trace.signals import cleanup_request, process_request
 from django_user_trace.utils import rgetattr
 
 if TYPE_CHECKING:
     from django.http import HttpRequest, HttpResponse
 
     GetResponseCallable = Callable[[HttpRequest], Union[HttpResponse, Awaitable[HttpResponse]]]
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def process_request(request: HttpRequest) -> None:
+def process_incoming_request(request: HttpRequest) -> None:
     """
-    Process an incoming HTTP request.
+    Processes an incoming HTTP request.
 
     :param request: http request
     """
 
     # Check that authentication has been performed by an earlier middleware
     if not hasattr(request, "user"):
         raise ImproperlyConfigured(
@@ -46,14 +47,28 @@
                 else None
             )
             for key, lookup in settings.USER_ATTRS.items()
         }
     )
     logger.debug("set `user_attrs` context var to %s", user_attrs.get())
 
+    # Send a signal
+    process_request.send(django_user_trace_middleware, request=request)
+
+
+def process_outgoing_request(request: HttpRequest) -> None:
+    """
+    Processes an outgoing HTTP request.
+
+    :param request: http request
+    """
+
+    # Send a signal
+    cleanup_request.send(django_user_trace_middleware, request=request)
+
 
 @sync_and_async_middleware
 def django_user_trace_middleware(get_response: GetResponseCallable) -> GetResponseCallable:
     """
     Observes the Django user context of a request for use in Python's logging framework.
 
     :param get_response: next callable for the http response
@@ -63,19 +78,23 @@
     # async middleware
     if asyncio.iscoroutinefunction(get_response):
 
         async def middleware(request: HttpRequest) -> HttpResponse:
             logger.debug("async middleware called")
             if hasattr(request, "user"):
                 await sync_to_async(request.user._setup)()  # type: ignore
-            process_request(request)
-            return await get_response(request)  # type: ignore
+            process_incoming_request(request)
+            res: HttpResponse = await get_response(request)
+            process_outgoing_request(request)
+            return res
 
     # sync middleware
     else:
 
         def middleware(request: HttpRequest) -> HttpResponse:  # type: ignore[misc]
             logger.debug("sync middleware called")
-            process_request(request)
-            return get_response(request)  # type: ignore
+            process_incoming_request(request)
+            res: HttpResponse = get_response(request)  # type: ignore
+            process_outgoing_request(request)
+            return res
 
     return middleware
```

### Comparing `django_user_trace-1.0.0/src/django_user_trace/signals.py` & `django_user_trace-1.1.0/src/django_user_trace/signals.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from __future__ import annotations
 
 import logging
-from typing import Any
+from typing import Any, Final
 
 from django.core.signals import request_finished
-from django.dispatch import receiver
+from django.dispatch import Signal, receiver
 
 from django_user_trace.context import user_attrs
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+# Signaled before the view is called, during the `django-user-trace` middleware
+#   :param request: HttpRequest
+process_request: Final[Signal] = Signal()
+
+
+# Signaled after the view has been called, during the `django-user-trace` middleware
+#   :param request: HttpRequest
+cleanup_request: Final[Signal] = Signal()
+
+
 @receiver(request_finished)
 def clear_user_attrs_after_request(sender: Any, **kwargs: dict[str, Any]) -> None:
     """
     Clears the `user_attrs` context variable after each HTTP request.
 
     :param sender: signal sender
     :param kwargs: signal keyword arguments
```

### Comparing `django_user_trace-1.0.0/src/django_user_trace/utils.py` & `django_user_trace-1.1.0/src/django_user_trace/utils.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/tests/feature/test_async_request.py` & `django_user_trace-1.1.0/tests/feature/test_async_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     from django.test.client import AsyncClient
 
 
 async def test_anonymous_async_request(async_client: AsyncClient, caplog: LogCaptureFixture) -> None:
     """Tests that logs during an unauthenticated async request contain the *anonymous* user context."""
 
     # Fetch the index page
-    await async_client.get("/")
+    await async_client.get("/asgi/")
 
     # Expect the log messages to have Django's *anonymous* user context
     assert [(r.message, getattr(r, "username", None)) for r in caplog.records] == [
         ("async middleware called", None),
         ("set `user_attrs` context var to {'username': None}", None),
-        ("load `index_view` view", None),
+        ("load `aindex_view` view", None),
         ("received signal `request_finished`, clearing `user_attrs` context var", None),
     ]
 
 
 @pytest.mark.django_db(transaction=True)
 async def test_authenticated_async_request(async_client: AsyncClient, caplog: LogCaptureFixture) -> None:
     """Tests that logs during an authenticated async request contain the logged-in user context."""
@@ -37,31 +37,31 @@
     # Create a new user
     user: AbstractUser = await sync_to_async(get_user_model().objects.create)(
         username=(username := "jonathan"), email="jonathan@localhost", first_name="Jonathan", last_name="Hiles"
     )
 
     # Fetch the index page
     await sync_to_async(async_client.force_login)(user)
-    await async_client.get("/")
+    await async_client.get("/asgi/")
 
     # Expect the log messages to have the expected Django user context
     assert [(r.message, getattr(r, "username", None)) for r in caplog.records] == [
         ("async middleware called", None),
         (f"set `user_attrs` context var to {{'username': '{username}'}}", username),
-        ("load `index_view` view", username),
+        ("load `aindex_view` view", username),
         ("received signal `request_finished`, clearing `user_attrs` context var", username),
     ]
 
 
 @pytest.mark.django_db(transaction=True)
 async def test_concurrent_authenticated_async_requests(async_client: AsyncClient, caplog: LogCaptureFixture) -> None:
     """Tests that the user context from an authenticated async request does not bleed into other request logs."""
 
     # Create new users
-    users: tuple[AbstractUser, ...] = await asyncio.gather(
+    users: list[AbstractUser] = await asyncio.gather(
         # Jane Doe
         sync_to_async(get_user_model().objects.create)(
             username="jane", email="jane@localhost", first_name="Jane", last_name="Doe"
         ),
         # John Doe
         sync_to_async(get_user_model().objects.create)(
             username="john", email="john@localhost", first_name="John", last_name="Doe"
@@ -72,24 +72,24 @@
         ),
     )
 
     # Fetch the index page as each user concurrently
     async def _async_request(login_as: AbstractUser) -> HttpResponseBase:
         _async_client: AsyncClient = deepcopy(async_client)
         await sync_to_async(_async_client.force_login)(login_as)
-        return await _async_client.get("/")
+        return await _async_client.get("/asgi/")
 
     await asyncio.gather(*(_async_request(user) for user in users))
 
     # Expect the log messages to have the expected Django user context
     assert sorted([(r.message, getattr(r, "username", None)) for r in caplog.records]) == sorted(
         [
             entry
             for user in users
             for entry in (
-                ("async middleware called", None),  # user attributes from prior requests should not remain afterwards
+                ("async middleware called", None),  # user attributes from prior requests should not remain afterward
                 (f"set `user_attrs` context var to {{'username': '{user.get_username()}'}}", user.get_username()),
-                ("load `index_view` view", user.get_username()),
+                ("load `aindex_view` view", user.get_username()),
                 ("received signal `request_finished`, clearing `user_attrs` context var", user.get_username()),
             )
         ]
     )
```

### Comparing `django_user_trace-1.0.0/tests/feature/test_conf.py` & `django_user_trace-1.1.0/tests/feature/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/tests/feature/test_sync_request.py` & `django_user_trace-1.1.0/tests/feature/test_sync_request.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/tests/unit/test_conf.py` & `django_user_trace-1.1.0/tests/unit/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/tests/unit/test_middleware.py` & `django_user_trace-1.1.0/tests/unit/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/tests/unit/test_utils.py` & `django_user_trace-1.1.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_user_trace-1.0.0/PKG-INFO` & `django_user_trace-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: django-user-trace
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python logging filter for Django user attributes.
 Home-page: https://github.com/axieum/django-user-trace
 License: MIT
 Keywords: async,django,logs,logging,middleware,sync,trace,tracing,user,web
 Author: Jonathan Hiles
 Author-email: jonathan@hil.es
 Requires-Python: >=3.8,<4.0
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Provides-Extra: celery
+Requires-Dist: celery (>=5.3.0,<6.0.0) ; extra == "celery"
 Requires-Dist: django (>=3.0,<5.0)
 Project-URL: Documentation, https://axieum.github.io/django-user-trace/latest/
 Project-URL: Funding, https://github.com/sponsors/axieum
 Project-URL: Issue tracker, https://github.com/axieum/django-user-trace/issues
 Project-URL: Repository, https://github.com/axieum/django-user-trace
 Project-URL: Release notes, https://axieum.github.io/django-user-trace/latest/changelog/
 Description-Content-Type: text/markdown
@@ -62,14 +71,18 @@
     django_user_trace -->> logging: `ContextVar` for user attrs
     django ->>+ django_user_trace: signal `request_finished`
     note over django, django_user_trace: Clear user attributes from the `ContextVar`
     django_user_trace ->>+ django: continue
     django -->> User: send response
 ```
 
+#### Supports
+
+* [Celery task logging][celery]
+
 #### Resources
 
 * [Django &mdash; How to configure and use logging][django:logging]
 
 #### Related Projects
 
 * [madzak/python-json-logger][python-json-logger]
@@ -100,14 +113,15 @@
 vulnerabilities.
 
 ## Licence
 
 `django-user-trace` is open-sourced software licenced under the
 [MIT licence][licence].
 
+[celery]: https://docs.celeryq.dev/
 [ci:release]: https://github.com/axieum/django-user-trace/actions/workflows/release.yml
 [ci:test]: https://github.com/axieum/django-user-trace/actions/workflows/test.yml
 [codecov]: https://app.codecov.io/gh/axieum/django-user-trace
 [contributing]: CONTRIBUTING.md
 [django]: https://djangoproject.com/
 [django:logging]: https://docs.djangoproject.com/en/stable/howto/logging/
 [django-guid]: https://github.com/snok/django-guid
```

