# Comparing `tmp/quart_auth-0.8.0.tar.gz` & `tmp/quart_auth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_auth-0.8.0.tar", max compression
+gzip compressed data, was "quart_auth-0.9.0.tar", max compression
```

## Comparing `quart_auth-0.8.0.tar` & `quart_auth-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1050 2022-07-23 20:32:30.310576 quart_auth-0.8.0/LICENSE
--rw-r--r--   0        0        0     4055 2022-07-23 20:32:30.310576 quart_auth-0.8.0/README.rst
--rw-r--r--   0        0        0     2094 2023-01-01 14:47:13.531196 quart_auth-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    13960 2023-01-01 14:47:13.531196 quart_auth-0.8.0/src/quart_auth/__init__.py
--rw-r--r--   0        0        0        7 2022-07-23 20:32:30.314576 quart_auth-0.8.0/src/quart_auth/py.typed
--rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 quart_auth-0.8.0/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 quart_auth-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-07-02 14:33:53.627236 quart_auth-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4037 2023-07-02 14:33:53.627236 quart_auth-0.9.0/README.rst
+-rw-r--r--   0        0        0     2150 2023-07-02 14:33:53.627236 quart_auth-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      587 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/basic_auth.py
+-rw-r--r--   0        0        0    11462 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/extension.py
+-rw-r--r--   0        0        0     3205 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/globals.py
+-rw-r--r--   0        0        0        7 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/py.typed
+-rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 quart_auth-0.9.0/PKG-INFO
```

### Comparing `quart_auth-0.8.0/LICENSE` & `quart_auth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_auth-0.8.0/README.rst` & `quart_auth-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 <https://gitlab.com/pgjones/quart>`_ to provide for secure cookie
 authentication (session management). It allows for a session to be
 logged in, authenticated and logged out.
 
 Usage
 -----
 
-To use Quart-Auth with a Quart app you have to create an AuthManager and
+To use Quart-Auth with a Quart app you have to create an QuartAuth and
 initialise it with the application,
 
 .. code-block:: python
 
     app = Quart(__name__)
-    AuthManager(app)
+    QuartAuth(app)
 
 or via the factory pattern,
 
 .. code-block:: python
 
-    auth_manager = AuthManager()
+    auth_manager = QuartAuth()
 
     def create_app():
         app = Quart(__name__)
         auth_manager.init_app(app)
         return app
 
 In addition you will need to configure Quart-Auth, which defaults to
@@ -43,15 +43,15 @@
 
     >>> import secrets
     >>> secrets.token_urlsafe(16)
 
 Tou may also need to disable secure cookies to use in development, see
 configuration below.
 
-With AuthManager initialised you can use the ``login_required``
+With QuartAuth initialised you can use the ``login_required``
 function to decorate routes that should only be accessed by
 authenticated users,
 
 .. code-block:: python
 
     from quart_auth import login_required
 
@@ -103,16 +103,16 @@
 
 Contributing
 ------------
 
 Quart-Auth is developed on `GitHub
 <https://github.com/pgjones/quart-auth>`_. You are very welcome to
 open `issues <https://github.com/pgjones/quart-auth/issues>`_ or
-propose `merge requests
-<https://github.com/pgjones/quart-auth/merge_requests>`_.
+propose `pull requests
+<https://github.com/pgjones/quart-auth/pulls>`_.
 
 Testing
 ~~~~~~~
 
 The best way to test Quart-Auth is with Tox,
 
 .. code-block:: console
```

### Comparing `quart_auth-0.8.0/pyproject.toml` & `quart_auth-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quart-auth"
-version = "0.8.0"
+version = "0.9.0"
 description = "A Quart extension to provide secure cookie authentication"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -56,14 +56,15 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry.dependencies]
 pydata_sphinx_theme = { version = "*", optional = true }
 python = ">=3.7"
 quart = ">=0.18"
+typing_extensions = { version = "*", python = "<3.10" }
 
 [tool.poetry.dev-dependencies]
 tox = "*"
 
 [tool.poetry.extras]
 docs = ["pydata_sphinx_theme"]
```

### Comparing `quart_auth-0.8.0/setup.py` & `quart_auth-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,181 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: quart-auth
+Version: 0.9.0
+Summary: A Quart extension to provide secure cookie authentication
+Home-page: https://github.com/pgjones/quart-auth/
+License: MIT
+Author: pgjones
+Author-email: philip.graham.jones@googlemail.com
+Requires-Python: >=3.7
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
+Requires-Dist: pydata_sphinx_theme ; extra == "docs"
+Requires-Dist: quart (>=0.18)
+Requires-Dist: typing_extensions ; python_version < "3.10"
+Project-URL: Repository, https://github.com/pgjones/quart-auth/
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+Quart-Auth
+==========
 
-packages = \
-['quart_auth']
+|Build Status| |docs| |pypi| |python| |license|
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['quart>=0.18']
-
-extras_require = \
-{'docs': ['pydata_sphinx_theme']}
-
-setup_kwargs = {
-    'name': 'quart-auth',
-    'version': '0.8.0',
-    'description': 'A Quart extension to provide secure cookie authentication',
-    'long_description': 'Quart-Auth\n==========\n\n|Build Status| |docs| |pypi| |python| |license|\n\nQuart-Auth is an extension for `Quart\n<https://gitlab.com/pgjones/quart>`_ to provide for secure cookie\nauthentication (session management). It allows for a session to be\nlogged in, authenticated and logged out.\n\nUsage\n-----\n\nTo use Quart-Auth with a Quart app you have to create an AuthManager and\ninitialise it with the application,\n\n.. code-block:: python\n\n    app = Quart(__name__)\n    AuthManager(app)\n\nor via the factory pattern,\n\n.. code-block:: python\n\n    auth_manager = AuthManager()\n\n    def create_app():\n        app = Quart(__name__)\n        auth_manager.init_app(app)\n        return app\n\nIn addition you will need to configure Quart-Auth, which defaults to\nthe most secure. At a minimum you will need to set secret key,\n\n.. code-block:: python\n\n    app.secret_key = "secret key"  # Do not use this key\n\nwhich you can generate via,\n\n.. code-block:: python\n\n    >>> import secrets\n    >>> secrets.token_urlsafe(16)\n\nTou may also need to disable secure cookies to use in development, see\nconfiguration below.\n\nWith AuthManager initialised you can use the ``login_required``\nfunction to decorate routes that should only be accessed by\nauthenticated users,\n\n.. code-block:: python\n\n    from quart_auth import login_required\n\n    @app.route("/")\n    @login_required\n    async def restricted_route():\n        ...\n\nIf no user is logged in, an ``Unauthorized`` exception is raised. To catch it,\ninstall an error handler,\n\n.. code-block:: python\n\n    @app.errorhandler(Unauthorized)\n    async def redirect_to_login(*_: Exception) -> ResponseReturnValue:\n        return redirect(url_for("login"))\n\nYou can also use the ``login_user``, and ``logout_user`` functions to\nstart and end sessions for a specific ``AuthenticatedUser`` instance,\n\n.. code-block:: python\n\n    from quart_auth import AuthUser, login_user, logout_user\n\n    @app.route("/login")\n    async def login():\n        # Check Credentials here, e.g. username & password.\n        ...\n        # We\'ll assume the user has an identifying ID equal to 2\n        login_user(AuthUser(2))\n        ...\n\n    @app.route("/logout")\n    async def logout():\n        logout_user()\n        ...\n\nThe user (authenticated or not) is available via the global\n``current_user`` including within templates,\n\n.. code-block:: python\n\n    from quart import render_template_string\n    from quart_auth import current_user\n\n    @app.route("/")\n    async def user():\n        return await render_template_string("{{ current_user.is_authenticated }}")\n\nContributing\n------------\n\nQuart-Auth is developed on `GitHub\n<https://github.com/pgjones/quart-auth>`_. You are very welcome to\nopen `issues <https://github.com/pgjones/quart-auth/issues>`_ or\npropose `merge requests\n<https://github.com/pgjones/quart-auth/merge_requests>`_.\n\nTesting\n~~~~~~~\n\nThe best way to test Quart-Auth is with Tox,\n\n.. code-block:: console\n\n    $ pip install tox\n    $ tox\n\nthis will check the code style and run the tests.\n\nHelp\n----\n\nThe Quart-Auth `documentation\n<https://quart-auth.readthedocs.io>`_ is the best places to\nstart, after that try searching `stack overflow\n<https://stackoverflow.com/questions/tagged/quart>`_ or ask for help\n`on gitter <https://gitter.im/python-quart/lobby>`_. If you still\ncan\'t find an answer please `open an issue\n<https://github.com/pgjones/quart-auth/issues>`_.\n\n\n.. |Build Status| image:: https://github.com/pgjones/quart-auth/actions/workflows/ci.yml/badge.svg\n   :target: https://github.com/pgjones/quart-auth/commits/main\n\n.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg\n   :target: https://quart-auth.readthedocs.io\n\n.. |pypi| image:: https://img.shields.io/pypi/v/quart-auth.svg\n   :target: https://pypi.python.org/pypi/Quart-Auth/\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/quart-auth.svg\n   :target: https://pypi.python.org/pypi/Quart-Auth/\n\n.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg\n   :target: https://github.com/pgjones/quart-auth/blob/main/LICENSE\n',
-    'author': 'pgjones',
-    'author_email': 'philip.graham.jones@googlemail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pgjones/quart-auth/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7',
-}
+Quart-Auth is an extension for `Quart
+<https://gitlab.com/pgjones/quart>`_ to provide for secure cookie
+authentication (session management). It allows for a session to be
+logged in, authenticated and logged out.
 
+Usage
+-----
+
+To use Quart-Auth with a Quart app you have to create an QuartAuth and
+initialise it with the application,
+
+.. code-block:: python
+
+    app = Quart(__name__)
+    QuartAuth(app)
+
+or via the factory pattern,
+
+.. code-block:: python
+
+    auth_manager = QuartAuth()
+
+    def create_app():
+        app = Quart(__name__)
+        auth_manager.init_app(app)
+        return app
+
+In addition you will need to configure Quart-Auth, which defaults to
+the most secure. At a minimum you will need to set secret key,
+
+.. code-block:: python
+
+    app.secret_key = "secret key"  # Do not use this key
+
+which you can generate via,
+
+.. code-block:: python
+
+    >>> import secrets
+    >>> secrets.token_urlsafe(16)
+
+Tou may also need to disable secure cookies to use in development, see
+configuration below.
+
+With QuartAuth initialised you can use the ``login_required``
+function to decorate routes that should only be accessed by
+authenticated users,
+
+.. code-block:: python
+
+    from quart_auth import login_required
+
+    @app.route("/")
+    @login_required
+    async def restricted_route():
+        ...
+
+If no user is logged in, an ``Unauthorized`` exception is raised. To catch it,
+install an error handler,
+
+.. code-block:: python
+
+    @app.errorhandler(Unauthorized)
+    async def redirect_to_login(*_: Exception) -> ResponseReturnValue:
+        return redirect(url_for("login"))
+
+You can also use the ``login_user``, and ``logout_user`` functions to
+start and end sessions for a specific ``AuthenticatedUser`` instance,
+
+.. code-block:: python
+
+    from quart_auth import AuthUser, login_user, logout_user
+
+    @app.route("/login")
+    async def login():
+        # Check Credentials here, e.g. username & password.
+        ...
+        # We'll assume the user has an identifying ID equal to 2
+        login_user(AuthUser(2))
+        ...
+
+    @app.route("/logout")
+    async def logout():
+        logout_user()
+        ...
+
+The user (authenticated or not) is available via the global
+``current_user`` including within templates,
+
+.. code-block:: python
+
+    from quart import render_template_string
+    from quart_auth import current_user
+
+    @app.route("/")
+    async def user():
+        return await render_template_string("{{ current_user.is_authenticated }}")
+
+Contributing
+------------
+
+Quart-Auth is developed on `GitHub
+<https://github.com/pgjones/quart-auth>`_. You are very welcome to
+open `issues <https://github.com/pgjones/quart-auth/issues>`_ or
+propose `pull requests
+<https://github.com/pgjones/quart-auth/pulls>`_.
+
+Testing
+~~~~~~~
+
+The best way to test Quart-Auth is with Tox,
+
+.. code-block:: console
+
+    $ pip install tox
+    $ tox
+
+this will check the code style and run the tests.
+
+Help
+----
+
+The Quart-Auth `documentation
+<https://quart-auth.readthedocs.io>`_ is the best places to
+start, after that try searching `stack overflow
+<https://stackoverflow.com/questions/tagged/quart>`_ or ask for help
+`on gitter <https://gitter.im/python-quart/lobby>`_. If you still
+can't find an answer please `open an issue
+<https://github.com/pgjones/quart-auth/issues>`_.
+
+
+.. |Build Status| image:: https://github.com/pgjones/quart-auth/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pgjones/quart-auth/commits/main
+
+.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
+   :target: https://quart-auth.readthedocs.io
+
+.. |pypi| image:: https://img.shields.io/pypi/v/quart-auth.svg
+   :target: https://pypi.python.org/pypi/Quart-Auth/
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/quart-auth.svg
+   :target: https://pypi.python.org/pypi/Quart-Auth/
+
+.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/pgjones/quart-auth/blob/main/LICENSE
 
-setup(**setup_kwargs)
```

