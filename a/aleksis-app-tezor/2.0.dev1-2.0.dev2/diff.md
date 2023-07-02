# Comparing `tmp/aleksis_app_tezor-2.0.dev1.tar.gz` & `tmp/aleksis_app_tezor-2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_tezor-2.0.dev1.tar", max compression
+gzip compressed data, was "aleksis_app_tezor-2.0.dev2.tar", max compression
```

## Comparing `aleksis_app_tezor-2.0.dev1.tar` & `aleksis_app_tezor-2.0.dev2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1997 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/LICENCE.rst
--rw-r--r--   0        0        0     1156 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/README.rst
--rw-r--r--   0        0        0      151 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/__init__.py
--rw-r--r--   0        0        0      558 2022-03-30 18:35:28.416997 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/apps.py
--rw-r--r--   0        0        0      523 2023-03-27 19:32:05.885076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/filters.py
--rw-r--r--   0        0        0     2358 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/forms.py
--rw-r--r--   0        0        0     4525 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/frontend/index.js
--rw-r--r--   0        0        0      189 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9740 2023-07-02 13:14:36.075605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6023 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12477 2023-07-02 13:14:36.071606 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9656 2023-07-02 13:14:36.083605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.091606 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.099605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8109 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13340 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.087605 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8107 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13321 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5839 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0001_initial.py
--rw-r--r--   0        0        0      404 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0002_invoice_due_date.py
--rw-r--r--   0        0        0     2367 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py
--rw-r--r--   0        0        0      622 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0004_client_email.py
--rw-r--r--   0        0        0      748 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py
--rw-r--r--   0        0        0      769 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py
--rw-r--r--   0        0        0     6003 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py
--rw-r--r--   0        0        0      698 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py
--rw-r--r--   0        0        0      475 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0009_invoice_billing_phone.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/__init__.py
--rw-r--r--   0        0        0      239 2023-03-27 19:32:10.025086 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/model_extensions.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/__init__.py
--rw-r--r--   0        0        0     3981 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/base.py
--rw-r--r--   0        0        0     7088 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/invoice.py
--rw-r--r--   0        0        0      967 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/predicates.py
--rw-r--r--   0        0        0     1860 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/preferences.py
--rw-r--r--   0        0        0     5234 2023-03-27 19:32:05.885076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/rules.py
--rw-r--r--   0        0        0      210 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/settings.py
--rw-r--r--   0        0        0      810 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/signals.py
--rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/static/.keepdir
--rw-r--r--   0        0        0     2942 2023-03-27 19:32:05.889076 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tables.py
--rw-r--r--   0        0        0      972 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tasks.py
--rw-r--r--   0        0        0     1187 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email
--rw-r--r--   0        0        0      501 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/create.html
--rw-r--r--   0        0        0      496 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/edit.html
--rw-r--r--   0        0        0      519 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/full.html
--rw-r--r--   0        0        0      459 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/list.html
--rw-r--r--   0        0        0     5249 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html
--rw-r--r--   0        0        0      343 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/list.html
--rw-r--r--   0        0        0      606 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html
--rw-r--r--   0        0        0      515 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html
--rw-r--r--   0        0        0      510 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/edit.html
--rw-r--r--   0        0        0     1755 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html
--rw-r--r--   0        0        0     2018 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/urls.py
--rw-r--r--   0        0        0        0 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/__init__.py
--rw-r--r--   0        0        0     1873 2022-04-14 20:29:59.017733 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/invoice.py
--rw-r--r--   0        0        0     9777 2023-07-02 13:07:40.095212 aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/views.py
--rw-r--r--   0        0        0     1640 2023-07-02 13:15:24.631656 aleksis_app_tezor-2.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev1/tox.ini
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev1/setup.py
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1997 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev2/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/LICENCE.rst
+-rw-r--r--   0        0        0     1156 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev2/README.rst
+-rw-r--r--   0        0        0      151 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/__init__.py
+-rw-r--r--   0        0        0      558 2022-03-30 18:35:28.416997 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/apps.py
+-rw-r--r--   0        0        0      523 2023-03-27 19:32:05.885076 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/filters.py
+-rw-r--r--   0        0        0     2358 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/forms.py
+-rw-r--r--   0        0        0     4538 2023-07-02 19:48:56.379004 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/frontend/index.js
+-rw-r--r--   0        0        0      189 2023-07-02 13:07:06.371180 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9740 2023-07-02 13:14:36.075605 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6023 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12477 2023-07-02 13:14:36.071606 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9656 2023-07-02 13:14:36.083605 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.091606 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.099605 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8109 2023-01-07 21:03:05.834930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13340 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9610 2023-07-02 13:14:36.087605 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8107 2023-01-07 21:03:05.838930 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13321 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5839 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0001_initial.py
+-rw-r--r--   0        0        0      404 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0002_invoice_due_date.py
+-rw-r--r--   0        0        0     2367 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0003_manual_invoicing.py
+-rw-r--r--   0        0        0      622 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0004_client_email.py
+-rw-r--r--   0        0        0      748 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py
+-rw-r--r--   0        0        0      769 2022-03-14 14:15:22.826360 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0006_invoice_constraints.py
+-rw-r--r--   0        0        0     6003 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0007_client_payment_variants.py
+-rw-r--r--   0        0        0      698 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0008_always_set_person.py
+-rw-r--r--   0        0        0      475 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0009_invoice_billing_phone.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/__init__.py
+-rw-r--r--   0        0        0      239 2023-03-27 19:32:10.025086 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/model_extensions.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/models/__init__.py
+-rw-r--r--   0        0        0     3981 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/models/base.py
+-rw-r--r--   0        0        0     7088 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/models/invoice.py
+-rw-r--r--   0        0        0      967 2022-03-17 19:34:02.661335 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/predicates.py
+-rw-r--r--   0        0        0     1860 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/preferences.py
+-rw-r--r--   0        0        0     5402 2023-07-02 19:48:56.379004 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/rules.py
+-rw-r--r--   0        0        0      210 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/settings.py
+-rw-r--r--   0        0        0      810 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/signals.py
+-rw-r--r--   0        0        0        0 2022-03-06 17:34:30.628198 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/static/.keepdir
+-rw-r--r--   0        0        0     2942 2023-03-27 19:32:05.889076 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/tables.py
+-rw-r--r--   0        0        0      972 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/tasks.py
+-rw-r--r--   0        0        0     1187 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/templated_email/invoice.email
+-rw-r--r--   0        0        0      501 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/client/create.html
+-rw-r--r--   0        0        0      496 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/client/edit.html
+-rw-r--r--   0        0        0      519 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/client/full.html
+-rw-r--r--   0        0        0      459 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/client/list.html
+-rw-r--r--   0        0        0     5249 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice/full.html
+-rw-r--r--   0        0        0      343 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice/list.html
+-rw-r--r--   0        0        0      606 2022-03-13 13:11:02.079552 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice/payment.html
+-rw-r--r--   0        0        0      515 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice_group/create.html
+-rw-r--r--   0        0        0      510 2022-03-10 21:44:17.388321 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice_group/edit.html
+-rw-r--r--   0        0        0     1755 2022-03-19 19:54:19.308794 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice_group/full.html
+-rw-r--r--   0        0        0     2018 2023-07-02 13:07:02.563177 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/urls.py
+-rw-r--r--   0        0        0        0 2022-03-30 14:55:27.454221 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/util/__init__.py
+-rw-r--r--   0        0        0     1873 2022-04-14 20:29:59.017733 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/util/invoice.py
+-rw-r--r--   0        0        0     9777 2023-07-02 13:07:40.095212 aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/views.py
+-rw-r--r--   0        0        0     1640 2023-07-02 19:49:15.723095 aleksis_app_tezor-2.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-07-02 13:07:06.375181 aleksis_app_tezor-2.0.dev2/tox.ini
+-rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev2/setup.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 aleksis_app_tezor-2.0.dev2/PKG-INFO
```

### Comparing `aleksis_app_tezor-2.0.dev1/CHANGELOG.rst` & `aleksis_app_tezor-2.0.dev2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/LICENCE.rst` & `aleksis_app_tezor-2.0.dev2/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/README.rst` & `aleksis_app_tezor-2.0.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/apps.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/filters.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/forms.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/frontend/index.js` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/frontend/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 import {
-    notLoggedInValidator,
-    hasPersonValidator,
+    hasPersonValidator
 } from "aleksis.core/routeValidators";
 
 export default {
     meta: {
         inMenu: true,
         titleKey: "tezor.menu_title",
         icon: "mdi-piggy-bank-outline",
+        permission: "tezor.view_menu_rule",
     },
     children: [{
         path: "invoice/:token/print/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
```

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0001_initial.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0003_manual_invoicing.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0003_manual_invoicing.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0004_client_email.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0004_client_email.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0005_alter_fields_invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0006_invoice_constraints.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0006_invoice_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0007_client_payment_variants.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0007_client_payment_variants.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/migrations/0008_always_set_person.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/migrations/0008_always_set_person.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/base.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/models/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/models/invoice.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/predicates.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/preferences.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/rules.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,7 +149,10 @@
     | has_global_perm("tezor.send_invoice_email")
     | has_object_perm("tezor.send_invoice_email")
 )
 rules.add_perm("tezor.send_invoice_email_rule", send_invoice_email_predicate)
 
 view_own_invoices_predicate = has_person
 rules.add_perm("tezor.view_own_invoices_list_rule", view_own_invoices_predicate)
+
+view_menu_predicate = view_own_invoices_predicate | view_clients_predicate | view_invoice_groups_predicate
+rules.add_perm("tezor.view_menu_rule", view_menu_predicate)
```

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/signals.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/signals.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tables.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/tasks.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/templated_email/invoice.email` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/templated_email/invoice.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/client/full.html` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/client/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/full.html` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice/payment.html` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice/payment.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/create.html` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice_group/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/templates/tezor/invoice_group/full.html` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/templates/tezor/invoice_group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/urls.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/util/invoice.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/util/invoice.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/aleksis/apps/tezor/views.py` & `aleksis_app_tezor-2.0.dev2/aleksis/apps/tezor/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/pyproject.toml` & `aleksis_app_tezor-2.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Tezor"
-version = "2.0dev1"
+version = "2.0dev2"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_app_tezor-2.0.dev1/tox.ini` & `aleksis_app_tezor-2.0.dev2/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_tezor-2.0.dev1/setup.py` & `aleksis_app_tezor-2.0.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
  'django-payments[sofort]>=1.0.0,<2.0.0']
 
 entry_points = \
 {'aleksis.app': ['tezor = aleksis.apps.tezor.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-tezor',
-    'version': '2.0.dev1',
+    'version': '2.0.dev2',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Tezor (account and payment system)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Tezor (account and payment system)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_tezor-2.0.dev1/PKG-INFO` & `aleksis_app_tezor-2.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-tezor
-Version: 2.0.dev1
+Version: 2.0.dev2
 Summary: AlekSIS (School Information System) — App Tezor (account and payment system)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

