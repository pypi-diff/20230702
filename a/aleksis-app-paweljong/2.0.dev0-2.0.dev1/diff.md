# Comparing `tmp/aleksis_app_paweljong-2.0.dev0.tar.gz` & `tmp/aleksis_app_paweljong-2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_paweljong-2.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_paweljong-2.0.dev1.tar", max compression
```

## Comparing `aleksis_app_paweljong-2.0.dev0.tar` & `aleksis_app_paweljong-2.0.dev1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     3513 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev0/README.rst
--rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/__init__.py
--rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/apps.py
--rw-r--r--   0        0        0     1253 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/data_checks.py
--rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/filters.py
--rw-r--r--   0        0        0    16277 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/forms.py
--rw-r--r--   0        0        0    12846 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/index.js
--rw-r--r--   0        0        0      563 2023-07-02 13:18:57.467867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47795 2023-07-02 13:33:45.628654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    31084 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    64927 2023-07-02 13:33:45.600654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47711 2023-07-02 13:33:45.608654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-06-07 21:25:48.599903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.584654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-06-07 21:25:48.603903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.572654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-06-07 21:25:48.599903 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 13:33:45.616654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8646 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0001_initial.py
--rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0002_event_website.py
--rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
--rw-r--r--   0        0        0      911 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
--rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
--rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
--rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0007_terms.py
--rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
--rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
--rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
--rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
--rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0012_event_slug.py
--rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0013_info_mailings.py
--rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
--rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0015_registrationstate.py
--rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
--rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
--rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
--rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0019_retractions.py
--rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0020_check_in.py
--rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0021_checkpoint.py
--rw-r--r--   0        0        0      681 2022-07-08 20:57:59.622407 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py
--rw-r--r--   0        0        0      452 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0023_eventregistration_cost.py
--rw-r--r--   0        0        0      430 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0024_add_cost_to_registration.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/__init__.py
--rw-r--r--   0        0        0    16558 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/models.py
--rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/predicates.py
--rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/preferences.py
--rw-r--r--   0        0        0     9079 2022-06-30 15:18:35.332204 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/rules.py
--rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/settings.py
--rw-r--r--   0        0        0     1076 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/css/paweljong.css
--rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
--rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
--rw-r--r--   0        0        0     4445 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tables.py
--rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tasks.py
--rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
--rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
--rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/create.html
--rw-r--r--   0        0        0     3557 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/detail.html
--rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/edit.html
--rw-r--r--   0        0        0     2480 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/full.html
--rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/list.html
--rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/manage.html
--rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
--rw-r--r--   0        0        0     5118 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
--rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
--rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
--rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/registered.html
--rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/terms.html
--rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
--rw-r--r--   0        0        0    13116 2022-06-28 20:06:29.947789 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
--rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
--rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
--rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
--rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
--rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
--rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/corona.html
--rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
--rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
--rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
--rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/manage.html
--rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
--rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register.html
--rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register_start.html
--rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
--rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
--rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
--rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
--rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/create.html
--rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/edit.html
--rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/term/list.html
--rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
--rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
--rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
--rw-r--r--   0        0        0     2272 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/account_registered.email
--rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_created.email
--rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_notification.email
--rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_registered.email
--rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
--rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templatetags/coerce.py
--rw-r--r--   0        0        0     5596 2023-07-02 13:18:57.471867 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/urls.py
--rw-r--r--   0        0        0    40215 2023-07-02 13:19:17.651886 aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/views.py
--rw-r--r--   0        0        0     1522 2023-07-02 13:39:36.044937 aleksis_app_paweljong-2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev0/setup.py
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3513 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev1/README.rst
+-rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/__init__.py
+-rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/apps.py
+-rw-r--r--   0        0        0     1253 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/data_checks.py
+-rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/filters.py
+-rw-r--r--   0        0        0    16277 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/forms.py
+-rw-r--r--   0        0        0    12884 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/frontend/index.js
+-rw-r--r--   0        0        0      563 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47795 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31014 2023-07-02 21:38:39.358049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    64927 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47711 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.358049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8628 2023-07-02 21:37:58.185924 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0001_initial.py
+-rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0002_event_website.py
+-rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
+-rw-r--r--   0        0        0      893 2023-07-02 21:37:58.185924 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
+-rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
+-rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
+-rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0007_terms.py
+-rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
+-rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
+-rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
+-rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
+-rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0012_event_slug.py
+-rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0013_info_mailings.py
+-rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
+-rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0015_registrationstate.py
+-rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
+-rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
+-rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
+-rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0019_retractions.py
+-rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0020_check_in.py
+-rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0021_checkpoint.py
+-rw-r--r--   0        0        0      681 2022-07-08 20:57:59.622407 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py
+-rw-r--r--   0        0        0      452 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0023_eventregistration_cost.py
+-rw-r--r--   0        0        0      430 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0024_add_cost_to_registration.py
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/__init__.py
+-rw-r--r--   0        0        0    16558 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/models.py
+-rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/predicates.py
+-rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/preferences.py
+-rw-r--r--   0        0        0     9079 2022-06-30 15:18:35.332204 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/rules.py
+-rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/settings.py
+-rw-r--r--   0        0        0     1076 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/static/css/paweljong.css
+-rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
+-rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
+-rw-r--r--   0        0        0     4445 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/tables.py
+-rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/tasks.py
+-rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
+-rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
+-rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/create.html
+-rw-r--r--   0        0        0     3557 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/detail.html
+-rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/edit.html
+-rw-r--r--   0        0        0     2480 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/full.html
+-rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/list.html
+-rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/manage.html
+-rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
+-rw-r--r--   0        0        0     5118 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
+-rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
+-rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
+-rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/registered.html
+-rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/terms.html
+-rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
+-rw-r--r--   0        0        0    13116 2022-06-28 20:06:29.947789 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
+-rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
+-rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
+-rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
+-rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
+-rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
+-rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/corona.html
+-rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
+-rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
+-rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
+-rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/manage.html
+-rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
+-rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/register.html
+-rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/register_start.html
+-rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
+-rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
+-rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
+-rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
+-rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/create.html
+-rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/edit.html
+-rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/list.html
+-rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
+-rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
+-rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
+-rw-r--r--   0        0        0     2272 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/account_registered.email
+-rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_created.email
+-rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_notification.email
+-rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_registered.email
+-rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
+-rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templatetags/coerce.py
+-rw-r--r--   0        0        0     5596 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/urls.py
+-rw-r--r--   0        0        0    40215 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/views.py
+-rw-r--r--   0        0        0     1523 2023-07-02 21:38:00.321931 aleksis_app_paweljong-2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev1/setup.py
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_paweljong-2.0.dev0/CHANGELOG.rst` & `aleksis_app_paweljong-2.0.dev1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/LICENCE.rst` & `aleksis_app_paweljong-2.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/README.rst` & `aleksis_app_paweljong-2.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/apps.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/data_checks.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/filters.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/forms.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/index.js` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/frontend/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,14 +4,15 @@
 } from "aleksis.core/routeValidators";
 
 export default {
     meta: {
         inMenu: true,
         titleKey: "paweljong.events.menu_title",
         icon: "mdi-calendar-text",
+        validators: [hasPersonValidator],
     },
     children: [{
         path: "event/:slug/edit/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "paweljong.editEventBySlug",
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
```

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/frontend/messages/en.json` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -519,17 +519,14 @@
 "Aus verschiedenen Gründen, z.B da wir aus rechtlichen Gründen die "
 "Geschlechtertrennung während der Nacht aufrechterhalten müssen, müssen wir "
 "wissen, ob du ein Junge oder ein Mädchen bist."
 
 msgid "Generate list"
 msgstr "Liste generieren"
 
-msgid "Generate participant list"
-msgstr "Teilnehmerlisten generieren"
-
 msgid "Group"
 msgstr "Gruppe"
 
 msgid "Guardian"
 msgstr "Erziehungsberechtigter"
 
 msgid "Guardian's email address"
```

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0001_initial.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.2.9 on 2021-11-30 15:23
 
 import django.contrib.sites.managers
 from django.db import migrations, models
 import django.db.models.deletion
-import django_iban.fields
+import localflavor.generic.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -81,15 +81,15 @@
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('extended_data', models.JSONField(default=dict, editable=False)),
                 ('date_registered', models.DateTimeField(auto_now_add=True, verbose_name='Registration date')),
                 ('comment', models.TextField(blank=True, default='', verbose_name='Comment / remarks')),
                 ('channel', models.CharField(blank=True, default='', max_length=255, verbose_name='Channel')),
                 ('donation', models.PositiveIntegerField(blank=True, null=True, verbose_name='Donation')),
                 ('accept_sepa', models.BooleanField(verbose_name='SEPA direct debit')),
-                ('iban', django_iban.fields.IBANField(enforce_database_constraint=True, max_length=34, null=True, verbose_name='IBAN (for SEPA direct debit)')),
+                ('iban', localflavor.generic.models.IBANField(max_length=34, null=True, verbose_name='IBAN (for SEPA direct debit)')),
                 ('accept_terms', models.BooleanField(verbose_name='Delcaration of consent by parents')),
                 ('accept_data', models.BooleanField(verbose_name='Declaration of consent data protection')),
                 ('accept_general_terms', models.BooleanField(verbose_name='Declatation of consent terms and condition')),
                 ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='paweljong.event', verbose_name='Event')),
                 ('person', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='core.person', verbose_name='Person')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
                 ('voucher', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='paweljong.voucher', verbose_name='Voucher')),
```

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 3.2.12 on 2022-02-16 18:52
 
 import ckeditor.fields
 from django.db import migrations
-import django_iban.fields
+import localflavor.generic.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('paweljong', '0003_alter_event_feedback_aspects'),
     ]
@@ -21,10 +21,10 @@
             name='information',
             field=ckeditor.fields.RichTextField(default='', verbose_name='Information about the event'),
             preserve_default=False,
         ),
         migrations.AlterField(
             model_name='eventregistration',
             name='iban',
-            field=django_iban.fields.IBANField(blank=True, enforce_database_constraint=True, max_length=34, null=True, verbose_name='IBAN (for SEPA direct debit)'),
+            field=localflavor.generic.models.IBANField(blank=True, max_length=34, null=True, verbose_name='IBAN (for SEPA direct debit)'),
         ),
     ]
```

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0006_unique_constraints.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0006_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0007_terms.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0007_terms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0009_remove_feedback.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0009_remove_feedback.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0013_info_mailings.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0013_info_mailings.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0015_registrationstate.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0015_registrationstate.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0019_retractions.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0019_retractions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0020_check_in.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0020_check_in.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0021_checkpoint.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0021_checkpoint.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/models.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/predicates.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/preferences.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/rules.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/css/paweljong.css` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/static/css/paweljong.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/tables.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/account_wizard.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/account_wizard.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/create.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/detail.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/edit.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/full.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/list.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/manage.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/manage.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_start.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_start.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event/terms.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/terms.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/corona.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/corona.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/print/voucher.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/voucher.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/register_start.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/register_start.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/create.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/paweljong/voucher/list.html` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/account_registered.email` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/account_registered.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_created.email` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_created.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/templates/templated_email/event_registered.email` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_registered.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/urls.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/aleksis/apps/paweljong/views.py` & `aleksis_app_paweljong-2.0.dev1/aleksis/apps/paweljong/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev0/pyproject.toml` & `aleksis_app_paweljong-2.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Paweljong"
-version = "2.0.dev0"
+version = "2.0.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Paweljong (Camp/Event management)"
@@ -22,15 +22,15 @@
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aleksis-core = "^3.0b0"
-django-iban-field = "^0.8"
+django-localflavor = "^3.0"
 django-formtools = "2.3"
 django-starfield = "^1.0"
 aleksis-app-postbuero = { version = "2.0.1.dev0" , allow-prereleases = true }
 aleksis-app-tezor = {version = "2.0dev1", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
```

### Comparing `aleksis_app_paweljong-2.0.dev0/setup.py` & `aleksis_app_paweljong-2.0.dev1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,23 @@
                             'templates/templated_email/*']}
 
 install_requires = \
 ['aleksis-app-postbuero==2.0.1.dev0',
  'aleksis-app-tezor==2.0dev1',
  'aleksis-core>=3.0b0,<4.0',
  'django-formtools==2.3',
- 'django-iban-field>=0.8,<0.9',
+ 'django-localflavor>=3.0,<4.0',
  'django-starfield>=1.0,<2.0']
 
 entry_points = \
 {'aleksis.app': ['paweljong = aleksis.apps.paweljong.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-paweljong',
-    'version': '2.0.dev0',
+    'version': '2.0.dev1',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Paweljong (Camp/Event management)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Paweljong (Camp/Event management)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2018, 2021, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://hacknfun.camp',
```

### Comparing `aleksis_app_paweljong-2.0.dev0/PKG-INFO` & `aleksis_app_paweljong-2.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-paweljong
-Version: 2.0.dev0
+Version: 2.0.dev1
 Summary: AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 Home-page: https://hacknfun.camp
 License: EUPL-1.2-or-later
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Requires-Dist: aleksis-app-postbuero (==2.0.1.dev0)
 Requires-Dist: aleksis-app-tezor (==2.0dev1)
 Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: django-formtools (==2.3)
-Requires-Dist: django-iban-field (>=0.8,<0.9)
+Requires-Dist: django-localflavor (>=3.0,<4.0)
 Requires-Dist: django-starfield (>=1.0,<2.0)
 Project-URL: Repository, https://edugit.org/Teckids/hacknfun/AlekSIS-App-Paweljong
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 ==================================================================================================
```

