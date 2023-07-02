# Comparing `tmp/django-request-1.6.2.tar.gz` & `tmp/django-request-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-request-1.6.2.tar", last modified: Tue Jan 10 16:13:49 2023, max compression
+gzip compressed data, was "django-request-1.6.3.tar", last modified: Sun Jul  2 13:52:28 2023, max compression
```

## Comparing `django-request-1.6.2.tar` & `django-request-1.6.3.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1732 2023-01-10 16:08:13.000000 django-request-1.6.2/CHANGELOG.md
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1288 2023-01-10 16:06:03.000000 django-request-1.6.2/LICENSE
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      190 2020-12-10 21:11:32.000000 django-request-1.6.2/MANIFEST.in
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4311 2023-01-10 16:13:49.480350 django-request-1.6.2/PKG-INFO
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     2929 2023-01-10 16:05:43.000000 django-request-1.6.2/README.rst
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/django_request.egg-info/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4311 2023-01-10 16:13:49.000000 django-request-1.6.2/django_request.egg-info/PKG-INFO
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     2196 2023-01-10 16:13:49.000000 django-request-1.6.2/django_request.egg-info/SOURCES.txt
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        1 2023-01-10 16:13:49.000000 django-request-1.6.2/django_request.egg-info/dependency_links.txt
--rw-rw-r--   0 felixx    (1000) felixx    (1000)       28 2023-01-10 16:13:49.000000 django-request-1.6.2/django_request.egg-info/requires.txt
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        8 2023-01-10 16:13:49.000000 django-request-1.6.2/django_request.egg-info/top_level.txt
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/docs/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      162 2020-12-10 21:11:33.000000 django-request-1.6.2/docs/description.txt
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      414 2022-01-09 14:53:10.000000 django-request-1.6.2/docs/long_description.txt
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      266 2023-01-10 16:06:18.000000 django-request-1.6.2/request/__init__.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     3043 2021-12-12 18:13:49.000000 django-request-1.6.2/request/admin.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      148 2021-12-12 18:13:49.000000 django-request-1.6.2/request/apps.py
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/locale/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/locale/de/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/locale/de/LC_MESSAGES/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     2977 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    10182 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/locale/en/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/locale/en/LC_MESSAGES/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     9175 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/locale/es/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/locale/es/LC_MESSAGES/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     6158 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    11309 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/locale/fr/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     6419 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    11070 2023-01-10 16:05:43.000000 django-request-1.6.2/request/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/management/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.2/request/management/__init__.py
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/management/commands/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.2/request/management/commands/__init__.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     2321 2021-12-12 18:13:49.000000 django-request-1.6.2/request/management/commands/purgerequests.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4223 2021-12-12 18:13:49.000000 django-request-1.6.2/request/managers.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1630 2022-01-09 12:52:07.000000 django-request-1.6.2/request/middleware.py
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/migrations/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     3293 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0001_initial.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      347 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0002_alter_request_ip.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      378 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0003_auto_20160331_1430.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      425 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0004_alter_time_timezone_default.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      464 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0005_alter_request_user.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      375 2021-12-12 18:13:49.000000 django-request-1.6.2/request/migrations/0006_alter_request_method_default.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      498 2022-01-08 12:32:18.000000 django-request-1.6.2/request/migrations/0007_alter_request_is_ajax.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.2/request/migrations/__init__.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4048 2021-12-12 18:13:49.000000 django-request-1.6.2/request/models.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4358 2021-12-12 18:13:49.000000 django-request-1.6.2/request/plugins.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      787 2021-12-12 18:13:49.000000 django-request-1.6.2/request/router.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1608 2020-12-10 21:11:33.000000 django-request-1.6.2/request/settings.py
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/static/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/static/request/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/static/request/js/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    19415 2020-12-10 21:11:33.000000 django-request-1.6.2/request/static/request/js/excanvas.min.js
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    72173 2020-12-10 21:11:33.000000 django-request-1.6.2/request/static/request/js/jquery-1.4.2.min.js
--rw-rw-r--   0 felixx    (1000) felixx    (1000)    89666 2020-12-10 21:11:33.000000 django-request-1.6.2/request/static/request/js/jquery.flot.js
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     7363 2020-12-10 21:11:33.000000 django-request-1.6.2/request/static/request/js/jquery.timeago.js
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1349 2020-12-10 21:11:33.000000 django-request-1.6.2/request/static/request/js/request.js
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/templates/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/templates/admin/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/templates/admin/request/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1677 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/admin/request/app_index.html
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/templates/admin/request/request/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      515 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/admin/request/request/change_list.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     2451 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/admin/request/request/overview.html
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.476350 django-request-1.6.2/request/templates/request/
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/templates/request/plugins/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      387 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/activeusers.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)       61 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/base.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      847 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/latestrequests.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      116 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/table.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      162 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/topbrowsers.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      459 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/toppaths.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      444 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/topreferrers.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      356 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/topsearchphrases.html
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      542 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templates/request/plugins/trafficinformation.html
-drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-01-10 16:13:49.480350 django-request-1.6.2/request/templatetags/
--rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.2/request/templatetags/__init__.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)      401 2021-12-12 18:13:49.000000 django-request-1.6.2/request/templatetags/request_admin.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1883 2021-12-12 18:13:49.000000 django-request-1.6.2/request/templatetags/request_tag.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     4886 2021-12-12 18:13:49.000000 django-request-1.6.2/request/traffic.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     6078 2023-01-10 16:05:43.000000 django-request-1.6.2/request/utils.py
--rw-rw-r--   0 felixx    (1000) felixx    (1000)     1757 2023-01-10 16:13:49.480350 django-request-1.6.2/setup.cfg
--rw-rw-r--   0 felixx    (1000) felixx    (1000)       60 2020-12-10 21:11:33.000000 django-request-1.6.2/setup.py
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.318569 django-request-1.6.3/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1863 2023-07-02 13:46:32.000000 django-request-1.6.3/CHANGELOG.md
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1288 2023-01-10 16:06:03.000000 django-request-1.6.3/LICENSE
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      190 2020-12-10 21:11:32.000000 django-request-1.6.3/MANIFEST.in
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4355 2023-07-02 13:52:28.318569 django-request-1.6.3/PKG-INFO
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2934 2023-07-02 13:46:32.000000 django-request-1.6.3/README.rst
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/django_request.egg-info/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4355 2023-07-02 13:52:28.000000 django-request-1.6.3/django_request.egg-info/PKG-INFO
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2254 2023-07-02 13:52:28.000000 django-request-1.6.3/django_request.egg-info/SOURCES.txt
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        1 2023-07-02 13:52:28.000000 django-request-1.6.3/django_request.egg-info/dependency_links.txt
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)       28 2023-07-02 13:52:28.000000 django-request-1.6.3/django_request.egg-info/requires.txt
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        8 2023-07-02 13:52:28.000000 django-request-1.6.3/django_request.egg-info/top_level.txt
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/docs/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      162 2020-12-10 21:11:33.000000 django-request-1.6.3/docs/description.txt
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      414 2022-01-09 14:53:10.000000 django-request-1.6.3/docs/long_description.txt
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      266 2023-07-02 13:48:17.000000 django-request-1.6.3/request/__init__.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     3043 2021-12-12 18:13:49.000000 django-request-1.6.3/request/admin.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      148 2021-12-12 18:13:49.000000 django-request-1.6.3/request/apps.py
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/locale/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/locale/de/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2977 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    10182 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/locale/en/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     9175 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/locale/es/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     6158 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    11309 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/locale/fr/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     6419 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    11070 2023-01-10 16:05:43.000000 django-request-1.6.3/request/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/management/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.3/request/management/__init__.py
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.226562 django-request-1.6.3/request/management/commands/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.3/request/management/commands/__init__.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2321 2021-12-12 18:13:49.000000 django-request-1.6.3/request/management/commands/purgerequests.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4223 2021-12-12 18:13:49.000000 django-request-1.6.3/request/managers.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1630 2022-01-09 12:52:07.000000 django-request-1.6.3/request/middleware.py
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.230562 django-request-1.6.3/request/migrations/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     3293 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0001_initial.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      347 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0002_alter_request_ip.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      378 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0003_auto_20160331_1430.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      425 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0004_alter_time_timezone_default.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      464 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0005_alter_request_user.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      375 2021-12-12 18:13:49.000000 django-request-1.6.3/request/migrations/0006_alter_request_method_default.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      498 2022-01-08 12:32:18.000000 django-request-1.6.3/request/migrations/0007_alter_request_is_ajax.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2155 2023-07-02 13:46:32.000000 django-request-1.6.3/request/migrations/0008_alter_request_response_choices.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.3/request/migrations/__init__.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4048 2021-12-12 18:13:49.000000 django-request-1.6.3/request/models.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4358 2021-12-12 18:13:49.000000 django-request-1.6.3/request/plugins.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      787 2021-12-12 18:13:49.000000 django-request-1.6.3/request/router.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1608 2020-12-10 21:11:33.000000 django-request-1.6.3/request/settings.py
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/static/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/static/request/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.310569 django-request-1.6.3/request/static/request/js/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    19415 2020-12-10 21:11:33.000000 django-request-1.6.3/request/static/request/js/excanvas.min.js
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    72173 2020-12-10 21:11:33.000000 django-request-1.6.3/request/static/request/js/jquery-1.4.2.min.js
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)    89666 2020-12-10 21:11:33.000000 django-request-1.6.3/request/static/request/js/jquery.flot.js
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     7363 2020-12-10 21:11:33.000000 django-request-1.6.3/request/static/request/js/jquery.timeago.js
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1349 2020-12-10 21:11:33.000000 django-request-1.6.3/request/static/request/js/request.js
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/templates/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/templates/admin/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.310569 django-request-1.6.3/request/templates/admin/request/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1677 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/admin/request/app_index.html
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.310569 django-request-1.6.3/request/templates/admin/request/request/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      515 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/admin/request/request/change_list.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     2451 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/admin/request/request/overview.html
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.222562 django-request-1.6.3/request/templates/request/
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.314569 django-request-1.6.3/request/templates/request/plugins/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      387 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/activeusers.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)       61 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/base.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      847 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/latestrequests.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      116 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/table.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      162 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/topbrowsers.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      459 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/toppaths.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      444 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/topreferrers.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      356 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/topsearchphrases.html
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      542 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templates/request/plugins/trafficinformation.html
+drwxrwxr-x   0 felixx    (1000) felixx    (1000)        0 2023-07-02 13:52:28.318569 django-request-1.6.3/request/templatetags/
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)        0 2020-12-10 21:11:33.000000 django-request-1.6.3/request/templatetags/__init__.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)      401 2021-12-12 18:13:49.000000 django-request-1.6.3/request/templatetags/request_admin.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1883 2021-12-12 18:13:49.000000 django-request-1.6.3/request/templatetags/request_tag.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     4886 2021-12-12 18:13:49.000000 django-request-1.6.3/request/traffic.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     6078 2023-01-10 16:05:43.000000 django-request-1.6.3/request/utils.py
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)     1785 2023-07-02 13:52:28.318569 django-request-1.6.3/setup.cfg
+-rw-rw-r--   0 felixx    (1000) felixx    (1000)       60 2020-12-10 21:11:33.000000 django-request-1.6.3/setup.py
```

### Comparing `django-request-1.6.2/CHANGELOG.md` & `django-request-1.6.3/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog for django-request
 
+## 1.6.3
+
+### Enhancements
+
+* Confirms support for Django 4.2.
+
+### Bug Fixes
+
+* Adds a missing migration with HTTP status codes.
+
 ## 1.6.2
 
 ### Enhancements
 
 * Adds support for missing HTTP status codes: 103, 208, 226, 308, 428, 429,
   431, 451, and 511.
```

### Comparing `django-request-1.6.2/LICENSE` & `django-request-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/PKG-INFO` & `django-request-1.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-request
-Version: 1.6.2
+Version: 1.6.3
 Summary: django-request is a statistics module for django. It stores requests in a database for admins to see, it can also be used to get statistics on who is online etc.
 Home-page: https://django-request.readthedocs.io/en/latest/
 Author: Kyle Fuller
 Author-email: kyle@fuller.li
 Maintainer: Mariusz Felisiak
 Maintainer-email: felisiak.mariusz@gmail.com
 License: BSD
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -62,15 +63,15 @@
 To find the request overview page, please click on Requests inside the admin,
 then “Overview” on the top right, next to “add request”.
 
 Requirements
 ------------
 
 * **Python**: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
-* **Django**: 2.2, 3.2, 4.0, 4.1
+* **Django**: 2.2, 3.2, 4.0, 4.1, 4.2
 * **python-dateutil**
 
 django-request 1.5.1_ is the last version that supports Django 1.4, 1.5, 1.6.
 
 django-request 1.5.4_ is the last version that supports Django 1.7, 1.8, 1.9.
 
 django-request 1.5.5_ is the last version that supports Django 1.10.
```

### Comparing `django-request-1.6.2/README.rst` & `django-request-1.6.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 To find the request overview page, please click on Requests inside the admin,
 then “Overview” on the top right, next to “add request”.
 
 Requirements
 ------------
 
 * **Python**: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
-* **Django**: 2.2, 3.2, 4.0, 4.1
+* **Django**: 2.2, 3.2, 4.0, 4.1, 4.2
 * **python-dateutil**
 
 django-request 1.5.1_ is the last version that supports Django 1.4, 1.5, 1.6.
 
 django-request 1.5.4_ is the last version that supports Django 1.7, 1.8, 1.9.
 
 django-request 1.5.5_ is the last version that supports Django 1.10.
```

### Comparing `django-request-1.6.2/django_request.egg-info/PKG-INFO` & `django-request-1.6.3/django_request.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-request
-Version: 1.6.2
+Version: 1.6.3
 Summary: django-request is a statistics module for django. It stores requests in a database for admins to see, it can also be used to get statistics on who is online etc.
 Home-page: https://django-request.readthedocs.io/en/latest/
 Author: Kyle Fuller
 Author-email: kyle@fuller.li
 Maintainer: Mariusz Felisiak
 Maintainer-email: felisiak.mariusz@gmail.com
 License: BSD
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -62,15 +63,15 @@
 To find the request overview page, please click on Requests inside the admin,
 then “Overview” on the top right, next to “add request”.
 
 Requirements
 ------------
 
 * **Python**: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
-* **Django**: 2.2, 3.2, 4.0, 4.1
+* **Django**: 2.2, 3.2, 4.0, 4.1, 4.2
 * **python-dateutil**
 
 django-request 1.5.1_ is the last version that supports Django 1.4, 1.5, 1.6.
 
 django-request 1.5.4_ is the last version that supports Django 1.7, 1.8, 1.9.
 
 django-request 1.5.5_ is the last version that supports Django 1.10.
```

### Comparing `django-request-1.6.2/django_request.egg-info/SOURCES.txt` & `django-request-1.6.3/django_request.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 request/migrations/0001_initial.py
 request/migrations/0002_alter_request_ip.py
 request/migrations/0003_auto_20160331_1430.py
 request/migrations/0004_alter_time_timezone_default.py
 request/migrations/0005_alter_request_user.py
 request/migrations/0006_alter_request_method_default.py
 request/migrations/0007_alter_request_is_ajax.py
+request/migrations/0008_alter_request_response_choices.py
 request/migrations/__init__.py
 request/static/request/js/excanvas.min.js
 request/static/request/js/jquery-1.4.2.min.js
 request/static/request/js/jquery.flot.js
 request/static/request/js/jquery.timeago.js
 request/static/request/js/request.js
 request/templates/admin/request/app_index.html
```

### Comparing `django-request-1.6.2/request/admin.py` & `django-request-1.6.3/request/admin.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/de/LC_MESSAGES/django.mo` & `django-request-1.6.3/request/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/de/LC_MESSAGES/django.po` & `django-request-1.6.3/request/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/en/LC_MESSAGES/django.po` & `django-request-1.6.3/request/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/es/LC_MESSAGES/django.mo` & `django-request-1.6.3/request/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/es/LC_MESSAGES/django.po` & `django-request-1.6.3/request/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/fr/LC_MESSAGES/django.mo` & `django-request-1.6.3/request/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/locale/fr/LC_MESSAGES/django.po` & `django-request-1.6.3/request/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/management/commands/purgerequests.py` & `django-request-1.6.3/request/management/commands/purgerequests.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/managers.py` & `django-request-1.6.3/request/managers.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/middleware.py` & `django-request-1.6.3/request/middleware.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/migrations/0001_initial.py` & `django-request-1.6.3/request/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/models.py` & `django-request-1.6.3/request/models.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/plugins.py` & `django-request-1.6.3/request/plugins.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/router.py` & `django-request-1.6.3/request/router.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/settings.py` & `django-request-1.6.3/request/settings.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/static/request/js/excanvas.min.js` & `django-request-1.6.3/request/static/request/js/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/static/request/js/jquery-1.4.2.min.js` & `django-request-1.6.3/request/static/request/js/jquery-1.4.2.min.js`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/static/request/js/jquery.flot.js` & `django-request-1.6.3/request/static/request/js/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/static/request/js/jquery.timeago.js` & `django-request-1.6.3/request/static/request/js/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/static/request/js/request.js` & `django-request-1.6.3/request/static/request/js/request.js`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templates/admin/request/app_index.html` & `django-request-1.6.3/request/templates/admin/request/app_index.html`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templates/admin/request/request/change_list.html` & `django-request-1.6.3/request/templates/admin/request/request/change_list.html`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templates/admin/request/request/overview.html` & `django-request-1.6.3/request/templates/admin/request/request/overview.html`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templates/request/plugins/latestrequests.html` & `django-request-1.6.3/request/templates/request/plugins/latestrequests.html`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templates/request/plugins/trafficinformation.html` & `django-request-1.6.3/request/templates/request/plugins/trafficinformation.html`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/templatetags/request_tag.py` & `django-request-1.6.3/request/templatetags/request_tag.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/traffic.py` & `django-request-1.6.3/request/traffic.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/request/utils.py` & `django-request-1.6.3/request/utils.py`

 * *Files identical despite different names*

### Comparing `django-request-1.6.2/setup.cfg` & `django-request-1.6.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-request
-version = 1.6.2
+version = 1.6.3
 url = https://django-request.readthedocs.io/en/latest/
 download_url = https://pypi.org/project/django-request/
 author = Kyle Fuller
 author_email = kyle@fuller.li
 maintainer = Mariusz Felisiak
 maintainer_email = felisiak.mariusz@gmail.com
 description = django-request is a statistics module for django. It stores requests in a database for admins to see, it can also be used to get statistics on who is online etc.
@@ -16,14 +16,15 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
```

