# Comparing `tmp/non_local_detector-0.2.3.dev0.tar.gz` & `tmp/non_local_detector-0.2.4.dev0.tar.gz`

## Comparing `non_local_detector-0.2.3.dev0.tar` & `non_local_detector-0.2.4.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.gitattributes
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/environment.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/environment_gpu.yml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.github/workflows/test_package_build.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.vscode/settings.json
--rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test.ipynb
--rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_clusterless.ipynb
--rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local.ipynb
--rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local_2D.ipynb
--rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_local_spike_times.ipynb
--rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
--rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_simulated.ipynb
--rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_simulated2.ipynb
--rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_sorted_spikes.ipynb
--rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/notebooks/test_spike_times.ipynb
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/_version.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/continuous_state_transitions.py
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/core.py
--rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/discrete_state_transitions.py
--rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/environment.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/initial_conditions.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/observation_models.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/types.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/visualization.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/__init__.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/no_spike.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/__init__.py
--rw-r--r--   0        0        0    51007 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/base.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/cont_frag_model.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/decoder.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/multienvironment_model.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/models/non_local_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/__init__.py
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/clusterless_simulation.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/simulate.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/src/non_local_detector/tests/test_version_import.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/LICENSE
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/README.md
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/pyproject.toml
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/.gitattributes
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/environment.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/environment_gpu.yml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/.github/workflows/test_package_build.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/.vscode/settings.json
+-rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test.ipynb
+-rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_clusterless.ipynb
+-rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_non_local.ipynb
+-rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_non_local_2D.ipynb
+-rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_non_local_spike_times.ipynb
+-rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
+-rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_simulated.ipynb
+-rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_simulated2.ipynb
+-rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_sorted_spikes.ipynb
+-rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/notebooks/test_spike_times.ipynb
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/_version.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/continuous_state_transitions.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/core.py
+-rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/discrete_state_transitions.py
+-rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/environment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/initial_conditions.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/observation_models.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/types.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/visualization.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/__init__.py
+-rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/no_spike.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/__init__.py
+-rw-r--r--   0        0        0    51007 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/base.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/cont_frag_model.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/decoder.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/multienvironment_model.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/models/non_local_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/__init__.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/clusterless_simulation.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/simulate.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/src/non_local_detector/tests/test_version_import.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/LICENSE
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.4.dev0/PKG-INFO
```

### Comparing `non_local_detector-0.2.3.dev0/.github/workflows/test_package_build.yml` & `non_local_detector-0.2.4.dev0/.github/workflows/test_package_build.yml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_clusterless.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_non_local.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_non_local.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_non_local_2D.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_non_local_2D.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_non_local_spike_times.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_non_local_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_non_stationary_discrete_transition.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_non_stationary_discrete_transition.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_simulated.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_simulated.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_simulated2.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_simulated2.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_sorted_spikes.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_sorted_spikes.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/notebooks/test_spike_times.ipynb` & `non_local_detector-0.2.4.dev0/notebooks/test_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/continuous_state_transitions.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/continuous_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/core.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/core.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/discrete_state_transitions.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/discrete_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/environment.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/environment.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/initial_conditions.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/observation_models.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/observation_models.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/types.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/types.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/visualization.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/visualization.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/__init__.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/clusterless_kde.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/clusterless_kde.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         position_std = jnp.array([position_std] * position.shape[1])
     if isinstance(waveform_std, (int, float)):
         waveform_std = jnp.array([waveform_std] * spike_waveform_features[0].shape[1])
 
     is_track_interior = environment.is_track_interior_.ravel(order="F")
     interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
 
-    if environment.track_graph is not None:
+    if environment.track_graph is not None and position.shape[1] > 1:
         # convert to 1D
         position1D = get_linearized_position(
             position,
             environment.track_graph,
             edge_order=environment.edge_order,
             edge_spacing=environment.edge_spacing,
         ).linear_position.to_numpy()[:, None]
@@ -253,22 +253,27 @@
     mean_rates = []
     gpi_models = []
     summed_ground_process_intensity = jnp.zeros(
         (environment.place_bin_centers_.shape[0],)
     )
 
     n_time_bins = int((position_time[-1] - position_time[0]) * sampling_frequency)
+    bounded_spike_waveform_features = []
 
-    for electrode_spike_times in spike_times:
-        electrode_spike_times = electrode_spike_times[
-            jnp.logical_and(
-                electrode_spike_times >= position_time[0],
-                electrode_spike_times <= position_time[-1],
-            )
-        ]
+    for electrode_spike_waveform_features, electrode_spike_times in zip(
+        spike_times, spike_waveform_features
+    ):
+        is_in_bounds = jnp.logical_and(
+            electrode_spike_times >= position_time[0],
+            electrode_spike_times <= position_time[-1],
+        )
+        electrode_spike_times = electrode_spike_times[is_in_bounds]
+        bounded_spike_waveform_features.append(
+            electrode_spike_waveform_features[is_in_bounds]
+        )
         mean_rates.append(len(electrode_spike_times) / n_time_bins)
         encoding_positions.append(
             get_position_at_time(
                 position_time, position, electrode_spike_times, environment
             )
         )
 
@@ -281,15 +286,15 @@
             is_track_interior
         ].add(gpi_model.predict(interior_place_bin_centers))
 
     return {
         "occupancy": occupancy,
         "occupancy_model": occupancy_model,
         "gpi_models": gpi_models,
-        "encoding_spike_waveform_features": spike_waveform_features,
+        "encoding_spike_waveform_features": bounded_spike_waveform_features,
         "encoding_positions": encoding_positions,
         "environment": environment,
         "mean_rates": mean_rates,
         "summed_ground_process_intensity": summed_ground_process_intensity,
         "position_std": position_std,
         "waveform_std": waveform_std,
         "block_size": block_size,
```

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/no_spike.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/no_spike.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     position_std: float = 6.0,
     block_size: int = 100,
     disable_progress_bar: bool = False,
 ):
     is_track_interior = environment.is_track_interior_.ravel(order="F")
     interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
 
-    if environment.track_graph is not None:
+    if environment.track_graph is not None and position.shape[1] > 1:
         # convert to 1D
         position1D = get_linearized_position(
             position,
             environment.track_graph,
             edge_order=environment.edge_order,
             edge_spacing=environment.edge_spacing,
         ).linear_position.to_numpy()[:, None]
```

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/__init__.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/base.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/base.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/cont_frag_model.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/cont_frag_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/decoder.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/decoder.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/multienvironment_model.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/multienvironment_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/models/non_local_model.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/models/non_local_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/clusterless_simulation.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/clusterless_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/simulate.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py` & `non_local_detector-0.2.4.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/.gitignore` & `non_local_detector-0.2.4.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/LICENSE` & `non_local_detector-0.2.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/pyproject.toml` & `non_local_detector-0.2.4.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.3.dev0/PKG-INFO` & `non_local_detector-0.2.4.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non_local_detector
-Version: 0.2.3.dev0
+Version: 0.2.4.dev0
 Summary: A python package to decode non-local activity from neural data
 Project-URL: Homepage, https://github.com/LorenFrankLab/non_local_detector
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/non_local_detector/issues
 Author-email: Eric Denovellis <eric.denovellis@ucsf.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Denovellis
```

