# Comparing `tmp/flux-local-2.0.0.tar.gz` & `tmp/flux-local-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-2.0.0.tar", last modified: Sat Jul  1 18:49:40 2023, max compression
+gzip compressed data, was "flux-local-2.0.1.tar", last modified: Sat Jul  1 22:28:37 2023, max compression
```

## Comparing `flux-local-2.0.0.tar` & `flux-local-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 18:49:30.000000 flux-local-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 18:49:40.254690 flux-local-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-01 18:49:30.000000 flux-local-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.250690 flux-local-2.0.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.250690 flux-local-2.0.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-01 18:49:40.254690 flux-local-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 18:49:30.000000 flux-local-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 22:28:23.000000 flux-local-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 22:28:37.262033 flux-local-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-01 22:28:23.000000 flux-local-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.258033 flux-local-2.0.1/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-01 22:28:23.000000 flux-local-2.0.1/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 22:28:37.000000 flux-local-2.0.1/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-01 22:28:37.262033 flux-local-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 22:28:23.000000 flux-local-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 22:28:37.262033 flux-local-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-01 22:28:23.000000 flux-local-2.0.1/tests/test_manifest.py
```

### Comparing `flux-local-2.0.0/LICENSE` & `flux-local-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/PKG-INFO` & `flux-local-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 2.0.0
+Version: 2.0.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-2.0.0/README.md` & `flux-local-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/command.py` & `flux-local-2.0.1/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/exceptions.py` & `flux-local-2.0.1/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/git_repo.py` & `flux-local-2.0.1/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/helm.py` & `flux-local-2.0.1/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/kustomize.py` & `flux-local-2.0.1/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/manifest.py` & `flux-local-2.0.1/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/build.py` & `flux-local-2.0.1/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/diff.py` & `flux-local-2.0.1/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/flux_local.py` & `flux-local-2.0.1/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/format.py` & `flux-local-2.0.1/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/get.py` & `flux-local-2.0.1/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/selector.py` & `flux-local-2.0.1/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local/tool/test.py` & `flux-local-2.0.1/flux_local/tool/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,16 +385,14 @@
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         enable_helm: bool,
         enable_kyverno: bool,
         test_path: str | None,
         verbosity: int,
-        kube_version: str | None,
-        api_versions: str | None,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_cluster_selector(**kwargs)
         if test_path:
             parts = test_path.split("::")
             query.path.path = Path(parts[0])
```

### Comparing `flux-local-2.0.0/flux_local/tool/visitor.py` & `flux-local-2.0.1/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/flux_local.egg-info/PKG-INFO` & `flux-local-2.0.1/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 2.0.0
+Version: 2.0.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-2.0.0/flux_local.egg-info/SOURCES.txt` & `flux-local-2.0.1/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/setup.cfg` & `flux-local-2.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 2.0.0
+version = 2.0.1
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-2.0.0/tests/test_command.py` & `flux-local-2.0.1/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/tests/test_git_repo.py` & `flux-local-2.0.1/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/tests/test_helm.py` & `flux-local-2.0.1/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/tests/test_kustomize.py` & `flux-local-2.0.1/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-2.0.0/tests/test_manifest.py` & `flux-local-2.0.1/tests/test_manifest.py`

 * *Files identical despite different names*

