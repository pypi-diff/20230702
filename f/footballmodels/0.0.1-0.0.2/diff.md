# Comparing `tmp/footballmodels-0.0.1.tar.gz` & `tmp/footballmodels-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footballmodels-0.0.1.tar", last modified: Fri Jun 30 18:09:57 2023, max compression
+gzip compressed data, was "footballmodels-0.0.2.tar", last modified: Sun Jul  2 10:36:37 2023, max compression
```

## Comparing `footballmodels-0.0.1.tar` & `footballmodels-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.139535 footballmodels-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 18:09:48.000000 footballmodels-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-30 18:09:48.000000 footballmodels-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 18:09:48.000000 footballmodels-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 18:09:48.000000 footballmodels-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 18:09:48.000000 footballmodels-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 18:09:57.139535 footballmodels-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 18:09:48.000000 footballmodels-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 18:09:48.000000 footballmodels-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 18:09:48.000000 footballmodels-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-30 18:09:57.139535 footballmodels-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-30 18:09:48.000000 footballmodels-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/src/footballmodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/src/footballmodels/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/definitions/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/src/footballmodels/player_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/player_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/player_similarity/column_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/player_similarity/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.139535 footballmodels-0.0.1/src/footballmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-30 18:09:48.000000 footballmodels-0.0.1/src/footballmodels/utils/possession_adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:09:57.135535 footballmodels-0.0.1/src/footballmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 18:09:57.000000 footballmodels-0.0.1/src/footballmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-30 18:09:57.000000 footballmodels-0.0.1/src/footballmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:09:57.000000 footballmodels-0.0.1/src/footballmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 18:09:57.000000 footballmodels-0.0.1/src/footballmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 18:09:57.000000 footballmodels-0.0.1/src/footballmodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.659916 footballmodels-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-02 10:36:26.000000 footballmodels-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 10:36:37.667916 footballmodels-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-02 10:36:26.000000 footballmodels-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-02 10:36:26.000000 footballmodels-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 10:36:26.000000 footballmodels-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-02 10:36:37.667916 footballmodels-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-02 10:36:26.000000 footballmodels-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.659916 footballmodels-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/src/footballmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/definitions/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/player_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/column_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/possession_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/top_level.txt
```

### Comparing `footballmodels-0.0.1/.gitignore` & `footballmodels-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/.vscode/settings.json` & `footballmodels-0.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/LICENSE` & `footballmodels-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/PKG-INFO` & `footballmodels-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.1
+Version: 0.0.2
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.1/setup.cfg` & `footballmodels-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/setup.py` & `footballmodels-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/src/footballmodels/definitions/templates.py` & `footballmodels-0.0.2/src/footballmodels/definitions/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 CLEARANCES_PADJ = TemplateAttribute(
     "PAdj Clearances",
     lambda df: df["clearances"],
     True,
     columns_used=["clearances"],
     possession_adjust=PossessionAdjustment.OUT_OF_POSS,
 )
-CROSSES_COMPLETED = TemplateAttribute(
-    name="Completed Crosses",
-    calculation=lambda df: df["crosses_into_penalty_area"],
+DELIVERIES_INTO_PEN_AREA = TemplateAttribute(
+    name="Deliveries Into Penalty Area",
+    calculation=lambda df: df["crosses_into_penalty_area"]+df['passes_into_penalty_area'],
     ascending_rank=True,
-    columns_used=["crosses_into_penalty_area"],
+    columns_used=["crosses_into_penalty_area",'passes_into_penalty_area'],
     sig_figs=2,
 )
 CROSSES_PCT = TemplateAttribute(
     name="Crosses %",
     calculation=lambda df: (100 * df["crosses_into_penalty_area"] / df["crosses"]).fillna(0),
     ascending_rank=True,
     columns_used=["crosses_into_penalty_area", "crosses"],
@@ -299,22 +299,24 @@
     PASSES_PROGRESSIVE,
     PASSES_PROGRESSIVE_PCT,
 ]
 FBTemplate = [
     PASSING_PCT,
     TACKLES_PADJ,
     INTERCEPTIONS_PADJ,
+    PCT_DRIBBLERS_TACKLED,
     KEY_PASSES,
-    CROSSES_COMPLETED,
+    DELIVERIES_INTO_PEN_AREA,
     CROSSES_PCT,
+    OPEN_PLAY_SHOTS_FOR_OTHERS,
     SUCCESSFUL_DRIBBLES,
     CARRY_PROGRESSIVE_DISTANCE,
     DISPOSSESSED,
     SCORING_CONTRIBUTIONS,
-    PCT_DRIBBLERS_TACKLED,
+    
     FOULS,
 ]
 AttackerTemplate = [
     NON_PENALTY_GOALS,
     SHOTS,
     SHOOTING_PCT,
     PASSING_PCT,
```

### Comparing `footballmodels-0.0.1/src/footballmodels/player_similarity/column_defs.py` & `footballmodels-0.0.2/src/footballmodels/player_similarity/column_defs.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/src/footballmodels/player_similarity/models.py` & `footballmodels-0.0.2/src/footballmodels/player_similarity/models.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/src/footballmodels/utils/distance.py` & `footballmodels-0.0.2/src/footballmodels/utils/distance.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/src/footballmodels/utils/possession_adjustment.py` & `footballmodels-0.0.2/src/footballmodels/utils/possession_adjustment.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.1/src/footballmodels.egg-info/PKG-INFO` & `footballmodels-0.0.2/src/footballmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.1
+Version: 0.0.2
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.1/src/footballmodels.egg-info/SOURCES.txt` & `footballmodels-0.0.2/src/footballmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

