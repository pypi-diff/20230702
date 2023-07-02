# Comparing `tmp/lamin_logger-0.7.3.tar.gz` & `tmp/lamin_logger-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.3.tar` & `lamin_logger-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.3/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.3/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.3/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.3/docs/api.md
--rw-r--r--   0        0        0     4628 2023-06-30 14:11:53.021008 lamin_logger-0.7.3/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.3/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.3/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.3/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-30 14:11:44.881763 lamin_logger-0.7.3/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.3/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.3/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.3/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.3/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7294 2023-06-30 14:10:22.361261 lamin_logger-0.7.3/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.3/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.3/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.3/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.3/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.3/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.3/tests/test_lookup.py
--rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.3/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.3/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.3/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.4/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.4/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.4/docs/api.md
+-rw-r--r--   0        0        0     4800 2023-07-02 09:39:40.064971 lamin_logger-0.7.4/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.4/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.4/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.4/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-07-02 09:39:33.617770 lamin_logger-0.7.4/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.4/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.4/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.4/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.4/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7391 2023-07-02 09:39:13.613524 lamin_logger-0.7.4/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.4/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.4/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.4/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.4/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.4/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.4/tests/test_lookup.py
+-rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.4/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.4/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.4/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.4/PKG-INFO
```

### Comparing `lamin_logger-0.7.3/.github/workflows/build.yml` & `lamin_logger-0.7.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/.gitignore` & `lamin_logger-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/.pre-commit-config.yaml` & `lamin_logger-0.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/LICENSE` & `lamin_logger-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/docs/changelog.md` & `lamin_logger-0.7.4/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑️ Fix for multiple matches in map_synonyms | [33](https://github.com/laminlabs/lamin-logger/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-02 | 0.7.4
 🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
 🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
 ✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
```

### Comparing `lamin_logger-0.7.3/docs/quickstart.ipynb` & `lamin_logger-0.7.4/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_core.py` & `lamin_logger-0.7.4/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_inspect.py` & `lamin_logger-0.7.4/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_logger.py` & `lamin_logger-0.7.4/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_lookup.py` & `lamin_logger-0.7.4/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.4/lamin_logger/_map_synonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     mapped_df["__agg__"] = to_str(mapped_df["orig_ids"], case_sensitive=case_sensitive)
 
     # __agg__ is a column of identifiers based on case_sensitive
     df["__agg__"] = to_str(df[field], case_sensitive=case_sensitive)
     field_map = pd.merge(mapped_df, df, on="__agg__").set_index("__agg__")[field]
 
     # only runs if synonyms mapping is needed
-    if len(field_map) < mapped_df.shape[0]:
+    # unique of field_map is needed here due to possible multiple matches of identifier
+    if len(field_map.unique()) < mapped_df.shape[0]:
         # only map synonyms for those ids that don't match the field case insensitively
         # {synonym: name}
         syn_map = explode_aggregated_column_to_map(
             df=df[~df["__agg__"].isin(mapped_df["__agg__"])],
             agg_col=synonyms_field,
             target_col=field,
             keep=keep,
```

### Comparing `lamin_logger-0.7.3/lamin_logger/_python_version.py` & `lamin_logger-0.7.4/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/lamin_logger/_search.py` & `lamin_logger-0.7.4/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/pyproject.toml` & `lamin_logger-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/tests/test_inspect.py` & `lamin_logger-0.7.4/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/tests/test_lookup.py` & `lamin_logger-0.7.4/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/tests/test_map_synonyms.py` & `lamin_logger-0.7.4/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/tests/test_search.py` & `lamin_logger-0.7.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.3/PKG-INFO` & `lamin_logger-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.3
+Version: 0.7.4
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

