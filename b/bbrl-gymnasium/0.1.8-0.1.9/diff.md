# Comparing `tmp/bbrl_gymnasium-0.1.8.tar.gz` & `tmp/bbrl_gymnasium-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.1.8.tar", last modified: Sat Jul  1 10:12:59 2023, max compression
+gzip compressed data, was "bbrl_gymnasium-0.1.9.tar", last modified: Sat Jul  1 10:17:08 2023, max compression
```

## Comparing `bbrl_gymnasium-0.1.8.tar` & `bbrl_gymnasium-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.967622 bbrl_gymnasium-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.967622 bbrl_gymnasium-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.967622 bbrl_gymnasium-0.1.8/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/maze_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/rocket_lander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/single_state_mdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.967622 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 10:12:59.000000 bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:59.971622 bbrl_gymnasium-0.1.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-07-01 10:12:47.000000 bbrl_gymnasium-0.1.8/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.612558 bbrl_gymnasium-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/maze_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/rocket_lander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/single_state_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 10:17:08.000000 bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:17:08.616558 bbrl_gymnasium-0.1.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-07-01 10:16:57.000000 bbrl_gymnasium-0.1.9/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.8/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/.pre-commit-config.yaml` & `bbrl_gymnasium-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/LICENSE` & `bbrl_gymnasium-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/Makefile` & `bbrl_gymnasium-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/PKG-INFO` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bbrl_gymnasium
-Version: 0.1.8
+Name: bbrl-gymnasium
+Version: 0.1.9
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.8/README.md` & `bbrl_gymnasium-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_cartpole.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_cartpole.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/envs/single_state_mdp.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/envs/single_state_mdp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any, Dict, Optional
 import numpy as np
 from gymnasium import spaces
 import gymnasium as gym
 
 class SingleStateMDP(gym.Env):
     def __init__(self, A0=0.3, A1=0.9, nu=5, sigma=0.25, seed=None):
         self.action_space = spaces.Box(-1, 1, shape=(1,), dtype=np.float32)
```

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bbrl-gymnasium
-Version: 0.1.8
+Name: bbrl_gymnasium
+Version: 0.1.9
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.8/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.1.9/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/setup.py` & `bbrl_gymnasium-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.1.9/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.8/tests/test_maze.py` & `bbrl_gymnasium-0.1.9/tests/test_maze.py`

 * *Files identical despite different names*

