# Comparing `tmp/non_local_detector-0.2.0.dev0.tar.gz` & `tmp/non_local_detector-0.2.1.dev0.tar.gz`

## Comparing `non_local_detector-0.2.0.dev0.tar` & `non_local_detector-0.2.1.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/.gitattributes
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/environment.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/environment_gpu.yml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/.github/workflows/test_package_build.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/.vscode/settings.json
--rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test.ipynb
--rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_clusterless.ipynb
--rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_non_local.ipynb
--rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_non_local_2D.ipynb
--rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_non_local_spike_times.ipynb
--rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
--rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_simulated.ipynb
--rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_simulated2.ipynb
--rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_sorted_spikes.ipynb
--rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/notebooks/test_spike_times.ipynb
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/_version.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/continuous_state_transitions.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/core.py
--rw-r--r--   0        0        0    19361 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/discrete_state_transitions.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/environment.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/initial_conditions.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/observation_models.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/types.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/visualization.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/__init__.py
--rw-r--r--   0        0        0    14686 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/no_spike.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/__init__.py
--rw-r--r--   0        0        0    49652 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/base.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/cont_frag_model.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/decoder.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/multienvironment_model.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/models/non_local_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/__init__.py
--rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/clusterless_simulation.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/simulate.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/src/non_local_detector/tests/test_version_import.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/LICENSE
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/README.md
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 non_local_detector-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/.gitattributes
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/environment.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/environment_gpu.yml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/.github/workflows/test_package_build.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/.vscode/settings.json
+-rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test.ipynb
+-rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_clusterless.ipynb
+-rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_non_local.ipynb
+-rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_non_local_2D.ipynb
+-rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_non_local_spike_times.ipynb
+-rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_non_stationary_discrete_transition.ipynb
+-rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_simulated.ipynb
+-rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_simulated2.ipynb
+-rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_sorted_spikes.ipynb
+-rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/notebooks/test_spike_times.ipynb
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/_version.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/continuous_state_transitions.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/core.py
+-rw-r--r--   0        0        0    19344 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/discrete_state_transitions.py
+-rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/environment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/initial_conditions.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/observation_models.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/types.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/visualization.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/__init__.py
+-rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/clusterless_kde.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/no_spike.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/__init__.py
+-rw-r--r--   0        0        0    49653 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/base.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/cont_frag_model.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/decoder.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/multienvironment_model.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/models/non_local_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/__init__.py
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/clusterless_simulation.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/simulate.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/src/non_local_detector/tests/test_version_import.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/LICENSE
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 non_local_detector-0.2.1.dev0/PKG-INFO
```

### Comparing `non_local_detector-0.2.0.dev0/.github/workflows/test_package_build.yml` & `non_local_detector-0.2.1.dev0/.github/workflows/test_package_build.yml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_clusterless.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_non_local.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_non_local.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_non_local_2D.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_non_local_2D.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_non_local_spike_times.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_non_local_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_non_stationary_discrete_transition.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_non_stationary_discrete_transition.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_simulated.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_simulated.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_simulated2.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_simulated2.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_sorted_spikes.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_sorted_spikes.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/notebooks/test_spike_times.ipynb` & `non_local_detector-0.2.1.dev0/notebooks/test_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/core.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 import numpy as np
-from replay_trajectory_classification.core import atleast_2d, check_converged  # noqa
 
 np.seterr(divide="ignore", invalid="ignore")
 
 
 def convert_to_state_probability(
     causal_posterior: np.ndarray,
     acausal_posterior: np.ndarray,
@@ -205,7 +204,43 @@
 
     return (
         marginal_loglik,
         filtered_probs,
         predicted_probs,
         smoothed_probs,
     )
+
+
+def check_converged(
+    log_likelihood: np.ndarray,
+    previous_log_likelihood: np.ndarray,
+    tolerance: float = 1e-4,
+) -> tuple[bool, bool]:
+    """We have converged if the slope of the log-likelihood function falls below 'tolerance',
+
+    i.e., |f(t) - f(t-1)| / avg < tolerance,
+    where avg = (|f(t)| + |f(t-1)|)/2 and f(t) is log lik at iteration t.
+
+    Parameters
+    ----------
+    log_likelihood : np.ndarray
+        Current log likelihood
+    previous_log_likelihood : np.ndarray
+        Previous log likelihood
+    tolerance : float, optional
+        threshold for similarity, by default 1e-4
+
+    Returns
+    -------
+    is_converged : bool
+    is_increasing : bool
+
+    """
+    delta_log_likelihood = abs(log_likelihood - previous_log_likelihood)
+    avg_log_likelihood = (
+        abs(log_likelihood) + abs(previous_log_likelihood) + np.spacing(1)
+    ) / 2
+
+    is_increasing = log_likelihood - previous_log_likelihood >= -1e-3
+    is_converged = (delta_log_likelihood / avg_log_likelihood) < tolerance
+
+    return is_converged, is_increasing
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/discrete_state_transitions.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/discrete_state_transitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import jax.numpy as jnp
 import numpy as np
 import pandas as pd
 from jax.nn import log_softmax
 from patsy import build_design_matrices, dmatrix
 from scipy.optimize import minimize
 from scipy.special import softmax
-from statsmodels.tsa.stattools import lagmat
 
 
 def centered_softmax_forward(y: np.ndarray) -> np.ndarray:
     """`softmax(x) = exp(x-c) / sum(exp(x-c))` where c is the last coordinate
 
     Example
     -------
@@ -381,15 +380,15 @@
         diag = np.array([0.90, 0.90, 0.90, 0.98])
         discrete_transition = make_transition_from_diag(diag)
 
         if speed_knots is None:
             speed_knots = [1.0, 4.0, 16.0, 32.0, 64.0]
 
         formula = f"1 + bs(speed, knots={speed_knots})"
-        data = {"speed": lagmat(speed, maxlag=1)}
+        data = {"speed": np.concatenate(([0.0], speed[:-1]))}  # lagged speed
         discrete_transition_design_matrix = dmatrix(formula, data)
 
         n_time, n_coefficients = discrete_transition_design_matrix.shape
 
         discrete_transition_coefficients = np.zeros(
             (n_coefficients, n_states, n_states - 1)
         )
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/initial_conditions.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/initial_conditions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 import numpy as np
-from replay_trajectory_classification.environments import Environment
 
+from non_local_detector.environment import Environment
 from non_local_detector.observation_models import ObservationModel
 
 
 @dataclass
 class UniformInitialConditions:
     """Initial conditions where all position bins are
     equally likely."""
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/observation_models.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/observation_models.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/types.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/types.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/visualization.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/visualization.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/__init__.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/clusterless_kde.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/clusterless_kde.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
     environment: Environment,
     sampling_frequency: int = 500,
     position_std: float = 6.0,
     waveform_std: float = 24.0,
     block_size: int = 100,
     disable_progress_bar: bool = False,
 ):
+    position = position if position.ndim > 1 else jnp.expand_dims(position, axis=1)
     if isinstance(position_std, (int, float)):
         position_std = jnp.array([position_std] * position.shape[1])
     if isinstance(waveform_std, (int, float)):
         waveform_std = jnp.array([waveform_std] * spike_waveform_features[0].shape[1])
 
     is_track_interior = environment.is_track_interior_.ravel(order="F")
     interior_place_bin_centers = environment.place_bin_centers_[is_track_interior]
@@ -247,15 +248,17 @@
             position
         )
 
     occupancy = occupancy_model.predict(interior_place_bin_centers)
     encoding_positions = []
     mean_rates = []
     gpi_models = []
-    summed_ground_process_intensity = jnp.zeros_like(occupancy)
+    summed_ground_process_intensity = jnp.zeros(
+        (environment.place_bin_centers_.shape[0],)
+    )
 
     n_time_bins = int((position_time[-1] - position_time[0]) * sampling_frequency)
 
     for electrode_spike_times in spike_times:
         electrode_spike_times = electrode_spike_times[
             jnp.logical_and(
                 electrode_spike_times >= position_time[0],
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/no_spike.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/no_spike.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import jax.numpy as jnp
-import numpy as np
 import jax.scipy
 
 
 def get_spikecount_per_time_bin(spike_times, time):
     spike_times = spike_times[
         jnp.logical_and(spike_times >= time[0], spike_times <= time[-1])
     ]
@@ -11,15 +10,15 @@
         jnp.digitize(spike_times, time[1:-1]),
         minlength=time.shape[0],
     )
 
 
 def predict_no_spike_log_likelihood(
     time,
-    spike_times: np.ndarray,
+    spike_times: jnp.ndarray,
     no_spike_rate: float = 1e-10,
     sampling_frequency: float = 500.0,
 ):
     no_spike_rates = no_spike_rate / sampling_frequency
     spike_count_per_time_bin = jnp.stack(
         [
             get_spikecount_per_time_bin(neuron_spike_times, time)
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/sorted_spikes_glm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 from patsy import build_design_matrices, dmatrix
 from scipy.optimize import minimize
 from tqdm.autonotebook import tqdm
 
-from non_local_detector.core import atleast_2d
 from non_local_detector.environment import get_n_bins
 
 EPS = 1e-15
 
 
 def make_spline_design_matrix(
     position: np.ndarray, place_bin_edges: np.ndarray, knot_spacing: float = 10.0
 ):
-    position = atleast_2d(position)
+    position = position if position.ndim > 1 else position[:, np.newaxis]
     inner_knots = []
     for pos, edges in zip(position.T, place_bin_edges.T):
         n_points = get_n_bins(edges, bin_size=knot_spacing)
         knots = np.linspace(edges.min(), edges.max(), n_points)[1:-1]
         knots = knots[(knots > pos.min()) & (knots < pos.max())]
         inner_knots.append(knots)
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/likelihoods/sorted_spikes_kde.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/__init__.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/base.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,17 @@
 
         # Continuous state transition parameters
         self.continuous_transition_types = continuous_transition_types
 
         # Environment parameters
         if environments is None:
             environments = (Environment(),)
-        if isinstance(environments, Environment):
+        if not hasattr(environments, "__iter__"):
             environments = (environments,)
+
         self.environments = environments
         self.infer_track_interior = infer_track_interior
 
         # Observation model parameters
         if observation_models is None:
             n_states = len(continuous_transition_types)
             env_name = environments[0].environment_name
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/cont_frag_model.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/cont_frag_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/decoder.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from non_local_detector.continuous_state_transitions import RandomWalk, Uniform
+from non_local_detector.continuous_state_transitions import RandomWalk
 from non_local_detector.discrete_state_transitions import DiscreteStationaryDiagonal
 from non_local_detector.environment import Environment
 from non_local_detector.initial_conditions import UniformInitialConditions
 from non_local_detector.models.base import (
     _DEFAULT_CLUSTERLESS_ALGORITHM_PARAMS,
     _DEFAULT_SORTED_SPIKES_ALGORITHM_PARAMS,
     ClusterlessDetector,
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/multienvironment_model.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/multienvironment_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/models/non_local_model.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/models/non_local_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/clusterless_simulation.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/clusterless_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Simulate clusterless spikes and associated spike waveform features."""
 
 import numpy as np
-from replay_trajectory_classification.simulate import (
+from non_local_detector.simulate.simulate import (
     get_trajectory_direction,
     simulate_multiunit_with_place_fields,
     simulate_position,
     simulate_time,
 )
 
 SAMPLING_FREQUENCY = 1000
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/simulate.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/simulate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Main code for simulating position and sorted spikes or clusterless spikes and waveforms."""
 from typing import Optional
 
 import numpy as np
-from replay_trajectory_classification.core import atleast_2d
 from scipy.stats import multivariate_normal
 
 
 def simulate_time(n_samples: int, sampling_frequency: float) -> np.ndarray:
     """Simulate a time in seconds.
 
     Parameters
@@ -127,15 +126,15 @@
     Returns
     -------
     firing_rate : np.ndarray, shape (n_time,)
 
     """
     if is_condition is None:
         is_condition = np.ones(position.shape[0], dtype=bool)
-    position = atleast_2d(position)
+    position = position if position.ndim > 1 else position[:, np.newaxis]
     firing_rate = multivariate_normal(means, variance).pdf(position)
     firing_rate /= firing_rate.max()
     firing_rate *= max_rate
     firing_rate[~is_condition] = 0.0
 
     return firing_rate
```

### Comparing `non_local_detector-0.2.0.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py` & `non_local_detector-0.2.1.dev0/src/non_local_detector/simulate/sorted_spikes_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/.gitignore` & `non_local_detector-0.2.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/LICENSE` & `non_local_detector-0.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.2.0.dev0/pyproject.toml` & `non_local_detector-0.2.1.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
     "scipy",
     "jax",
     "jaxlib",
+    "pandas",
     "networkx",
     "xarray",
     "scikit-learn",
     "patsy",
     "tqdm",
     "track_linearization",
-    "replay_trajectory_classification",
     "matplotlib",
     "seaborn",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/LorenFrankLab/non_local_detector"
```

### Comparing `non_local_detector-0.2.0.dev0/PKG-INFO` & `non_local_detector-0.2.1.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non_local_detector
-Version: 0.2.0.dev0
+Version: 0.2.1.dev0
 Summary: A python package to decode non-local activity from neural data
 Project-URL: Homepage, https://github.com/LorenFrankLab/non_local_detector
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/non_local_detector/issues
 Author-email: Eric Denovellis <eric.denovellis@ucsf.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Denovellis
@@ -32,16 +32,16 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.11,>=3.8
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
+Requires-Dist: pandas
 Requires-Dist: patsy
-Requires-Dist: replay-trajectory-classification
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: track-linearization
 Requires-Dist: xarray
 Provides-Extra: gpu
```

