# Comparing `tmp/non_local_detector-0.2.2.dev0.tar.gz` & `tmp/non_local_detector-0.2.3.dev0.tar.gz`

## Comparing `non_local_detector-0.2.2.dev0.tar` & `non_local_detector-0.2.3.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/.gitattributes
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/environment.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/environment_gpu.yml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/.github/workflows/test_package_build.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/.vscode/settings.json
--rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test.ipynb
--rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_clusterless.ipynb
--rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_non_local.ipynb
--rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_non_local_2D.ipynb
--rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_non_local_spike_times.ipynb
--rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
--rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_simulated.ipynb
--rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_simulated2.ipynb
--rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_sorted_spikes.ipynb
--rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/notebooks/test_spike_times.ipynb
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/_version.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/continuous_state_transitions.py
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/core.py
--rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/discrete_state_transitions.py
--rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/environment.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/initial_conditions.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/observation_models.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/types.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/visualization.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/__init__.py
--rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/no_spike.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/__init__.py
--rw-r--r--   0        0        0    49653 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/base.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/cont_frag_model.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/decoder.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/multienvironment_model.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/models/non_local_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/__init__.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/clusterless_simulation.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/simulate.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/src/non_local_detector/tests/test_version_import.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/LICENSE
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/README.md
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.gitattributes
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/environment.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/environment_gpu.yml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.github/workflows/test_package_build.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.vscode/settings.json
+-rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test.ipynb
+-rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_clusterless.ipynb
+-rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local.ipynb
+-rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local_2D.ipynb
+-rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local_spike_times.ipynb
+-rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
+-rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_simulated.ipynb
+-rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_simulated2.ipynb
+-rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_sorted_spikes.ipynb
+-rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_spike_times.ipynb
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/_version.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/continuous_state_transitions.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/core.py
+-rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/discrete_state_transitions.py
+-rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/environment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/initial_conditions.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/observation_models.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/types.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/visualization.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/__init__.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/no_spike.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/__init__.py
+-rw-r--r--   0        0        0    51007 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/base.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/cont_frag_model.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/decoder.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/multienvironment_model.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/non_local_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/__init__.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/clusterless_simulation.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/simulate.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/tests/test_version_import.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/LICENSE
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/PKG-INFO
```

### Comparing `non_local_detector-0.2.2.dev0/.github/workflows/test_package_build.yml` & `non_local_detector-0.2.3.dev0/.github/workflows/test_package_build.yml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_clusterless.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_non_local.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_non_local.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_non_local_2D.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_non_local_2D.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_non_local_spike_times.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_non_local_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_non_stationary_discrete_transition.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_non_stationary_discrete_transition.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_simulated.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_simulated.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_simulated2.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_simulated2.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_sorted_spikes.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_sorted_spikes.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/notebooks/test_spike_times.ipynb` & `non_local_detector-0.2.3.dev0/notebooks/test_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/continuous_state_transitions.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/continuous_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/core.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/core.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/discrete_state_transitions.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/discrete_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/environment.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/environment.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/initial_conditions.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/observation_models.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/observation_models.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/types.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/types.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/visualization.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/visualization.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/__init__.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/clusterless_kde.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/clusterless_kde.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     )
     if env is not None and env.track_graph is not None:
         position_at_spike_times = get_linearized_position(
             position_at_spike_times,
             env.track_graph,
             edge_order=env.edge_order,
             edge_spacing=env.edge_spacing,
-        ).linear_position.to_numpy()
+        ).linear_position.to_numpy()[:, None]
 
     return position_at_spike_times
 
 
 def fit_clusterless_kde_encoding_model(
     position_time: jnp.ndarray,
     position: jnp.ndarray,
@@ -235,15 +235,15 @@
     if environment.track_graph is not None:
         # convert to 1D
         position1D = get_linearized_position(
             position,
             environment.track_graph,
             edge_order=environment.edge_order,
             edge_spacing=environment.edge_spacing,
-        ).linear_position.to_numpy()
+        ).linear_position.to_numpy()[:, None]
         occupancy_model = KDEModel(std=position_std, block_size=block_size).fit(
             position1D
         )
     else:
         occupancy_model = KDEModel(std=position_std, block_size=block_size).fit(
             position
         )
```

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/no_spike.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/no_spike.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     )
     if env is not None and env.track_graph is not None:
         position_at_spike_times = get_linearized_position(
             position_at_spike_times,
             env.track_graph,
             edge_order=env.edge_order,
             edge_spacing=env.edge_spacing,
-        ).linear_position.to_numpy()
+        ).linear_position.to_numpy()[:, None]
 
     return position_at_spike_times
 
 
 def fit_sorted_spikes_kde_encoding_model(
     position_time: jnp.ndarray,
     position: jnp.ndarray,
@@ -118,15 +118,15 @@
     if environment.track_graph is not None:
         # convert to 1D
         position1D = get_linearized_position(
             position,
             environment.track_graph,
             edge_order=environment.edge_order,
             edge_spacing=environment.edge_spacing,
-        ).linear_position.to_numpy()
+        ).linear_position.to_numpy()[:, None]
         occupancy_model = KDEModel(std=position_std, block_size=block_size).fit(
             position1D
         )
     else:
         occupancy_model = KDEModel(std=position_std, block_size=block_size).fit(
             position
         )
```

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/__init__.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/base.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -806,27 +806,36 @@
         spike_waveform_features,
         is_training=None,
         encoding_group_labels=None,
         environment_labels=None,
     ):
         logger.info("Fitting clusterless spikes...")
         n_time = position.shape[0]
+        position = position if position.ndim > 1 else position[:, np.newaxis]
+
         if is_training is None:
             is_training = np.ones((n_time,), dtype=bool)
 
         if encoding_group_labels is None:
             encoding_group_labels = np.zeros((n_time,), dtype=np.int32)
 
         if environment_labels is None:
             environment_labels = np.asarray(
                 [self.environments[0].environment_name] * n_time
             )
 
         is_training = np.asarray(is_training).squeeze()
 
+        is_nan = np.any(np.isnan(position), axis=1)
+        position = position[~is_nan]
+        position_time = position_time[~is_nan]
+        is_training = is_training[~is_nan]
+        encoding_group_labels = encoding_group_labels[~is_nan]
+        environment_labels = environment_labels[~is_nan]
+
         kwargs = self.clusterless_algorithm_params
         if kwargs is None:
             kwargs = {}
 
         self.encoding_model_ = {}
 
         for obs in np.unique(self.observation_models):
@@ -964,14 +973,19 @@
         position=None,
         position_time=None,
         is_missing=None,
         discrete_transition_covariate_data=None,
     ):
         if position is not None:
             position = position[:, np.newaxis] if position.ndim == 1 else position
+            nan_position = np.any(np.isnan(position), axis=1)
+            if np.any(nan_position) and is_missing is None:
+                is_missing = nan_position
+            elif np.any(nan_position) and is_missing is not None:
+                is_missing = np.logical_or(is_missing, nan_position)
 
         n_time_bins = (
             int((time_range[-1] - time_range[0]) * self.sampling_frequency) + 1
         )
         time = time_range[0] + np.arange(n_time_bins) / self.sampling_frequency
 
         if is_missing is not None and len(is_missing) != len(time):
@@ -1135,26 +1149,33 @@
         spike_times,
         is_training=None,
         encoding_group_labels=None,
         environment_labels=None,
     ):
         logger.info("Fitting place fields...")
         n_time = position.shape[0]
+        position = position if position.ndim > 1 else position[:, np.newaxis]
         if is_training is None:
             is_training = np.ones((n_time,), dtype=bool)
 
         if encoding_group_labels is None:
             encoding_group_labels = np.zeros((n_time,), dtype=np.int32)
 
         if environment_labels is None:
             environment_labels = np.asarray(
                 [self.environments[0].environment_name] * n_time
             )
 
         is_training = np.asarray(is_training).squeeze()
+        is_nan = np.any(np.isnan(position), axis=1)
+        position = position[~is_nan]
+        position_time = position_time[~is_nan]
+        is_training = is_training[~is_nan]
+        encoding_group_labels = encoding_group_labels[~is_nan]
+        environment_labels = environment_labels[~is_nan]
 
         kwargs = self.sorted_spikes_algorithm_params
         if kwargs is None:
             kwargs = {}
 
         self.encoding_model_ = {}
 
@@ -1288,14 +1309,19 @@
         n_time_bins = (
             int((time_range[-1] - time_range[0]) * self.sampling_frequency) + 1
         )
         time = time_range[0] + np.arange(n_time_bins) / self.sampling_frequency
 
         if position is not None:
             position = position[:, np.newaxis] if position.ndim == 1 else position
+            nan_position = np.any(np.isnan(position), axis=1)
+            if np.any(nan_position) and is_missing is None:
+                is_missing = nan_position
+            elif np.any(nan_position) and is_missing is not None:
+                is_missing = np.logical_or(is_missing, nan_position)
 
         if is_missing is not None and len(is_missing) != len(time):
             raise ValueError(
                 f"Length of is_missing must match length of time. Time is n_samples: {len(time)}"
             )
 
         if discrete_transition_covariate_data is not None:
```

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/cont_frag_model.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/cont_frag_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/decoder.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/decoder.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/multienvironment_model.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/multienvironment_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/models/non_local_model.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/models/non_local_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/clusterless_simulation.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/clusterless_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/simulate.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py` & `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/.gitignore` & `non_local_detector-0.2.3.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/LICENSE` & `non_local_detector-0.2.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/pyproject.toml` & `non_local_detector-0.2.3.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.2.dev0/PKG-INFO` & `non_local_detector-0.2.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non_local_detector
-Version: 0.2.2.dev0
+Version: 0.2.3.dev0
 Summary: A python package to decode non-local activity from neural data
 Project-URL: Homepage, https://github.com/LorenFrankLab/non_local_detector
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/non_local_detector/issues
 Author-email: Eric Denovellis <eric.denovellis@ucsf.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Denovellis
```

