# Comparing `tmp/giteasy-9.4.0.tar.gz` & `tmp/giteasy-9.5.0.tar.gz`

## Comparing `giteasy-9.4.0.tar` & `giteasy-9.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 giteasy-9.4.0/.gitattributes
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 giteasy-9.4.0/src/giteasy/__init__.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 giteasy-9.4.0/src/giteasy/github_releases.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 giteasy-9.4.0/src/giteasy/github_repo.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 giteasy-9.4.0/src/giteasy/githubb.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 giteasy-9.4.0/tests/t_github.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 giteasy-9.4.0/tests/t_github_releases.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 giteasy-9.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 giteasy-9.4.0/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 giteasy-9.4.0/README.md
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 giteasy-9.4.0/pyproject.toml
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 giteasy-9.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 giteasy-9.5.0/.gitattributes
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 giteasy-9.5.0/src/giteasy/__init__.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 giteasy-9.5.0/src/giteasy/github_releases.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 giteasy-9.5.0/src/giteasy/github_repo.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 giteasy-9.5.0/src/giteasy/githubb.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 giteasy-9.5.0/tests/t_github.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 giteasy-9.5.0/tests/t_github_releases.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 giteasy-9.5.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 giteasy-9.5.0/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 giteasy-9.5.0/README.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 giteasy-9.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 giteasy-9.5.0/PKG-INFO
```

### Comparing `giteasy-9.4.0/src/giteasy/github_releases.py` & `giteasy-9.5.0/src/giteasy/github_releases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 
     """
 
 import re
 from pathlib import Path
+import tarfile
 
 import requests
 from mirutil.files import write_to_file
 from mirutil.files import untar_to
 
 from .github_repo import GitHubRepo
 
@@ -39,16 +40,19 @@
         local_path = Path.cwd()
     fp = Path(local_path) / fn
 
     write_to_file(r.content , fp , 'wb')
 
     return fp
 
+def get_dirname_fr_github_tarball(fp) :
+    with tarfile.open(fp) as tar :
+        return tar.getnames()[0]
+
 def download_latest_release_of_public_github_repo(repo_url ,
                                                   local_path = None) :
     tar_fp = download_latest_release_tarball_of_a_public_github_repo(repo_url ,
                                                                      local_path)
     untar_to(tar_fp , tar_fp.parent)
+    dirp = tar_fp.parent / get_dirname_fr_github_tarball(tar_fp)
     tar_fp.unlink()
-    dirn = tar_fp.name.split('.tar.gz')[0]
-    dirp = tar_fp.parent / dirn
     return dirp
```

### Comparing `giteasy-9.4.0/src/giteasy/github_repo.py` & `giteasy-9.5.0/src/giteasy/github_repo.py`

 * *Files identical despite different names*

### Comparing `giteasy-9.4.0/src/giteasy/githubb.py` & `giteasy-9.5.0/src/giteasy/githubb.py`

 * *Files identical despite different names*

### Comparing `giteasy-9.4.0/tests/t_github.py` & `giteasy-9.5.0/tests/t_github.py`

 * *Files identical despite different names*

### Comparing `giteasy-9.4.0/.gitignore` & `giteasy-9.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `giteasy-9.4.0/LICENSE` & `giteasy-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giteasy-9.4.0/pyproject.toml` & `giteasy-9.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "giteasy"
-version = "9.4.0"
+version = "9.5.0"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "A simple tool to get last/full version of a github repository and committing back to it"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
     "dulwich",
     "PyGithub",
```

### Comparing `giteasy-9.4.0/PKG-INFO` & `giteasy-9.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giteasy
-Version: 9.4.0
+Version: 9.5.0
 Summary: A simple tool to get last/full version of a github repository and committing back to it
 Project-URL: Homepage, https://github.com/imahdimir/giteasy
 Project-URL: Bug Tracker, https://github.com/imahdimir/giteasy/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

