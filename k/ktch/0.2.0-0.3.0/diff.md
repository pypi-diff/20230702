# Comparing `tmp/ktch-0.2.0.tar.gz` & `tmp/ktch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktch-0.2.0.tar", max compression
+gzip compressed data, was "ktch-0.3.0.tar", max compression
```

## Comparing `ktch-0.2.0.tar` & `ktch-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0    11356 2021-09-20 07:55:48.345883 ktch-0.2.0/LICENSE
--rw-r--r--   0        0        0      316 2023-04-13 04:50:43.332584 ktch-0.2.0/README.md
--rw-r--r--   0        0        0      814 2023-06-01 00:37:37.601300 ktch-0.2.0/ktch/__init__.py
--rw-r--r--   0        0        0      553 2023-05-30 07:52:28.753316 ktch-0.2.0/ktch/datasets/__init__.py
--rw-r--r--   0        0        0    11047 2023-05-30 07:52:28.754382 ktch-0.2.0/ktch/datasets/_base.py
--rw-r--r--   0        0        0        0 2022-12-11 05:38:36.524177 ktch-0.2.0/ktch/datasets/data/__init__.py
--rw-r--r--   0        0        0    46290 2022-08-04 14:54:31.590989 ktch-0.2.0/ktch/datasets/data/data_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0    88299 2022-08-05 14:24:20.181451 ktch-0.2.0/ktch/datasets/data/data_outline_bottles.csv
--rw-r--r--   0        0        0   285403 2022-08-04 15:02:34.740790 ktch-0.2.0/ktch/datasets/data/data_outline_mosquito_wings.csv
--rw-r--r--   0        0        0      799 2022-08-04 14:54:31.592162 ktch-0.2.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0      846 2022-08-05 14:24:29.858660 ktch-0.2.0/ktch/datasets/data/meta_outline_bottles.csv
--rw-r--r--   0        0        0      792 2022-12-28 15:03:59.552650 ktch-0.2.0/ktch/datasets/data/meta_outline_mosquito_wings.csv
--rw-r--r--   0        0        0    18006 2022-08-06 16:19:26.502747 ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
--rw-r--r--   0        0        0    17900 2022-08-06 16:21:05.211446 ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
--rw-r--r--   0        0        0        0 2022-12-11 05:38:47.499486 ktch-0.2.0/ktch/datasets/descr/__init__.py
--rw-r--r--   0        0        0       71 2022-08-04 13:17:19.062753 ktch-0.2.0/ktch/datasets/descr/data_landmark_mosquito_wings.rst
--rw-r--r--   0        0        0       68 2022-08-05 14:26:37.531493 ktch-0.2.0/ktch/datasets/descr/data_outline_bottles.rst
--rw-r--r--   0        0        0       68 2022-08-04 15:14:08.538505 ktch-0.2.0/ktch/datasets/descr/data_outline_mosquito_wings.rst
--rw-r--r--   0        0        0     5340 2023-05-30 08:44:14.197928 ktch-0.2.0/ktch/landmark/_Procrustes_analysis.py
--rw-r--r--   0        0        0      835 2023-03-24 02:11:14.247029 ktch-0.2.0/ktch/landmark/__init__.py
--rw-r--r--   0        0        0     3992 2021-09-21 01:54:55.378710 ktch-0.2.0/ktch/landmark/_landmark.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901541 ktch-0.2.0/ktch/landmark/tests/__init__.py
--rw-r--r--   0        0        0     1097 2023-06-01 00:10:23.018240 ktch-0.2.0/ktch/outline/__init__.py
--rw-r--r--   0        0        0    12904 2023-06-01 00:09:48.310946 ktch-0.2.0/ktch/outline/_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0      690 2023-05-18 08:04:07.126268 ktch-0.2.0/ktch/outline/_plot/reconstructed_shapes.py
--rw-r--r--   0        0        0     7401 2023-01-07 02:23:20.969778 ktch-0.2.0/ktch/outline/_spherical_harmonic_analysis.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901733 ktch-0.2.0/ktch/outline/tests/__init__.py
--rw-r--r--   0        0        0     1763 2023-05-31 04:22:10.407679 ktch-0.2.0/ktch/outline/tests/test_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.2.0/ktch/tests/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-01 01:01:59.041878 ktch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 ktch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-23 03:21:23.404492 ktch-0.3.0/LICENSE
+-rw-r--r--   0        0        0      350 2023-06-26 04:27:07.675589 ktch-0.3.0/README.md
+-rw-r--r--   0        0        0      864 2023-07-02 16:48:19.809070 ktch-0.3.0/ktch/__init__.py
+-rw-r--r--   0        0        0      661 2023-06-27 10:00:20.339645 ktch-0.3.0/ktch/datasets/__init__.py
+-rw-r--r--   0        0        0    11067 2023-07-01 04:29:50.150850 ktch-0.3.0/ktch/datasets/_base.py
+-rw-r--r--   0        0        0     2974 2023-06-28 00:54:07.102190 ktch-0.3.0/ktch/datasets/_sample_generator.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:21:39.664617 ktch-0.3.0/ktch/datasets/data/__init__.py
+-rw-r--r--   0        0        0    46290 2023-06-23 03:21:39.535438 ktch-0.3.0/ktch/datasets/data/data_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0    88299 2023-06-23 03:21:39.553325 ktch-0.3.0/ktch/datasets/data/data_outline_bottles.csv
+-rw-r--r--   0        0        0   285403 2023-06-23 03:21:39.537674 ktch-0.3.0/ktch/datasets/data/data_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0      799 2023-06-23 03:21:39.538090 ktch-0.3.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0      846 2023-06-23 03:21:39.553737 ktch-0.3.0/ktch/datasets/data/meta_outline_bottles.csv
+-rw-r--r--   0        0        0      792 2023-06-23 03:21:39.701830 ktch-0.3.0/ktch/datasets/data/meta_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0    18006 2023-06-23 03:21:39.554248 ktch-0.3.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
+-rw-r--r--   0        0        0    17900 2023-06-23 03:21:39.554771 ktch-0.3.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
+-rw-r--r--   0        0        0        0 2023-06-23 03:21:39.664691 ktch-0.3.0/ktch/datasets/descr/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-23 03:21:39.538419 ktch-0.3.0/ktch/datasets/descr/data_landmark_mosquito_wings.rst
+-rw-r--r--   0        0        0       68 2023-06-23 03:21:39.555073 ktch-0.3.0/ktch/datasets/descr/data_outline_bottles.rst
+-rw-r--r--   0        0        0       68 2023-06-23 03:21:39.538754 ktch-0.3.0/ktch/datasets/descr/data_outline_mosquito_wings.rst
+-rw-r--r--   0        0        0      746 2023-06-28 09:51:49.737612 ktch-0.3.0/ktch/io/__init__.py
+-rw-r--r--   0        0        0     9697 2023-06-30 10:03:13.720872 ktch-0.3.0/ktch/io/_tps.py
+-rw-r--r--   0        0        0     6075 2023-07-02 16:46:57.851454 ktch-0.3.0/ktch/landmark/_Procrustes_analysis.py
+-rw-r--r--   0        0        0      835 2023-06-23 03:23:35.051862 ktch-0.3.0/ktch/landmark/__init__.py
+-rw-r--r--   0        0        0     3992 2023-06-23 03:21:23.420003 ktch-0.3.0/ktch/landmark/_landmark.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:21:39.444203 ktch-0.3.0/ktch/landmark/tests/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-23 03:23:59.235815 ktch-0.3.0/ktch/motion/__init__.py
+-rw-r--r--   0        0        0     1252 2023-07-01 05:21:21.330953 ktch-0.3.0/ktch/outline/__init__.py
+-rw-r--r--   0        0        0    13480 2023-07-01 05:21:04.417578 ktch-0.3.0/ktch/outline/_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0      690 2023-07-02 16:46:57.852452 ktch-0.3.0/ktch/outline/_plot/reconstructed_shapes.py
+-rw-r--r--   0        0        0    12956 2023-06-26 04:27:07.677178 ktch-0.3.0/ktch/outline/_spherical_harmonic_analysis.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:21:39.444317 ktch-0.3.0/ktch/outline/tests/__init__.py
+-rw-r--r--   0        0        0     1763 2023-06-23 03:23:52.942126 ktch-0.3.0/ktch/outline/tests/test_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.3.0/ktch/tests/__init__.py
+-rw-r--r--   0        0        0     2370 2023-07-02 16:48:40.747870 ktch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 ktch-0.3.0/PKG-INFO
```

### Comparing `ktch-0.2.0/LICENSE` & `ktch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/__init__.py` & `ktch-0.3.0/ktch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 import types
 from pathlib import Path
 from importlib.metadata import version
 
 
 from . import landmark
 from . import outline
+from . import io
+from . import datasets
 
 __version__ = version(__name__)
 
 __all__ = [
     "landmark",
     "outline",
+    "io",
     "datasets",
     "__version__",
 ]
```

### Comparing `ktch-0.2.0/ktch/datasets/__init__.py` & `ktch-0.3.0/ktch/datasets/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,20 @@
     load_outline_mosquito_wings,
     load_outline_bottles,
     load_coefficient_bottles,
     convert_coords_df_to_list,
     convert_coords_df_to_df_sklearn_transform,
 )
 
+from ._sample_generator import (
+    make_landmarks_from_reference,
+)
+
 __all__ = [
     "load_landmark_mosquito_wings",
     "load_outline_mosquito_wings",
     "load_outline_bottles",
     "load_coefficient_bottles",
     "convert_coords_df_to_list",
     "convert_coords_df_to_df_sklearn_transform",
+    "make_landmarks_from_reference",
 ]
```

### Comparing `ktch-0.2.0/ktch/datasets/_base.py` & `ktch-0.3.0/ktch/datasets/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 
 import pandas as pd
 from sklearn.utils import Bunch
 from sklearn.datasets._base import load_descr
 
 
 def load_landmark_mosquito_wings(*, as_frame=False):
-    """Load and return the mosquito wing landmark dataset used in [Rohlf_and_Slice_1990]_.
+    """Load and return the mosquito wing landmark dataset used in
+    [Rohlf_and_Slice_1990]_.
 
-    The original of this dataset is available at `SB Morphometrics <https://www.sbmorphometrics.org/data/RohlfSlice1990Mosq.nts>`_.
+    The original of this dataset is available at
+    `SB Morphometrics <https://www.sbmorphometrics.org/data/RohlfSlice1990Mosq.nts>`_.
 
     ========================   ============
     Specimens                      127
     Landmarks per specimen          18
     Landmark dimensionality          2
     Features                      real
     ========================   ============
@@ -86,17 +88,20 @@
         meta=meta,
         DESCR=fdescr,
         filename=data_file_name,
     )
 
 
 def load_outline_mosquito_wings(*, as_frame=False):
-    """Load and return the mosquito wing outline dataset used in [Rohlf_and_Archie_1984]_, however includes only 126 of 127 specimens because of missing in the original NTS file.
+    """Load and return the mosquito wing outline dataset used in
+    [Rohlf_and_Archie_1984]_, however includes only 126 of 127 specimens
+    because of missing in the original NTS file.
 
-    The original NTS file of this data is available at `SB Morphometrics <https://www.sbmorphometrics.org/data/RohlfArchieWingOutlines.nts>`_.
+    The original NTS file of this data is available at
+    `SB Morphometrics <https://www.sbmorphometrics.org/data/RohlfArchieWingOutlines.nts>`_.
 
     ========================   ===========
     Specimens                      126
     Landmarks per specimen         100
     Landmark dimensionality          2
     Features                      real
     ========================   ===========
```

### Comparing `ktch-0.2.0/ktch/datasets/data/data_landmark_mosquito_wings.csv` & `ktch-0.3.0/ktch/datasets/data/data_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/data_outline_bottles.csv` & `ktch-0.3.0/ktch/datasets/data/data_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/data_outline_mosquito_wings.csv` & `ktch-0.3.0/ktch/datasets/data/data_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv` & `ktch-0.3.0/ktch/datasets/data/meta_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/meta_outline_bottles.csv` & `ktch-0.3.0/ktch/datasets/data/meta_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/meta_outline_mosquito_wings.csv` & `ktch-0.3.0/ktch/datasets/data/meta_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv` & `ktch-0.3.0/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv` & `ktch-0.3.0/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/landmark/_Procrustes_analysis.py` & `ktch-0.3.0/ktch/landmark/_Procrustes_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 # limitations under the License.
 
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
 import scipy as sp
 
+import numpy.typing as npt
+
+
 from sklearn.base import (
     BaseEstimator,
     TransformerMixin,
     ClassNamePrefixFeaturesOutMixin,
 )
 
 
@@ -149,14 +152,42 @@
         X_centered = np.array([x - np.mean(x, axis=0) for x in X])
         return X_centered
 
     def _scale(self, X):
         X_scaled = np.array([x / centroid_size(x) for x in X])
         return X_scaled
 
+    def get_feature_names_out(
+        self, input_features: None | npt.ArrayLike = None
+    ) -> np.ndarray:
+        """Get output feature names.
+
+        Parameters
+        ----------
+        input_features : None | npt.ArrayLike, optional
+            Input feature names, by default None
+
+        Returns
+        -------
+        feature_names_out : ndarray of str objects
+            Transformed feature names.
+
+        """
+        # x
+        # y
+        # z
+
+        feature_names_out = np.asarray(xn + yn + zn, dtype=str)
+        return feature_names_out
+
+    @property
+    def _n_features_out(self):
+        """Number of transformed output features."""
+        return self.n_landmarks * self.n_dim
+
 
 class LandmarkImputer(TransformerMixin, BaseEstimator):
     def __init__(self, missing_values=np.nan):
         pass
 
 
 def centroid_size(x):
```

### Comparing `ktch-0.2.0/ktch/landmark/__init__.py` & `ktch-0.3.0/ktch/landmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/landmark/_landmark.py` & `ktch-0.3.0/ktch/landmark/_landmark.py`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/outline/__init__.py` & `ktch-0.3.0/ktch/outline/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # from ._polar_Fourier_analysis import PFA
-from ._elliptic_Fourier_analysis import EllipticFourierAnalysis
+from ._elliptic_Fourier_analysis import EllipticFourierAnalysis, rotation_matrix_2d
+from ._spherical_harmonic_analysis import spharm, SPHARMCoefficients
 
 # from ._spherical_harmonic_analysis import SphericalHarmonicAnalysis, PCContribDisplay
 
 __all__ = [
     "EllipticFourierAnalysis",
+    "rotation_matrix_2d",
     # "SphericalHarmonicAnalysis",
     # "PCContribDisplay",
+    "spharm",
+    "SPHARMCoefficients",
 ]
```

### Comparing `ktch-0.2.0/ktch/outline/_elliptic_Fourier_analysis.py` & `ktch-0.3.0/ktch/outline/_elliptic_Fourier_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import Literal
+from enum import IntEnum
 
 from operator import index
+
 import numpy as np
 import numpy.typing as npt
 import scipy as sp
 from scipy.spatial.transform import Rotation as R
 import pandas as pd
 
 from sklearn.base import (
@@ -40,14 +42,17 @@
     Elliptic Fourier Analysis (EFA) 
 
     Parameters
     ------------
     n_harmonics: int, default=20
         harmonics
 
+    n_dim: int, default=2
+        dimension
+
     reflect: bool, default=False
         reflect
 
     metric: str
         metric
 
     impute: bool, False
@@ -72,29 +77,49 @@
     References
     ------------
     .. [Kuhl_Giardina_1982] Kuhl, F.P., Giardina, C.R. (1982) Elliptic Fourier features of a closed contour. Comput. Graph. Image Process. 18: 236–258.
 
 
     """
 
-    def __init__(self, n_harmonics=20, dim=2, reflect=False, metric="", impute=False):
+    def __init__(
+        self,
+        n_harmonics=20,
+        n_dim=2,
+        reflect=False,
+        metric="",
+        impute=False,
+    ):
+        """
+        ToDo
+        -------
+        * EHN: excluding position from the output
+        """
         # self.dtype = dtype
         self.n_harmonics = n_harmonics
-        self.dim = dim
+        if n_dim not in (2, 3):
+            raise ValueError("n_dim must be 2 or 3")
+        elif n_dim == 3:
+            raise NotImplementedError("n_dim=3 is not implemented yet")
+        else:
+            self.n_dim = n_dim
         self.reflect = reflect
         self.metric = metric
         self.impute = impute
 
     def fit_transform(self, X, t=None, norm=True):
         return self.transform(X, t, norm=norm)
 
-    def transform(self, X, t=None, norm=True):
-        """
-
-        Fit the model with X.
+    def transform(
+        self,
+        X: list(npt.ArrayLike) | npt.ArrayLike,
+        t: npt.ArrayLike = None,
+        norm: bool = True,
+    ) -> npt.ArrayLike:
+        """EFA.
 
         Parameters
         ------------
         X: {list of array-like, array-like} of shape (n_samples, n_coords, dim)
             Coordinate values of n_samples.
             The i-th array-like of shape (n_coords_i, 2) represents
             2D coordinate values of the i-th sample.
@@ -105,35 +130,34 @@
             each coordinate value in the i-th element of X.
             If `t=None`, then t is calculated based on
             the coordinate values with the linear interpolation.
 
         norm: bool, default=True
             Normalize the elliptic Fourier coefficients by the major axis of the 1st ellipse.
 
-        as_frame: bool, default=False
-            Return the result as a pandas DataFrame.
-
         Returns
         ------------
         X_transformed: array-like of shape (n_samples, (1+2*n_harmonics)*n_dim)
             Returns the array-like of coefficients.
-            (a_0, a_1, ..., a_n, b_0, b_1, ..., b_n, , c_0, c_1, ..., c_n, , d_0, d_1, ..., d_n)
+            (a_0, a_1, ..., a_n, b_0, b_1, ..., b_n, , c_0, c_1, ..., c_n, d_0, d_1, ..., d_n)
 
         """
-        dim = self.dim
+        n_dim = self.n_dim
+        n_harmonics = self.n_harmonics
 
         if t is None:
             t_ = [None for i in range(len(X))]
 
         if len(t_) != len(X):
             raise ValueError("t must have a same length of X ")
 
         if isinstance(X, pd.DataFrame):
             X_ = [
-                row.dropna().to_numpy().reshape(dim, -1).T for idx, row in X.iterrows()
+                row.dropna().to_numpy().reshape(n_dim, -1).T
+                for idx, row in X.iterrows()
             ]
         else:
             X_ = X
 
         X_transformed = np.stack(
             [self._transform_single(X_[i], t_[i], norm=norm) for i in range(len(X_))]
         )
@@ -246,17 +270,17 @@
         c_s = c1 * np.cos(theta) + d1 * np.sin(theta)
         scale = np.sqrt(a_s**2 + c_s**2)
         psi = np.arctan2(c_s, a_s)
         if psi < 0:
             psi = psi + 2 * np.pi
 
         coef_norm_list = []
-        r_psi = _rotation_matrix_2d(-psi)
+        r_psi = rotation_matrix_2d(-psi)
         for n in range(1, len(an)):
-            r_ntheta = _rotation_matrix_2d(n * theta)
+            r_ntheta = rotation_matrix_2d(n * theta)
             coef_orig = np.array([[an[n], bn[n]], [cn[n], dn[n]]])
             coef_norm_tmp = (1 / scale) * np.dot(np.dot(r_psi, coef_orig), r_ntheta)
             coef_norm_list.append(coef_norm_tmp.reshape(-1))
 
         coef_norm = np.stack(coef_norm_list)
         An = np.append(an[0], coef_norm[:, 0])
         Bn = np.append(bn[0], coef_norm[:, 1])
@@ -374,22 +398,22 @@
 ###########################################################
 #
 #   utility functions
 #
 ###########################################################
 
 
-def _rotation_matrix_2d(theta):
+def rotation_matrix_2d(theta):
     rot_mat = np.array(
         [[np.cos(theta), -np.sin(theta)], [np.sin(theta), np.cos(theta)]]
     )
     return rot_mat
 
 
-def _cse(dx, dt, n_harmonics):
+def _cse(dx: np.ndarray, dt: np.ndarray, n_harmonics: int) -> np.ndarray:
     """Cos series expansion
 
     Parameters
     ----------
     dx : np.ndarray
         differences of coordinates
     dt : np.ndarray
@@ -417,15 +441,15 @@
     ]
 
     coef = np.array([c0] + cn)
 
     return coef
 
 
-def _sse(dx, dt, n_harmonics):
+def _sse(dx: np.ndarray, dt: np.ndarray, n_harmonics: int) -> np.ndarray:
     """Sin series expansion"""
     t = np.concatenate([[0], np.cumsum(dt)])
     T = t[-1]
 
     c0 = 0
     cn = [
         (T / (2 * (np.pi**2) * (n**2)))
```

### Comparing `ktch-0.2.0/ktch/outline/_plot/reconstructed_shapes.py` & `ktch-0.3.0/ktch/outline/_plot/reconstructed_shapes.py`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/ktch/outline/tests/test_elliptic_Fourier_analysis.py` & `ktch-0.3.0/ktch/outline/tests/test_elliptic_Fourier_analysis.py`

 * *Files identical despite different names*

### Comparing `ktch-0.2.0/pyproject.toml` & `ktch-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,22 @@
   'Topic :: Scientific/Engineering',
   'Operating System :: Microsoft :: Windows',
   'Operating System :: POSIX',
   'Operating System :: Unix',
   'Operating System :: MacOS',
   'Programming Language :: Python :: 3.8',
 ]
-description = "**ktch** is a python package for model-based morphometrics."
-homepage = "https://doc.ktch.dev/index.html"
+description = "ktch is a python package for model-based morphometrics."
+homepage = "https://doc.ktch.dev"
 keywords = ["morphometrics", "theoretical morphology"]
 license = "Apache-2.0"
 name = "ktch"
 readme = "README.md"
 repository = "https://github.com/noshita/ktch"
-version = "0.2.0"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 numpy = "^1.22"
 pandas = "^1.4"
 python = ">= 3.8, < 3.12"
 scikit-learn = "^1.2"
 scipy = "^1.8"
@@ -46,34 +46,35 @@
 jupyter = "^1.0.0"
 jupyterlab = "^3.4.4"
 jupytext = "^1.14.5"
 liccheck = "^0.7.2"
 llvmlite = "^0.39.1"
 matplotlib = "^3.5.2"
 module-name = "^0.6.0"
-myst-nb = "^0.17.2"
-nbsphinx = "^0.9.2"
 numba = "^0.56.4"
-numpydoc = "^1.4.0"
 opencv-python = "^4.7.0.68"
 plotly = "^5.9.0"
 poetry2conda = "^0.3.0"
-pydata-sphinx-theme = "^0.12"
 pytest = "^7.1"
 pytest-cov = "^3.0"
 seaborn = "^0.11.0"
 setuptools = "<60.0"
+tqdm = "^4.64.1"
+tslearn = "^0.5.3.2"
+xarray = "^2022.6.0"
+
+[tool.poetry.group.doc.dependencies]
+myst-nb = "^0.17.2"
+nbsphinx = "^0.9.2"
+numpydoc = "^1.4.0"
+pydata-sphinx-theme = "^0.12"
 sphinx = "^5.3"
 sphinx-autobuild = "^2021.3"
 sphinx-gallery = "^0.11"
-sphinx-notfound-page = "^0.8.3"
 sphinxcontrib-bibtex = "^2.5"
-tqdm = "^4.64.1"
-tslearn = "^0.5.3.2"
-xarray = "^2022.6.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry2conda]
 name = "ktch"
```

### Comparing `ktch-0.2.0/PKG-INFO` & `ktch-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ktch
-Version: 0.2.0
-Summary: **ktch** is a python package for model-based morphometrics.
-Home-page: https://doc.ktch.dev/index.html
+Version: 0.3.0
+Summary: ktch is a python package for model-based morphometrics.
+Home-page: https://doc.ktch.dev
 License: Apache-2.0
 Keywords: morphometrics,theoretical morphology
 Author: Noshita, Koji
 Author-email: noshita@morphometrics.jp
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,14 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: docs
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: scipy (>=1.8,<2.0)
@@ -33,14 +32,20 @@
 Project-URL: Repository, https://github.com/noshita/ktch
 Description-Content-Type: text/markdown
 
 # ktch - A python package for model-based morphometrics
 
 [![codecov](https://codecov.io/gh/noshita/ktch/branch/main/graph/badge.svg?token=SJN66K7KJY)](https://codecov.io/gh/noshita/ktch)
 
-**ktch** is a python package for model-based morphometrics.
+ktch is a python package for model-based morphometrics.
+
+## Usage
+
+```sh
+pip install ktch
+```
 
 
 ## License
 
 ktch is licensed under the Apache License, Version2.0
```

