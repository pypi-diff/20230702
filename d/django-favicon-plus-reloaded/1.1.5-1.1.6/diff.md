# Comparing `tmp/django-favicon-plus-reloaded-1.1.5.tar.gz` & `tmp/django-favicon-plus-reloaded-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-favicon-plus-reloaded-1.1.5.tar", last modified: Mon Dec 20 13:56:14 2021, max compression
+gzip compressed data, was "django-favicon-plus-reloaded-1.1.6.tar", last modified: Sat Jul  1 23:12:07 2023, max compression
```

## Comparing `django-favicon-plus-reloaded-1.1.5.tar` & `django-favicon-plus-reloaded-1.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/
--rw-r--r--   0 nik       (1000) nik       (1000)      129 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/AUTHORS.txt
--rw-r--r--   0 nik       (1000) nik       (1000)     1174 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/LICENSE
--rw-r--r--   0 nik       (1000) nik       (1000)      212 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/MANIFEST.in
--rw-r--r--   0 nik       (1000) nik       (1000)     6610 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     5524 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/README.md
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)     6610 2021-12-20 13:56:14.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      705 2021-12-20 13:56:14.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2021-12-20 13:56:14.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2021-12-20 13:12:46.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/not-zip-safe
--rw-r--r--   0 nik       (1000) nik       (1000)       14 2021-12-20 13:56:14.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        8 2021-12-20 13:56:14.000000 django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/top_level.txt
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/favicon/
--rw-r--r--   0 nik       (1000) nik       (1000)       22 2021-12-20 13:53:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)      735 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/admin.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/favicon/migrations/
--rw-r--r--   0 nik       (1000) nik       (1000)     1389 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/migrations/0001_initial.py
--rw-r--r--   0 nik       (1000) nik       (1000)      668 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/migrations/0002_favicon_site.py
--rw-r--r--   0 nik       (1000) nik       (1000)     1151 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/migrations/0003_site_manager.py
--rw-r--r--   0 nik       (1000) nik       (1000)      424 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/migrations/0004_faviconimg_favicon_size_rel_unique.py
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/migrations/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     5090 2021-12-20 13:53:03.000000 django-favicon-plus-reloaded-1.1.5/favicon/models.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/favicon/templatetags/
--rw-r--r--   0 nik       (1000) nik       (1000)        0 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/templatetags/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)      528 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/favicon/templatetags/favtags.py
--rw-r--r--   0 nik       (1000) nik       (1000)       14 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/requirements.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2021-12-20 13:56:14.437946 django-favicon-plus-reloaded-1.1.5/setup.cfg
--rw-r--r--   0 nik       (1000) nik       (1000)     1458 2021-12-20 13:08:37.000000 django-favicon-plus-reloaded-1.1.5/setup.py
+drwxr-xr-x   0 wethjo    (1000) wethjo    (1000)        0 2023-07-01 23:12:07.982338 django-favicon-plus-reloaded-1.1.6/
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      129 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/AUTHORS.txt
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     1174 2021-08-25 15:19:53.000000 django-favicon-plus-reloaded-1.1.6/LICENSE
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      212 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/MANIFEST.in
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     6589 2023-07-01 23:12:07.978338 django-favicon-plus-reloaded-1.1.6/PKG-INFO
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     5524 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/README.md
+drwxr-xr-x   0 wethjo    (1000) wethjo    (1000)        0 2023-07-01 23:12:07.978338 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     6589 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      705 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)        1 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)        1 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/not-zip-safe
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)       40 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/requires.txt
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)        8 2023-07-01 23:12:07.000000 django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/top_level.txt
+drwxr-xr-x   0 wethjo    (1000) wethjo    (1000)        0 2023-07-01 23:12:07.978338 django-favicon-plus-reloaded-1.1.6/favicon/
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)       22 2023-07-01 23:11:45.000000 django-favicon-plus-reloaded-1.1.6/favicon/__init__.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      735 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/favicon/admin.py
+drwxr-xr-x   0 wethjo    (1000) wethjo    (1000)        0 2023-07-01 23:12:07.978338 django-favicon-plus-reloaded-1.1.6/favicon/migrations/
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     1389 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/favicon/migrations/0001_initial.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      668 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/favicon/migrations/0002_favicon_site.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     1151 2021-08-25 15:19:53.000000 django-favicon-plus-reloaded-1.1.6/favicon/migrations/0003_site_manager.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      424 2021-08-25 15:19:53.000000 django-favicon-plus-reloaded-1.1.6/favicon/migrations/0004_faviconimg_favicon_size_rel_unique.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)        1 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/favicon/migrations/__init__.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     5088 2023-07-01 22:59:45.000000 django-favicon-plus-reloaded-1.1.6/favicon/models.py
+drwxr-xr-x   0 wethjo    (1000) wethjo    (1000)        0 2023-07-01 23:12:07.978338 django-favicon-plus-reloaded-1.1.6/favicon/templatetags/
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)        0 2020-05-04 15:46:13.000000 django-favicon-plus-reloaded-1.1.6/favicon/templatetags/__init__.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)      528 2021-08-25 15:19:53.000000 django-favicon-plus-reloaded-1.1.6/favicon/templatetags/favtags.py
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)       42 2023-07-01 23:10:37.000000 django-favicon-plus-reloaded-1.1.6/requirements.txt
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)       38 2023-07-01 23:12:07.982338 django-favicon-plus-reloaded-1.1.6/setup.cfg
+-rw-r--r--   0 wethjo    (1000) wethjo    (1000)     1457 2023-07-01 23:05:39.000000 django-favicon-plus-reloaded-1.1.6/setup.py
```

### Comparing `django-favicon-plus-reloaded-1.1.5/LICENSE` & `django-favicon-plus-reloaded-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/PKG-INFO` & `django-favicon-plus-reloaded-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-favicon-plus-reloaded
-Version: 1.1.5
-Summary:  simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon
+Version: 1.1.6
+Summary: Simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon
 Home-page: https://edugit.org/AlekSIS/libs/django-favicon-plus
 Author: arteria GmbH
 Author-email: arteria@arteria.ch
 Maintainer: AlekSIS Team
 Maintainer-email: aleksis-dev@lists.teckids.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -145,9 +144,7 @@
 <link rel="apple-touch-icon-precomposed" sizes="57x57" href="/images/apple-touch-icon-57x57.png">
 ```
 Android versions 1.5 and 1.6 will read the second tag (with "-precomposed"), and versions 2.1 and newer will read the first tag.
 
 Google's specifications say that you should use 48x48 pixel PNGs, but you can use a large image (128x128), like Google does for its own apps.
 
 https://mathiasbynens.be/notes/touch-icons
-
-
```

### Comparing `django-favicon-plus-reloaded-1.1.5/README.md` & `django-favicon-plus-reloaded-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/PKG-INFO` & `django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-favicon-plus-reloaded
-Version: 1.1.5
-Summary:  simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon
+Version: 1.1.6
+Summary: Simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon
 Home-page: https://edugit.org/AlekSIS/libs/django-favicon-plus
 Author: arteria GmbH
 Author-email: arteria@arteria.ch
 Maintainer: AlekSIS Team
 Maintainer-email: aleksis-dev@lists.teckids.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -145,9 +144,7 @@
 <link rel="apple-touch-icon-precomposed" sizes="57x57" href="/images/apple-touch-icon-57x57.png">
 ```
 Android versions 1.5 and 1.6 will read the second tag (with "-precomposed"), and versions 2.1 and newer will read the first tag.
 
 Google's specifications say that you should use 48x48 pixel PNGs, but you can use a large image (128x128), like Google does for its own apps.
 
 https://mathiasbynens.be/notes/touch-icons
-
-
```

### Comparing `django-favicon-plus-reloaded-1.1.5/django_favicon_plus_reloaded.egg-info/SOURCES.txt` & `django-favicon-plus-reloaded-1.1.6/django_favicon_plus_reloaded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/admin.py` & `django-favicon-plus-reloaded-1.1.6/favicon/admin.py`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/migrations/0001_initial.py` & `django-favicon-plus-reloaded-1.1.6/favicon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/migrations/0002_favicon_site.py` & `django-favicon-plus-reloaded-1.1.6/favicon/migrations/0002_favicon_site.py`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/migrations/0003_site_manager.py` & `django-favicon-plus-reloaded-1.1.6/favicon/migrations/0003_site_manager.py`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/models.py` & `django-favicon-plus-reloaded-1.1.6/favicon/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     def as_html(self):
         """Return a <link> tag forthis favicon image."""
         return f'<link rel="{self.rel}" sizes="{self.size}x{self.size}" href="{self.faviconImage.url}"/>'
 
     def generate_image(self):
         tmp = Image.open(storage.open(self.faviconFK.faviconImage.name))
-        tmp.thumbnail((self.size, self.size), Image.ANTIALIAS)
+        tmp.thumbnail((self.size, self.size), Image.LANCZOS)
 
         tmp_io = BytesIO()
         tmp.save(tmp_io, format='PNG')
         file_name = f"{slugify(self.faviconFK.title)}-{self.size}s.png"
         tmp_file = InMemoryUploadedFile(tmp_io, None, file_name, 'image/png', sys.getsizeof(tmp_io), None)
 
         self.faviconImage = tmp_file
```

### Comparing `django-favicon-plus-reloaded-1.1.5/favicon/templatetags/favtags.py` & `django-favicon-plus-reloaded-1.1.6/favicon/templatetags/favtags.py`

 * *Files identical despite different names*

### Comparing `django-favicon-plus-reloaded-1.1.5/setup.py` & `django-favicon-plus-reloaded-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     name='django-favicon-plus-reloaded',
     version=version,
     url='https://edugit.org/AlekSIS/libs/django-favicon-plus',
     packages=find_packages(),
     license='MIT',
-    description=' simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon',
+    description='Simple Django app which allows you to upload a image and it renders a wide variety for html link tags to display the favicon',
     long_description=codecs.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').read().split('\n'),
     author='arteria GmbH',
     author_email='arteria@arteria.ch',
     maintainer='AlekSIS Team',
     maintainer_email='aleksis-dev@lists.teckids.org',
```

