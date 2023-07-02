# Comparing `tmp/aleksis_app_buelleten-2.0.dev0.tar.gz` & `tmp/aleksis_app_buelleten-2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_buelleten-2.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_buelleten-2.0.dev1.tar", max compression
```

## Comparing `aleksis_app_buelleten-2.0.dev0.tar` & `aleksis_app_buelleten-2.0.dev1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      685 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1205 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/README.rst
--rw-r--r--   0        0        0      155 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/__init__.py
--rw-r--r--   0        0        0     1459 2022-08-10 18:11:25.887031 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/apps.py
--rw-r--r--   0        0        0      176 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/filters.py
--rw-r--r--   0        0        0      651 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/forms.py
--rw-r--r--   0        0        0     3675 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/frontend/index.js
--rw-r--r--   0        0        0      129 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/.keepdir
--rw-r--r--   0        0        0     4965 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4881 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4866 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0001_initial.py
--rw-r--r--   0        0        0     1491 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/__init__.py
--rw-r--r--   0        0        0     1991 2022-08-08 18:24:51.742024 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/base.py
--rw-r--r--   0        0        0     1184 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/slides.py
--rw-r--r--   0        0        0     2776 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/rules.py
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/static/.keepdir
--rw-r--r--   0        0        0     1444 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/tables.py
--rw-r--r--   0        0        0      477 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display/create.html
--rw-r--r--   0        0        0      473 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display/edit.html
--rw-r--r--   0        0        0      489 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/create.html
--rw-r--r--   0        0        0      485 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/edit.html
--rw-r--r--   0        0        0     1810 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html
--rw-r--r--   0        0        0      725 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html
--rw-r--r--   0        0        0      734 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html
--rw-r--r--   0        0        0      648 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html
--rw-r--r--   0        0        0     1340 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/urls.py
--rw-r--r--   0        0        0     8975 2022-08-08 18:24:51.930023 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/views.py
--rw-r--r--   0        0        0     1549 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/tox.ini
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev0/setup.py
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      685 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1205 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/README.rst
+-rw-r--r--   0        0        0      155 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/__init__.py
+-rw-r--r--   0        0        0     1459 2022-08-10 18:11:25.887031 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/apps.py
+-rw-r--r--   0        0        0      176 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/filters.py
+-rw-r--r--   0        0        0      651 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/forms.py
+-rw-r--r--   0        0        0     3675 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/frontend/index.js
+-rw-r--r--   0        0        0      129 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/.keepdir
+-rw-r--r--   0        0        0     4965 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4881 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4866 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1491 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/migrations/0002_display_variants.py
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/migrations/__init__.py
+-rw-r--r--   0        0        0     1991 2022-08-08 18:24:51.742024 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/models/base.py
+-rw-r--r--   0        0        0     1184 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/models/slides.py
+-rw-r--r--   0        0        0     2776 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/rules.py
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/static/.keepdir
+-rw-r--r--   0        0        0     1444 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/tables.py
+-rw-r--r--   0        0        0      477 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display/create.html
+-rw-r--r--   0        0        0      473 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display/edit.html
+-rw-r--r--   0        0        0      489 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/create.html
+-rw-r--r--   0        0        0      485 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/edit.html
+-rw-r--r--   0        0        0     1810 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/full.html
+-rw-r--r--   0        0        0      725 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/list.html
+-rw-r--r--   0        0        0      734 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/slide/create.html
+-rw-r--r--   0        0        0      648 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/slide/edit.html
+-rw-r--r--   0        0        0     1340 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/urls.py
+-rw-r--r--   0        0        0     8975 2022-08-08 18:24:51.930023 aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/views.py
+-rw-r--r--   0        0        0     1549 2023-07-02 18:38:22.704857 aleksis_app_buelleten-2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev1/tox.ini
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev1/setup.py
+-rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_buelleten-2.0.dev0/CHANGELOG.rst` & `aleksis_app_buelleten-2.0.dev1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/LICENCE.rst` & `aleksis_app_buelleten-2.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/README.rst` & `aleksis_app_buelleten-2.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/apps.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/forms.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/frontend/index.js` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0001_initial.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/migrations/0002_display_variants.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/base.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/models/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/slides.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/models/slides.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/rules.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/tables.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/display_group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/slide/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/templates/buelleten/slide/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/urls.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/views.py` & `aleksis_app_buelleten-2.0.dev1/aleksis/apps/buelleten/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/pyproject.toml` & `aleksis_app_buelleten-2.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Buelleten"
-version = "2.0.dev0"
+version = "2.0.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -26,15 +26,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = {version = ">=3.0, <3.1", allow-prereleases = true }
+aleksis-core = {version = ">=3.0, <3.2", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = {version=">=2023.1.dev0", allow-prereleases=true}
 
 [tool.poetry.plugins."aleksis.app"]
 buelleten = "aleksis.apps.buelleten.apps:DefaultConfig"
```

### Comparing `aleksis_app_buelleten-2.0.dev0/tox.ini` & `aleksis_app_buelleten-2.0.dev1/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_buelleten-2.0.dev0/setup.py` & `aleksis_app_buelleten-2.0.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,22 @@
                             'locale/tr_TR/LC_MESSAGES/*',
                             'static/*',
                             'templates/buelleten/display/*',
                             'templates/buelleten/display_group/*',
                             'templates/buelleten/slide/*']}
 
 install_requires = \
-['aleksis-core>=3.0,<3.1']
+['aleksis-core>=3.0,<3.2']
 
 entry_points = \
 {'aleksis.app': ['buelleten = aleksis.apps.buelleten.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-buelleten',
-    'version': '2.0.dev0',
+    'version': '2.0.dev1',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Bülleten (Digital Signage)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Bülleten (Digital Signage)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2021 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_buelleten-2.0.dev0/PKG-INFO` & `aleksis_app_buelleten-2.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aleksis-app-buelleten
-Version: 2.0.dev0
+Version: 2.0.dev1
 Summary: AlekSIS (School Information System) — App Bülleten (Digital Signage)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=3.0,<3.1)
+Requires-Dist: aleksis-core (>=3.0,<3.2)
 Project-URL: Documentation, https://aleksis.edugit.io/official/AlekSIS-Core/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Buelleten
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Bülleten (Digital Signage)
 ==================================================================================================
```

