# Comparing `tmp/AlekSIS-App-Paweljong-1.9.tar.gz` & `tmp/aleksis_app_paweljong-2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlekSIS-App-Paweljong-1.9.tar", max compression
+gzip compressed data, was "aleksis_app_paweljong-2.0.dev0.tar", max compression
```

## Comparing `AlekSIS-App-Paweljong-1.9.tar` & `aleksis_app_paweljong-2.0.dev0.tar`

### file list

```diff
@@ -1,103 +1,108 @@
--rw-r--r--   0        0        0     3437 2022-05-04 17:07:49.804504 AlekSIS-App-Paweljong-1.9/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/LICENCE.rst
--rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.9/README.rst
--rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/__init__.py
--rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/apps.py
--rw-r--r--   0        0        0     1254 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/data_checks.py
--rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/filters.py
--rw-r--r--   0        0        0    16143 2022-06-27 11:04:58.585278 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/forms.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/.keepdir
--rw-r--r--   0        0        0      463 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44339 2022-06-28 15:44:36.897766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    28604 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    60401 2022-06-28 15:44:36.941766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44255 2022-06-28 15:44:36.909766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.921766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-28 15:45:03.630316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.965767 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-06-28 15:45:03.634316 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44209 2022-06-28 15:44:36.953766 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3256 2022-06-27 10:59:49.965700 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/menus.py
--rw-r--r--   0        0        0     8646 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0001_initial.py
--rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0002_event_website.py
--rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
--rw-r--r--   0        0        0      911 2022-02-21 09:18:10.132166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
--rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
--rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
--rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0007_terms.py
--rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
--rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
--rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
--rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
--rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0012_event_slug.py
--rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0013_info_mailings.py
--rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
--rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0015_registrationstate.py
--rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
--rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
--rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
--rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0019_retractions.py
--rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0020_check_in.py
--rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0021_checkpoint.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/__init__.py
--rw-r--r--   0        0        0    15306 2022-06-28 15:42:20.693243 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/models.py
--rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/predicates.py
--rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/preferences.py
--rw-r--r--   0        0        0     8923 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/rules.py
--rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/settings.py
--rw-r--r--   0        0        0      990 2022-06-19 19:58:48.687395 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/css/paweljong.css
--rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
--rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
--rw-r--r--   0        0        0     4446 2022-06-24 14:54:41.596452 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tables.py
--rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tasks.py
--rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
--rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
--rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/create.html
--rw-r--r--   0        0        0     3547 2022-06-28 15:43:45.196693 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/detail.html
--rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/edit.html
--rw-r--r--   0        0        0     2475 2022-02-21 22:05:46.538591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/full.html
--rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/list.html
--rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/manage.html
--rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
--rw-r--r--   0        0        0     4488 2022-02-21 20:54:12.455591 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
--rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
--rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
--rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/registered.html
--rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/terms.html
--rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
--rw-r--r--   0        0        0    12811 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
--rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
--rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
--rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
--rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
--rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
--rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/corona.html
--rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
--rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
--rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
--rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/manage.html
--rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
--rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register.html
--rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register_start.html
--rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
--rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
--rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
--rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
--rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/create.html
--rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/edit.html
--rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/term/list.html
--rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
--rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
--rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
--rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_created.email
--rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_notification.email
--rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_registered.email
--rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
--rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templatetags/coerce.py
--rw-r--r--   0        0        0     5382 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/urls.py
--rw-r--r--   0        0        0    38228 2022-06-28 08:40:58.099898 AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/views.py
--rw-r--r--   0        0        0     1452 2022-06-28 15:44:26.977692 AlekSIS-App-Paweljong-1.9/pyproject.toml
--rw-r--r--   0        0        0    17809 2022-06-28 15:45:06.274288 AlekSIS-App-Paweljong-1.9/setup.py
--rw-r--r--   0        0        0     2208 2022-06-28 15:45:06.274820 AlekSIS-App-Paweljong-1.9/PKG-INFO
+-rw-r--r--   0        0        0     3513 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/LICENCE.rst
+-rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev0/README.rst
+-rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/__init__.py
+-rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/apps.py
+-rw-r--r--   0        0        0     1253 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/data_checks.py
+-rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/filters.py
+-rw-r--r--   0        0        0    16277 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/forms.py
+-rw-r--r--   0        0        0    12846 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/index.js
+-rw-r--r--   0        0        0      563 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47795 2023-07-02 13:33:45.628654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31084 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    64927 2023-07-02 13:33:45.600654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47711 2023-07-02 13:33:45.608654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-06-07 21:25:48.599903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.584654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.572654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-06-07 21:25:48.599903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.616654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8646 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0001_initial.py
+-rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0002_event_website.py
+-rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
+-rw-r--r--   0        0        0      911 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
+-rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
+-rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
+-rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0007_terms.py
+-rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
+-rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
+-rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
+-rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
+-rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0012_event_slug.py
+-rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0013_info_mailings.py
+-rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
+-rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0015_registrationstate.py
+-rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
+-rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
+-rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
+-rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0019_retractions.py
+-rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0020_check_in.py
+-rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0021_checkpoint.py
+-rw-r--r--   0        0        0      681 2022-07-08 20:57:59.622407 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py
+-rw-r--r--   0        0        0      452 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0023_eventregistration_cost.py
+-rw-r--r--   0        0        0      430 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0024_add_cost_to_registration.py
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/__init__.py
+-rw-r--r--   0        0        0    16558 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/models.py
+-rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/predicates.py
+-rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/preferences.py
+-rw-r--r--   0        0        0     9079 2022-06-30 15:18:35.332204 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/rules.py
+-rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/settings.py
+-rw-r--r--   0        0        0     1076 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/css/paweljong.css
+-rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
+-rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
+-rw-r--r--   0        0        0     4445 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tables.py
+-rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tasks.py
+-rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
+-rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
+-rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/create.html
+-rw-r--r--   0        0        0     3557 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/detail.html
+-rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/edit.html
+-rw-r--r--   0        0        0     2480 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/full.html
+-rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/list.html
+-rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/manage.html
+-rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
+-rw-r--r--   0        0        0     5118 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
+-rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
+-rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
+-rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/registered.html
+-rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/terms.html
+-rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
+-rw-r--r--   0        0        0    13116 2022-06-28 20:06:29.947789 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
+-rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
+-rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
+-rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
+-rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
+-rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
+-rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/corona.html
+-rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
+-rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
+-rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
+-rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/manage.html
+-rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
+-rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register.html
+-rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register_start.html
+-rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
+-rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
+-rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
+-rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
+-rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/create.html
+-rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/edit.html
+-rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/list.html
+-rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
+-rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
+-rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
+-rw-r--r--   0        0        0     2272 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/account_registered.email
+-rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_created.email
+-rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_notification.email
+-rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_registered.email
+-rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
+-rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templatetags/coerce.py
+-rw-r--r--   0        0        0     5596 2023-07-02 13:18:57.471867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/urls.py
+-rw-r--r--   0        0        0    40215 2023-07-02 13:19:17.651886 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/views.py
+-rw-r--r--   0        0        0     1522 2023-07-02 13:39:36.044937 aleksis_app_paweljong-2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev0/setup.py
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev0/PKG-INFO
```

### Comparing `AlekSIS-App-Paweljong-1.9/CHANGELOG.rst` & `aleksis_app_paweljong-2.0.dev0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+Unreleased
+----------
+
+Added
+~~~~~
+
+* Add SPA support for AlekSIS-Core 3.0
+
 `1.5.1`_
 --------
 
 Fixed
 ~~~~~
 
 * Fix total amount calculation for event registrations with donations.
```

### Comparing `AlekSIS-App-Paweljong-1.9/LICENCE.rst` & `aleksis_app_paweljong-2.0.dev0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/README.rst` & `aleksis_app_paweljong-2.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/apps.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/apps.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/data_checks.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/data_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from aleksis.core.data_checks import DataCheck, IgnoreSolveOption, SolveOption
 
 
 class SyncEventMembers(SolveOption):
     name = "sync_event_members"
     verbose_name = _("Sync members")
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/filters.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/filters.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/forms.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django import forms
 from django.forms import fields
 from django.utils import dateformat, formats
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from allauth.account.views import SignupForm
 from django_select2.forms import ModelSelect2MultipleWidget, ModelSelect2Widget
 from material import Fieldset, Layout, Row
 from phonenumber_field.formfields import PhoneNumberField
 
 from aleksis.apps.tezor.models.invoice import InvoiceGroup
@@ -457,15 +457,15 @@
         )
 
 
 class EditInfoMailingForm(forms.ModelForm):
 
     layout = Layout(
         Row("sender", "reply_to", "active"),
-        Row("send_to_person", "send_to_guardians"),
+        Row("send_to_person", "send_to_guardians", "send_to_retracted", "send_to_not_checked_in"),
         Row("subject"),
         Row("text"),
     )
 
     class Meta:
         model = InfoMailing
         exclude = ["sent_to"]
@@ -503,31 +503,33 @@
         widget=forms.TextInput(attrs={"autofocus": "", "autocomplete": "off"}),
         help_text=_("Please enter a username."),
     )
 
 
 class EventCheckpointForm(forms.Form):
     class Media:
-        js = ("https://unpkg.com/html5-qrcode", "js/paweljong/qrscanner.js", "js/paweljong/checkpoint.js")
+        js = (
+            "https://unpkg.com/html5-qrcode",
+            "js/paweljong/qrscanner.js",
+            "js/paweljong/checkpoint.js",
+        )
 
-    layout = Layout(
-        "comment", "use_latlon",
-    )
+    layout = Layout("comment", "use_latlon", "username")
 
     comment = forms.CharField(
         required=True,
         label=_("Comment"),
         help_text=_("Please enter a comment describing the checkpoint (e.g. Dinner)."),
     )
 
     username = forms.CharField(
         required=True,
         label=_("Person"),
         help_text=_("Please enter a username."),
-        widget=forms.HiddenInput(),
+        widget=forms.TextInput(attrs={"autofocus": "", "autocomplete": "off"}),
     )
 
     use_latlon = forms.BooleanField(
         required=False,
         label=_("Submit geolocation"),
         initial=True,
     )
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -78,25 +78,23 @@
 msgid "Date data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -106,15 +104,15 @@
 msgid "Person the voucher is valid for"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -177,15 +175,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr ""
 
@@ -202,69 +200,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr ""
 
@@ -284,23 +300,23 @@
 msgid "School place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr ""
 
@@ -344,73 +360,45 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
 msgstr ""
 
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr ""
-
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr ""
 
@@ -454,175 +442,189 @@
 msgid "Send to registered person"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:412
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:413
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:414
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
@@ -647,15 +649,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr ""
 
@@ -670,29 +672,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr ""
 
@@ -785,26 +787,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -837,94 +849,102 @@
 "           "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:34
@@ -939,68 +959,72 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr ""
@@ -1112,14 +1136,18 @@
 msgid "To use the voucher, register for the event "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1132,14 +1160,19 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1162,14 +1195,45 @@
 msgid "Filter vouchers"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1191,35 +1255,23 @@
 #, python-format
 msgid ""
 "\n"
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1227,152 +1279,156 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1003
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-06-24 15:05+0000\n"
+"PO-Revision-Date: 2023-06-07 13:14+0000\n"
 "Last-Translator: Tom Teichler <tom.teichler@teckids.org>\n"
 "Language-Team: German <https://translate.edugit.org/projects/hacknfun/"
 "aleksis-app-paweljong/de/>\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -47,24 +47,30 @@
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address "
 "must be one\n"
 "           that you, the participating child, check and read yourself, not "
 "one owned by your\n"
 "           parents. Of course, we will always send important information to "
-"your parents as well.\n"
+"your parents as\n"
+"           well, and of course you should always talk to your parents if "
+"you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 "\n"
 "           Jeder Teilnehmende benötigt seine eigene E-Mail-Adresse. Diese "
 "Adresse muss eine Adresse sein,\n"
 "           die du selbst abrufst und liest, und die nicht deinen Eltern "
 "gehört.\n"
 "           Wichtige Informationen senden wir natürlich immer zusätzlich an "
 "deine Eltern.\n"
+"\tNatürlich solltest du mit deinen Eltern immer reden, falls du beim Lesen "
+"deiner E-Mails\n"
+"\tFragen oder Sorgen hast.\n"
 "           "
 
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must "
 "be one\n"
 "           that you, the participating child, check and read yourself, not "
@@ -83,15 +89,15 @@
 
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register "
 "a new one. Login\n"
 "           with your existing username and password. If you have forgotten "
 "your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your "
+"           send us an e-mail (please do this yourself, with the help of your "
 "parents, if needed).\n"
 "           "
 msgstr ""
 "\n"
 "           Wenn du bereits einen Teckids-Account hast, lege Dir bitte keinen "
 "neuen an. Melde\n"
 "           dich mit deinem vorhandenen Benutzernamen und Passwort an. Wenn "
@@ -122,19 +128,35 @@
 "           Dir bei uns eine E-Mail-Adresse registrieren.\n"
 "           "
 
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their "
 "child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents "
+"to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 "\n"
-"           Wir bitten die Eltern darum, diese Anmeldung nicht "
-"stellvertretend für ihr Kind auszufüllen.\n"
+"           Wir bitten Eltern, die Anmeldung nicht stellvertretend für ihr "
+"Kind auszufüllen.\n"
+"\tUnser Teilnehmenden müssen freien Zugriff auf ihre Accounts und "
+"Postfächer\n"
+"\thaben und ihre Eltern müssen erlauben, dass sie ihre Passwörter "
+"geheimhalten.\n"
+"\tWir bitten Eltern, uns zu kontaktieren, falls sie Fragen zu dieser "
+"Regelung haben\n"
+"\tund natürlich ermutigen wir alle Kinder, ihren Eltern alles, was sie nicht "
+"verstehen\n"
+"\toder wozu sie Fragen haben, zu zeigen.\n"
 "           "
 
 msgid ""
 "\n"
 "           Welcome to the registration for this event! Please make sure to "
 "fill in\n"
 "           the registration yourself, as the child who wants to "
@@ -280,32 +302,44 @@
 
 msgid "Billing information"
 msgstr "Zahlungsinformationen"
 
 msgid "Check in"
 msgstr "Einchecken"
 
+msgid "Checked by person"
+msgstr "Eingechecked von person"
+
 msgid "Checked in"
 msgstr "Eingechecked"
 
 msgid "Checked in at"
 msgstr "Eingechecked am"
 
+msgid "Checked person"
+msgstr "Eingecheckte Person"
+
+msgid "Checkpoint"
+msgstr "Checkpoint"
+
 msgid "Child groups"
 msgstr "Kind-Gruppen"
 
 msgid "Clear"
 msgstr "Leeren"
 
 msgid "Code"
 msgstr "Code"
 
 msgid "Colour"
 msgstr "Farbe"
 
+msgid "Comment"
+msgstr "Kommentar"
+
 msgid "Comment / remarks"
 msgstr "Kommentar / Anmerkungen"
 
 msgid "Confirmation text"
 msgstr "Bestätigungstext"
 
 msgid "Consent"
@@ -360,14 +394,17 @@
 msgid "Creative Commons with attribution, 4.0 or later"
 msgstr ""
 "Creative Commons mit Namensnennung 4.0 International (CC BY 4.0) oder neuer"
 
 msgid "Date"
 msgstr "Datum"
 
+msgid "Date and time of check"
+msgstr "Datum und Uhrzeit des Check-Ins"
+
 msgid "Date data"
 msgstr "Kalenderdaten"
 
 msgid "Date of birth"
 msgstr "Geburtsdatum"
 
 msgid "Date of event"
@@ -522,15 +559,15 @@
 msgid "I already have an account"
 msgstr "Ich habe bereits ein Konto"
 
 msgid ""
 "I confirm that the retraction of the registration is not possible anymore "
 "after {}"
 msgstr ""
-"Ich bestätigte, dass eine Stornierung nach dem {} nicht mehr möglich ist"
+"Ich bestätige, dass eine Stornierung nach dem {} nicht mehr möglich ist"
 
 msgid "I don't have a personal email address"
 msgstr "Ich habe keine persönliche E-Mail-Adresse"
 
 msgid "I have a personal email address"
 msgstr "Ich habe eine persönliche E-Mail-Adresse"
 
@@ -569,29 +606,38 @@
 "parents. After that, you will need to confirm that you agree with everything "
 "yourself, and that your parents also agree."
 msgstr ""
 "Zuletzt lies bitte alle Bedingungen sorgfältig zusammen mit deinen Eltern "
 "durch. Danach musst du bestätigen, dass du und deine Eltern alles gelesen "
 "habt und akzeptiert."
 
+msgid "Latitude of check"
+msgstr "Breitengrad des Check-Ins"
+
 msgid "Legal guardians / parents"
 msgstr "Erziehungsberechtigte / Eltern"
 
 msgid "Login"
 msgstr "Anmelden"
 
+msgid "Longitude of check"
+msgstr "Längengrad des Check-Ins"
+
 msgid "Mail recipient for event notifications"
 msgstr "Mail-Empfänger für Veranstaltungsbenachrichtigungen"
 
 msgid "Mailing is active"
 msgstr "Mailing ist aktiv"
 
 msgid "Manage events"
 msgstr "Veranstaltungen verwalten"
 
+msgid "Mark payed"
+msgstr "Als bezahlt markieren"
+
 msgid "Max. participants"
 msgstr "Maximale Teilnehmerzahl"
 
 msgid "Maximum participants"
 msgstr "Maximale Teilnehmerzahl"
 
 msgid "Medical information / intolerances"
@@ -605,14 +651,20 @@
 
 msgid "Name"
 msgstr "Name"
 
 msgid "Name of school"
 msgstr "Name der Schule"
 
+msgid "New account"
+msgstr "Neues Konto"
+
+msgid "New account: %(person)s"
+msgstr "Neues Konto: %(person)s"
+
 msgid "New event"
 msgstr "Neue Veranstaltung"
 
 msgid "New registration"
 msgstr "Neue Anmeldung"
 
 msgid "New registration: %(event)s"
@@ -724,14 +776,19 @@
 "select a payment method. The real payment will be done in a separate step, "
 "after the registration is complete."
 msgstr ""
 "Bitte wählen mit Deinen Eltern, wie Du bezahlen möchtest. In diesem Schritt "
 "wird nur die Zahlungsmethode ausgewählt. Die eigentliche Zahlung wird in "
 "einem separaten Schritt nach der Anmeldung durchgeführt."
 
+msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
+msgstr ""
+"Bitte gib einen Kommentar ein, der den Checkpoint beschreibt (z.B. "
+"Abendessen)."
+
 msgid "Please enter a username."
 msgstr "Bitte wähle einen Benutzernamen."
 
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr "Bitte trage die Klasse ein, in die du gehst (z.B. 8a)."
 
 msgid ""
@@ -812,14 +869,17 @@
 
 msgid "Registration until"
 msgstr "Anmeldung möglich bis"
 
 msgid "Registrations"
 msgstr "Anmeldungen"
 
+msgid "Related event"
+msgstr "Zugehörige Veranstaltung"
+
 msgid "Request replies to"
 msgstr "Antworten an"
 
 msgid "Retract"
 msgstr "Stornieren"
 
 msgid "Retracted"
@@ -872,14 +932,20 @@
 
 msgid "Send notification"
 msgstr "Benachrichtigung senden"
 
 msgid "Send to guardians"
 msgstr "An Erziehungsberechtigte senden"
 
+msgid "Send to participants who did not check in"
+msgstr "An Teilnehmende senden, die nicht eingechecked sind"
+
+msgid "Send to participants who retracted"
+msgstr "An Teilnehmende senden, die storniert haben"
+
 msgid "Send to registered person"
 msgstr "An angemeldete Personen senden"
 
 msgid "Sender"
 msgstr "Absender"
 
 msgid "Sent to persons"
@@ -902,17 +968,23 @@
 
 msgid "States"
 msgstr "Status"
 
 msgid "Street"
 msgstr "Straße"
 
+msgid "Submit geolocation"
+msgstr "Standort speichern"
+
 msgid "Successfully checked in."
 msgstr "Erfolgreich eingechecked."
 
+msgid "Successfully marked as payed!"
+msgstr "Erfolgreich als bezahlt markiert!"
+
 msgid "Sync members"
 msgstr "Teilnehmer syncronisieren"
 
 msgid ""
 "Tell us how we can contact you. You will receive information about the event "
 "by e-mail. Please use your personal e-mail address where you will read mails "
 "yourself, not an address of your parents. We will always send all important "
@@ -962,14 +1034,17 @@
 
 msgid "The info mailing has been deleted."
 msgstr "Das Info-Mailing wurde gelöscht."
 
 msgid "The info mailing has been saved."
 msgstr "Das Info-Mailing wurde gespeichert."
 
+msgid "The provided username is not linked to a person."
+msgstr "Der angegebene Benutzername ist nicht mit einer Person verknüpft."
+
 msgid "The registration has been deleted."
 msgstr "Die Veranstaltung wurde gelöscht."
 
 msgid "The registration has been saved."
 msgstr "Die Anmeldung wurde gespeichert."
 
 msgid "The term has been created."
@@ -1005,14 +1080,17 @@
 
 msgid "Upcoming events"
 msgstr "Anstehende Veranstaltungen"
 
 msgid "Used by"
 msgstr "Benutzt von"
 
+msgid "Username"
+msgstr "Benutzername"
+
 msgid "View"
 msgstr "Ansehen"
 
 msgid "View registration"
 msgstr "Anmeldung ansehen"
 
 msgid "Voucher"
@@ -1103,7 +1181,10 @@
 msgstr "Unterschriftenliste"
 
 msgid "subject"
 msgstr "Betreff"
 
 msgid "to visit event"
 msgstr "für die Veranstaltung"
+
+msgid "{} successfully checked for {}."
+msgstr "{} erfolgreich für {} eingechecked."
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
-"PO-Revision-Date: 2022-06-24 15:05+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
+"PO-Revision-Date: 2023-06-07 13:14+0000\n"
 "Last-Translator: Tom Teichler <tom.teichler@teckids.org>\n"
 "Language-Team: German <https://translate.edugit.org/projects/hacknfun/aleksis-app-paweljong/de/>\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -78,25 +78,23 @@
 msgid "Date data"
 msgstr "Kalenderdaten"
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr "Veranstaltungsdetails"
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr "Bedingungen"
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr "Info-Mailings"
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -106,15 +104,15 @@
 msgid "Person the voucher is valid for"
 msgstr "Person, für die der Gutschein gültig ist"
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr "Rabatt"
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr "Gruppe"
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -177,15 +175,15 @@
 msgstr "Persönliche Daten"
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr "Addressdaten"
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr "Kontaktdaten"
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr "Angaben zur Schule"
 
@@ -202,69 +200,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr "Nachname"
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr "Straße"
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr "Hausnummer"
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr "Postleitzahl"
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr "Stadt"
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr "Handynummer"
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr "deine Handynummer hilft uns, dich bei Notfällen während der Veranstaltung zu erreichen, z.B. wenn du alleine mit deiner Gruppe auf einer Konferenz unterwegs bist. Wenn du kein Handy hast, kannst du dieses Feld ignorieren."
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr "Geburtsdatum"
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr "Geschlecht"
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr "Aus verschiedenen Gründen, z.B da wir aus rechtlichen Gründen die Geschlechtertrennung während der Nacht aufrechterhalten müssen, müssen wir wissen, ob du ein Junge oder ein Mädchen bist."
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr "E-Mail-Adresse"
 
@@ -284,23 +300,23 @@
 msgid "School place"
 msgstr "Ort der Schule"
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr "Bitte trage die Stadt ein, wo sich deine Schule befindet."
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr "Schulklasse"
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr "Bitte trage die Klasse ein, in die du gehst (z.B. 8a)."
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr "Medizinische Informationen / Intoleranzen"
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr "Sonstige Anmerkungen"
 
@@ -334,83 +350,55 @@
 
 #: aleksis/apps/paweljong/forms.py:361
 msgid "Our association would like to offer all children and young people the opportunity to participate in our events. Sometimes, however, families cannot afford the full fee. We therefore have a budget from which we can promote participation after we have carefully examined the necessity and eligibility. We rely on donations for this budget. If you would like to donate a voluntary additional amount for this budget, please indicate this here."
 msgstr "Unser Verein möchte allen Kindern und Jugendlichen die Möglichkeit bieten, an unseren Veranstaltungen teilzunehmen. Manchmal können sich Familien jedoch nicht die volle Gebühr leisten. Wir haben also ein Budget, aus dem wir die Teilnahme fördern können, nachdem wir die Notwendigkeit und Förderfähigkeit sorgfältig geprüft haben. Für dieses Budget sind wir auf Spenden angewiesen. Wenn Sie für dieses Budget einen freiwilligen Zusatzbetrag spenden möchten, geben Sie dies bitte hier an."
 
 #: aleksis/apps/paweljong/forms.py:393
 msgid "I confirm that the retraction of the registration is not possible anymore after {}"
-msgstr "Ich bestätigte, dass eine Stornierung nach dem {} nicht mehr möglich ist"
+msgstr "Ich bestätige, dass eine Stornierung nach dem {} nicht mehr möglich ist"
 
 #: aleksis/apps/paweljong/forms.py:440
 msgid "Account data"
 msgstr "Kontodaten"
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr "Der Benutzername darf nur Kleinbuchstaben und Zahlen beinhalten, und muss mit einem Buchstaben beginnen."
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr "Person"
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr "Bitte wähle einen Benutzernamen."
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
-msgstr ""
+msgstr "Kommentar"
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
-msgstr ""
+msgstr "Bitte gib einen Kommentar ein, der den Checkpoint beschreibt (z.B. Abendessen)."
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr "Registrieren"
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr "Veranstaltungen"
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr "Gutscheine"
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr "Registrierungsstatus"
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr "Teilnehmerlisten generieren"
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr "Anstehende Veranstaltungen"
+msgstr "Standort speichern"
 
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr "Name"
 
@@ -454,183 +442,191 @@
 msgid "Send to registered person"
 msgstr "An angemeldete Personen senden"
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr "An Erziehungsberechtigte senden"
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr "An Teilnehmende senden, die storniert haben"
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr "An Teilnehmende senden, die nicht eingechecked sind"
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr "Anzeigename"
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr "Beschreibung"
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr "Veröffentlichen"
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr "Slug"
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr "Datum der Veranstaltung"
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr "Anmeldungsschluss"
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr "Kündigungsfrist"
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr "Kosten in €"
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr "Maximale Teilnehmerzahl"
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr "Informationen über die Veranstaltung"
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr "An Personen gesendet"
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr "Gutscheine"
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr "Veranstaltung"
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr "Benutzt von"
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr "Anmeldedatum"
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr "Name der Schule"
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr "Ort der Schule"
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr "Kommentar / Anmerkungen"
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr "Gutschein"
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr "Spende"
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr "Akzeptierte Bedingungen"
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr "Status"
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr "Storniert"
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr "Storniert am"
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr "Eingechecked"
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr "Eingechecked am"
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr "Person ist bereits eingechecked!"
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr "Teilnahme von {} bei Veranstaltung {}"
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr "Social-Sponsoring / Spende"
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr "Rabatt"
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr "Veranstaltungsanmeldung"
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr "Veranstaltungsanmeldungen"
 
-#: aleksis/apps/paweljong/models.py:412
-#, fuzzy
-#| msgid "Create event"
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
-msgstr "Veranstaltung erstellen"
+msgstr "Zugehörige Veranstaltung"
 
-#: aleksis/apps/paweljong/models.py:413
-#, fuzzy
-#| msgid "Checked in"
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
-msgstr "Eingechecked"
+msgstr "Eingecheckte Person"
 
-#: aleksis/apps/paweljong/models.py:414
-#, fuzzy
-#| msgid "Checked in"
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
-msgstr "Eingechecked"
+msgstr "Eingechecked von person"
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
-msgstr ""
+msgstr "Datum und Uhrzeit des Check-Ins"
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
-msgstr ""
+msgstr "Breitengrad des Check-Ins"
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
-msgstr ""
+msgstr "Längengrad des Check-Ins"
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr "Paweljong"
 
 #: aleksis/apps/paweljong/preferences.py:20
 msgid "Mail recipient for event notifications"
@@ -653,15 +649,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr "Bearbeiten"
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr "Öffentliche Seite"
 
@@ -676,29 +672,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr "Code"
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr "Löschen"
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr "Drucken"
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr "Anmeldung ansehen"
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr "Einchecken"
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr "Personen hinzufügen"
 
@@ -730,18 +726,16 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:58
 msgid "Next"
 msgstr "Weiter"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:30
-#, fuzzy
-#| msgid "Check in"
 msgid "Checkpoint"
-msgstr "Einchecken"
+msgstr "Checkpoint"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:20
 msgid "Create event"
 msgstr "Veranstaltung erstellen"
 
@@ -793,26 +787,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr "Veranstaltung bearbeiten"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr "Jetzt anmelden"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr "Nicht verfügbar"
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr "Veranstaltungen"
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr "Anstehende Veranstaltungen"
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr "Veranstaltungen an denen du teilgenommen hast"
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -850,35 +854,50 @@
 "           deinen Eltern oder Erziehungsberechtigten ausfüllen.\n"
 "           "
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 "\n"
-"           Wir bitten die Eltern darum, diese Anmeldung nicht stellvertretend für ihr Kind auszufüllen.\n"
+"           Wir bitten Eltern, die Anmeldung nicht stellvertretend für ihr Kind auszufüllen.\n"
+"\tUnser Teilnehmenden müssen freien Zugriff auf ihre Accounts und Postfächer\n"
+"\thaben und ihre Eltern müssen erlauben, dass sie ihre Passwörter geheimhalten.\n"
+"\tWir bitten Eltern, uns zu kontaktieren, falls sie Fragen zu dieser Regelung haben\n"
+"\tund natürlich ermutigen wir alle Kinder, ihren Eltern alles, was sie nicht verstehen\n"
+"\toder wozu sie Fragen haben, zu zeigen.\n"
 "           "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 "\n"
 "           Jeder Teilnehmende benötigt seine eigene E-Mail-Adresse. Diese Adresse muss eine Adresse sein,\n"
 "           die du selbst abrufst und liest, und die nicht deinen Eltern gehört.\n"
 "           Wichtige Informationen senden wir natürlich immer zusätzlich an deine Eltern.\n"
+"\tNatürlich solltest du mit deinen Eltern immer reden, falls du beim Lesen deiner E-Mails\n"
+"\tFragen oder Sorgen hast.\n"
 "           "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
@@ -887,60 +906,60 @@
 "\n"
 "           Wenn du bisher keine eigene E-Mail-Adresse hast, und keine bei den \"großen\"\n"
 "           Anbietern anlegen kannst oder möchtest (denke daran, dass Google, Outlook etc.\n"
 "           Accounts erst ab 16 erlauben, und oft deine Daten sammeln und analysieren), kannst du\n"
 "           Dir bei uns eine E-Mail-Adresse registrieren.\n"
 "           "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 "\n"
 "           Wenn du bereits einen Teckids-Account hast, lege Dir bitte keinen neuen an. Melde\n"
 "           dich mit deinem vorhandenen Benutzernamen und Passwort an. Wenn du dein\n"
 "           Passwort vergessen hast, schreibe uns bitte eine E-Mail (bitte mache das selbst mit der Hilfe\n"
 "           deiner Eltern, falls nötig).\n"
 "           "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr "Ich habe bereits ein Konto"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr "Ich habe eine persönliche E-Mail-Adresse"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr "Ich habe keine persönliche E-Mail-Adresse"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 "\n"
 "         Wenn du bereits einen Teckids-Account hast, melde dich bitte hier an. Wenn du dein Passwort\n"
 "         vergessen hast, oder Probleme bei der Anmeldung hast, sende uns bitte eine E-Mail.\n"
 "         "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr "Anmelden"
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
@@ -949,30 +968,30 @@
 "\n"
 "         Du kannst Dir jetzt eine bei uns gehostete E-Mail-Adresse aussuchen.\n"
 "         Informationen, wie Du deine Mails abrufen kannst, findest Du unter <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 "\n"
 "         Du wirst nach deiner persönlichen E-Mail-Adresse gefragt werden. Bitte denke daran,\n"
 "         dass du keine Adresse nutzen solltest, die deinen Eltern gehört. Wenn du keine persönliche\n"
 "         E-Mail-Adresse hast, nutze die dafür vorgesehene Option!\n"
 "         "
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 "\n"
 "         Die Anmeldung ist nicht mehr möglich.\n"
@@ -990,68 +1009,72 @@
 msgstr "Erfolgreich angemeldet"
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr "Anmeldung bearbeiten"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr "Stornieren"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr "Benachrichtigung"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr "Rechnung"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr "Person bearbeiten"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr "Stornierungsinformationen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr "Ja"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr "Anmeldungsinformationen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr "Akzeptiert"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr "Noch nicht eingechecked."
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr "Rechnungsinformationen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr "Zahlungsinformationen"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr "Bezahlung"
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr "Als bezahlt markieren"
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr "Erziehungsberechtigte / Eltern "
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr "Benachrichtigung senden"
@@ -1173,14 +1196,18 @@
 msgid "To use the voucher, register for the event "
 msgstr "Um den Gutschein zu nutzen, registriere dich für die Veranstaltung "
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr "hier"
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr "Registrieren"
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1198,14 +1225,19 @@
 msgstr "Registrierungsstatus erstellen"
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr "Registrierungsstatus bearbeiten"
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr "Registrierungsstatus"
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr "Bedingung erstellen"
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1228,14 +1260,45 @@
 msgid "Filter vouchers"
 msgstr "Gutscheine filtern"
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr "Ausgewählte Gutscheine"
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr "Neues Konto"
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr "Neues Konto: %(person)s"
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr "Benutzername"
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr "Erziehungsberechtigter"
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr "Dein AlekSIS-Team"
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr "Neue Veranstaltung"
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1260,35 +1323,23 @@
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 "\n"
 "        Die Veranstaltung wurde von %(sender)s erstellt\n"
 "    "
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr "Dein AlekSIS-Team"
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr "Neue Anmeldung"
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr "Neue Anmeldung: %(event)s"
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr "Erziehungsberechtigter"
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr "Angaben zur Bezahlung"
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1296,162 +1347,176 @@
 msgstr "Zusätzliches"
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr "Neue Anmeldung: %(registration)s"
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr "Die Veranstaltung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr "Die Veranstaltungsanmeldung wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr "Die Veranstaltungsanmeldung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr "Die Anmeldung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr "Die Veranstaltung wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr "Der Gutschein wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr "Der Gutschein wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr "Der Gutschein wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr "E-Mail-Adresse erstellen"
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr "Alle Teilnehmenden brauchen eine persönliche Adresse, die sie selbst abrufen und lesen. Wir bieten die Möglichkeit an, E-Mail-Adressen auf unseren sicheren Servern zu registrieren. Informationen, wie Du deine Mails abrufen kannst, findest Du unter <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr "Zuerst, gib bitte einige Informationen über dich an und prüfe, dass alle Informationen korrekt sind."
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr "Kontaktinformationen"
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr "Teile uns mit, wie wir dich erreichen können. Du wirst Informationen zu der Veranstaltung per E-Mail erhalten. Bitte nutze deine persönliche E-Mail-Adresse, die selbst liest, nicht die E-Mail-Adresse deiner Eltern. Wir senden wichtige Informationen immer zusätzlich an deine Eltern. Ihre E-Mail-Adresse wirst du im nächsten Schritt eingeben."
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr "Erziehungsberechtigte / Eltern"
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr "Teile uns mit, wie wir deine Eltern oder Erziehungsberechtigten während der Veranstaltung erreichen können. Das sollte eine Person sein, die während der Anmeldung (also jetzt gerade), bei Dir ist. Wenn du einen weiteren Erziehungsberechtigten angeben möchtest, kannst du uns das später als Kommentar mitteilen."
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr "Zusätzliche Anmeldungsinformationen"
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr "Bitte beantworte die folgenden Fragen so genau wie möglich, sodass wir sicher gehen können, dass deine Teilnahme bei der Veranstaltung so gut wie möglich organisiert ist."
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr "Bitte wählen mit Deinen Eltern, wie Du bezahlen möchtest. In diesem Schritt wird nur die Zahlungsmethode ausgewählt. Die eigentliche Zahlung wird in einem separaten Schritt nach der Anmeldung durchgeführt."
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr "Einverständnis"
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr "Zuletzt lies bitte alle Bedingungen sorgfältig zusammen mit deinen Eltern durch. Danach musst du bestätigen, dass du und deine Eltern alles gelesen habt und akzeptiert."
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr "Du hast einen ungütigen Gutscheincode eingegeben!"
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr "Du hast dich erfolgreich zu der Veranstaltung angemeldet. Bitte gib uns ein paar Tage, um deine Anmeldung zu bearbeiten. Du wirst dann eine E-Mail von uns bekommen."
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr "Du hast dich zu einer Veranstaltung angemeldet"
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr "Du hast dich zur Veranstaltung %s angemeldet"
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr "Die Bedingung wurde erfolgreich erstellt."
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr "Die Bedingung wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr "Ankündigungs-Feed aller bevorstehenden Veranstaltungen"
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr "Das Info-Mailing wurde erstellt."
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr "Das Info-Mailing wurde gespeichert."
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr "Das Info-Mailing wurde gelöscht."
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr "Anmeldung erfolgreich storniert."
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr "Person {person} erfolgreich hinzugefügt!"
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr "Person existiert nicht!"
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
-msgstr ""
+msgstr "Der angegebene Benutzername ist nicht mit einer Person verknüpft."
 
-#: aleksis/apps/paweljong/views.py:1003
-#, fuzzy
-#| msgid "Successfully checked in."
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
-msgstr "Erfolgreich eingechecked."
+msgstr "{} erfolgreich für {} eingechecked."
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr "Erfolgreich eingechecked."
 
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr "Erfolgreich als bezahlt markiert!"
+
+#~ msgid "Generate participant list"
+#~ msgstr "Teilnehmerlisten generieren"
+
+#~ msgid ""
+#~ "\n"
+#~ "           We ask parents to not fill in the registration on behalf of their child.\n"
+#~ "           "
+#~ msgstr ""
+#~ "\n"
+#~ "           Wir bitten die Eltern darum, diese Anmeldung nicht stellvertretend für ihr Kind auszufüllen.\n"
+#~ "           "
+
 #~ msgid "Filter registrations"
 #~ msgstr "Anmeldungen filtern"
 
 #~ msgid "Selected registrations"
 #~ msgstr "Ausgewählte Anmeldungen"
 
 #~ msgid "Parents: I authorize the creditor Teckids e.V., Kennedyallee 18, 53175 Bonn with creditor ID DE70ZZZ00001497650, to collect the participant fee from my account once using the SEPA core direct debit. At the same time, I instruct my bank to redeem the SEPA core direct debit withdrawn from my account by Teckids e.V."
@@ -1504,17 +1569,14 @@
 
 #~ msgid "incl. program, overnight stays, trips and meals"
 #~ msgstr "inkl. Programm, Übernachtungen Fahrten und Mahlzeiten"
 
 #~ msgid "(if part of the event)"
 #~ msgstr "(falls Teil der Veranstaltung)"
 
-#~ msgid "Booked participants slots"
-#~ msgstr "Gebuchte Teilnehmerplätze"
-
 #~ msgid ""
 #~ "\n"
 #~ "         You can now choose a personal e-mail address hosted on our servers.\n"
 #~ "         "
 #~ msgstr ""
 #~ "\n"
 #~ "         du kannst eine persönliche E-Mail-Adresse wählen, die auf unseren Servern gehostet wird.\n"
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -78,25 +78,23 @@
 msgid "Date data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -106,15 +104,15 @@
 msgid "Person the voucher is valid for"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -177,15 +175,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr ""
 
@@ -202,69 +200,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr ""
 
@@ -284,23 +300,23 @@
 msgid "School place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr ""
 
@@ -344,73 +360,45 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
 msgstr ""
 
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr ""
-
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr ""
 
@@ -454,175 +442,189 @@
 msgid "Send to registered person"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:412
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:413
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:414
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
@@ -647,15 +649,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr ""
 
@@ -670,29 +672,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr ""
 
@@ -785,26 +787,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -837,94 +849,102 @@
 "           "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:34
@@ -939,68 +959,72 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr ""
@@ -1112,14 +1136,18 @@
 msgid "To use the voucher, register for the event "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1132,14 +1160,19 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1162,14 +1195,45 @@
 msgid "Filter vouchers"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1191,35 +1255,23 @@
 #, python-format
 msgid ""
 "\n"
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1227,152 +1279,156 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1003
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -77,25 +77,23 @@
 msgid "Date data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -105,15 +103,15 @@
 msgid "Person the voucher is valid for"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -176,15 +174,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr ""
 
@@ -201,69 +199,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr ""
 
@@ -283,23 +299,23 @@
 msgid "School place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr ""
 
@@ -343,73 +359,45 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
 msgstr ""
 
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr ""
-
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr ""
 
@@ -453,175 +441,189 @@
 msgid "Send to registered person"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:412
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:413
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:414
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
@@ -646,15 +648,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr ""
 
@@ -669,29 +671,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr ""
 
@@ -784,26 +786,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -836,94 +848,102 @@
 "           "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:34
@@ -938,68 +958,72 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr ""
@@ -1111,14 +1135,18 @@
 msgid "To use the voucher, register for the event "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1131,14 +1159,19 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1161,14 +1194,45 @@
 msgid "Filter vouchers"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1190,35 +1254,23 @@
 #, python-format
 msgid ""
 "\n"
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1226,152 +1278,156 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1003
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -77,25 +77,23 @@
 msgid "Date data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -105,15 +103,15 @@
 msgid "Person the voucher is valid for"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -176,15 +174,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr ""
 
@@ -201,69 +199,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr ""
 
@@ -283,23 +299,23 @@
 msgid "School place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr ""
 
@@ -343,73 +359,45 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
 msgstr ""
 
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr ""
-
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr ""
 
@@ -453,175 +441,189 @@
 msgid "Send to registered person"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:412
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:413
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:414
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
@@ -646,15 +648,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr ""
 
@@ -669,29 +671,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr ""
 
@@ -784,26 +786,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -836,94 +848,102 @@
 "           "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:34
@@ -938,68 +958,72 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr ""
@@ -1111,14 +1135,18 @@
 msgid "To use the voucher, register for the event "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1131,14 +1159,19 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1161,14 +1194,45 @@
 msgid "Filter vouchers"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1190,35 +1254,23 @@
 #, python-format
 msgid ""
 "\n"
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1226,152 +1278,156 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1003
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-28 15:44+0000\n"
+"POT-Creation-Date: 2023-07-02 13:33+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -77,25 +77,23 @@
 msgid "Date data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:51
 msgid "Event details"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/menus.py:37
-#: aleksis/apps/paweljong/models.py:129
+#: aleksis/apps/paweljong/forms.py:52 aleksis/apps/paweljong/models.py:141
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/terms.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:7
 msgid "Terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/menus.py:59
-#: aleksis/apps/paweljong/models.py:132
+#: aleksis/apps/paweljong/forms.py:53 aleksis/apps/paweljong/models.py:144
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:6
 #: aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html:7
 msgid "Info mailings"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:108
 msgid "Event the voucher is valid for"
@@ -105,15 +103,15 @@
 msgid "Person the voucher is valid for"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:110
 msgid "Voucher discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:113
+#: aleksis/apps/paweljong/forms.py:118 aleksis/apps/paweljong/models.py:125
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:36
 msgid "Group"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:120
 msgid "Select group to generate list"
@@ -176,15 +174,15 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:193
 msgid "Address data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:198
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:71
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:72
 msgid "Contact details"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:202
 msgid "School details"
 msgstr ""
 
@@ -201,69 +199,87 @@
 #: aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html:19
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:20
 #: aleksis/apps/paweljong/templates/paweljong/print/list_sign.html:20
 msgid "Last name"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:218
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:15
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:18
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:67
 msgid "Street"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:222
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:16
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:46
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:19
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:68
 msgid "Housenumber"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:226
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:17
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:47
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:20
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:69
 msgid "Postal code"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:230
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:18
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:48
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:11
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:39
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:21
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:70
 msgid "Place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:234
 #: aleksis/apps/paweljong/templates/paweljong/print/corona.html:22
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:23
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:14
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:26
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:44
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:55
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:17
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:27
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:66
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:76
 msgid "Mobile number"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:237
 msgid "Your mobile number helps us to reach you in an emergency during the event, e.g. if you are alone with your group at a conference or similar. If you don't have a cell phone, you can leave the field blank."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:244 aleksis/apps/paweljong/forms.py:449
 #: aleksis/apps/paweljong/templates/paweljong/print/list_participants.html:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:12
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:42
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:15
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:64
 msgid "Date of birth"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:248
 msgid "Sex"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:250
 msgid "For various reasons, e.g. because we have to keep gender segregation during the night for legal reasons, we need to know if you are a boy or a girl."
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:258
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:13
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:25
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:43
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:54
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:16
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:26
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:65
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:75
 msgid "Email address"
 msgstr ""
 
@@ -283,23 +299,23 @@
 msgid "School place"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:273
 msgid "Enter the place (city) where your school is located."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:261
+#: aleksis/apps/paweljong/forms.py:277 aleksis/apps/paweljong/models.py:281
 msgid "School class"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:278
 msgid "Please enter the class you are in (e.g. 8a)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:266
+#: aleksis/apps/paweljong/forms.py:286 aleksis/apps/paweljong/models.py:286
 msgid "Medical information / intolerances"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:290
 msgid "Other remarks"
 msgstr ""
 
@@ -343,73 +359,45 @@
 msgid "Account data"
 msgstr ""
 
 #: aleksis/apps/paweljong/forms.py:455
 msgid "The username must only contain lower case letters and numbers, and must begin with a letter."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:524
-#: aleksis/apps/paweljong/models.py:228 aleksis/apps/paweljong/models.py:257
+#: aleksis/apps/paweljong/forms.py:502 aleksis/apps/paweljong/forms.py:526
+#: aleksis/apps/paweljong/models.py:248 aleksis/apps/paweljong/models.py:277
 #: aleksis/apps/paweljong/tables.py:46
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:8
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:38
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:61
 msgid "Person"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:525
+#: aleksis/apps/paweljong/forms.py:504 aleksis/apps/paweljong/forms.py:527
 msgid "Please enter a username."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:518 aleksis/apps/paweljong/models.py:417
+#: aleksis/apps/paweljong/forms.py:520 aleksis/apps/paweljong/models.py:454
 msgid "Comment"
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:519
+#: aleksis/apps/paweljong/forms.py:521
 msgid "Please enter a comment describing the checkpoint (e.g. Dinner)."
 msgstr ""
 
-#: aleksis/apps/paweljong/forms.py:531
+#: aleksis/apps/paweljong/forms.py:533
 msgid "Submit geolocation"
 msgstr ""
 
-#: aleksis/apps/paweljong/menus.py:6
-#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
-msgid "Register"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:14
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
-msgid "Events"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:26 aleksis/apps/paweljong/models.py:214
-#: aleksis/apps/paweljong/models.py:215
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
-msgid "Vouchers"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:48
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
-#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
-msgid "Registration states"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:70
-msgid "Generate participant list"
-msgstr ""
-
-#: aleksis/apps/paweljong/menus.py:81
-#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
-#: aleksis/apps/paweljong/views.py:748
-msgid "Upcoming events"
-msgstr ""
-
 #: aleksis/apps/paweljong/models.py:28
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:10
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:24
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:40
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:53
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:25
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:63
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:74
 msgid "Name"
 msgstr ""
 
@@ -453,175 +441,189 @@
 msgid "Send to registered person"
 msgstr ""
 
 #: aleksis/apps/paweljong/models.py:53
 msgid "Send to guardians"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:111
+#: aleksis/apps/paweljong/models.py:55
+msgid "Send to participants who retracted"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:58
+msgid "Send to participants who did not check in"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:123
 msgid "Display name"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:115
+#: aleksis/apps/paweljong/models.py:127
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:9
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:37
 msgid "Description"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:116
+#: aleksis/apps/paweljong/models.py:128
 msgid "Publish"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:118
+#: aleksis/apps/paweljong/models.py:130
 msgid "Slug"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:121
+#: aleksis/apps/paweljong/models.py:133
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:12
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:40
 msgid "Date of event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:122
+#: aleksis/apps/paweljong/models.py:134
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:13
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:41
 msgid "Registration deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:123
+#: aleksis/apps/paweljong/models.py:135
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:14
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:42
 msgid "Retraction deadline"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:126
+#: aleksis/apps/paweljong/models.py:138 aleksis/apps/paweljong/models.py:312
 msgid "Cost in €"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:127
+#: aleksis/apps/paweljong/models.py:139
 msgid "Maximum participants"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:128
+#: aleksis/apps/paweljong/models.py:140
 msgid "Information about the event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:205
+#: aleksis/apps/paweljong/models.py:225
 msgid "Sent to persons"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:221 aleksis/apps/paweljong/models.py:255
+#: aleksis/apps/paweljong/models.py:234 aleksis/apps/paweljong/models.py:235
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:7
+msgid "Vouchers"
+msgstr ""
+
+#: aleksis/apps/paweljong/models.py:241 aleksis/apps/paweljong/models.py:275
 #: aleksis/apps/paweljong/tables.py:12 aleksis/apps/paweljong/tables.py:43
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:4
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:8
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:10
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:57
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:59
 msgid "Event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:237
+#: aleksis/apps/paweljong/models.py:257
 msgid "Used by"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:258
+#: aleksis/apps/paweljong/models.py:278
 msgid "Registration date"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:260
+#: aleksis/apps/paweljong/models.py:280
 msgid "Name of school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:262
+#: aleksis/apps/paweljong/models.py:282
 msgid "Place of the school"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:264
+#: aleksis/apps/paweljong/models.py:284
 msgid "Comment / remarks"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:271
+#: aleksis/apps/paweljong/models.py:291
 msgid "Voucher"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:275
+#: aleksis/apps/paweljong/models.py:295
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:31
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:80
 msgid "Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:278
+#: aleksis/apps/paweljong/models.py:298
 msgid "Accepted terms"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:283
+#: aleksis/apps/paweljong/models.py:303
 msgid "States"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:286
+#: aleksis/apps/paweljong/models.py:306
 msgid "Retracted"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:287
+#: aleksis/apps/paweljong/models.py:307
 msgid "Retracted at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:289
+#: aleksis/apps/paweljong/models.py:309
 msgid "Checked in"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:290
+#: aleksis/apps/paweljong/models.py:310
 msgid "Checked in at"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:298 aleksis/apps/paweljong/views.py:1034
+#: aleksis/apps/paweljong/models.py:321 aleksis/apps/paweljong/views.py:1087
 msgid "Person is already checked in!"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:334
+#: aleksis/apps/paweljong/models.py:358
 msgid "Participation of {} in event {}"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:363
+#: aleksis/apps/paweljong/models.py:387
 msgid "Social Sponsoring / Extra Donation"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:374
+#: aleksis/apps/paweljong/models.py:398
 msgid "Voucher / Granted discount"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:402 aleksis/apps/paweljong/views.py:392
+#: aleksis/apps/paweljong/models.py:428 aleksis/apps/paweljong/views.py:422
 msgid "Event registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:403
+#: aleksis/apps/paweljong/models.py:429
 msgid "Event registrations"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:412
+#: aleksis/apps/paweljong/models.py:439
 msgid "Related event"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:413
+#: aleksis/apps/paweljong/models.py:443
 msgid "Checked person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:414
+#: aleksis/apps/paweljong/models.py:449
 msgid "Checked by person"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:419
+#: aleksis/apps/paweljong/models.py:456
 msgid "Date and time of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:420
+#: aleksis/apps/paweljong/models.py:458
 msgid "Latitude of check"
 msgstr ""
 
-#: aleksis/apps/paweljong/models.py:421
+#: aleksis/apps/paweljong/models.py:461
 msgid "Longitude of check"
 msgstr ""
 
 #: aleksis/apps/paweljong/preferences.py:10
 msgid "Paweljong"
 msgstr ""
 
@@ -646,15 +648,15 @@
 #: aleksis/apps/paweljong/tables.py:20 aleksis/apps/paweljong/tables.py:21
 #: aleksis/apps/paweljong/tables.py:54 aleksis/apps/paweljong/tables.py:84
 #: aleksis/apps/paweljong/tables.py:85 aleksis/apps/paweljong/tables.py:102
 #: aleksis/apps/paweljong/tables.py:103 aleksis/apps/paweljong/tables.py:116
 #: aleksis/apps/paweljong/tables.py:117 aleksis/apps/paweljong/tables.py:136
 #: aleksis/apps/paweljong/tables.py:137
 #: aleksis/apps/paweljong/templates/paweljong/event/detail.html:24
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:25
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:26
 msgid "Edit"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:27 aleksis/apps/paweljong/tables.py:28
 msgid "Public page"
 msgstr ""
 
@@ -669,29 +671,29 @@
 
 #: aleksis/apps/paweljong/tables.py:45
 msgid "Code"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:50 aleksis/apps/paweljong/tables.py:51
 #: aleksis/apps/paweljong/tables.py:122 aleksis/apps/paweljong/tables.py:123
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:42
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:43
 msgid "Delete"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:57
 #: aleksis/apps/paweljong/templates/paweljong/print/manage.html:11
 msgid "Print"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:72
 msgid "View registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:78 aleksis/apps/paweljong/tables.py:79
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:29
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:30
 msgid "Check in"
 msgstr ""
 
 #: aleksis/apps/paweljong/tables.py:157 aleksis/apps/paweljong/tables.py:158
 msgid "Add persons"
 msgstr ""
 
@@ -784,26 +786,36 @@
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event/edit.html:5
 msgid "Edit event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:58
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:60
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:101
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:111
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:109
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:119
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:57
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:67
 msgid "Register now"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/full.html:62
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:77
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
 msgid "Not available"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:5
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:6
+msgid "Events"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event/list.html:10
+#: aleksis/apps/paweljong/views.py:789
+msgid "Upcoming events"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/event/list.html:17
 msgid "Events you've taken part"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:6
 #: aleksis/apps/paweljong/templates/paweljong/event/manage.html:7
 msgid "Manage events"
@@ -836,94 +848,102 @@
 "           "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:28
 msgid ""
 "\n"
 "           We ask parents to not fill in the registration on behalf of their child.\n"
+"           It is a requirement that our participants can freely access and\n"
+"           manage their accounts and inboxes, and that parents allow their\n"
+"           children to keep their passwords secret. We kindly ask parents to\n"
+"           get in contact with us if they have questions about this rule,\n"
+"           and of course, we encourage all children to show everything they\n"
+"           do not understand or have questions about to their parents.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:33
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:39
 msgid ""
 "\n"
 "           Every participant needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
-"           parents. Of course, we will always send important information to your parents as well.\n"
+"           parents. Of course, we will always send important information to your parents as\n"
+"           well, and of course you should always talk to your parents if you\n"
+"           have questions or concerns while reading your e-mail.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:40
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:23
 msgid ""
 "\n"
 "           If you do not have a personal e-mail address yet, and do not want or cannot register\n"
 "           one with one of the \"big\" providers (keep in mind that Google, Outlook, etc. are\n"
 "           allowed from 16 years only, and often collect and analyse your private mail), you can\n"
 "           register an e-mail address with us.\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:48
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:56
 msgid ""
 "\n"
 "           If you already have a user account with Teckids, do not register a new one. Login\n"
 "           with your existing username and password. If you have forgotten your password, please\n"
-"           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).\n"
+"           send us an e-mail (please do this yourself, with the help of your parents, if needed).\n"
 "           "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:62
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:70
 msgid "I already have an account"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:67
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:75
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:37
 msgid "I have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:72
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:80
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:42
 msgid "I don't have a personal email address"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:85
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:93
 msgid ""
 "\n"
 "         If you already have a Teckids account, please login here. If you forgot your password,\n"
 "         or have problems logging in, please send us an e-mail.\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:90
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:98
 msgid "Login"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:94
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:102
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:50
 msgid ""
 "\n"
 "         You can now choose a personal e-mail address hosted on our servers.\n"
 "         For information about receiving mails, see <a\n"
 "         href=\"https://leopard.institute/pages/services.html\">\n"
 "         https://leopard.institute/pages/services.html</a>\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:105
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:113
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:61
 msgid ""
 "\n"
 "         You will be asked for your existing, personal e-mail address. Please remember\n"
 "         that you should not use an address owned by your parents. If you do not have\n"
 "         a personal e-mail address, please choose the respective option instead!\n"
 "         "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:116
+#: aleksis/apps/paweljong/templates/paweljong/event/register_start.html:124
 msgid ""
 "\n"
 "         Registration is no longer possible.\n"
 "         "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html:34
@@ -938,68 +958,72 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html:5
 msgid "Edit registration"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:35
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:36
 msgid "Retract"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:49
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:50
 msgid "Notification"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:56
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:57
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:16
 #: aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html:200
 msgid "Invoice"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:63
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:64
 msgid "Edit person"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:142
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:143
 msgid "Retraction information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:149
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:150
 msgid "True"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:164
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:165
 msgid "Registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:197
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:198
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:45
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:96
 msgid "Accepted"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:231
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:232
 msgid "No checked in yet."
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:240
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:241
 msgid "Invoice details"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:246
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:247
 msgid "Billing information"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:278
-#: aleksis/apps/paweljong/views.py:421
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:279
+#: aleksis/apps/paweljong/views.py:451
 msgid "Payment"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:316
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:310
+msgid "Mark payed"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/paweljong/event_registration/full.html:323
 msgid "Guardians / Parents "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:4
 #: aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html:5
 msgid "Send notification"
 msgstr ""
@@ -1111,14 +1135,18 @@
 msgid "To use the voucher, register for the event "
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/print/voucher.html:21
 msgid "here"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/register_start.html:4
+msgid "Register"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/register_start.html:16
 msgid ""
 "\n"
 "           Every person needs a personal e-mail address. This address must be one\n"
 "           that you, the participating child, check and read yourself, not one owned by your\n"
 "           parents.\n"
 "           "
@@ -1131,14 +1159,19 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:4
 #: aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html:5
 msgid "Edit registration state"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:6
+#: aleksis/apps/paweljong/templates/paweljong/registration_state/list.html:7
+msgid "Registration states"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:4
 #: aleksis/apps/paweljong/templates/paweljong/term/create.html:5
 #: aleksis/apps/paweljong/templates/paweljong/term/list.html:11
 msgid "Create term"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/term/edit.html:4
@@ -1161,14 +1194,45 @@
 msgid "Filter vouchers"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/paweljong/voucher/list.html:23
 msgid "Selected vouchers"
 msgstr ""
 
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:3
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:35
+msgid "New account"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:6
+#, python-format
+msgid "New account: %(person)s"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:11
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:41
+msgid "Username"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:22
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:51
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
+msgid "Guardian"
+msgstr ""
+
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:30
+#: aleksis/apps/paweljong/templates/templated_email/account_registered.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
+#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
+#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
+msgid "Your AlekSIS team"
+msgstr ""
+
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:3
 msgid "New event"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:6
 #: aleksis/apps/paweljong/templates/templated_email/event_created.email:31
 #, python-format
@@ -1190,35 +1254,23 @@
 #, python-format
 msgid ""
 "\n"
 "        The event was created by %(sender)s\n"
 "    "
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:26
-#: aleksis/apps/paweljong/templates/templated_email/event_created.email:61
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:49
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:103
-msgid "Your AlekSIS team"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:3
 msgid "New registration"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:6
 #, python-format
 msgid "New registration: %(event)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:23
-#: aleksis/apps/paweljong/templates/templated_email/event_registered.email:72
-msgid "Guardian"
-msgstr ""
-
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:29
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:78
 msgid "Financial details"
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:33
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:82
@@ -1226,152 +1278,156 @@
 msgstr ""
 
 #: aleksis/apps/paweljong/templates/templated_email/event_registered.email:54
 #, python-format
 msgid "New registration: %(registration)s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:68 aleksis/apps/paweljong/views.py:80
+#: aleksis/apps/paweljong/views.py:77 aleksis/apps/paweljong/views.py:89
 msgid "The event has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:152
+#: aleksis/apps/paweljong/views.py:161
 msgid "The event registration has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:164
+#: aleksis/apps/paweljong/views.py:173
 msgid "The event registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:185
+#: aleksis/apps/paweljong/views.py:194
 msgid "The registration has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:230
+#: aleksis/apps/paweljong/views.py:239
 msgid "The registration has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:242
+#: aleksis/apps/paweljong/views.py:251
 msgid "The voucher has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:254
+#: aleksis/apps/paweljong/views.py:263
 msgid "The voucher has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:264
+#: aleksis/apps/paweljong/views.py:273
 msgid "The voucher has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:383
+#: aleksis/apps/paweljong/views.py:413
 msgid "Create e-mail address"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:385
+#: aleksis/apps/paweljong/views.py:415
 msgid "All participants need a personal e-mail address, which they check and read temselves. We offer the possibility to register an e-mail address on our secure servers, made for young users. For information about receiving mails, see: <a href='https://leopard.institute/pages/services.html'>https://leopard.institute/pages/services.html</a>."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:394
+#: aleksis/apps/paweljong/views.py:424
 msgid "First, please enter some basic information about yourself, and check whether all information is correct."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:398
+#: aleksis/apps/paweljong/views.py:428
 msgid "Contact information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:400
+#: aleksis/apps/paweljong/views.py:430
 msgid "Tell us how we can contact you. You will receive information about the event by e-mail. Please use your personal e-mail address where you will read mails yourself, not an address of your parents. We will always send all important information to your parents as well, and you will enter their e-mail address on the next page."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:407
+#: aleksis/apps/paweljong/views.py:437
 msgid "Legal guardians / parents"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:409
+#: aleksis/apps/paweljong/views.py:439
 msgid "Tell us how we can reach your parents or other legal guardians. This should be the person who was present when you registered for the event (which is now). If you want to add another parent, please tell us later as a comment."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:415
+#: aleksis/apps/paweljong/views.py:445
 msgid "Additional registration information"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:417
+#: aleksis/apps/paweljong/views.py:447
 msgid "Please answer the following questions as precisely as you can, so we can make sure your event attendance will be organised as wel las possible."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:423
+#: aleksis/apps/paweljong/views.py:453
 msgid "Please decide with your parents how you want to pay. In this step, you only select a payment method. The real payment will be done in a separate step, after the registration is complete."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:428
+#: aleksis/apps/paweljong/views.py:458
 msgid "Consent"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:430
+#: aleksis/apps/paweljong/views.py:460
 msgid "Lastly, please read the terms and conditions carefully, together with your parents. After that, you will need to confirm that you agree with everything yourself, and that your parents also agree."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:528 aleksis/apps/paweljong/views.py:638
+#: aleksis/apps/paweljong/views.py:567 aleksis/apps/paweljong/views.py:677
 msgid "You entered an invalid voucher code!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:664
+#: aleksis/apps/paweljong/views.py:703
 msgid "You have successfully registered for the event. Please give us up to two days to process your registration. You will then receive an email from us."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:671
+#: aleksis/apps/paweljong/views.py:710
 msgid "You registered for an event"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:672
+#: aleksis/apps/paweljong/views.py:711
 #, python-format
 msgid "You registered for the event %s"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:729 aleksis/apps/paweljong/views.py:880
+#: aleksis/apps/paweljong/views.py:770 aleksis/apps/paweljong/views.py:921
 msgid "The term has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:741 aleksis/apps/paweljong/views.py:892
+#: aleksis/apps/paweljong/views.py:782 aleksis/apps/paweljong/views.py:933
 msgid "The term has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:757
+#: aleksis/apps/paweljong/views.py:798
 msgid "Announcement feed of all upcoming events"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:798
+#: aleksis/apps/paweljong/views.py:839
 msgid "The info mailing has been created."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:810
+#: aleksis/apps/paweljong/views.py:851
 msgid "The info mailing has been saved."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:820
+#: aleksis/apps/paweljong/views.py:861
 msgid "The info mailing has been deleted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:906
+#: aleksis/apps/paweljong/views.py:947
 msgid "Registration successfully retracted."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:964
+#: aleksis/apps/paweljong/views.py:1005
 #, python-brace-format
 msgid "Person {person} added successfully!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:966
+#: aleksis/apps/paweljong/views.py:1007
 msgid "Person does not exist!"
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:993
+#: aleksis/apps/paweljong/views.py:1037
 msgid "The provided username is not linked to a person."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1003
+#: aleksis/apps/paweljong/views.py:1049
 msgid "{} successfully checked for {}."
 msgstr ""
 
-#: aleksis/apps/paweljong/views.py:1032
+#: aleksis/apps/paweljong/views.py:1085
 msgid "Successfully checked in."
 msgstr ""
+
+#: aleksis/apps/paweljong/views.py:1106
+msgid "Successfully marked as payed!"
+msgstr ""
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0001_initial.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0006_unique_constraints.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0006_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0007_terms.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0007_terms.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0009_remove_feedback.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0009_remove_feedback.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0013_info_mailings.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0013_info_mailings.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0015_registrationstate.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0015_registrationstate.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0019_retractions.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0019_retractions.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0020_check_in.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0020_check_in.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/migrations/0021_checkpoint.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0021_checkpoint.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/models.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 from decimal import Decimal
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.urls import reverse
 from django.utils.text import slugify
@@ -47,28 +47,40 @@
     reply_to = models.EmailField(verbose_name=_("Request replies to"), blank=True)
 
     active = models.BooleanField(verbose_name=_("Mailing is active"), default=False)
 
     sender = models.EmailField(verbose_name=_("Sender"), blank=True)
     send_to_person = models.BooleanField(verbose_name=_("Send to registered person"), default=True)
     send_to_guardians = models.BooleanField(verbose_name=_("Send to guardians"), default=False)
+    send_to_retracted = models.BooleanField(
+        verbose_name=_("Send to participants who retracted"), default=False
+    )
+    send_to_not_checked_in = models.BooleanField(
+        verbose_name=_("Send to participants who did not check in"), default=True
+    )
 
     def __str__(self) -> str:
         return self.subject
 
     @classmethod
     def get_active_mailings(cls):
         return cls.objects.filter(active=True)
 
     def send(self):
         for event in self.events.all():
             through = EventInfoMailingThrough.objects.get(info_mailing=self, event=event)
             sent_to = through.sent_to.all()
 
-            for registration in event.registrations.filter(retracted=False):
+            filter_args = {}
+            if not self.send_to_retracted:
+                filter_args["retracted"] = False
+            if not self.send_to_not_checked_in:
+                filter_args["checked_in"] = True
+
+            for registration in event.registrations.filter(**filter_args):
                 if registration.person in sent_to:
                     continue
 
                 subject = self.subject.format(
                     event=event, registration=registration, person=registration.person
                 )
                 body = self.text.format(
@@ -175,14 +187,22 @@
         if self.date_registration:
             return self.date_registration >= now
         return self.date_event > now
 
     def get_absolute_url(self):
         return reverse("event_by_name", kwargs={"slug": self.slug})
 
+    def individual_cost(self, request=None):
+        if request and request.user.is_authenticated and Voucher.objects.filter(event=self, person=request.user.person, used=False).exists():
+            voucher = Voucher.objects.get(event=self, person=request.user.person, used=False)
+            individual_cost = (100 - voucher.discount) * self.cost / 100
+            return individual_cost
+        else:
+            return self.cost
+
     @property
     def booked_percentage(self):
         return self.linked_group.members.count() / self.max_participants * 100
 
     @property
     def members_persons(self):
         return self.linked_group.members.all()
@@ -285,14 +305,17 @@
 
     retracted = models.BooleanField(verbose_name=_("Retracted"), default=False)
     retracted_date = models.DateField(verbose_name=_("Retracted at"), null=True, blank=True)
 
     checked_in = models.BooleanField(verbose_name=_("Checked in"), default=False)
     checked_in_date = models.DateTimeField(verbose_name=_("Checked in at"), null=True, blank=True)
 
+    cost = models.IntegerField(verbose_name=_("Cost in €"), null=True, blank=True)
+
+
     def mark_checked_in(self):
         if not self.checked_in:
             self.checked_in = True
             self.checked_in_date = now()
             self.save()
         else:
             raise ValidationError(_("Person is already checked in!"))
@@ -326,14 +349,15 @@
             for_content_type=ContentType.objects.get_for_model(self),
             for_object_id=self.pk,
             defaults={
                 "group": group,
                 "number": f"HNF-{self.date_registered.strftime('%Y-%m')}-{self.id}",
                 "currency": "EUR",
                 "total": self._get_total_amount()[0],
+                "due_date": now().date() + timedelta(days=7),
                 "tax": self._get_total_amount()[1],
                 "description": _("Participation of {} in event {}").format(
                     self.person.addressing_name, self.event.display_name
                 ),
                 "billing_first_name": self.person.first_name,
                 "billing_last_name": self.person.last_name,
                 "billing_address_1": f"{self.person.street} {self.person.housenumber}",
@@ -347,15 +371,15 @@
 
     def get_purchased_items(self):
         # FIXME Maybe do not hard-code the tax rate and currency
         # First, return main amount
         yield PurchasedItem(
             name=self.event.display_name,
             quantity=1,
-            price=Decimal(self.event.cost / 1.07),
+            price=Decimal(self.cost / 1.07),
             currency="EUR",
             sku="EVENT",
             tax_rate=7,
         )
 
         # If a dnoation was made, add it
         if self.donation:
@@ -369,15 +393,15 @@
             )
 
         # If a voucher was used, add it
         if self.voucher:
             yield PurchasedItem(
                 name=_("Voucher / Granted discount"),
                 quantity=1,
-                price=Decimal(-1 * self.voucher.discount * (self.event.cost / 1.07) / 100),
+                price=Decimal(-1 * self.voucher.discount * (self.cost / 1.07) / 100),
                 currency="EUR",
                 sku="DISCO",
                 tax_rate=7,
             )
 
     def _get_total_amount(self):
         total, total_tax = 0, 0
@@ -388,14 +412,16 @@
         return total, total_tax
 
     def __str__(self) -> str:
         return f"{self.event}, {self.person.first_name} {self.person.last_name}"
 
     def save(self, *args, **kwargs):
         self.event.sync_group_members()
+        if self.cost is None:
+            self.cost = self.event.cost
         super().save(*args, **kwargs)
 
     def delete(self, *args, **kwargs):
         self.event.sync_group_members()
         super().delete(*args, **kwargs)
 
     class Meta:
@@ -405,17 +431,32 @@
             models.UniqueConstraint(
                 fields=["person", "event"], name="unique_person_registration_per_event"
             )
         ]
 
 
 class Checkpoint(ExtensibleModel):
-    event = models.ForeignKey(Event, verbose_name=_("Related event"), related_name="checkpoints", on_delete=models.CASCADE)
-    person = models.ForeignKey(Person, verbose_name=_("Checked person"), related_name="event_checkpoints", on_delete=models.CASCADE)
-    checked_by = models.ForeignKey(Person, verbose_name=_("Checked by person"), related_name="event_checkpoints_created", on_delete=models.CASCADE)
-
+    event = models.ForeignKey(
+        Event, verbose_name=_("Related event"), related_name="checkpoints", on_delete=models.CASCADE
+    )
+    person = models.ForeignKey(
+        Person,
+        verbose_name=_("Checked person"),
+        related_name="event_checkpoints",
+        on_delete=models.CASCADE,
+    )
+    checked_by = models.ForeignKey(
+        Person,
+        verbose_name=_("Checked by person"),
+        related_name="event_checkpoints_created",
+        on_delete=models.CASCADE,
+    )
 
     comment = models.CharField(max_length=60, verbose_name=_("Comment"))
 
     timestamp = models.DateTimeField(verbose_name=_("Date and time of check"), auto_now_add=True)
-    lat = models.DecimalField(max_digits=10, decimal_places=8, verbose_name=_("Latitude of check"), blank=True, null=True)
-    lon = models.DecimalField(max_digits=11, decimal_places=8, verbose_name=_("Longitude of check"), blank=True, null=True)
+    lat = models.DecimalField(
+        max_digits=10, decimal_places=8, verbose_name=_("Latitude of check"), blank=True, null=True
+    )
+    lon = models.DecimalField(
+        max_digits=11, decimal_places=8, verbose_name=_("Longitude of check"), blank=True, null=True
+    )
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/predicates.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/predicates.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/preferences.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/preferences.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/rules.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,28 +55,28 @@
 
 # View events
 view_events_predicate = has_person & (
     has_global_perm("paweljong.view_event") | has_any_object("paweljong.view_event_rule", Event)
 )
 rules.add_perm("paweljong.view_events_rule", view_events_predicate)
 
-# Edit events
-change_events_predicate = has_person & (
-    has_global_perm("paweljong.change_event") | has_any_object("paweljong.change_event_rule", Event)
-)
-rules.add_perm("paweljong.change_events_rule", change_events_predicate)
-
 # Edit event
 change_event_predicate = has_person & (
     has_global_perm("paweljong.change_event")
     | has_object_perm("paweljong.change_event")
     | is_organiser
 )
 rules.add_perm("paweljong.change_event_rule", change_event_predicate)
 
+# Edit events
+change_events_predicate = has_person & (
+    has_global_perm("paweljong.change_event") | has_any_object("paweljong.change_event_rule", Event)
+)
+rules.add_perm("paweljong.change_events_rule", change_events_predicate)
+
 # Checkpoint
 checkpoint_predicate = change_event_predicate
 rules.add_perm("paweljong.event_checkpoint_rule", checkpoint_predicate)
 
 # View event
 view_event_predicate = (
     is_event_published | (has_person & is_organiser) | has_object_perm("paweljong.view_event")
@@ -249,7 +249,10 @@
 rules.add_perm("paweljong.view_menu", can_view_menu_predicate)
 
 can_retract_registration_predicate = has_person & (is_organiser)
 rules.add_perm("paweljong.can_retract_registration_rule", can_retract_registration_predicate)
 
 can_view_terms_predicate = has_person & (is_participant)
 rules.add_perm("paweljong.can_view_terms_rule", can_view_terms_predicate)
+
+can_mark_payment_as_payed_predicate = has_person & (is_organiser)
+rules.add_perm("paweljong.mark_payment_payed_rule", can_mark_payment_as_payed_predicate)
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/tables.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.template.loader import render_to_string
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 import django_tables2 as tables
 from django_tables2.utils import A
 
 
 class ManageEventsTable(tables.Table):
     class Meta:
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/account_wizard.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/account_wizard.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/create.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/detail.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     <p>
      {% if can_change_event_rule %}
       <a href="{% url 'edit_event_by_slug' event.slug %}" class="btn waves-effect waves-light">
         <i class="material-icons left iconify" data-icon="mdi:edit"></i>
         {% trans "Edit" %}
       </a>
      {% endif %}
-     {% if can_checkpoint %}
+     {% if can_checkpoint_rule %}
        <a href="{% url 'event_by_name_checkpoint' event.slug %}" class="btn waves-effect waves-light">
          <i class="material-icons left iconify" data-icon="mdi:access-point-check"></i>
          {% trans "Checkpoint" %}
        </a>
      {% endif %}
     </p>
 
@@ -46,15 +46,15 @@
             <td><i class="material-icons small">edit_calendar</i></td>
             <td colspan="2">{% trans "Registration open until" %}:</td>
             <td>{{ event.date_registration }}</td>
           </tr>
           <tr>
             <td><i class="material-icons small">money</i></td>
             <td colspan="2">{% trans "Participation fee (all inclusive)" %}</td>
-            <td>{{ event.cost }}</td>
+            <td>{{ individual_cost }}</td>
           </tr>
           <tr>
             <td><i class="material-icons small">group</i></td>
             <td colspan="2">{{ event.linked_group.members.count }}</td>
             <td>{% trans "of" %} {{ event.max_participants }}</td>
           </tr>
           <tr>
```

#### html2text {}

```diff
@@ -5,25 +5,25 @@
  {% endblock %} {% block content %}
 *** {{ event }} ***
 {% has_perm 'paweljong.change_event_rule' user event as can_change_event_rule
 %} {% has_perm 'paweljong.event_checkpoint_rule' user event as
 can_checkpoint_rule %}
 {% if can_change_event_rule %}
  {%_trans_"Edit"_%}
- {% endif %} {% if can_checkpoint %}
+ {% endif %} {% if can_checkpoint_rule %}
  {%_trans_"Checkpoint"_%}
  {% endif %}
 {{ event.description }}
 event         {{ event.date_event location_on        {{ event.place }}
               }}
                                                      {
 edit_calendar {% trans "Registration open until" %}: {
                                                      event.date_registration
                                                      }}
-money         {% trans "Participation fee (all       {{ event.cost }}
+money         {% trans "Participation fee (all       {{ individual_cost }}
               inclusive)" %}
                                                      {% trans "of" %} {
 group         {{ event.linked_group.members.count }} { event.max_participants
                                                      }}
                                                      {% for owner in
                                                      event.owners_persons.all
               {% trans "Owners" %}                   %}
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/edit.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/full.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/full.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
               <td><i class="material-icons small">edit_calendar</i></td>
               <td colspan="2">{% trans "Registration open until" %}:</td>
               <td>{{ event.date_registration }}</td>
             </tr>
             <tr>
               <td><i class="material-icons small">money</i></td>
               <td colspan="2">{% trans "Participation fee (all inclusive)" %}</td>
-              <td>{{ event.cost }}</td>
+              <td>{{ individual_cost }}</td>
             </tr>
             <tr>
               <td><i class="material-icons small">group</i></td>
               <td>{{ event.linked_group.members.count }}</td>
               <td colspan="2">{% trans "of" %} {{ event.max_participants }}</td>
             </tr>
             <tr>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
  {{ event.display_name }}
 {{ event.description }}
 event         {{ event.date_event }}           location_on {{ event.place }}
                                                            {
 edit_calendar {% trans "Registration open until" %}:       {
                                                            event.date_registration
                                                            }}
-money         {% trans "Participation fee (all inclusive)" {{ event.cost }}
+money         {% trans "Participation fee (all inclusive)" {{ individual_cost }}
               %}
               {
 group         {                                {% trans "of" %} {
               event.linked_group.members.count { event.max_participants }}
               }}
 {% if can_register and not is_authenticated %}
  event.slug %}">{% trans "Register now" %}
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/list.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/list.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/manage.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/manage.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_start.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_start.html`

 * *Files 16% similar despite different names*

```diff
@@ -20,39 +20,47 @@
            {% blocktrans %}
            Welcome to the registration for this event! Please make sure to fill in
            the registration yourself, as the child who wants to participate.
            You should fill in the registration together with a parent (or other legal
            guardian).
            {% endblocktrans %}
          </p>
-         <p>
+         <p class="important-info">
            {% blocktrans %}
            We ask parents to not fill in the registration on behalf of their child.
+           It is a requirement that our participants can freely access and
+           manage their accounts and inboxes, and that parents allow their
+           children to keep their passwords secret. We kindly ask parents to
+           get in contact with us if they have questions about this rule,
+           and of course, we encourage all children to show everything they
+           do not understand or have questions about to their parents.
            {% endblocktrans %}
          </p>
          <p>
            {% blocktrans %}
            Every participant needs a personal e-mail address. This address must be one
            that you, the participating child, check and read yourself, not one owned by your
-           parents. Of course, we will always send important information to your parents as well.
+           parents. Of course, we will always send important information to your parents as
+           well, and of course you should always talk to your parents if you
+           have questions or concerns while reading your e-mail.
            {% endblocktrans %}
          </p>
          <p>
            {% blocktrans %}
            If you do not have a personal e-mail address yet, and do not want or cannot register
            one with one of the "big" providers (keep in mind that Google, Outlook, etc. are
            allowed from 16 years only, and often collect and analyse your private mail), you can
            register an e-mail address with us.
            {% endblocktrans %}
          </p>
-         <p>
+         <p class="important-info">
            {% blocktrans %}
            If you already have a user account with Teckids, do not register a new one. Login
            with your existing username and password. If you have forgotten your password, please
-           send us an e-mail (pelase do this yourself, with the help of your parents, if needed).
+           send us an e-mail (please do this yourself, with the help of your parents, if needed).
            {% endblocktrans %}
          </p>
        </div>
      </div>
    </div>
    <div class="card-tabs">
      <ul class="tabs tabs-fixed-width">
```

#### html2text {}

```diff
@@ -4,27 +4,34 @@
  {% endblock %} {% block content %}
  {{ event.display_name }}
 {% blocktrans %} Welcome to the registration for this event! Please make sure
 to fill in the registration yourself, as the child who wants to participate.
 You should fill in the registration together with a parent (or other legal
 guardian). {% endblocktrans %}
 {% blocktrans %} We ask parents to not fill in the registration on behalf of
-their child. {% endblocktrans %}
+their child. It is a requirement that our participants can freely access and
+manage their accounts and inboxes, and that parents allow their children to
+keep their passwords secret. We kindly ask parents to get in contact with us if
+they have questions about this rule, and of course, we encourage all children
+to show everything they do not understand or have questions about to their
+parents. {% endblocktrans %}
 {% blocktrans %} Every participant needs a personal e-mail address. This
 address must be one that you, the participating child, check and read yourself,
 not one owned by your parents. Of course, we will always send important
-information to your parents as well. {% endblocktrans %}
+information to your parents as well, and of course you should always talk to
+your parents if you have questions or concerns while reading your e-mail. {%
+endblocktrans %}
 {% blocktrans %} If you do not have a personal e-mail address yet, and do not
 want or cannot register one with one of the "big" providers (keep in mind that
 Google, Outlook, etc. are allowed from 16 years only, and often collect and
 analyse your private mail), you can register an e-mail address with us. {%
 endblocktrans %}
 {% blocktrans %} If you already have a user account with Teckids, do not
 register a new one. Login with your existing username and password. If you have
-forgotten your password, please send us an e-mail (pelase do this yourself,
+forgotten your password, please send us an e-mail (please do this yourself,
 with the help of your parents, if needed). {% endblocktrans %}
     * {% if can_register %}
     * {%_trans_"I_already_have_an_account"_%}
     * {%_trans_"I_have_a_personal_email_address"_%}
     * {%_trans_"I_don't_have_a_personal_email_address"_%}
     * {% else %}
     * {%_trans_"Not_available"_%}
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event/terms.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/terms.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 {% block content %}
   <h4>{{ registration }} </h4>
 
   {% has_perm 'paweljong.manage_registration' user registration as can_manage_registration %}
   {% has_perm 'paweljong.delete_registration' user registration as can_delete_registration %}
   {% has_perm 'paweljong.send_notification_mail' user registration as can_send_notification %}
   {% has_perm 'paweljong.can_retract_registration_rule' user registration as can_retract_registration %}
+  {% has_perm 'paweljong.mark_payment_payed_rule' user registration as can_mark_registration_payed %}
   {% has_perm 'tezor.view_invoice_rule' user registration as can_view_invoice %}
   {% has_perm 'core.edit_person_rule' user person as can_change_person %}
 
   {% if can_manage_registration or can_manage_registration_preferences or can_delete_registration or can_send_notification or can_retract_registration %}
     <p>
       {% if can_manage_registration %}
         <a href="{% url 'edit_registration_by_pk' registration.pk %}" class="btn waves-effect waves-light">
@@ -278,19 +279,15 @@
             <span class="card-title">{% trans "Payment" %}</span>
             <table class="highlight">
               <tr>
                 <td>
                   <i class="material-icons iconify" data-icon="{{ invoice.get_variant_icon }}"></i>
                 </td>
                 <td>
-                  <select name="variant" disabled>
-                    {% for choice in invoice.get_variant_choices %}
-                      <option value="{{ choice.0 }}" {% if invoice.variant == choice.0 %}selected{% endif %}>{{ choice.1 }}</option>
-                    {% endfor %}
-                  </select>
+                  {{ invoice.variant }}
                 </td>
               </tr>
               <tr>
                 <td>
                   <i class="material-icons iconify" data-icon="{{ invoice.get_status_icon }}"></i>
                 </td>
                 <td>
@@ -301,14 +298,24 @@
                 <td>
                   <i class="material-icons iconify" data-icon="mdi:calendar-end"></i>
                 </td>
                 <td>
                   {{ invoice.due_date }}
                 </td>
               </tr>
+              {% if can_mark_registration_payed and not invoice.status == "confirmed" %}
+              <tr>
+                <td>
+                  <a href="{% url 'pay_registration_by_pk' registration.pk %}" class="btn waves-effect waves-light">
+                    <i class="material-icons left iconify" data-icon="mdi:account-check"></i>
+                    {% trans "Mark payed" %}
+                  </a>
+                </td>
+              </tr>
+              {% endif %}
             </table>
           </div>
         </div>
       </div>
     </div>
   </div>
```

#### html2text {}

```diff
@@ -4,19 +4,20 @@
 content %}
 *** {{ registration }} ***
 {% has_perm 'paweljong.manage_registration' user registration as
 can_manage_registration %} {% has_perm 'paweljong.delete_registration' user
 registration as can_delete_registration %} {% has_perm
 'paweljong.send_notification_mail' user registration as can_send_notification
 %} {% has_perm 'paweljong.can_retract_registration_rule' user registration as
-can_retract_registration %} {% has_perm 'tezor.view_invoice_rule' user
-registration as can_view_invoice %} {% has_perm 'core.edit_person_rule' user
-person as can_change_person %} {% if can_manage_registration or
-can_manage_registration_preferences or can_delete_registration or
-can_send_notification or can_retract_registration %}
+can_retract_registration %} {% has_perm 'paweljong.mark_payment_payed_rule'
+user registration as can_mark_registration_payed %} {% has_perm
+'tezor.view_invoice_rule' user registration as can_view_invoice %} {% has_perm
+'core.edit_person_rule' user person as can_change_person %} {% if
+can_manage_registration or can_manage_registration_preferences or
+can_delete_registration or can_send_notification or can_retract_registration %}
 {% if can_manage_registration %}
  {%_trans_"Edit"_%}
 
  {%_trans_"Check_in"_%}
  {% endif %} {% if can_retract_registration %}
  {%_trans_"Retract"_%}
  {% endif %} {% if can_delete_registration %}
@@ -70,19 +71,18 @@
 ** {% trans "Invoice details" %} **
 {% trans "Billing information" %}
  {{ invoice.billing_first_name }} {{invoice.billing_last_name }}
  {{ invoice.billing_address_1 }} {{ invoice.billing_address_2 }}
  {{ invoice.billing_postcode }} {{ invoice.billing_city}}
  {{_invoice.billing_email_}}
 {% trans "Payment" %}
- {% for choice in invoice.get_variant_choices %}
- % if invoice.variant == choice.0 %}selected{% endif %}>{{ choice.1 }}
- {% endfor %}
- {{ invoice.get_status_display }}
- {{ invoice.due_date }}
+                          {{ invoice.variant }}
+                          {{ invoice.get_status_display }}
+                          {{ invoice.due_date }}
+ {%_trans_"Mark_payed"_%}
 {% if registration.person.guardians.all %}
 ** {% trans "Guardians / Parents "%} **
 {% for person in registration.person.guardians.all %}
         {                   {
  person { person.first_name {                      {{ person.last_name
         }}                  person.additional_name }}
                             }}
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/corona.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/corona.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/print/voucher.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/voucher.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/register_start.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register_start.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/create.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/create.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/paweljong/voucher/list.html` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/list.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_created.email` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_created.email`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/templates/templated_email/event_registered.email` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_registered.email`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/urls.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,131 +32,140 @@
 ]
 
 account_conditions = {
     "email": views.is_email_needed,
 }
 
 urlpatterns = [
-    path("event/<slug:slug>/edit", views.EditEventView.as_view(), name="edit_event_by_slug"),
-    path("event/<slug:slug>/terms", views.ViewTerms.as_view(), name="view_event_terms_by_slug"),
+    path("event/<slug:slug>/edit/", views.EditEventView.as_view(), name="edit_event_by_slug"),
+    path("event/<slug:slug>/terms/", views.ViewTerms.as_view(), name="view_event_terms_by_slug"),
     path(
-        "event/<slug:slug>/register",
+        "event/<slug:slug>/register/",
         views.RegisterEventWizardView.as_view(register_forms, condition_dict=condition_dict),
         name="register_event_by_slug",
     ),
     path(
-        "group_persons/<int:pk>/add",
+        "group_persons/<int:pk>/add/",
         views.PersonGroupView.as_view(),
         name="add_persons_to_group",
     ),
-    path("event/<slug:slug>", views.EventFullView.as_view(), name="event_by_name"),
-    path("event/<slug:slug>/detail", views.EventDetailView.as_view(), name="event_detail_by_name"),
-    path("event/<slug:slug>/checkpoint", views.EventCheckpointView.as_view(), name="event_by_name_checkpoint"),
+    path("event/<slug:slug>/", views.EventFullView.as_view(), name="event_by_name"),
+    path("event/<slug:slug>/detail/", views.EventDetailView.as_view(), name="event_detail_by_name"),
     path(
-        "event/<slug:slug>/start",
+        "event/<slug:slug>/checkpoint/",
+        views.EventCheckpointView.as_view(),
+        name="event_by_name_checkpoint",
+    ),
+    path(
+        "event/<slug:slug>/start/",
         views.RegisterEventStart.as_view(),
         name="register_event_by_slug_start",
     ),
-    path("misc/set_email_needed/<slug:slug>", views.set_email_needed, name="set_email_needed"),
+    path("misc/set_email_needed/<slug:slug>/", views.set_email_needed, name="set_email_needed"),
     path("misc/set_email_needed/", views.set_email_needed, name="set_email_needed_no_slug"),
     path(
-        "account/register/start",
+        "account/register/start/",
         views.AccountRegisterStart.as_view(),
         name="register_account_start",
     ),
     path(
-        "account/register",
+        "account/register/",
         views.AccountRegisterWizardView.as_view(account_forms, condition_dict=account_conditions),
         name="register_account",
     ),
-    path("events/feed", views.UpcomingEventsRSSFeed(), name="upcoming_events_rss_feed"),
-    path("events/create", views.CreateEventView.as_view(), name="create_event"),
-    path("events/manage", views.manage_events, name="manage_events"),
-    path("vouchers/create", views.VoucherCreateView.as_view(), name="create_vouchers"),
+    path("events/feed/", views.UpcomingEventsRSSFeed(), name="upcoming_events_rss_feed"),
+    path("events/create/", views.CreateEventView.as_view(), name="create_event"),
+    path("events/manage/", views.manage_events, name="manage_events"),
+    path("vouchers/create/", views.VoucherCreateView.as_view(), name="create_vouchers"),
     path(
-        "vouchers/<int:pk>/delete", views.VoucherDeleteView.as_view(), name="delete_voucher_by_pk"
+        "vouchers/<int:pk>/delete/", views.VoucherDeleteView.as_view(), name="delete_voucher_by_pk"
     ),
-    path("vouchers/<int:pk>/edit", views.VoucherEditView.as_view(), name="edit_voucher_by_pk"),
-    path("vouchers/<int:pk>/print", views.print_voucher, name="print_voucher_by_pk"),
+    path("vouchers/<int:pk>/edit/", views.VoucherEditView.as_view(), name="edit_voucher_by_pk"),
+    path("vouchers/<int:pk>/print/", views.print_voucher, name="print_voucher_by_pk"),
     path("vouchers/", views.vouchers, name="vouchers"),
-    path("event/lists/generate", views.generate_lists, name="generate_lists"),
+    path("event/lists/generate/", views.generate_lists, name="generate_lists"),
     path(
-        "event/registrations/<int:pk>/check_in",
+        "event/registrations/<int:pk>/check_in/",
         views.CheckInRegistration.as_view(),
         name="check_in_registration_by_pk",
     ),
     path(
-        "event/registrations/<int:pk>/retract",
+        "event/registrations/<int:pk>/pay/",
+        views.MarkRegistrationPayed.as_view(),
+        name="pay_registration_by_pk",
+    ),
+    path(
+        "event/registrations/<int:pk>/retract/",
         views.RetractRegistration.as_view(),
         name="retract_registration_by_pk",
     ),
     path(
-        "event/registrations/<int:pk>",
+        "event/registrations/<int:pk>/",
         views.EventRegistrationDetailView.as_view(),
         name="registration_by_pk",
     ),
     path(
-        "event/registrations/<int:pk>/edit",
+        "event/registrations/<int:pk>/edit/",
         views.EventRegistrationEditView.as_view(),
         name="edit_registration_by_pk",
     ),
     path(
-        "event/registrations/<int:pk>/delete",
+        "event/registrations/<int:pk>/delete/",
         views.EventRegistrationDeleteView.as_view(),
         name="delete_registration_by_pk",
     ),
     path(
-        "event/registrations/<int:pk>/notification",
+        "event/registrations/<int:pk>/notification/",
         views.SendMailFromRegistration.as_view(),
         name="registration_notification_by_pk",
     ),
     path(
-        "event/terms/list",
+        "event/terms/list/",
         views.TermListView.as_view(),
         name="terms",
     ),
     path(
-        "event/terms/create",
+        "event/terms/create/",
         views.TermCreateView.as_view(),
         name="create_term",
     ),
     path(
-        "event/terms/<int:pk>/edit",
+        "event/terms/<int:pk>/edit/",
         views.TermEditView.as_view(),
         name="edit_term_by_pk",
     ),
     path(
-        "event/registrations/states/list",
+        "event/registrations/states/list/",
         views.RegistrationStateListView.as_view(),
         name="registration_states",
     ),
     path(
-        "event/registrations/states/create",
+        "event/registrations/states/create/",
         views.RegistrationStateCreateView.as_view(),
         name="create_registration_state",
     ),
     path(
-        "event/registrations/states/<int:pk>/edit",
+        "event/registrations/states/<int:pk>/edit/",
         views.RegistrationStateEditView.as_view(),
         name="edit_registration_state_by_pk",
     ),
     path(
-        "info_mailings/list",
+        "info_mailings/list/",
         views.InfoMailingListView.as_view(),
         name="info_mailings",
     ),
     path(
-        "info_mailings/create",
+        "info_mailings/create/",
         views.InfoMailingCreateView.as_view(),
         name="create_info_mailing",
     ),
     path(
-        "info_mailings/<int:pk>/edit",
+        "info_mailings/<int:pk>/edit/",
         views.InfoMailingEditView.as_view(),
         name="edit_info_mailing_by_pk",
     ),
     path(
-        "info_mailings/<int:pk>/delete",
+        "info_mailings/<int:pk>/delete/",
         views.InfoMailingDeleteView.as_view(),
         name="delete_info_mailing_by_pk",
     ),
 ]
```

### Comparing `AlekSIS-App-Paweljong-1.9/aleksis/apps/paweljong/views.py` & `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from django.http import HttpRequest, HttpResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse, reverse_lazy
 from django.utils import timezone
 from django.utils.decorators import method_decorator
 from django.utils.http import urlencode
 from django.utils.text import slugify
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.decorators.cache import never_cache
 from django.views.generic import FormView, TemplateView, View
 from django.views.generic.detail import DetailView
 
 import reversion
 from django_tables2 import RequestConfig
 from django_tables2.views import SingleTableView
 from formtools.wizard.views import SessionWizardView
 from reversion.views import RevisionMixin
 from rules.contrib.views import PermissionRequiredMixin, permission_required
 from templated_email import send_templated_mail
 
 from aleksis.apps.postbuero.models import MailAddress
+from aleksis.apps.tezor.models.invoice import Invoice
 from aleksis.core.mixins import AdvancedCreateView, AdvancedDeleteView, AdvancedEditView
 from aleksis.core.models import Activity, Group, Person
 from aleksis.core.util import messages
 from aleksis.core.util.core_helpers import get_site_preferences, objectgetter_optional
 
 from .filters import EventFilter, EventRegistrationFilter, VoucherFilter
 from .forms import (
@@ -39,15 +40,23 @@
     EditVoucherForm,
     EventCheckpointForm,
     GenerateListForm,
     PersonGroupFormPerson,
     RegistrationNotificationForm,
     RegistrationStatesForm,
 )
-from .models import Checkpoint, Event, EventRegistration, InfoMailing, RegistrationState, Terms, Voucher
+from .models import (
+    Checkpoint,
+    Event,
+    EventRegistration,
+    InfoMailing,
+    RegistrationState,
+    Terms,
+    Voucher,
+)
 from .tables import (
     AdditionalFieldsTable,
     ChildGroupsTable,
     EventRegistrationsTable,
     InfoMailingsTable,
     ManageEventsTable,
     RegistrationStatesTable,
@@ -83,15 +92,15 @@
 @permission_required("paweljong.view_events_rule")
 def manage_events(request: HttpRequest) -> HttpResponse:
     """List view listing all registrations."""
     context = {}
 
     # Get all registrations
     now = timezone.datetime.today()
-    events = Event.objects.filter(date_event__gte=now)
+    events = Event.objects.all()
 
     # Get filter
     events_filter = EventFilter(request.GET, queryset=events)
     context["events_filter"] = events_filter
 
     # Build table
     events_table = ManageEventsTable(events_filter.qs)
@@ -144,27 +153,27 @@
 class EventRegistrationCreateView(PermissionRequiredMixin, AdvancedCreateView):
     """Create view for event registrations."""
 
     model = EventRegistration
     form_class = EditEventRegistrationForm
     permission_required = "paweljong.create_registration_rule"
     template_name = "paweljong/event_registration/create.html"
-    success_url = reverse_lazy("registrations")
+    success_url = reverse_lazy("manage_events")
     success_message = _("The event registration has been created.")
 
 
 @method_decorator(never_cache, name="dispatch")
 class EventRegistrationEditView(PermissionRequiredMixin, AdvancedEditView):
     """Edit view for event registrations."""
 
     model = EventRegistration
     form_class = EditEventRegistrationForm
     permission_required = "paweljong.change_registration_rule"
     template_name = "paweljong/event_registration/edit.html"
-    success_url = reverse_lazy("registrations")
+    success_url = reverse_lazy("manage_events")
     success_message = _("The event registration has been saved.")
 
 
 @permission_required(
     "paweljong.change_registration_rule",
     fn=objectgetter_optional(EventRegistration, None, False),
 )
@@ -222,15 +231,15 @@
 
 class EventRegistrationDeleteView(PermissionRequiredMixin, AdvancedDeleteView):
     """Delete view for registrations."""
 
     model = EventRegistration
     permission_required = "paweljong.delete_eventregistration_rule"
     template_name = "core/pages/delete.html"
-    success_url = reverse_lazy("registrations")
+    success_url = reverse_lazy("manage_events")
     success_message = _("The registration has been deleted.")
 
 
 @method_decorator(never_cache, name="dispatch")
 class VoucherCreateView(PermissionRequiredMixin, AdvancedCreateView):
     """Create view for vouchers."""
 
@@ -330,18 +339,20 @@
                     }
                 )
 
         return self.initial_dict.get(step, initial)
 
     def done(self, form_list, **kwargs):
 
+        context = {}
         cleaned_data_email = self.get_cleaned_data_for_step("email")
         cleaned_data_register = self.get_cleaned_data_for_step("register")
 
         # Create email address
+        _email = None
         if cleaned_data_email:
             _email = MailAddress.objects.create(
                 local_part=cleaned_data_email["local_part"],
                 domain=cleaned_data_email["domain"],
             )
 
         # Create user
@@ -361,14 +372,33 @@
                 "email": cleaned_data_register["email"],
                 "first_name": cleaned_data_register["first_name"],
                 "last_name": cleaned_data_register["last_name"],
                 "date_of_birth": cleaned_data_register["date_of_birth"],
             },
         )
 
+        context["person"] = person
+
+        send_templated_mail(
+            template_name="account_registered",
+            from_email=get_site_preferences()["mail__address"],
+            recipient_list=['root@teckids.org'],
+            headers={
+                "reply_to": [
+                    person.email,
+                ],
+                "X-Zammad-Customer-Email": person.email,
+            },
+            context=context,
+        )
+
+        if _email:
+            _email.person = person
+            _email.save()
+
         return redirect("index")
 
 
 class RegisterEventWizardView(SessionWizardView):
     template_name = "paweljong/event/register_wizard.html"
     file_storage = settings.DEFAULT_FILE_STORAGE
 
@@ -501,35 +531,44 @@
                             "first_name": cleaned_data_register["first_name"],
                             "last_name": cleaned_data_register["last_name"],
                             "email": cleaned_data_register["email"],
                             "date_of_birth": cleaned_data_register["date_of_birth"],
                         }
                     )
 
+        if step == "financial":
+            if getattr(self.request.user, "person", None):
+                vouchers = Voucher.objects.filter(
+                    person=self.request.user.person, event__slug=self.kwargs["slug"], used=False
+                )
+                if vouchers:
+                    initial.update({"voucher_code": vouchers.first().code})
+
         return self.initial_dict.get(step, initial)
 
     def done(self, form_list, **kwargs):
 
         event = Event.objects.get(slug=self.kwargs["slug"])
         cleaned_data_email = self.get_cleaned_data_for_step("email")
         cleaned_data_contact_details = self.get_cleaned_data_for_step("contact_details")
         cleaned_data_guardians = self.get_cleaned_data_for_step("guardians")
         cleaned_data_register = self.get_cleaned_data_for_step("register")
         cleaned_data_additional = self.get_cleaned_data_for_step("additional")
         cleaned_data_financial = self.get_cleaned_data_for_step("financial")
         cleaned_data_consent = self.get_cleaned_data_for_step("consent")
 
         if cleaned_data_financial["voucher_code"]:
-            vouchers = Voucher.objects.filter(
-                person=person, event=event, used=False, code=cleaned_data_financial["voucher_code"]
-            )
-            if vouchers:
-                voucher = vouchers.first()
-            else:
-                messages.error(self.request, _("You entered an invalid voucher code!"))
+            if getattr(self.request.user, "person", None):
+                vouchers = Voucher.objects.filter(
+                    person=self.request.user.person, event=event, used=False, code=cleaned_data_financial["voucher_code"]
+                )
+                if vouchers:
+                    voucher = vouchers.first()
+                else:
+                    messages.error(self.request, _("You entered an invalid voucher code!"))
 
         # Create email address
         if cleaned_data_email:
             _email = MailAddress.objects.create(
                 local_part=cleaned_data_email["local_part"],
                 domain=cleaned_data_email["domain"],
             )
@@ -686,14 +725,16 @@
     permission_required = "paweljong.view_event_rule"
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         context["can_register"] = context["event"].can_register(request=self.request)
         context["is_authenticated"] = self.request.user.is_authenticated
+        context["individual_cost"] = context["event"].individual_cost(request=self.request)
+
         return context
 
 
 class RegisterEventStart(PermissionRequiredMixin, DetailView):
 
     model = Event
     slug_field = "slug"
@@ -821,15 +862,15 @@
 
 
 class SendMailFromRegistration(PermissionRequiredMixin, FormView):
 
     template_name = "paweljong/event_registration/notification.html"
     permission_required = "paweljong.send_notification_mail_rule"
     form_class = RegistrationNotificationForm
-    success_url = reverse_lazy("registrations")
+    success_url = reverse_lazy("manage_events")
 
     def form_valid(self, form):
 
         registration = EventRegistration.objects.get(id=self.kwargs["pk"])
 
         context = {}
         recipient_list = []
@@ -970,17 +1011,20 @@
     def get_success_url(self):
         return reverse("add_persons_to_group", kwargs={"pk": self.kwargs["pk"]})
 
 
 class EventCheckpointView(PermissionRequiredMixin, FormView):
 
     template_name = "paweljong/event/checkpoint.html"
-    permission_required = "paweljong.can_checkpoint"
+    permission_required = "paweljong.event_checkpoint_rule"
     form_class = EventCheckpointForm
 
+    def get_object(self):
+        return Event.objects.get(slug=self.kwargs["slug"])
+
     def get_initial(self):
         initial = super().get_initial() or {}
         if "comment" in self.request.GET:
             initial["comment"] = self.request.GET.get("comment")
         return initial
 
     def form_valid(self, form):
@@ -996,20 +1040,29 @@
         checkpoint.comment = form.cleaned_data["comment"]
         checkpoint.timestamp = timezone.now()
         if form.cleaned_data["use_latlon"]:
             checkpoint.lat = form.cleaned_data["lat"]
             checkpoint.lon = form.cleaned_data["lon"]
 
         checkpoint.save()
-        messages.success(self.request, _("{} successfully checked for {}.").format(str(checkpoint.person), str(checkpoint.comment)))
+        messages.success(
+            self.request,
+            _("{} successfully checked for {}.").format(
+                str(checkpoint.person), str(checkpoint.comment)
+            ),
+        )
         self._comment = checkpoint.comment
         return super().form_valid(self)
 
     def get_success_url(self):
-        return reverse("event_by_name_checkpoint", kwargs={"slug": self.kwargs["slug"]}) + "?" + urlencode({"comment": self._comment})
+        return (
+            reverse("event_by_name_checkpoint", kwargs={"slug": self.kwargs["slug"]})
+            + "?"
+            + urlencode({"comment": self._comment})
+        )
 
 
 class ViewTerms(PermissionRequiredMixin, DetailView):
 
     context_object_name = "event"
     template_name = "paweljong/event/terms.html"
     permission_required = "paweljong.can_view_terms_rule"
@@ -1030,7 +1083,26 @@
         try:
             registration.mark_checked_in()
             messages.success(self.request, _("Successfully checked in."))
         except ValidationError:
             messages.error(self.request, _("Person is already checked in!"))
 
         return redirect("event_detail_by_name", slug=registration.event.slug)
+
+
+class MarkRegistrationPayed(PermissionRequiredMixin, View):
+
+    permission_required = "paweljong.mark_payment_payed_rule"
+
+    def get_object(self, *args, **kwargs):
+        registration = EventRegistration.objects.get(id=self.kwargs["pk"])
+        invoice = registration.get_invoice()
+        return invoice
+
+    def get(self, *args, **kwargs):
+        invoice = self.get_object()
+
+        invoice.status = "confirmed"
+        invoice.save()
+        messages.success(request, _("Successfully marked as payed!"))
+
+        return redirect("registration_by_pk", pk=invoice.for_object.pk)
```

### Comparing `AlekSIS-App-Paweljong-1.9/pyproject.toml` & `aleksis_app_paweljong-2.0.dev0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Paweljong"
-version = "1.9"
+version = "2.0.dev0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Paweljong (Camp/Event management)"
@@ -21,20 +21,20 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^2.8.1"
+aleksis-core = "^3.0b0"
 django-iban-field = "^0.8"
-django-formtools = "^2.3"
+django-formtools = "2.3"
 django-starfield = "^1.0"
-aleksis-app-postbuero = "1.0+20220218233830.a212f707"
-aleksis-app-tezor = "^1.0"
+aleksis-app-postbuero = { version = "2.0.1.dev0" , allow-prereleases = true }
+aleksis-app-tezor = {version = "2.0dev1", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 paweljong = "aleksis.apps.paweljong.apps:DefaultConfig"
```

### Comparing `AlekSIS-App-Paweljong-1.9/PKG-INFO` & `aleksis_app_paweljong-2.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: aleksis-app-paweljong
-Version: 1.9
+Version: 2.0.dev0
 Summary: AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 Home-page: https://hacknfun.camp
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
-Requires-Dist: aleksis-app-postbuero (==1.0+20220218233830.a212f707)
-Requires-Dist: aleksis-app-tezor (>=1.0,<2.0)
-Requires-Dist: aleksis-core (>=2.8.1,<3.0.0)
-Requires-Dist: django-formtools (>=2.3,<3.0)
+Requires-Dist: aleksis-app-postbuero (==2.0.1.dev0)
+Requires-Dist: aleksis-app-tezor (==2.0dev1)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
+Requires-Dist: django-formtools (==2.3)
 Requires-Dist: django-iban-field (>=0.8,<0.9)
 Requires-Dist: django-starfield (>=1.0,<2.0)
 Project-URL: Repository, https://edugit.org/Teckids/hacknfun/AlekSIS-App-Paweljong
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 ==================================================================================================
```

