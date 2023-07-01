# Comparing `tmp/universal_test_runner-0.3.0.tar.gz` & `tmp/universal_test_runner-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_test_runner-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "universal_test_runner-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `universal_test_runner-0.3.0.tar` & `universal_test_runner-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.3.0/LICENSE
--rw-r--r--   0        0        0     4145 2023-06-20 00:04:36.575042 universal_test_runner-0.3.0/README.md
--rw-r--r--   0        0        0     1306 2023-06-20 07:30:24.762970 universal_test_runner-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.3.0/universal_test_runner/__init__.py
--rw-r--r--   0        0        0      628 2023-06-19 22:38:42.426279 universal_test_runner-0.3.0/universal_test_runner/cli.py
--rw-r--r--   0        0        0     1784 2023-06-19 22:41:04.042871 universal_test_runner-0.3.0/universal_test_runner/context.py
--rw-r--r--   0        0        0     3559 2023-06-20 07:19:47.780665 universal_test_runner-0.3.0/universal_test_runner/matchers.py
--rw-r--r--   0        0        0      812 2023-06-19 22:38:32.764857 universal_test_runner-0.3.0/universal_test_runner/runner.py
--rw-r--r--   0        0        0     5301 1970-01-01 00:00:00.000000 universal_test_runner-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7088 2023-06-29 02:00:26.259769 universal_test_runner-0.4.0/README.md
+-rw-r--r--   0        0        0     1364 2023-07-01 23:10:25.755823 universal_test_runner-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.4.0/universal_test_runner/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-19 22:38:42.426279 universal_test_runner-0.4.0/universal_test_runner/cli.py
+-rw-r--r--   0        0        0     1791 2023-07-01 23:05:16.489107 universal_test_runner-0.4.0/universal_test_runner/context.py
+-rw-r--r--   0        0        0     4996 2023-07-01 23:05:13.811691 universal_test_runner-0.4.0/universal_test_runner/matchers.py
+-rw-r--r--   0        0        0     1027 2023-06-28 03:19:59.457422 universal_test_runner-0.4.0/universal_test_runner/runner.py
+-rw-r--r--   0        0        0     8381 1970-01-01 00:00:00.000000 universal_test_runner-0.4.0/PKG-INFO
```

### Comparing `universal_test_runner-0.3.0/LICENSE` & `universal_test_runner-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.3.0/pyproject.toml` & `universal_test_runner-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [project]
 name = "universal-test-runner"
-version = "0.3.0"
+version = "0.4.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Universal, language-aware unit test runner."
 readme = "README.md"
 license = { file = "LICENSE" }
 
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Testing",
 ]
 keywords = ["testing", "test-runner", "pytest"]
 
-dependencies = ["click==8.1.3"]
+dependencies = ["click==8.1.3", "colorama==0.4.6"]
 
 [project.optional-dependencies]
-test = ["pytest==7.3.1", "responses==0.23.1", "pyright==1.1.309"]
+test = ["pytest==7.3.1", "responses==0.23.1"]
 release = ["twine==4.0.2", "build==0.10.0"]
+ci = ["black==23.3.0", "isort==5.12.0", "pyright==1.1.309"]
 
 [project.urls]
 "Homepage" = "https://github.com/xavdid/universal-test-runner"
 "Bug Tracker" = "https://github.com/xavdid/universal-test-runner/issues"
 "Author" = "https://xavd.id"
 "Changelog" = "https://github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md"
```

### Comparing `universal_test_runner-0.3.0/universal_test_runner/cli.py` & `universal_test_runner-0.4.0/universal_test_runner/cli.py`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.3.0/universal_test_runner/context.py` & `universal_test_runner-0.4.0/universal_test_runner/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         used by the CLI to auto-capture info about the working directory
         """
         return Context.build(os.getcwd(), sys.argv[1:], debugging=debugging)
 
     @cache
     def _load_file(self, filename: str) -> str:
-        return Path(self.cwd, filename).read_text()
+        return Path(self.cwd, filename).read_text("utf-8")
 
     def read_file(self, filename: str) -> list[str]:
         return self._load_file(filename).splitlines()
 
     def read_json(self, filename: str):
         return json.loads(self._load_file(filename))
```

