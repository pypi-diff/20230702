# Comparing `tmp/autopack_tools-0.1.9.tar.gz` & `tmp/autopack_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.9.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.0.tar", max compression
```

## Comparing `autopack_tools-0.1.9.tar` & `autopack_tools-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.9/LICENSE
--rw-r--r--   0        0        0     2925 2023-06-28 18:38:55.268381 autopack_tools-0.1.9/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.9/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.9/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.9/autopack/__main__.py
--rw-r--r--   0        0        0     2344 2023-06-28 22:13:39.865795 autopack_tools-0.1.9/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.9/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.9/autopack/errors.py
--rw-r--r--   0        0        0     4827 2023-06-28 23:23:28.263867 autopack_tools-0.1.9/autopack/get_pack.py
--rw-r--r--   0        0        0     2804 2023-06-28 20:52:32.647683 autopack_tools-0.1.9/autopack/installation.py
--rw-r--r--   0        0        0     2383 2023-06-28 23:21:27.392151 autopack_tools-0.1.9/autopack/pack.py
--rw-r--r--   0        0        0      955 2023-06-28 22:16:21.117129 autopack_tools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 autopack_tools-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.0/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.0/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.0/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-06-30 20:09:47.859652 autopack_tools-0.2.0/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-06-30 20:09:47.833824 autopack_tools-0.2.0/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.0/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-06-30 20:09:48.256517 autopack_tools-0.2.0/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-02 21:30:44.097116 autopack_tools-0.2.0/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-06-30 20:09:47.867664 autopack_tools-0.2.0/autopack/pack.py
+-rw-r--r--   0        0        0      636 2023-06-30 20:05:59.914181 autopack_tools-0.2.0/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.0/autopack/search.py
+-rw-r--r--   0        0        0     2628 2023-07-02 21:50:44.992073 autopack_tools-0.2.0/autopack/selection.py
+-rw-r--r--   0        0        0     4450 2023-07-02 21:30:44.111776 autopack_tools-0.2.0/autopack/utils.py
+-rw-r--r--   0        0        0      910 2023-07-02 21:53:27.971841 autopack_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.0/PKG-INFO
```

### Comparing `autopack_tools-0.1.9/LICENSE` & `autopack_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.9/README.md` & `autopack_tools-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,68 @@
-# AutoPack Tools
+# AutoPack
 
-[AutoPack](https://autopack.ai) is a repository for tools that are specifically designed for AI Agents.
-
-The `autopack-tools` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
-repository. Tools in AutoPack are called Packs.
-
-## Note
-
-This is still in the alpha stage. It's roughly at MVP level, and things will not work, features aren't complete, and
-things will change. Be forewarned.
+AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai), a
+collection of tools for AI
+Agents, currently tailored for LangChain implementations.
 
 ## Installation
 
-Install the `autopack-tools` package from PyPI using pip:
+You can install AutoPack using pip:
 
 ```bash
 pip install autopack-tools
 ```
 
-Or Poetry:
-
-```bash
-poetry add autopack-tools
-```
-
 ## Usage
 
-### Pack IDs
-
-Each pack in the AutoPack repository is identified by a fully qualified path based on its GitHub repository. This format
-ensures uniqueness, prevents namespace collisions, and allows for easy identification of the source code location.
-Importantly, it enables us to uniquely refer to a pack while keeping pack names intuitive and understandable for an LLM.
+AutoPack provides both a CLI and a Python library for interacting with the AutoPack repository.
 
-For example, the ID of a pack named `web_search` hosted in the GitHub repository `erik-megarad/my_packs` would be:
+### CLI: `autopack`
 
-`erik-megarad/my_packs/web_search`
+- Search for Packs: `autopack search {query}`
+- Install Packs: `autopack install {Pack ID}`
 
-This format allows us to use the pack's name, `web_search`, within an Agent, making it convenient and straightforward
-to reference the desired tool.
+### Python library: `autopack`
 
-### Manual Tool Installation
+The `autopack` Python library allows you to work with Packs programmatically. Key functionalities include:
 
-You can manually install a pack using the following command:
+- Search for Packs: `pack_search(query)`
+- Get a Pack: `get_pack(pack_id)`
+- Get all installed Packs: `get_all_installed_packs()`
+- Install a Pack: `install_pack(pack_id)`
+- Select packs using an LLM: `select_packs(task_description, llm)`
 
-```bash
-autopack install author/repo_name/tool_name
-```
-
-### Using with LangChain
-
-To use a tool with LangChain, you can retrieve it using the `get_pack` function from the `autopack` module:
-
-```python
-from autopack import get_pack
-
-tool = get_pack("author/repo_name/pack_name").tool
-
-# Add the tool to the 'tools' argument when instantiating your AgentExecutor
-agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=[tool()])
-```
+For detailed examples and more information, refer to
+the [AutoPack documentation](https://github.com/AutoPackAI/autopack/wiki).
 
-### Using with Auto-GPT
+## Safety and Security Notice
 
-We are actively working on improving the integration with Auto-GPT. Stay tuned for updates!
+Please exercise caution when using the AutoPack repository and library. The repository and library are currently in the
+early stages and intended for research purposes only. Ensure you review the Packs you install as they are directly
+cloned from GitHub. AutoPack and its maintainers are not liable for any misuse or negligence regarding the repository
+and library.
 
-To use `autopack` with Auto-GPT, you can edit the file `autogpt/main.py` and add `autopack` to the `COMMAND_CATEGORIES`
-list.
+For more details, please refer to
+the [Safety and Security section](https://github.com/AutoPackAI/autopack/wiki#safety-and-security-notice) in the
+documentation.
 
-## TODOs
+## Contributing
 
-This project is still in its early stages, and there are several features and enhancements that need to be implemented.
-If you are interested and willing to contribute, the following list provides a good starting point:
+We welcome contributions to the AutoPack ecosystem. Here are some ways you can help:
 
-- Tool search functionality within the CLI
-- Tool search capability from Python
-- Optional automatic pack installation in the `get_pack` function
-- Tools for Agents to independently search for, install, and utilize other Tools
-- Tool for utilizing the pack selection API of the AutoPack repository
-- Optional contribution of feedback back to the AutoPack repository
+- **Create new tools!** Expand the AutoPack repository by developing and submitting your own tools. Share your ideas and
+  solutions with the AutoPack community.
+- **Submit GitHub repos**: If you come across GitHub repositories containing useful tools, submit them to
+  the [AutoPack repository](https://autopack.ai/submissions). We'll create Packs out of the tools in those repositories
+  by providing the necessary metadata.
+- **Try it out for yourself**: Test AutoPack in your projects and provide feedback. Share your experiences, report bugs,
+  and suggest improvements by opening issues on GitHub.
+- **Contribute code**: Help improve AutoPack by opening pull requests. You can choose to work on unresolved issues or
+  implement new features that you believe would enhance the functionality of the library. Please note that the AutoPack
+  library is intentionally designed to be compact and straightforward.
 
-## Development
+We appreciate your contributions and look forward to your involvement in making AutoPack a vibrant and valuable resource
+for the autonomous AI community.
 
-For information on how to contribute to AutoPack, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+## License
 
-Feel free to modify this README to provide more specific details about your project and its functionalities.
+AutoPack is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `autopack_tools-0.1.9/autopack/cli.py` & `autopack_tools-0.2.0/autopack/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import argparse
 
 from autopack.installation import install_pack
+from autopack.search import print_search
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="AutoPack CLI tool")
 
     subparsers = parser.add_subparsers(dest="command")
     install_parser = subparsers.add_parser("install", help="Install a pack")
     install_parser.add_argument(
         "pack", help="ID (author/repo/pack_name) of the pack to install"
     )
+
+    search_parser = subparsers.add_parser("search", help="Search for packs")
+    search_parser.add_argument("query", help="The search query")
+
     parser.add_argument(
         "-f",
         "--force",
         help="Force automatic dependency installation",
         action="store_true",
     )
 
@@ -27,10 +32,13 @@
     if args.command == "install":
         result = install_pack(args.pack, args.force)
         if result:
             print("Installation completed")
         else:
             print("Installation failed")
 
+    if args.command == "search":
+        print_search(args.query)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `autopack_tools-0.1.9/autopack/get_pack.py` & `autopack_tools-0.2.0/autopack/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import importlib
 import inspect
+import json
 import os
 import sys
+from json import JSONDecodeError
 from types import ModuleType
-from typing import Type, Union
+from typing import Any, Type
 
-from autopack.api import PackResponse, get_pack_details
-from autopack.errors import (
-    AutoPackError,
-    AutoPackLoadError,
-    AutoPackNotFoundError,
-    AutoPackNotInstalledError,
-)
+from autopack.errors import (AutoPackLoadError, AutoPackNotFoundError,
+                             AutoPackNotInstalledError)
 from autopack.pack import Pack
+from autopack.pack_response import PackResponse
 
 
-def try_get_pack(pack_id: str, quiet=False) -> Union[Pack, None]:
+def find_or_create_autopack_dir(depth=0) -> str:
+    """Try to find a suitable .autopack directory. Tries in this order:
+    1. Directory specified in environment variable AUTOPACK_DIR
+    2. Existing .autopack directory in current directory
+    3. Existing .autopack directory up to 3 directories up
+    4. Creates an .autopack directory in current directory
     """
-    Get a pack based on its ID, in `author/repo_name/pack_name` format. Same as `get_pack` but does not raise an
-    Exception. If there is a problem finding or loading a pack it will return None.
+    env_dir = os.environ.get("AUTOPACK_DIR")
+    if env_dir:
+        return env_dir
 
-    Args:
-        pack_id (str): The ID of the pack to fetch.
-        quiet (bool, Optional): If True, won't print any output
+    autopack_dir = os.path.abspath(
+        os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack")
+    )
 
-    Returns:
-        BaseTool or None: The fetched pack as a LangChain BaseTool object, None if the pack could not be loaded
-    """
+    if not os.path.exists(autopack_dir) or not os.path.isdir(autopack_dir):
+        if depth > 3:
+            os.makedirs(".autopack", exist_ok=True)
+            return ".autopack"
+        return find_or_create_autopack_dir(depth=depth + 1)
 
-    try:
-        return get_pack(pack_id, quiet=quiet)
-    except AutoPackError:
-        return None
+    return autopack_dir
 
 
-def get_pack(pack_id: str, quiet=False) -> Pack:
-    """
-    Get a pack based on its ID, in `author/repo_name/pack_name` format.
+def load_metadata_file() -> dict[str, Any]:
+    """Return the parsed contents of the metadata file, returning an empty dict if not found or otherwise failed"""
+    metadata_dir = find_or_create_autopack_dir()
+    metadata_file = os.path.join(metadata_dir, "pack_metadata.json")
 
-    Args:
-        pack_id (str): The ID of the pack to fetch.
-        quiet (bool, Optional): If True, won't print any output
-
-    Returns:
-        BaseTool: The fetched pack as a LangChain BaseTool object
-
-    Raises:
-        AutoPackFetchError: If there was an error during the data fetch.
-        AutoPackNotInstalledError: If the pack was found but not installed.
-        AutoPackNotFoundError: If no pack matching that ID was found.
-        AutoPackLoadError: If the pack was found but there was an error importing or finding the pack class.
-    """
-    pack_data = get_pack_details(pack_id)
+    if not os.path.exists(metadata_file):
+        return {}
+
+    with open(metadata_file, "r") as f:
+        try:
+            return json.load(f)
+        except JSONDecodeError:
+            return {}
 
-    if not pack_data:
-        raise AutoPackNotFoundError()
 
-    return find_pack(pack_data, quiet=quiet)
+def write_metadata_file(data: dict[str, Any]):
+    metadata_dir = find_or_create_autopack_dir()
+    metadata_file = os.path.join(metadata_dir, "pack_metadata.json")
+
+    with open(metadata_file, "w+") as f:
+        json.dump(data, f)
 
 
 def find_module(pack_data: PackResponse) -> ModuleType:
     module_path = pack_data.module_path
 
     # Just in case they already have it in their path for whatever reason
     try:
@@ -71,41 +72,27 @@
 
         try:
             return importlib.import_module(pack_data.pack_path() + "." + module_path)
         finally:
             sys.path.remove(autopack_dir)
 
 
-def find_or_create_autopack_dir(depth=0) -> str:
-    """Search in current and parent directories looking for .autopack"""
-    autopack_dir = os.path.abspath(
-        os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack")
-    )
-
-    if not os.path.exists(autopack_dir) or not os.path.isdir(autopack_dir):
-        if depth > 3:
-            raise ModuleNotFoundError(".autopack directory could not be found")
-        return find_or_create_autopack_dir(depth=depth + 1)
-
-    return autopack_dir
-
-
-def find_pack(pack_data: PackResponse, quiet=False) -> Pack:
+def fetch_pack_object(pack_data: PackResponse, quiet=False) -> Pack:
     try:
         module = find_module(pack_data)
         if not module:
             message = (
                 f"Pack {pack_data.pack_id} could not be found. Either it is misconfigured or .autopack directory not "
                 f"found"
             )
             raise AutoPackNotFoundError(message)
 
         for _, obj in inspect.getmembers(module):
             if is_valid_pack(obj, pack_data.name):
-                return Pack(**{"tool": obj, **pack_data.__dict__})
+                return Pack(**{"tool_class": obj, **pack_data.__dict__})
 
         message = f"Pack {pack_data.pack_id} found, but {pack_data.name} is not found in its module"
         raise AutoPackNotFoundError(message)
     except ModuleNotFoundError:
         message = f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
         if not quiet:
             print(message)
```

### Comparing `autopack_tools-0.1.9/autopack/pack.py` & `autopack_tools-0.2.0/autopack/pack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Type
+from typing import Any, Optional
 
 from langchain.tools import BaseTool
 
 from autopack.api import PackResponse
 
 
 class Pack(BaseTool):
@@ -17,30 +17,46 @@
     module_path: str
     description: str
     name: str
     dependencies: list[str]
     source: str
     run_args: dict[str, Any]
     init_args: dict[str, Any]
-    # TODO/FIXME: This isn't guaranteed to be an actual BaseTool, by design, but typechecking complains otherwise
-    tool: Type[BaseTool]
+    tool_class: Any
+    tool: Any = None
 
-    def init_tool(self, init_args: dict[str, Any] = None):
+    def __getattr__(self, name):
+        """Tool classes may implement helper functions of various sorts, just pass those through to the tool"""
+        if hasattr(self.tool, name):
+            method = getattr(self.tool, name)
+
+            if callable(method):
+                # Wrap the call so that `self` is `self.tool`
+                def wrapped_call(*args, **kwargs):
+                    return method(self.tool, *args, **kwargs)
+
+                return wrapped_call
+
+        raise AttributeError(
+            f"'{self.__class__.__name__}' object has no attribute '{name}'"
+        )
+
+    def init_tool(self, init_args: Optional[dict[str, Any]] = None):
         init_args = init_args or {}
         is_valid = validate_tool_args(self.init_args, init_args)
         # TODO: Error handling on invalid args
         if is_valid:
-            self.tool(**init_args)
+            self.tool = self.tool_class(**init_args)
 
     def _run(self, *args, **kwargs):
         is_valid = validate_tool_args(self.run_args, kwargs)
         # TODO: Error handling on invalid args
         if is_valid:
             if hasattr(self.tool, "_run"):
-                return self.tool._run(self, *args, **kwargs)
+                return self.tool._run(*args, **kwargs)
             else:
                 return self.run(*args, **kwargs)
 
     async def _arun(self, *args, **kwargs):
         if hasattr(self.tool, "_run"):
             return await self.tool._arun(*args, **kwargs)
         else:
@@ -53,26 +69,26 @@
     @property
     def is_single_input(self) -> bool:
         """Hack on top of BaseTool to allow 0-arg tools"""
         keys = {k for k in self.args if k != "kwargs"}
         return len(keys) <= 1
 
     @classmethod
-    def from_pack_data(cls, tool: BaseTool, pack_data: PackResponse):
+    def from_pack_data(cls, tool_class: BaseTool, pack_data: PackResponse):
         return cls(
             pack_id=pack_data.pack_id,
             author=pack_data.author,
             repo=pack_data.repo,
             module_path=pack_data.module_path,
             description=pack_data.description,
             name=pack_data.name,
             dependencies=pack_data.dependencies,
             source=pack_data.source,
             run_args=pack_data.run_args,
             init_args=pack_data.init_args,
-            tool=tool,
+            tool_class=tool_class,
         )
 
 
 def validate_tool_args(spec: dict[str, Any], actual: dict[str, Any]):
     # TODO: This. Plus maybe some helpful errors?
     return True
```

### Comparing `autopack_tools-0.1.9/pyproject.toml` & `autopack_tools-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.9"
+version = "0.2.0"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
@@ -14,28 +14,26 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
-langchain = "^0.0.218"
+langchain = "^0.0.215"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 pytest = "^7.3.2"
 pytest-mock = "^3.11.1"
 types-requests = "^2.31.0.1"
 psycopg2 = "^2.9.6"
-docopt = "^0.6.2"
 autoflake = "^2.2.0"
 types-psycopg2 = "^2.9.21.10"
-types-docopt = "^0.6.11.3"
 pipreqs = "^0.4.13"
 gitpython = "^3.1.31"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autopack_tools-0.1.9/PKG-INFO` & `autopack_tools-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,90 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.9
+Version: 0.2.0
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: langchain (>=0.0.218,<0.0.219)
+Requires-Dist: langchain (>=0.0.215,<0.0.216)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/AutoPackAI/autopack
 Description-Content-Type: text/markdown
 
-# AutoPack Tools
+# AutoPack
 
-[AutoPack](https://autopack.ai) is a repository for tools that are specifically designed for AI Agents.
-
-The `autopack-tools` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
-repository. Tools in AutoPack are called Packs.
-
-## Note
-
-This is still in the alpha stage. It's roughly at MVP level, and things will not work, features aren't complete, and
-things will change. Be forewarned.
+AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai), a
+collection of tools for AI
+Agents, currently tailored for LangChain implementations.
 
 ## Installation
 
-Install the `autopack-tools` package from PyPI using pip:
+You can install AutoPack using pip:
 
 ```bash
 pip install autopack-tools
 ```
 
-Or Poetry:
-
-```bash
-poetry add autopack-tools
-```
-
 ## Usage
 
-### Pack IDs
-
-Each pack in the AutoPack repository is identified by a fully qualified path based on its GitHub repository. This format
-ensures uniqueness, prevents namespace collisions, and allows for easy identification of the source code location.
-Importantly, it enables us to uniquely refer to a pack while keeping pack names intuitive and understandable for an LLM.
+AutoPack provides both a CLI and a Python library for interacting with the AutoPack repository.
 
-For example, the ID of a pack named `web_search` hosted in the GitHub repository `erik-megarad/my_packs` would be:
+### CLI: `autopack`
 
-`erik-megarad/my_packs/web_search`
+- Search for Packs: `autopack search {query}`
+- Install Packs: `autopack install {Pack ID}`
 
-This format allows us to use the pack's name, `web_search`, within an Agent, making it convenient and straightforward
-to reference the desired tool.
+### Python library: `autopack`
 
-### Manual Tool Installation
+The `autopack` Python library allows you to work with Packs programmatically. Key functionalities include:
 
-You can manually install a pack using the following command:
+- Search for Packs: `pack_search(query)`
+- Get a Pack: `get_pack(pack_id)`
+- Get all installed Packs: `get_all_installed_packs()`
+- Install a Pack: `install_pack(pack_id)`
+- Select packs using an LLM: `select_packs(task_description, llm)`
 
-```bash
-autopack install author/repo_name/tool_name
-```
-
-### Using with LangChain
-
-To use a tool with LangChain, you can retrieve it using the `get_pack` function from the `autopack` module:
-
-```python
-from autopack import get_pack
-
-tool = get_pack("author/repo_name/pack_name").tool
-
-# Add the tool to the 'tools' argument when instantiating your AgentExecutor
-agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=[tool()])
-```
+For detailed examples and more information, refer to
+the [AutoPack documentation](https://github.com/AutoPackAI/autopack/wiki).
 
-### Using with Auto-GPT
+## Safety and Security Notice
 
-We are actively working on improving the integration with Auto-GPT. Stay tuned for updates!
+Please exercise caution when using the AutoPack repository and library. The repository and library are currently in the
+early stages and intended for research purposes only. Ensure you review the Packs you install as they are directly
+cloned from GitHub. AutoPack and its maintainers are not liable for any misuse or negligence regarding the repository
+and library.
 
-To use `autopack` with Auto-GPT, you can edit the file `autogpt/main.py` and add `autopack` to the `COMMAND_CATEGORIES`
-list.
+For more details, please refer to
+the [Safety and Security section](https://github.com/AutoPackAI/autopack/wiki#safety-and-security-notice) in the
+documentation.
 
-## TODOs
+## Contributing
 
-This project is still in its early stages, and there are several features and enhancements that need to be implemented.
-If you are interested and willing to contribute, the following list provides a good starting point:
+We welcome contributions to the AutoPack ecosystem. Here are some ways you can help:
 
-- Tool search functionality within the CLI
-- Tool search capability from Python
-- Optional automatic pack installation in the `get_pack` function
-- Tools for Agents to independently search for, install, and utilize other Tools
-- Tool for utilizing the pack selection API of the AutoPack repository
-- Optional contribution of feedback back to the AutoPack repository
+- **Create new tools!** Expand the AutoPack repository by developing and submitting your own tools. Share your ideas and
+  solutions with the AutoPack community.
+- **Submit GitHub repos**: If you come across GitHub repositories containing useful tools, submit them to
+  the [AutoPack repository](https://autopack.ai/submissions). We'll create Packs out of the tools in those repositories
+  by providing the necessary metadata.
+- **Try it out for yourself**: Test AutoPack in your projects and provide feedback. Share your experiences, report bugs,
+  and suggest improvements by opening issues on GitHub.
+- **Contribute code**: Help improve AutoPack by opening pull requests. You can choose to work on unresolved issues or
+  implement new features that you believe would enhance the functionality of the library. Please note that the AutoPack
+  library is intentionally designed to be compact and straightforward.
 
-## Development
+We appreciate your contributions and look forward to your involvement in making AutoPack a vibrant and valuable resource
+for the autonomous AI community.
 
-For information on how to contribute to AutoPack, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+## License
 
-Feel free to modify this README to provide more specific details about your project and its functionalities.
+AutoPack is released under the [MIT License](https://opensource.org/licenses/MIT).
```

