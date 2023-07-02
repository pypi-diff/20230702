# Comparing `tmp/AlekSIS-App-Discourse-1.0.dev0.tar.gz` & `tmp/aleksis_app_discourse-2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlekSIS-App-Discourse-1.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_discourse-2.0.dev0.tar", max compression
```

## Comparing `AlekSIS-App-Discourse-1.0.dev0.tar` & `aleksis_app_discourse-2.0.dev0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0      441 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1124 2022-09-05 19:28:06.812585 AlekSIS-App-Discourse-1.0.dev0/README.rst
--rw-r--r--   0        0        0      155 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/__init__.py
--rw-r--r--   0        0        0      429 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/apps.py
--rw-r--r--   0        0        0        0 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/locale/.keepdir
--rw-r--r--   0        0        0       41 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/menus.py
--rw-r--r--   0        0        0        0 2022-09-05 19:22:16.867272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/migrations/__init__.py
--rw-r--r--   0        0        0     2793 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/preferences.py
--rw-r--r--   0        0        0        0 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/static/.keepdir
--rw-r--r--   0        0        0     5844 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/tasks.py
--rw-r--r--   0        0        0      212 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/templates/discourse/empty.html
--rw-r--r--   0        0        0       17 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/urls.py
--rw-r--r--   0        0        0      673 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/util.py
--rw-r--r--   0        0        0     1505 2022-09-05 19:22:29.379324 AlekSIS-App-Discourse-1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2318 2022-09-05 19:22:16.871272 AlekSIS-App-Discourse-1.0.dev0/tox.ini
--rw-r--r--   0        0        0     2203 2022-09-05 19:28:09.555072 AlekSIS-App-Discourse-1.0.dev0/setup.py
--rw-r--r--   0        0        0     2060 2022-09-05 19:28:09.555273 AlekSIS-App-Discourse-1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      441 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/LICENCE.rst
+-rw-r--r--   0        0        0     1124 2022-09-05 19:28:06.812585 aleksis_app_discourse-2.0.dev0/README.rst
+-rw-r--r--   0        0        0      155 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/__init__.py
+-rw-r--r--   0        0        0      429 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/apps.py
+-rw-r--r--   0        0        0        0 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/.keepdir
+-rw-r--r--   0        0        0     2779 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2647 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2692 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2647 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2647 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2647 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0       41 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/menus.py
+-rw-r--r--   0        0        0        0 2022-09-05 19:22:16.867272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/migrations/__init__.py
+-rw-r--r--   0        0        0     2793 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/preferences.py
+-rw-r--r--   0        0        0        0 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/static/.keepdir
+-rw-r--r--   0        0        0     5844 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/tasks.py
+-rw-r--r--   0        0        0      212 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/templates/discourse/empty.html
+-rw-r--r--   0        0        0       17 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/urls.py
+-rw-r--r--   0        0        0      673 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/util.py
+-rw-r--r--   0        0        0     1505 2023-07-02 13:51:41.097643 aleksis_app_discourse-2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2318 2022-09-05 19:22:16.871272 aleksis_app_discourse-2.0.dev0/tox.ini
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 aleksis_app_discourse-2.0.dev0/setup.py
+-rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 aleksis_app_discourse-2.0.dev0/PKG-INFO
```

### Comparing `AlekSIS-App-Discourse-1.0.dev0/LICENCE.rst` & `aleksis_app_discourse-2.0.dev0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/README.rst` & `aleksis_app_discourse-2.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/preferences.py` & `aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/preferences.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/tasks.py` & `aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/tasks.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/aleksis/apps/discourse/util.py` & `aleksis_app_discourse-2.0.dev0/aleksis/apps/discourse/util.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/pyproject.toml` & `aleksis_app_discourse-2.0.dev0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Discourse"
-version = "1.0.dev0"
+version = "2.0.dev0"
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
-aleksis-core = "^2.7"
+aleksis-core = "^3.1"
 pydiscourse = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 discourse = "aleksis.apps.discourse.apps:DefaultConfig"
```

### Comparing `AlekSIS-App-Discourse-1.0.dev0/tox.ini` & `aleksis_app_discourse-2.0.dev0/tox.ini`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Discourse-1.0.dev0/setup.py` & `aleksis_app_discourse-2.0.dev0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,39 @@
 from setuptools import setup
 
 packages = \
 ['aleksis', 'aleksis.apps.discourse', 'aleksis.apps.discourse.migrations']
 
 package_data = \
 {'': ['*'],
- 'aleksis.apps.discourse': ['locale/*', 'static/*', 'templates/discourse/*']}
+ 'aleksis.apps.discourse': ['locale/*',
+                            'locale/ar/LC_MESSAGES/*',
+                            'locale/de_DE/LC_MESSAGES/*',
+                            'locale/fr/LC_MESSAGES/*',
+                            'locale/la/LC_MESSAGES/*',
+                            'locale/nb_NO/LC_MESSAGES/*',
+                            'locale/tr_TR/LC_MESSAGES/*',
+                            'static/*',
+                            'templates/discourse/*']}
 
 install_requires = \
-['aleksis-core>=2.7,<3.0', 'pydiscourse>=1.3.0,<2.0.0']
+['aleksis-core>=3.1,<4.0', 'pydiscourse>=1.3.0,<2.0.0']
 
 entry_points = \
 {'aleksis.app': ['discourse = aleksis.apps.discourse.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-discourse',
-    'version': '1.0.dev0',
+    'version': '2.0.dev0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Discourse (Integration with the Discourse discussion forum)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Discourse (Integration with the Discourse discussion forum)\n=====================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://aleksis.org',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `AlekSIS-App-Discourse-1.0.dev0/PKG-INFO` & `aleksis_app_discourse-2.0.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aleksis-app-discourse
-Version: 1.0.dev0
+Version: 2.0.dev0
 Summary: AlekSIS (School Information System) — App Discourse (Integration with the Discourse discussion forum)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=2.7,<3.0)
+Requires-Dist: aleksis-core (>=3.1,<4.0)
 Requires-Dist: pydiscourse (>=1.3.0,<2.0.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Discourse
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Discourse (Integration with the Discourse discussion forum)
 =====================================================================================================
```

