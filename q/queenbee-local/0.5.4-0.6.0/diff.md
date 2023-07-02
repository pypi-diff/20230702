# Comparing `tmp/queenbee-local-0.5.4.tar.gz` & `tmp/queenbee-local-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/queenbee-local-0.5.4.tar", last modified: Sun May  7 02:10:30 2023, max compression
+gzip compressed data, was "dist/queenbee-local-0.6.0.tar", last modified: Sun Jul  2 20:22:47 2023, max compression
```

## Comparing `queenbee-local-0.5.4.tar` & `queenbee-local-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local/
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local/
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/setup.py
```

### Comparing `queenbee-local-0.5.4/.github/workflows/ci.yaml` & `queenbee-local-0.6.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/LICENSE` & `queenbee-local-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/PKG-INFO` & `queenbee-local-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.4
+Version: 0.6.0
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.4/docs/conf.py` & `queenbee-local-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/queenbee_local/__init__.py` & `queenbee-local-0.6.0/queenbee_local/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import time
 import shutil
 import tempfile
 import platform
 import json
 import warnings
+import re
 from datetime import datetime, timedelta
 
 import luigi
 
 # importing all the methods to make it easy for the extensions to grab them all from here
 from .helper import parse_input_args, to_snake_case, update_params, _change_permission, \
     _copy_artifacts, to_camel_case, tab_forward
@@ -144,14 +145,40 @@
 
         Overwrite this method.
         """
         raise NotImplementedError(
             'Command method must be overwritten in every subclass.'
         )
 
+    def _copy_script(self, dst):
+        """Render and copy the template script to dst folder.
+
+        Args:
+            dst: Execution folder.
+        """
+        logger = self.get_interface_logger()
+        logger.info(f"{self.__class__.__name__}: started copying script.")
+        script_file = self.__script__
+        data = {
+            f'inputs.{k.replace("_", "-")}': v
+            for k, v in self.input_parameters.items()
+        }
+        pattern = r'[^{\{]+(?=}\})'
+        script_content = script_file.read_text()
+        matches = re.finditer(pattern, script_content, re.MULTILINE)
+        for match in matches:
+            place_holder = match.group()
+            script_content = script_content.replace(
+                f'{{{{{place_holder}}}}}', str(data[place_holder.strip()])
+            )
+        out_file = pathlib.Path(dst, '__scripts__', 'script.py')
+        out_file.parent.mkdir(mode=0o777, parents=True, exist_ok=True)
+        out_file.write_text(script_content)
+        logger.info(f"{self.__class__.__name__}: finished copying script.")
+
     def _copy_input_artifacts(self, dst):
         """Copy input artifacts to destination folder.
 
         Args:
             dst: Execution folder.
         """
         logger = self.get_interface_logger()
@@ -290,14 +317,17 @@
             command = command.replace('"', '\'')
 
         cur_dir = os.getcwd()
         dst_dir, dst = self._get_dst_folder(command)
         os.chdir(dst)
 
         self._copy_input_artifacts(dst)
+        if self.is_script:
+            self._copy_script(dst)
+
         logger.info(f'Started running {self.__class__.__name__}...')
         qb_logger.info(f'Started running {self.__class__.__name__}...')
         self._update_status(logger=qb_logger, started=True)
 
         # TODO: offer an option for podman
         if self._run_inside_container:
             dst_path = pathlib.Path(dst)
```

### Comparing `queenbee-local-0.5.4/queenbee_local/cli.py` & `queenbee-local-0.6.0/queenbee_local/cli.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/queenbee_local/helper.py` & `queenbee-local-0.6.0/queenbee_local/helper.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/queenbee_local.egg-info/PKG-INFO` & `queenbee-local-0.6.0/queenbee_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.4
+Version: 0.6.0
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.4/queenbee_local.egg-info/SOURCES.txt` & `queenbee-local-0.6.0/queenbee_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.4/setup.py` & `queenbee-local-0.6.0/setup.py`

 * *Files identical despite different names*

