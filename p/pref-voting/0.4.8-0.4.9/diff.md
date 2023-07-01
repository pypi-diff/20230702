# Comparing `tmp/pref_voting-0.4.8.tar.gz` & `tmp/pref_voting-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.4.8.tar", max compression
+gzip compressed data, was "pref_voting-0.4.9.tar", max compression
```

## Comparing `pref_voting-0.4.8.tar` & `pref_voting-0.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.4.8/LICENSE
--rw-r--r--   0        0        0     3528 2023-06-02 10:11:51.114635 pref_voting-0.4.8/README.md
--rw-r--r--   0        0        0       22 2023-06-02 10:11:56.283855 pref_voting-0.4.8/pref_voting/__init__.py
--rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.4.8/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.4.8/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.4.8/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.4.8/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.4.8/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.4.8/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.4.8/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.4.8/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     4347 2023-06-01 14:59:17.885777 pref_voting-0.4.8/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     4874 2023-06-01 02:28:51.128709 pref_voting-0.4.8/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.4.8/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.4.8/pref_voting/helper.py
--rw-r--r--   0        0        0    80807 2023-06-02 10:13:04.013698 pref_voting-0.4.8/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.4.8/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.4.8/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.4.8/pref_voting/other_methods.py
--rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.4.8/pref_voting/profiles.py
--rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.4.8/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.4.8/pref_voting/rankings.py
--rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.4.8/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     6840 2023-06-01 14:59:19.931166 pref_voting-0.4.8/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0     3066 2023-05-31 23:53:43.134760 pref_voting-0.4.8/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.4.8/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    15702 2023-06-02 02:53:42.477653 pref_voting-0.4.8/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.4.8/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.4.8/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.4.8/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.4.8/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      689 2023-06-02 10:11:56.282805 pref_voting-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 pref_voting-0.4.8/setup.py
--rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 pref_voting-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3528 2023-06-02 10:11:51.114635 pref_voting-0.4.9/README.md
+-rw-r--r--   0        0        0       22 2023-06-02 14:35:53.771090 pref_voting-0.4.9/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.4.9/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.4.9/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.4.9/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.4.9/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.4.9/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.4.9/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.4.9/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.4.9/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4347 2023-06-01 14:59:17.885777 pref_voting-0.4.9/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     5184 2023-06-02 14:34:09.881209 pref_voting-0.4.9/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.4.9/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.4.9/pref_voting/helper.py
+-rw-r--r--   0        0        0    80808 2023-06-02 14:30:48.418411 pref_voting-0.4.9/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.4.9/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.4.9/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.4.9/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.4.9/pref_voting/profiles.py
+-rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.4.9/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.4.9/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.4.9/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     6840 2023-06-01 14:59:19.931166 pref_voting-0.4.9/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0     3066 2023-05-31 23:53:43.134760 pref_voting-0.4.9/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     6670 2023-06-02 14:35:21.653749 pref_voting-0.4.9/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    15702 2023-06-02 02:53:42.477653 pref_voting-0.4.9/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.4.9/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.4.9/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.4.9/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.4.9/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      689 2023-06-02 14:35:53.769598 pref_voting-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 pref_voting-0.4.9/setup.py
+-rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 pref_voting-0.4.9/PKG-INFO
```

### Comparing `pref_voting-0.4.8/LICENSE` & `pref_voting-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/README.md` & `pref_voting-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/analysis.py` & `pref_voting-0.4.9/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/axiom.py` & `pref_voting-0.4.9/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/c1_methods.py` & `pref_voting-0.4.9/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/combined_methods.py` & `pref_voting-0.4.9/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/dominance_axioms.py` & `pref_voting-0.4.9/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/generate_profiles.py` & `pref_voting-0.4.9/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/generate_spatial_profiles.py` & `pref_voting-0.4.9/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/generate_utility_profiles.py` & `pref_voting-0.4.9/pref_voting/generate_utility_profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,34 +40,42 @@
     """
 
     utilities = [{c: np.random.uniform() for c in range(num_candidates)} 
                  for _ in range(num_voters)]
     
     return UtilityProfile(utilities)
 
-def generate_utility_profile_normal(num_candidates, num_voters, std = 0.1):
+def generate_utility_profile_normal(num_candidates, num_voters, std = 0.1, normalize = None):
     """
-    Generate a utility profile where each voter assigns a random number drawn from a normal distribution with a randomly chosen mean (between 0 and 1) with standard deviation ``std`` to each candidate.  Normalize the 
+    Generate a utility profile where each voter assigns a random number drawn from a normal distribution with a randomly chosen mean (between 0 and 1) with standard deviation ``std`` to each candidate.   
     
     Args:
         num_candidates (int): The number of candidates.
         num_voters (int): The number of voters. 
         std (float): The standard deviation of the normal distribution. The default is 0.1.
+        normalize (str): The normalization method to use. The default is None.
     
     Returns:
         UtilityProfile: A utility profile.
     """
 
     utilities = list()
     
     mean_utilities = {c: np.random.uniform(0, 1) for c in range(num_candidates)}
-    utilities = [{c: np.random.normal(mean_utilities[c], std) for c in range(num_candidates)} 
-                 for _ in range(num_voters)]
+    utilities = [
+        {c: np.random.normal(mean_utilities[c], std) 
+         for c in range(num_candidates)} 
+         for _ in range(num_voters)]
     
-    return UtilityProfile(utilities).normalize()
+    if normalize == "range": 
+        return UtilityProfile(utilities).normalize_by_range()
+    elif normalize == "score":
+        return UtilityProfile(utilities).normalize_by_standard_score()
+    else: # do not normalize
+        return UtilityProfile(utilities)
 
 
 
 utility_functions = {
     "RM": {
         "func": mixed_rm_utility,
         "param": 1
```

### Comparing `pref_voting-0.4.8/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.4.9/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/helper.py` & `pref_voting-0.4.9/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/iterative_methods.py` & `pref_voting-0.4.9/pref_voting/iterative_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1781,15 +1781,15 @@
     instant_runoff_tb,
     instant_runoff_put,
     hare,
     ranked_choice,
     bottom_two_runoff_instant_runoff,
     benham,
     benham_put,
-    benham_tb
+    benham_tb,
     plurality_with_runoff,
     coombs,
     coombs_tb,
     coombs_put,
     baldwin,
     baldwin_tb,
     baldwin_put,
```

### Comparing `pref_voting-0.4.8/pref_voting/maj_graph_ex1.png` & `pref_voting-0.4.9/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/margin_based_methods.py` & `pref_voting-0.4.9/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/other_methods.py` & `pref_voting-0.4.9/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/profiles.py` & `pref_voting-0.4.9/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/profiles_with_ties.py` & `pref_voting-0.4.9/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/rankings.py` & `pref_voting-0.4.9/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/scoring_methods.py` & `pref_voting-0.4.9/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/spatial_profiles.py` & `pref_voting-0.4.9/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/utility_functions.py` & `pref_voting-0.4.9/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/utility_methods.py` & `pref_voting-0.4.9/pref_voting/utility_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     .. note::
         Before restricting to curr_cands, we normalize with respect to *all* alternatives in the domain. 
 
     """
     
     curr_cands = curr_cands if curr_cands is not None else uprof.domain
 
-    rel_utils = [u.normalize() for u in uprof.utilities]
+    rel_utils = [u.normalize_by_range() for u in uprof.utilities]
     sums = {x:np.sum([u(x) for u in rel_utils if u(x) is not None]) for x in curr_cands}
     sorted_sums = sorted(list(set(sums.values())), reverse=True)
     return Ranking({x: uidx+1 for uidx, u in enumerate(sorted_sums) 
                     for x in curr_cands if sums[x] == u})
 
 @vm(name="Relative Utilitarianism")
 def relative_utilitarian_ws(uprof, curr_cands=None):
```

### Comparing `pref_voting-0.4.8/pref_voting/utility_profiles.py` & `pref_voting-0.4.9/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/variable_voter_axioms.py` & `pref_voting-0.4.9/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/voting_method.py` & `pref_voting-0.4.9/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.4.9/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.8/pyproject.toml` & `pref_voting-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.4.8"
+version = "0.4.9"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.4.8/setup.py` & `pref_voting-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.\n- v0.4.7 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.\n- v0.4.8 (2023-5-31): Add bottom two IRV and Tideman\'s alternative voting methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-0.4.8/PKG-INFO` & `pref_voting-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.4.8
+Version: 0.4.9
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

