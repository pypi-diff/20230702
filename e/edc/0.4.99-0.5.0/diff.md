# Comparing `tmp/edc-0.4.99.tar.gz` & `tmp/edc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.99.tar", last modified: Wed Jun 21 14:18:42 2023, max compression
+gzip compressed data, was "edc-0.5.0.tar", last modified: Sun Jul  2 19:04:49 2023, max compression
```

## Comparing `edc-0.4.99.tar` & `edc-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.177269 edc-0.4.99/
--rw-r--r--   0 jw         (502) staff       (20)     1410 2023-04-18 18:48:47.000000 edc-0.4.99/.gitignore
--rw-r--r--   0 jw         (502) staff       (20)     1076 2023-06-20 12:58:31.000000 edc-0.4.99/.pre-commit-config.yaml
--rw-r--r--   0 jw         (502) staff       (20)      291 2023-04-18 18:48:47.000000 edc-0.4.99/.yamllint
--rw-r--r--   0 jw         (502) staff       (20)        0 2023-04-18 18:48:47.000000 edc-0.4.99/AUTHORS
--rw-r--r--   0 jw         (502) staff       (20)    40501 2023-06-21 14:18:31.000000 edc-0.4.99/CHANGES
--rw-r--r--   0 jw         (502) staff       (20)    35147 2021-07-06 12:52:00.000000 edc-0.4.99/LICENSE
--rw-r--r--   0 jw         (502) staff       (20)      151 2021-07-06 12:52:00.000000 edc-0.4.99/MANIFEST.in
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-21 14:18:42.177508 edc-0.4.99/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)    37432 2023-05-07 19:08:23.000000 edc-0.4.99/README.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.144749 edc-0.4.99/bin/
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.152889 edc-0.4.99/bin/nginx/
--rw-r--r--   0 jw         (502) staff       (20)      350 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc-sites.conf
--rw-r--r--   0 jw         (502) staff       (20)      706 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc-uat.conf
--rw-r--r--   0 jw         (502) staff       (20)      656 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc.conf
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.155165 edc-0.4.99/bin/scripts/
--rw-r--r--   0 jw         (502) staff       (20)     2753 2023-04-18 18:48:47.000000 edc-0.4.99/bin/scripts/dev_repos.sh
--rw-r--r--   0 jw         (502) staff       (20)      276 2021-07-06 12:52:00.000000 edc-0.4.99/bin/scripts/list_db_files.sh
--rw-r--r--   0 jw         (502) staff       (20)      416 2021-07-06 12:52:00.000000 edc-0.4.99/bin/scripts/restore_db_file.sh
--rw-r--r--   0 jw         (502) staff       (20)     2408 2023-04-18 18:48:47.000000 edc-0.4.99/bin/scripts/update_edc.sh
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.158560 edc-0.4.99/bin/systemd/
--rw-r--r--   0 jw         (502) staff       (20)      835 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celery-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      820 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celery.service
--rw-r--r--   0 jw         (502) staff       (20)      501 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      487 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celerybeat.service
--rw-r--r--   0 jw         (502) staff       (20)      485 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      121 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 jw         (502) staff       (20)      474 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn.service
--rw-r--r--   0 jw         (502) staff       (20)      111 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.167423 edc-0.4.99/docs/
--rw-r--r--   0 jw         (502) staff       (20)      634 2023-04-18 18:48:47.000000 edc-0.4.99/docs/Makefile
--rw-r--r--   0 jw         (502) staff       (20)    12969 2023-05-07 19:08:23.000000 edc-0.4.99/docs/README.rst
--rw-r--r--   0 jw         (502) staff       (20)     4441 2023-04-18 18:48:47.000000 edc-0.4.99/docs/backup.rst
--rw-r--r--   0 jw         (502) staff       (20)     5437 2023-04-27 10:01:42.000000 edc-0.4.99/docs/celery.rst
--rw-r--r--   0 jw         (502) staff       (20)      580 2023-04-18 18:48:47.000000 edc-0.4.99/docs/conda.rst
--rw-r--r--   0 jw         (502) staff       (20)      975 2023-04-18 18:48:47.000000 edc-0.4.99/docs/conf.py
--rw-r--r--   0 jw         (502) staff       (20)     4806 2023-04-18 18:48:47.000000 edc-0.4.99/docs/configure_web_services.rst
--rw-r--r--   0 jw         (502) staff       (20)     3646 2023-04-18 18:48:47.000000 edc-0.4.99/docs/deploy_new_droplet.rst
--rw-r--r--   0 jw         (502) staff       (20)      163 2021-07-06 12:52:00.000000 edc-0.4.99/docs/dump_users.rst
--rw-r--r--   0 jw         (502) staff       (20)      845 2021-07-06 12:52:00.000000 edc-0.4.99/docs/exporting_encrypted_data.rst
--rw-r--r--   0 jw         (502) staff       (20)   258708 2023-04-18 18:48:47.000000 edc-0.4.99/docs/forms_reference.md
--rw-r--r--   0 jw         (502) staff       (20)      445 2023-04-18 18:48:47.000000 edc-0.4.99/docs/index.rst
--rw-r--r--   0 jw         (502) staff       (20)      778 2021-07-06 12:52:00.000000 edc-0.4.99/docs/landing_page.rst
--rw-r--r--   0 jw         (502) staff       (20)      765 2023-04-18 18:48:47.000000 edc-0.4.99/docs/make.bat
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.99/docs/multisite_deployment.rst
--rw-r--r--   0 jw         (502) staff       (20)     3928 2023-04-18 18:48:47.000000 edc-0.4.99/docs/prepare_database.rst
--rw-r--r--   0 jw         (502) staff       (20)     1211 2023-04-18 18:48:47.000000 edc-0.4.99/docs/printing.rst
--rw-r--r--   0 jw         (502) staff       (20)      187 2021-07-06 12:52:00.000000 edc-0.4.99/docs/redis.rst
--rw-r--r--   0 jw         (502) staff       (20)      766 2021-07-06 12:52:00.000000 edc-0.4.99/docs/update_deployment.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.169774 edc-0.4.99/edc.egg-info/
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)     1508 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2021-09-27 09:58:54.000000 edc-0.4.99/edc.egg-info/not-zip-safe
--rw-r--r--   0 jw         (502) staff       (20)     1923 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/requires.txt
--rw-r--r--   0 jw         (502) staff       (20)        6 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/top_level.txt
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.170056 edc-0.4.99/image/
--rw-r--r--   0 jw         (502) staff       (20)   160721 2021-08-24 11:21:23.000000 edc-0.4.99/image/icon-pycharm.png
--rw-r--r--   0 jw         (502) staff       (20)      162 2023-04-18 18:48:47.000000 edc-0.4.99/pyproject.toml
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.176102 edc-0.4.99/requirements.tests/
--rw-r--r--   0 jw         (502) staff       (20)       21 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/coverage.txt
--rw-r--r--   0 jw         (502) staff       (20)       14 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/docs.txt
--rw-r--r--   0 jw         (502) staff       (20)     1053 2023-05-07 19:16:29.000000 edc-0.4.99/requirements.tests/edc.txt
--rw-r--r--   0 jw         (502) staff       (20)     4100 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/edc_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       68 2021-07-06 12:52:00.000000 edc-0.4.99/requirements.tests/edc_offline.txt
--rw-r--r--   0 jw         (502) staff       (20)       54 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/lint.txt
--rw-r--r--   0 jw         (502) staff       (20)       11 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/mysql.txt
--rw-r--r--   0 jw         (502) staff       (20)       22 2021-07-06 12:52:00.000000 edc-0.4.99/requirements.tests/postgres.txt
--rw-r--r--   0 jw         (502) staff       (20)       86 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/test_utils.txt
--rw-r--r--   0 jw         (502) staff       (20)      238 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/third_party_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       50 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/tox.txt
--rw-r--r--   0 jw         (502) staff       (20)     2995 2023-06-21 14:18:42.178653 edc-0.4.99/setup.cfg
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.176897 edc-0.4.99/utils/
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.99/utils/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)      721 2023-04-18 18:48:47.000000 edc-0.4.99/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.344677 edc-0.5.0/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.0/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.0/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.0/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    40752 2023-07-02 19:04:41.000000 edc-0.5.0/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.0/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.0/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-02 19:04:49.344812 edc-0.5.0/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.0/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.322131 edc-0.5.0/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.326458 edc-0.5.0/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.0/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.0/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.0/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.327248 edc-0.5.0/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.0/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.0/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.0/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.0/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.328600 edc-0.5.0/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.0/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.332673 edc-0.5.0/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.0/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.0/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.0/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.0/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.0/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.0/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.0/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.0/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.0/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.0/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.0/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.0/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.0/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.0/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.0/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.0/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.0/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.0/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.0/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.340979 edc-0.5.0/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-02 19:04:49.000000 edc-0.5.0/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-02 19:04:49.000000 edc-0.5.0/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-02 19:04:49.000000 edc-0.5.0/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.0/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1941 2023-07-02 19:04:49.000000 edc-0.5.0/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-02 19:04:49.000000 edc-0.5.0/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.341110 edc-0.5.0/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.0/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.0/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.344142 edc-0.5.0/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.0/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.0/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.0/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.0/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.0/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.0/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.0/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.0/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.0/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.0/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.0/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     3014 2023-07-02 19:04:49.345277 edc-0.5.0/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 19:04:49.344441 edc-0.5.0/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.0/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.0/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.99/.gitignore` & `edc-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/.pre-commit-config.yaml` & `edc-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/CHANGES` & `edc-0.5.0/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changes
 -------
 
+0.5.0
+------
+- add additonal validation to check screening identifier and the screening
+  eligibility boolean. (edc-cosent)
+- add mixin to redirect all forms to a selected changelist (edc-model-admin)
+- improve redirect on delete (edc-model-admin)
+
+
+
 0.4.99
 ------
 - fix rounding issue with md section numbers, allow opt out of timestamp on
   every form rendered (edc-form-describer)
 
 0.4.98
 ------
```

### Comparing `edc-0.4.99/LICENSE` & `edc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/PKG-INFO` & `edc-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.99
+Version: 0.5.0
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
@@ -33,16 +33,16 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
```

### Comparing `edc-0.4.99/README.rst` & `edc-0.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
```

### Comparing `edc-0.4.99/bin/nginx/edc-uat.conf` & `edc-0.5.0/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/bin/nginx/edc.conf` & `edc-0.5.0/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/bin/scripts/dev_repos.sh` & `edc-0.5.0/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/bin/scripts/update_edc.sh` & `edc-0.5.0/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/bin/systemd/celery-uat.service` & `edc-0.5.0/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/bin/systemd/celery.service` & `edc-0.5.0/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/Makefile` & `edc-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/README.rst` & `edc-0.5.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/backup.rst` & `edc-0.5.0/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/celery.rst` & `edc-0.5.0/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/conda.rst` & `edc-0.5.0/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/conf.py` & `edc-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/configure_web_services.rst` & `edc-0.5.0/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/deploy_new_droplet.rst` & `edc-0.5.0/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/exporting_encrypted_data.rst` & `edc-0.5.0/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/forms_reference.md` & `edc-0.5.0/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/landing_page.rst` & `edc-0.5.0/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/make.bat` & `edc-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/prepare_database.rst` & `edc-0.5.0/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/printing.rst` & `edc-0.5.0/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/docs/update_deployment.rst` & `edc-0.5.0/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/edc.egg-info/PKG-INFO` & `edc-0.5.0/edc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.99
+Version: 0.5.0
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
@@ -33,16 +33,16 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials have been related to HIV/AIDS research. Recent work with the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ has expanded into Diabetes (DM),
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
```

### Comparing `edc-0.4.99/edc.egg-info/SOURCES.txt` & `edc-0.5.0/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/edc.egg-info/requires.txt` & `edc-0.5.0/edc.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 argon2-cffi
 boto3
 celery
 gunicorn
-inflect
+inflect==6.0.4
+pydantic<2
 mysqlclient
 pycups
 pyrabbit
 python-dateutil
 python-memcached
 reportlab
 tqdm
@@ -21,18 +22,18 @@
 django-multisite-edc==2.0.0
 django-revision==0.3.6
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
 edc-action-item==0.3.52
 edc-adherence==0.1.21
-edc-adverse-event==0.3.52
+edc-adverse-event==0.3.53
 edc-appointment==0.3.72
 edc-auth==0.3.60
-edc-consent==0.3.45
+edc-consent==0.3.46
 edc-constants==0.3.48
 edc-crf==0.3.43
 edc-dashboard==0.3.45
 edc-data-manager==0.3.53
 edc-device==0.3.11
 edc-document-status==0.1.4
 edc-dx==0.1.19
@@ -55,37 +56,37 @@
 edc-list-data==0.3.18
 edc-listboard==0.1.9
 edc-locator==0.3.23
 edc-ltfu==0.3.23
 edc-metadata==0.3.51
 edc-mnsi==0.1.16
 edc-model==0.3.30
-edc-model-admin==0.3.44
+edc-model-admin==0.3.45
 edc-model-fields==0.3.7
 edc-model-form==0.1.11
 edc-model-wrapper==0.3.10
 edc-navbar==0.3.16
 edc-notification==0.3.17
-edc-offstudy==0.3.31
+edc-offstudy==0.3.32
 edc-pdf-reports==0.3.13
 edc-pdutils==0.3.22
 edc-pharmacy==0.1.38
 edc-pharmacy-dashboard==0.1.3
 edc-prn==0.3.13
 edc-protocol==0.3.9
 edc-protocol-incident==0.1.25
 edc-qol==0.1.14
 edc-randomization==0.3.46
 edc-reference==0.3.15
-edc-refusal==0.1.11
+edc-refusal==0.1.12
 edc-registration==0.3.28
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
 edc-rx==0.1.6
-edc-screening==0.3.33
+edc-screening==0.3.34
 edc-search==0.3.7
 edc-sites==0.3.20
 edc-subject-dashboard==0.3.36
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
 edc-unblinding==0.1.14
```

### Comparing `edc-0.4.99/image/icon-pycharm.png` & `edc-0.5.0/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/requirements.tests/edc.txt` & `edc-0.5.0/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/requirements.tests/edc_dev.txt` & `edc-0.5.0/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.99/setup.cfg` & `edc-0.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 include_package_data = True
 packages = find:
 install_requires = 
 	argon2-cffi
 	boto3
 	celery
 	gunicorn
-	inflect
+	inflect==6.0.4
+	pydantic<2
 	mysqlclient
 	pycups
 	pyrabbit
 	python-dateutil
 	python-memcached
 	reportlab
 	tqdm
@@ -50,18 +51,18 @@
 	django-multisite-edc==2.0.0
 	django-revision==0.3.6
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
 	edc-action-item==0.3.52
 	edc-adherence==0.1.21
-	edc-adverse-event==0.3.52
+	edc-adverse-event==0.3.53
 	edc-appointment==0.3.72
 	edc-auth==0.3.60
-	edc-consent==0.3.45
+	edc-consent==0.3.46
 	edc-constants==0.3.48
 	edc-crf==0.3.43
 	edc-dashboard==0.3.45
 	edc-data-manager==0.3.53
 	edc-device==0.3.11
 	edc-document-status==0.1.4
 	edc-dx==0.1.19
@@ -84,37 +85,37 @@
 	edc-list-data==0.3.18
 	edc-listboard==0.1.9
 	edc-locator==0.3.23
 	edc-ltfu==0.3.23
 	edc-metadata==0.3.51
 	edc-mnsi==0.1.16
 	edc-model==0.3.30
-	edc-model-admin==0.3.44
+	edc-model-admin==0.3.45
 	edc-model-fields==0.3.7
 	edc-model-form==0.1.11
 	edc-model-wrapper==0.3.10
 	edc-navbar==0.3.16
 	edc-notification==0.3.17
-	edc-offstudy==0.3.31
+	edc-offstudy==0.3.32
 	edc-pdf-reports==0.3.13
 	edc-pdutils==0.3.22
 	edc-pharmacy==0.1.38
 	edc-pharmacy-dashboard==0.1.3
 	edc-prn==0.3.13
 	edc-protocol==0.3.9
 	edc-protocol-incident==0.1.25
 	edc-qol==0.1.14
 	edc-randomization==0.3.46
 	edc-reference==0.3.15
-	edc-refusal==0.1.11
+	edc-refusal==0.1.12
 	edc-registration==0.3.28
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
 	edc-rx==0.1.6
-	edc-screening==0.3.33
+	edc-screening==0.3.34
 	edc-search==0.3.7
 	edc-sites==0.3.20
 	edc-subject-dashboard==0.3.36
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
 	edc-unblinding==0.1.14
```

### Comparing `edc-0.4.99/utils/get_edc_requirements.py` & `edc-0.5.0/utils/get_edc_requirements.py`

 * *Files identical despite different names*

