# Comparing `tmp/mdsubsampler-0.0.1.tar.gz` & `tmp/mdsubsampler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdsubsampler-0.0.1.tar", max compression
+gzip compressed data, was "mdsubsampler-0.0.2.tar", max compression
```

## Comparing `mdsubsampler-0.0.1.tar` & `mdsubsampler-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0    35149 2022-12-05 15:58:50.114476 mdsubsampler-0.0.1/LICENSE
--rw-r--r--   0        0        0     3906 2023-04-12 13:15:31.348025 mdsubsampler-0.0.1/README.md
--rw-r--r--   0        0        0        0 2022-12-05 15:58:50.185981 mdsubsampler-0.0.1/mdss/__init__.py
--rw-r--r--   0        0        0     6783 2023-04-27 15:48:22.151466 mdsubsampler-0.0.1/mdss/dissimilarity.py
--rw-r--r--   0        0        0    11802 2023-04-27 15:48:15.399641 mdsubsampler-0.0.1/mdss/geometrical_property.py
--rw-r--r--   0        0        0     4348 2023-04-27 15:48:11.583771 mdsubsampler-0.0.1/mdss/graph.py
--rw-r--r--   0        0        0     1472 2023-04-27 15:48:05.514023 mdsubsampler-0.0.1/mdss/log_setup.py
--rw-r--r--   0        0        0     7258 2023-04-27 15:48:00.104763 mdsubsampler-0.0.1/mdss/parser.py
--rw-r--r--   0        0        0     3357 2023-04-27 15:47:49.978238 mdsubsampler-0.0.1/mdss/pca_property.py
--rw-r--r--   0        0        0    10103 2023-04-27 15:47:42.875663 mdsubsampler-0.0.1/mdss/property.py
--rw-r--r--   0        0        0    10665 2023-04-27 15:47:34.109481 mdsubsampler-0.0.1/mdss/protein_data.py
--rw-r--r--   0        0        0     6807 2023-04-27 15:49:40.124292 mdsubsampler-0.0.1/mdss/run.py
--rw-r--r--   0        0        0    20600 2023-04-27 15:49:44.185313 mdsubsampler-0.0.1/mdss/sampler.py
--rw-r--r--   0        0        0        0 2022-12-05 20:37:36.881138 mdsubsampler-0.0.1/mdss/scenarios/__init__.py
--rw-r--r--   0        0        0     3468 2023-04-27 18:15:55.649310 mdsubsampler-0.0.1/mdss/scenarios/scenario_1.py
--rw-r--r--   0        0        0     3379 2023-04-27 18:15:41.437080 mdsubsampler-0.0.1/mdss/scenarios/scenario_2.py
--rw-r--r--   0        0        0     3083 2023-04-27 18:15:47.352952 mdsubsampler-0.0.1/mdss/scenarios/scenario_3.py
--rw-r--r--   0        0        0     7253 2023-04-27 15:50:04.374693 mdsubsampler-0.0.1/mdss/utilities.py
--rw-r--r--   0        0        0      776 2023-04-27 18:23:26.462217 mdsubsampler-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 mdsubsampler-0.0.1/setup.py
--rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 mdsubsampler-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 15:58:50.114476 mdsubsampler-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5291 2023-06-23 09:33:16.100912 mdsubsampler-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2022-12-05 15:58:50.185981 mdsubsampler-0.0.2/mdss/__init__.py
+-rw-r--r--   0        0        0     9833 2023-06-23 12:44:50.302559 mdsubsampler-0.0.2/mdss/dissimilarity.py
+-rw-r--r--   0        0        0    15293 2023-06-23 09:56:37.625581 mdsubsampler-0.0.2/mdss/geometrical_property.py
+-rw-r--r--   0        0        0     5268 2023-06-23 09:22:08.411588 mdsubsampler-0.0.2/mdss/graph.py
+-rw-r--r--   0        0        0     1472 2023-04-27 15:48:05.514023 mdsubsampler-0.0.2/mdss/log_setup.py
+-rw-r--r--   0        0        0     7258 2023-04-27 15:48:00.104763 mdsubsampler-0.0.2/mdss/parser.py
+-rw-r--r--   0        0        0     5385 2023-06-23 18:33:30.402024 mdsubsampler-0.0.2/mdss/pca_property.py
+-rw-r--r--   0        0        0    13148 2023-06-23 18:27:25.013744 mdsubsampler-0.0.2/mdss/property.py
+-rw-r--r--   0        0        0    13055 2023-06-23 14:06:47.377391 mdsubsampler-0.0.2/mdss/protein_data.py
+-rw-r--r--   0        0        0     7164 2023-06-23 18:34:20.166148 mdsubsampler-0.0.2/mdss/run.py
+-rw-r--r--   0        0        0    29630 2023-06-23 18:10:09.182896 mdsubsampler-0.0.2/mdss/sampler.py
+-rw-r--r--   0        0        0        0 2022-12-05 20:37:36.881138 mdsubsampler-0.0.2/mdss/scenarios/__init__.py
+-rw-r--r--   0        0        0   191693 2023-06-22 13:33:04.969202 mdsubsampler-0.0.2/mdss/scenarios/scenario_1.ipynb
+-rw-r--r--   0        0        0     3467 2023-06-10 12:55:28.310981 mdsubsampler-0.0.2/mdss/scenarios/scenario_1.py
+-rw-r--r--   0        0        0    43759 2023-06-23 09:14:12.172387 mdsubsampler-0.0.2/mdss/scenarios/scenario_2.ipynb
+-rw-r--r--   0        0        0     3379 2023-04-27 18:31:24.549969 mdsubsampler-0.0.2/mdss/scenarios/scenario_2.py
+-rw-r--r--   0        0        0    41952 2023-06-01 20:05:14.614929 mdsubsampler-0.0.2/mdss/scenarios/scenario_3.ipynb
+-rw-r--r--   0        0        0     3051 2023-06-23 13:28:48.975774 mdsubsampler-0.0.2/mdss/scenarios/scenario_3.py
+-rw-r--r--   0        0        0     9159 2023-06-23 18:25:11.862648 mdsubsampler-0.0.2/mdss/utilities.py
+-rw-r--r--   0        0        0      817 2023-07-02 15:00:47.602330 mdsubsampler-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 mdsubsampler-0.0.2/setup.py
+-rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 mdsubsampler-0.0.2/PKG-INFO
```

### Comparing `mdsubsampler-0.0.1/LICENSE` & `mdsubsampler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.1/mdss/graph.py` & `mdsubsampler-0.0.2/mdss/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,62 +23,83 @@
 import pandas as pd
 import numpy as np
 import math
 
 
 class PropertyPlot:
     """
-    Represents vector plot after property calculation
+    Class representing overlaping distribution plot of calculated reference property for full and sample trajectory.
 
     Attributes
     -----------
-    protein_property: ProteinProperty class object
-        The object has access to all methods and attributes of ProteinProperty class
+    property : ProteinProperty
+        An instance of the ProteinProperty class representing the calculated reference property for
+        the full protein trajectory.
+    sampled_property : ProteinProperty
+        An instance of the ProteinProperty class representing the calculated reference property for
+        the sampled protein trajectory.
     outfilepath : str
-        path where output file with plot will be saved
+        Path where output file is saved.
     """
 
     def __init__(self, property, sampled_property, outfilepath):
+        """
+        Initialize the PropertyPlot object.
+
+        Parameters
+        ----------
+        property : ProteinProperty
+            An instance of the ProteinProperty class representing the calculated reference property for the full protein trajectory.
+        sampled_property : ProteinProperty
+            An instance of the ProteinProperty class representing the calculated reference property for the sampled protein trajectory.
+        outfilepath : str
+            Path where the output file will be saved.
+        """
         self.property = property
         self.property_vector = property.property_vector
         self.sampled_property = sampled_property
         self.sampled_property_vector = sampled_property.property_vector
         self.frame_indices = property.frame_indices
         self.outfilepath = outfilepath
 
     def convert_list_to_data_frame(self, calculated_property):
         """
-        Converts list with calculated property to pandas dataframe
+        Convert list with calculated property to pandas dataframe.
 
-        Attributes
+        Parameters
         -----------
         calculated_property: list
-            A list that contains a specific calculated property for protein trajectory
+            Contains the calculated property for protein trajectory.
+
+        Returns
+        -------
+        dataframe
+            Dataframe with calculated reference property for protein trajectory.
         """
         df = pd.DataFrame(calculated_property)
         return df
 
     def plot(
         self, property_name, reference_df, sample_df, sample_size, outfilepath=None
     ):
         """
-        Plots overlapped distribution of full and sample trajectory and saves file
+        Plot overlapped distribution of full and sample trajectory and save file.
 
-        Attributes
+        Parameters
         -----------
-        property_name: str
-            Name of property that is calculated
-        reference_df: dataframe
-            dataframe with calculated property for full protein trajectory
-        sample_df: dataframe
-            dataframe with calculated property for sample protein trajectory
-        sample_size: int
-            size of sample trajectory
+        property_name : str
+            Name of calculated reference property.
+        reference_df : dataframe
+            Dataframe with calculated property for full (i.e. reference) protein trajectory.
+        sample_df : dataframe
+            Dataframe with calculated property for sample protein trajectory.
+        sample_size : int
+            Size of sample trajectory.
         outfilepath : str
-            Path where output file with plot will be saved
+            Path where output file is saved.
         """
         if outfilepath is None:
             outfilepath = self.outfilepath
 
         reference_df = self.convert_list_to_data_frame(self.property.property_vector)
         sample_df = self.convert_list_to_data_frame(
             self.sampled_property.property_vector
```

### Comparing `mdsubsampler-0.0.1/mdss/log_setup.py` & `mdsubsampler-0.0.2/mdss/log_setup.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.1/mdss/parser.py` & `mdsubsampler-0.0.2/mdss/parser.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.1/mdss/pca_property.py` & `mdsubsampler-0.0.2/mdss/pca_property.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,40 +23,69 @@
 import MDAnalysis.analysis.pca as pca
 import numpy as np
 from mdss.log_setup import log
 
 
 class TrjPCAProj(ProteinProperty):
     """
-    Represents PCA property class. This class is used for calculation of pca_space
-    vector with number of columns being equal to the number of PCs and the number
-    of rows being equal to the number of frames in the trajectory
+    Subclass of ProteinProperty class representing PCA property. Calculates pca_space
+    vector while setting number of columns as number of PCs and number of rows as number
+    of frames in the trajectory.
 
     Attributes
     ----------
-    protein_data: ProteinData class object
-        The object has access to all methods and attributes of ProteinData class
-    atom_selection: str
-        Atom selection for property calculation
+    protein_data : ProteinData
+        An instance of the ProteinData class representing the protein data.
+    atom_selection : str, optional
+        Atom selection for property calculation. Default selection is CA atoms.
     """
 
     display_name = "TrjPCAProj"
 
     def __init__(self, protein_data, atom_selection="name CA"):
+        """
+        Initialize the TrjPCAProj object.
+
+        Parameters
+        ----------
+        protein_data : ProteinData
+            An instance of the ProteinData class representing the protein data.
+        atom_selection : str, optional
+            Atom selection for property calculation. Default selection is CA atoms.
+        """
         super().__init__(protein_data, atom_selection)
         self.pca_model = None
         self.n_pcs = None
         self.ed_n_pcs = None
         self.property_matrix = None
 
     def _run_pca(self):
+        """
+        Perform Principal Component Analysis for a given protein trajectory and selection of atoms.
+        Retrieve principal components.
+        """
         self.pca_model = pca.PCA(self.protein_data.trajectory_data, self.atom_selection)
         self.pca_model.run()
 
     def select_pc(self, pc_index=1):
+        """
+        Select principal components.
+
+        Parameters
+        ----------
+        pc_index : int, optional
+            Principal component index. Default option is index 1.
+
+        Notes
+        -----
+        If property values are not available, a warning message is printed.
+        If the specified PC index is larger than the number of PCs, a warning message is printed.
+        The selected principal component is assigned to the `property_vector` attribute.
+        The PC index is stored in the `pc_index` attribute.
+        """
         if not self.n_pcs:
             print("Warning: values not available. Please calculate property values.")
             log.warning(
                 "{:12s} Values not available. Please calculate property values".format(
                     "STEPS"
                 )
             )
@@ -66,17 +95,35 @@
                 log.warning(
                     "{:12s} PC index larger than number of PCs.".format("STEPS")
                 )
             else:
                 self.property_vector = self.property_matrix[:, (pc_index - 1)]
                 self.pc_index = pc_index
 
-    def calculate_property(self, var_threshold=0.8, pc_filter=False):
+    # def write_property_vector(self, outfilepath):
+    #     if outfilepath is None:
+    #         return
+
+    #     with open(outfilepath, "w") as f:
+    #         for i, values in zip(self.protein_data.frame_indices, self.property_matrix):
+    #             values_display = " ".join(str(v) for v in values)
+    #             f.write("{} {}\n".format(i, values_display))
+
+    def calculate_property(self, var_threshold=0.8, pc_filter=True):
         """
-        Calculates pca property including all trajectory frames
+        Perform Principal Component Analysis with all trajectory frames.
+
+        Parameters
+        ----------
+        var_threshold : float, optional
+            Threshold to compare cumulated variance to pick the right number of principal components.
+            Default is 0.8.
+        pc_filter : bool, optional
+            Flag to indicate whether to use the filtered number of principal components.
+            If True, `self.ed_n_pcs` will be used; otherwise, `self.n_pcs` will be used.
         """
 
         self._run_pca()
         self.n_pcs = self.pca_model.n_components
         self.ed_n_pcs = np.where(
             self.pca_model.results.cumulated_variance > var_threshold
         )[0][0]
@@ -85,7 +132,11 @@
             selected_pcs = self.ed_n_pcs
         else:
             selected_pcs = self.n_pcs
         self.property_matrix = self.pca_model.transform(
             atomgroup, n_components=selected_pcs
         )
         self.select_pc()
+        self.property_vector = self.property_matrix[:, 0]
+        self._property_statistics()
+        self.discretize_vector()
+        return self.property_vector
```

### Comparing `mdsubsampler-0.0.1/mdss/property.py` & `mdsubsampler-0.0.2/mdss/property.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,29 +24,42 @@
 from mdss.protein_data import ProteinData
 from mdss.log_setup import log
 from mdss.dissimilarity import *
 
 
 class ProteinProperty:
     """
-    Represents protein property on individual frames from trajectory
+    Class representing protein property on a single or multiple frames of a protein trajectory.
 
     Attributes
     ----------
-    protein_data: ProteinData class object
-        The object has access to all methods and attributes of ProteinData class
-    vector:
-        Simple vector with calculated statistics
-    atom_selection: str
-        Atom selection for property calculation
+    protein_data : ProteinData
+        An instance of the ProteinData class representing the protein data.
+    atom_selection : str, optional
+        Atom selection for property calculation. Default string value is CA atoms"
     """
 
     display_name = None
 
     def __init__(self, protein_data, atom_selection="name CA"):
+        """
+        Initialize the ProteinProperty object.
+
+        Parameters
+        ----------
+        protein_data : ProteinData
+            An instance of the ProteinData class representing the protein data.
+        atom_selection : str, optional
+            Atom selection for property calculation. Default string value is CA atoms"
+
+        Notes
+        -----
+        If the provided `protein_data` is not an instance of `ProteinData`, a warning
+        message is printed and `protein_data` attribute is set to None.
+        """
         if not isinstance(protein_data, ProteinData):
             log.warning(
                 "{:12s} An instance of ProteinData is required. protein_data attribute set to None".format(
                     "STEPS"
                 )
             )
             protein_data = None
@@ -62,45 +75,61 @@
         self.recalculate = False
         self.property_key = self._add_reference_to_protein_data()
         log.info("{:15s} Atom selection: {}".format("INPUT", self.atom_selection))
         log.info("{:15s} Property name: {}".format("INPUT", self.display_name))
 
     @classmethod
     def from_xvg(cls, xvg_filepath):
+        """
+        Class method that constructs an instance of the class directly from an xvg file.
+
+        Parameters
+        ----------
+
+        xvg_filepath : str
+            Path where the xvg file is located.
+
+        Returns
+        -------
+        object
+            An instance of the class that was used to call the method.
+        """
         instance = cls(protein_data=None, atom_selection=[None, None])
         _frames, distance_values = np.loadtxt(xvg_filepath, unpack=True)
         instance.property_vector = distance_values
         instance._property_statistics()
         instance.discretize_vector()
         return instance
 
     def _add_reference_to_protein_data(self):
         """
-        Links ProteinProperty and ProteinData classes
+        Link ProteinProperty to ProteinData class.
+
+        Returns
+        -------
+        string
+            Display name of reference property with unique identifier.
+
         """
         if self.protein_data is not None:
             property_key = self.protein_data.add_property(self, self.display_name)
             return property_key
 
     def discretize_vector(self, min_value=None, max_value=None, n_bins=100):
         """
-        Discretises vector for Bhatta and KL distances
+        Discretise vector for Bhattacharyya and Kullback-Leibler distances.
 
-        Attributes
+        Parameters
         ----------
-        min_value: int
-            minimum value for vector
-        max_value: int
-            maximum value for vector
-        n_bins: int
-            number of bins for discretized vector
-
-        Returns
-        -----------
-        Discretised vector
+        min_value : int
+            Minimum value for vector. Default is None.
+        max_value : int
+            Maximum value for vector. Default is None.
+        n_bins : int, optional
+            Number of bins for discretized vector. Default value is 100.
         """
         if min_value is None:
             min_value = self.min_value
         if max_value is None:
             max_value = self.max_value
         bin_size = (max_value - min_value) / n_bins
         bin_vector = np.arange(min_value, max_value, bin_size)
@@ -110,28 +139,37 @@
         counts, bins = np.histogram(self.property_vector, bins=bin_vector)
         self.property_distribution_dict = dict(
             zip(bins, (counts / len(self.property_vector)))
         )
 
     def _property_statistics(self):
         """
-        Calculates minimum, maximum and average values of specific vector
+        Calculate minimum, maximum and average values for a specific vector.
         """
         self.min_value = np.min(self.property_vector)
         self.max_value = np.max(self.property_vector)
         self.avg_value = np.average(self.property_vector)
 
     def set_reference_coordinates(self, frame_index=None):
         """
-        Sets up on first frame and extracts copy of coordinates
+        Set up on a reference frame and extract copy of coordinates.
 
-        Attributes
+        Parameters
         ----------
-        frame_index: int
-            frame index of reference frame
+        frame_index : int, optional
+            Reference structure (i.e. frame) from input protein trajectory. Default is None.
+
+        Returns
+        -------
+        Boolean
+            False if property is not associated to a protein data object, otherwise True.
+
+        Notes
+        -----
+        If associated protein data is not available, a warning message is printed.
         """
         if self.protein_data is not None:
             if frame_index is None:
                 trj_data = self.protein_data.topology_data
             else:
                 trj_data = self.protein_data.trajectory_data
                 trj_data.trajectory[frame_index]
@@ -153,84 +191,112 @@
                     "STEPS"
                 )
             )
             return False
 
     def write_property_vector(self, outfilepath):
         """
-        Creates file with calculations of specific property
+        Generate and save file with calculation of reference property for all frames in protein trajectory.
 
-        Attributes
+        Parameters
         ----------
-        outfilepath: str
-            path to output file
+        outfilepath : str
+            Path where output file is saved.
         """
+        if outfilepath is None:
+            return
+
         with open(outfilepath, "w") as f:
             for i, value in zip(self.frame_indices, self.property_vector):
                 f.write("{} {}\n".format(i, value))
 
     def write_discretized_property_vector(self, outfilepath):
         """
-        Creates discretised vector file with calculations of specific property
+        Generate and save file with calculation of discretised reference property for all frames in protein trajectory.
 
-        Attributes
+        Parameters
         ----------
-        outfilepath: str
-            path to output file
+        outfilepath : str
+            Path where output file is saved.
         """
         if len(self.property_distribution_dict) < 1:
             self.discretize_vector()
-        with open(outfilepath, "w") as f:
-            for i, value in zip(self.frame_indices, self.discretized_property_vector):
-                f.write("{} {}\n".format(i, value))
+        if outfilepath is not None:
+            with open(outfilepath, "w") as f:
+                for i, value in zip(
+                    self.frame_indices, self.discretized_property_vector
+                ):
+                    f.write("{} {}\n".format(i, value))
 
     def write_property_distribution_dict(self, outfilepath):
         """
-        Creates dictionary with information for property distribution
+        Generate and save dictionary file which contains information for property distribution values.
 
-        Attributes
+        Parameters
         ----------
-        outfilepath: str
-            path to output file
+        outfilepath : str
+            Path where output file is saved.
         """
         if len(self.property_distribution_dict) < 1:
             self.discretize_vector()
-        with open(outfilepath, "w") as f:
-            for (key, value) in self.property_distribution_dict.items():
-                f.write("{} {}\n".format(key, value))
+        if outfilepath is not None:
+            with open(outfilepath, "w") as f:
+                for key, value in self.property_distribution_dict.items():
+                    f.write("{} {}\n".format(key, value))
 
 
 class SampledProperty(ProteinProperty):
     """
-    Represents sampled protein property on individual frames from trajectory
+    Subclass of ProteinProperty class representing sampled protein property on individual frames from trajectory.
 
     Attributes
     ----------
-    original_property: vector
-        vector with calculated property for full trajectory
-    sampled_property_vector: vector
-        vector with calculated property for sample trajectory
-    sampled_frame_indices: list
-        list with frame indices of sampled trajectory
-    samples_indices: list
-        list with samples indices
-    sample_size: int
-        size of subsampled trajectory
-    dissimilarity_measure: Dissimilarity class object
+    original_property : vector
+        Contains calculated reference property for full trajectory.
+    sampled_property_vector : vector
+        Contains calculated reference property for sampled trajectory.
+    sampled_frame_indices : list
+        Contains frame indices for sampled trajectory.
+    samples_indices : list
+        Contains samples indices.
+    sample_size : int
+        Size of sampled trajectory.
+    dissimilarity_measure : Dissimilarity, optional
+        An instance of the Dissimilarity class representing the dissimilarity measure.
+        Default is Bhattacharyya.
     """
 
     def __init__(
         self,
         original_property,
         sampled_property_vector,
         sampled_frame_indices,
         samples_indices,
         sample_size,
         dissimilarity_measure=Bhattacharyya,
     ):
+        """
+        Initialize SampledProperty object.
+
+        Parameters
+        ----------
+        original_property : vector
+            Contains calculated reference property for full trajectory.
+        sampled_property_vector : vector
+            Contains calculated reference property for sampled trajectory.
+        sampled_frame_indices : list
+            Contains frame indices for sampled trajectory.
+        samples_indices : list
+            Contains samples indices.
+        sample_size : int
+            Size of sampled trajectory.
+        dissimilarity_measure : Dissimilarity, optional
+            An instance of the Dissimilarity class representing the dissimilarity measure.
+            Default is Bhattacharyya.
+        """
         self.protein_data = original_property.protein_data
         self.atom_selection = original_property.atom_selection
         self.ref_property = original_property
         self.ref_coordinates = []
         self.property_vector = sampled_property_vector
         self.discretized_property_vector = []
         self.property_distribution_dict = {}
@@ -241,32 +307,44 @@
         self._property_statistics()
         self.ref_dissimilarity = self._get_dissimilarity_to_ref(dissimilarity_measure)
         self.display_name = "{}_{}".format(sample_size, original_property.display_name)
         self.property_key = self._add_reference_to_protein_data()
 
     def _get_dissimilarity_to_ref(self, dissimilarity_measure):
         """
-        Measures dissimilarity between full and sampled property
+        Measure dissimilarity between full and sampled calculatd reference property.
 
-        Attributes
+        Parameters
         ----------
-        dissimilarity_measure: Dissimilarity class object
+        dissimilarity_measure : Dissimilarity
+            An instance of the Dissimilarity class representing the dissimilarity measure.
+
+        Returns
+        -------
+        Dissimilarity
+            An instance of Dissimilarity class.
         """
         diss_obj = dissimilarity_measure(self, self.ref_property)
         diss_obj.calculate_dissimilarity()
         self.dissimilarity_name = diss_obj.dissimilarity_name
         self.dissimilarity_threshold = diss_obj.dissimilarity_threshold
         return diss_obj.dissimilarity
 
     def calculate_property(self):
         pass
 
     def get_samples_averages(self):
         """
-        Retrieves average value for each sample trajectory
+        Retrieve average value for each sample trajectory.
+
+        Returns
+        -------
+        dictionary
+            Dictionary with sample sizes and their average values.
+
         """
         samples_labels = set(self.samples_indices)
         average_dict = {}
         for label in samples_labels:
             average_value = np.mean(
                 [
                     value
@@ -275,12 +353,17 @@
                 ]
             )
             average_dict[label] = average_value
         return average_dict
 
     def get_average(self):
         """
-        Retrieves average value from samples averages
+        Retrieve average value from samples averages.
+
+        Returns
+        -------
+        float
+            Average value among all values in a dictionary.
         """
         average_dict = self.get_samples_averages()
         average_value = np.mean(list(average_dict.values()))
         return average_value
```

### Comparing `mdsubsampler-0.0.1/mdss/protein_data.py` & `mdsubsampler-0.0.2/mdss/protein_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,32 +28,44 @@
 from mdss.log_setup import log
 import numpy as np
 import json
 
 
 class ProteinData:
     """
-    Represents protein data
+    Class representing protein data.
 
     Attributes
     -----------
     trajectory_filename : str
-        path to trajectory file
+        Path to trajectory file.
     topology_filename : str
-        path to topology file
-    config_parameters : str
-        protein's configuration parameters
+        Path to topology file.
+    config_parameters : str, optional
+        Protein's configuration parameters. Default is None.
     """
 
     def __init__(
         self,
         trajectory_filename,
         topology_filename,
         config_parameters=None,
     ):
+        """
+        Initialise ProteinData object.
+
+        Parameters
+        -----------
+        trajectory_filename : str
+            Path to trajectory file.
+        topology_filename : str
+            Path to topology file.
+        config_parameters : str, optional
+            Protein's configuration parameters. Default is None.
+        """
 
         self.trajectory_filename = trajectory_filename
         self.topology_filename = topology_filename
         self.trajectory_data = self._read_trajectory(
             self.trajectory_filename, self.topology_filename
         )
         self.topology_data = self._read_topology(self.topology_filename)
@@ -62,69 +74,73 @@
         self.frames = self._frames_of_trajectory()
         self.frame_indices = self._frame_indices_of_trajectory()
         self.ref_coordinates = self.topology_data.trajectory[0].positions
         self.property_dict = {}
 
     def _read_topology(self, topology_filename):
         """
-        Loads topology file
+        Load topology file.
 
-        Attributes
-        -----------
-        topology_filename: str,
-            path to topology file
+        Parameters
+        ----------
+        topology_filename : str
+            Path to topology file.
 
         Returns
-        -----------
-        topology data
+        -------
+        mda.Universe
+            An instance of the MDAnalysis Universe representing the loaded topology data.
         """
         top_data = mda.Universe(topology_filename)
         return top_data
 
     def _read_trajectory(self, trajectory_filename, topology_filename):
         """
-        Loads trajectory and topology files into Universe to build the object
+        Load trajectory and topology files into Universe to build the object.
 
-        Attributes
+        Parameters
         -----------
-        trajectory_filename: str,
-            path to trajectory file
-        topology_filename: str,
-            path to topology file
+        trajectory_filename : str
+            Path to trajectory file.
+        topology_filename : str
+            Path to topology file.
 
         Returns
         -----------
-        trajetory data
+        mda.Universe
+            An instance of the MDAnalysis Universe representing the loaded trajectory.
         """
         trajectory_data = mda.Universe(
             topology_filename,
             trajectory_filename,
             permissive=False,
             topology_format="GRO",
         )
         return trajectory_data
 
     def _select_CA_atoms(self):
         """
-        Reads c-alpha from the first frame of trajectory
+        Select C-alpha atoms from the first frame of the trajectory.
 
         Returns
-        -----------
-        Number of CA atoms from AtomGroup
+        -------
+        MDAnalysis.core.groups.AtomGroup
+            An AtomGroup containing the C-alpha atoms from the first frame of the trajectory.
         """
         ca_atom_group = self.trajectory_data.select_atoms("name CA")
         return ca_atom_group
 
     def _frames_of_trajectory(self):
         """
-        Creates a dictionary with frame number and timestep for protein trajectory
+        Generate a dictionary with frame numbers and timesteps for a protein trajectory.
 
         Returns
-        -----------
-        frames of protein trajectory
+        -------
+        list of tuples
+            A list of tuples containing the frame number (index) and corresponding timestep for each frame.
         """
         frames = []
         for x in range(len(self.trajectory_data.trajectory)):
             _ = self.trajectory_data.trajectory[x]
             frames.append(
                 (
                     x,
@@ -135,38 +151,52 @@
             )
 
         log.info("{:15s} Number of frames: {}".format("INPUT", len(frames)))
         return frames
 
     def _frame_indices_of_trajectory(self):
         """
-        Creates list with frame indices for protein trajectory
+        Generate a list of frame indices for a protein trajectory.
 
         Returns
-        -----------
-        Frame indices from protein trajectory
+        -------
+        list
+            A list of integers representing the frame indices from the protein trajectory.
+
         """
         frame_indices = []
         for x in range(len(self.trajectory_data.trajectory)):
             frame_indices.append(x)
         return frame_indices
 
     def frame_selection_iterator(self, selection_of_frames):
         """
-        Creates a new object with similar attributes to a trajectory object from a
-        specific selection of frames that can be used for further analysis.
+        Create a new object with similar attributes to a trajectory object from a specific selection of frames.
 
-        Attributes
-        -----------
-        selection_of_frames: int,
-            single frame or slice of frames from trajectory
+        Parameters
+        ----------
+        selection_of_frames : int or slice
+            Single frame or slice of frames from the trajectory to select.
 
         Returns
-        -----------
-        FrameIteratorIndices object with the selected frames
+        -------
+        FrameIteratorIndices
+            An instance of the MDAnalysis.coordinates.base.FrameIteratorIndices.
+            It is iterable over the frames of a trajectory.
+
+        Raises
+        ------
+        TypeError
+            If the `selection_of_frames` parameter is neither an integer nor a slice.
+
+        Notes
+        -----
+        The method creates a boolean mask array to indicate the selected frames.
+        If an integer or slice is provided, the corresponding indices in the mask are set to True.
+        The selected frames are extracted from the trajectory data using the mask.
         """
         trajectory_data = self.trajectory_data.trajectory
         mask = np.array([False for _ in trajectory_data])
         for i in selection_of_frames:
             if isinstance(i, int) or isinstance(i, slice):
                 mask[i] = True
             else:
@@ -182,24 +212,30 @@
                 "OUTPUT", len(selected_frames)
             )
         )
         return selected_frames
 
     def frame_selection_indices(self, selection_of_frames):
         """
-        Creates a list with only selected frames from a protein trajectory
+        Generate a list with only selected frames from a protein trajectory
 
-        Attributes
+        Parameters
         -----------
-        selection_of_frames: int,
-            single frame or slice of frames from trajectory
+        selection_of_frames : int or slice
+            Single frame or slice of frames from the trajectory to select.
 
         Returns
-        -----------
-        List with indices of selected frames
+        -------
+        List
+            Contains indices of selected frames.
+
+        Raises
+        ------
+        TypeError
+            If the `selection_of_frames` parameter is neither an integer nor a slice.
         """
         trajectory_data = self.trajectory_data.trajectory
         mask = np.array([False for _ in trajectory_data])
         for i in selection_of_frames:
             if isinstance(i, int) or isinstance(i, slice):
                 mask[i] = True
             else:
@@ -211,106 +247,131 @@
                 raise TypeError("Expected int or slice")
         selected_frames = trajectory_data[np.where(mask)[0]]
         indices_of_selected_frames = [ts.frame for ts in selected_frames]
         return indices_of_selected_frames
 
     def write_xtc_file(self, outfilepath, selected_frames):
         """
-        Writes an xtc file containing only specific frames from a protein trajectory
+        Generate an xtc file containing only selected frames from a protein trajectory.
 
-        Attributes
+        Parameters
         -----------
-        outfilepath: str
-            path to output file
-        selected_frames: int ot list,
-            single frame or list of frames from trajectory
+        outfilepath : str
+            Path where output file is saved.
+        selected_frames : int ot list,
+            Single frame or list of frames from trajectory.
         """
         protein = self.trajectory_data.select_atoms("protein")
         with mda.Writer(outfilepath, protein.n_atoms) as W:
             for t_idx in selected_frames:
                 self.trajectory_data.trajectory[t_idx]
                 W.write(protein)
 
     def cast_output_traj_to_numpy(self, outfilepath, subsampled_traj, unit="nanometer"):
         """
-        Casts an xtc file into a numpy array that can be readable
+        Casts an XTC file into a NumPy array for user readability.
 
-        Attributes
+        Parameters
         -----------
-        outfilepath: str
-            path to output file
-        subsampled_traj: .xtc file
-           subsampled trajectory file
-        unit: str
-            unit for coordinates values
+        outfilepath : str
+            Path where output file is saved.
+        subsampled_traj : MDAnalysis.coordinates.XTC.XTCReader
+            XTC trajectory file.
+        unit : str, optional
+            Unit for coordinates valuess.
+
+        Returns
+        -------
+        numpy.ndarray
+            NumPy array containing the coordinates of the subsampled trajectory.
+
         """
         coordinates_numpy = []
         for ts in subsampled_traj:
             coordinates_numpy.append(deepcopy(ts.positions))
         coordinates_numpy = np.array(coordinates_numpy)
         if unit == "nanometer":
             coordinates_numpy = coordinates_numpy / 10
         np.save(outfilepath, coordinates_numpy)
         return coordinates_numpy
 
     def convert_numpy_to_2D(self, infilepath, outfilepath):
+        """
+        Convert a 3D numpy array to a 2D numpy array and save it to a file.
+
+        Parameters
+        ----------
+        infilepath : numpy.ndarray
+            The input 3D numpy array to be converted.
+        outfilepath : str
+            The path where the output file will be saved.
+
+        Returns
+        -------
+        numpy.ndarray
+            The converted 2D numpy array.
+        """
         (x, y, z) = infilepath.shape
         outfile = np.reshape(infilepath, (x, y * z))
-        print("------")
-        print(outfilepath)
         np.save(outfilepath, outfile)
         return outfile
 
     def ML_input_prep(self, infilepath, outfilepath_training, outfilepath_testing):
         """
-        Prepares input for Machine Learning
+        Prepares input data for machine learning by splitting the input file into training and testing data.
 
-        Attributes
-        -----------
-        outfilepath: str
-            path to output file
-        subsampled_traj: .xtc files
-           subsampled trajectory file
-        unit: str
-            unit for coordinates values
+        Parameters
+        ----------
+        infilepath : str
+            Path to the input file containing the data to be split.
+        outfilepath_training : str
+            Path where the training data file will be saved.
+        outfilepath_testing : str
+            Path where the testing data file will be saved.
         """
         training_data, testing_data = train_test_split(
             infilepath, test_size=0.3, random_state=25
         )
         np.save(outfilepath_training, training_data)
         np.save(outfilepath_testing, testing_data)
 
     def add_property(self, protein_property, property_name):
         """
-        Retrieves key from property dictionary
+        Add a protein property to the dictionary.
 
-        Attributes
-        -----------
-        protein_property: ProteinProperty class object
-               The object has access to all methods and attributes of ProteinProperty class
-        property_name: str
-               property name
+        Parameters
+        ----------
+        protein_property : ProteinProperty
+            An object of the ProteinProperty class that represents the protein property.
+        property_name : str
+            The name of the property to be added.
 
         Returns
-        -----------
-        String that contains the propety name and timestamp.
+        -------
+        str
+            A string containing the property name and timestamp.
         """
         timestamp = str(datetime.now().timestamp())
         key = "{}_{}".format(property_name, timestamp)
         self.property_dict[key] = protein_property
         return key
 
     def property_data_report(self, outfilepath):
         """
-        Creates a .json report with key information and statistics for property
+        Create a JSON report with key information and statistics for the property.
 
-        Attributes
-        -----------
-        outfilepath: str
-            path to output file
+        Parameters
+        ----------
+        outfilepath : str
+            Path to the output file where the JSON report will be saved.
+
+        Returns
+        -------
+        dict
+            A dictionary containing the report information.
         """
         report_dict = {}
         for k, v in self.property_dict.items():
             report_dict[k] = {
                 "min": round(v.min_value, 3),
                 "max": round(v.max_value, 3),
                 "atom_selection": v.atom_selection,
```

### Comparing `mdsubsampler-0.0.1/mdss/run.py` & `mdsubsampler-0.0.2/mdss/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,47 +29,56 @@
 
 import os
 import sys
 
 
 def sampling_workflow(arg_list):
     """
-    Implements data sampling, measures dissimilarity between distributions and returns all output files
+    Implement data sampling, measure dissimilarity between distributions, and return all output files.
 
-    Attributes
-    -----------
-    arg_list: List of arguments - user input from parser
+    Parameters
+    ----------
+    arg_list : list
+        A list of arguments representing the user input from the parser.
     """
     args = p.parse_args(arg_list)
     print(args)
 
     log.info("{:15s} Prefix: {:4.5s}".format("INPUT", args.file_prefix))
     if not os.path.exists(args.output_folder):
         os.makedirs(args.output_folder)
     """
-    Create property class object with user input selection of geometric property
+    Create property class object with user input selection of geometric property.
     """
     property_class = p.PROPERTY_CLASS_MAPPING[args.property]
     """
     Check if user input includes an xvg file with precalculated property
-    otherwise read protein trajectory from input files and calculate property
+    otherwise read protein trajectory from input files and calculate property.
     """
     if args.xvg_file is not None:
         property = property_class.from_xvg(args.xvg_file)
-    else:
+    elif args.xvg_file is None and args.property == "RMSD":
         p_data = pd.ProteinData(
             args.trajectory_file,
             args.topology_file,
             config_parameters=None,
         )
         property = property_class(p_data, args.atom_selection, args.fit)
         property.calculate_property()
+    else:
+        p_data = pd.ProteinData(
+            args.trajectory_file,
+            args.topology_file,
+            config_parameters=None,
+        )
+        property = property_class(p_data, args.atom_selection)
+        property.calculate_property()
     """
     Create sampler class object with user input selection of sampling method sampler
-    Depending on sampling strategy ensure necessary arguments were provided
+    Depending on sampling strategy ensure necessary arguments were provided.
     """
     sampler_class = p.SAMPLER_CLASS_MAPPING[args.sampler]
     if args.sampler == "RandomSampler":
         sampler = sampler_class(
             protein_property=property,
             protein_data=p_data,
             seed_number=args.seed_number,
@@ -112,38 +121,40 @@
             output_folder=args.output_folder,
             file_prefix=args.file_prefix,
             number_of_iterations=args.number_of_iterations,
             seed_number=args.seed_number,
             dissimilarity_measure=dissimilarity_class_dict[args.dissimilarity],
         )
     """
-    Generate all output files in case of user input is list of sample sizes 
+    Generate all output files in case of user input is list of sample sizes.
     """
     if isinstance(args.size, list):
         sampled_property = sampler.scan_sample_size(
             perc_vector=args.size,
             dissimilarity_threshold=None,
             step_recording=args.step_recording,
         )
     else:
         sampled_property = sampler.sample(round(int(args.size) * p_data.n_frames / 100))
 
     """
-    Create dissimilarity class object user input selection of dissimilarity measure
+    Create dissimilarity class object user input selection of dissimilarity measure.
     """
     dissimilarity_class = p.DISSIMILARITY_CLASS_MAPPING[args.dissimilarity]
     dissimilarity_object = dissimilarity_class(property, sampled_property)
+
     """
-    Generate file with calculated property for full trajectory
+    Generate file with calculated property for full trajectory.
     """
     filename = "{}_{}.dat".format(args.file_prefix, property_class.display_name)
     filepath = os.path.join(args.output_folder, filename)
     property.write_property_vector(filepath)
+
     """
-    Generate all output files in case of user input is a single sample size
+    Generate all output files in case of user input is a single sample size.
     """
     if not isinstance(args.size, list):
         log.info(
             "{:15s} Sample percentage size: {:4.5s}".format("INPUT", str(args.size))
         )
         write_output_files(
             output_folder=args.output_folder,
@@ -163,20 +174,20 @@
         )
         log.info(
             "{:15s} Output files for selected sample size were generated successfully".format(
                 "OUTPUT"
             )
         )
     """
-    Generate data report file that includes important statistics about trajectory
+    Generate data report file that includes important statistics about trajectory.
     """
-    filename = "{}_{}.json".format(args.file_prefix, "stats_report")
-    filepath = os.path.join(args.output_folder, filename)
-    p_data.property_data_report(filepath)
-    log.info("{:15s} Statistics report was generated successfully".format("OUTPUT"))
+    # filename = "{}_{}.json".format(args.file_prefix, "stats_report")
+    # filepath = os.path.join(args.output_folder, filename)
+    # p_data.property_data_report(filepath)
+    # log.info("{:15s} Statistics report was generated successfully".format("OUTPUT"))
 
 
 def main(arg_list):
     sampling_workflow(arg_list)
 
 
 def run():
```

### Comparing `mdsubsampler-0.0.1/mdss/scenarios/scenario_1.py` & `mdsubsampler-0.0.2/mdss/scenarios/scenario_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 SAMPLER = "RandomSampler"
 # Size input is in int format but corresponds to percentage of total number of frames
 SIZE = "0.25,0.5,1,2.5,5,10,20,25,50"
 DISSIMILARITY = "Bhattacharyya"
 
 
 def main(trj_filename, top_filename, out_prefix):
-
     dissimilarity_score = sampling_workflow(
         [
             "--traj",
             trj_filename,
             "--top",
             top_filename,
             "--prefix",
```

### Comparing `mdsubsampler-0.0.1/mdss/scenarios/scenario_2.py` & `mdsubsampler-0.0.2/mdss/scenarios/scenario_2.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.1/mdss/scenarios/scenario_3.py` & `mdsubsampler-0.0.2/mdss/scenarios/scenario_3.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 SAMPLER = "WeightedSampler"
 # WEIGHTS_VECTOR = None
 SIZE = "10"
 DISSIMILARITY = "Bhattacharyya"
 
 
 def main(trj_filename, top_filename, out_prefix):
-
     dissimilarity_score = sampling_workflow(
         [
             "--traj",
             trj_filename,
             "--top",
             top_filename,
             "--prefix",
@@ -86,15 +85,14 @@
             "--size",
             str(SIZE),
             "--dissimilarity",
             DISSIMILARITY,
             "--fit",
         ]
     )
-    print(dissimilarity_score)
 
 
 def run():
     args = sys.argv[1:]
     trj_filename = args[0]
     top_filename = args[1]
     out_prefix = args[2]
```

### Comparing `mdsubsampler-0.0.1/mdss/utilities.py` & `mdsubsampler-0.0.2/mdss/utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,27 +20,38 @@
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 import os
 import psutil
 import mdss.graph as g
 from mdss.log_setup import log
 import mdss.protein_data as pd
+from mdss.pca_property import TrjPCAProj
 
 
 class NotEnoughMemoryError(Exception):
     pass
 
 
 class EmptyTrajectoryError(Exception):
     pass
 
 
 def check_file_size(filepath):
     """
-    Checks file size and machine memory to ensure there is enough memory in the system
+    Check file size and machine memory to ensure there is enough memory in the system.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to the file that will be checked.
+
+    Raises
+    ------
+    NotEnoughMemoryError
+        If the size of the file exceeds the available memory.
     """
     mem = psutil.virtual_memory()
     file_size = os.path.getsize(filepath)
     if file_size > mem:
         log.error(
             "{:15s} The size of {} is larger than the available memory".format(
                 "STEPS", filepath
@@ -51,14 +62,31 @@
         )
 
 
 def check_trajectory_size(trajectory_file_path, topology_file_path):
     """
     Checks trajectory size and that trajectory and topology files are not empty and
     contain at least X number of frames.
+
+    Parameters
+    ----------
+    trajectory_file_path : str
+        Path to the trajectory file.
+    topology_file_path : str
+        Path to the topology file.
+
+    Returns
+    -------
+    trajectory_size : int
+        Number of frames in the trajectory.
+
+    Raises
+    ------
+    EmptyTrajectoryError
+        If the trajectory file is empty or contains no frames.
     """
     protein_data = pd.ProteinData(
         trajectory_file_path,
         topology_file_path,
         config_parameters=None,
     )
     trajectory_size = len(
@@ -76,14 +104,28 @@
     return trajectory_size
 
 
 def check_multiple_trajectories_size(list_of_trajectory_files, topology_file_path):
     """
     Checks size of multiple trajectories and that trajectory and topology files are not
     empty and contain at least X number of frames.
+
+    Parameters
+    ----------
+    list_of_trajectory_files : list
+        List of trajectory file paths.
+    topology_file_path : str
+        Path to the topology file.
+
+    Raises
+    ------
+    EmptyTrajectoryError
+        If any of the trajectory files is empty or contains no frames.
+    RuntimeError
+        If one or more trajectory files have empty or no frames.
     """
     errors = []
     for traj in list_of_trajectory_files:
         try:
             check_trajectory_size(traj, topology_file_path)
         except EmptyTrajectoryError as e:
             errors.add(e)
@@ -96,14 +138,28 @@
         raise RuntimeError()
 
 
 def check_number_of_residues(trajectory_file_path, topology_file_path, atom_selection):
     """
     Checks that the number of selected residues that are used as an
     input matches the number of residues in the XTC file.
+
+    Parameters
+    ----------
+    trajectory_file_path : str
+        Path to the trajectory file.
+    topology_file_path : str
+        Path to the topology file.
+    atom_selection : str
+        Atom selection string.
+
+    Raises
+    ------
+    Exception
+        If the number of selected residues is greater than the number of residues in the XTC file.
     """
     protein_data = pd.ProteinData(
         trajectory_file_path,
         topology_file_path,
         config_parameters=None,
     )
     if len(atom_selection) > len(
@@ -115,15 +171,25 @@
             )
         )
         raise Exception("The atom selection is greater than the imported XTC file")
 
 
 def check_file_exists(filepath):
     """
-    Checks that file exists in a given filepath
+    Checks that a file exists at the specified filepath.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to the file.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the file does not exist.
     """
     if not os.path.isfile(filepath):
         raise FileNotFoundError("File {} does not exist".format(filepath))
 
 
 def write_output_files(
     output_folder,
@@ -132,35 +198,39 @@
     s_prop,
     p_data,
     p=None,
     unit="nanometer",
     machine_learning=False,
 ):
     """
-    Writes all output files
+    Writes all output files.
 
-    Attributes
-    -----------
-    output_folder: str,
-            file path for output folder given as user input
-    file_prefix: str,
-            prefix given as user input
-    p_prop: list
-            list with values of property for full trajectory to plot
-    s_prop: list
-            list with values of property for sample trajectory to plot
-    p_data: ProteinData Class object
-
-    p: int
-       percentage of sample trajectory
-    unit: str
-       unit that the property will be calculated and saved
+    Parameters
+    ----------
+    output_folder : str
+        File path for the output folder given as user input.
+    file_prefix : str
+        Prefix given as user input.
+    p_prop : list
+        List with values of the property for the full trajectory to plot.
+    s_prop : list
+        List with values of the property for the sample trajectory to plot.
+    p_data : ProteinData
+        ProteinData class object.
+    p : int, optional
+        Percentage of the sample trajectory.
+    unit : str, optional
+        Unit that the property will be calculated and saved. Default is "nanometer".
+    machine_learning : bool, optional
+        Indicates whether machine learning input files should be generated. Default is False.
     """
+    if output_folder is None:
+        return
 
-    p_format = "_" if p is None else f"_{p}_"
+    p_format = "_" if p is None else f"_{str(p).replace('.', '_')}_"
 
     filename = "{}{}{}.dat".format(
         file_prefix,
         p_format,
         p_prop.display_name,
     )
     filepath = os.path.join(output_folder, filename)
@@ -201,34 +271,38 @@
         )
         filepath_test = os.path.join(output_folder, filename_test)
         p_data.ML_input_prep(ML_input, filepath_train, filepath_test)
 
 
 def plot_property(output_folder, file_prefix, p_prop, s_prop, p=None):
     """
-    Plots overlapped property distributions of full and sample trajectory
+    Plots overlapped property distributions of the full and sample trajectories.
 
-    Attributes
-    -----------
-    output_folder: str,
-            file path for output folder given as user input
-    file_prefix: str,
-            prefix that was given as a choice by the user
-    p_prop: list
-            list with values of property for full trajectory to plot
-    s_prop: list
-            list with values of property for sample trajectory to plot
-    p: int
-       percentage of sample trajectory
+    Parameters
+    ----------
+    output_folder : str
+        File path for the output folder given as user input.
+    file_prefix : str
+        Prefix that was given as a choice by the user.
+    p_prop : list
+        List with values of the property for the full trajectory to plot.
+    s_prop : list
+        List with values of the property for the sample trajectory to plot.
+    p : int, optional
+        Percentage of the sample trajectory.
 
     Returns
-    -----------
-    png file with overlay property distribution of full and sample trajectories
+    -------
+    str
+        Path to the generated PNG file with the overlay property distribution.
 
     """
-    p_format = "_" if p is None else f"_{p}_"
+    if output_folder is None:
+        return
+
+    p_format = "_" if p is None else f"_{str(p).replace('.', '_')}_"
     filename = "{}{}{}_{}.png".format(
         file_prefix, p_format, p_prop.display_name, "plot"
     )
     filepath = os.path.join(output_folder, filename)
     graph = g.PropertyPlot(p_prop, s_prop, filepath)
-    graph.plot(p_prop.display_name, p_prop, s_prop, p, filepath)
+    return graph.plot(p_prop.display_name, p_prop, s_prop, p, filepath)
```

### Comparing `mdsubsampler-0.0.1/pyproject.toml` & `mdsubsampler-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdsubsampler"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Namir Oues <namir.oues@brunel.ac.uk>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "mdss" },
 ]
@@ -19,14 +19,16 @@
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 psutil = "^5.9.4"
 scikit-learn = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
+ipykernel = "^6.23.1"
+jupyter = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 mdss = "mdss.run:run"
```

### Comparing `mdsubsampler-0.0.1/setup.py` & `mdsubsampler-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 {'console_scripts': ['mdss = mdss.run:run',
                      'mdss_scenario_1 = mdss.scenarios.scenario_1:run',
                      'mdss_scenario_2 = mdss.scenarios.scenario_2:run',
                      'mdss_scenario_3 = mdss.scenarios.scenario_3:run']}
 
 setup_kwargs = {
     'name': 'mdsubsampler',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
-    'long_description': '# MDSubSampler: Molecular Dynamics SubSampler\n\nMDSubSampler is a Python library and toolkit for a posteriori subsampling of multiple trajectory data for further analysis. This toolkit implements uniform, random, stratified sampling, bootstrapping and targeted sampling to preserve the original distribution of relevant geometrical properties.\n\n## Prerequisites\n\nThis project requires Python (version 3.9.1 or later). To make sure you have the right version available on your machine, try running the following command. \n\n```sh\n$ python --version\nPython 3.9.1\n```\n\n## Table of contents\n\n- [Project Name](#project-name)\n  - [Prerequisites](#prerequisites)\n  - [Table of contents](#table-of-contents)\n  - [Getting Started](#getting-started)\n  - [Installation](#installation)\n  - [Usage](#usage)\n    - [Workflow](#workflow)\n    - [Scenarios](#scenarios)\n    - [Parser](#parser)\n    - [Development](#development)\n  - [Authors](#authors)\n  - [License](#license)\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for analysis and development purposes. \n\n## Installation\n\n**BEFORE YOU INSTALL:** please read the [prerequisites](#prerequisites)\n\nTo install and set up the library, run:\n\n```sh\n$ pip install MDSubSampler\n```\n\n## Usage \n\n### Workflow\n\nInput:\n- Molecular Dynamics trajectory \n- Geometric property\n- Atom selection [optional - default is "name CA"]\n- Reference structure [optional] \n- Sample size or range of sizes\n- Dissimilarity measure [optional - default is "Bhattacharyya"]\n\nOutput:\n- .dat file with calculated property for full trajectory (user input)\n- .dat file(s) with calculated property for one or all sample sizes input\n- .xtc file(s) with sample trajectory for one or all sample sizes\n- .npy file(s) with sample trajectory for one or all sample sizes \n- .npy training set for ML purposes for sample trajectory (optional)\n- .npy testing set for ML purposes for sample trajectory (optional)\n- .npy file(s) with sample trajectory for one or for all sample sizes \n- .png file with overlapped property distribution of reference and sample\n- .json file report with important statistics from the analysis\n- .txt log file with essential analysis steps and information\n\n### Scenarios\n\nTo run scenarios 1,2 or 3 you can download your protein trajectory and topology file (.xtc and .gro files) to the data folder and then run the following:\n\n```sh\n$ python mdss/scenarios/scenario_1.py data/<YourTrajectoryFile>.xtc data/<YourTopologyfile>.gro <YourPrefix>\n```\n\n### Parser\n\nIf you are a terminal lover you can use the terminal to run the code and make a choice for the parser arguments. To see all options and choices run:\n\n```sh\n$ python mdss/run.py --help\n```\nOnce you have made a selection of arguments, your command can look like the following example:\n\n```sh\n$ python mdss/run.py \\\n    --traj "data/<YourTrajectoryFile>.xtc" \\\n    --top "data/<YourTopologyFile>.gro" \\\n    --prefix "<YourPrefix>" \\\n    --output-folder "data/<YourResultsFolder>" \\\n    --property=\'DistanceBetweenAtoms\' \\\n    --atom-selection=\'G55,P127\' \\\n    --sampler=\'BootstrappingSampler\' \\\n    --n-iterations=50 \\\n    --size=<SampleSize> \\\n    --dissimilarity=\'Bhattacharyya\'\n```\n\n### Development\n\nStart by either downloading the tarball file from https://github.com/alepandini/MDSubSampler to your local machine or cloning this repo on your local machine:\n\n```sh\n$ git clone git@github.com:alepandini/MDSubSampler.git\n$ cd MDSubSampler\n```\n\nFollowing that, download and install poetry from https://python-poetry.org/docs/#installation\n\n\nFinally, run the following:\n\n```sh\n$ poetry install\n$ poetry build\n$ poetry shell\n```\nYou can now start developing the library.\n\n### Authors\n\n* **Namir Oues** - [namiroues](https://github.com/namiroues)\n* **Alessandro Pandini** [alepandini](https://github.com/alepandini)\n\n### License\n\nThe library is licensed by **GPL-3.0**',
+    'long_description': '# MDSubSampler: Molecular Dynamics SubSampler\n\n[![PyPI version](https://badge.fury.io/py/mdsubsampler.svg)](https://badge.fury.io/py/mdsubsampler)\n\nMDSubSampler is a Python library and toolkit for a posteriori subsampling of multiple trajectory data for further analysis. This toolkit implements uniform, random, stratified sampling, bootstrapping and targeted sampling to preserve the original distribution of relevant geometrical properties.\n\n## Prerequisites\n\nThis project requires Python (version 3.9.1 or later). To make sure you have the right version available on your machine, try running the following command. \n\n```sh\n$ python --version\nPython 3.9.1\n```\n\n## Table of contents\n\n- [Project Name](#project-name)\n  - [Prerequisites](#prerequisites)\n  - [Table of contents](#table-of-contents)\n  - [Getting Started](#getting-started)\n  - [Installation](#installation)\n  - [Usage](#usage)\n    - [Workflow](#workflow)\n    - [Scenarios](#scenarios)\n    - [Parser](#parser)\n    - [Development](#development)\n  - [Authors](#authors)\n  - [License](#license)\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for analysis and development purposes. \n\n## Installation\n\n**BEFORE YOU INSTALL:** please read the [prerequisites](#prerequisites)\n\nTo install and set up the library, run:\n\n```sh\npip install MDSubSampler\n```\n\n## Usage \n\n### Workflow\n\nInput:\n- Molecular Dynamics trajectory \n- Geometric property\n- Atom selection [optional - default is "name CA"]\n- Reference structure [optional] \n- Sample size or range of sizes\n- Dissimilarity measure [optional - default is "Bhattacharyya"]\n\nOutput:\n- .dat file with calculated property for full trajectory (user input)\n- .dat file(s) with calculated property for one or all sample sizes input\n- .xtc file(s) with sample trajectory for one or all sample sizes\n- .npy file(s) with sample trajectory for one or all sample sizes \n- .npy training set for ML purposes for sample trajectory (optional)\n- .npy testing set for ML purposes for sample trajectory (optional)\n- .npy file(s) with sample trajectory for one or for all sample sizes \n- .png file with overlapped property distribution of reference and sample\n- .json file report with important statistics from the analysis\n- .txt log file with essential analysis steps and information\n\n### Scenarios\n\nTo run scenarios 1,2 or 3 you can download your protein trajectory and topology file (.xtc and .gro files) to the data folder and then run the following:\n\n```sh\npython mdss/scenarios/scenario_1.py data/<YourTrajectoryFile>.xtc data/<YourTopologyfile>.gro <YourPrefix>\n```\nScenarios 1,2 and 3 are also available in Jupyter Notebooks format, can be used as templates and can be modified interactively according to the user\'s needs. You can also find more advanced scenarios in the cookbook directory. If you clone the library locally to your machine, then run the following command before you run the cells.  \n\n```sh\n%cd <pathToMDSubSamplerDirectory>\n```\n\n### Parser\n\nIf you are a terminal lover you can use the terminal to run the code and make a choice for the parser arguments. To see all options and choices run:\n\n```sh\npython mdss/run.py --help\n```\nOnce you have made a selection of arguments, your command can look like the following example:\n\n```sh\npython mdss/run.py \\\n  --traj "data/<YourTrajectoryFile>.xtc" \\\n  --top "data/<YourTopologyFile>.gro" \\\n  --prefix "<YourPrefix>" \\\n  --output-folder "data/<YourResultsFolder>" \\\n  --property=\'DistanceBetweenAtoms\' \\\n  --atom-selection=\'G55,P127\' \\\n  --sampler=\'BootstrappingSampler\' \\\n  --n-iterations=50 \\\n  --size=<SampleSize> \\\n  --dissimilarity=\'Bhattacharyya\'\n```\n\n### Development\n\n#### With Poetry\n\nStart by either downloading the tarball file from https://github.com/alepandini/MDSubSampler to your local machine or cloning this repo on your local machine:\n\n```sh\ngit clone git@github.com:alepandini/MDSubSampler.git\ncd MDSubSampler\n```\n\nFollowing that, download and install poetry from https://python-poetry.org/docs/#installation\n\n\nFinally, run the following:\n\n```sh\npoetry install\npoetry build\npoetry shell\n```\nYou can now start developing the library.\n\n#### With Docker\n\nStart by installing Docker using this link https://docs.docker.com/get-docker/.\n\nInitially a Docker image will need to be built. To do this run the following command:\n\n```sh\ndocker build -t <image name> .\n```\n\nThen run the following command to get access to a shell with all dependencies installed:\n\n```sh\ndocker run -it -v $(pwd):/app -e PYTHONPATH=/app <image name> /bin/bash\n```\n\nThis will also mirror the local filesystem in the Docker image, so that any local change will\nbe reflected in the running container, and vice-versa, using a Docker volume.\n\nThe repo also includes two handy scripts to run all of the above faster (an image called\n`subsampler` will be created):\n\n```sh\n./build-docker\n./run-docker\n```\n\nAfter dropping in the Docker shell, all dependencies will be installed, and the package scripts\nwill also be in scope (the `mdss` command and all scenarios declared in `pyproject.toml`).\n\n### Authors\n\n* **Namir Oues** - [namiroues](https://github.com/namiroues)\n* **Alessandro Pandini** [alepandini](https://github.com/alepandini)\n\n### License\n\nThe library is licensed by **GPL-3.0**\n',
     'author': 'Namir Oues',
     'author_email': 'namir.oues@brunel.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mdsubsampler-0.0.1/PKG-INFO` & `mdsubsampler-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,11 @@
-Metadata-Version: 2.1
-Name: mdsubsampler
-Version: 0.0.1
-Summary: 
-License: GPL-3.0-only
-Author: Namir Oues
-Author-email: namir.oues@brunel.ac.uk
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MDAnalysis (==2.1.0)
-Requires-Dist: dictances (==1.5.3)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Description-Content-Type: text/markdown
-
 # MDSubSampler: Molecular Dynamics SubSampler
 
+[![PyPI version](https://badge.fury.io/py/mdsubsampler.svg)](https://badge.fury.io/py/mdsubsampler)
+
 MDSubSampler is a Python library and toolkit for a posteriori subsampling of multiple trajectory data for further analysis. This toolkit implements uniform, random, stratified sampling, bootstrapping and targeted sampling to preserve the original distribution of relevant geometrical properties.
 
 ## Prerequisites
 
 This project requires Python (version 3.9.1 or later). To make sure you have the right version available on your machine, try running the following command. 
 
 ```sh
@@ -57,15 +35,15 @@
 ## Installation
 
 **BEFORE YOU INSTALL:** please read the [prerequisites](#prerequisites)
 
 To install and set up the library, run:
 
 ```sh
-$ pip install MDSubSampler
+pip install MDSubSampler
 ```
 
 ## Usage 
 
 ### Workflow
 
 Input:
@@ -89,61 +67,98 @@
 - .txt log file with essential analysis steps and information
 
 ### Scenarios
 
 To run scenarios 1,2 or 3 you can download your protein trajectory and topology file (.xtc and .gro files) to the data folder and then run the following:
 
 ```sh
-$ python mdss/scenarios/scenario_1.py data/<YourTrajectoryFile>.xtc data/<YourTopologyfile>.gro <YourPrefix>
+python mdss/scenarios/scenario_1.py data/<YourTrajectoryFile>.xtc data/<YourTopologyfile>.gro <YourPrefix>
+```
+Scenarios 1,2 and 3 are also available in Jupyter Notebooks format, can be used as templates and can be modified interactively according to the user's needs. You can also find more advanced scenarios in the cookbook directory. If you clone the library locally to your machine, then run the following command before you run the cells.  
+
+```sh
+%cd <pathToMDSubSamplerDirectory>
 ```
 
 ### Parser
 
 If you are a terminal lover you can use the terminal to run the code and make a choice for the parser arguments. To see all options and choices run:
 
 ```sh
-$ python mdss/run.py --help
+python mdss/run.py --help
 ```
 Once you have made a selection of arguments, your command can look like the following example:
 
 ```sh
-$ python mdss/run.py \
-    --traj "data/<YourTrajectoryFile>.xtc" \
-    --top "data/<YourTopologyFile>.gro" \
-    --prefix "<YourPrefix>" \
-    --output-folder "data/<YourResultsFolder>" \
-    --property='DistanceBetweenAtoms' \
-    --atom-selection='G55,P127' \
-    --sampler='BootstrappingSampler' \
-    --n-iterations=50 \
-    --size=<SampleSize> \
-    --dissimilarity='Bhattacharyya'
+python mdss/run.py \
+  --traj "data/<YourTrajectoryFile>.xtc" \
+  --top "data/<YourTopologyFile>.gro" \
+  --prefix "<YourPrefix>" \
+  --output-folder "data/<YourResultsFolder>" \
+  --property='DistanceBetweenAtoms' \
+  --atom-selection='G55,P127' \
+  --sampler='BootstrappingSampler' \
+  --n-iterations=50 \
+  --size=<SampleSize> \
+  --dissimilarity='Bhattacharyya'
 ```
 
 ### Development
 
+#### With Poetry
+
 Start by either downloading the tarball file from https://github.com/alepandini/MDSubSampler to your local machine or cloning this repo on your local machine:
 
 ```sh
-$ git clone git@github.com:alepandini/MDSubSampler.git
-$ cd MDSubSampler
+git clone git@github.com:alepandini/MDSubSampler.git
+cd MDSubSampler
 ```
 
 Following that, download and install poetry from https://python-poetry.org/docs/#installation
 
 
 Finally, run the following:
 
 ```sh
-$ poetry install
-$ poetry build
-$ poetry shell
+poetry install
+poetry build
+poetry shell
 ```
 You can now start developing the library.
 
+#### With Docker
+
+Start by installing Docker using this link https://docs.docker.com/get-docker/.
+
+Initially a Docker image will need to be built. To do this run the following command:
+
+```sh
+docker build -t <image name> .
+```
+
+Then run the following command to get access to a shell with all dependencies installed:
+
+```sh
+docker run -it -v $(pwd):/app -e PYTHONPATH=/app <image name> /bin/bash
+```
+
+This will also mirror the local filesystem in the Docker image, so that any local change will
+be reflected in the running container, and vice-versa, using a Docker volume.
+
+The repo also includes two handy scripts to run all of the above faster (an image called
+`subsampler` will be created):
+
+```sh
+./build-docker
+./run-docker
+```
+
+After dropping in the Docker shell, all dependencies will be installed, and the package scripts
+will also be in scope (the `mdss` command and all scenarios declared in `pyproject.toml`).
+
 ### Authors
 
 * **Namir Oues** - [namiroues](https://github.com/namiroues)
 * **Alessandro Pandini** [alepandini](https://github.com/alepandini)
 
 ### License
```

