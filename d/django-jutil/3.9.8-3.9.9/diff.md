# Comparing `tmp/django-jutil-3.9.8.tar.gz` & `tmp/django-jutil-3.9.9.tar.gz`

## Comparing `django-jutil-3.9.8.tar` & `django-jutil-3.9.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:09.000000 django-jutil-3.9.8/
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2021-08-25 20:57:04.000000 django-jutil-3.9.8/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)      174 2021-02-02 23:24:21.000000 django-jutil-3.9.8/requirements-dev.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)    20529 2021-08-25 20:57:04.000000 django-jutil-3.9.8/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)       92 2021-06-17 09:36:15.000000 django-jutil-3.9.8/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)       31 2021-07-15 23:57:21.000000 django-jutil-3.9.8/pyproject.toml
--rw-rw-r--   0 jani      (1000) jani      (1000)      931 2021-08-25 20:56:49.000000 django-jutil-3.9.8/setup.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:04.000000 django-jutil-3.9.8/django_jutil.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)   556077 2021-08-25 20:57:02.000000 django-jutil-3.9.8/django_jutil.egg-info/SOURCES.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)    20529 2021-08-25 20:56:53.000000 django-jutil-3.9.8/django_jutil.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-25 23:15:54.000000 django-jutil-3.9.8/django_jutil.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2021-08-25 20:56:53.000000 django-jutil-3.9.8/django_jutil.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)       92 2021-08-25 20:56:53.000000 django-jutil-3.9.8/django_jutil.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        6 2021-08-25 20:56:53.000000 django-jutil-3.9.8/django_jutil.egg-info/top_level.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)    14169 2020-11-06 20:07:34.000000 django-jutil-3.9.8/README.md
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:04.000000 django-jutil-3.9.8/jutil/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1345 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/bank_const_iban.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     9877 2021-08-11 21:04:58.000000 django-jutil-3.9.8/jutil/admin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15289 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/bank_const_fi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2614 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/cache.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11881 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/email.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    53500 2021-08-25 20:56:49.000000 django-jutil-3.9.8/jutil/tests.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:02.000000 django-jutil-3.9.8/jutil/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:02.000000 django-jutil-3.9.8/jutil/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:03.000000 django-jutil-3.9.8/jutil/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2343 2020-11-06 20:07:34.000000 django-jutil-3.9.8/jutil/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     4619 2020-11-06 20:07:34.000000 django-jutil-3.9.8/jutil/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:02.000000 django-jutil-3.9.8/jutil/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:03.000000 django-jutil-3.9.8/jutil/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)      381 2020-09-01 19:44:11.000000 django-jutil-3.9.8/jutil/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     3798 2020-11-06 20:07:34.000000 django-jutil-3.9.8/jutil/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jani      (1000) jani      (1000)    19653 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/validators.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1818 2020-12-04 19:37:11.000000 django-jutil-3.9.8/jutil/drf_exceptions.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      925 2021-07-04 14:10:51.000000 django-jutil-3.9.8/jutil/modelfields.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:04.000000 django-jutil-3.9.8/jutil/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-25 20:57:04.000000 django-jutil-3.9.8/jutil/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)      752 2021-03-28 17:47:31.000000 django-jutil-3.9.8/jutil/management/commands/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2144 2021-03-28 17:40:10.000000 django-jutil-3.9.8/jutil/management/commands/make_bank_const_dk.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5094 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/management/commands/make_bank_const_se.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      430 2021-03-28 17:47:31.000000 django-jutil-3.9.8/jutil/management/commands/geo_ip.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3099 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/management/commands/make_bank_const_fi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:46.000000 django-jutil-3.9.8/jutil/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2722 2021-03-28 17:47:31.000000 django-jutil-3.9.8/jutil/management/commands/send_email.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      831 2021-03-28 17:47:31.000000 django-jutil-3.9.8/jutil/management/commands/setpass.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1162 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/management/commands/list_files.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:46.000000 django-jutil-3.9.8/jutil/management/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      863 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/permissions.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     8729 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/xml.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       85 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    93215 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/bank_const_dk.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1668 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/testing.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3324 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/files.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2150 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/bank_const_se.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5611 2021-08-11 21:04:58.000000 django-jutil-3.9.8/jutil/command.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5913 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/middleware.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11897 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/dates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2632 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/responses.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3110 2021-08-04 21:36:41.000000 django-jutil-3.9.8/jutil/parse.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       46 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      905 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/urls.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4410 2021-08-25 20:56:49.000000 django-jutil-3.9.8/jutil/model.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3450 2021-07-15 23:57:21.000000 django-jutil-3.9.8/jutil/request.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1062 2021-07-24 18:43:47.000000 django-jutil-3.9.8/jutil/decorators.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1111 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/sms.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22897 2020-05-21 16:43:46.000000 django-jutil-3.9.8/jutil/bank_const_be.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-25 23:15:47.000000 django-jutil-3.9.8/jutil/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)    18254 2021-07-24 18:19:18.000000 django-jutil-3.9.8/jutil/format.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      348 2021-02-02 23:24:21.000000 django-jutil-3.9.8/jutil/dict.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1119 2020-11-06 20:07:34.000000 django-jutil-3.9.8/jutil/auth.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-27 20:28:20.000000 django-jutil-3.9.8/MANIFEST.in
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:46.000000 django-jutil-3.9.8/LICENSE.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:45.000000 django-jutil-3.9.9/
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2021-08-26 16:33:39.000000 django-jutil-3.9.9/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)      174 2021-02-02 23:24:21.000000 django-jutil-3.9.9/requirements-dev.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20529 2021-08-26 16:33:39.000000 django-jutil-3.9.9/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)       92 2021-06-17 09:36:15.000000 django-jutil-3.9.9/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)       31 2021-07-15 23:57:21.000000 django-jutil-3.9.9/pyproject.toml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      931 2021-08-26 16:33:25.000000 django-jutil-3.9.9/setup.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:39.000000 django-jutil-3.9.9/django_jutil.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)   556077 2021-08-26 16:33:38.000000 django-jutil-3.9.9/django_jutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20529 2021-08-26 16:33:27.000000 django-jutil-3.9.9/django_jutil.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-25 23:15:54.000000 django-jutil-3.9.9/django_jutil.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2021-08-26 16:33:27.000000 django-jutil-3.9.9/django_jutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)       92 2021-08-26 16:33:27.000000 django-jutil-3.9.9/django_jutil.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        6 2021-08-26 16:33:27.000000 django-jutil-3.9.9/django_jutil.egg-info/top_level.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)    14169 2020-11-06 20:07:34.000000 django-jutil-3.9.9/README.md
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:39.000000 django-jutil-3.9.9/jutil/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1345 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/bank_const_iban.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9877 2021-08-11 21:04:58.000000 django-jutil-3.9.9/jutil/admin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15289 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/bank_const_fi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2614 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/cache.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11881 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/email.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    53500 2021-08-25 20:56:49.000000 django-jutil-3.9.9/jutil/tests.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:38.000000 django-jutil-3.9.9/jutil/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:38.000000 django-jutil-3.9.9/jutil/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:38.000000 django-jutil-3.9.9/jutil/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2343 2020-11-06 20:07:34.000000 django-jutil-3.9.9/jutil/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4619 2020-11-06 20:07:34.000000 django-jutil-3.9.9/jutil/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:38.000000 django-jutil-3.9.9/jutil/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:38.000000 django-jutil-3.9.9/jutil/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      381 2020-09-01 19:44:11.000000 django-jutil-3.9.9/jutil/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3798 2020-11-06 20:07:34.000000 django-jutil-3.9.9/jutil/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19653 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/validators.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1818 2020-12-04 19:37:11.000000 django-jutil-3.9.9/jutil/drf_exceptions.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      925 2021-07-04 14:10:51.000000 django-jutil-3.9.9/jutil/modelfields.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:39.000000 django-jutil-3.9.9/jutil/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-08-26 16:33:39.000000 django-jutil-3.9.9/jutil/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      752 2021-03-28 17:47:31.000000 django-jutil-3.9.9/jutil/management/commands/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2144 2021-03-28 17:40:10.000000 django-jutil-3.9.9/jutil/management/commands/make_bank_const_dk.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5094 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/management/commands/make_bank_const_se.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      430 2021-03-28 17:47:31.000000 django-jutil-3.9.9/jutil/management/commands/geo_ip.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3099 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/management/commands/make_bank_const_fi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:46.000000 django-jutil-3.9.9/jutil/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2722 2021-03-28 17:47:31.000000 django-jutil-3.9.9/jutil/management/commands/send_email.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      831 2021-03-28 17:47:31.000000 django-jutil-3.9.9/jutil/management/commands/setpass.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1162 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/management/commands/list_files.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:46.000000 django-jutil-3.9.9/jutil/management/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      863 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/permissions.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8729 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/xml.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       85 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93215 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/bank_const_dk.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1668 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/testing.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3324 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/files.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2150 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/bank_const_se.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5611 2021-08-11 21:04:58.000000 django-jutil-3.9.9/jutil/command.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5913 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/middleware.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11897 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/dates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2632 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/responses.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3110 2021-08-04 21:36:41.000000 django-jutil-3.9.9/jutil/parse.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       46 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      905 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/urls.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4410 2021-08-25 20:56:49.000000 django-jutil-3.9.9/jutil/model.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3450 2021-07-15 23:57:21.000000 django-jutil-3.9.9/jutil/request.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1062 2021-07-24 18:43:47.000000 django-jutil-3.9.9/jutil/decorators.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1111 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/sms.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22897 2020-05-21 16:43:46.000000 django-jutil-3.9.9/jutil/bank_const_be.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-25 23:15:47.000000 django-jutil-3.9.9/jutil/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18589 2021-08-26 16:33:25.000000 django-jutil-3.9.9/jutil/format.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      348 2021-02-02 23:24:21.000000 django-jutil-3.9.9/jutil/dict.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1119 2020-11-06 20:07:34.000000 django-jutil-3.9.9/jutil/auth.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-27 20:28:20.000000 django-jutil-3.9.9/MANIFEST.in
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:46.000000 django-jutil-3.9.9/LICENSE.txt
```

### Comparing `django-jutil-3.9.8/PKG-INFO` & `django-jutil-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-jutil
-Version: 3.9.8
+Version: 3.9.9
 Summary: Collection of small utilities for Django and Django REST framework projects
 Home-page: https://github.com/kajala/django-jutil
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 Description: django-jutil
         ============
```

### Comparing `django-jutil-3.9.8/setup.py` & `django-jutil-3.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jutil",
-    version="3.9.8",
+    version="3.9.9",
     author=u"Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="https://github.com/kajala/django-jutil",
     license="MIT licence, see LICENCE.txt",
     description="Collection of small utilities for Django and Django REST framework projects",
```

### Comparing `django-jutil-3.9.8/django_jutil.egg-info/SOURCES.txt` & `django-jutil-3.9.9/django_jutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/django_jutil.egg-info/PKG-INFO` & `django-jutil-3.9.9/django_jutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-jutil
-Version: 3.9.8
+Version: 3.9.9
 Summary: Collection of small utilities for Django and Django REST framework projects
 Home-page: https://github.com/kajala/django-jutil
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 Description: django-jutil
         ============
```

### Comparing `django-jutil-3.9.8/README.md` & `django-jutil-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/bank_const_iban.py` & `django-jutil-3.9.9/jutil/bank_const_iban.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/admin.py` & `django-jutil-3.9.9/jutil/admin.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/bank_const_fi.py` & `django-jutil-3.9.9/jutil/bank_const_fi.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/cache.py` & `django-jutil-3.9.9/jutil/cache.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/email.py` & `django-jutil-3.9.9/jutil/email.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/tests.py` & `django-jutil-3.9.9/jutil/tests.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/locale/fi/LC_MESSAGES/django.mo` & `django-jutil-3.9.9/jutil/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/locale/fi/LC_MESSAGES/django.po` & `django-jutil-3.9.9/jutil/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/locale/en/LC_MESSAGES/django.po` & `django-jutil-3.9.9/jutil/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/validators.py` & `django-jutil-3.9.9/jutil/validators.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/drf_exceptions.py` & `django-jutil-3.9.9/jutil/drf_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/modelfields.py` & `django-jutil-3.9.9/jutil/modelfields.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/apps.py` & `django-jutil-3.9.9/jutil/management/commands/apps.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/make_bank_const_dk.py` & `django-jutil-3.9.9/jutil/management/commands/make_bank_const_dk.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/make_bank_const_se.py` & `django-jutil-3.9.9/jutil/management/commands/make_bank_const_se.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/make_bank_const_fi.py` & `django-jutil-3.9.9/jutil/management/commands/make_bank_const_fi.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/send_email.py` & `django-jutil-3.9.9/jutil/management/commands/send_email.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/setpass.py` & `django-jutil-3.9.9/jutil/management/commands/setpass.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/management/commands/list_files.py` & `django-jutil-3.9.9/jutil/management/commands/list_files.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/permissions.py` & `django-jutil-3.9.9/jutil/permissions.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/xml.py` & `django-jutil-3.9.9/jutil/xml.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/bank_const_dk.py` & `django-jutil-3.9.9/jutil/bank_const_dk.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/testing.py` & `django-jutil-3.9.9/jutil/testing.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/files.py` & `django-jutil-3.9.9/jutil/files.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/bank_const_se.py` & `django-jutil-3.9.9/jutil/bank_const_se.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/command.py` & `django-jutil-3.9.9/jutil/command.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/middleware.py` & `django-jutil-3.9.9/jutil/middleware.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/dates.py` & `django-jutil-3.9.9/jutil/dates.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/responses.py` & `django-jutil-3.9.9/jutil/responses.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/parse.py` & `django-jutil-3.9.9/jutil/parse.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/urls.py` & `django-jutil-3.9.9/jutil/urls.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/model.py` & `django-jutil-3.9.9/jutil/model.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/request.py` & `django-jutil-3.9.9/jutil/request.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/decorators.py` & `django-jutil-3.9.9/jutil/decorators.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/sms.py` & `django-jutil-3.9.9/jutil/sms.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/bank_const_be.py` & `django-jutil-3.9.9/jutil/bank_const_be.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/jutil/format.py` & `django-jutil-3.9.9/jutil/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from collections import OrderedDict
 from datetime import timedelta
 from decimal import Decimal
 import subprocess
 from io import StringIO
 from typing import List, Any, Optional, Union, Dict, Sequence, Tuple, TypeVar
 from django.conf import settings
-from django.core.exceptions import ValidationError
+from django.core.exceptions import ValidationError, ImproperlyConfigured
 from django.utils.functional import lazy
 import xml.dom.minidom  # type: ignore
 from django.utils.safestring import mark_safe
 from django.utils.text import capfirst
 
 logger = logging.getLogger(__name__)
 
@@ -433,15 +433,15 @@
 
 
 def is_media_full_path(file_path: str) -> bool:
     """
     Checks if file path is under (settings) MEDIA_ROOT.
     """
     if not hasattr(settings, "MEDIA_ROOT") or not settings.MEDIA_ROOT:
-        raise ValueError("MEDIA_ROOT not defined")
+        raise ImproperlyConfigured("MEDIA_ROOT not defined")
     full_path = os.path.abspath(file_path)
     return full_path.startswith(str(settings.MEDIA_ROOT))
 
 
 def strip_media_root(file_path: str) -> str:
     """
     If file path starts with (settings) MEDIA_ROOT,
@@ -449,34 +449,38 @@
     Otherwise file path is returned as is. This enabled stored file names in more
     portable format for different environment / storage.
     If MEDIA_ROOT is missing or empty, the filename is returned as is.
     Reverse operation of this is get_media_full_path().
     :param file_path: str
     :return: str
     """
+    if not hasattr(settings, "MEDIA_ROOT") or not settings.MEDIA_ROOT:
+        raise ImproperlyConfigured("MEDIA_ROOT not defined")
     full_path = os.path.abspath(file_path)
-    if not is_media_full_path(full_path):
+    if not full_path.startswith(str(settings.MEDIA_ROOT)):
         raise ValueError("Path {} not under MEDIA_ROOT".format(file_path))
-    file_path = full_path[len(settings.MEDIA_ROOT) :]
+    file_path = full_path[len(str(settings.MEDIA_ROOT)) :]
     if file_path.startswith("/"):
         return file_path[1:]
     return file_path
 
 
 def get_media_full_path(file_path: str) -> str:
     """
     Returns the absolute path from a (relative) path to (settings) MEDIA_ROOT.
     This enabled stored file names in more portable format for different environment / storage.
     If MEDIA_ROOT is missing or non-media path is passed to function, exception is raised.
     Reverse operation of this is strip_media_root().
     :param file_path: str
     :return: str
     """
+    if not hasattr(settings, "MEDIA_ROOT") or not settings.MEDIA_ROOT:
+        raise ImproperlyConfigured("MEDIA_ROOT not defined")
     full_path = os.path.abspath(file_path) if os.path.isabs(file_path) else os.path.join(settings.MEDIA_ROOT, file_path)
-    if not is_media_full_path(full_path):
+    if not full_path.startswith(str(settings.MEDIA_ROOT)):
         raise ValueError("Path {} not under MEDIA_ROOT".format(file_path))
     return full_path
 
 
 def camel_case_to_underscore(s: str) -> str:
     """
     Converts camelCaseWord to camel_case_word.
```

### Comparing `django-jutil-3.9.8/jutil/auth.py` & `django-jutil-3.9.9/jutil/auth.py`

 * *Files identical despite different names*

### Comparing `django-jutil-3.9.8/LICENSE.txt` & `django-jutil-3.9.9/LICENSE.txt`

 * *Files identical despite different names*

