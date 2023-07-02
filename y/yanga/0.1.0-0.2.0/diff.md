# Comparing `tmp/yanga-0.1.0.tar.gz` & `tmp/yanga-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.1.0.tar", max compression
+gzip compressed data, was "yanga-0.2.0.tar", max compression
```

## Comparing `yanga-0.1.0.tar` & `yanga-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-06 19:55:55.683953 yanga-0.1.0/LICENSE
--rw-r--r--   0        0        0     4695 2023-06-06 19:55:55.683953 yanga-0.1.0/README.md
--rw-r--r--   0        0        0     2309 2023-06-06 19:55:56.635954 yanga-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-06 19:55:56.587954 yanga-0.1.0/src/yanga/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     3052 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0     1583 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/spl/__init__.py
--rw-r--r--   0        0        0      886 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/spl/variant.py
--rw-r--r--   0        0        0      686 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/ybuild.py
--rw-r--r--   0        0        0      683 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/yinit.py
--rw-r--r--   0        0        0      635 2023-06-06 19:55:55.687953 yanga-0.1.0/src/yanga/ymain.py
--rw-r--r--   0        0        0     5807 1970-01-01 00:00:00.000000 yanga-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-02 16:31:02.263059 yanga-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-02 16:31:02.263059 yanga-0.2.0/README.md
+-rw-r--r--   0        0        0     2384 2023-07-02 16:31:03.239069 yanga-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-02 16:31:03.203068 yanga-0.2.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2298 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0      412 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0        7 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5312 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
+-rw-r--r--   0        0        0     3876 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0      157 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
+-rw-r--r--   0        0        0       34 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4221 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/logger.py
+-rw-r--r--   0        0        0     2910 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1349 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     3141 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0      670 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-02 16:31:02.267059 yanga-0.2.0/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0      857 2023-07-02 16:31:02.271059 yanga-0.2.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.2.0/PKG-INFO
```

### Comparing `yanga-0.1.0/LICENSE` & `yanga-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.1.0/README.md` & `yanga-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.1.0/pyproject.toml` & `yanga-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.1.0"
+version = "0.2.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
@@ -14,22 +14,26 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "yanga", from = "src" },
 ]
 
+[tool.poetry.scripts]
+yanga = "yanga.ymain:main"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cuinixam/yanga/issues"
 "Changelog" = "https://github.com/cuinixam/yanga/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 mashumaro = "^3.5"
 loguru = "^0.7.0"
+cookiecutter = "^2.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 black = "^23.1.0"
 pre-commit = "^3.1.1"
```

### Comparing `yanga-0.1.0/src/yanga/core/docs_utils.py` & `yanga-0.2.0/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.1.0/src/yanga/core/logger.py` & `yanga-0.2.0/src/yanga/core/logger.py`

 * *Files identical despite different names*

### Comparing `yanga-0.1.0/src/yanga/spl/variant.py` & `yanga-0.2.0/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.1.0/src/yanga/ymain.py` & `yanga-0.2.0/src/yanga/ymain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+import sys
 from pathlib import Path
 from sys import argv
 
+from yanga.commands.build import BuildCommand
+from yanga.commands.init import InitCommand
 from yanga.core.cmd_line import CommandLineHandlerBuilder
+from yanga.core.exceptions import UserNotificationException
 from yanga.core.logger import logger, setup_logger, time_it
-from yanga.ybuild import BuildCommand
-from yanga.yinit import InitCommand
 
 
 @time_it()
 def do_run() -> None:
     logger.debug("Starting yanga")
     builder = CommandLineHandlerBuilder()
     builder.add_command(BuildCommand()).add_command(InitCommand())
     handler = builder.create()
     handler.run(argv[1:])
 
 
-def main() -> None:
-    setup_logger(Path(".yanga/logs/yanga.log"), clear=True)
-    do_run()
+def main() -> int:
+    try:
+        setup_logger(Path(".yanga/logs/yanga.log"), clear=True)
+        do_run()
+    except UserNotificationException as e:
+        logger.error(f"{e}")
+        return 1
+    return 0
 
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

### Comparing `yanga-0.1.0/PKG-INFO` & `yanga-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.1.0
+Version: 0.2.0
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mashumaro (>=3.5,<4.0)
 Project-URL: Bug Tracker, https://github.com/cuinixam/yanga/issues
 Project-URL: Changelog, https://github.com/cuinixam/yanga/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://yanga.readthedocs.io
 Project-URL: Repository, https://github.com/cuinixam/yanga
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: yanga Version: 0.1.0 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.2.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
->=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: loguru
-(>=0.7.0,<0.8.0) Requires-Dist: mashumaro (>=3.5,<4.0) Project-URL: Bug
-Tracker, https://github.com/cuinixam/yanga/issues Project-URL: Changelog,
-https://github.com/cuinixam/yanga/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://yanga.readthedocs.io Project-URL: Repository, https://
-github.com/cuinixam/yanga Description-Content-Type: text/markdown # README
+>=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: cookiecutter (>=2.1.1,<3.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: mashumaro (>=3.5,<4.0) Project-URL: Bug Tracker, https://
+github.com/cuinixam/yanga/issues Project-URL: Changelog, https://github.com/
+cuinixam/yanga/blob/main/CHANGELOG.md Project-URL: Documentation, https://
+yanga.readthedocs.io Project-URL: Repository, https://github.com/cuinixam/yanga
+Description-Content-Type: text/markdown # README
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Yet another ninja generator to build C/CPP projects. ## Installation Install
 this via pip (or your favourite package manager): `pip install yanga` ## Start
 developing The project uses Poetry for dependencies management and packaging.
 If you do not have Poetry installed, you can run the `boostrap.ps1` script.
```

