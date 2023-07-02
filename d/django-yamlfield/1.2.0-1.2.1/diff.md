# Comparing `tmp/django-yamlfield-1.2.0.tar.gz` & `tmp/django-yamlfield-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-yamlfield-1.2.0.tar", last modified: Thu May 26 12:48:28 2022, max compression
+gzip compressed data, was "django-yamlfield-1.2.1.tar", last modified: Sun Jul  2 10:58:40 2023, max compression
```

## Comparing `django-yamlfield-1.2.0.tar` & `django-yamlfield-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.314451 django-yamlfield-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/.github/workflows/continuous-deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    36453 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/django_yamlfield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-05-26 12:48:27.000000 django-yamlfield-1.2.0/django_yamlfield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-26 12:48:28.000000 django-yamlfield-1.2.0/django_yamlfield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 12:48:27.000000 django-yamlfield-1.2.0/django_yamlfield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-26 12:48:27.000000 django-yamlfield-1.2.0/django_yamlfield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-26 12:48:28.000000 django-yamlfield-1.2.0/django_yamlfield.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.314451 django-yamlfield-1.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-26 12:48:28.322451 django-yamlfield-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 12:48:28.318451 django-yamlfield-1.2.0/yamlfield/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-05-26 12:47:01.000000 django-yamlfield-1.2.0/yamlfield/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.321113 django-yamlfield-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.321113 django-yamlfield-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/.github/workflows/continuous-deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38266 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/django_yamlfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-02 10:58:40.000000 django-yamlfield-1.2.1/django_yamlfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-02 10:58:40.000000 django-yamlfield-1.2.1/django_yamlfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:58:40.000000 django-yamlfield-1.2.1/django_yamlfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 10:58:40.000000 django-yamlfield-1.2.1/django_yamlfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 10:58:40.000000 django-yamlfield-1.2.1/django_yamlfield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.321113 django-yamlfield-1.2.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:40.325114 django-yamlfield-1.2.1/yamlfield/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-02 10:58:23.000000 django-yamlfield-1.2.1/yamlfield/tests.py
```

### Comparing `django-yamlfield-1.2.0/.github/workflows/continuous-deployment.yaml` & `django-yamlfield-1.2.1/.github/workflows/continuous-deployment.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 name: Test
+
 on:
   push:
   workflow_dispatch:
 
 jobs:
   lint-python:
     name: Lint
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Install pipenv
         run: pipx install pipenv
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install --dev --python `which python`
 
       - id: run
         name: Run
         run: pipenv run flake8 yamlfield
 
   test-python:
     strategy:
       matrix:
-        python: ['3.7', '3.8', '3.9', '3.10']
-        django: ['3.1', '4.0']
-        exclude:
-        - python: '3.7'
-          django: '4.0'
+        python: ['3.8', '3.9', '3.10', '3.11']
+        django: ['3.2', '4.1', '4.2']
     name: Test
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Install pipenv
         run: pipx install pipenv
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           cache: 'pipenv'
 
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install pyyaml Django~=${{ matrix.django }} --python ${{ matrix.python }} --skip-lock
@@ -60,22 +58,22 @@
 
   test-build:
     name: Build Python package
     runs-on: ubuntu-latest
     needs: [test-python]
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Install pipenv
         run: pipx install pipenv
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv install --dev --python `which python`
 
       - id: build
@@ -88,33 +86,33 @@
       - id: check
         name: Check release
         run: |
             pipenv run twine check dist/*
 
       - id: save
         name: Save artifact
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: test-release-${{ github.run_number }}
           path: ./dist
           if-no-files-found: error
 
   tag-release:
     name: Tagged PyPI release
     runs-on: ubuntu-latest
     needs: [test-build]
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     steps:
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
 
       - id: fetch
         name: Fetch artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: test-release-${{ github.run_number }}
           path: ./dist
 
       - id: publish
         name: Publish release
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `django-yamlfield-1.2.0/.github/workflows/docs.yaml` & `django-yamlfield-1.2.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/.pre-commit-config.yaml` & `django-yamlfield-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/LICENSE` & `django-yamlfield-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/PKG-INFO` & `django-yamlfield-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: django-yamlfield
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Django database field for storing YAML data
 Home-page: https://palewi.re/docs/django-yamlfield/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, https://palewi.re/docs/django-yamlfield/
-Project-URL: Source, https://github.com/datadesk/django-yamlfield/
-Project-URL: Tracker, https://github.com/datadesk/django-yamlfield/issues
+Project-URL: Source, https://github.com/palewire/django-yamlfield/
+Project-URL: Tracker, https://github.com/palewire/django-yamlfield/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Links
 
 * Docs: [palewi.re/docs/django-yamlfield/](https://palewi.re/docs/django-yamlfield/)
```

### Comparing `django-yamlfield-1.2.0/Pipfile.lock` & `django-yamlfield-1.2.1/Pipfile.lock`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8691181657848324%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'10ec14868b3bb859e7bce25643e40eff53dbf51fb51d6dd6626b82a01b5d6dd3'}, 'requires': "*

 * *            "{'python_version': '3.10'}}",*

 * * "'default'": "{'asgiref': {'hashes': "*

 * *              "['sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e', "*

 * *              "'sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed'], "*

 * *              "'version': '==3.7.2'}, 'django': {'hashes': "*

 * *              "['sha256:2a6b6fbff5b59dd07bef10bcb01 […]*

```diff
@@ -1,552 +1,566 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1dc9017f559c7e416ab1ec1457daed49d5847a6a5be9a5f63a25eaf2c1a4d457"
+            "sha256": "10ec14868b3bb859e7bce25643e40eff53dbf51fb51d6dd6626b82a01b5d6dd3"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "asgiref": {
             "hashes": [
-                "sha256:1d2880b792ae8757289136f1db2b7b99100ce959b2aa57fd69dab783d05afac4",
-                "sha256:4a29362a6acebe09bf1d6640db38c1dc3d9217c68e6f9f6204d72667fc19a424"
+                "sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e",
+                "sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.2"
+            "version": "==3.7.2"
         },
         "django": {
             "hashes": [
-                "sha256:07c8638e7a7f548dc0acaaa7825d84b7bd42b10e8d22268b3d572946f1e9b687",
-                "sha256:4e8177858524417563cc0430f29ea249946d831eacb0068a1455686587df40b5"
+                "sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf",
+                "sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5"
             ],
             "index": "pypi",
-            "version": "==4.0.4"
+            "version": "==4.2.2"
         },
         "pyyaml": {
             "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
                 "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
                 "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
                 "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
                 "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
                 "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
                 "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
                 "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
                 "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
                 "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
                 "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
                 "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
                 "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
                 "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
                 "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
                 "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
                 "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
                 "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
                 "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
                 "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
                 "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
                 "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
                 "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
                 "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "sqlparse": {
             "hashes": [
-                "sha256:0c00730c74263a94e5a9919ade150dfc3b19c574389985446148402998287dae",
-                "sha256:48719e356bb8b42991bdbb1e8b83223757b93789c00910a616a071910ca4a64d"
+                "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3",
+                "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==0.4.2"
+            "version": "==0.4.4"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==4.7.0"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "babel": {
             "hashes": [
-                "sha256:3f349e85ad3154559ac4930c3918247d319f21910d5ce4b25d439ed8693b98d2",
-                "sha256:98aeaca086133efb3e1e2aad0396987490c8425929ddbcfe0550184fdc54cd13"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.10.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "bleach": {
             "hashes": [
-                "sha256:08a1fe86d253b5c88c92cc3d810fd8048a16d15762e1e5b74d502256e5926aa1",
-                "sha256:c6d6cc054bdc9c83b48b8083e236e5f00f238428666d2ce2e083eaa5fd568565"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==5.0.0"
+            "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:9c5705e395cd70084351dd8ad5c41e65655e08ce46f2ec9cf6c2c08390f71eb7",
-                "sha256:f1d53542ee8cbedbe2118b5686372fb33c297fcd6379b050cca0ef13a597382a"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.5.18.1"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3",
-                "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2",
-                "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636",
-                "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20",
-                "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728",
-                "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27",
-                "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66",
-                "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443",
-                "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0",
-                "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7",
-                "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39",
-                "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605",
-                "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a",
-                "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37",
-                "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029",
-                "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139",
-                "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc",
-                "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df",
-                "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14",
-                "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880",
-                "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2",
-                "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a",
-                "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e",
-                "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474",
-                "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024",
-                "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8",
-                "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0",
-                "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e",
-                "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a",
-                "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e",
-                "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032",
-                "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6",
-                "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e",
-                "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b",
-                "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e",
-                "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954",
-                "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962",
-                "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c",
-                "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4",
-                "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55",
-                "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962",
-                "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023",
-                "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c",
-                "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6",
-                "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8",
-                "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382",
-                "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7",
-                "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc",
-                "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
-                "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
-            ],
-            "version": "==1.15.0"
+            "version": "==2023.5.7"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.12"
-        },
-        "commonmark": {
-            "hashes": [
-                "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
-                "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
-            ],
-            "version": "==0.9.1"
-        },
-        "cryptography": {
-            "hashes": [
-                "sha256:093cb351031656d3ee2f4fa1be579a8c69c754cf874206be1d4cf3b542042804",
-                "sha256:0cc20f655157d4cfc7bada909dc5cc228211b075ba8407c46467f63597c78178",
-                "sha256:1b9362d34363f2c71b7853f6251219298124aa4cc2075ae2932e64c91a3e2717",
-                "sha256:1f3bfbd611db5cb58ca82f3deb35e83af34bb8cf06043fa61500157d50a70982",
-                "sha256:2bd1096476aaac820426239ab534b636c77d71af66c547b9ddcd76eb9c79e004",
-                "sha256:31fe38d14d2e5f787e0aecef831457da6cec68e0bb09a35835b0b44ae8b988fe",
-                "sha256:3b8398b3d0efc420e777c40c16764d6870bcef2eb383df9c6dbb9ffe12c64452",
-                "sha256:3c81599befb4d4f3d7648ed3217e00d21a9341a9a688ecdd615ff72ffbed7336",
-                "sha256:419c57d7b63f5ec38b1199a9521d77d7d1754eb97827bbb773162073ccd8c8d4",
-                "sha256:46f4c544f6557a2fefa7ac8ac7d1b17bf9b647bd20b16decc8fbcab7117fbc15",
-                "sha256:471e0d70201c069f74c837983189949aa0d24bb2d751b57e26e3761f2f782b8d",
-                "sha256:59b281eab51e1b6b6afa525af2bd93c16d49358404f814fe2c2410058623928c",
-                "sha256:731c8abd27693323b348518ed0e0705713a36d79fdbd969ad968fbef0979a7e0",
-                "sha256:95e590dd70642eb2079d280420a888190aa040ad20f19ec8c6e097e38aa29e06",
-                "sha256:a68254dd88021f24a68b613d8c51d5c5e74d735878b9e32cc0adf19d1f10aaf9",
-                "sha256:a7d5137e556cc0ea418dca6186deabe9129cee318618eb1ffecbd35bee55ddc1",
-                "sha256:aeaba7b5e756ea52c8861c133c596afe93dd716cbcacae23b80bc238202dc023",
-                "sha256:dc26bb134452081859aa21d4990474ddb7e863aa39e60d1592800a8865a702de",
-                "sha256:e53258e69874a306fcecb88b7534d61820db8a98655662a3dd2ec7f1afd9132f",
-                "sha256:ef15c2df7656763b4ff20a9bc4381d8352e6640cfeb95c2972c38ef508e75181",
-                "sha256:f224ad253cc9cea7568f49077007d2263efa57396a2f2f78114066fd54b5c68e",
-                "sha256:f8ec91983e638a9bcd75b39f1396e5c0dc2330cbd9ce4accefe68717e6779e0a"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==37.0.2"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "version": "==0.3.4"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125",
-                "sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==0.17.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:b795f1b42a61bbf8ec7113c341dad679d772567b936fbd1bf43c9a238e673e20",
-                "sha256:c7b5fdb219b398a5b28c8e4c1893ef5f98ece6a38c6ab2c22e26ec161556fed6"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:479b1304f72536a55948cb40a32dce8bb0ffe3501e26eaf292c7e60eb5e0428d",
-                "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
+                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
+                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
-            "version": "==4.0.1"
+            "version": "==6.0.0"
         },
         "identify": {
             "hashes": [
-                "sha256:0dca2ea3e4381c435ef9c33ba100a78a9b40c0bab11189c7cf121f75815efeaa",
-                "sha256:3d11b16f3fe19f52039fb7e39c9c884b21cb1b586988114fbe42671f03de3e82"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.1"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
-                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
-                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:5d26852efe48c0a32b0509ffbc583fda1a2266545a78d104a6f4aff3db17d700",
-                "sha256:c58c8eb8a762858f49e18436ff552e83914778e50e9d2f1660535ffb364552ec"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.11.4"
+            "version": "==6.7.0"
         },
-        "jeepney": {
+        "jaraco.classes": {
             "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
+                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.2.3"
         },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:9ef58314bcc823f426b49ec787539a2d73571b37de4cd498f839803b01acff1e",
-                "sha256:dee502cdf18a98211bef428eea11456a33c00718b2f08524fd5727c7f424bffd"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.5.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
+        },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
+        },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
+        "more-itertools": {
+            "hashes": [
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==9.1.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:3ef13ff90291ba2a4a7a4ff9a979b63ffdd00a464dbe04acf0ea6471517a4c2b",
-                "sha256:621e6b7076565ddcacd2db0294c0381e01fd28945ab36bcf00f41c5daf63bef7"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
-            "version": "==1.6.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
-                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
-                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
-            "version": "==1.8.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:027d8e83a2d7de06bbac4e5ef7e023c02b863d7ea5d079477e722bb41ab25788",
-                "sha256:58c8abb07dcb441e6ee4b11d8df0ac856038f944ab98b7be6b27b2a3c7feef19"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.2"
+            "version": "==3.8.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:10c62741aa5704faea2ad69cb550ca78082efe5697d6f04e5710c3c229afdd10",
-                "sha256:4233a1e38621c87d9dda9808c6606d7e7ba0e087cd56d3fe03202a01d2919615"
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
-            "version": "==2.19.0"
+            "version": "==3.3.3"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
-                "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.8.0"
-        },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
+                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
-            "version": "==2.21"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.10.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c",
-                "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.4.0"
-        },
-        "pygments": {
-            "hashes": [
-                "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb",
-                "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"
+                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
+                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.12.0"
+            "version": "==3.0.1"
         },
-        "pyparsing": {
-            "hashes": [
-                "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
-                "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
-            ],
-            "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.0.9"
-        },
-        "pytz": {
+        "pygments": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "version": "==2022.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyyaml": {
             "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
                 "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
                 "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
                 "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
                 "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
                 "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
                 "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
                 "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
                 "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
                 "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
                 "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
                 "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
                 "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
                 "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
                 "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
                 "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
                 "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
                 "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
                 "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
                 "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
                 "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
                 "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
                 "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
                 "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:73b84905d091c31f36e50b4ae05ae2acead661f6a09a9abb4df7d2ddcdb6a698",
-                "sha256:a727999acfc222fc21d82a12ed48c957c4989785e5865807c65a487d21677497"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==35.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==2.27.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
-                "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
-            "version": "==0.9.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:4c586de507202505346f3e32d1363eb9ed6932f0c2f63184dea88983ff4971e2",
-                "sha256:d2bbd99c320a2532ac71ff6a3164867884357da3e3301f0240090c5d2fdac7ec"
-            ],
-            "markers": "python_version < '4' and python_full_version >= '3.6.3'",
-            "version": "==12.4.4"
-        },
-        "secretstorage": {
-            "hashes": [
-                "sha256:0a8eb9645b320881c222e827c26f4cfcf55363e8b374a021981ef886657a912f",
-                "sha256:755dc845b6ad76dcbcbc07ea3da75ae54bb1ea529eb72d15f83d26499a5df319"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.2"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:68e45d17c9281ba25dc0104eadd2647172b3472d9e01f911efa57965e8d51a36",
-                "sha256:a43bdedf853c670e5fed28e5623403bad2f73cf02f9a2774e91def6bda8265a7"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==62.3.2"
+            "version": "==68.0.0"
         },
         "setuptools-scm": {
             "hashes": [
-                "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
-                "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
+                "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
+                "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
-            "version": "==6.4.2"
+            "version": "==7.1.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -557,43 +571,43 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:7bf8ca9637a4ee15af412d1a1d9689fec70523a68ca9bb9127c2f3eeb344e2e6",
-                "sha256:ebf612653238bcc8f4359627a9b7ce44ede6fdd75d9d30f68255c7383d3a6226"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "index": "pypi",
-            "version": "==4.5.0"
+            "version": "==7.0.1"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -611,64 +625,64 @@
             "hashes": [
                 "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.2"
-        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "twine": {
             "hashes": [
-                "sha256:6f7496cf14a3a8903474552d5271c79c71916519edb42554f23f42a8563498a9",
-                "sha256:817aa0c0bdc02a5ebe32051e168e23c71a0608334e624c793011f120dbbc05b7"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==4.0.0"
+            "version": "==4.0.2"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==4.7.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:e617f16e25b42eb4f6e74096b9c9e37713cf10bf30168fb4a739f3fa8f898a3a",
-                "sha256:ef589a79795589aada0c1c5b319486797c03b67ac3984c48c669c0e4f50df3a5"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.14.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.23.1"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:56bf8aadb83c24db6c4b577e13de374ccfb67da2078beba1d037c17980bf43ad",
-                "sha256:c4f6e5bbf48e74f7a38e7cc5b0480ff42b0ae5178957d564d18932525d5cf099"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `django-yamlfield-1.2.0/django_yamlfield.egg-info/PKG-INFO` & `django-yamlfield-1.2.1/django_yamlfield.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: django-yamlfield
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Django database field for storing YAML data
 Home-page: https://palewi.re/docs/django-yamlfield/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, https://palewi.re/docs/django-yamlfield/
-Project-URL: Source, https://github.com/datadesk/django-yamlfield/
-Project-URL: Tracker, https://github.com/datadesk/django-yamlfield/issues
+Project-URL: Source, https://github.com/palewire/django-yamlfield/
+Project-URL: Tracker, https://github.com/palewire/django-yamlfield/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Links
 
 * Docs: [palewi.re/docs/django-yamlfield/](https://palewi.re/docs/django-yamlfield/)
```

### Comparing `django-yamlfield-1.2.0/django_yamlfield.egg-info/SOURCES.txt` & `django-yamlfield-1.2.1/django_yamlfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/Makefile` & `django-yamlfield-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/_static/css/custom.css` & `django-yamlfield-1.2.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/_templates/nav.html` & `django-yamlfield-1.2.1/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/conf.py` & `django-yamlfield-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/index.md` & `django-yamlfield-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/docs/make.bat` & `django-yamlfield-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/setup.py` & `django-yamlfield-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,27 +78,28 @@
     include_package_data=True,
     license="MIT",
     install_requires=("PyYAML>=3.10"),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django",
-        "Framework :: Django :: 3.1",
-        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "License :: OSI Approved :: MIT License",
     ],
     cmdclass={
         "test": TestCommand,
     },
     setup_requires=["setuptools_scm"],
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     project_urls={
         "Documentation": "https://palewi.re/docs/django-yamlfield/",
-        "Source": "https://github.com/datadesk/django-yamlfield/",
-        "Tracker": "https://github.com/datadesk/django-yamlfield/issues",
+        "Source": "https://github.com/palewire/django-yamlfield/",
+        "Tracker": "https://github.com/palewire/django-yamlfield/issues",
     },
 )
```

### Comparing `django-yamlfield-1.2.0/yamlfield/fields.py` & `django-yamlfield-1.2.1/yamlfield/fields.py`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/yamlfield/serializers.py` & `django-yamlfield-1.2.1/yamlfield/serializers.py`

 * *Files identical despite different names*

### Comparing `django-yamlfield-1.2.0/yamlfield/tests.py` & `django-yamlfield-1.2.1/yamlfield/tests.py`

 * *Files identical despite different names*

