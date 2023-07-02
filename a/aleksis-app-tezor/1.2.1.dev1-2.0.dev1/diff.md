# Comparing `tmp/aleksis_app_tezor-1.2.1.dev1.tar.gz` & `tmp/aleksis_app_tezor-2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_tezor-1.2.1.dev1.tar", max compression
+gzip compressed data, was "aleksis_app_tezor-2.0.dev1.tar", max compression
```

## Comparing `aleksis_app_tezor-1.2.1.dev1.tar` & `aleksis_app_tezor-2.0.dev1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1684 2022-03-30 14:55:27.450220 aleksis_app_tezor-1.2.1.dev1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/LICENCE.rst
--rw-r--r--   0        0        0     1156 2022-03-13 13:11:02.079552 aleksis_app_tezor-1.2.1.dev1/README.rst
--rw-r--r--   0        0        0      151 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/__init__.py
--rw-r--r--   0        0        0      558 2022-03-30 18:35:28.416997 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/apps.py
--rw-r--r--   0        0        0      523 2022-03-30 14:55:27.450220 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/filters.py
--rw-r--r--   0        0        0     2358 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/forms.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-01-07 21:03:05.838930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9499 2022-05-02 11:42:45.361278 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6023 2023-01-07 21:03:05.838930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11071 2022-08-13 09:47:33.221896 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-01-07 21:03:05.834930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9412 2022-05-02 11:42:45.361278 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9367 2022-05-02 11:42:45.361278 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.834930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9367 2022-05-02 11:42:45.361278 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8109 2023-01-07 21:03:05.834930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13338 2022-08-13 09:47:33.221896 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9367 2022-05-02 11:42:45.365278 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8107 2023-01-07 21:03:05.838930 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13336 2022-08-13 09:47:33.221896 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1270 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/menus.py
--rw-r--r--   0        0        0     5839 2022-03-13 13:11:02.079552 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0001_initial.py
--rw-r--r--   0        0        0      404 2022-03-13 13:11:02.079552 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0002_invoice_due_date.py
--rw-r--r--   0        0        0     2367 2022-03-17 19:34:02.661335 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py
--rw-r--r--   0        0        0      622 2022-03-14 14:15:22.826360 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0004_client_email.py
--rw-r--r--   0        0        0      748 2022-03-14 14:15:22.826360 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py
--rw-r--r--   0        0        0      769 2022-03-14 14:15:22.826360 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py
--rw-r--r--   0        0        0     6003 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py
--rw-r--r--   0        0        0      698 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py
--rw-r--r--   0        0        0      475 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0009_invoice_billing_phone.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/__init__.py
--rw-r--r--   0        0        0      239 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/model_extensions.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/models/__init__.py
--rw-r--r--   0        0        0     3981 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/models/base.py
--rw-r--r--   0        0        0     7088 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/models/invoice.py
--rw-r--r--   0        0        0      967 2022-03-17 19:34:02.661335 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/predicates.py
--rw-r--r--   0        0        0     1860 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/preferences.py
--rw-r--r--   0        0        0     5234 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/rules.py
--rw-r--r--   0        0        0      210 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/settings.py
--rw-r--r--   0        0        0      810 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/signals.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/static/.keepdir
--rw-r--r--   0        0        0     2942 2022-03-19 19:54:19.308794 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/tables.py
--rw-r--r--   0        0        0      972 2022-03-19 19:54:19.308794 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/tasks.py
--rw-r--r--   0        0        0     1187 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email
--rw-r--r--   0        0        0      501 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/client/create.html
--rw-r--r--   0        0        0      496 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/client/edit.html
--rw-r--r--   0        0        0      519 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/client/full.html
--rw-r--r--   0        0        0      459 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/client/list.html
--rw-r--r--   0        0        0     4850 2023-01-07 20:32:19.359984 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html
--rw-r--r--   0        0        0      343 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice/list.html
--rw-r--r--   0        0        0      606 2022-03-13 13:11:02.079552 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html
--rw-r--r--   0        0        0      515 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html
--rw-r--r--   0        0        0      510 2022-03-10 21:44:17.388321 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/edit.html
--rw-r--r--   0        0        0     1755 2022-03-19 19:54:19.308794 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html
--rw-r--r--   0        0        0     1875 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/urls.py
--rw-r--r--   0        0        0        0 2022-03-30 14:55:27.454221 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/util/__init__.py
--rw-r--r--   0        0        0     1873 2022-04-14 20:29:59.017733 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/util/invoice.py
--rw-r--r--   0        0        0     9291 2022-12-12 16:23:12.094467 aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/views.py
--rw-r--r--   0        0        0     1644 2023-01-07 20:32:37.768024 aleksis_app_tezor-1.2.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     2352 2022-05-02 11:42:45.365278 aleksis_app_tezor-1.2.1.dev1/tox.ini
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 aleksis_app_tezor-1.2.1.dev1/setup.py
--rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 aleksis_app_tezor-1.2.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1997 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1156 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/README.rst
+-rw-r--r--   0        0        0      151 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/__init__.py
+-rw-r--r--   0        0        0      558 2022-03-30 18:35:28.416997 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/apps.py
+-rw-r--r--   0        0        0      523 2023-03-27 19:32:05.885076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/filters.py
+-rw-r--r--   0        0        0     2358 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/forms.py
+-rw-r--r--   0        0        0     4525 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/frontend/index.js
+-rw-r--r--   0        0        0      189 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9740 2023-07-02 13:14:36.075605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6023 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12477 2023-07-02 13:14:36.071606 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9656 2023-07-02 13:14:36.083605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.091606 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.099605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8109 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13340 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.087605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8107 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13321 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5839 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0001_initial.py
+-rw-r--r--   0        0        0      404 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0002_invoice_due_date.py
+-rw-r--r--   0        0        0     2367 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py
+-rw-r--r--   0        0        0      622 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0004_client_email.py
+-rw-r--r--   0        0        0      748 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py
+-rw-r--r--   0        0        0      769 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py
+-rw-r--r--   0        0        0     6003 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py
+-rw-r--r--   0        0        0      698 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py
+-rw-r--r--   0        0        0      475 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0009_invoice_billing_phone.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/__init__.py
+-rw-r--r--   0        0        0      239 2023-03-27 19:32:10.025086 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/model_extensions.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/__init__.py
+-rw-r--r--   0        0        0     3981 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/base.py
+-rw-r--r--   0        0        0     7088 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/invoice.py
+-rw-r--r--   0        0        0      967 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/predicates.py
+-rw-r--r--   0        0        0     1860 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/preferences.py
+-rw-r--r--   0        0        0     5234 2023-03-27 19:32:05.885076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/rules.py
+-rw-r--r--   0        0        0      210 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/settings.py
+-rw-r--r--   0        0        0      810 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/signals.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/static/.keepdir
+-rw-r--r--   0        0        0     2942 2023-03-27 19:32:05.889076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tables.py
+-rw-r--r--   0        0        0      972 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tasks.py
+-rw-r--r--   0        0        0     1187 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email
+-rw-r--r--   0        0        0      501 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/create.html
+-rw-r--r--   0        0        0      496 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/edit.html
+-rw-r--r--   0        0        0      519 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/full.html
+-rw-r--r--   0        0        0      459 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/list.html
+-rw-r--r--   0        0        0     5249 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html
+-rw-r--r--   0        0        0      343 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/list.html
+-rw-r--r--   0        0        0      606 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html
+-rw-r--r--   0        0        0      515 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html
+-rw-r--r--   0        0        0      510 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/edit.html
+-rw-r--r--   0        0        0     1755 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html
+-rw-r--r--   0        0        0     2018 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/urls.py
+-rw-r--r--   0        0        0        0 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/__init__.py
+-rw-r--r--   0        0        0     1873 2022-04-14 20:29:59.017733 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/invoice.py
+-rw-r--r--   0        0        0     9777 2023-07-02 13:07:40.095212 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/views.py
+-rw-r--r--   0        0        0     1640 2023-07-02 13:15:24.631656 aleksis_app_tezor-2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/tox.ini
+-rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev1/setup.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/CHANGELOG.rst` & `aleksis_app_tezor-2.0.dev1/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,36 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+Unreleased
+----------
+
+This version requires AlekSIS-Core 3.0. It is incompatible with any previous
+version.
+
+Removed
+~~~~~~~
+
+* Legacy menu integration for AlekSIS-Core pre-3.0
+
+
+Added
+~~~~~
+
+* Support for SPA in AlekSIS-Core 3.0
+
+Fixed
+-----
+
+* Replace usage of deprecated `ugettext_lazy` with `gettext_lazy`.
+
 `1.2`_ - 2022-03-20
 -------------------
 
 Added
 -----
 
 * Update django-payments to 1.0
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/LICENCE.rst` & `aleksis_app_tezor-2.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/README.rst` & `aleksis_app_tezor-2.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/apps.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/filters.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/forms.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,56 +4,50 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-23 12:54+0000\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
-#: aleksis/apps/tezor/forms.py:18
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr ""
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:15
@@ -160,39 +154,39 @@
 msgid "Invoice items"
 msgstr ""
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr ""
 
@@ -208,14 +202,22 @@
 msgid "Enable pledged payments"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr ""
 
+#: aleksis/apps/tezor/preferences.py:54
+msgid "SEPA Direct Debit - IBAN"
+msgstr ""
+
+#: aleksis/apps/tezor/preferences.py:65
+msgid "SEPA Direct Debit - BIC"
+msgstr ""
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr ""
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
 msgstr ""
@@ -330,14 +332,23 @@
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr ""
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr ""
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -369,30 +380,30 @@
 msgid "Selected invoices"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:187
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:212
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:222
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr ""
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -3,59 +3,52 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-03-22 21:24+0000\n"
-"PO-Revision-Date: 2022-08-03 16:34+0000\n"
-"Last-Translator: Jonathan Weth <teckids@jonathanweth.de>\n"
-"Language-Team: German <https://translate.edugit.org/projects/aleksis/"
-"aleksis-app-tezor/de/>\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
+"PO-Revision-Date: 2023-01-10 19:53+0000\n"
+"Last-Translator: Robert Seimetz <robert.seimetz@teckids.org>\n"
+"Language-Team: German <https://translate.edugit.org/projects/aleksis/aleksis-app-tezor/de/>\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.12.1\n"
 
-#: aleksis/apps/tezor/forms.py:18
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr "E-Mails senden"
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr "Zahlungsversprechen"
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr "Sofort / Klarna"
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr "PayPal"
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr "Lastschrift"
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr "Zahlungen und Geld"
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr "Klienten verwalten"
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
-msgstr "Meine Rechnungen"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
+msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr "Klarna / Sofort"
 
 #: aleksis/apps/tezor/models/base.py:15
 msgid "Payment pledge / manual payment"
@@ -161,39 +154,39 @@
 msgid "Invoice items"
 msgstr "Rechnungspositionen"
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr "Kann Rechnung als E-Mail versenden"
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr "MWSt. {} %"
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr "Bruttosumme"
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr "Artikel Nr."
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr "Gekaufter Artikel"
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr "Artikel-Nettopreis"
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr "Währung"
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr "Steuersatz"
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr "Zahlungen"
 
@@ -209,21 +202,33 @@
 msgid "Enable pledged payments"
 msgstr "Manuelle Zahlungen aktivieren"
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr "Rechnungen aktualisieren, wenn Personendaten sich ändern"
 
+#: aleksis/apps/tezor/preferences.py:54
+#, fuzzy
+#| msgid "SEPA Direct Debit"
+msgid "SEPA Direct Debit - IBAN"
+msgstr "SEPA-Lastschrift"
+
+#: aleksis/apps/tezor/preferences.py:65
+#, fuzzy
+#| msgid "SEPA Direct Debit"
+msgid "SEPA Direct Debit - BIC"
+msgstr "SEPA-Lastschrift"
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr "Art. Nr."
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
-msgstr "Artikel"
+msgstr "Objekt"
 
 #: aleksis/apps/tezor/tables.py:13
 msgid "Tax Rate"
 msgstr "Steuersatz"
 
 #: aleksis/apps/tezor/tables.py:17
 msgid "Qty."
@@ -278,14 +283,45 @@
 "    Please visit the following link to view and make the payment:\n"
 "    "
 msgstr ""
 "\n"
 "    Bitte rufen Sie den folgenden Link auf, um die Zahlung zu veranlassen:\n"
 "    "
 
+#: aleksis/apps/tezor/templates/templated_email/invoice.email:24
+#, fuzzy, python-format
+#| msgid ""
+#| "\n"
+#| "    Please find attached invoice number %(number)s for %(description)s.\n"
+#| "    Please carefully read the PDF file concerning all payment details.\n"
+#| "    "
+msgid ""
+"\n"
+"Please find attached invoice number %(number)s for %(description)s.\n"
+"Please carefully read the PDF file concerning all payment details.\n"
+msgstr ""
+"\n"
+"    Im Anhang finden Sie die Rechnung Nr. %(number)s für %(description)s.\n"
+"    Bitte lesen Sie das PDF mit allen Zahlungsdetails sorgfältig durch.\n"
+"    "
+
+#: aleksis/apps/tezor/templates/templated_email/invoice.email:30
+#, fuzzy
+#| msgid ""
+#| "\n"
+#| "    Please visit the following link to view and make the payment:\n"
+#| "    "
+msgid ""
+"\n"
+"Please visit the following link to view and make the payment:\n"
+msgstr ""
+"\n"
+"    Bitte rufen Sie den folgenden Link auf, um die Zahlung zu veranlassen:\n"
+"    "
+
 #: aleksis/apps/tezor/templates/tezor/client/create.html:4
 #: aleksis/apps/tezor/templates/tezor/client/create.html:5
 #: aleksis/apps/tezor/templates/tezor/client/list.html:11
 msgid "Create client"
 msgstr "Klient erstellen"
 
 #: aleksis/apps/tezor/templates/tezor/client/edit.html:4
@@ -324,14 +360,23 @@
 msgid "Payment"
 msgstr "Zahlung"
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr "Jetzt zahlen"
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr "Meine Rechnungen"
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr "Bezahlung durchführen für"
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -363,33 +408,39 @@
 msgid "Selected invoices"
 msgstr "Ausgewählte Rechnungen"
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr "Ausführen"
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr "Der Klient wurde erstellt."
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr "Der Klient wurde gespeichert."
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr "Der Klient wurde gelöscht."
 
-#: aleksis/apps/tezor/views.py:189
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr "Die Rechnungsgruppe wurde erstellt."
 
-#: aleksis/apps/tezor/views.py:214
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr "Die Rechnungsgruppe wurde gespeichert."
 
-#: aleksis/apps/tezor/views.py:224
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr "Die Rechnungsgruppe wurde gelöscht."
 
+#~ msgid "Payments and Money"
+#~ msgstr "Zahlungen und Geld"
+
+#~ msgid "Manage clients"
+#~ msgstr "Klienten verwalten"
+
 #~ msgid "Gross"
 #~ msgstr "Brutto"
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,55 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-23 12:54+0000\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: aleksis/apps/tezor/forms.py:18
+
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr ""
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:15
@@ -159,39 +153,39 @@
 msgid "Invoice items"
 msgstr ""
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr ""
 
@@ -207,14 +201,22 @@
 msgid "Enable pledged payments"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr ""
 
+#: aleksis/apps/tezor/preferences.py:54
+msgid "SEPA Direct Debit - IBAN"
+msgstr ""
+
+#: aleksis/apps/tezor/preferences.py:65
+msgid "SEPA Direct Debit - BIC"
+msgstr ""
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr ""
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
 msgstr ""
@@ -329,14 +331,23 @@
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr ""
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr ""
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -368,30 +379,30 @@
 msgid "Selected invoices"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:187
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:212
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:222
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr ""
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,55 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-23 12:54+0000\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aleksis/apps/tezor/forms.py:18
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr ""
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:15
@@ -159,39 +153,39 @@
 msgid "Invoice items"
 msgstr ""
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr ""
 
@@ -207,14 +201,22 @@
 msgid "Enable pledged payments"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr ""
 
+#: aleksis/apps/tezor/preferences.py:54
+msgid "SEPA Direct Debit - IBAN"
+msgstr ""
+
+#: aleksis/apps/tezor/preferences.py:65
+msgid "SEPA Direct Debit - BIC"
+msgstr ""
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr ""
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
 msgstr ""
@@ -329,14 +331,23 @@
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr ""
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr ""
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -368,30 +379,30 @@
 msgid "Selected invoices"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:187
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:212
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:222
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr ""
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,55 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-23 12:54+0000\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aleksis/apps/tezor/forms.py:18
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr ""
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:15
@@ -159,39 +153,39 @@
 msgid "Invoice items"
 msgstr ""
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr ""
 
@@ -207,14 +201,22 @@
 msgid "Enable pledged payments"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr ""
 
+#: aleksis/apps/tezor/preferences.py:54
+msgid "SEPA Direct Debit - IBAN"
+msgstr ""
+
+#: aleksis/apps/tezor/preferences.py:65
+msgid "SEPA Direct Debit - BIC"
+msgstr ""
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr ""
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
 msgstr ""
@@ -329,14 +331,23 @@
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr ""
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr ""
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -368,30 +379,30 @@
 msgid "Selected invoices"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:187
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:212
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:222
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr ""
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-04-23 12:54+0000\n"
-"PO-Revision-Date: 2022-06-12 05:32+0000\n"
+"PO-Revision-Date: 2023-05-26 04:39+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
-"aleksis-app-tezor/ru/>\n"
+"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/aleksis-app-tezor/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/tezor/forms.py:18
 msgid "Send e-mails"
 msgstr "Отправить эл.почту"
 
 #: aleksis/apps/tezor/forms.py:33
@@ -65,15 +62,15 @@
 
 #: aleksis/apps/tezor/models/base.py:16
 msgid "SEPA Direct Debit"
 msgstr "Прямой дебет SEPA"
 
 #: aleksis/apps/tezor/models/base.py:18
 msgid "Name"
-msgstr "Имя"
+msgstr "Полное имя"
 
 #: aleksis/apps/tezor/models/base.py:19
 msgid "Email"
 msgstr "Эл.почта"
 
 #: aleksis/apps/tezor/models/base.py:21
 msgid "Sofort / Klarna enabled"
@@ -219,15 +216,15 @@
 
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr "Арт.№"
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
-msgstr "Артикул"
+msgstr "Объект"
 
 #: aleksis/apps/tezor/tables.py:13
 msgid "Tax Rate"
 msgstr "Налоговая ставка"
 
 #: aleksis/apps/tezor/tables.py:17
 msgid "Qty."
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -4,55 +4,50 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-23 12:54+0000\n"
+"POT-Creation-Date: 2023-07-02 13:14+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: aleksis/apps/tezor/forms.py:18
+#: aleksis/apps/tezor/forms.py:21
 msgid "Send e-mails"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:33
+#: aleksis/apps/tezor/forms.py:39
+msgid "Get SEPA XML"
+msgstr ""
+
+#: aleksis/apps/tezor/forms.py:54
 msgid "Payment pledge"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:37
+#: aleksis/apps/tezor/forms.py:58
 msgid "Sofort / Klarna"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:42 aleksis/apps/tezor/models/base.py:13
+#: aleksis/apps/tezor/forms.py:63 aleksis/apps/tezor/models/base.py:13
 msgid "PayPal"
 msgstr ""
 
-#: aleksis/apps/tezor/forms.py:47
+#: aleksis/apps/tezor/forms.py:68
 msgid "Debit"
 msgstr ""
 
-#: aleksis/apps/tezor/menus.py:6
-msgid "Payments and Money"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:16
-msgid "Manage clients"
-msgstr ""
-
-#: aleksis/apps/tezor/menus.py:27
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
-#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
-msgid "My invoices"
+#: aleksis/apps/tezor/model_extensions.py:8
+msgid "External accounting number"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:14
 msgid "Klarna / Sofort"
 msgstr ""
 
 #: aleksis/apps/tezor/models/base.py:15
@@ -159,39 +154,39 @@
 msgid "Invoice items"
 msgstr ""
 
 #: aleksis/apps/tezor/models/invoice.py:144
 msgid "Can send invoice by email"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:168
+#: aleksis/apps/tezor/models/invoice.py:169
 msgid "VAT {} %"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:176
+#: aleksis/apps/tezor/models/invoice.py:177
 msgid "Gross total"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:195
+#: aleksis/apps/tezor/models/invoice.py:196
 msgid "Article no."
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:196
+#: aleksis/apps/tezor/models/invoice.py:197
 msgid "Purchased item"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:198
+#: aleksis/apps/tezor/models/invoice.py:199
 msgid "Item net price"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:200
+#: aleksis/apps/tezor/models/invoice.py:201
 msgid "Currency"
 msgstr ""
 
-#: aleksis/apps/tezor/models/invoice.py:202
+#: aleksis/apps/tezor/models/invoice.py:203
 msgid "Tax rate"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:8
 msgid "Payments"
 msgstr ""
 
@@ -207,14 +202,22 @@
 msgid "Enable pledged payments"
 msgstr ""
 
 #: aleksis/apps/tezor/preferences.py:43
 msgid "Update Invoices if person data changes"
 msgstr ""
 
+#: aleksis/apps/tezor/preferences.py:54
+msgid "SEPA Direct Debit - IBAN"
+msgstr ""
+
+#: aleksis/apps/tezor/preferences.py:65
+msgid "SEPA Direct Debit - BIC"
+msgstr ""
+
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr ""
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
 msgstr ""
@@ -329,14 +332,23 @@
 msgid "Payment"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/full.html:105
 msgid "Pay now"
 msgstr ""
 
+#: aleksis/apps/tezor/templates/tezor/invoice/full.html:113
+msgid "Mark as payed"
+msgstr ""
+
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:6
+#: aleksis/apps/tezor/templates/tezor/invoice/list.html:7
+msgid "My invoices"
+msgstr ""
+
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:6
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:7
 msgid "Make payment for"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice/payment.html:13
 msgid "Confirm payment"
@@ -368,30 +380,30 @@
 msgid "Selected invoices"
 msgstr ""
 
 #: aleksis/apps/tezor/templates/tezor/invoice_group/full.html:42
 msgid "Execute"
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:103
+#: aleksis/apps/tezor/views.py:105
 msgid "The client has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:115
+#: aleksis/apps/tezor/views.py:117
 msgid "The client has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:125
+#: aleksis/apps/tezor/views.py:127
 msgid "The client has been deleted."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:187
+#: aleksis/apps/tezor/views.py:190
 msgid "The invoice group has been created."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:212
+#: aleksis/apps/tezor/views.py:213
 msgid "The invoice group has been saved."
 msgstr ""
 
-#: aleksis/apps/tezor/views.py:222
+#: aleksis/apps/tezor/views.py:223
 msgid "The invoice group has been deleted."
 msgstr ""
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-04-23 12:54+0000\n"
-"PO-Revision-Date: 2022-07-01 11:55+0000\n"
+"PO-Revision-Date: 2023-01-25 05:58+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/"
-"aleksis-app-tezor/uk/>\n"
+"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/aleksis-app-tezor/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 "
-"? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > "
-"14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % "
-"100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/tezor/forms.py:18
 msgid "Send e-mails"
 msgstr "Відправити ел.листи"
 
 #: aleksis/apps/tezor/forms.py:33
@@ -220,15 +216,15 @@
 
 #: aleksis/apps/tezor/tables.py:10
 msgid "Art. No."
 msgstr "Арт.№"
 
 #: aleksis/apps/tezor/tables.py:11
 msgid "Item"
-msgstr "Артикул"
+msgstr "Об'єкт"
 
 #: aleksis/apps/tezor/tables.py:13
 msgid "Tax Rate"
 msgstr "Розмір Податку"
 
 #: aleksis/apps/tezor/tables.py:17
 msgid "Qty."
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0001_initial.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0004_client_email.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0004_client_email.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/models/base.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/models/invoice.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/predicates.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/preferences.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/rules.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/signals.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/signals.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/tables.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/tasks.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/client/full.html` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,22 @@
             <div class="card-action">
               <button class="btn waves-effect waves-light green" type="submit">
                 <i class="material-icons left iconify" data-icon="mdi:cash-fast"></i>
                 {% trans "Pay now" %}
               </button>
             </div>
             {% endif %}
+            {% if object.status == "preauth" %}
+            <div class="card-action">
+              <a class="btn waves-effect waves-light green" href="{% url 'mark_invoice_payed_by_token' object.token %}">
+                <i class="material-icons left iconify" data-icon="mdi:check-all"></i>
+                {% trans "Mark as payed" %}
+              </a>
+            </div>
+            {% endif %}
           </div>
         </div>
       </form>
     </div>
 
     {% render_table object.purchased_items_table %}
     {% render_table object.totals_table %}
```

#### html2text {}

```diff
@@ -27,10 +27,12 @@
  % if object.variant == choice.0 %}selected{% endif %}>{{ choice.1 }}
  {% endfor %}
  {{ object.get_status_display }}
  {{ object.due_date }}
 {% if object.status == "waiting" or object.status == "rejected" or
 object.status == "input" and can_do_payment %}
   {% trans "Pay now" %}
+{% endif %} {% if object.status == "preauth" %}
+ {%_trans_"Mark_as_payed"_%}
 {% endif %}
 {% render_table object.purchased_items_table %} {% render_table
 object.totals_table %} {% endblock %}
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/urls.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,8 +59,13 @@
         name="invoice_by_token",
     ),
     path(
         "invoice/<str:token>/send/",
         views.SendInvoiceEmail.as_view(),
         name="send_invoice_by_token",
     ),
+    path(
+        "invoice/<str:token>/mark_payed/",
+        views.MarkPayedView.as_view(),
+        name="mark_invoice_payed_by_token",
+    ),
 ]
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/util/invoice.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-1.2.1.dev1/aleksis/apps/tezor/views.py` & `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.core.exceptions import PermissionDenied, SuspiciousOperation
 from django.http import HttpResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse, reverse_lazy
 from django.utils.decorators import method_decorator
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.decorators.cache import never_cache
 from django.views.generic import View
 from django.views.generic.detail import DetailView
 
 from django_tables2.views import RequestConfig, SingleTableView
 from djp_sepa.models import SEPAMandate
 from payments import PaymentStatus, RedirectNeeded
@@ -187,19 +187,17 @@
     form_class = EditInvoiceGroupForm
     permission_required = "tezor.create_invoice_groups_rule"
     template_name = "tezor/invoice_group/create.html"
     success_message = _("The invoice group has been created.")
 
     def form_valid(self, form):
         client = Client.objects.get(id=self.kwargs["pk"])
-        InvoiceGroup.objects.create(
-            client=client,
-            name=form.cleaned_data["name"],
-            template_name=form.cleaned_data["template_name"],
-        )
+        self.object = form.save()
+        self.object.client = client
+        self.object.save()
 
         return super().form_valid(form)
 
     def get_success_url(self):
         return reverse("client_by_pk", args=[self.object.client.pk])
 
 
@@ -275,7 +273,25 @@
     permission_required = "tezor.view_own_invoices_list_rule"
     template_name = "tezor/invoice/list.html"
 
     def get_queryset(self, *args, **kwargs):
         invoices = self.model.objects.filter(person=self.request.user.person)
 
         return invoices
+
+
+class MarkPayedView(PermissionRequiredMixin, View):
+
+    model = Invoice
+    permission_required = "tezor.mark_payed_rule"
+    template_name = "tezor/invoice/full.html"
+
+
+    def dispatch(self, request, token):
+        self.object = get_object_or_404(self.model, token=token)
+
+        if self.object.status != PaymentStatus.PREAUTH:
+            return reverse("invoice_by_token", args=[self.object.token])
+        else:
+            self.object.status = "confirmed"
+            self.object.save()
+            return reverse("invoce_by_token", args=[self.object.token])
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/pyproject.toml` & `aleksis_app_tezor-2.0.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Tezor"
-version = "1.2.1.dev1"
+version = "2.0dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -26,16 +26,16 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^2.10"
 django-payments-sepa = { version = "^1.2.dev0", allow-prereleases = true, extras = ["fints"] }
+aleksis-core = "^3.0"
 django-payments = { version = "^1.0.0", extras = ["sofort"] }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 tezor = "aleksis.apps.tezor.apps:DefaultConfig"
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/setup.py` & `aleksis_app_tezor-2.0.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,17 @@
  'aleksis.apps.tezor',
  'aleksis.apps.tezor.migrations',
  'aleksis.apps.tezor.models',
  'aleksis.apps.tezor.util']
 
 package_data = \
 {'': ['*'],
- 'aleksis.apps.tezor': ['locale/*',
+ 'aleksis.apps.tezor': ['frontend/*',
+                        'frontend/messages/*',
+                        'locale/*',
                         'locale/ar/LC_MESSAGES/*',
                         'locale/de_DE/LC_MESSAGES/*',
                         'locale/fr/LC_MESSAGES/*',
                         'locale/la/LC_MESSAGES/*',
                         'locale/nb_NO/LC_MESSAGES/*',
                         'locale/ru/LC_MESSAGES/*',
                         'locale/tr_TR/LC_MESSAGES/*',
@@ -30,24 +32,24 @@
                         'templates/tezor/invoice/list.html',
                         'templates/tezor/invoice/payment.html',
                         'templates/tezor/invoice/payment.html',
                         'templates/tezor/invoice/payment.html',
                         'templates/tezor/invoice_group/*']}
 
 install_requires = \
-['aleksis-core>=2.10,<3.0',
+['aleksis-core>=3.0,<4.0',
  'django-payments-sepa[fints]>=1.2.dev0,<2.0',
  'django-payments[sofort]>=1.0.0,<2.0.0']
 
 entry_points = \
 {'aleksis.app': ['tezor = aleksis.apps.tezor.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-tezor',
-    'version': '1.2.1.dev1',
+    'version': '2.0.dev1',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Tezor (account and payment system)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Tezor (account and payment system)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_tezor-1.2.1.dev1/PKG-INFO` & `aleksis_app_tezor-2.0.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aleksis-app-tezor
-Version: 1.2.1.dev1
+Version: 2.0.dev1
 Summary: AlekSIS (School Information System) — App Tezor (account and payment system)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=2.10,<3.0)
+Requires-Dist: aleksis-core (>=3.0,<4.0)
 Requires-Dist: django-payments-sepa[fints] (>=1.2.dev0,<2.0)
 Requires-Dist: django-payments[sofort] (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Tezor
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Tezor (account and payment system)
```

