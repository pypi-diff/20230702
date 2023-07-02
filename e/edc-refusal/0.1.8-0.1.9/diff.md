# Comparing `tmp/edc-refusal-0.1.8.tar.gz` & `tmp/edc-refusal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-refusal-0.1.8.tar", last modified: Tue Aug 23 02:21:30 2022, max compression
+gzip compressed data, was "edc-refusal-0.1.9.tar", last modified: Thu Sep 15 02:07:26 2022, max compression
```

## Comparing `edc-refusal-0.1.8.tar` & `edc-refusal-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.036503 edc-refusal-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       93 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.028707 edc-refusal-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.031891 edc-refusal-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1944 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-14 21:14:37.000000 edc-refusal-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1655 2022-08-23 02:21:30.036607 edc-refusal-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      689 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-23 02:21:22.000000 edc-refusal-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.033656 edc-refusal-0.1.8/edc_refusal/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2074 2022-08-23 02:21:22.000000 edc-refusal-0.1.8/edc_refusal/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      278 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      273 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2854 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/edc_refusal/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.034929 edc-refusal-0.1.8/edc_refusal/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     7966 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6792 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/edc_refusal/migrations/0002_historicalsubjectrefusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)      815 2022-07-06 07:04:07.000000 edc-refusal-0.1.8/edc_refusal/migrations/0003_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/model_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1852 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.035131 edc-refusal-0.1.8/edc_refusal/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.036172 edc-refusal-0.1.8/edc_refusal/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      375 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.036382 edc-refusal-0.1.8/edc_refusal/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1079 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/tests/tests/test_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/edc_refusal/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:21:30.034213 edc-refusal-0.1.8/edc_refusal.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1655 2022-08-23 02:21:29.000000 edc-refusal-0.1.8/edc_refusal.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1326 2022-08-23 02:21:30.000000 edc-refusal-0.1.8/edc_refusal.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 02:21:29.000000 edc-refusal-0.1.8/edc_refusal.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-14 21:40:13.000000 edc-refusal-0.1.8/edc_refusal.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       12 2022-08-23 02:21:29.000000 edc-refusal-0.1.8/edc_refusal.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1707 2022-08-16 16:52:27.000000 edc-refusal-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1621 2022-06-01 23:31:30.000000 edc-refusal-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1241 2022-08-23 02:21:30.036930 edc-refusal-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.288099 edc-refusal-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       93 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.279615 edc-refusal-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.283006 edc-refusal-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1944 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-15 02:07:18.000000 edc-refusal-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-14 21:14:37.000000 edc-refusal-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1655 2022-09-15 02:07:26.288214 edc-refusal-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      689 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-15 02:07:18.000000 edc-refusal-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.284928 edc-refusal-0.1.9/edc_refusal/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2074 2022-08-23 02:21:22.000000 edc-refusal-0.1.9/edc_refusal/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      278 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      273 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2854 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/edc_refusal/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.286300 edc-refusal-0.1.9/edc_refusal/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     7966 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6792 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/edc_refusal/migrations/0002_historicalsubjectrefusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      815 2022-07-06 07:04:07.000000 edc-refusal-0.1.9/edc_refusal/migrations/0003_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-09-15 02:07:18.000000 edc-refusal-0.1.9/edc_refusal/migrations/0004_refusalreasons_plural_name.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/model_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1852 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.286711 edc-refusal-0.1.9/edc_refusal/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.287766 edc-refusal-0.1.9/edc_refusal/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      375 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.287981 edc-refusal-0.1.9/edc_refusal/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1079 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/tests/tests/test_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/edc_refusal/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:07:26.285485 edc-refusal-0.1.9/edc_refusal.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1655 2022-09-15 02:07:26.000000 edc-refusal-0.1.9/edc_refusal.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1384 2022-09-15 02:07:26.000000 edc-refusal-0.1.9/edc_refusal.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-15 02:07:26.000000 edc-refusal-0.1.9/edc_refusal.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-14 21:40:13.000000 edc-refusal-0.1.9/edc_refusal.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       12 2022-09-15 02:07:26.000000 edc-refusal-0.1.9/edc_refusal.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1707 2022-08-16 16:52:27.000000 edc-refusal-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1621 2022-06-01 23:31:30.000000 edc-refusal-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1241 2022-09-15 02:07:26.288534 edc-refusal-0.1.9/setup.cfg
```

### Comparing `edc-refusal-0.1.8/.github/workflows/build.yml` & `edc-refusal-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/.gitignore` & `edc-refusal-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/.pre-commit-config.yaml` & `edc-refusal-0.1.9/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
```

### Comparing `edc-refusal-0.1.8/LICENSE` & `edc-refusal-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/PKG-INFO` & `edc-refusal-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-refusal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to document a subject's refusal to join a study for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-refusal
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc refusal,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-refusal-0.1.8/README.rst` & `edc-refusal-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/admin.py` & `edc-refusal-0.1.9/edc_refusal/admin.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/forms.py` & `edc-refusal-0.1.9/edc_refusal/forms.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/list_data.py` & `edc-refusal-0.1.9/edc_refusal/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/migrations/0001_initial.py` & `edc-refusal-0.1.9/edc_refusal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/migrations/0002_historicalsubjectrefusal.py` & `edc-refusal-0.1.9/edc_refusal/migrations/0002_historicalsubjectrefusal.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/migrations/0003_auto_20220704_1841.py` & `edc-refusal-0.1.9/edc_refusal/migrations/0003_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/models.py` & `edc-refusal-0.1.9/edc_refusal/models.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-local-private.pem` & `edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/tests/etc/user-rsa-restricted-private.pem` & `edc-refusal-0.1.9/edc_refusal/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal/tests/tests/test_model.py` & `edc-refusal-0.1.9/edc_refusal/tests/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/edc_refusal.egg-info/PKG-INFO` & `edc-refusal-0.1.9/edc_refusal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-refusal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to document a subject's refusal to join a study for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-refusal
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc refusal,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-refusal-0.1.8/edc_refusal.egg-info/SOURCES.txt` & `edc-refusal-0.1.9/edc_refusal.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 edc_refusal.egg-info/SOURCES.txt
 edc_refusal.egg-info/dependency_links.txt
 edc_refusal.egg-info/not-zip-safe
 edc_refusal.egg-info/top_level.txt
 edc_refusal/migrations/0001_initial.py
 edc_refusal/migrations/0002_historicalsubjectrefusal.py
 edc_refusal/migrations/0003_auto_20220704_1841.py
+edc_refusal/migrations/0004_refusalreasons_plural_name.py
 edc_refusal/migrations/__init__.py
 edc_refusal/tests/__init__.py
 edc_refusal/tests/models.py
 edc_refusal/tests/etc/user-aes-local.key
 edc_refusal/tests/etc/user-aes-restricted.key
 edc_refusal/tests/etc/user-rsa-local-private.pem
 edc_refusal/tests/etc/user-rsa-local-public.pem
```

### Comparing `edc-refusal-0.1.8/pyproject.toml` & `edc-refusal-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/runtests.py` & `edc-refusal-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-refusal-0.1.8/setup.cfg` & `edc-refusal-0.1.9/setup.cfg`

 * *Files identical despite different names*

