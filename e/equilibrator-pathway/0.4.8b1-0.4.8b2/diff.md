# Comparing `tmp/equilibrator-pathway-0.4.8b1.tar.gz` & `tmp/equilibrator-pathway-0.4.8b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-pathway-0.4.8b1.tar", last modified: Mon Apr 24 08:14:47 2023, max compression
+gzip compressed data, was "equilibrator-pathway-0.4.8b2.tar", last modified: Sun Jul  2 13:52:51 2023, max compression
```

## Comparing `equilibrator-pathway-0.4.8b1.tar` & `equilibrator-pathway-0.4.8b2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.251419 equilibrator-pathway-0.4.8b1/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4067 2023-04-24 08:14:47.252419 equilibrator-pathway-0.4.8b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2020 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.242418 equilibrator-pathway-0.4.8b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7210 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/analysis_solution.py
--rwxrwxrwx   0 root         (0) root         (0)    23350 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/cost_function.py
--rw-rw-rw-   0 root         (0) root         (0)    12964 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10368 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_solution.py
--rw-rw-rw-   0 root         (0) root         (0)     6593 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdf_solution.py
--rwxrwxrwx   0 root         (0) root         (0)     7404 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdmc_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    10429 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/pathway.py
--rw-rw-rw-   0 root         (0) root         (0)     4343 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    10878 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/thermo_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4363 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.251419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4067 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      832 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      335 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.281863 equilibrator-pathway-0.4.8b2/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-02 13:52:51.281863 equilibrator-pathway-0.4.8b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.275863 equilibrator-pathway-0.4.8b2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/analysis_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)    23350 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/cost_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10311 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)     6600 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdf_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)     7446 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdmc_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    10429 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/pathway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4343 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10878 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/thermo_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.280863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/versioneer.py
```

### Comparing `equilibrator-pathway-0.4.8b1/LICENSE` & `equilibrator-pathway-0.4.8b2/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/PKG-INFO` & `equilibrator-pathway-0.4.8b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.8b1
+Version: 0.4.8b2
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
```

### Comparing `equilibrator-pathway-0.4.8b1/README.md` & `equilibrator-pathway-0.4.8b2/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/setup.cfg` & `equilibrator-pathway-0.4.8b2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 license = MIT
 description = Pathway analysis tools by eQuilibrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
@@ -29,24 +30,22 @@
 	pathway analysis
 	enzyme cost minimization
 	max-min driving force
 
 [options]
 zip_safe = True
 install_requires = 
-	pint~=0.19
-	numpy~=1.23
-	pandas~=1.4
-	scipy~=1.9
+	pint~=0.21
+	pandas~=1.5
 	seaborn~=0.12
 	uncertainties~=3.1
 	osqp~=0.6
-	cvxpy~=1.2
+	cvxpy~=1.3
 	sbtab~=1.0
-	equilibrator-api==0.4.7
+	equilibrator-api==0.4.8b1
 python_requires = >=3.8
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
 
@@ -56,19 +55,20 @@
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-raises
 development = 
 	jupyter~=1.0
-	jupyterlab~=3.2
-	black[jupyter]~=22.1
-	isort~=5.10
-	safety~=1.10
-	tox~=3.24
+	jupyterlab~=4.0
+	black[jupyter]~=23.3
+	isort~=5.12
+	safety~=2.3
+	tox~=4.6
+	twine~=4.0
 deployment = 
 	click
 	click-log
 	python-dateutil
 	requests
 	tqdm
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/__init__.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/analysis_solution.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/analysis_solution.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,25 +106,25 @@
                 "optimized_dg_prime",
             ],
         )
 
         lbs, ubs = pathway.bounds
         compound_data = zip(
             pathway.compound_ids,
-            np.exp(self.ln_conc).flatten() * standard_concentration,
-            lbs,
-            ubs,
+            np.exp(self.ln_conc).flatten() * standard_concentration.m_as("M"),
+            map(lambda x: x.m_as("M"), lbs),
+            map(lambda x: x.m_as("M"), ubs),
         )
         self._compound_df = pd.DataFrame(
             data=list(compound_data),
             columns=[
                 "compound_id",
-                "concentration",
-                "lower_bound",
-                "upper_bound",
+                "concentration_in_molar",
+                "lower_bound_in_molar",
+                "upper_bound_in_molar",
             ],
         )
 
     @property
     def reaction_df(self) -> pd.DataFrame:
         """Get a DataFrame with all the reaction data.
 
@@ -142,17 +142,17 @@
 
     @property
     def compound_df(self) -> pd.DataFrame:
         """Get a DataFrame with all the compound data.
 
         The columns are:
             compound_id
-            concentration
-            lower_bound
-            upper_bound
+            concentration_in_molar
+            lower_bound_in_molar
+            upper_bound_in_molar
 
         """
         return self._compound_df
 
     @property
     def reaction_ids(self) -> Iterable[str]:
         """Return the reaction IDs."""
@@ -170,15 +170,15 @@
         # add a table with the optimized metabolite concentrations
         met_data = []
         for row in self.compound_df.itertuples():
             met_data.append(
                 (
                     "concentration",
                     row.compound_id,
-                    f"{row.concentration.m_as('M'):.3e}",
+                    f"{row.concentration_in_molar:.3e}",
                 )
             )
         met_df = pd.DataFrame(
             columns=["!QuantityType", "!Compound", "!Value"], data=met_data
         )
         met_sbtab = SBtab.SBtabTable.from_data_frame(
             met_df,
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/cost_function.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/cost_function.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_model.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_model.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_solution.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
-from equilibrator_api import Q_
 from matplotlib import pyplot as plt
 from sbtab import SBtab
 
 from .analysis_solution import PathwayAnalysisSolution
 from .cost_function import EnzymeCostFunction
 from .ecm_model import EnzymeCostModel
 from .util import PlotCorrelation
@@ -67,19 +66,19 @@
             self.meas_enz_conc = ecm_model._get_measured_enzyme_conc()
         else:
             self.meas_met_conc = None
             self.meas_enz_conc = None
 
         self.enzyme_df = pd.DataFrame(
             data=self.costs.tolist(),
-            columns=["capacity", "thermodynamic", "saturation", "allosteric"],
+            columns=["capacity_in_molar", "thermodynamic", "saturation", "allosteric"],
         )
 
-        self.enzyme_df["concentration"] = [
-            np.exp(x.value) * Q_("M") for x in self.ecf.ECF(self.ln_conc)
+        self.enzyme_df["concentration_in_molar"] = [
+            np.exp(x.value) for x in self.ecf.ECF(self.ln_conc)
         ]
 
         self.enzyme_df.insert(0, "reaction_id", pd.Series(list(self.reaction_ids)))
 
     @property
     def driving_forces(self) -> np.ndarray:
         """Calculate the driving forces of all reactions."""
@@ -221,17 +220,15 @@
         ax.set_xticklabels(self.reaction_ids, size="medium", rotation=90)
         ax.legend(loc="best", framealpha=0.2)
         ax.set_ylabel("enzyme demand [M]")
         ax.set_ylim(bottom=base)
 
     def validate_metabolite_conc(self, ax: plt.Axes, scale: str = "log") -> None:
         """Create a correlation plot validating the metabolite concentrations."""
-        pred_met_conc = self.compound_df.concentration.apply(
-            lambda x: x.m_as("M")
-        ).values
+        pred_met_conc = self.compound_df.concentration_in_molar.values
 
         # remove NaNs and zeros
         mask = np.nan_to_num(self.meas_met_conc) > 0
         mask &= np.nan_to_num(pred_met_conc) > 0
 
         # remove compounds with fixed concentrations
         mask &= self.ecf.ln_conc_sigma > self.ecf.MINIMAL_STDEV
@@ -246,15 +243,15 @@
         )
         ax.set_xlabel("measured [M]")
         ax.set_ylabel("predicted [M]")
 
     def validate_enzyme_conc(self, ax: plt.Axes, scale: str = "log") -> None:
         """Create a correlation plot validating the enzyme concentrations."""
 
-        pred_enz_conc = self.enzyme_df.concentration.apply(lambda x: x.m_as("M")).values
+        pred_enz_conc = self.enzyme_df.concentration_in_molar.values
 
         PlotCorrelation(
             ax,
             self.meas_enz_conc.m_as("M"),
             pred_enz_conc,
             labels=self.enzyme_df.reaction_id,
             scale=scale,
@@ -264,21 +261,21 @@
         ax.set_ylabel("predicted [M]")
 
     def to_sbtab(self) -> SBtab.SBtabDocument:
         """Export the results to an SBtab file."""
         sbtabdoc = super(PathwayEcmSolution, self).to_sbtab()
 
         # add another table containing the optimized enzyme concentrations
-        enz_df = self.enzyme_df[["reaction_id", "concentration"]].copy()
-        enz_df["concentration"] = enz_df.concentration.apply(
-            lambda x: f"{x.m_as('M'):.3e}"
+        enz_df = self.enzyme_df[["reaction_id", "concentration_in_molar"]].copy()
+        enz_df["concentration_in_molar"] = enz_df["concentration_in_molar"].apply(
+            lambda x: f"{x:.3e}"
         )
         enz_df.insert(0, "!QuantityType", "concentration of enzyme")
         enz_df = enz_df.rename(
-            columns={"reaction_id": "!Reaction", "concentration": "!Value"}
+            columns={"reaction_id": "!Reaction", "concentration_in_molar": "!Value"}
         )
 
         enz_sbtab = SBtab.SBtabTable.from_data_frame(
             enz_df,
             table_id="Predicted enzyme levels",
             table_type="Quantity",
             unit="M",
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdf_solution.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdf_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,30 +91,30 @@
                 color, marker, label = ("blue", "<", "shadow price < 0")
             elif shadow_sign == 1:
                 color, marker, label = ("red", ">", "shadow price > 0")
             else:
                 color, marker, label = ("grey", "d", "shadow price = 0")
 
             group_df.plot.scatter(
-                x="concentration",
+                x="concentration_in_molar",
                 y="y",
                 s=40,
                 c=color,
                 marker=marker,
                 ax=ax,
                 zorder=2,
                 colorbar=False,
                 label=label,
             )
         ax.set_ylabel("")
         ax.set_yticks(data_df.y)
 
         for j, row in enumerate(data_df.itertuples(index=True)):
             ax.plot(
-                [row.lower_bound.m_as("M"), row.upper_bound.m_as("M")],
+                [row.lower_bound_in_molar, row.upper_bound_in_molar],
                 [row.y, row.y],
                 color="lightgrey",
                 linewidth=3,
                 zorder=1,
                 label="allowed range" if j == 0 else None,
             )
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdmc_solution.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdmc_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,24 @@
         )
         self.objective_values.name = "Total squared Z-scores"
 
         grouped_df = self.solution_df.groupby(["value_type", "var_type", "var_name"])
 
         self.concentration_df = grouped_df.get_group(
             ("primal", "var", "log_conc")
-        ).pivot("name", "df_lb", "value")
+        ).pivot(index="name", columns="df_lb", values="value")
         self.concentration_df = np.exp(self.concentration_df)
 
         self.zscore_df = grouped_df.get_group(("zscore", "var", "log_conc")).pivot(
             "name", "df_lb", "value"
         )
 
         self._reaction_prices_df = grouped_df.get_group(
             ("shadow_price", "cnstr", "driving_force")
-        ).pivot("name", "df_lb", "value")
+        ).pivot(index="name", columns="df_lb", values="value")
 
     def reaction_prices_df(self, normalized=False) -> pd.DataFrame:
         """Get the reaction shadow prices."""
         abs_prices = self._reaction_prices_df.apply(np.abs)
         if normalized:
             # normalize the shadow prices in each column to 1
             return abs_prices.multiply(1.0 / abs_prices.sum(0))
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/pathway.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/pathway.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/simulator.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/simulator.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/thermo_models.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/thermo_models.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/util.py` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/util.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/PKG-INFO` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.8b1
+Version: 0.4.8b2
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
```

### Comparing `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/SOURCES.txt` & `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b1/versioneer.py` & `equilibrator-pathway-0.4.8b2/versioneer.py`

 * *Files identical despite different names*

