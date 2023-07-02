# Comparing `tmp/equilibrator-api-0.4.7.tar.gz` & `tmp/equilibrator-api-0.4.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-api-0.4.7.tar", last modified: Mon Sep 12 10:29:21 2022, max compression
+gzip compressed data, was "equilibrator-api-0.4.8b1.tar", last modified: Sun Jul  2 09:01:36 2023, max compression
```

## Comparing `equilibrator-api-0.4.7.tar` & `equilibrator-api-0.4.8b1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.935112 equilibrator-api-0.4.7/
--rw-rw-rw-   0 root         (0) root         (0)     1311 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4728 2022-09-12 10:29:21.935112 equilibrator-api-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3300 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1992 2022-09-12 10:29:21.937112 equilibrator-api-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.925111 equilibrator-api-0.4.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.937112 equilibrator-api-0.4.7/src/equilibrator_api/
--rw-rw-rw-   0 root         (0) root         (0)     2180 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-09-12 10:29:21.937112 equilibrator-api-0.4.7/src/equilibrator_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    34449 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/component_contribution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.934112 equilibrator-api-0.4.7/src/equilibrator_api/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4237 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/data/cofactors.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.935112 equilibrator-api-0.4.7/src/equilibrator_api/model/
--rw-rw-rw-   0 root         (0) root         (0)     2171 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10479 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/model/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)    34563 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)    18294 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/phased_compound.py
--rw-rw-rw-   0 root         (0) root         (0)    15948 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/phased_reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4146 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/src/equilibrator_api/reaction_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 10:29:21.933112 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4728 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      796 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      292 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 10:29:21.000000 equilibrator-api-0.4.7/src/equilibrator_api.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2022-09-12 10:29:10.000000 equilibrator-api-0.4.7/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.075604 equilibrator-api-0.4.8b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.082604 equilibrator-api-0.4.8b1/src/equilibrator_api/
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-02 09:01:36.082604 equilibrator-api-0.4.8b1/src/equilibrator_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    34583 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/component_contribution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.080604 equilibrator-api-0.4.8b1/src/equilibrator_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/data/cofactors.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.081604 equilibrator-api-0.4.8b1/src/equilibrator_api/model/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10479 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)    34592 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    18294 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/phased_compound.py
+-rw-rw-rw-   0 root         (0) root         (0)    15969 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/phased_reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/src/equilibrator_api/reaction_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 09:01:36.080604 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      796 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      292 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 09:01:36.000000 equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-02 09:01:24.000000 equilibrator-api-0.4.8b1/versioneer.py
```

### Comparing `equilibrator-api-0.4.7/LICENSE` & `equilibrator-api-0.4.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/PKG-INFO` & `equilibrator-api-0.4.8b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.4.7
+Version: 0.4.8b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
@@ -64,17 +64,17 @@
 package.
 
 ## Cite us
 
 If you plan to use results from `equilibrator-api` in a scientific publication,
 please cite our paper:
 
-Noor E, Haraldsdóttir HS, Milo R, Fleming RMT (2013)
-[Consistent Estimation of Gibbs Energy Using Component Contributions](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003098),
-PLoS Comput Biol 9:e1003098, DOI: 10.1371/journal.pcbi.1003098
+M. E. Beber, M. G. Gollub, D. Mozaffari, K. M. Shebek, A. I. Flamholz, R. Milo, and E. Noor,
+*eQuilibrator 3.0: a database solution for thermodynamic constant estimation*
+Nucleic Acids Research (2021), [DOI:10.1093/nar/gkab1106](http://dx.doi.org/10.1093/nar/gkab1106)
 
 ## A very simple example
 
 Note that creating a `ComponentContribution` object for the first time after
 installation, starts an initialization step which downloads ~1.5 GBytes of data
 to your computer. It can take more than an hour (depending on the connection speed).
 Note that the initialization might not work inside a Jupyter notebook environment -
```

### Comparing `equilibrator-api-0.4.7/README.md` & `equilibrator-api-0.4.8b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 package.
 
 ## Cite us
 
 If you plan to use results from `equilibrator-api` in a scientific publication,
 please cite our paper:
 
-Noor E, Haraldsdóttir HS, Milo R, Fleming RMT (2013)
-[Consistent Estimation of Gibbs Energy Using Component Contributions](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003098),
-PLoS Comput Biol 9:e1003098, DOI: 10.1371/journal.pcbi.1003098
+M. E. Beber, M. G. Gollub, D. Mozaffari, K. M. Shebek, A. I. Flamholz, R. Milo, and E. Noor,
+*eQuilibrator 3.0: a database solution for thermodynamic constant estimation*
+Nucleic Acids Research (2021), [DOI:10.1093/nar/gkab1106](http://dx.doi.org/10.1093/nar/gkab1106)
 
 ## A very simple example
 
 Note that creating a `ComponentContribution` object for the first time after
 installation, starts an initialization step which downloads ~1.5 GBytes of data
 to your computer. It can take more than an hour (depending on the connection speed).
 Note that the initialization might not work inside a Jupyter notebook environment -
```

### Comparing `equilibrator-api-0.4.7/setup.cfg` & `equilibrator-api-0.4.8b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/__init__.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/compatibility.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/component_contribution.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/component_contribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,16 @@
 
         S = self.ccache.get_element_data_frame(compounds)
         balancing_atoms = S.index
 
         atom_bag = reaction._get_reaction_atom_bag()
         if atom_bag is None:
             logging.warning(
-                "Cannot balance this reaction due to missing chemical formulas"
+                "Cannot balance this reaction due to missing chemical formulas",
+                stacklevel=3,
             )
             return reaction
         atom_vector = np.array(list(map(lambda a: atom_bag.get(a, 0), balancing_atoms)))
 
         other_atoms = set(atom_bag.keys()).difference(balancing_atoms)
         if other_atoms:
             raise ValueError(
@@ -476,15 +477,18 @@
             the uncertainty matrix (in either 'cov', 'sqrt' or 'fullrank'
             format)
         """
         rxn_dg_pairs = map(lambda r: r.separate_stored_dg(), reactions)
         residual_reactions, stored_dg = zip(*rxn_dg_pairs)
         stored_dg = np.array(stored_dg)
 
-        (standard_dg, dg_uncertainty,) = self.predictor.standard_dg_multi(
+        (
+            standard_dg,
+            dg_uncertainty,
+        ) = self.predictor.standard_dg_multi(
             residual_reactions,
             uncertainty_representation=uncertainty_representation,
         )
 
         standard_dg += Q_(stored_dg, "kJ/mol")
         return standard_dg, dg_uncertainty
 
@@ -567,15 +571,18 @@
                 ionic_strength=self.ionic_strength,
                 temperature=self.temperature,
             ),
             reactions,
         )
         residual_reactions, stored_dg_primes = zip(*rxn_dg_pairs)
 
-        (standard_dg_prime, dg_uncertainty,) = self.predictor.standard_dg_multi(
+        (
+            standard_dg_prime,
+            dg_uncertainty,
+        ) = self.predictor.standard_dg_multi(
             residual_reactions,
             uncertainty_representation=uncertainty_representation,
         )
         standard_dg_prime += np.hstack(stored_dg_primes)
 
         # So far, standard_dg_prime is actually storing only the untransformed
         # standard ΔG. We must add the Legendre transform to each reaction to
@@ -586,15 +593,16 @@
                     p_h=self.p_h,
                     p_mg=self.p_mg,
                     ionic_strength=self.ionic_strength,
                     temperature=self.temperature,
                 )
             except MissingDissociationConstantsException as e:
                 warnings.warn(
-                    f"Cannot calculate Legendre transform for reaction #{i}: " + str(e)
+                    f"Cannot calculate Legendre transform for reaction #{i}: " + str(e),
+                    stacklevel=3,
                 )
 
         if minimize_norm:
             # Calculate the residual matrix (X) that represents the DOFs that
             # are completely free (infinite uncertianty).
             _preprocessor = self.predictor.preprocess
             X = _preprocessor.get_reaction_prediction_orthogonal_dof(residual_reactions)
```

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/data/cofactors.csv` & `equilibrator-api-0.4.8b1/src/equilibrator_api/data/cofactors.csv`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/model/__init__.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/model/bounds.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/model/bounds.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/model/model.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
             rxn = PhasedReaction(
                 sparse=sparse,
                 arrow="=",
                 rid=rid,
                 sparse_with_phases=sparse_with_phases,
             )
             if not rxn.is_balanced(ignore_atoms=("H",)):
-                warnings.warn(f"Reaction {rxn.rid} is not balanced")
+                warnings.warn(f"Reaction {rxn.rid} is not balanced", stacklevel=3)
             reaction_objects.append(rxn)
         reaction_df["ReactionObject"] = reaction_objects
 
         thermo_sbtab = sbtabdoc.get_sbtab_by_id("Thermodynamics")
         if thermo_sbtab:
             rid2dg0 = StoichiometricModel.read_thermodynamics(thermo_sbtab, config_dict)
 
@@ -770,15 +770,15 @@
     @classmethod
     def from_network_sbtab(
         cls,
         filename: Union[str, SBtabDocument],
         comp_contrib: Optional[ComponentContribution] = None,
         freetext: bool = True,
         bounds: Optional[Bounds] = None,
-    ) -> object:
+    ) -> "StoichiometricModel":
         """Initialize a Pathway object using a 'network'-only SBtab.
 
         Parameters
         ----------
         filename : str, SBtabDocument
             a filename containing an SBtabDocument (or the SBtabDocument
             object itself) defining the network (topology) only
```

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/phased_compound.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/phased_compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/phased_reaction.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/phased_reaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             for atom, count in compound.atom_bag.items()
         ]
 
         # create the elemental matrix, where each column is a compound and each
         # row is an element (or e-)
         return (
             pd.DataFrame(atom_data, columns=["compound", "atom", "count"])
-            .pivot("atom", "compound", "count")
+            .pivot(columns="compound", index="atom", values="count")
             .fillna(0.0)
         )
 
     @staticmethod
     def _hashable_reactants(
         sparse_with_phases: Dict[PhasedCompound, float],
         reversible: bool = False,
```

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api/reaction_parser.py` & `equilibrator-api-0.4.8b1/src/equilibrator_api/reaction_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     compound_with_separator = pyparsing.Forward()
     compound_with_separator << (compound_with_coeff + compound_separator)
 
     reaction_side = pyparsing.Forward()
     reaction_side << (
         pyparsing.ZeroOrMore(compound_with_separator) + compound_with_coeff
     )
-    reaction_side.setParseAction(lambda l: [l])
+    reaction_side.setParseAction(lambda _list: [_list])
     reaction_side.setResultsName("reaction_side")
     return reaction_side
 
 
 def make_reaction_parser() -> pyparsing.Forward:
     """Build pyparsing-based recursive descent parser for chemical reactions.
```

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api.egg-info/PKG-INFO` & `equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.4.7
+Version: 0.4.8b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
@@ -64,17 +64,17 @@
 package.
 
 ## Cite us
 
 If you plan to use results from `equilibrator-api` in a scientific publication,
 please cite our paper:
 
-Noor E, Haraldsdóttir HS, Milo R, Fleming RMT (2013)
-[Consistent Estimation of Gibbs Energy Using Component Contributions](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003098),
-PLoS Comput Biol 9:e1003098, DOI: 10.1371/journal.pcbi.1003098
+M. E. Beber, M. G. Gollub, D. Mozaffari, K. M. Shebek, A. I. Flamholz, R. Milo, and E. Noor,
+*eQuilibrator 3.0: a database solution for thermodynamic constant estimation*
+Nucleic Acids Research (2021), [DOI:10.1093/nar/gkab1106](http://dx.doi.org/10.1093/nar/gkab1106)
 
 ## A very simple example
 
 Note that creating a `ComponentContribution` object for the first time after
 installation, starts an initialization step which downloads ~1.5 GBytes of data
 to your computer. It can take more than an hour (depending on the connection speed).
 Note that the initialization might not work inside a Jupyter notebook environment -
```

### Comparing `equilibrator-api-0.4.7/src/equilibrator_api.egg-info/SOURCES.txt` & `equilibrator-api-0.4.8b1/src/equilibrator_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.4.7/versioneer.py` & `equilibrator-api-0.4.8b1/versioneer.py`

 * *Files identical despite different names*

