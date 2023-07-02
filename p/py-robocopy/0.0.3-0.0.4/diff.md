# Comparing `tmp/py-robocopy-0.0.3.tar.gz` & `tmp/py-robocopy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-robocopy-0.0.3.tar", last modified: Sat Jul  1 20:46:42 2023, max compression
+gzip compressed data, was "py-robocopy-0.0.4.tar", last modified: Sun Jul  2 18:02:09 2023, max compression
```

## Comparing `py-robocopy-0.0.3.tar` & `py-robocopy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 20:46:42.030176 py-robocopy-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-01 14:23:24.000000 py-robocopy-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1701 2023-07-01 20:46:42.028175 py-robocopy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-01 20:40:10.000000 py-robocopy-0.0.3/README.md
--rw-rw-rw-   0        0        0      552 2023-07-01 20:43:50.000000 py-robocopy-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 20:46:42.032178 py-robocopy-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 20:46:41.919683 py-robocopy-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 20:46:42.005227 py-robocopy-0.0.3/src/RoboCopy/
--rw-rw-rw-   0        0        0        0 2023-07-01 14:09:58.000000 py-robocopy-0.0.3/src/RoboCopy/__init__.py
--rw-rw-rw-   0        0        0      149 2023-07-01 19:35:16.000000 py-robocopy-0.0.3/src/RoboCopy/robocopy.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:46:42.019164 py-robocopy-0.0.3/src/py_robocopy.egg-info/
--rw-rw-rw-   0        0        0     1701 2023-07-01 20:46:41.000000 py-robocopy-0.0.3/src/py_robocopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-01 20:46:41.000000 py-robocopy-0.0.3/src/py_robocopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 20:46:41.000000 py-robocopy-0.0.3/src/py_robocopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 20:46:41.000000 py-robocopy-0.0.3/src/py_robocopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/py_robocopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/robocopy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/src/robocopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/src/robocopy/robocopy.py
```

### Comparing `py-robocopy-0.0.3/LICENSE` & `py-robocopy-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `py-robocopy-0.0.3/PKG-INFO` & `py-robocopy-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-Metadata-Version: 2.1
-Name: py-robocopy
-Version: 0.0.3
-Summary: Copies file data from one location to another.
-Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
-Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
-Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Package robocopy
-
-Copies file data from one location to another.
-
-## Usage
-### Import the library
-`pip install py-robocopy`
-
-## Syntax
-`robocopy <source> <destination> [<file>[ ...]] [<options>]`
-
-For example, to copy a file named yearly-report.mov from c:\reports to a file share \\marketing\videos while enabling multi-threading for higher performance (with the /mt parameter) and the ability to restart the transfer in case it's interrupted (with the /z parameter), type:
-`robocopy c:\reports "\\marketing\videos" yearly-report.mov /mt /z`
-
-For more details : https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
-
-## Parameters
-### Parameter	Description
-- `<source>`	Specifies the path to the source directory.
-- `<destination>`	Specifies the path to the destination directory.
-- `<file>`	Specifies the file or files to be copied. Wildcard characters (* or ?) are supported. If you don't specify this parameter, *.* is used as the default value.
-- `<options>`	Specifies the options to use with the robocopy command, including copy, file, retry, logging, and job options.
-
+Metadata-Version: 2.1
+Name: py-robocopy
+Version: 0.0.4
+Summary: Copies file data from one location to another.
+Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
+Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
+Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Package robocopy
+
+Copies file data from one location to another.
+
+### Import the library
+`pip install py-robocopy`
+
+## Usage
+
+`from RoboCopy import robocopy`
+
+`robocopy.copy(<source-file-path>,<destination-file-path>)`
+
+## Syntax
+`robocopy <source> <destination> [<file>[ ...]] [<options>]`
+
+For example, to copy a file named yearly-report.mov from c:\reports to a file share \\marketing\videos while enabling multi-threading for higher performance (with the /mt parameter) and the ability to restart the transfer in case it's interrupted (with the /z parameter), type:
+`robocopy c:\reports "\\marketing\videos" yearly-report.mov /mt /z`
+
+For more details : https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
+
+## Parameters
+### Parameter	Description
+- `<source>`	Specifies the path to the source directory.
+- `<destination>`	Specifies the path to the destination directory.
+- `<file>`	Specifies the file or files to be copied. Wildcard characters (* or ?) are supported. If you don't specify this parameter, *.* is used as the default value.
+- `<options>`	Specifies the options to use with the robocopy command, including copy, file, retry, logging, and job options.
+
```

### Comparing `py-robocopy-0.0.3/README.md` & `py-robocopy-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Package robocopy
 
 Copies file data from one location to another.
 
-## Usage
 ### Import the library
 `pip install py-robocopy`
 
+## Usage
+
+`from RoboCopy import robocopy`
+
+`robocopy.copy(<source-file-path>,<destination-file-path>)`
+
 ## Syntax
 `robocopy <source> <destination> [<file>[ ...]] [<options>]`
 
 For example, to copy a file named yearly-report.mov from c:\reports to a file share \\marketing\videos while enabling multi-threading for higher performance (with the /mt parameter) and the ability to restart the transfer in case it's interrupted (with the /z parameter), type:
 `robocopy c:\reports "\\marketing\videos" yearly-report.mov /mt /z`
 
 For more details : https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
```

### Comparing `py-robocopy-0.0.3/pyproject.toml` & `py-robocopy-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-[project]
-name = "py-robocopy"
-version = "0.0.3"
-authors = [
-  { name="Suyash Sonkesaria", email="suyashsonkesaria@gmail.com" },
-]
-description = "Copies file data from one location to another."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/suyashsonkesaria/robocopy"
+[project]
+name = "py-robocopy"
+version = "0.0.4"
+authors = [
+  { name="Suyash Sonkesaria", email="suyashsonkesaria@gmail.com" },
+]
+description = "Copies file data from one location to another."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/suyashsonkesaria/robocopy"
 "Bug Tracker" = "https://github.com/suyashsonkesaria/robocopy/issues"
```

### Comparing `py-robocopy-0.0.3/src/py_robocopy.egg-info/PKG-INFO` & `py-robocopy-0.0.4/src/py_robocopy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-Metadata-Version: 2.1
-Name: py-robocopy
-Version: 0.0.3
-Summary: Copies file data from one location to another.
-Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
-Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
-Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Package robocopy
-
-Copies file data from one location to another.
-
-## Usage
-### Import the library
-`pip install py-robocopy`
-
-## Syntax
-`robocopy <source> <destination> [<file>[ ...]] [<options>]`
-
-For example, to copy a file named yearly-report.mov from c:\reports to a file share \\marketing\videos while enabling multi-threading for higher performance (with the /mt parameter) and the ability to restart the transfer in case it's interrupted (with the /z parameter), type:
-`robocopy c:\reports "\\marketing\videos" yearly-report.mov /mt /z`
-
-For more details : https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
-
-## Parameters
-### Parameter	Description
-- `<source>`	Specifies the path to the source directory.
-- `<destination>`	Specifies the path to the destination directory.
-- `<file>`	Specifies the file or files to be copied. Wildcard characters (* or ?) are supported. If you don't specify this parameter, *.* is used as the default value.
-- `<options>`	Specifies the options to use with the robocopy command, including copy, file, retry, logging, and job options.
-
+Metadata-Version: 2.1
+Name: py-robocopy
+Version: 0.0.4
+Summary: Copies file data from one location to another.
+Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
+Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
+Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Package robocopy
+
+Copies file data from one location to another.
+
+### Import the library
+`pip install py-robocopy`
+
+## Usage
+
+`from RoboCopy import robocopy`
+
+`robocopy.copy(<source-file-path>,<destination-file-path>)`
+
+## Syntax
+`robocopy <source> <destination> [<file>[ ...]] [<options>]`
+
+For example, to copy a file named yearly-report.mov from c:\reports to a file share \\marketing\videos while enabling multi-threading for higher performance (with the /mt parameter) and the ability to restart the transfer in case it's interrupted (with the /z parameter), type:
+`robocopy c:\reports "\\marketing\videos" yearly-report.mov /mt /z`
+
+For more details : https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy
+
+## Parameters
+### Parameter	Description
+- `<source>`	Specifies the path to the source directory.
+- `<destination>`	Specifies the path to the destination directory.
+- `<file>`	Specifies the file or files to be copied. Wildcard characters (* or ?) are supported. If you don't specify this parameter, *.* is used as the default value.
+- `<options>`	Specifies the options to use with the robocopy command, including copy, file, retry, logging, and job options.
+
```

