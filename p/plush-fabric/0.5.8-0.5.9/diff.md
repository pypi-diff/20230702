# Comparing `tmp/plush-fabric-0.5.8.tar.gz` & `tmp/plush-fabric-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plush-fabric-0.5.8.tar", last modified: Tue Feb 28 21:14:58 2023, max compression
+gzip compressed data, was "plush-fabric-0.5.9.tar", last modified: Wed Apr  5 22:12:30 2023, max compression
```

## Comparing `plush-fabric-0.5.8.tar` & `plush-fabric-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 21:14:58.465911 plush-fabric-0.5.8/
--rw-rw-rw-   0        0        0     1088 2019-11-22 18:46:33.000000 plush-fabric-0.5.8/LICENSE.TXT
--rw-rw-rw-   0        0        0       40 2022-06-02 02:26:43.000000 plush-fabric-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2438 2023-02-28 21:14:58.465911 plush-fabric-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-06-02 02:26:43.000000 plush-fabric-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 21:14:58.414648 plush-fabric-0.5.8/plush/
--rw-rw-rw-   0        0        0        0 2017-05-24 00:51:53.000000 plush-fabric-0.5.8/plush/__init__.py
--rw-rw-rw-   0        0        0     1514 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/console.py
-drwxrwxrwx   0        0        0        0 2023-02-28 21:14:58.422768 plush-fabric-0.5.8/plush/fabric_commands/
--rw-rw-rw-   0        0        0     3148 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/fabric_commands/__init__.py
--rw-rw-rw-   0        0        0      615 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/fabric_commands/git.py
--rw-rw-rw-   0        0        0     1825 2023-01-03 04:13:04.000000 plush-fabric-0.5.8/plush/fabric_commands/permissions.py
--rw-rw-rw-   0        0        0      938 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/fabric_commands/ssh_key.py
--rw-rw-rw-   0        0        0     1989 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/oauth_flow.py
--rw-rw-rw-   0        0        0     1311 2022-06-01 22:10:39.000000 plush-fabric-0.5.8/plush/repo_keys.py
-drwxrwxrwx   0        0        0        0 2023-02-28 21:14:58.464610 plush-fabric-0.5.8/plush_fabric.egg-info/
--rw-rw-rw-   0        0        0     2438 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-28 21:14:58.000000 plush-fabric-0.5.8/plush_fabric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1207 2023-02-28 21:14:58.468451 plush-fabric-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-06-02 02:26:43.000000 plush-fabric-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.814624 plush-fabric-0.5.9/
+-rw-rw-rw-   0        0        0     1088 2019-11-22 18:46:33.000000 plush-fabric-0.5.9/LICENSE.TXT
+-rw-rw-rw-   0        0        0       40 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2438 2023-04-05 22:12:30.814624 plush-fabric-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1539 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.778824 plush-fabric-0.5.9/plush/
+-rw-rw-rw-   0        0        0        0 2017-05-24 00:51:53.000000 plush-fabric-0.5.9/plush/__init__.py
+-rw-rw-rw-   0        0        0     1514 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/console.py
+drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.784377 plush-fabric-0.5.9/plush/fabric_commands/
+-rw-rw-rw-   0        0        0     3148 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/__init__.py
+-rw-rw-rw-   0        0        0      615 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/git.py
+-rw-rw-rw-   0        0        0     1825 2023-01-03 04:13:04.000000 plush-fabric-0.5.9/plush/fabric_commands/permissions.py
+-rw-rw-rw-   0        0        0      938 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/ssh_key.py
+-rw-rw-rw-   0        0        0     1989 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/oauth_flow.py
+-rw-rw-rw-   0        0        0     1311 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/repo_keys.py
+drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.813624 plush-fabric-0.5.9/plush_fabric.egg-info/
+-rw-rw-rw-   0        0        0     2438 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1209 2023-04-05 22:12:30.816629 plush-fabric-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/setup.py
```

### Comparing `plush-fabric-0.5.8/LICENSE.TXT` & `plush-fabric-0.5.9/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/PKG-INFO` & `plush-fabric-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plush-fabric
-Version: 0.5.8
+Version: 0.5.9
 Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
 Home-page: https://github.com/kbarnes3/Plush
 Author: Kevin Barnes
 Author-email: kbarnes3@gmail.com
 Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
 Keywords: Fabric,GitHub,deployment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plush-fabric-0.5.8/README.md` & `plush-fabric-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/console.py` & `plush-fabric-0.5.9/plush/console.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/fabric_commands/__init__.py` & `plush-fabric-0.5.9/plush/fabric_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/fabric_commands/git.py` & `plush-fabric-0.5.9/plush/fabric_commands/git.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/fabric_commands/permissions.py` & `plush-fabric-0.5.9/plush/fabric_commands/permissions.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/fabric_commands/ssh_key.py` & `plush-fabric-0.5.9/plush/fabric_commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/oauth_flow.py` & `plush-fabric-0.5.9/plush/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush/repo_keys.py` & `plush-fabric-0.5.9/plush/repo_keys.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.8/plush_fabric.egg-info/PKG-INFO` & `plush-fabric-0.5.9/plush_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plush-fabric
-Version: 0.5.8
+Version: 0.5.9
 Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
 Home-page: https://github.com/kbarnes3/Plush
 Author: Kevin Barnes
 Author-email: kbarnes3@gmail.com
 Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
 Keywords: Fabric,GitHub,deployment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plush-fabric-0.5.8/setup.cfg` & `plush-fabric-0.5.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6c75 7368 2d66 6162 7269 630d   = plush-fabric.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e38  .version = 0.5.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e39  .version = 0.5.9
 00000030: 0d0a 6175 7468 6f72 203d 204b 6576 696e  ..author = Kevin
 00000040: 2042 6172 6e65 730d 0a61 7574 686f 725f   Barnes..author_
 00000050: 656d 6169 6c20 3d20 6b62 6172 6e65 7333  email = kbarnes3
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000070: 7269 7074 696f 6e20 3d20 4865 6c70 6572  ription = Helper
 00000080: 206c 6962 7261 7279 2066 6f72 2046 6162   library for Fab
 00000090: 7269 6320 746f 2073 696d 706c 6966 7920  ric to simplify 
@@ -49,28 +49,28 @@
 00000300: 636b 6167 6573 203d 200d 0a09 706c 7573  ckages = ...plus
 00000310: 680d 0a09 706c 7573 682e 6661 6272 6963  h...plush.fabric
 00000320: 5f63 6f6d 6d61 6e64 730d 0a70 7974 686f  _commands..pytho
 00000330: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
 00000340: 2e31 300d 0a69 6e73 7461 6c6c 5f72 6571  .10..install_req
 00000350: 7569 7265 7320 3d20 0d0a 096f 6175 7468  uires = ...oauth
 00000360: 3263 6c69 656e 743e 3d34 2e31 2e33 0d0a  2client>=4.1.3..
-00000370: 0950 7947 6974 6875 623e 3d31 2e35 380d  .PyGithub>=1.58.
-00000380: 0a09 6b65 7972 696e 673e 3d32 332e 3133  ..keyring>=23.13
-00000390: 2e31 0d0a 0966 6162 7269 633e 3d32 2e37  .1...fabric>=2.7
-000003a0: 2e31 0d0a 0970 6174 6368 776f 726b 3e3d  .1...patchwork>=
-000003b0: 312e 302e 310d 0a09 636f 6c6f 7261 6d61  1.0.1...colorama
-000003c0: 3e3d 302e 342e 360d 0a0d 0a5b 6f70 7469  >=0.4.6....[opti
-000003d0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
-000003e0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
-000003f0: 7473 203d 200d 0a09 6175 7468 203d 2070  ts = ...auth = p
-00000400: 6c75 7368 2e63 6f6e 736f 6c65 3a61 7574  lush.console:aut
-00000410: 685f 656e 7472 790d 0a09 6c69 7374 6b65  h_entry...listke
-00000420: 7973 203d 2070 6c75 7368 2e63 6f6e 736f  ys = plush.conso
-00000430: 6c65 3a6c 6973 745f 6b65 7973 5f65 6e74  le:list_keys_ent
-00000440: 7279 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  ry....[options.e
-00000450: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-00000460: 7465 7374 203d 2070 796c 696e 740d 0a70  test = pylint..p
-00000470: 7562 6c69 7368 203d 200d 0a09 6275 696c  ublish = ...buil
-00000480: 640d 0a09 7477 696e 650d 0a0d 0a5b 6567  d...twine....[eg
-00000490: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000004a0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000004b0: 3d20 300d 0a0d 0a                        = 0....
+00000370: 0950 7947 6974 6875 623e 3d31 2e35 382e  .PyGithub>=1.58.
+00000380: 310d 0a09 6b65 7972 696e 673e 3d32 332e  1...keyring>=23.
+00000390: 3133 2e31 0d0a 0966 6162 7269 633e 3d32  13.1...fabric>=2
+000003a0: 2e37 2e31 0d0a 0970 6174 6368 776f 726b  .7.1...patchwork
+000003b0: 3e3d 312e 302e 310d 0a09 636f 6c6f 7261  >=1.0.1...colora
+000003c0: 6d61 3e3d 302e 342e 360d 0a0d 0a5b 6f70  ma>=0.4.6....[op
+000003d0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000003e0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000003f0: 6970 7473 203d 200d 0a09 6175 7468 203d  ipts = ...auth =
+00000400: 2070 6c75 7368 2e63 6f6e 736f 6c65 3a61   plush.console:a
+00000410: 7574 685f 656e 7472 790d 0a09 6c69 7374  uth_entry...list
+00000420: 6b65 7973 203d 2070 6c75 7368 2e63 6f6e  keys = plush.con
+00000430: 736f 6c65 3a6c 6973 745f 6b65 7973 5f65  sole:list_keys_e
+00000440: 6e74 7279 0d0a 0d0a 5b6f 7074 696f 6e73  ntry....[options
+00000450: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+00000460: 0d0a 7465 7374 203d 2070 796c 696e 740d  ..test = pylint.
+00000470: 0a70 7562 6c69 7368 203d 200d 0a09 6275  .publish = ...bu
+00000480: 696c 640d 0a09 7477 696e 650d 0a0d 0a5b  ild...twine....[
+00000490: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000004a0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000004b0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

