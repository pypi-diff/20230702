# Comparing `tmp/katalytic_pkg-0.4.1.tar.gz` & `tmp/katalytic_pkg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_pkg-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_pkg-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_pkg-0.4.1.tar` & `katalytic_pkg-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic_pkg-0.4.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_pkg-0.4.1/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_pkg-0.4.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2564 2023-06-29 17:28:54.379685 katalytic_pkg-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic_pkg-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1537 2023-05-14 08:37:36.967341 katalytic_pkg-0.4.1/README.md
--rw-r--r--   0        0        0     1119 2023-06-29 17:28:54.379685 katalytic_pkg-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6150 2023-06-29 17:14:46.039481 katalytic_pkg-0.4.1/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2914 2023-06-29 17:26:02.006220 katalytic_pkg-0.4.1/tests/test_pkg.py
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 katalytic_pkg-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic_pkg-0.5.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_pkg-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_pkg-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2738 2023-07-02 15:49:27.315014 katalytic_pkg-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic_pkg-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1537 2023-05-14 08:37:36.967341 katalytic_pkg-0.5.0/README.md
+-rw-r--r--   0        0        0     1119 2023-07-02 15:49:27.315014 katalytic_pkg-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6351 2023-07-02 15:30:33.585191 katalytic_pkg-0.5.0/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2914 2023-06-29 17:26:02.006220 katalytic_pkg-0.5.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 katalytic_pkg-0.5.0/PKG-INFO
```

### Comparing `katalytic_pkg-0.4.1/.gitignore` & `katalytic_pkg-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_pkg-0.4.1/.gitlab-ci.yml` & `katalytic_pkg-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_pkg-0.4.1/CHANGELOG.md` & `katalytic_pkg-0.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.5.0 (2023-07-02)
+### feat
+- [[`b72a259`](https://gitlab.com/katalytic/katalytic-pkg/commit/b72a2599dfe824d12bf935c5b4200d235a775c39)] define class KatalyticInterrupt:
+
+
 ## 0.4.1 (2023-06-29)
 ### refactor
 - [[`eb5f392`](https://gitlab.com/katalytic/katalytic-pkg/commit/eb5f3921112948dd1c7e6c8c954e18e7907f6076)] rename get_functions_in_group() -> find_functions_marked_with()
 - [[`852af88`](https://gitlab.com/katalytic/katalytic-pkg/commit/852af883b95eb4a314750fbda2b4f58f862cbc07)] rename get_functions_in_group() -> find_functions_marked_with() --- See previous commit. I made this change because the merge commit will not trigger the rebuild
 
 
 ## 0.4.0 (2023-05-02)
```

### Comparing `katalytic_pkg-0.4.1/LICENSE.txt` & `katalytic_pkg-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_pkg-0.4.1/README.md` & `katalytic_pkg-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic_pkg-0.4.1/pyproject.toml` & `katalytic_pkg-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.4.1"
+version = "0.5.0"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_pkg-0.4.1/src/katalytic/pkg.py` & `katalytic_pkg-0.5.0/src/katalytic/pkg.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,21 @@
         for p2 in iglob(f'{p}/**.egg-info', recursive=True):
             if re.search(f'{pkg}-[^/]*[.]egg-info', p2):
                 yield p2
                 if Path(f'{p2}/PKG-INFO').is_file():
                     yield f'{p2}/PKG-INFO'
 
 
+class KatalyticInterrupt(Exception):
+    """
+    This exception is used in testing how code behaves when it gets interrupted.
+    I can catch all exceptions and re-raise if it's not this one
+    """
+
+
 def get_version(dunder_name):  # pragma: no cover -- I can't test all branches at the same time
     """
     Get the version information for a package.
 
     Args:
         dunder_name (str):
             The dunder name of the package (i.e., __name__).
```

### Comparing `katalytic_pkg-0.4.1/tests/test_pkg.py` & `katalytic_pkg-0.5.0/tests/test_pkg.py`

 * *Files identical despite different names*

### Comparing `katalytic_pkg-0.4.1/PKG-INFO` & `katalytic_pkg-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.4.1
+Version: 0.5.0
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

