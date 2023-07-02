# Comparing `tmp/suisa_sendemeldung-0.9.1.tar.gz` & `tmp/suisa_sendemeldung-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suisa_sendemeldung-0.9.1.tar", last modified: Mon Mar  6 16:38:17 2023, max compression
+gzip compressed data, was "suisa_sendemeldung-0.9.2.tar", last modified: Fri Mar 10 15:35:37 2023, max compression
```

## Comparing `suisa_sendemeldung-0.9.1.tar` & `suisa_sendemeldung-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.github/workflows/lint-and-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.github/workflows/semantic-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/suisa_sendemeldung.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/etc/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/sysconfig/suisa_sendemeldung
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/etc/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/systemd/suisa_sendemeldung.docker.service
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/systemd/suisa_sendemeldung.docker.timer
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/systemd/suisa_sendemeldung.service
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/etc/systemd/suisa_sendemeldung.timer
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/suisa_sendemeldung/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung/acrclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung/suisa_sendemeldung.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:38:17.000000 suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:38:17.864811 suisa_sendemeldung-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/tests/test_acrclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-03-06 16:37:59.000000 suisa_sendemeldung-0.9.1/tests/test_suisa_sendemeldung.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.github/workflows/lint-and-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.github/workflows/semantic-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/suisa_sendemeldung.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/etc/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/sysconfig/suisa_sendemeldung
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/etc/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/systemd/suisa_sendemeldung.docker.service
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/systemd/suisa_sendemeldung.docker.timer
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/systemd/suisa_sendemeldung.service
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/etc/systemd/suisa_sendemeldung.timer
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/suisa_sendemeldung/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung/acrclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung/suisa_sendemeldung.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 15:35:37.000000 suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 15:35:37.312580 suisa_sendemeldung-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/tests/test_acrclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-03-10 15:35:11.000000 suisa_sendemeldung-0.9.2/tests/test_suisa_sendemeldung.py
```

### Comparing `suisa_sendemeldung-0.9.1/.flake8` & `suisa_sendemeldung-0.9.2/.flake8`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/.github/dependabot.yml` & `suisa_sendemeldung-0.9.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/.github/workflows/lint-and-test.yaml` & `suisa_sendemeldung-0.9.2/.github/workflows/lint-and-test.yaml`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/.github/workflows/release.yaml` & `suisa_sendemeldung-0.9.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/.gitignore` & `suisa_sendemeldung-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/.pre-commit-config.yaml` & `suisa_sendemeldung-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/LICENSE` & `suisa_sendemeldung-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/README.md` & `suisa_sendemeldung-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/etc/suisa_sendemeldung.conf` & `suisa_sendemeldung-0.9.2/etc/suisa_sendemeldung.conf`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/setup.py` & `suisa_sendemeldung-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/suisa_sendemeldung/acrclient.py` & `suisa_sendemeldung-0.9.2/suisa_sendemeldung/acrclient.py`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/suisa_sendemeldung/suisa_sendemeldung.py` & `suisa_sendemeldung-0.9.2/suisa_sendemeldung/suisa_sendemeldung.py`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/suisa_sendemeldung.egg-info/SOURCES.txt` & `suisa_sendemeldung-0.9.2/suisa_sendemeldung.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/tests/test_acrclient.py` & `suisa_sendemeldung-0.9.2/tests/test_acrclient.py`

 * *Files identical despite different names*

### Comparing `suisa_sendemeldung-0.9.1/tests/test_suisa_sendemeldung.py` & `suisa_sendemeldung-0.9.2/tests/test_suisa_sendemeldung.py`

 * *Files identical despite different names*

