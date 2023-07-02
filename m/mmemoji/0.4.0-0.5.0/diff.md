# Comparing `tmp/mmemoji-0.4.0.tar.gz` & `tmp/mmemoji-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmemoji-0.4.0.tar", max compression
+gzip compressed data, was "mmemoji-0.5.0.tar", max compression
```

## Comparing `mmemoji-0.4.0.tar` & `mmemoji-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35147 2022-03-28 04:18:13.049319 mmemoji-0.4.0/LICENSE
--rw-r--r--   0        0        0     2912 2022-03-28 04:18:13.049319 mmemoji-0.4.0/README.md
--rw-r--r--   0        0        0     2309 2022-03-28 04:18:13.049319 mmemoji-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      349 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/__init__.py
--rw-r--r--   0        0        0     1378 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/cli.py
--rw-r--r--   0        0        0        0 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/__init__.py
--rw-r--r--   0        0        0     1577 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/create.py
--rw-r--r--   0        0        0     1216 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/delete.py
--rw-r--r--   0        0        0     2770 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/download.py
--rw-r--r--   0        0        0      402 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/list.py
--rw-r--r--   0        0        0      631 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/commands/search.py
--rw-r--r--   0        0        0     6113 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/decorators.py
--rw-r--r--   0        0        0     6676 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/emoji.py
--rw-r--r--   0        0        0      686 2022-03-28 04:18:13.049319 mmemoji-0.4.0/src/mmemoji/exceptions.py
--rw-r--r--   0        0        0     4073 2022-03-28 04:18:21.636834 mmemoji-0.4.0/setup.py
--rw-r--r--   0        0        0     4177 2022-03-28 04:18:21.637267 mmemoji-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-02 19:36:02.618996 mmemoji-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2933 2023-07-02 19:36:02.618996 mmemoji-0.5.0/README.md
+-rw-r--r--   0        0        0     2258 2023-07-02 19:36:02.622996 mmemoji-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      179 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/__main__.py
+-rw-r--r--   0        0        0     1340 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/cli.py
+-rw-r--r--   0        0        0        0 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/create.py
+-rw-r--r--   0        0        0     1180 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/delete.py
+-rw-r--r--   0        0        0     2775 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/download.py
+-rw-r--r--   0        0        0      401 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/list.py
+-rw-r--r--   0        0        0      630 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/commands/search.py
+-rw-r--r--   0        0        0     6212 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/decorators.py
+-rw-r--r--   0        0        0     6684 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/emoji.py
+-rw-r--r--   0        0        0      670 2023-07-02 19:36:02.622996 mmemoji-0.5.0/src/mmemoji/exceptions.py
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 mmemoji-0.5.0/PKG-INFO
```

### Comparing `mmemoji-0.4.0/LICENSE` & `mmemoji-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmemoji-0.4.0/README.md` & `mmemoji-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 ```shell
 pip install mmemoji
 mmemoji --help
 ```
 
-_(Requires Python >=3.7)_
+_(Requires Python >=3.8)_
 
 ## Usage example
 
 Let's take the [Party Parrot][COTPP] Emojis as an example.
 
 * First, clone the Git repository or retrieve an archive of it:
 
@@ -45,26 +45,26 @@
 
 * Finally, run `mmemoji` to import all the parrots:
 
 ```shell
 mmemoji create --no-clobber {parrots,guests}/hd/*.gif {parrots,guests}/*.gif
 ```
 
-> _Notes_:
+> **Note**
 >
 > * Here we rely on [shell globbing][glob] to select all emojis from the directories.
 > * Specifying the `hd` directories first with `--no-clobber` ensures these emojis are created first and not overwritten by their lower quality counterpart.
 
 * If you ever want to remove them all, simply run the following:
 
 ```shell
 mmemoji delete --force {parrots,guests}/hd/*.gif {parrots,guests}/*.gif
 ```
 
-> _Notes_:
+> **Note**
 >
 > * The emoji names are extracted from the filenames the same way they have been during creation.
 > * `--force` is used to ignore the absent low quality duplicates.
 
 ## Development
 
 * You can clone this repository and install the project with [Poetry][poetry]:
@@ -93,13 +93,13 @@
 
 [pypi badge]: https://img.shields.io/pypi/v/mmemoji.svg
 [pypi link]: https://pypi.python.org/pypi/mmemoji
 [build badge]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml/badge.svg
 [build link]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml
 [sonarcloud badge]: https://sonarcloud.io/api/project_badges/measure?project=maxbrunet_mmemoji&metric=alert_status
 [sonarcloud link]: https://sonarcloud.io/dashboard?id=maxbrunet_mmemoji
-[mattermost]: https://www.mattermost.org
+[mattermost]: https://github.com/mattermost/mattermost-server
 [COTPP]: https://cultofthepartyparrot.com
 [glob]: https://en.wikipedia.org/wiki/Glob_(programming)
 [poetry]: https://python-poetry.org/docs/
 [docker]: https://www.docker.com
 [pre-commit]: https://pre-commit.com
```

### Comparing `mmemoji-0.4.0/pyproject.toml` & `mmemoji-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 
 [tool.coverage.run]
 source = ["src"]
 relative_files = true
 
 [tool.black]
 line-length = 79
-target_version = ["py37", "py38", "py39", "py310"]
-
-[tool.isort]
-profile = "black"
-line_length = 79
+target_version = ["py38", "py39", "py310", "py311"]
 
 [tool.mypy]
 files = ["."]
 exclude = "^build/"
 mypy_path = "src"
 show_column_numbers = true
 strict = true
@@ -31,63 +27,64 @@
 # importlib_metadata is not fully typed
 # and package-level overrides do not work
 # https://github.com/python/importlib_metadata/pull/342
 # https://github.com/python/mypy/issues/10757
 disallow_untyped_calls = false
 
 [[tool.mypy.overrides]]
-module = ["mattermostdriver.*"]
+module = ["filetype", "mattermostdriver.*"]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "mmemoji"
-version = "0.4.0"
+version = "0.5.0"
 description = "Custom Emoji manager command-line for Mattermost 😎"
 readme = "README.md"
 authors = []
 classifiers=[
     "Environment :: Web Environment",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
 ]
 keywords = ["cli", "emoji", "mattermost"]
 repository = "https://github.com/maxbrunet/mmemoji.git"
 license = "GPLv3"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 click = ">=8.0.0"
-importlib-metadata = { version = ">=1.4.0", python = "<3.8" }
+filetype = ">=0.1.3"
 mattermostdriver = ">=6.1.2"
-mypy-extensions = ">=0.4.3"
 requests = ">=2.19.0"
 tabulate = ">=0.7.3"
+typing-extensions = { version = ">=3.10.0.0", python = "<3.10" }
 Unidecode = ">=0.04.1"
 
-[tool.poetry.dev-dependencies]
-black = "==22.1.0"
-isort = "==5.10.1"
-flake8 = "==4.0.1"
-mypy = "==0.942"
-pytest = "==7.1.1"
-pytest-black = "==0.3.12"
-pytest-cov = "==3.0.0"
-pytest-flake8 = "==1.1.1"
-pytest-isort = "==3.0.0"
-pytest-mypy = "==0.9.1"
-types-requests = "==2.27.14"
-types-tabulate = "==0.8.6"
+[tool.poetry.group.dev.dependencies]
+black = "==23.3.0"
+mypy = "==1.4.0"
+pytest = "==7.4.0"
+pytest-cov = "==4.1.0"
+ruff = "==0.0.275"
+types-requests = "==2.31.0.1"
+types-tabulate = "==0.9.0.2"
 
 [tool.poetry.plugins."console_scripts"]
 "mmemoji" = "mmemoji.cli:cli"
 
 [tool.pytest.ini_options]
 addopts = "--verbose"
+
+[tool.ruff]
+line-length = 79
+select = ["E", "F", "I", "UP"]
+src = ["src"]
+target-version = "py38"
```

### Comparing `mmemoji-0.4.0/src/mmemoji/cli.py` & `mmemoji-0.5.0/src/mmemoji/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import logging
 import os
-from typing import Any, List, cast
+from typing import List, cast
 
 import click
 
 from mmemoji import __summary__, __version__
 
 logging.getLogger("mattermostdriver.websocket").disabled = True
 
 
 class EmojiCLI(click.MultiCommand):
     """Custom Click Command class to dynamically discover subcommands"""
 
-    def list_commands(self, ctx: Any) -> List[str]:
+    def list_commands(self, ctx: click.Context) -> List[str]:
         rv = []
         cmd_folder = os.path.abspath(
             os.path.join(os.path.dirname(__file__), "commands")
         )
         for filename in os.listdir(cmd_folder):
-            if filename.endswith(".py") and not filename == "__init__.py":
+            if filename.endswith(".py") and filename != "__init__.py":
                 rv.append(filename[:-3])
         rv.sort()
         return rv
 
-    def get_command(self, ctx: Any, name: str) -> click.Command:
+    def get_command(self, ctx: click.Context, name: str) -> click.Command:
         try:
             module = __import__(
                 "mmemoji.commands." + name, None, None, ["cli"]
             )
             return cast(click.Command, module.cli)
         except ModuleNotFoundError:
             raise click.ClickException(
-                'Unknown command "{}" for "{}"\n'
-                "Run '{} --help' for usage.".format(
-                    name, ctx.info_name, ctx.info_name
-                )
+                f'Unknown command "{name}" for "{ctx.info_name}"\n'
+                f"Run '{ctx.info_name} --help' for usage."
             )
 
 
 @click.command(name="mmemoji", cls=EmojiCLI, help=__summary__)
 @click.version_option(version=__version__, message="%(prog)s %(version)s")
 def cli() -> None:
     """CLI entry-point"""
```

### Comparing `mmemoji-0.4.0/src/mmemoji/commands/create.py` & `mmemoji-0.5.0/src/mmemoji/commands/create.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, List
+from typing import List
 
 import click
 from requests import HTTPError
 
 from mmemoji import Emoji
-from mmemoji.decorators import parse_global_options
+from mmemoji.decorators import EmojiContext, parse_global_options
 
 
 @click.command(help="Create custom Emojis")
 @click.argument("images", type=click.File("rb", lazy=True), nargs=-1)
 @click.option(
     "-f",
     "--force",
@@ -25,30 +25,30 @@
     help="do not overwrite an existing file (overrides -i option)",
 )
 @click.option(
     "-i", "--interactive", is_flag=True, help="prompt before overwrite"
 )
 @parse_global_options
 def cli(
-    ctx: Any,
+    ctx: EmojiContext,
     images: List[str],
     force: bool,
     no_clobber: bool,
     interactive: bool,
 ) -> None:
     emojis = []
 
     try:
         with click.progressbar(images, show_pos=True) as pb_images:
             for image in pb_images:
                 emoji = Emoji(ctx.mattermost, image.name)
 
                 if emoji.metadata and not no_clobber and interactive:
                     force = click.confirm(
-                        'overwrite "{}"?'.format(emoji.name), err=True
+                        f'overwrite "{emoji.name}"?', err=True
                     )
                     if not force:
                         continue
 
                 with image as img:
                     if emoji.create(img, force, no_clobber):
                         emojis.append(emoji.metadata)
```

### Comparing `mmemoji-0.4.0/src/mmemoji/commands/delete.py` & `mmemoji-0.5.0/src/mmemoji/commands/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-from typing import Any, List
+from typing import List
 
 import click
 from requests import HTTPError
 
 from mmemoji import Emoji
-from mmemoji.decorators import parse_global_options
+from mmemoji.decorators import EmojiContext, parse_global_options
 
 
 @click.command(help="Delete custom Emojis")
 @click.argument("emoji_names", nargs=-1)
 @click.option("-f", "--force", is_flag=True, help="ignore nonexistent files")
 @click.option(
     "-i", "--interactive", is_flag=True, help="prompt before every removal"
 )
 @parse_global_options
 def cli(
-    ctx: Any, emoji_names: List[str], force: bool, interactive: bool
+    ctx: EmojiContext, emoji_names: List[str], force: bool, interactive: bool
 ) -> None:
     emojis = []
     try:
         with click.progressbar(emoji_names, show_pos=True) as pb_names:
             for name in pb_names:
                 emoji = Emoji(ctx.mattermost, name)
 
                 if (
                     interactive
                     and emoji.metadata
-                    and not click.confirm(
-                        'delete "{}"?'.format(emoji.name), err=True
-                    )
+                    and not click.confirm(f'delete "{emoji.name}"?', err=True)
                 ):
                     continue
 
                 if emoji.delete(force):
                     emojis.append(emoji.metadata)
     except HTTPError as e:
         raise click.ClickException(e.args[0] if e.args != () else repr(e))
```

### Comparing `mmemoji-0.4.0/src/mmemoji/commands/download.py` & `mmemoji-0.5.0/src/mmemoji/commands/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import imghdr
 import os
-from typing import Any, List
+from typing import List
 
 import click
+from filetype import filetype
 from requests import HTTPError
 
 from mmemoji import Emoji
-from mmemoji.decorators import parse_global_options
+from mmemoji.decorators import EmojiContext, parse_global_options
 
 
-def check_destination(ctx: Any, param: click.Parameter, value: str) -> str:
+def check_destination(
+    ctx: EmojiContext, param: click.Parameter, value: str
+) -> str:
     """Ensure destination is valid.
 
     For 1 emoji, the destination can be a file
     with an existing parent directory, or an existing directory,
     but if the destination is explicitly a directory,
     the full path must exits.
 
@@ -23,21 +25,21 @@
     """
     count = len(ctx.params["emoji_names"])
     if count == 1 and value[-1] != os.path.sep and not os.path.isdir(value):
         directory = os.path.dirname(value) or os.getcwd()
     else:
         directory = value
     if not os.path.isdir(directory):
-        raise click.ClickException("{}: Not a directory".format(directory))
+        raise click.ClickException(f"{directory}: Not a directory")
     if (
         not os.access(directory, os.W_OK)
         or os.path.isfile(value)
         and not os.access(value, os.W_OK)
     ):
-        raise click.ClickException("{}: Permission denied".format(directory))
+        raise click.ClickException(f"{directory}: Permission denied")
     return value
 
 
 @click.command(help="Download custom Emojis")
 @click.argument("emoji_names", nargs=-1)
 @click.argument("destination", callback=check_destination, type=click.Path())
 @click.option(
@@ -53,15 +55,15 @@
     help="do not overwrite an existing file (overrides -f and -i options)",
 )
 @click.option(
     "-i", "--interactive", is_flag=True, help="prompt before overwrite"
 )
 @parse_global_options
 def cli(
-    ctx: Any,
+    ctx: EmojiContext,
     emoji_names: List[str],
     destination: str,
     force: bool,
     no_clobber: bool,
     interactive: bool,
 ) -> None:
     try:
@@ -69,24 +71,23 @@
             emoji = Emoji(ctx.mattermost, name)
             image = emoji.download()
 
             if not os.path.isdir(destination):
                 filename = destination
             else:
                 filename = os.path.join(
-                    destination, "{}.{}".format(name, imghdr.what(None, image))
+                    destination,
+                    f"{name}.{filetype.guess_extension(image)}",
                 )
 
             if os.path.exists(filename) and (
                 not interactive
                 and (no_clobber or not force)
                 or interactive
-                and not click.confirm(
-                    'overwrite "{}"?'.format(filename), err=True
-                )
+                and not click.confirm(f'overwrite "{filename}"?', err=True)
             ):
                 continue
 
             with open(filename, "wb") as f:
                 f.write(image)
             click.echo(filename)
     except HTTPError as e:
```

### Comparing `mmemoji-0.4.0/src/mmemoji/commands/search.py` & `mmemoji-0.5.0/src/mmemoji/commands/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from typing import Any
-
 import click
 from requests import HTTPError
 
 from mmemoji import Emoji
-from mmemoji.decorators import parse_global_options
+from mmemoji.decorators import EmojiContext, parse_global_options
 
 
 @click.command(help="Search custom Emojis (200 results maximum)")
 @click.argument("term")
 @click.option(
     "-p",
     "--prefix-only",
     is_flag=True,
     help="only search for names starting with the search term",
 )
 @parse_global_options
-def cli(ctx: Any, term: str, prefix_only: bool) -> None:
+def cli(ctx: EmojiContext, term: str, prefix_only: bool) -> None:
     try:
         ctx.print_dict(Emoji.search(ctx.mattermost, term, prefix_only))
     except HTTPError as e:
         raise click.ClickException(e.args[0] if e.args != () else repr(e))
```

### Comparing `mmemoji-0.4.0/src/mmemoji/decorators.py` & `mmemoji-0.5.0/src/mmemoji/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,136 @@
 import json
+import sys
 from contextlib import contextmanager
 from functools import wraps
-from typing import Any, Callable, Dict, List, TypeVar
+from typing import Any, Callable, Dict, Iterator, List, TypeVar
 from urllib.parse import ParseResult, urlparse
 
 import click
 import requests.exceptions
 from mattermostdriver import Driver as Mattermost
 from mattermostdriver.exceptions import MethodNotAllowed
-from mypy_extensions import KwArg, VarArg
 from tabulate import tabulate
 
-Decorator = TypeVar("Decorator", bound=Callable[..., Any])
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
 
+P = ParamSpec("P")
+R = TypeVar("R")
 
-def validate_url(ctx: Any, param: click.Parameter, value: str) -> ParseResult:
+
+class EmojiContext(click.Context):
+    """
+    Custom Click Context class
+    to store global settings and manage authentication
+    """
+
+    def __init__(self) -> None:
+        self.output = "table"
+        self.mattermost: Any = None
+
+    @contextmanager
+    def authenticate(
+        self,
+        url: ParseResult,
+        token: str,
+        login_id: str,
+        password: str,
+        mfa_token: str,
+        insecure: bool,
+    ) -> Iterator[None]:
+        """Authenticate against the Mattermost server"""
+
+        if token and (login_id or password or mfa_token):
+            click.echo(
+                "Warning: Token specified along"
+                " with Login-ID/Password/MFA-token."
+                "Only Token will be used.",
+                err=True,
+            )
+
+        settings = {
+            "scheme": url.scheme,
+            "url": url.hostname,
+            "basepath": getattr(url, "path", ""),
+            "verify": not insecure,
+            "login_id": login_id,
+            "password": password,
+            "token": token,
+            "mfa_token": mfa_token,
+        }
+
+        if url.port:
+            settings["port"] = url.port
+        elif url.scheme == "https":
+            settings["port"] = 443
+        else:
+            settings["port"] = 80
+
+        self.mattermost = Mattermost(settings)
+        try:
+            try:
+                self.mattermost.login()
+                yield
+            finally:
+                # Logout is unnecessary if token was used
+                if token is None:
+                    self.mattermost.logout()
+        except (requests.exceptions.ConnectionError, MethodNotAllowed):
+            raise click.ClickException(
+                "Unable to reach Mattermost API at "
+                + self.mattermost.client.url
+            )
+        except requests.exceptions.HTTPError as e:
+            raise click.ClickException(e.args[0] if e.args != () else repr(e))
+
+    def print_dict(self, data: List[Dict[str, Any]]) -> None:
+        """Print dataset generated by a command to the standard output"""
+        count = len(data)
+        if count:
+            if self.output == "table":
+                click.echo(tabulate(data, headers="keys"))
+            else:
+                click.echo(json.dumps(data, indent=2))
+
+        click.echo(
+            f"\n({count} emoji{'' if count == 1 else 's'})",
+            err=True,
+        )
+
+
+pass_context = click.make_pass_decorator(EmojiContext, ensure=True)
+
+
+def validate_url(
+    ctx: EmojiContext, param: click.Parameter, value: str
+) -> ParseResult:
     """Ensure URL contains minimum information to be used"""
     url = urlparse(value)
     if not url.scheme or not url.hostname:
-        raise click.BadParameter("Malformed URL: {}".format(value))
+        raise click.BadParameter(f"Malformed URL: {value}")
     return url
 
 
 def compose(
-    *decorators: Callable[[Decorator], Decorator]
-) -> Callable[[Decorator], Decorator]:
+    *decorators: Callable[[Callable[P, R]], Callable[P, R]]
+) -> Callable[[Callable[P, R]], Callable[P, R]]:
     """Merge multiple decorators into a single one"""
 
-    def decorate(func: Decorator) -> Decorator:
+    def decorate(func: Callable[P, R]) -> Callable[P, R]:
         for decorator in reversed(decorators):
             func = decorator(func)
         return func
 
     return decorate
 
 
-global_options = compose(
+global_options: Callable[[Callable[P, R]], Callable[P, R]] = compose(
     click.option(
         "-u",
         "--url",
         metavar="URL",
         envvar="MM_URL",
         callback=validate_url,
         required=True,
@@ -99,110 +190,27 @@
 # Workaround for the help option of subcommands not being eager enough
 # The parent command is executed anyway
 # https://github.com/pallets/click/issues/295
 # https://github.com/pallets/click/issues/814
 # This moves all global options to the subcommand which isn't that bad
 # This way all options are visible when asking for help on a subcommand
 def parse_global_options(
-    func: Decorator,
-) -> Callable[[VarArg(Any), KwArg(Any)], Any]:
+    func: Callable[P, R],
+) -> Callable[P, R]:
     """Parse options used by every commands such as auth and output format"""
 
-    @wraps(global_options(func))  # type: ignore
-    @pass_context  # type: ignore
-    def wrapper(*args: Any, **kwargs: Any) -> Any:
+    @wraps(global_options(func))
+    @pass_context
+    def wrapper(*args: Any, **kwargs: Any) -> R:
         ctx = args[0]
         ctx.output = kwargs.pop("output")
         with ctx.authenticate(
             kwargs.pop("url"),
             kwargs.pop("token"),
             kwargs.pop("login_id"),
             kwargs.pop("password"),
             kwargs.pop("mfa_token"),
             kwargs.pop("insecure"),
         ):
             return func(*args, **kwargs)
 
     return wrapper
-
-
-class EmojiContext:
-    """
-    Custom Click Context class
-    to store global settings and manage authentication
-    """
-
-    def __init__(self) -> None:
-        self.output = "table"
-        self.mattermost: Any = None
-
-    @contextmanager
-    def authenticate(
-        self,
-        url: ParseResult,
-        token: str,
-        login_id: str,
-        password: str,
-        mfa_token: str,
-        insecure: bool,
-    ) -> Any:
-        """Authenticate against the Mattermost server"""
-
-        if token and (login_id or password or mfa_token):
-            click.echo(
-                "Warning: Token specified along"
-                " with Login-ID/Password/MFA-token."
-                "Only Token will be used.",
-                err=True,
-            )
-
-        settings = {
-            "scheme": url.scheme,
-            "url": url.hostname,
-            "basepath": getattr(url, "path", ""),
-            "verify": not insecure,
-            "login_id": login_id,
-            "password": password,
-            "token": token,
-            "mfa_token": mfa_token,
-        }
-
-        if url.port:
-            settings["port"] = url.port
-        elif url.scheme == "https":
-            settings["port"] = 443
-        else:
-            settings["port"] = 80
-
-        self.mattermost = Mattermost(settings)
-        try:
-            try:
-                yield self.mattermost.login()
-            finally:
-                # Logout is unnecessary if token was used
-                if token is None:
-                    self.mattermost.logout()
-        except (requests.exceptions.ConnectionError, MethodNotAllowed):
-            raise click.ClickException(
-                "Unable to reach Mattermost API at {}".format(
-                    self.mattermost.client.url
-                )
-            )
-        except requests.exceptions.HTTPError as e:
-            raise click.ClickException(e.args[0] if e.args != () else repr(e))
-
-    def print_dict(self, data: List[Dict[str, Any]]) -> None:
-        """Print dataset generated by a command to the standard output"""
-        count = len(data)
-        if count:
-            if self.output == "table":
-                click.echo(tabulate(data, headers="keys"))
-            else:
-                click.echo(json.dumps(data, indent=2))
-
-        click.echo(
-            "\n({} emoji{})".format(count, "" if count == 1 else "s"),
-            err=True,
-        )
-
-
-pass_context = click.make_pass_decorator(EmojiContext, ensure=True)
```

### Comparing `mmemoji-0.4.0/src/mmemoji/emoji.py` & `mmemoji-0.5.0/src/mmemoji/emoji.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from mmemoji.exceptions import EmojiAlreadyExists, EmojiNotFound
 
 
 class Emoji:
     """Interact with Mattermost custom Emojis."""
 
     def __init__(self, mattermost: Any, name: str) -> None:
-        """Init Emoji class with a Mattermost client instance and an Emoji name.
+        """Init Emoji class with a Mattermost client instance
+        and an Emoji name.
 
         Parameters
         ----------
         mattermost : :obj:`mattermostdriver.Driver`
             an instance of `mattermostdriver`_
         name : str
             an Emoji name. It can be a file path,
```

### Comparing `mmemoji-0.4.0/src/mmemoji/exceptions.py` & `mmemoji-0.5.0/src/mmemoji/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mmemoji import Emoji
 
 
 class EmojiNotFound(ResourceNotFound):  # type: ignore
     """Raised when an Emoji is not found on the Mattermost server"""
 
     def __init__(self, emoji: "Emoji") -> None:
-        super().__init__('Emoji "{}" does not exist'.format(emoji.name))
+        super().__init__(f'Emoji "{emoji.name}" does not exist')
 
 
 class EmojiAlreadyExists(InvalidOrMissingParameters):  # type: ignore
     """Raised when an Emoji already exists on the Mattermost server"""
 
     def __init__(self, emoji: "Emoji") -> None:
-        super().__init__('Emoji "{}" exists'.format(emoji.name))
+        super().__init__(f'Emoji "{emoji.name}" exists')
```

### Comparing `mmemoji-0.4.0/setup.py` & `mmemoji-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,137 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mmemoji
+Version: 0.5.0
+Summary: Custom Emoji manager command-line for Mattermost 😎
+Home-page: https://github.com/maxbrunet/mmemoji.git
+License: GPLv3
+Keywords: cli,emoji,mattermost
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: Unidecode (>=0.04.1)
+Requires-Dist: click (>=8.0.0)
+Requires-Dist: filetype (>=0.1.3)
+Requires-Dist: mattermostdriver (>=6.1.2)
+Requires-Dist: requests (>=2.19.0)
+Requires-Dist: tabulate (>=0.7.3)
+Requires-Dist: typing-extensions (>=3.10.0.0) ; python_version < "3.10"
+Project-URL: Repository, https://github.com/maxbrunet/mmemoji.git
+Description-Content-Type: text/markdown
+
+[![PyPI][pypi badge]][pypi link]
+[![Build Status][build badge]][build link]
+[![Quality Gate][sonarcloud badge]][sonarcloud link]
+
+# mmemoji
+
+Custom Emoji manager command-line for [Mattermost][mattermost] 😎
+
+Features:
+
+* Create custom Emojis
+* Delete custom Emojis
+* List custom Emojis
+* Search custom Emojis
+* Export custom Emojis
+
+## Installation
+
+
+```shell
+pip install mmemoji
+mmemoji --help
+```
+
+_(Requires Python >=3.8)_
+
+## Usage example
+
+Let's take the [Party Parrot][COTPP] Emojis as an example.
+
+* First, clone the Git repository or retrieve an archive of it:
+
+```shell
+git clone https://github.com/jmhobbs/cultofthepartyparrot.com.git
+cd cultofthepartyparrot.com
+```
+
+* Then you'll need your Mattermost credentials. You can either pass them to `mmemoji` with the arguments `--url`/`--login-id`/`--password` or via environment variables, for example:
+
+```shell
+export MM_URL='http://127.0.0.1:8065/api/v4'
+export MM_LOGIN_ID='user-1@sample.mattermost.com'
+export MM_PASSWORD='user-1'
+```
+
+* Finally, run `mmemoji` to import all the parrots:
+
+```shell
+mmemoji create --no-clobber {parrots,guests}/hd/*.gif {parrots,guests}/*.gif
+```
+
+> **Note**
+>
+> * Here we rely on [shell globbing][glob] to select all emojis from the directories.
+> * Specifying the `hd` directories first with `--no-clobber` ensures these emojis are created first and not overwritten by their lower quality counterpart.
+
+* If you ever want to remove them all, simply run the following:
+
+```shell
+mmemoji delete --force {parrots,guests}/hd/*.gif {parrots,guests}/*.gif
+```
+
+> **Note**
+>
+> * The emoji names are extracted from the filenames the same way they have been during creation.
+> * `--force` is used to ignore the absent low quality duplicates.
+
+## Development
+
+* You can clone this repository and install the project with [Poetry][poetry]:
+
+```shell
+poetry install
+```
+
+* You'll find a script to create a local [Docker][docker] test instance under `tests/`:
+
+```shell
+./tests/scripts/setup-mattermost.sh
+```
+
+* You can run the test suite with:
+
+```shell
+pytest
+```
+
+* And last thing, you can install the [pre-commit][pre-commit] hooks to help with the formatting of your code.
+
+```shell
+pre-commit install
+```
+
+[pypi badge]: https://img.shields.io/pypi/v/mmemoji.svg
+[pypi link]: https://pypi.python.org/pypi/mmemoji
+[build badge]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml/badge.svg
+[build link]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml
+[sonarcloud badge]: https://sonarcloud.io/api/project_badges/measure?project=maxbrunet_mmemoji&metric=alert_status
+[sonarcloud link]: https://sonarcloud.io/dashboard?id=maxbrunet_mmemoji
+[mattermost]: https://github.com/mattermost/mattermost-server
+[COTPP]: https://cultofthepartyparrot.com
+[glob]: https://en.wikipedia.org/wiki/Glob_(programming)
+[poetry]: https://python-poetry.org/docs/
+[docker]: https://www.docker.com
+[pre-commit]: https://pre-commit.com
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['mmemoji', 'mmemoji.commands']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Unidecode>=0.04.1',
- 'click>=8.0.0',
- 'mattermostdriver>=6.1.2',
- 'mypy-extensions>=0.4.3',
- 'requests>=2.19.0',
- 'tabulate>=0.7.3']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=1.4.0']}
-
-entry_points = \
-{'console_scripts': ['mmemoji = mmemoji.cli:cli']}
-
-setup_kwargs = {
-    'name': 'mmemoji',
-    'version': '0.4.0',
-    'description': 'Custom Emoji manager command-line for Mattermost 😎',
-    'long_description': "[![PyPI][pypi badge]][pypi link]\n[![Build Status][build badge]][build link]\n[![Quality Gate][sonarcloud badge]][sonarcloud link]\n\n# mmemoji\n\nCustom Emoji manager command-line for [Mattermost][mattermost] 😎\n\nFeatures:\n\n* Create custom Emojis\n* Delete custom Emojis\n* List custom Emojis\n* Search custom Emojis\n* Export custom Emojis\n\n## Installation\n\n\n```shell\npip install mmemoji\nmmemoji --help\n```\n\n_(Requires Python >=3.7)_\n\n## Usage example\n\nLet's take the [Party Parrot][COTPP] Emojis as an example.\n\n* First, clone the Git repository or retrieve an archive of it:\n\n```shell\ngit clone https://github.com/jmhobbs/cultofthepartyparrot.com.git\ncd cultofthepartyparrot.com\n```\n\n* Then you'll need your Mattermost credentials. You can either pass them to `mmemoji` with the arguments `--url`/`--login-id`/`--password` or via environment variables, for example:\n\n```shell\nexport MM_URL='http://127.0.0.1:8065/api/v4'\nexport MM_LOGIN_ID='user-1@sample.mattermost.com'\nexport MM_PASSWORD='user-1'\n```\n\n* Finally, run `mmemoji` to import all the parrots:\n\n```shell\nmmemoji create --no-clobber {parrots,guests}/hd/*.gif {parrots,guests}/*.gif\n```\n\n> _Notes_:\n>\n> * Here we rely on [shell globbing][glob] to select all emojis from the directories.\n> * Specifying the `hd` directories first with `--no-clobber` ensures these emojis are created first and not overwritten by their lower quality counterpart.\n\n* If you ever want to remove them all, simply run the following:\n\n```shell\nmmemoji delete --force {parrots,guests}/hd/*.gif {parrots,guests}/*.gif\n```\n\n> _Notes_:\n>\n> * The emoji names are extracted from the filenames the same way they have been during creation.\n> * `--force` is used to ignore the absent low quality duplicates.\n\n## Development\n\n* You can clone this repository and install the project with [Poetry][poetry]:\n\n```shell\npoetry install\n```\n\n* You'll find a script to create a local [Docker][docker] test instance under `tests/`:\n\n```shell\n./tests/scripts/setup-mattermost.sh\n```\n\n* You can run the test suite with:\n\n```shell\npytest\n```\n\n* And last thing, you can install the [pre-commit][pre-commit] hooks to help with the formatting of your code.\n\n```shell\npre-commit install\n```\n\n[pypi badge]: https://img.shields.io/pypi/v/mmemoji.svg\n[pypi link]: https://pypi.python.org/pypi/mmemoji\n[build badge]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml/badge.svg\n[build link]: https://github.com/maxbrunet/mmemoji/actions/workflows/build.yml\n[sonarcloud badge]: https://sonarcloud.io/api/project_badges/measure?project=maxbrunet_mmemoji&metric=alert_status\n[sonarcloud link]: https://sonarcloud.io/dashboard?id=maxbrunet_mmemoji\n[mattermost]: https://www.mattermost.org\n[COTPP]: https://cultofthepartyparrot.com\n[glob]: https://en.wikipedia.org/wiki/Glob_(programming)\n[poetry]: https://python-poetry.org/docs/\n[docker]: https://www.docker.com\n[pre-commit]: https://pre-commit.com\n",
-    'author': None,
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/maxbrunet/mmemoji.git',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

