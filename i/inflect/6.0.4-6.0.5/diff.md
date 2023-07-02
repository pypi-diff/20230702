# Comparing `tmp/inflect-6.0.4.tar.gz` & `tmp/inflect-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflect-6.0.4.tar", last modified: Thu Apr  6 02:02:04 2023, max compression
+gzip compressed data, was "inflect-6.0.5.tar", last modified: Sun Jul  2 19:10:59 2023, max compression
```

## Comparing `inflect-6.0.4.tar` & `inflect-6.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.817537 inflect-6.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-06 02:01:44.000000 inflect-6.0.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 02:01:44.000000 inflect-6.0.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-06 02:01:44.000000 inflect-6.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.813537 inflect-6.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 02:01:44.000000 inflect-6.0.4/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-06 02:01:44.000000 inflect-6.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.813537 inflect-6.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-06 02:01:44.000000 inflect-6.0.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-06 02:01:44.000000 inflect-6.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 02:01:44.000000 inflect-6.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-06 02:01:44.000000 inflect-6.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-06 02:01:44.000000 inflect-6.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-06 02:01:44.000000 inflect-6.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-04-06 02:02:04.817537 inflect-6.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-04-06 02:01:44.000000 inflect-6.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.813537 inflect-6.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-06 02:01:44.000000 inflect-6.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 02:01:44.000000 inflect-6.0.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-06 02:01:44.000000 inflect-6.0.4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.813537 inflect-6.0.4/inflect/
--rw-r--r--   0 runner    (1001) docker     (123)   103763 2023-04-06 02:01:44.000000 inflect-6.0.4/inflect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:01:44.000000 inflect-6.0.4/inflect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.817537 inflect-6.0.4/inflect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-04-06 02:02:04.000000 inflect-6.0.4/inflect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-06 02:02:04.000000 inflect-6.0.4/inflect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:02:04.000000 inflect-6.0.4/inflect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-06 02:02:04.000000 inflect-6.0.4/inflect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 02:02:04.000000 inflect-6.0.4/inflect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-06 02:01:44.000000 inflect-6.0.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-06 02:01:44.000000 inflect-6.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-06 02:01:44.000000 inflect-6.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-06 02:02:04.821537 inflect-6.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:02:04.817537 inflect-6.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/inflections.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_an.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_ancient.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_herd.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_person.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_classical_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_compounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_inflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_numwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_pl_si.py
--rw-r--r--   0 runner    (1001) docker     (123)    46037 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-06 02:01:44.000000 inflect-6.0.4/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 02:01:44.000000 inflect-6.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.721276 inflect-6.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 19:10:39.000000 inflect-6.0.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 19:10:39.000000 inflect-6.0.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-02 19:10:39.000000 inflect-6.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 19:10:39.000000 inflect-6.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 19:10:39.000000 inflect-6.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 19:10:39.000000 inflect-6.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-02 19:10:39.000000 inflect-6.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-02 19:10:39.000000 inflect-6.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-07-02 19:10:59.721276 inflect-6.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-07-02 19:10:39.000000 inflect-6.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.713276 inflect-6.0.5/inflect/
+-rw-r--r--   0 runner    (1001) docker     (123)   103763 2023-07-02 19:10:39.000000 inflect-6.0.5/inflect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:39.000000 inflect-6.0.5/inflect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.713276 inflect-6.0.5/inflect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-02 19:10:39.000000 inflect-6.0.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 19:10:39.000000 inflect-6.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-02 19:10:39.000000 inflect-6.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-02 19:10:59.721276 inflect-6.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.721276 inflect-6.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/inflections.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_an.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_compounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_inflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_numwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_pl_si.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46037 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 19:10:39.000000 inflect-6.0.5/tox.ini
```

### Comparing `inflect-6.0.4/.github/workflows/main.yml` & `inflect-6.0.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/CHANGES.rst` & `inflect-6.0.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v6.0.5
+======
+
+* Pin to Pydantic 1 to avoid breaking in Pydantic 2.
+
 v6.0.4
 ======
 
 * Internal cleanup.
 
 v6.0.3
 ======
```

### Comparing `inflect-6.0.4/LICENSE` & `inflect-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/PKG-INFO` & `inflect-6.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.0.4
+Version: 6.0.5
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.0.4/README.rst` & `inflect-6.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/docs/conf.py` & `inflect-6.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/inflect/__init__.py` & `inflect-6.0.5/inflect/__init__.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/inflect.egg-info/PKG-INFO` & `inflect-6.0.5/inflect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.0.4
+Version: 6.0.5
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.0.4/inflect.egg-info/SOURCES.txt` & `inflect-6.0.5/inflect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/pytest.ini` & `inflect-6.0.5/pytest.ini`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/setup.cfg` & `inflect-6.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Topic :: Text Processing :: Linguistic
 
 [options]
 packages = find_namespace:
 include_package_data = true
 python_requires = >=3.7
 install_requires = 
-	pydantic >= 1.9.1
+	pydantic >= 1.9.1, < 2
 keywords = plural inflect participle
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
```

### Comparing `inflect-6.0.4/tests/inflections.txt` & `inflect-6.0.5/tests/inflections.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_an.py` & `inflect-6.0.5/tests/test_an.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_all.py` & `inflect-6.0.5/tests/test_classical_all.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_ancient.py` & `inflect-6.0.5/tests/test_classical_ancient.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_herd.py` & `inflect-6.0.5/tests/test_classical_herd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_names.py` & `inflect-6.0.5/tests/test_classical_names.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_person.py` & `inflect-6.0.5/tests/test_classical_person.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_classical_zero.py` & `inflect-6.0.5/tests/test_classical_zero.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_compounds.py` & `inflect-6.0.5/tests/test_compounds.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_inflections.py` & `inflect-6.0.5/tests/test_inflections.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_join.py` & `inflect-6.0.5/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_numwords.py` & `inflect-6.0.5/tests/test_numwords.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tests/test_pwd.py` & `inflect-6.0.5/tests/test_pwd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.4/tox.ini` & `inflect-6.0.5/tox.ini`

 * *Files identical despite different names*

