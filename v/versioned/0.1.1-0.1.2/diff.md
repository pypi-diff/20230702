# Comparing `tmp/versioned-0.1.1.tar.gz` & `tmp/versioned-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.1.1.tar", last modified: Sun Jul  2 07:05:15 2023, max compression
+gzip compressed data, was "versioned-0.1.2.tar", last modified: Sun Jul  2 18:26:46 2023, max compression
```

## Comparing `versioned-0.1.1.tar` & `versioned-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.927819 versioned-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3633 2023-07-02 07:05:15.927659 versioned-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2498 2023-07-02 06:36:26.000000 versioned-0.1.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1173 2023-07-02 06:43:09.000000 versioned-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-02 07:05:15.927971 versioned-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.921651 versioned-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      888 2023-07-02 07:01:56.000000 versioned-0.1.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9240 2023-07-02 07:03:16.000000 versioned-0.1.1/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.924994 versioned-0.1.1/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.1.1/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      639 2023-07-02 06:42:24.000000 versioned-0.1.1/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2037 2023-07-02 06:41:57.000000 versioned-0.1.1/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.1.1/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13206 2023-07-02 06:59:37.000000 versioned-0.1.1/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.925804 versioned-0.1.1/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3609 2023-07-02 06:42:16.000000 versioned-0.1.1/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.1.1/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.926530 versioned-0.1.1/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.1.1/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.927390 versioned-0.1.1/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.1.1/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.1.1/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 07:05:15.925691 versioned-0.1.1/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3633 2023-07-02 07:05:15.000000 versioned-0.1.1/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-02 07:05:15.000000 versioned-0.1.1/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-02 07:05:15.000000 versioned-0.1.1/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-02 07:05:15.000000 versioned-0.1.1/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-02 07:05:15.000000 versioned-0.1.1/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.226823 versioned-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-02 18:26:46.226667 versioned-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.1.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1674 2023-07-02 18:13:48.000000 versioned-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-02 18:26:46.226866 versioned-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.222532 versioned-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      928 2023-07-02 18:12:33.000000 versioned-0.1.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9398 2023-07-02 18:13:00.000000 versioned-0.1.2/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.224549 versioned-0.1.2/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.1.2/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-02 18:24:06.000000 versioned-0.1.2/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      681 2023-07-02 15:34:12.000000 versioned-0.1.2/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2037 2023-07-02 06:41:57.000000 versioned-0.1.2/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.1.2/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13257 2023-07-02 18:12:10.000000 versioned-0.1.2/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225291 versioned-0.1.2/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.1.2/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.1.2/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225812 versioned-0.1.2/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.1.2/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.226455 versioned-0.1.2/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.1.2/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225175 versioned-0.1.2/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.1.1/AUTHORS.rst` & `versioned-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/LICENSE.txt` & `versioned-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/PKG-INFO` & `versioned-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.1.1
+Version: 0.1.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -80,14 +80,18 @@
     :target: https://pypi.org/pypi/versioned#files
 
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
+Tutorial:
+
+- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.1.1/README.rst` & `versioned-0.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     :target: https://pypi.org/pypi/versioned#files
 
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
+Tutorial:
+
+- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.1.1/requirements-doc.txt` & `versioned-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/setup.py` & `versioned-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/tests/test_api.py` & `versioned-0.1.2/tests/test_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,27 @@
     _ = api.S3_PREFIX
     _ = api.LATEST_VERSION
     _ = api.VERSION_ZFILL
     _ = api.bootstrap
     _ = api.Artifact
     _ = api.Alias
     _ = api.put_artifact
-    _ = api.get_artifact
-    _ = api.list_artifacts
-    _ = api.publish_version
-    _ = api.delete_artifact
+    _ = api.get_artifact_version
+    _ = api.list_artifact_versions
+    _ = api.publish_artifact_version
+    _ = api.delete_artifact_version
     _ = api.put_alias
     _ = api.get_alias
     _ = api.list_aliases
     _ = api.delete_alias
-    _ = api.purge
+    _ = api.purge_artifact
     _ = api.Artifact.s3path
     _ = api.Artifact.get_content
     _ = api.Alias.s3path_version
     _ = api.Alias.get_version_content
-    _ = api.Alias.s3path_additional_version
-    _ = api.Alias.get_additional_version_content
+    _ = api.Alias.s3path_secondary_version
+    _ = api.Alias.get_secondary_version_content
 
 if __name__ == "__main__":
     from versioned.tests import run_cov_test
 
     run_cov_test(__file__, "versioned.api", preview=False)
```

### Comparing `versioned-0.1.1/tests/test_core.py` & `versioned-0.1.2/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from versioned import exc
 from versioned import constants
 from versioned.bootstrap import bootstrap
 from versioned.dynamodb import encode_version
 from versioned.tests.mock_aws import BaseMockTest
 from versioned.core import (
     put_artifact,
-    list_artifacts,
-    get_artifact,
-    publish_version,
-    delete_artifact,
+    list_artifact_versions,
+    get_artifact_version,
+    publish_artifact_version,
+    delete_artifact_version,
     put_alias,
     get_alias,
     list_aliases,
     delete_alias,
-    purge,
+    purge_artifact,
 )
 
 from rich import print as rprint
 
 
 class Test(BaseMockTest):
     use_mock = True
@@ -40,154 +40,154 @@
         context.attach_boto_session(cls.bsm.boto_ses)
         bootstrap(cls.bsm)
 
     def _test(self):
         name = "deploy"
         alias = "LIVE"
 
-        purge(bsm=self.bsm, name=name)
+        purge_artifact(bsm=self.bsm, name=name)
 
         # ======================================================================
         # Artifact
         # ======================================================================
         # --- test ArtifactNotFoundError ---
         # at this moment, no artifact exists
         with pytest.raises(exc.ArtifactNotFoundError):
-            publish_version(bsm=self.bsm, name=name)
+            publish_artifact_version(bsm=self.bsm, name=name)
 
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact(bsm=self.bsm, name=name)
+            get_artifact_version(bsm=self.bsm, name=name)
 
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
 
         # put artifact
         artifact = put_artifact(bsm=self.bsm, name=name, content=b"v1")
         # rprint(artifact)
 
         def _assert_artifact(artifact):
             assert artifact.name == name
             assert artifact.version == constants.LATEST_VERSION
             assert artifact.s3uri.endswith(constants.LATEST_VERSION)
             assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         _assert_artifact(artifact)
 
-        artifact = get_artifact(bsm=self.bsm, name=name)
+        artifact = get_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         _assert_artifact(artifact)
 
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         # rprint(artifact_list)
         assert len(artifact_list) == 1
         _assert_artifact(artifact_list[0])
 
-        artifact = publish_version(bsm=self.bsm, name=name)
+        artifact = publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "1"
         assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL))
         assert artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL)
         assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         # put artifact again
         artifact = put_artifact(bsm=self.bsm, name=name, content=b"v2")
         # rprint(artifact)
         assert artifact.version == constants.LATEST_VERSION
         assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
 
-        artifact = publish_version(bsm=self.bsm, name=name)
+        artifact = publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "2"
         s3path = S3Path(artifact.s3uri)
         assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL))
         assert artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL)
         assert artifact.get_content(bsm=self.bsm) == b"v2"
 
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 3
 
         # ======================================================================
         # Artifact
         # ======================================================================
         # --- test raises error ---
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
             put_alias(bsm=self.bsm, name=name, alias=alias, version=999)
 
-        # additional_version_weight type is wrong
+        # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
-            put_alias(bsm=self.bsm, name=name, alias=alias, additional_version=999)
+            put_alias(bsm=self.bsm, name=name, alias=alias, secondary_version=999)
 
-        # additional_version_weight type is wrong
+        # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
             put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
-                additional_version=999,
-                additional_version_weight=0.5,
+                secondary_version=999,
+                secondary_version_weight=0.5,
             )
 
-        # additional_version_weight value range is wrong
+        # secondary_version_weight value range is wrong
         with pytest.raises(ValueError):
             put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
-                additional_version=999,
-                additional_version_weight=-100,
+                secondary_version=999,
+                secondary_version_weight=-100,
             )
 
-        # additional_version_weight value range is wrong
+        # secondary_version_weight value range is wrong
         with pytest.raises(ValueError):
             put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
-                additional_version=999,
-                additional_version_weight=999,
+                secondary_version=999,
+                secondary_version_weight=999,
             )
 
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
             put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
-                additional_version=999,
-                additional_version_weight=20,
+                secondary_version=999,
+                secondary_version_weight=20,
             )
 
-        # version and additional_version is the same
+        # version and secondary_version is the same
         with pytest.raises(ValueError):
             put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 version=1,
-                additional_version=1,
-                additional_version_weight=20,
+                secondary_version=1,
+                secondary_version_weight=20,
             )
 
         # alias not exists
         with pytest.raises(exc.AliasNotFoundError):
             get_alias(bsm=self.bsm, name=name, alias="Invalid")
 
         # put alias
         ali = put_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
             assert ali.version == constants.LATEST_VERSION
-            assert ali.additional_version is None
-            assert ali.additional_version_weight is None
+            assert ali.secondary_version is None
+            assert ali.secondary_version_weight is None
             assert ali.version_s3uri.endswith(constants.LATEST_VERSION)
-            assert ali.additional_version_s3uri is None
+            assert ali.secondary_version_s3uri is None
             assert ali.get_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
         ali = get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
         _assert_alias(ali)
@@ -198,29 +198,29 @@
 
         # put alias again
         ali = put_alias(
             bsm=self.bsm,
             name=name,
             alias=alias,
             version=1,
-            additional_version=2,
-            additional_version_weight=20,
+            secondary_version=2,
+            secondary_version_weight=20,
         )
         # rprint(ali)
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
             assert ali.version == "1"
-            assert ali.additional_version == "2"
-            assert ali.additional_version_weight == 20
+            assert ali.secondary_version == "2"
+            assert ali.secondary_version_weight == 20
             assert ali.version_s3uri.endswith(encode_version(1))
-            assert ali.additional_version_s3uri.endswith(encode_version(2))
+            assert ali.secondary_version_s3uri.endswith(encode_version(2))
             assert ali.get_version_content(bsm=self.bsm) == b"v1"
-            assert ali.get_additional_version_content(bsm=self.bsm) == b"v2"
+            assert ali.get_secondary_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
         ali = get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
         _assert_alias(ali)
 
@@ -231,40 +231,40 @@
         # --- test delete methods
         delete_alias(bsm=self.bsm, name=name, alias=alias)
         with pytest.raises(exc.AliasNotFoundError):
             get_alias(bsm=self.bsm, name=name, alias=alias)
         ali_list = list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 0
 
-        delete_artifact(bsm=self.bsm, name=name)
+        delete_artifact_version(bsm=self.bsm, name=name)
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact(bsm=self.bsm, name=name)
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+            get_artifact_version(bsm=self.bsm, name=name)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 2
 
-        delete_artifact(bsm=self.bsm, name=name, version=1)
+        delete_artifact_version(bsm=self.bsm, name=name, version=1)
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact(bsm=self.bsm, name=name, version=1)
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+            get_artifact_version(bsm=self.bsm, name=name, version=1)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 1
 
         # it is a soft delete, so S3 artifact is not deleted
         assert s3path.parent.count_objects(bsm=self.bsm) == 3
 
         # --- purge
         with pytest.raises(exc.ArtifactNotFoundError):
             put_alias(bsm=self.bsm, name=name, alias="DEV", version=1)
 
         put_alias(bsm=self.bsm, name=name, alias="DEV", version=2)
         ali_list = list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 1
 
-        purge(bsm=self.bsm, name=name)
+        purge_artifact(bsm=self.bsm, name=name)
         assert s3path.parent.count_objects(bsm=self.bsm) == 0
-        artifact_list = list_artifacts(bsm=self.bsm, name=name)
+        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
         ali_list = list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 0
 
     def test(self):
         self._test()
```

### Comparing `versioned-0.1.1/versioned/api.py` & `versioned-0.1.2/versioned/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from .constants import S3_PREFIX
 from .constants import LATEST_VERSION
 from .constants import VERSION_ZFILL
 from .bootstrap import bootstrap
 from .core import Artifact
 from .core import Alias
 from .core import put_artifact
-from .core import get_artifact
-from .core import list_artifacts
-from .core import publish_version
-from .core import delete_artifact
+from .core import get_artifact_version
+from .core import list_artifact_versions
+from .core import publish_artifact_version
+from .core import delete_artifact_version
 from .core import put_alias
 from .core import get_alias
 from .core import list_aliases
 from .core import delete_alias
-from .core import purge
+from .core import purge_artifact
```

### Comparing `versioned-0.1.1/versioned/bootstrap.py` & `versioned-0.1.2/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/versioned/core.py` & `versioned-0.1.2/versioned/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,27 +52,27 @@
 class Alias:
     """
     Data class for alias.
 
     :param name: artifact name.
     :param alias: alias name. alias name cannot have hyphen
     :param version: artifact version. If ``None``, the latest version is used.
-    :param additional_version: see above.
-    :param additional_version_weight: an integer between 0 ~ 100.
+    :param secondary_version: see above.
+    :param secondary_version_weight: an integer between 0 ~ 100.
     :param version_s3uri: s3uri of the primary artifact version of this alias.
-    :param additional_version_s3uri: s3uri of the additional artifact version of this alias.
+    :param secondary_version_s3uri: s3uri of the secondary artifact version of this alias.
     """
 
     name: str
     alias: str
     version: str
-    additional_version: T.Optional[str]
-    additional_version_weight: T.Optional[int]
+    secondary_version: T.Optional[str]
+    secondary_version_weight: T.Optional[int]
     version_s3uri: str
-    additional_version_s3uri: T.Optional[str]
+    secondary_version_s3uri: T.Optional[str]
 
     @property
     def s3path_version(self) -> S3Path:
         """
         Return the s3path of the primary artifact version of this alias.
         """
         return S3Path(self.version_s3uri)
@@ -80,25 +80,25 @@
     def get_version_content(self, bsm: BotoSesManager) -> bytes:
         """
         Get the content of the primary artifact version of this alias.
         """
         return self.s3path_version.read_bytes(bsm=bsm)
 
     @property
-    def s3path_additional_version(self) -> S3Path:
+    def s3path_secondary_version(self) -> S3Path:
         """
-        Return the s3path of the additional artifact version of this alias.
+        Return the s3path of the secondary artifact version of this alias.
         """
-        return S3Path(self.additional_version_s3uri)
+        return S3Path(self.secondary_version_s3uri)
 
-    def get_additional_version_content(self, bsm: BotoSesManager) -> bytes:
+    def get_secondary_version_content(self, bsm: BotoSesManager) -> bytes:
         """
-        Get the content of the additional artifact version of this alias.
+        Get the content of the secondary artifact version of this alias.
         """
-        return self.s3path_additional_version.read_bytes(bsm=bsm)
+        return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
 
 def _get_artifact_class(bsm: BotoSesManager) -> T.Type[dynamodb.Artifact]:
     class Artifact(dynamodb.Artifact):
         class Meta:
             table_name = constants.DYNAMODB_TABLE_NAME
             region = bsm.aws_region
@@ -146,21 +146,21 @@
 ) -> Alias:
     dct = alias.to_dict()
     dct["version_s3uri"] = _get_s3path(
         bsm=bsm,
         name=alias.name,
         version=alias.version,
     ).uri
-    if alias.additional_version is None:
-        dct["additional_version_s3uri"] = None
+    if alias.secondary_version is None:
+        dct["secondary_version_s3uri"] = None
     else:
-        dct["additional_version_s3uri"] = _get_s3path(
+        dct["secondary_version_s3uri"] = _get_s3path(
             bsm=bsm,
             name=alias.name,
-            version=alias.additional_version,
+            version=alias.secondary_version,
         ).uri
     return Alias(**dct)
 
 
 # ------------------------------------------------------------------------------
 # Artifact
 # ------------------------------------------------------------------------------
@@ -206,15 +206,15 @@
         if artifact.is_deleted:
             raise exc.ArtifactNotFoundError(f"name = {name!r}, version = {version!r}")
         return artifact
     except artifact_class.DoesNotExist:
         raise exc.ArtifactNotFoundError(f"name = {name!r}, version = {version!r}")
 
 
-def get_artifact(
+def get_artifact_version(
     bsm: BotoSesManager,
     name: str,
     version: T.Optional[T.Union[int, str]] = None,
 ) -> Artifact:
     """
     Return the information about the artifact or artifact version.
 
@@ -225,15 +225,15 @@
     Artifact = _get_artifact_class(bsm)
     if version is None:
         version = constants.LATEST_VERSION
     artifact = _get_artifact_dynamodb_item(Artifact, name=name, version=version)
     return _get_artifact_dict(bsm=bsm, artifact=artifact)
 
 
-def list_artifacts(
+def list_artifact_versions(
     bsm: BotoSesManager,
     name: str,
 ) -> T.List[Artifact]:
     """
     Return a list of artifact versions. The latest version is always the first item.
     And the newer version comes first.
 
@@ -247,20 +247,20 @@
             hash_key=name,
             scan_index_forward=False,
             filter_condition=Artifact.is_deleted == False,
         )
     ]
 
 
-def publish_version(
+def publish_artifact_version(
     bsm: BotoSesManager,
     name: str,
 ) -> Artifact:
     """
-    Creates a version from the latest artifact. Use versions to create a
+    Creates a version from the latest artifact. Use versions to create an
     immutable snapshot of your latest artifact.
 
     :param bsm: ``boto_session_manager.BotoSesManager`` object.
     :param name: artifact name.
     """
     Artifact = _get_artifact_class(bsm)
     artifacts = list(Artifact.query(hash_key=name, scan_index_forward=False, limit=2))
@@ -275,15 +275,15 @@
     artifact.save()
     s3path_old = _get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
     s3path_new = _get_s3path(bsm=bsm, name=name, version=new_version)
     s3path_old.copy_to(s3path_new, bsm=bsm)
     return _get_artifact_dict(bsm=bsm, artifact=artifact)
 
 
-def delete_artifact(
+def delete_artifact_version(
     bsm: BotoSesManager,
     name: str,
     version: T.Optional[T.Union[int, str]] = None,
 ):
     """
     Deletes a specific version of artifact. If version is not specified,
     the latest version is deleted. Note that this is a soft delete,
@@ -309,57 +309,57 @@
 # Alias
 # ------------------------------------------------------------------------------
 def put_alias(
     bsm: BotoSesManager,
     name: str,
     alias: str,
     version: T.Optional[T.Union[int, str]] = None,
-    additional_version: T.Optional[T.Union[int, str]] = None,
-    additional_version_weight: T.Optional[int] = None,
+    secondary_version: T.Optional[T.Union[int, str]] = None,
+    secondary_version_weight: T.Optional[int] = None,
 ) -> Alias:
     """
     Creates an alias for an artifact version. If ``version`` is not specified,
     the latest version is used.
 
     You can also map an alias to split invocation requests between two versions.
-    Use the ``additional_version`` and ``additional_version_weight`` to specify
+    Use the ``secondary_version`` and ``secondary_version_weight`` to specify
     a second version and the percentage of invocation requests that it receives.
 
     :param bsm: ``boto_session_manager.BotoSesManager`` object.
     :param name: artifact name.
     :param alias: alias name. alias name cannot have hyphen
     :param version: artifact version. If ``None``, the latest version is used.
-    :param additional_version: see above.
-    :param additional_version_weight: an integer between 0 ~ 100.
+    :param secondary_version: see above.
+    :param secondary_version_weight: an integer between 0 ~ 100.
     """
     # validate argument
     if "-" in alias:  # pragma: no cover
         raise ValueError("alias cannot have hyphen")
 
-    if additional_version is not None:
-        if not isinstance(additional_version_weight, int):
-            raise TypeError("additional_version_weight must be int")
-        if not (0 <= additional_version_weight < 100):
-            raise ValueError("additional_version_weight must be 0 <= x < 100")
+    if secondary_version is not None:
+        if not isinstance(secondary_version_weight, int):
+            raise TypeError("secondary_version_weight must be int")
+        if not (0 <= secondary_version_weight < 100):
+            raise ValueError("secondary_version_weight must be 0 <= x < 100")
 
     # ensure the artifact exists
     Artifact = _get_artifact_class(bsm)
     if version is None:
         version = constants.LATEST_VERSION
     _get_artifact_dynamodb_item(Artifact, name=name, version=version)
-    if additional_version is not None:
-        _get_artifact_dynamodb_item(Artifact, name=name, version=additional_version)
+    if secondary_version is not None:
+        _get_artifact_dynamodb_item(Artifact, name=name, version=secondary_version)
 
     Alias = _get_alias_class(bsm)
     alias = Alias.new(
         name=name,
         alias=alias,
         version=version,
-        additional_version=additional_version,
-        additional_version_weight=additional_version_weight,
+        secondary_version=secondary_version,
+        secondary_version_weight=secondary_version_weight,
     )
 
     alias.save()
     return _get_alias_dict(bsm=bsm, alias=alias)
 
 
 def get_alias(
@@ -375,15 +375,15 @@
     :param alias: alias name. alias name cannot have hyphen
     """
     Alias = _get_alias_class(bsm)
     try:
         return _get_alias_dict(
             bsm=bsm,
             alias=Alias.get(
-                hash_key=f"__{name}-alias",
+                hash_key=dynamodb.encode_alias_key(name),
                 range_key=alias,
             ),
         )
     except Alias.DoesNotExist:
         raise exc.AliasNotFoundError(f"name = {name!r}, alias = {alias!r}")
 
 
@@ -396,15 +396,15 @@
 
     :param bsm: ``boto_session_manager.BotoSesManager`` object.
     :param name: artifact name.
     """
     Alias = _get_alias_class(bsm)
     return [
         _get_alias_dict(bsm=bsm, alias=alias)
-        for alias in Alias.query(hash_key=f"__{name}-alias")
+        for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name))
     ]
 
 
 def delete_alias(
     bsm: BotoSesManager,
     name: str,
     alias: str,
@@ -413,15 +413,15 @@
     Deletes an alias.
     """
     Alias = _get_alias_class(bsm)
     res = Alias.new(name=name, alias=alias).delete()
     # print(res)
 
 
-def purge(
+def purge_artifact(
     bsm: BotoSesManager,
     name: str,
 ):
     """
     Completely delete all artifacts and aliases of the given artifact name.
     This operation is irreversible. It will remove all related S3 artifacts
     and DynamoDB items.
@@ -435,9 +435,9 @@
 
     Artifact = _get_artifact_class(bsm)
     Alias = _get_alias_class(bsm)
     with Artifact.batch_write() as batch:
         for artifact in Artifact.query(hash_key=name):
             batch.delete(artifact)
     with Alias.batch_write() as batch:
-        for alias in Alias.query(hash_key=f"__{name}-alias"):
+        for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name)):
             batch.delete(alias)
```

### Comparing `versioned-0.1.1/versioned/paths.py` & `versioned-0.1.2/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/versioned/tests/mock_aws.py` & `versioned-0.1.2/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/versioned/vendor/hashes.py` & `versioned-0.1.2/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/versioned/vendor/pytest_cov_helper.py` & `versioned-0.1.2/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.1/versioned.egg-info/PKG-INFO` & `versioned-0.1.2/versioned.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.1.1
+Version: 0.1.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -80,14 +80,18 @@
     :target: https://pypi.org/pypi/versioned#files
 
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
+Tutorial:
+
+- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``versioned`` is released on PyPI, so all you need is to:
```

### Comparing `versioned-0.1.1/versioned.egg-info/SOURCES.txt` & `versioned-0.1.2/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

