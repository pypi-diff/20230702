# Comparing `tmp/django-data-browser-4.2.3.tar.gz` & `tmp/django-data-browser-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-browser-4.2.3.tar", last modified: Thu Jun 15 07:09:12 2023, max compression
+gzip compressed data, was "django-data-browser-4.2.4.tar", last modified: Sun Jul  2 18:09:50 2023, max compression
```

## Comparing `django-data-browser-4.2.3.tar` & `django-data-browser-4.2.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:12.012404 django-data-browser-4.2.3/
--rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.3/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.3/LICENSE
--rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0    62765 2023-06-15 07:09:12.011407 django-data-browser-4.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    61632 2023-06-15 07:08:40.000000 django-data-browser-4.2.3/README.rst
--rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.3/build.sh
--rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.3/build_fe.sh
--rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.3/build_whl.sh
--rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.3/clean.sh
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.878240 django-data-browser-4.2.3/data_browser/
--rw-rw-rw-   0        0        0       18 2023-06-15 07:08:36.000000 django-data-browser-4.2.3/data_browser/__init__.py
--rw-rw-rw-   0        0        0     2009 2023-06-08 21:24:56.000000 django-data-browser-4.2.3/data_browser/admin.py
--rw-rw-rw-   0        0        0     4818 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/api.py
--rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.3/data_browser/apps.py
--rw-rw-rw-   0        0        0     5599 2023-06-15 07:06:33.000000 django-data-browser-4.2.3/data_browser/common.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.880234 django-data-browser-4.2.3/data_browser/fe_build/
--rw-rw-rw-   0        0        0      374 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/asset-manifest.json
--rw-rw-rw-   0        0        0     2400 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/index.html
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.823222 django-data-browser-4.2.3/data_browser/fe_build/static/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.882229 django-data-browser-4.2.3/data_browser/fe_build/static/css/
--rw-rw-rw-   0        0        0     7170 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/static/css/main.a2cd42f2.css
--rw-rw-rw-   0        0        0    10320 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/static/css/main.a2cd42f2.css.map
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.887723 django-data-browser-4.2.3/data_browser/fe_build/static/js/
--rw-rw-rw-   0        0        0   328249 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js
--rw-rw-rw-   0        0        0     1447 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1220644 2023-06-15 07:09:03.000000 django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js.map
--rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.3/data_browser/format_csv.py
--rw-rw-rw-   0        0        0     5819 2023-05-28 08:26:29.000000 django-data-browser-4.2.3/data_browser/helpers.py
--rw-rw-rw-   0        0        0     2566 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/migration_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.906672 django-data-browser-4.2.3/data_browser/migrations/
--rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0002_auto_20200331_1842.py
--rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0003_remove_view_app.py
--rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0004_auto_20200501_0903.py
--rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0005_auto_20200516_1726.py
--rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0006_auto_20200531_1450.py
--rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0007_view_public_slug.py
--rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/migrations/0008_view_limit.py
--rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.3/data_browser/migrations/0009_migrate_saved_views.py
--rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/data_browser/migrations/0010_shared.py
--rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/data_browser/migrations/0011_folder.py
--rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.3/data_browser/migrations/0012_can_share.py
--rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.3/data_browser/migrations/__init__.py
--rw-rw-rw-   0        0        0     2646 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/models.py
--rw-rw-rw-   0        0        0    15460 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/orm_admin.py
--rw-rw-rw-   0        0        0     3923 2023-03-06 07:51:43.000000 django-data-browser-4.2.3/data_browser/orm_aggregates.py
--rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.3/data_browser/orm_debug.py
--rw-rw-rw-   0        0        0     8339 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/orm_fields.py
--rw-rw-rw-   0        0        0     4991 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/orm_functions.py
--rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.3/data_browser/orm_lookups.py
--rw-rw-rw-   0        0        0     9234 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/orm_results.py
--rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.3/data_browser/orm_types.py
--rw-rw-rw-   0        0        0     9969 2023-06-04 16:30:52.000000 django-data-browser-4.2.3/data_browser/query.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.824220 django-data-browser-4.2.3/data_browser/templates/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.907670 django-data-browser-4.2.3/data_browser/templates/data_browser/
--rw-rw-rw-   0        0        0     2400 2023-06-15 07:09:04.000000 django-data-browser-4.2.3/data_browser/templates/data_browser/index.html
--rw-rw-rw-   0        0        0    16949 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/data_browser/types.py
--rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.3/data_browser/urls.py
--rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.3/data_browser/util.py
--rw-rw-rw-   0        0        0    12967 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/data_browser/views.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.914651 django-data-browser-4.2.3/data_browser/web_root/
--rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/apple-touch-icon.png
--rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/favicon-16x16.png
--rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/favicon-32x32.png
--rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.3/data_browser/web_root/favicon.ico
--rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/data_browser/web_root/site.webmanifest
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.927125 django-data-browser-4.2.3/django_data_browser.egg-info/
--rw-rw-rw-   0        0        0    62765 2023-06-15 07:09:11.000000 django-data-browser-4.2.3/django_data_browser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3438 2023-06-15 07:09:11.000000 django-data-browser-4.2.3/django_data_browser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:09:11.000000 django-data-browser-4.2.3/django_data_browser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-15 07:09:11.000000 django-data-browser-4.2.3/django_data_browser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 07:09:11.000000 django-data-browser-4.2.3/django_data_browser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.932111 django-data-browser-4.2.3/frontend/
--rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.3/frontend/README.md
--rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/frontend/package-lock.json
--rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.3/frontend/package.json
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.933109 django-data-browser-4.2.3/frontend/public/
--rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.3/frontend/public/index.html
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.964026 django-data-browser-4.2.3/frontend/src/
--rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/frontend/src/App.js
--rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.3/frontend/src/App.scss
--rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.3/frontend/src/App.test.js
--rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/frontend/src/Config.js
--rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.3/frontend/src/ContextMenu.js
--rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/frontend/src/CurrentSavedView.js
--rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.3/frontend/src/HomePage.js
--rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.3/frontend/src/Query.js
--rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.3/frontend/src/Query.test.js
--rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.3/frontend/src/QueryPage.js
--rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.3/frontend/src/Results.js
--rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.3/frontend/src/SavedViewPage.js
--rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.3/frontend/src/Tooltip.js
--rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.3/frontend/src/Util.js
--rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.3/frontend/src/WindowDimensions.js
--rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.3/frontend/src/index.js
--rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.3/frontend/src/index.scss
--rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.3/frontend/src/logo.svg
--rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.3/frontend/src/setupTests.js
--rw-rw-rw-   0        0        0     2837 2023-05-01 18:51:44.000000 django-data-browser-4.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.3/requirements.txt
--rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.3/screenshot.png
--rw-rw-rw-   0        0        0       42 2023-06-15 07:09:12.012404 django-data-browser-4.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.3/setup.py
--rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.3/structure.svg
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.981978 django-data-browser-4.2.3/tests/
--rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.984486 django-data-browser-4.2.3/tests/array/
--rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.3/tests/array/__init__.py
--rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.3/tests/array/models.py
--rw-rw-rw-   0        0        0     2600 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:11.995450 django-data-browser-4.2.3/tests/core/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.3/tests/core/__init__.py
--rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.3/tests/core/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:12.000436 django-data-browser-4.2.3/tests/core/migrations/
--rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.3/tests/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.3/tests/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.3/tests/core/models.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:12.003428 django-data-browser-4.2.3/tests/json/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.3/tests/json/__init__.py
--rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.3/tests/json/models.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:09:12.009413 django-data-browser-4.2.3/tests/snapshots/
--rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.3/tests/snapshots/__init__.py
--rw-rw-rw-   0        0        0   439282 2023-05-21 15:04:07.000000 django-data-browser-4.2.3/tests/snapshots/snap_test_views.py
--rw-rw-rw-   0        0        0     6618 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_admin.py
--rw-rw-rw-   0        0        0    20582 2023-06-04 21:17:05.000000 django-data-browser-4.2.3/tests/test_api.py
--rw-rw-rw-   0        0        0     7227 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_array_field.py
--rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.3/tests/test_common.py
--rw-rw-rw-   0        0        0     3744 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_helpers.py
--rw-rw-rw-   0        0        0     6156 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_json_field.py
--rw-rw-rw-   0        0        0     4472 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_migrations.py
--rw-rw-rw-   0        0        0     1392 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_models.py
--rw-rw-rw-   0        0        0    34997 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_orm.py
--rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.3/tests/test_orm_debug.py
--rw-rw-rw-   0        0        0    25645 2023-05-21 16:31:25.000000 django-data-browser-4.2.3/tests/test_query.py
--rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.3/tests/test_tests.py
--rw-rw-rw-   0        0        0    18706 2023-06-08 07:10:28.000000 django-data-browser-4.2.3/tests/test_views.py
--rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.3/tests/urls.py
--rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.3/tests/util.py
--rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.445522 django-data-browser-4.2.4/
+-rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.4/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.4/LICENSE
+-rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    65961 2023-07-02 18:09:50.443529 django-data-browser-4.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    64745 2023-07-02 18:09:04.000000 django-data-browser-4.2.4/README.rst
+-rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.4/build.sh
+-rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.4/build_fe.sh
+-rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.4/build_whl.sh
+-rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.4/clean.sh
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.281941 django-data-browser-4.2.4/data_browser/
+-rw-rw-rw-   0        0        0       18 2023-07-02 18:09:11.000000 django-data-browser-4.2.4/data_browser/__init__.py
+-rw-rw-rw-   0        0        0     2009 2023-06-08 21:24:56.000000 django-data-browser-4.2.4/data_browser/admin.py
+-rw-rw-rw-   0        0        0     4818 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/api.py
+-rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.4/data_browser/apps.py
+-rw-rw-rw-   0        0        0     5599 2023-06-15 07:06:33.000000 django-data-browser-4.2.4/data_browser/common.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.283935 django-data-browser-4.2.4/data_browser/fe_build/
+-rw-rw-rw-   0        0        0      374 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2400 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.215101 django-data-browser-4.2.4/data_browser/fe_build/static/
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.289437 django-data-browser-4.2.4/data_browser/fe_build/static/css/
+-rw-rw-rw-   0        0        0     7170 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css
+-rw-rw-rw-   0        0        0    10320 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css.map
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.294417 django-data-browser-4.2.4/data_browser/fe_build/static/js/
+-rw-rw-rw-   0        0        0   328249 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js
+-rw-rw-rw-   0        0        0     1447 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1220644 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.map
+-rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.4/data_browser/format_csv.py
+-rw-rw-rw-   0        0        0     5819 2023-05-28 08:26:29.000000 django-data-browser-4.2.4/data_browser/helpers.py
+-rw-rw-rw-   0        0        0     2566 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/migration_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.314871 django-data-browser-4.2.4/data_browser/migrations/
+-rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0002_auto_20200331_1842.py
+-rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0003_remove_view_app.py
+-rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0004_auto_20200501_0903.py
+-rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0005_auto_20200516_1726.py
+-rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0006_auto_20200531_1450.py
+-rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0007_view_public_slug.py
+-rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/data_browser/migrations/0008_view_limit.py
+-rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.4/data_browser/migrations/0009_migrate_saved_views.py
+-rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/migrations/0010_shared.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/migrations/0011_folder.py
+-rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.4/data_browser/migrations/0012_can_share.py
+-rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.4/data_browser/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2646 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/models.py
+-rw-rw-rw-   0        0        0    15460 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/orm_admin.py
+-rw-rw-rw-   0        0        0     3482 2023-07-01 15:54:32.000000 django-data-browser-4.2.4/data_browser/orm_aggregates.py
+-rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.4/data_browser/orm_debug.py
+-rw-rw-rw-   0        0        0     8339 2023-07-01 15:18:54.000000 django-data-browser-4.2.4/data_browser/orm_fields.py
+-rw-rw-rw-   0        0        0     4885 2023-07-01 15:59:41.000000 django-data-browser-4.2.4/data_browser/orm_functions.py
+-rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.4/data_browser/orm_lookups.py
+-rw-rw-rw-   0        0        0     9234 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/orm_results.py
+-rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/data_browser/orm_types.py
+-rw-rw-rw-   0        0        0     9969 2023-06-04 16:30:52.000000 django-data-browser-4.2.4/data_browser/query.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.215101 django-data-browser-4.2.4/data_browser/templates/
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.314871 django-data-browser-4.2.4/data_browser/templates/data_browser/
+-rw-rw-rw-   0        0        0     2400 2023-07-02 18:09:39.000000 django-data-browser-4.2.4/data_browser/templates/data_browser/index.html
+-rw-rw-rw-   0        0        0    17004 2023-07-01 14:24:41.000000 django-data-browser-4.2.4/data_browser/types.py
+-rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.4/data_browser/urls.py
+-rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.4/data_browser/util.py
+-rw-rw-rw-   0        0        0    12967 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/data_browser/views.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.330830 django-data-browser-4.2.4/data_browser/web_root/
+-rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon-16x16.png
+-rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.4/data_browser/web_root/favicon.ico
+-rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/data_browser/web_root/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.344792 django-data-browser-4.2.4/django_data_browser.egg-info/
+-rw-rw-rw-   0        0        0    65961 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3438 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 18:09:50.000000 django-data-browser-4.2.4/django_data_browser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.349779 django-data-browser-4.2.4/frontend/
+-rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/README.md
+-rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/package-lock.json
+-rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.4/frontend/package.json
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.349779 django-data-browser-4.2.4/frontend/public/
+-rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.4/frontend/public/index.html
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.395656 django-data-browser-4.2.4/frontend/src/
+-rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/App.js
+-rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.4/frontend/src/App.scss
+-rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/App.test.js
+-rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/Config.js
+-rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.4/frontend/src/ContextMenu.js
+-rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/CurrentSavedView.js
+-rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.4/frontend/src/HomePage.js
+-rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.4/frontend/src/Query.js
+-rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/frontend/src/Query.test.js
+-rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.4/frontend/src/QueryPage.js
+-rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.4/frontend/src/Results.js
+-rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.4/frontend/src/SavedViewPage.js
+-rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.4/frontend/src/Tooltip.js
+-rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.4/frontend/src/Util.js
+-rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.4/frontend/src/WindowDimensions.js
+-rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.4/frontend/src/index.js
+-rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/index.scss
+-rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/logo.svg
+-rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.4/frontend/src/setupTests.js
+-rw-rw-rw-   0        0        0     2864 2023-07-01 15:58:55.000000 django-data-browser-4.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.4/requirements.txt
+-rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.4/screenshot.png
+-rw-rw-rw-   0        0        0       42 2023-07-02 18:09:50.445522 django-data-browser-4.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/setup.py
+-rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/structure.svg
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.422584 django-data-browser-4.2.4/tests/
+-rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.427570 django-data-browser-4.2.4/tests/array/
+-rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.4/tests/array/__init__.py
+-rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.4/tests/array/models.py
+-rw-rw-rw-   0        0        0     2600 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.430562 django-data-browser-4.2.4/tests/core/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.4/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.4/tests/core/admin.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.432557 django-data-browser-4.2.4/tests/core/migrations/
+-rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.4/tests/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.4/tests/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.4/tests/core/models.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.433554 django-data-browser-4.2.4/tests/json/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.4/tests/json/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tests/json/models.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:09:50.438541 django-data-browser-4.2.4/tests/snapshots/
+-rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.4/tests/snapshots/__init__.py
+-rw-rw-rw-   0        0        0   439282 2023-07-01 13:49:30.000000 django-data-browser-4.2.4/tests/snapshots/snap_test_views.py
+-rw-rw-rw-   0        0        0     6618 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_admin.py
+-rw-rw-rw-   0        0        0    20582 2023-06-04 21:17:05.000000 django-data-browser-4.2.4/tests/test_api.py
+-rw-rw-rw-   0        0        0     7227 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_array_field.py
+-rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.4/tests/test_common.py
+-rw-rw-rw-   0        0        0     3744 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     6156 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_json_field.py
+-rw-rw-rw-   0        0        0     4472 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_migrations.py
+-rw-rw-rw-   0        0        0     1392 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_models.py
+-rw-rw-rw-   0        0        0    35257 2023-07-01 07:55:19.000000 django-data-browser-4.2.4/tests/test_orm.py
+-rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tests/test_orm_debug.py
+-rw-rw-rw-   0        0        0    25645 2023-05-21 16:31:25.000000 django-data-browser-4.2.4/tests/test_query.py
+-rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.4/tests/test_tests.py
+-rw-rw-rw-   0        0        0    18706 2023-06-08 07:10:28.000000 django-data-browser-4.2.4/tests/test_views.py
+-rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.4/tests/urls.py
+-rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.4/tests/util.py
+-rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.4/tox.ini
```

### Comparing `django-data-browser-4.2.3/.pre-commit-config.yaml` & `django-data-browser-4.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/CONTRIBUTING.rst` & `django-data-browser-4.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/LICENSE` & `django-data-browser-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/MANIFEST.in` & `django-data-browser-4.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/PKG-INFO` & `django-data-browser-4.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.3
+Version: 4.2.4
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -338,14 +338,94 @@
 You can override the ``data_browser/index.html`` template per `Djangoâ€™s template overriding docs <https://docs.djangoproject.com/en/stable/howto/overriding-templates/#extending-an-overridden-template>`__, and replace the ``extrahead`` block.
 (Ensure ``"data_browser"`` is after your app in ``INSTALLED_APPS``.)
 
 This will let you inject custom CSS and stylesheets.
 
 However note that because of how the normal CSS is injected any custom CSS will be before the normal CSS so you will need to use more specific selectors or ``!important``.
 
+
+Custom functions and aggregations
+---------------------------------
+
+It is possible to register additional functions and aggregations with the Data Browser, including custom ones.
+
+Types
+^^^^^
+
+Functions and Aggregations are attached to the Data Browsers core types, these are in ``data_browser.types``.
+
+Functions
+^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The function registry is in ``data_browser.orm_functions.TYPE_FUNCTIONS`` this has type ``dict[BaseType, dict[str, data_browser.orm_functions.Func]]``. It is safe to insert new entries into this at runtime.
+
+For example to add the MD5 function to string fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models.functions import MD5
+    from data_browser.types import StringType
+    from data_browser.orm_functions import Func, TYPE_FUNCTIONS
+
+    TYPE_FUNCTIONS[StringType]["md5"] = Func(MD5, StringType)
+
+Aggregates
+^^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The aggregate registry is in ``data_browser.orm_aggregates.TYPE_AGGREGATES`` this has type ``dict[BaseType, dict[str, data_browser.orm_aggregates.Agg]]``. It is safe to insert new entries into this at runtime.
+
+For example to add a count that does not apply distinct to number fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models import Count
+    from data_browser.types import NumberType
+    from data_browser.orm_aggregates import Agg, TYPE_AGGREGATES
+
+    TYPE_AGGREGATES[NumberType]["full_count"] = Agg(
+        lambda x: Count(x, distinct=False), NumberType
+    )
+
+Custom SQL example
+^^^^^^^^^^^^^^^^^^
+
+For a larger example imagine you wanted to use Postgres's ``percentile_cont`` functionality to add a ``p95`` aggregate to duration fields, perhaps for some kind of application performance monitoring usecase.
+
+First we need to explain ``percentile_cont`` to Django.
+
+.. code-block:: python
+
+    from django.db.models import Aggregate
+
+    class Percentile(Aggregate):
+        arity = 1
+        function = "percentile_cont"
+        template = "%(function)s(%(percentile)s) WITHIN GROUP (ORDER BY %(expressions)s)"
+        name = "Percentile"
+
+        def __init__(self, percentile, expressions, **extra):
+            super().__init__(expressions, percentile=percentile, **extra)
+
+Then we need to tell the Data Browser we want ``p95`` on duration fields.
+
+.. code-block:: python
+
+    from data_browser.orm_aggregates import TYPE_AGGREGATES, Agg
+    from data_browser.types import DurationType
+
+    TYPE_AGGREGATES[DurationType]["p95"] = Agg(
+        lambda x: Percentile(0.95, x), DurationType
+    )
+
+
+
 Version numbers
 ---------------
 
 The Data Browser uses the standard ``Major.Minor.Patch`` version numbering scheme.
 
 Patch versions may include bug fixes and minor features.
 
@@ -365,14 +445,17 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
+|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
```

### Comparing `django-data-browser-4.2.3/README.rst` & `django-data-browser-4.2.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -324,14 +324,94 @@
 You can override the ``data_browser/index.html`` template per `Django’s template overriding docs <https://docs.djangoproject.com/en/stable/howto/overriding-templates/#extending-an-overridden-template>`__, and replace the ``extrahead`` block.
 (Ensure ``"data_browser"`` is after your app in ``INSTALLED_APPS``.)
 
 This will let you inject custom CSS and stylesheets.
 
 However note that because of how the normal CSS is injected any custom CSS will be before the normal CSS so you will need to use more specific selectors or ``!important``.
 
+
+Custom functions and aggregations
+---------------------------------
+
+It is possible to register additional functions and aggregations with the Data Browser, including custom ones.
+
+Types
+^^^^^
+
+Functions and Aggregations are attached to the Data Browsers core types, these are in ``data_browser.types``.
+
+Functions
+^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The function registry is in ``data_browser.orm_functions.TYPE_FUNCTIONS`` this has type ``dict[BaseType, dict[str, data_browser.orm_functions.Func]]``. It is safe to insert new entries into this at runtime.
+
+For example to add the MD5 function to string fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models.functions import MD5
+    from data_browser.types import StringType
+    from data_browser.orm_functions import Func, TYPE_FUNCTIONS
+
+    TYPE_FUNCTIONS[StringType]["md5"] = Func(MD5, StringType)
+
+Aggregates
+^^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The aggregate registry is in ``data_browser.orm_aggregates.TYPE_AGGREGATES`` this has type ``dict[BaseType, dict[str, data_browser.orm_aggregates.Agg]]``. It is safe to insert new entries into this at runtime.
+
+For example to add a count that does not apply distinct to number fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models import Count
+    from data_browser.types import NumberType
+    from data_browser.orm_aggregates import Agg, TYPE_AGGREGATES
+
+    TYPE_AGGREGATES[NumberType]["full_count"] = Agg(
+        lambda x: Count(x, distinct=False), NumberType
+    )
+
+Custom SQL example
+^^^^^^^^^^^^^^^^^^
+
+For a larger example imagine you wanted to use Postgres's ``percentile_cont`` functionality to add a ``p95`` aggregate to duration fields, perhaps for some kind of application performance monitoring usecase.
+
+First we need to explain ``percentile_cont`` to Django.
+
+.. code-block:: python
+
+    from django.db.models import Aggregate
+
+    class Percentile(Aggregate):
+        arity = 1
+        function = "percentile_cont"
+        template = "%(function)s(%(percentile)s) WITHIN GROUP (ORDER BY %(expressions)s)"
+        name = "Percentile"
+
+        def __init__(self, percentile, expressions, **extra):
+            super().__init__(expressions, percentile=percentile, **extra)
+
+Then we need to tell the Data Browser we want ``p95`` on duration fields.
+
+.. code-block:: python
+
+    from data_browser.orm_aggregates import TYPE_AGGREGATES, Agg
+    from data_browser.types import DurationType
+
+    TYPE_AGGREGATES[DurationType]["p95"] = Agg(
+        lambda x: Percentile(0.95, x), DurationType
+    )
+
+
+
 Version numbers
 ---------------
 
 The Data Browser uses the standard ``Major.Minor.Patch`` version numbering scheme.
 
 Patch versions may include bug fixes and minor features.
 
@@ -351,14 +431,17 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
+|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
```

### Comparing `django-data-browser-4.2.3/data_browser/admin.py` & `django-data-browser-4.2.4/data_browser/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/api.py` & `django-data-browser-4.2.4/data_browser/api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/common.py` & `django-data-browser-4.2.4/data_browser/common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/index.html` & `django-data-browser-4.2.4/data_browser/fe_build/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/static/css/main.a2cd42f2.css` & `django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/static/css/main.a2cd42f2.css.map` & `django-data-browser-4.2.4/data_browser/fe_build/static/css/main.a2cd42f2.css.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js` & `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt` & `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/fe_build/static/js/main.c57e8af0.js.map` & `django-data-browser-4.2.4/data_browser/fe_build/static/js/main.c57e8af0.js.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/format_csv.py` & `django-data-browser-4.2.4/data_browser/format_csv.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/helpers.py` & `django-data-browser-4.2.4/data_browser/helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/migration_helpers.py` & `django-data-browser-4.2.4/data_browser/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/migrations/0001_initial.py` & `django-data-browser-4.2.4/data_browser/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/migrations/0002_auto_20200331_1842.py` & `django-data-browser-4.2.4/data_browser/migrations/0002_auto_20200331_1842.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/migrations/0006_auto_20200531_1450.py` & `django-data-browser-4.2.4/data_browser/migrations/0006_auto_20200531_1450.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/migrations/0012_can_share.py` & `django-data-browser-4.2.4/data_browser/migrations/0012_can_share.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/models.py` & `django-data-browser-4.2.4/data_browser/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_admin.py` & `django-data-browser-4.2.4/data_browser/orm_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_debug.py` & `django-data-browser-4.2.4/data_browser/orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_fields.py` & `django-data-browser-4.2.4/data_browser/orm_fields.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_lookups.py` & `django-data-browser-4.2.4/data_browser/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_results.py` & `django-data-browser-4.2.4/data_browser/orm_results.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/orm_types.py` & `django-data-browser-4.2.4/data_browser/orm_types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/query.py` & `django-data-browser-4.2.4/data_browser/query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/templates/data_browser/index.html` & `django-data-browser-4.2.4/data_browser/templates/data_browser/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/types.py` & `django-data-browser-4.2.4/data_browser/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,15 +566,14 @@
         return [cls.element_type._parse(v, choices) for v in value]
 
 
 # Array types
 for _cls in [
     BooleanType,
     DurationType,
-    BooleanType,
     DateTimeType,
     DateType,
     UUIDType,
     URLType,
     StringType,
     NumberType,
     StringableType,
@@ -590,7 +589,8 @@
 
 class NumberChoiceArrayType(ArrayTypeMixin, BaseType):
     element_type = NumberChoiceType
     raw_type = NumberArrayType  # noqa: F821
 
 
 TYPES = {cls.name: cls for cls in all_subclasses(BaseType)}
+ARRAY_TYPES = {cls.name: cls for cls in all_subclasses(ArrayTypeMixin)}
```

### Comparing `django-data-browser-4.2.3/data_browser/urls.py` & `django-data-browser-4.2.4/data_browser/urls.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/views.py` & `django-data-browser-4.2.4/data_browser/views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/web_root/android-chrome-192x192.png` & `django-data-browser-4.2.4/data_browser/web_root/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/web_root/android-chrome-512x512.png` & `django-data-browser-4.2.4/data_browser/web_root/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/web_root/apple-touch-icon.png` & `django-data-browser-4.2.4/data_browser/web_root/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/web_root/favicon-32x32.png` & `django-data-browser-4.2.4/data_browser/web_root/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/data_browser/web_root/favicon.ico` & `django-data-browser-4.2.4/data_browser/web_root/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/django_data_browser.egg-info/PKG-INFO` & `django-data-browser-4.2.4/django_data_browser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.3
+Version: 4.2.4
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -338,14 +338,94 @@
 You can override the ``data_browser/index.html`` template per `Djangoâ€™s template overriding docs <https://docs.djangoproject.com/en/stable/howto/overriding-templates/#extending-an-overridden-template>`__, and replace the ``extrahead`` block.
 (Ensure ``"data_browser"`` is after your app in ``INSTALLED_APPS``.)
 
 This will let you inject custom CSS and stylesheets.
 
 However note that because of how the normal CSS is injected any custom CSS will be before the normal CSS so you will need to use more specific selectors or ``!important``.
 
+
+Custom functions and aggregations
+---------------------------------
+
+It is possible to register additional functions and aggregations with the Data Browser, including custom ones.
+
+Types
+^^^^^
+
+Functions and Aggregations are attached to the Data Browsers core types, these are in ``data_browser.types``.
+
+Functions
+^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The function registry is in ``data_browser.orm_functions.TYPE_FUNCTIONS`` this has type ``dict[BaseType, dict[str, data_browser.orm_functions.Func]]``. It is safe to insert new entries into this at runtime.
+
+For example to add the MD5 function to string fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models.functions import MD5
+    from data_browser.types import StringType
+    from data_browser.orm_functions import Func, TYPE_FUNCTIONS
+
+    TYPE_FUNCTIONS[StringType]["md5"] = Func(MD5, StringType)
+
+Aggregates
+^^^^^^^^^^
+
+*This functionality is provisional and not subject to normal backward compatible guarantees.*
+
+The aggregate registry is in ``data_browser.orm_aggregates.TYPE_AGGREGATES`` this has type ``dict[BaseType, dict[str, data_browser.orm_aggregates.Agg]]``. It is safe to insert new entries into this at runtime.
+
+For example to add a count that does not apply distinct to number fields you could do the following:
+
+.. code-block:: python
+
+    from django.db.models import Count
+    from data_browser.types import NumberType
+    from data_browser.orm_aggregates import Agg, TYPE_AGGREGATES
+
+    TYPE_AGGREGATES[NumberType]["full_count"] = Agg(
+        lambda x: Count(x, distinct=False), NumberType
+    )
+
+Custom SQL example
+^^^^^^^^^^^^^^^^^^
+
+For a larger example imagine you wanted to use Postgres's ``percentile_cont`` functionality to add a ``p95`` aggregate to duration fields, perhaps for some kind of application performance monitoring usecase.
+
+First we need to explain ``percentile_cont`` to Django.
+
+.. code-block:: python
+
+    from django.db.models import Aggregate
+
+    class Percentile(Aggregate):
+        arity = 1
+        function = "percentile_cont"
+        template = "%(function)s(%(percentile)s) WITHIN GROUP (ORDER BY %(expressions)s)"
+        name = "Percentile"
+
+        def __init__(self, percentile, expressions, **extra):
+            super().__init__(expressions, percentile=percentile, **extra)
+
+Then we need to tell the Data Browser we want ``p95`` on duration fields.
+
+.. code-block:: python
+
+    from data_browser.orm_aggregates import TYPE_AGGREGATES, Agg
+    from data_browser.types import DurationType
+
+    TYPE_AGGREGATES[DurationType]["p95"] = Agg(
+        lambda x: Percentile(0.95, x), DurationType
+    )
+
+
+
 Version numbers
 ---------------
 
 The Data Browser uses the standard ``Major.Minor.Patch`` version numbering scheme.
 
 Patch versions may include bug fixes and minor features.
 
@@ -365,14 +445,17 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.4   | 2023-07-02 | Provisional support for adding custom functions and aggregations.                                        |
+|         |            | Fix ``all`` aggregate on booleans and durations. (Postgres only)                                         |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.3   | 2023-06-15 | Fix ASGI compatibility issue.                                                                            |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
```

### Comparing `django-data-browser-4.2.3/django_data_browser.egg-info/SOURCES.txt` & `django-data-browser-4.2.4/django_data_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/README.md` & `django-data-browser-4.2.4/frontend/README.md`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/package-lock.json` & `django-data-browser-4.2.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/package.json` & `django-data-browser-4.2.4/frontend/package.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/public/index.html` & `django-data-browser-4.2.4/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/App.js` & `django-data-browser-4.2.4/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/App.scss` & `django-data-browser-4.2.4/frontend/src/App.scss`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/ContextMenu.js` & `django-data-browser-4.2.4/frontend/src/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/CurrentSavedView.js` & `django-data-browser-4.2.4/frontend/src/CurrentSavedView.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/HomePage.js` & `django-data-browser-4.2.4/frontend/src/HomePage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/Query.js` & `django-data-browser-4.2.4/frontend/src/Query.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/QueryPage.js` & `django-data-browser-4.2.4/frontend/src/QueryPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/Results.js` & `django-data-browser-4.2.4/frontend/src/Results.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/SavedViewPage.js` & `django-data-browser-4.2.4/frontend/src/SavedViewPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/Tooltip.js` & `django-data-browser-4.2.4/frontend/src/Tooltip.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/Util.js` & `django-data-browser-4.2.4/frontend/src/Util.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/WindowDimensions.js` & `django-data-browser-4.2.4/frontend/src/WindowDimensions.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/index.js` & `django-data-browser-4.2.4/frontend/src/index.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/frontend/src/logo.svg` & `django-data-browser-4.2.4/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/pyproject.toml` & `django-data-browser-4.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         "pragma: no cover",
     ]
     show_missing = true
     skip_covered = true
     skip_empty = true
 
 [tool.flake8]
+    target-version = "3.7"
     extend-ignore = [
         # Loop control variable not used within the loop body TODO enable this
         "B007",
         # use raise exception instead of assert False TODO enable this
         "B011",
         # Abstract base class with no abstract method.
         "B024",
```

### Comparing `django-data-browser-4.2.3/screenshot.png` & `django-data-browser-4.2.4/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/setup.py` & `django-data-browser-4.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/structure.svg` & `django-data-browser-4.2.4/structure.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/array/models.py` & `django-data-browser-4.2.4/tests/array/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/conftest.py` & `django-data-browser-4.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/core/admin.py` & `django-data-browser-4.2.4/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/core/migrations/0001_initial.py` & `django-data-browser-4.2.4/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/core/models.py` & `django-data-browser-4.2.4/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/snapshots/snap_test_views.py` & `django-data-browser-4.2.4/tests/snapshots/snap_test_views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_admin.py` & `django-data-browser-4.2.4/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_api.py` & `django-data-browser-4.2.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_array_field.py` & `django-data-browser-4.2.4/tests/test_array_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_common.py` & `django-data-browser-4.2.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_helpers.py` & `django-data-browser-4.2.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_json_field.py` & `django-data-browser-4.2.4/tests/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_migrations.py` & `django-data-browser-4.2.4/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_models.py` & `django-data-browser-4.2.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_orm.py` & `django-data-browser-4.2.4/tests/test_orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,14 +397,21 @@
 @pytest.mark.usefixtures("products")
 @pytest.mark.skipif(not POSTGRES, reason="Postgres specific feature")
 def test_get_all_aggregate(get_product_flat):
     data = get_product_flat(1, "size_unit,size__all", [])
     assert data == [["g", "[1.0, 2.0]"]]
 
 
+@pytest.mark.usefixtures("products")
+@pytest.mark.skipif(not POSTGRES, reason="Postgres specific feature")
+def test_get_all_aggregate_boolean(get_product_flat):
+    data = get_product_flat(1, "size_unit,onsale__all", [])
+    assert data == [["g", "[null]"]]
+
+
 def test_get_aggregate_underscore(products, get_product_flat):
     products[0]._underscore = 1
     products[0].save()
     data = get_product_flat(1, "size_unit,_underscore__count", [])
     assert data == [["g", 1]]
```

### Comparing `django-data-browser-4.2.3/tests/test_orm_debug.py` & `django-data-browser-4.2.4/tests/test_orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_query.py` & `django-data-browser-4.2.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tests/test_views.py` & `django-data-browser-4.2.4/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.3/tox.ini` & `django-data-browser-4.2.4/tox.ini`

 * *Files identical despite different names*

