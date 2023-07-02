# Comparing `tmp/AlekSIS-App-Buelleten-1.0.7.dev0.tar.gz` & `tmp/aleksis_app_buelleten-2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlekSIS-App-Buelleten-1.0.7.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_buelleten-2.0.dev0.tar", max compression
```

## Comparing `AlekSIS-App-Buelleten-1.0.7.dev0.tar` & `aleksis_app_buelleten-2.0.dev0.tar`

### file list

```diff
@@ -1,43 +1,38 @@
--rw-r--r--   0        0        0      453 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1205 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/README.rst
--rw-r--r--   0        0        0      155 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/__init__.py
--rw-r--r--   0        0        0     1458 2022-08-08 18:24:53.798020 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/apps.py
--rw-r--r--   0        0        0      176 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/filters.py
--rw-r--r--   0        0        0      651 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/forms.py
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/.keepdir
--rw-r--r--   0        0        0      463 2022-08-08 18:25:35.149942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5077 2022-08-08 17:33:32.095796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-08 18:25:35.149942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4945 2022-08-08 17:33:32.095796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2022-08-08 18:25:35.145942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4990 2022-08-08 17:33:32.099796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-08 18:25:35.149942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4945 2022-08-08 17:33:32.099796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-08 18:25:35.149942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4945 2022-08-08 17:33:32.095796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-08 18:25:35.149942 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4945 2022-08-08 17:33:32.095796 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      805 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/menus.py
--rw-r--r--   0        0        0     4866 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/migrations/0001_initial.py
--rw-r--r--   0        0        0     1491 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/migrations/__init__.py
--rw-r--r--   0        0        0     1991 2022-08-08 18:24:51.742024 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/models/base.py
--rw-r--r--   0        0        0     1184 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/models/slides.py
--rw-r--r--   0        0        0     2776 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/rules.py
--rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/static/.keepdir
--rw-r--r--   0        0        0     1444 2022-06-27 20:34:36.006318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/tables.py
--rw-r--r--   0        0        0      477 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display/create.html
--rw-r--r--   0        0        0      473 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display/edit.html
--rw-r--r--   0        0        0      489 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/create.html
--rw-r--r--   0        0        0      485 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/edit.html
--rw-r--r--   0        0        0     1810 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html
--rw-r--r--   0        0        0      725 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html
--rw-r--r--   0        0        0      734 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html
--rw-r--r--   0        0        0      648 2022-06-27 20:34:36.010318 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html
--rw-r--r--   0        0        0     1317 2022-08-08 18:24:51.726024 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/urls.py
--rw-r--r--   0        0        0     8975 2022-08-08 18:24:51.930023 AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/views.py
--rw-r--r--   0        0        0     1504 2022-08-09 10:20:05.078367 AlekSIS-App-Buelleten-1.0.7.dev0/pyproject.toml
--rw-r--r--   0        0        0     2354 2022-08-08 18:24:42.890040 AlekSIS-App-Buelleten-1.0.7.dev0/tox.ini
--rw-r--r--   0        0        0     2788 2022-08-09 10:20:13.893308 AlekSIS-App-Buelleten-1.0.7.dev0/setup.py
--rw-r--r--   0        0        0     2074 2022-08-09 10:20:13.893552 AlekSIS-App-Buelleten-1.0.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0      685 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/LICENCE.rst
+-rw-r--r--   0        0        0     1205 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/README.rst
+-rw-r--r--   0        0        0      155 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/__init__.py
+-rw-r--r--   0        0        0     1459 2022-08-10 18:11:25.887031 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/apps.py
+-rw-r--r--   0        0        0      176 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/filters.py
+-rw-r--r--   0        0        0      651 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/forms.py
+-rw-r--r--   0        0        0     3675 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/frontend/index.js
+-rw-r--r--   0        0        0      129 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/.keepdir
+-rw-r--r--   0        0        0     4965 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4881 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4835 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4866 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1491 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/__init__.py
+-rw-r--r--   0        0        0     1991 2022-08-08 18:24:51.742024 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/base.py
+-rw-r--r--   0        0        0     1184 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/slides.py
+-rw-r--r--   0        0        0     2776 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/rules.py
+-rw-r--r--   0        0        0        0 2022-06-25 20:36:08.802607 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/static/.keepdir
+-rw-r--r--   0        0        0     1444 2022-06-27 20:34:36.006318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/tables.py
+-rw-r--r--   0        0        0      477 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display/create.html
+-rw-r--r--   0        0        0      473 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display/edit.html
+-rw-r--r--   0        0        0      489 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/create.html
+-rw-r--r--   0        0        0      485 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/edit.html
+-rw-r--r--   0        0        0     1810 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html
+-rw-r--r--   0        0        0      725 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html
+-rw-r--r--   0        0        0      734 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html
+-rw-r--r--   0        0        0      648 2022-06-27 20:34:36.010318 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html
+-rw-r--r--   0        0        0     1340 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/urls.py
+-rw-r--r--   0        0        0     8975 2022-08-08 18:24:51.930023 aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/views.py
+-rw-r--r--   0        0        0     1549 2023-07-02 13:47:51.825331 aleksis_app_buelleten-2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-07-02 13:42:42.749085 aleksis_app_buelleten-2.0.dev0/tox.ini
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev0/setup.py
+-rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 aleksis_app_buelleten-2.0.dev0/PKG-INFO
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/LICENCE.rst` & `aleksis_app_buelleten-2.0.dev0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/README.rst` & `aleksis_app_buelleten-2.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/apps.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     dist_name = "AlekSIS-App-Buelleten"
 
     urls = {
         "Repository": "https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Buelleten",
     }
     licence = "EUPL-1.2+"
     copyright_info = (
-        ([2021], "Tom Teichler", "dev@jonathanweth.de"),
+        ([2021], "Tom Teichler", "tom.teichler@teckids.org"),
         ([2022], "Dominik George", "dominik.george@teckids.org"),
-        ([2022], "Tom Teichler", "tom.teichler@teckids.org"),
+        ([2022], "Jonathan Weth", "dev@jonathanweth.de"),
     )
 
     @classmethod
     def get_all_scopes(cls) -> dict[str, str]:
         """Return all OAuth scopes and their descriptions for this app."""
         DisplayGroup = apps.get_model("buelleten", "DisplayGroup")
         label_prefix = _("Access content for display group")
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/forms.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/forms.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
-#: aleksis/apps/buelleten/apps.py:29
-msgid "Access content for display group"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
+#: aleksis/apps/buelleten/apps.py:28
+msgid "Access content for display group"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
@@ -44,34 +34,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -135,14 +125,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -175,14 +170,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: aleksis/apps/buelleten/apps.py:29
+#: aleksis/apps/buelleten/apps.py:28
 msgid "Access content for display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
-msgstr ""
-
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
 msgid "Slug"
 msgstr ""
@@ -43,34 +34,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -134,14 +125,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -174,14 +170,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: aleksis/apps/buelleten/apps.py:29
-msgid "Access content for display group"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
 
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
+#: aleksis/apps/buelleten/apps.py:28
+msgid "Access content for display group"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
@@ -43,34 +33,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -134,14 +124,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -174,14 +169,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/la/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aleksis/apps/buelleten/apps.py:29
+#: aleksis/apps/buelleten/apps.py:28
 msgid "Access content for display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
-msgstr ""
-
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
 msgid "Slug"
 msgstr ""
@@ -43,34 +33,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -134,14 +124,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -174,14 +169,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aleksis/apps/buelleten/apps.py:29
+#: aleksis/apps/buelleten/apps.py:28
 msgid "Access content for display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
-msgstr ""
-
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
 msgid "Slug"
 msgstr ""
@@ -43,34 +33,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -134,14 +124,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -174,14 +169,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-08 17:33+0000\n"
+"POT-Creation-Date: 2023-07-02 13:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aleksis/apps/buelleten/apps.py:29
+#: aleksis/apps/buelleten/apps.py:28
 msgid "Access content for display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/menus.py:6
-msgid "Digital signage"
-msgstr ""
-
-#: aleksis/apps/buelleten/menus.py:15
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
-#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
-msgid "Display groups"
-msgstr ""
-
 #: aleksis/apps/buelleten/models/base.py:13
 msgid "Name"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:14
 msgid "Slug"
 msgstr ""
@@ -43,34 +33,34 @@
 msgid "Impressive based PDF/image/video display"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/base.py:29
 msgid "Website display based on surf browser"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:33
-#: aleksis/apps/buelleten/models/base.py:50
+#: aleksis/apps/buelleten/models/base.py:34
+#: aleksis/apps/buelleten/models/base.py:56
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:8
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:9
 msgid "Display group"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:35
+#: aleksis/apps/buelleten/models/base.py:38
 msgid "Hostname"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:36
+#: aleksis/apps/buelleten/models/base.py:39
 msgid "Profile"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:37
+#: aleksis/apps/buelleten/models/base.py:41
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/buelleten/models/base.py:52
+#: aleksis/apps/buelleten/models/base.py:60
 msgid "Order"
 msgstr ""
 
 #: aleksis/apps/buelleten/models/slides.py:14
 msgid "URL"
 msgstr ""
 
@@ -134,14 +124,19 @@
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/display_group/full.html:44
 #, python-format
 msgid "Create %(name)s"
 msgstr ""
 
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:8
+#: aleksis/apps/buelleten/templates/buelleten/display_group/list.html:9
+msgid "Display groups"
+msgstr ""
+
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:8
 #: aleksis/apps/buelleten/templates/buelleten/slide/create.html:12
 #, python-format
 msgid "Create %(slide)s"
 msgstr ""
 
 #: aleksis/apps/buelleten/templates/buelleten/slide/edit.html:8
@@ -174,14 +169,14 @@
 msgid "The display group has been deleted."
 msgstr ""
 
 #: aleksis/apps/buelleten/views.py:159
 msgid "The slide has been saved."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:190
+#: aleksis/apps/buelleten/views.py:191
 msgid "The slide has been created."
 msgstr ""
 
-#: aleksis/apps/buelleten/views.py:201
+#: aleksis/apps/buelleten/views.py:203
 msgid "The slide has been deleted."
 msgstr ""
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/migrations/0001_initial.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/migrations/0002_display_variants.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/models/base.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/base.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/models/slides.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/models/slides.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/rules.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/rules.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/tables.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/tables.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/full.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/display_group/list.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/templates/buelleten/slide/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/urls.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,21 @@
     path("display_groups/", views.DisplayGroupListView.as_view(), name="display_groups"),
     path(
         "display_groups/create/",
         views.DisplayGroupCreateView.as_view(),
         name="create_display_group",
     ),
     path(
-        "display_groups/<int:pk>/edit",
+        "display_groups/<int:pk>/edit/",
         views.DisplayGroupEditView.as_view(),
         name="edit_display_group",
     ),
     path(
         "display_groups/<int:pk>/", views.DisplayGroupFullView.as_view(), name="display_group_by_id"
     ),
-    path(
-        "api/impressive/<slug:slug>.txt",
-        views.ImpressiveDisplayURLList.as_view(),
-        name="impressive_display_list",
-    ),
     path("displays/", views.DisplayListView.as_view(), name="displays"),
     path("displays/create/", views.DisplayCreateView.as_view(), name="create_display"),
     path("displays/<int:pk>/", views.DisplayEditView.as_view(), name="edit_display"),
     path(
         "slides/<int:pk>/edit/",
         views.SlideEditView.as_view(),
         name="edit_slide",
@@ -37,7 +32,15 @@
     ),
     path(
         "slides/<str:app>/<str:model>/new/",
         views.SlideCreateView.as_view(),
         name="create_slide",
     ),
 ]
+
+api_urlpatterns= [
+    path(
+        "api/impressive/<slug:slug>.txt",
+        views.ImpressiveDisplayURLList.as_view(),
+        name="impressive_display_list",
+    ),
+]
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/aleksis/apps/buelleten/views.py` & `aleksis_app_buelleten-2.0.dev0/aleksis/apps/buelleten/views.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/pyproject.toml` & `aleksis_app_buelleten-2.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Buelleten"
-version = "1.0.7dev0"
+version = "2.0.dev0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -26,18 +26,18 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = {version = ">=2.7, <3.1", allow-prereleases = true }
+aleksis-core = {version = ">=3.0, <3.1", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
-aleksis-builddeps = "*"
+aleksis-builddeps = {version=">=2023.1.dev0", allow-prereleases=true}
 
 [tool.poetry.plugins."aleksis.app"]
 buelleten = "aleksis.apps.buelleten.apps:DefaultConfig"
 
 [tool.black]
 line-length = 100
 exclude = "/migrations/"
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/tox.ini` & `aleksis_app_buelleten-2.0.dev0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tox]
 skipsdist = True
 skip_missing_interpreters = true
-envlist = py37,py38,py39
+envlist = py39,py310,py311
 
 [testenv]
 whitelist_externals = poetry
-		      sudo
 skip_install = true
 envdir = {toxworkdir}/globalenv
 commands_pre =
      poetry install
-     poetry run aleksis-admin webpack_bundle
+     poetry run aleksis-admin vite build
      poetry run aleksis-admin collectstatic --no-input
 commands =
     poetry run pytest --cov=. {posargs} aleksis/
 
 [testenv:selenium]
 setenv =
     TEST_SCREENSHOT_PATH = {env:TEST_SCREENSHOT_PATH:.tox/screenshots}
@@ -23,14 +22,16 @@
     TEST_HOST = {env:TEST_HOST:172.17.0.1}
 
 [testenv:lint]
 commands =
     poetry run black --check --diff aleksis/
     poetry run isort -c --diff --stdout aleksis/
     poetry run flake8 {posargs} aleksis/
+    poetry run sh -c "aleksis-admin yarn run prettier --check --ignore-path={toxinidir}/.prettierignore {toxinidir}"
+    poetry run sh -c "aleksis-admin yarn run eslint {toxinidir}/aleksis/**/*/frontend/**/*.{js,vue} --config={toxinidir}/.eslintrc.js --resolve-plugins-relative-to=."
 
 [testenv:security]
 commands =
     poetry show --no-dev
     poetry run safety check --full-report
 
 [testenv:build]
@@ -42,24 +43,25 @@
 [testenv:docs]
 commands = poetry run make -C docs/ html {posargs}
 
 [testenv:reformat]
 commands =
     poetry run isort aleksis/
     poetry run black aleksis/
+    poetry run sh -c "aleksis-admin yarn run prettier --write --ignore-path={toxinidir}/.prettierignore {toxinidir}"
 
 [testenv:makemessages]
 commands =
     poetry run aleksis-admin makemessages --no-wrap -e html,txt,py,email -i static -l ar -l de_DE -l fr -l nb_NO -l tr_TR -l la -l uk -l ru
     poetry run aleksis-admin makemessages --no-wrap -d djangojs -i **/node_modules -l ar -l de_DE -l fr -l nb_NO -l tr_TR -l la -l uk -l ru
 
 [flake8]
 max_line_length = 100
 exclude = migrations,tests
-ignore = A002,A003,BLK100,E203,E231,W503,D100,D101,D102,D103,D104,D105,D106,D107,RST215,RST214,F821,F841,S106,T100,T101,DJ05
+ignore = BLK100,E203,E231,W503,D100,D101,D102,D103,D104,D105,D106,D107,RST215,RST214,F821,F841,S106,T100,T101,DJ05
 
 [isort]
 profile = black
 line_length = 100
 default_section = THIRDPARTY
 known_first_party = aleksis
 known_django = django
```

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/setup.py` & `aleksis_app_buelleten-2.0.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 ['aleksis',
  'aleksis.apps.buelleten',
  'aleksis.apps.buelleten.migrations',
  'aleksis.apps.buelleten.models']
 
 package_data = \
 {'': ['*'],
- 'aleksis.apps.buelleten': ['locale/*',
+ 'aleksis.apps.buelleten': ['frontend/*',
+                            'frontend/messages/*',
+                            'locale/*',
                             'locale/ar/LC_MESSAGES/*',
                             'locale/de_DE/LC_MESSAGES/*',
                             'locale/fr/LC_MESSAGES/*',
                             'locale/la/LC_MESSAGES/*',
                             'locale/nb_NO/LC_MESSAGES/*',
                             'locale/tr_TR/LC_MESSAGES/*',
                             'static/*',
                             'templates/buelleten/display/*',
                             'templates/buelleten/display_group/*',
                             'templates/buelleten/slide/*']}
 
 install_requires = \
-['aleksis-core>=2.7,<3.1']
+['aleksis-core>=3.0,<3.1']
 
 entry_points = \
 {'aleksis.app': ['buelleten = aleksis.apps.buelleten.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-buelleten',
-    'version': '1.0.7.dev0',
+    'version': '2.0.dev0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Bülleten (Digital Signage)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Bülleten (Digital Signage)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2021 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
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

### Comparing `AlekSIS-App-Buelleten-1.0.7.dev0/PKG-INFO` & `aleksis_app_buelleten-2.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aleksis-app-buelleten
-Version: 1.0.7.dev0
+Version: 2.0.dev0
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
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=2.7,<3.1)
+Requires-Dist: aleksis-core (>=3.0,<3.1)
 Project-URL: Documentation, https://aleksis.edugit.io/official/AlekSIS-Core/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Buelleten
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Bülleten (Digital Signage)
 ==================================================================================================
```

