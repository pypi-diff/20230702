# Comparing `tmp/cterasdk-2.8.32.tar.gz` & `tmp/cterasdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cterasdk-2.8.32.tar", last modified: Wed Mar  8 22:03:08 2023, max compression
+gzip compressed data, was "cterasdk-2.9.0.tar", last modified: Fri Jan 15 19:01:04 2021, max compression
```

## Comparing `cterasdk-2.8.32.tar` & `cterasdk-2.9.0.tar`

### file list

```diff
@@ -1,185 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:08.001707 cterasdk-2.8.32/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.981707 cterasdk-2.8.32/.actionspanel/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-08 22:03:02.000000 cterasdk-2.8.32/.actionspanel/buttons.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.981707 cterasdk-2.8.32/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.981707 cterasdk-2.8.32/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-08 22:03:02.000000 cterasdk-2.8.32/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-08 22:03:07.000000 cterasdk-2.8.32/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-03-08 22:03:07.000000 cterasdk-2.8.32/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-08 22:03:02.000000 cterasdk-2.8.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-08 22:03:02.000000 cterasdk-2.8.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-08 22:03:08.001707 cterasdk-2.8.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-08 22:03:02.000000 cterasdk-2.8.32/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.985707 cterasdk-2.8.32/cterasdk/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.985707 cterasdk-2.8.32/cterasdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/client/cteraclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/client/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/client/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/client/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.985707 cterasdk-2.8.32/cterasdk/common/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.985707 cterasdk-2.8.32/cterasdk/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/convert/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/convert/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/convert/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/convert/xml_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.989707 cterasdk-2.8.32/cterasdk/core/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/antivirus.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/base_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/cloudfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/directoryservice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.993707 cterasdk-2.8.32/cterasdk/core/files/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/fetch_resources_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/file_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/ln.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/files/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/firmwares.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/portals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/storage_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/taskmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/core/zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.997707 cterasdk-2.8.32/cterasdk/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/afp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/base_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/directoryservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/directorytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.997707 cterasdk-2.8.32/cterasdk/edge/files/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/file_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/move.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/files/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/migration_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/nfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/smb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/taskmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/telnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/timezone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/edge/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:08.001707 cterasdk-2.8.32/cterasdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/consent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/file_access_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/session_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/task_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:08.001707 cterasdk-2.8.32/cterasdk/object/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/object/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/object/Gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/object/Portal.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/object/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:08.001707 cterasdk-2.8.32/cterasdk/transcript/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/transcript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/transcript/apidoc.template
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-08 22:03:02.000000 cterasdk-2.8.32/cterasdk/transcript/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 22:03:07.985707 cterasdk-2.8.32/cterasdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-08 22:03:07.000000 cterasdk-2.8.32/cterasdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-08 22:03:02.000000 cterasdk-2.8.32/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-08 22:03:08.001707 cterasdk-2.8.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-08 22:03:02.000000 cterasdk-2.8.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.346538 cterasdk-2.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/.actionspanel/
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2021-01-15 19:00:50.000000 cterasdk-2.9.0/.actionspanel/buttons.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.330538 cterasdk-2.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2346 2021-01-15 19:00:50.000000 cterasdk-2.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      223 2021-01-15 19:01:03.000000 cterasdk-2.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)     7935 2021-01-15 19:01:03.000000 cterasdk-2.9.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (116)      555 2021-01-15 19:00:50.000000 cterasdk-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      296 2021-01-15 19:00:50.000000 cterasdk-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     3929 2021-01-15 19:01:04.346538 cterasdk-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2440 2021-01-15 19:00:50.000000 cterasdk-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/cterasdk/
+-rw-r--r--   0 runner    (1001) docker     (116)      775 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/cterasdk/client/
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4657 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/client/cteraclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9737 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/client/host.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9303 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (116)      596 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/client/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/cterasdk/common/
+-rw-r--r--   0 runner    (1001) docker     (116)      444 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      844 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/enum.py
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/item.py
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/object.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5667 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3984 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2010 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/cterasdk/convert/
+-rw-r--r--   0 runner    (1001) docker     (116)      181 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       42 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/convert/exception.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3635 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/convert/format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4434 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/convert/parse.py
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/convert/xml_types.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.338538 cterasdk-2.9.0/cterasdk/core/
+-rw-r--r--   0 runner    (1001) docker     (116)      483 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      932 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/activation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3930 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/antivirus.py
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7367 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/cloudfs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      106 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1059 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6066 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/devices.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3627 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/directoryservice.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7844 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.338538 cterasdk-2.9.0/cterasdk/core/files/
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8056 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/browser.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12179 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1753 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/common.py
+-rw-r--r--   0 runner    (1001) docker     (116)      578 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/cp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2143 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/directory.py
+-rw-r--r--   0 runner    (1001) docker     (116)      793 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/fetch_resources_param.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1948 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/file_access.py
+-rw-r--r--   0 runner    (1001) docker     (116)      630 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/ln.py
+-rw-r--r--   0 runner    (1001) docker     (116)      717 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/ls.py
+-rw-r--r--   0 runner    (1001) docker     (116)      554 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/mv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1804 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      500 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/recover.py
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/rename.py
+-rw-r--r--   0 runner    (1001) docker     (116)      486 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/files/rm.py
+-rw-r--r--   0 runner    (1001) docker     (116)      712 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3709 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10215 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/plans.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5477 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/portals.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5699 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)      668 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1418 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/reports.py
+-rw-r--r--   0 runner    (1001) docker     (116)      758 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/servers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1007 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10729 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1568 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/startup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1164 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/taskmgr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6528 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      290 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/uri.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7054 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/users.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7455 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/core/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.342538 cterasdk-2.9.0/cterasdk/edge/
+-rw-r--r--   0 runner    (1001) docker     (116)      929 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      554 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/afp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1361 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/aio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2105 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/array.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2576 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/audit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9445 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/backup.py
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3088 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)      614 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3054 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      475 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      629 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5151 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/directoryservice.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5144 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/directorytree.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1290 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/drive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9984 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.342538 cterasdk-2.9.0/cterasdk/edge/files/
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3335 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/browser.py
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/copy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1236 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/file_access.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1366 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/move.py
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/open.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1200 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      279 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/files/rm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2074 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2804 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3154 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/groups.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (116)      933 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2062 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1860 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/mail.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5371 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/network.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1895 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/nfs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1034 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2386 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/power.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1244 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1802 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7962 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/services.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2310 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/session.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12907 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/shares.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/shell.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4716 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/smb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3357 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/support.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3917 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3108 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1609 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/taskmgr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (116)      688 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7733 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1512 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/uri.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4141 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/users.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8021 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/edge/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3378 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.342538 cterasdk-2.9.0/cterasdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (116)      429 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      181 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (116)      450 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/consent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3309 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/file_access_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4816 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (116)      806 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      882 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/platform.py
+-rw-r--r--   0 runner    (1001) docker     (116)      576 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/registry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1429 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/session_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2549 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/task_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2859 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (116)      910 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.346538 cterasdk-2.9.0/cterasdk/object/
+-rw-r--r--   0 runner    (1001) docker     (116)     1451 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/object/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8839 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/object/Gateway.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7348 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/object/Portal.py
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/object/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.346538 cterasdk-2.9.0/cterasdk/transcript/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/transcript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      551 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/transcript/apidoc.template
+-rw-r--r--   0 runner    (1001) docker     (116)     3356 2021-01-15 19:00:50.000000 cterasdk-2.9.0/cterasdk/transcript/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:01:04.334538 cterasdk-2.9.0/cterasdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3929 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3900 2021-01-15 19:01:04.000000 cterasdk-2.9.0/cterasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-01-15 19:01:03.000000 cterasdk-2.9.0/cterasdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-15 19:00:50.000000 cterasdk-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      905 2021-01-15 19:01:04.346538 cterasdk-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-01-15 19:00:50.000000 cterasdk-2.9.0/setup.py
```

### Comparing `cterasdk-2.8.32/.github/workflows/ci.yml` & `cterasdk-2.9.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     types: [published, prereleased]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8]
+        python-version: [3.6, 3.7, 3.8]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -48,22 +48,28 @@
         python-version: 3.x
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools wheel
     - name: Build package
       run: |
         python setup.py sdist bdist_wheel
+    - name: Deploy to Test PyPi
+      uses: pypa/gh-action-pypi-publish@master
+      with:
+        user: __token__
+        password: ${{ secrets.TEST_PYPI_TOKEN }}
+        repository_url: https://test.pypi.org/legacy/
     - name: Deploy to PyPi
       uses: pypa/gh-action-pypi-publish@master
       with:
         user: __token__
         password: ${{ secrets.PYPI_TOKEN }}
       if: github.event.action == 'published'
     - id: tagName
       uses: little-core-labs/get-git-tag@v3.0.1
     - name: Notify Teams
       uses: aliencube/microsoft-teams-actions@v0.8.0
       with:
         webhook_uri: ${{ secrets.MS_TEAMS_WEBHOOK_URI }}
         title: CTERA Python SDK version ${{ steps.tagName.outputs.tag }} was released
         summary: Python SDK Version
-        actions: '[{ "@type": "OpenUri", "name": "PyPi", "targets": [{ "os": "default", "uri": "https://pypi.org/project/cterasdk/"}] }]'
+        actions: '[{ "@type": "OpenUri", "name": "PyPi", "targets": [{ "os": "default", "uri": "https://pypi.org/project/cterasdk/"}] }]'
```

### Comparing `cterasdk-2.8.32/ChangeLog` & `cterasdk-2.9.0/ChangeLog`

 * *Files 26% similar despite different names*

```diff
@@ -1,307 +1,10 @@
 CHANGES
 =======
 
-2.8.32
-------
-
-* Saimon/local dedup (#179)
-
-2.8.31
-------
-
-* Saimon/storage classes and evict (#178)
-
-2.18.30
--------
-
-* Saimon/migration tool updates (#177)
-
-2.18.29
--------
-
-* Saimon/sdk enhancements (#176)
-* Saimon/migration tool (#175)
-
-2.18.28
--------
-
-* Saimon/migration tool (#174)
-
-2.18.27
--------
-
-* Saimon/server tasks (#172)
-
-2.18.26
--------
-
-* fix for allowing unicode characters in request and response (#170)
-
-2.18.25
--------
-
-* set folder/owner acl (#159)
-* CTERA Messaging service (#169)
-
-2.18.24
--------
-
-* cterasdk/core/types.py GenericS3 (#167)
-
-2.18.23
--------
-
-* fix documentation (#166)
-
-2.18.22
--------
-
-* enum.BucketType.GenericS3 (#165)
-
-2.18.21
--------
-
-* Server timeout exception fix (#164)
-
-2.18.20
--------
-
-* Saimon/remove prints (#163)
-
-2.18.19
--------
-
-* Saimon/list search zones (#162)
-
-2.18.18
--------
-
-* update xml parser - deprecated method (#161)
-
-2.18.17
--------
-
-* Update SNMP v3 extensions to support authentication and privacy passw… (#160)
-* added support for core/admins.Administrators (#155)
-
-2.18.16
--------
-
-* Saimon/log based alerts (#157)
-* Edge-Network-StaticRoutes-get/set/del/clean + UnitTests (#156)
-
-2.18.15
--------
-
-* Saimon/configure advanced mapping (#154)
-
-2.18.14
--------
-
-* Ignore protected-access warning in tests
-* Do not deploy to PyPi Test
-
-2.18.13
--------
-
-* Add support for configuring insecure NFS connections
-* Allow the caller to limit NFS to specific host
-
-2.18.12
--------
-
-* added FixedBlockSize support param to mkfg() added enum obj
-
-2.18.11
--------
-
-* Support modifying all the NFS configuration values
-
-2.18.10
--------
-
-* Edge Shares - allow the user to pass the UUID when creating the share
-
-2.18.9
-------
-
-* Add Edge Sync API to get and set LinuxAvoidUsingFAnotify
-
-2.18.8
-------
-
-* Use f-Strings instead of formatting
-* Ignore coverage report file
-
-2.18.7
-------
-
-* Add LVM array type option (#145)
-
-2.18.6
-------
-
-* update find\_attr (#144)
-* Saimon/import filer config (#140)
-* Saimon/smb protocol version (#141)
-* Saimon/backups file browser (#139)
-* Saimon/minor infra improvement (#142)
-* Saimon/templates scripts cli (#138)
-* Saimon/fix pylint (#143)
-
-2.18.5
-------
-
-* Saimon/improve ntp config (#137)
-
-2.18.4
-------
-
-* Change proto to protocol to resolve Ansible play (#136)
-
-2.18.3
-------
-
-* Support modifying syslog server config (#135)
-
-2.18.2
-------
-
-* SDK Improvements for Ansible Plays (#134)
-
-2.18.1
-------
-
-* Add a method for obtaining the connected domain (#133)
-
-2.18.0
-------
-
-* Support Portal Active Directory conn. mgmt. (#132)
-* Saimon/update servers (#131)
-* Enhancements: (#130)
-
-2.17.3
-------
-
-* Change hex computation to be backward compatible with Python 3.6 (#129)
-
-2.17.2
-------
-
-* Catch OS errors when loading private key and certificate files. (e.g.… (#128)
-
-2.17.1
-------
-
-* Improve SSL mangement: (#127)
-* Resolve documentation issues (#126)
-
-2.17.0
-------
-
-* Saimon/create array with all drives (#124)
-* Address PyLint issues
-
-2.16.3
-------
-
-* Edge Share - complete CRUD
-
-2.16.2
-------
-
-* Gateway Share - Add APIs for directly managing NFS Trusted Clients
-
-2.16.1
-------
-
-* Change replicate\_from to an optional value (#120)
-
-2.16.0
-------
-
-* Add NetApp StorageGRID storage type (#119)
-* Update GlobalAdmin.rst
-
-2.15.0
-------
-
-* Support managing local licenses on an edge filer (#117)
-* Saimon/expand template support (#118)
-* Saimon/logout if session active (#116)
-
-2.14.1
-------
-
-* Agent - Omit internal fields from string output
-* Update FileBrowser.rst
-* fix: test-requirements.txt to reduce vulnerabilities
-* Doc badge should point to latest
-* Docs - Add cryptography to the docs requirements file
-
-2.14.0
-------
-
-* Add partial support for Portal configuration templates: (#113)
-
-2.13.3
-------
-
-* Crypto - Restrict private key permissions
-
-2.13.2
-------
-
-* Support enabling SSH daemon (#110)
-
-2.12.0
-------
-
-* Support iperf (#108)
-
-2.11.5
-------
-
-* Saimon/support blocking sync suspend (#107)
-* fix: test-requirements.txt to reduce vulnerabilities
-
-2.11.4
-------
-
-* Filer Share - Add get ACL
-* Use freeze\_time instead of mocking datetime
-
-2.11.3
-------
-
-* Auto include name, group and owner in find method (#103)
-
-2.11.2
-------
-
-* Support locating a cloud drive folder owned by a domain user (#102)
-
-2.11.1
-------
-
-* Load relevant modules for Agent to allow execution from remote access (#101)
-
-2.11.0
-------
-
-* Support sync exclusion rules, update docs (#99)
-* Update doc strings (#100)
-
-2.10.0
-------
-
-* Add support for storage buckets (#98)
-
 2.9.0
 -----
 
 * Add support for Portal antivirus APIs (#97)
 * Fix typo (#96)
 
 2.8.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cterasdk-2.8.32/LICENSE` & `cterasdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/PKG-INFO` & `cterasdk-2.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,95 @@
 Metadata-Version: 2.1
 Name: cterasdk
-Version: 2.8.32
+Version: 2.9.0
 Summary: CTERA Python SDK
 Home-page: https://pypi.org/project/cterasdk/
 Author: CTERA Networks
 Author-email: support@ctera.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ctera/ctera-python-sdk/issues
 Project-URL: Documentation, https://ctera-python-sdk.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ctera/ctera-python-sdk
+Description: ****************
+        CTERA for Python
+        ****************
+        .. image:: https://travis-ci.com/ctera/ctera-python-sdk.svg?branch=master
+           :target: https://travis-ci.com/ctera/ctera-python-sdk
+        .. image:: https://github.com/ctera/ctera-python-sdk/workflows/CI/badge.svg
+           :target: https://github.com/ctera/ctera-python-sdk/actions?query=workflow%3ACI
+        .. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=stable
+           :target: https://ctera-python-sdk.readthedocs.io/en/stable
+           :alt: [Latest Release Documentation]
+        .. image:: https://snyk.io/test/github/ctera/ctera-python-sdk/badge.svg
+           :target: https://snyk.io/test/github/ctera/ctera-python-sdk
+        .. image:: https://img.shields.io/pypi/v/cterasdk
+           :target: https://pypi.org/pypi/cterasdk
+           :alt: [Latest Release Version]
+        .. image:: https://img.shields.io/pypi/wheel/cterasdk
+           :target: https://pypi.org/pypi/cterasdk
+           :alt: PyPI - Wheel
+        .. image:: https://img.shields.io/pypi/l/cterasdk
+           :target: https://opensource.org/licenses/Apache-2.0
+           :alt: [Latest Release License]
+        .. image:: https://img.shields.io/pypi/pyversions/cterasdk
+            :target: https://pypi.org/pypi/cterasdk
+            :alt: [Latest Release Supported Python Versions]
+        .. image:: https://img.shields.io/pypi/status/cterasdk
+            :target: https://pypi.org/pypi/cterasdk
+            :alt: [Latest Release Development Stage]
+        
+        A Python SDK for integrating with the CTERA Global File System API. Compatible with Python
+        3.5+. 
+        
+        Documentation
+        -------------
+        User documentation is available on `Read the Docs <http://ctera-python-sdk.readthedocs.org/>`_.
+        
+        Installation
+        ------------
+        Installing via `pip <https://pip.pypa.io/>`_:
+        
+        .. code-block:: console
+        
+            $ pip install cterasdk
+        
+        Install from source:
+        
+        .. code-block:: console
+        
+           $ git clone https://github.com/ctera/ctera-python-sdk.git
+           $ cd ctera-python-sdk
+           $ python setup.py install
+        
+        Importing the Library
+        ---------------------
+        After installation, to get started, open a Python console:
+        
+        .. code-block:: pycon
+        
+            >>> from cterasdk import *
+        
+        Building Documentation
+        -------------------------
+        Documentation can be compiled by running ``make html`` from the ``docs``
+        folder. After compilation, open ``docs/build/html/index.html``. 
+        
+        Testing
+        -------
+        We use the `tox <https://tox.readthedocs.org/>`_ package to run tests in Python
+        3. To install, use :code:`pip install tox`. Once installed, run `tox` from the
+        root directory.
+        
+        .. code-block:: console
+        
+           $ tox
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
 Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
-
-****************
-CTERA for Python
-****************
-.. image:: https://travis-ci.com/ctera/ctera-python-sdk.svg?branch=master
-   :target: https://travis-ci.com/ctera/ctera-python-sdk
-.. image:: https://github.com/ctera/ctera-python-sdk/workflows/CI/badge.svg
-   :target: https://github.com/ctera/ctera-python-sdk/actions?query=workflow%3ACI
-.. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=latest
-   :target: https://ctera-python-sdk.readthedocs.io/en/latest
-   :alt: [Latest Release Documentation]
-.. image:: https://snyk.io/test/github/ctera/ctera-python-sdk/badge.svg
-   :target: https://snyk.io/test/github/ctera/ctera-python-sdk
-.. image:: https://img.shields.io/pypi/v/cterasdk
-   :target: https://pypi.org/pypi/cterasdk
-   :alt: [Latest Release Version]
-.. image:: https://img.shields.io/pypi/wheel/cterasdk
-   :target: https://pypi.org/pypi/cterasdk
-   :alt: PyPI - Wheel
-.. image:: https://img.shields.io/pypi/l/cterasdk
-   :target: https://opensource.org/licenses/Apache-2.0
-   :alt: [Latest Release License]
-.. image:: https://img.shields.io/pypi/pyversions/cterasdk
-    :target: https://pypi.org/pypi/cterasdk
-    :alt: [Latest Release Supported Python Versions]
-.. image:: https://img.shields.io/pypi/status/cterasdk
-    :target: https://pypi.org/pypi/cterasdk
-    :alt: [Latest Release Development Stage]
-
-A Python SDK for integrating with the CTERA Global File System API. Compatible with Python
-3.5+.
-
-Documentation
--------------
-User documentation is available on `Read the Docs <http://ctera-python-sdk.readthedocs.org/>`_.
-
-Installation
-------------
-Installing via `pip <https://pip.pypa.io/>`_:
-
-.. code-block:: console
-
-    $ pip install cterasdk
-
-..
-
-If you receive a certificate error, add the following trusted hosts:
-
-.. code-block:: console
-
-    $ pip install cterasdk --trusted-host pypi.org --trusted-host files.pythonhosted.org  # [SSL: CERTIFICATE_VERIFY_FAILED]
-
-..
-
-Installation via proxy:
-
-.. code-block:: console
-
-    $ pip install cterasdk --proxy http://user:password@proxyserver:port  # use proxy
-
-..
-
-Install from source:
-
-.. code-block:: console
-
-   $ git clone https://github.com/ctera/ctera-python-sdk.git
-   $ cd ctera-python-sdk
-   $ python setup.py install
-
-Importing the Library
----------------------
-After installation, to get started, open a Python console:
-
-.. code-block:: python
-
-    >>> from cterasdk import *
-
-Building Documentation
--------------------------
-Documentation can be compiled by running ``make html`` from the ``docs``
-folder. After compilation, open ``docs/build/html/index.html``.
-
-Testing
--------
-We use the `tox <https://tox.readthedocs.org/>`_ package to run tests in Python
-3. To install, use :code:`pip install tox`. Once installed, run `tox` from the
-root directory.
-
-.. code-block:: console
-
-   $ tox
-
```

### Comparing `cterasdk-2.8.32/README.rst` & `cterasdk-2.9.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ****************
 CTERA for Python
 ****************
 .. image:: https://travis-ci.com/ctera/ctera-python-sdk.svg?branch=master
    :target: https://travis-ci.com/ctera/ctera-python-sdk
 .. image:: https://github.com/ctera/ctera-python-sdk/workflows/CI/badge.svg
    :target: https://github.com/ctera/ctera-python-sdk/actions?query=workflow%3ACI
-.. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=latest
-   :target: https://ctera-python-sdk.readthedocs.io/en/latest
+.. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=stable
+   :target: https://ctera-python-sdk.readthedocs.io/en/stable
    :alt: [Latest Release Documentation]
 .. image:: https://snyk.io/test/github/ctera/ctera-python-sdk/badge.svg
    :target: https://snyk.io/test/github/ctera/ctera-python-sdk
 .. image:: https://img.shields.io/pypi/v/cterasdk
    :target: https://pypi.org/pypi/cterasdk
    :alt: [Latest Release Version]
 .. image:: https://img.shields.io/pypi/wheel/cterasdk
@@ -23,66 +23,48 @@
     :target: https://pypi.org/pypi/cterasdk
     :alt: [Latest Release Supported Python Versions]
 .. image:: https://img.shields.io/pypi/status/cterasdk
     :target: https://pypi.org/pypi/cterasdk
     :alt: [Latest Release Development Stage]
 
 A Python SDK for integrating with the CTERA Global File System API. Compatible with Python
-3.5+.
+3.5+. 
 
 Documentation
 -------------
 User documentation is available on `Read the Docs <http://ctera-python-sdk.readthedocs.org/>`_.
 
 Installation
 ------------
 Installing via `pip <https://pip.pypa.io/>`_:
 
 .. code-block:: console
 
     $ pip install cterasdk
 
-..
-
-If you receive a certificate error, add the following trusted hosts:
-
-.. code-block:: console
-
-    $ pip install cterasdk --trusted-host pypi.org --trusted-host files.pythonhosted.org  # [SSL: CERTIFICATE_VERIFY_FAILED]
-
-..
-
-Installation via proxy:
-
-.. code-block:: console
-
-    $ pip install cterasdk --proxy http://user:password@proxyserver:port  # use proxy
-
-..
-
 Install from source:
 
 .. code-block:: console
 
    $ git clone https://github.com/ctera/ctera-python-sdk.git
    $ cd ctera-python-sdk
    $ python setup.py install
 
 Importing the Library
 ---------------------
 After installation, to get started, open a Python console:
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from cterasdk import *
 
 Building Documentation
 -------------------------
 Documentation can be compiled by running ``make html`` from the ``docs``
-folder. After compilation, open ``docs/build/html/index.html``.
+folder. After compilation, open ``docs/build/html/index.html``. 
 
 Testing
 -------
 We use the `tox <https://tox.readthedocs.org/>`_ package to run tests in Python
 3. To install, use :code:`pip install tox`. Once installed, run `tox` from the
 root directory.
```

### Comparing `cterasdk-2.8.32/cterasdk/__init__.py` & `cterasdk-2.9.0/cterasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/client/cteraclient.py` & `cterasdk-2.9.0/cterasdk/client/cteraclient.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .http import HTTPClient, ContentType, HTTPException, HTTPResponse, geturi
-from ..convert import fromxmlstr, fromjsonstr, toxmlstr, tojsonstr
+from ..convert import fromxmlstr, toxmlstr
 from ..exception import CTERAClientException
 from ..lib import Command
 from ..common import Object
 from ..transcript import transcribe
 from .. import config
 
 
@@ -84,85 +84,28 @@
         self.http_client.set_session_id(session_id)
 
     def set_authorization_headers(self, headers):
         self.http_client.set_custom_headers(headers)
 
     @staticmethod
     def fromxmlstr(request, response):
-        response = transcribe_request(request, response, True)
+        if not config.transcript['disabled']:
+            response = HTTPResponse(response)
+            transcribe.transcribe(request, response)
         return fromxmlstr(response.text)
 
     @staticmethod
     def file_descriptor(request, response):
-        return transcribe_request(request, response, False)
+        if not config.transcript['disabled']:
+            transcribe.transcribe(request)
+        return response
 
     @staticmethod
     def _execute(function, return_function=None):
         return_function = return_function or CTERAClient.fromxmlstr
-        return execute_request(function, return_function)
-
-
-def execute_request(request_function, return_function):
-    """
-    Execute an HTTP request
-    """
-    try:
-        request, response = request_function()
-        return return_function(request, response)
-    except HTTPException as http_error:
-        client_error = CTERAClientException()
-        client_error.__dict__ = http_error.__dict__.copy()
-        raise client_error
-
-
-def transcribe_request(request, response, transcribe_response=True):
-    """
-    Transcribe the HTTP request
-    """
-    if not config.transcript['disabled']:
-        if transcribe_response:
-            response = HTTPResponse(response)
-            transcribe.transcribe(request, response)
-        else:
-            transcribe.transcribe(request)
-    return response
-
-
-class RESTClient:
-
-    def __init__(self, http_client=None, session_id_key=None):
-        self.http_client = http_client if http_client else HTTPClient(session_id_key)
-
-    def get(self, baseurl, path, params=None):
-        function = Command(HTTPClient.get, self.http_client, geturi(baseurl, path), params if params else {})
-        return self._execute(function)
-
-    def put(self, baseurl, path, data):
-        function = Command(HTTPClient.put, self.http_client, geturi(baseurl, path), ContentType.application_json, tojsonstr(data))
-        return self._execute(function)
-
-    def post(self, baseurl, path, data):
-        function = Command(HTTPClient.post, self.http_client, geturi(baseurl, path), ContentType.application_json, tojsonstr(data))
-        return self._execute(function)
-
-    def delete(self, baseurl, path):
-        function = Command(HTTPClient.delete, self.http_client, geturi(baseurl, path))
-        return self._execute(function)
-
-    @staticmethod
-    def fromjsonstr(request, response):
-        response = transcribe_request(request, response, True)
-        return fromjsonstr(response.text)
-
-    @staticmethod
-    def _execute(function):
-        return execute_request(function, RESTClient.fromjsonstr)
-
-
-class MigrationClient(RESTClient):
-
-    XSRF_TOKEN_ID = 'x-mt-x'
-
-    def login(self, baseurl, path):
-        _, response = self.http_client.get(geturi(baseurl, path))
-        xsrf_token = response.headers.get(MigrationClient.XSRF_TOKEN_ID, None)
-        self.http_client.set_custom_headers({MigrationClient.XSRF_TOKEN_ID: xsrf_token})
+        try:
+            request, response = function()
+            return return_function(request, response)
+        except HTTPException as http_error:
+            client_error = CTERAClientException()
+            client_error.__dict__ = http_error.__dict__.copy()
+            raise client_error
```

### Comparing `cterasdk-2.8.32/cterasdk/client/host.py` & `cterasdk-2.9.0/cterasdk/client/host.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import logging
 import socket
 
 from ..common import Object
 from ..convert import tojsonstr
 from ..exception import HostUnreachable
-from .cteraclient import CTERAClient, MigrationClient, RESTClient
+from .cteraclient import CTERAClient
 from ..exception import CTERAException
 
 
 def authenticated(function):
     @functools.wraps(function)
     def check_authenticated_and_call(self, *args, **kwargs):
         if self._is_authenticated(function, *args, **kwargs):  # pylint: disable=protected-access
@@ -63,57 +63,19 @@
 
     def __str__(self):
         x = Object()
         x.__dict__ = {k: v for k, v in self.__dict__.items() if not (k.startswith('_') or k in self._omit_fields)}
         return tojsonstr(x)
 
 
-class MigrationHost(NetworkHost):
-
-    def __init__(self, host, port, https, is_authenticated=None, http_client=None):
-        super().__init__(host, port, https)
-
-        def always_authenticated(self, function):  # pylint: disable=unused-argument
-            return True
-        self._is_authenticated = is_authenticated if is_authenticated else always_authenticated
-        self._client = MigrationClient(http_client) if http_client else RESTClient()
-
-    @staticmethod
-    def from_ctera_host(ctera_host):
-        """Create a RESTful host instance from an existing CTERA host instance"""
-        return MigrationHost(ctera_host.host(), ctera_host.port(), ctera_host.https(),
-                             ctera_host._is_authenticated, ctera_host._ctera_client.http_client)  # pylint: disable=protected-access
-
-    @authenticated
-    def login(self, path):
-        return self._client.login(self.baseurl(), path)
-
-    @authenticated
-    def get(self, path, params=None):
-        return self._client.get(self.baseurl(), path, params or {})
-
-    @authenticated
-    def put(self, path, value):
-        return self._client.put(self.baseurl(), path, value)
-
-    @authenticated
-    def post(self, path, value):
-        return self._client.post(self.baseurl(), path, value)
-
-    @authenticated
-    def delete(self, path):
-        return self._client.delete(self.baseurl(), path)
-
-
 class CTERAHost(NetworkHost):  # pylint: disable=too-many-public-methods
 
     def __init__(self, host, port, https):
         super().__init__(host, port, https)
         self._ctera_client = CTERAClient(self._session_id_key)
-        self._ctera_migrate = MigrationHost.from_ctera_host(self)
         self._session = None
 
     @property
     def _omit_fields(self):
         return super()._omit_fields + [
             'login',
             'logout'
@@ -148,17 +110,16 @@
         :param str password: User password
         """
         self._login_object.login(username, password)
         self._session.start_local_session(self)
 
     def logout(self):
         """ Log out """
-        if self._session.active:
-            self._login_object.logout()
-            self._session.terminate()
+        self._login_object.logout()
+        self._session.terminate()
 
     def session(self):
         return self._session
 
     def register_session(self, session):
         self._session = session
 
@@ -288,10 +249,10 @@
         self._session.local_auth = True  # pylint: disable=protected-access
         self._session.start_local_session(self)
 
     def whoami(self):
         """
         Return the name of the logged in user.
 
-        :return cterasdk.common.object.Object: The session object of the current user
+        :return str: The name of the logged in user
         """
         return self._session.whoami()
```

### Comparing `cterasdk-2.8.32/cterasdk/client/http.py` & `cterasdk-2.9.0/cterasdk/client/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 import urllib.parse
 import logging
-import time
 
 import requests
 import requests.exceptions as requests_exceptions
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 # from .ssl import CertificateServices
-from ..convert import fromxmlstr, ParseException
+from ..convert import fromxmlstr
 from ..common import Object, merge
 from .. import config
 from ..exception import SSLException, HostUnreachable, ExhaustedException
 from ..lib import ask
 
 
 class HTTPException(Exception):
 
     def __init__(self, http_error):
         super().__init__()
         self.response = Object()
         self.response.code = http_error.response.status_code
         self.response.reason = http_error.response.reason
-        try:
-            self.response.body = fromxmlstr(http_error.response.text)
-        except ParseException:
-            self.response.body = ''
+        self.response.body = fromxmlstr(http_error.response.text)
         if config.http['verbose']:
             self.response.headers = http_error.response.headers
             self.request = HTTPException._parse_request(http_error.request)
 
     @staticmethod
     def _parse_request(request):
         o = urllib.parse.urlparse(request.url)
@@ -74,15 +70,14 @@
         return baseurl + '/' + path
     raise ValueError("Invalid baseurl/path combination")
 
 
 class ContentType:
     urlencoded = {'Content-Type': 'application/x-www-form-urlencoded'}
     textplain = {'Content-Type': 'text/plain'}
-    application_json = {'Content-Type': 'application/json'}
 
 
 class HttpClientBase():
     def __init__(self, session_id_key):
         self.timeout = config.http['timeout']
         self.retries = config.http['retries']
         self.ssl_error_handling = config.http['ssl']
@@ -92,31 +87,25 @@
 
     def dispatch(self, ctera_request):
         attempt = 0
         while attempt < self.retries:
             try:
                 return self._do_dispatch(ctera_request)
             except requests_exceptions.HTTPError as error:
-                http_exception = HTTPException(error)
-                if http_exception.response.code != 504:
-                    raise http_exception
-                logging.getLogger().warning('Server timed out. %s', {'attempt': (attempt + 1)})
+                raise HTTPException(error)
             except requests_exceptions.Timeout:
                 self.on_timeout(attempt)
             except requests_exceptions.SSLError as error:
                 self.on_ssl_error(error.request)
                 attempt = -1
             except requests_exceptions.ConnectionError as error:
                 self._on_unreachable(error)
             except requests_exceptions.RequestException as error:
                 logging.getLogger().warning(error)
-
             attempt = attempt + 1
-            if attempt < self.retries:
-                time.sleep(self.timeout)
         logging.getLogger().error('Reached maximum number of retries. %s', {'retries': self.retries, 'timeout': self.timeout})
         raise ExhaustedException(self.retries, self.timeout)
 
     def _do_dispatch(self, ctera_request):
         response = self.session.request(ctera_request.method, ctera_request.url, **ctera_request.kwargs)
         response.raise_for_status()
         return (response.request, response)
```

### Comparing `cterasdk-2.8.32/cterasdk/client/ssl.py` & `cterasdk-2.9.0/cterasdk/client/ssl.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/common/datetime_utils.py` & `cterasdk-2.9.0/cterasdk/common/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/config.py` & `cterasdk-2.9.0/cterasdk/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import logging
 
 
-class Logging:  # pylint: disable=unused-private-member
+class Logging:
 
     __instance = None
 
     @staticmethod
     def get():
         if Logging.__instance is None:
             Logging()
@@ -66,16 +66,16 @@
     level=logging.INFO,
     fmt='%(asctime)s,%(msecs)3d %(levelname)7s [%(filename)s:%(lineno)d] [%(funcName)s] - %(message)s',
     df='%Y-%m-%d %H:%M:%S',
     filename=os.environ.get('CTERASDK_LOG_FILE')
 )
 
 http = dict(
-    timeout=10,  # http client or server timeout (seconds)
-    retries=3,  # handle client or server timeout
+    timeout=20,  # http client timeout (seconds)
+    retries=3,  # handle connection timeout
     ssl='Consent',  # ['Consent', 'Trust']
     verbose=False  # include request info on error
 )
 
 connect = dict(
     ssl='Consent'  # ['Consent', 'Trust']
 )
```

### Comparing `cterasdk-2.8.32/cterasdk/convert/format.py` & `cterasdk-2.9.0/cterasdk/convert/format.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import queue
 import json
 import copy
 from xml.etree.ElementTree import Element, SubElement, tostring
 from xml.dom import minidom
 
-from cterasdk.common import Item, Object, Device
+from cterasdk.common import Item, Object
 from cterasdk.convert.xml_types import XMLTypes
 
 
 _sdk_hidden = [
     'password',
     'awsSecretKey',
     'sharedSecret',
@@ -16,16 +16,15 @@
     'encPassphrase',
     'encryptedFolderKey',
     'oldPassword',
     'newPassword',
     'secretkey',
     'activationCode',
     'masterPassword',
-    'masterKey',
-    'secretAccess'
+    'masterKey'
 ]
 
 
 def _to_protected_dict(o):
     ret = copy.deepcopy(o.__dict__)
     for key in _sdk_hidden:
         if key in ret:
@@ -60,18 +59,18 @@
     """
     if obj is None:
         return None
     xml = toxml(obj)
     if pretty_print:
         string = minidom.parseString(tostring(xml)).toprettyxml(indent="   ")
         return ''.join(string.split('\n', 1)[1:])
-    return tostring(xml, 'utf-8')
+    return tostring(xml)
 
 
-def toxml(obj):  # pylint: disable=too-many-branches
+def toxml(obj):
     root = Item()
     root.node = None
     root.parent = None
     root.obj = obj
 
     q = queue.Queue()
     q.put(root)
@@ -87,31 +86,14 @@
             item.node = CreateElement(item.parent, XMLTypes.LIST)
             for member in item.obj:
                 kid = Item()
                 kid.node = None
                 kid.parent = item.node
                 kid.obj = member
                 q.put(kid)
-        elif isinstance(item.obj, Device):  # db.xml
-            item.node = CreateElement(item.parent, XMLTypes.DB)
-            for key, value in [
-                (XMLTypes.NS, item.obj.namespace),
-                (XMLTypes.LOCATION, item.obj.location),
-                (XMLTypes.ID, item.obj.id),
-                (XMLTypes.VERSION, item.obj.version),
-                (XMLTypes.FIRMWARE, item.obj.firmware)
-            ]:
-                if value is not None:
-                    item.node.set(key, value)
-
-            kid = Item()
-            kid.node = None
-            kid.parent = item.node
-            kid.obj = item.obj.config
-            q.put(kid)
         elif isinstance(item.obj, Object):
             item.node = CreateElement(item.parent, XMLTypes.OBJ)
             classname = item.obj.__dict__.get('_classname')  # Convert { "_classname" : "ShareConfig" }
             if classname is not None:
                 item.node.set(XMLTypes.CLASS, classname)
             uuid = item.obj.__dict__.get('_uuid')  # Convert { "_uuid" : "6f0e8c79-..." }
             if uuid is not None:
```

### Comparing `cterasdk-2.8.32/cterasdk/convert/parse.py` & `cterasdk-2.9.0/cterasdk/convert/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import json
 import queue
 from xml.etree.ElementTree import fromstring, ParseError
 
 from cterasdk.convert.xml_types import XMLTypes
 from .exception import ParseException
-from ..common import Item, Object, Device
+from ..common import Item, Object
 
 
 def ParseValue(data):
     if not data:
         return data
 
     try:
@@ -141,22 +141,9 @@
                         kid = Item()
                         kid.id = item.id
                         kid.parent = item.parent
                         kid.node = kidnode
                         q.put(kid)
             else:
                 SetAppendValue(item, None)              # include empty attrs
-        elif item.node.tag == XMLTypes.DB:              # db.xml
-            item.value = Device(
-                item.node.attrib.get(XMLTypes.ID),
-                item.node.attrib.get(XMLTypes.VERSION),
-                item.node.attrib.get(XMLTypes.FIRMWARE)
-            )
-            SetAppendValue(item, item.value)
-
-            kid = Item()
-            kid.id = item.node.attrib.get(XMLTypes.ID)
-            kid.parent = item
-            kid.node = list(item.node)[0]
-            q.put(kid)
 
     return root.value
```

### Comparing `cterasdk-2.8.32/cterasdk/core/activation.py` & `cterasdk-2.9.0/cterasdk/core/activation.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/admins.py` & `cterasdk-2.9.0/cterasdk/core/portals.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,161 @@
 import logging
 
+from ..exception import CTERAException
 from .base_command import BaseCommand
-from ..exception import CTERAException, ObjectNotFoundException
-from ..common import Object, DateTimeUtils
+from ..lib import Iterator, Command
+from ..common import Object
 from ..common import union
+from . import enum
 from . import query
 
 
-class Administrators(BaseCommand):
+class Portals(BaseCommand):
     """
-    Portal Global Administrators User Management APIs
+    Global Admin Portals APIs
     """
 
     default = ['name']
 
-    def _get_entire_object(self, name):
-        ref = f'/administrators/{name}'
-        try:
-            return self._portal.get(ref)
-        except CTERAException as error:
-            raise CTERAException('Failed to get the user', error)
-
     def get(self, name, include=None):
         """
-        Get a Global Administrator user account
+        Get a tenant
 
-        :param str name: Global administrator username
+        :param str name: Name of the tenant
         :param list[str] include: List of fields to retrieve, defaults to ['name']
-        :return: The user account, including the requested fields
         """
-        baseurl = f'/administrators/{name}'
-        include = union(include or [], Administrators.default)
+        include = union(include or [], Portals.default)
         include = ['/' + attr for attr in include]
-        user_object = self._portal.get_multi(baseurl, include)
-        if user_object.name is None:
-            raise ObjectNotFoundException('Could not find user', baseurl, username=name)
-        return user_object
+        tenant = self._portal.get_multi('/portals/' + name, include)
+        if tenant.name is None:
+            raise CTERAException('Could not find tenant', None, name=name)
+        return tenant
 
-    def list_admins(self, include=None):
+    def list_tenants(self, include=None, portal_type=None):
         """
-        List local administrators
+        List tenants.\n
+        To retrieve tenants, you must first browse the Global Administration Portal, using: `GlobalAdmin.portals.browse_global_admin()`
 
-        :param list[str] include: List of fields to retrieve, defaults to ['name']
-        :return: Iterator for local administrators
-        :rtype: cterasdk.lib.iterator.Iterator
+        :param list[str],optional include: List of fields to retrieve, defaults to ['name']
+        :param cterasdk.core.enum.PortalType portal_type: The Portal type
         """
-        include = union(include or [], Administrators.default)
+        # browse administration
+        include = union(include or [], Portals.default)
         param = query.QueryParamBuilder().include(include).build()
-        return query.iterator(self._portal, '/administrators', param)
-
-    def add(self, name, email, first_name, last_name, password, role, company=None, comment=None, password_change=False):
+        baseurl = '/portals'
+        if portal_type == enum.PortalType.Team:
+            baseurl = '/teamPortals'
+        elif portal_type == enum.PortalType.Reseller:
+            baseurl = '/resellerPortals'
+        return query.iterator(self._portal, baseurl, param)
+
+    def _query_portals(self, param):
+        response = self._portal.execute('', 'getPortalsDisplayInfo', param)
+        return (response.hasMore, response.objects)
+
+    def tenants(self, include_deleted=False):
+        """
+        Get all tenants
+
+        :param bool,optional include_deleted: Include deleted tenants, defaults to False
+        """
+        # Check if current session is global admin
+        param = query.QueryParamBuilder().include_classname().put('isTrashcan', include_deleted).build()
+        function = Command(self._query_portals)
+        return Iterator(function, param)
+
+    def add(self, name, display_name=None, billing_id=None, company=None, plan=None, comment=None):
+        """
+        Add a new tenant
+
+        :param str name: Name of the new tenant
+        :param str,optional display_name: Display Name of the new tenant, defaults to None
+        :param str,optional billing_id: Billing ID of the new tenant, defaults to None
+        :param str,optional company: Company Name of the new tenant, defaults to None
+        :param str,optional plan: Subscription plan name to assign to the new tenant, defaults to None
+        :param str,optional comment: Assign a comment to the new tenant, defaults to None
+        :return str: A relative url path to the Team Portal
         """
-        Create a Global Administrator
 
-        :param str name: User name for the new GlobalAdmin
-        :param str email: E-mail address of the new GlobalAdmin
-        :param str first_name: The first name of the new GlobalAdmin
-        :param str last_name: The last name of the new GlobalAdmin
-        :param str password: Password for the new GlobalAdmin
-        :param cterasdk.core.enum.Role role: User role of the new GlobalAdmin
-        :param str,optional company: The name of the company of the new GlobalAdmin, defaults to None
-        :param str,optional comment: Additional comment for the new GlobalAdmin, defaults to None
-        :param variable,optional password_change:
-            Require the user to change the password on the first login.
-            Pass datetime.date for a specific date, integer for days from creation, or True for immediate , defaults to False
-        """
         param = Object()
-        param._classname = "PortalAdmin"  # pylint: disable=protected-access
+        if plan:
+            param.plan = self._portal.plans.get(plan, include=['baseObjectRef']).baseObjectRef
+        param._classname = 'TeamPortal'  # pylint: disable=protected-access
         param.name = name
-        param.email = email
-        param.firstName = first_name
-        param.lastName = last_name
-        param.password = password
-        param.role = role
-        param.company = company
+        param.displayName = display_name
+        param.externalPortalId = billing_id
+        param.companyName = company
         param.comment = comment
-        if password_change:
-            param.requirePasswordChangeOn = DateTimeUtils.get_expiration_date(password_change).strftime('%Y-%m-%d')
 
-        logging.getLogger().info('Creating a global administrator. %s', {'user': name})
-        response = self._portal.add('/administrators', param)
-        logging.getLogger().info('Global administrator created. %s', {'user': name, 'email': email, 'role': role})
+        logging.getLogger().info('Creating Team Portal. %s', {'name': name})
+
+        response = self._portal.add('/teamPortals', param)
+
+        logging.getLogger().info('Team Portal created. %s', {'name': name})
 
         return response
 
-    def modify(self, current_username, new_username=None, email=None, first_name=None,
-               last_name=None, password=None, role=None, company=None, comment=None):
+    def subscribe(self, tenant, plan):
         """
-        Modify a Global Administrator user account
+        Subscribe a tenant to a plan
 
-        :param str current_username: The current GlobalAdmin username
-        :param str,optional new_username: New name
-        :param str,optional email: E-mail address
-        :param str,optional first_name: First name
-        :param str,optional last_name: Last name
-        :param str,optional password: Password
-        :param cterasdk.core.enum.Role,optional role: User role
-        :param str,optional company: Company name
-        :param str,optional comment: Comment
-        """
-        user = self._get_entire_object(current_username)
-        if new_username:
-            user.name = new_username
-        if email:
-            user.email = email
-        if first_name:
-            user.firstName = first_name
-        if last_name:
-            user.lastName = last_name
-        if password:
-            user.password = password
-        if role:
-            user.role = role
-        if company is not None:
-            user.company = company
-        if comment is not None:
-            user.comment = comment
-
-        try:
-            response = self._portal.put('/administrators/' + current_username, user)
-            logging.getLogger().info("User modified. %s", {'username': user.name})
-            return response
-        except CTERAException as error:
-            logging.getLogger().error("Failed to modify user.")
-            raise CTERAException('Failed to modify user', error)
+        :param str name: Name of the tenant
+        :param str,plan: Name of the subscription plan
+        """
+        return self._portal.execute('/portals/' + tenant, 'subscribe', plan)
 
     def delete(self, name):
         """
-        Delete a Global Administrator
+        Delete an existing tenant
 
-        :param str username: Global administrator username
+        :param str name: Name of the tenant to delete
         """
-        logging.getLogger().info('Deleting user. %s', {'user': name})
-        baseurl = f'/administrators/{name}'
-        response = self._portal.execute(baseurl, 'delete', True)
-        logging.getLogger().info('User deleted. %s', {'user': name})
+        logging.getLogger().info('Deleting Portal. %s', {'name': name})
+
+        response = self._portal.execute('/teamPortals/' + name, 'delete')
+
+        logging.getLogger().info('Portal deleted. %s', {'name': name})
 
         return response
+
+    def undelete(self, name):
+        """
+        Undelete a previously deleted tenant
+
+        :param str name: Name of the tenant to undelete
+        """
+        logging.getLogger().info('Recovering Portal. %s', {'name': name})
+
+        response = self._portal.execute('/teamPortals/' + name, 'moveFromTrashcan')
+
+        logging.getLogger().info('Portal recovered. %s', {'name': name})
+
+        return response
+
+    def browse(self, tenant):
+        """
+        Browse a tenant
+
+        :param str tenant: Name of the tenant to browse
+        """
+        self._portal.put('/currentPortal', tenant)
+
+    def browse_global_admin(self):
+        """
+        Browse the Global Admin
+        """
+        self.browse('')
+
+    def apply_changes(self, wait=False):
+        """
+        Apply provisioning changes.\n
+
+        :param bool,optional wait: Wait for all changes to apply
+        """
+        param = Object()
+        param.objectId = None
+        param.type = 'portals'
+        logging.getLogger().info('Applying provisioning changes.')
+        task = self._portal.execute('', 'updatePortals', param)
+        if wait:
+            task = self._portal.tasks.wait(task)
+        return task
```

### Comparing `cterasdk-2.8.32/cterasdk/core/antivirus.py` & `cterasdk-2.9.0/cterasdk/core/antivirus.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .enum import ICAPServices
 from .base_command import BaseCommand
 
 
 class Antivirus(BaseCommand):
     """
     Portal Antivirus APIs
-
-    :ivar cterasdk.core.antivirus.AntivirusServers servers: Object holding the Portal antivirus server APIs
     """
 
     default = ['name', 'type']
 
     def __init__(self, portal):
         super().__init__(portal)
         self.servers = AntivirusServers(self._portal)
@@ -66,15 +64,15 @@
 
     def get(self, name):
         """
         Get an antivirus server's configuration
 
         :param str name: Server name
         """
-        return self._portal.get(f'/antiviruses/{name}')
+        return self._portal.get('/antiviruses/%s' % name)
 
     def add(self, name, vendor, url, connection_timeout=5):
         """
         Add an antivirus server
 
         :param str name: Server name
         :param cterasdk.core.enum.AntivirusType vendor: Server type
@@ -92,24 +90,24 @@
         logging.getLogger().info("Added antivirus server. %s", {'name': name, 'type': vendor, 'url': url})
         return response
 
     def delete(self, name):
         """
         Remove an antivirus server
         """
-        return self._portal.delete(f'/antiviruses/{name}')
+        return self._portal.delete('/antiviruses/%s' % name)
 
     def suspend(self, name):
         """
         Suspend an antivirus server
         """
         logging.getLogger().info("Suspending antivirus server. %s", {'name': name})
-        self._portal.put(f'/antiviruses/{name}/enabled', False)
+        self._portal.put('/antiviruses/%s/enabled' % name, False)
         logging.getLogger().info("Suspended antivirus server. %s", {'name': name})
 
     def unsuspend(self, name):
         """
         Unsuspend antivirus scanning
         """
         logging.getLogger().info("Unsuspending antivirus server. %s", {'name': name})
-        self._portal.put(f'/antiviruses/{name}/enabled', True)
+        self._portal.put('/antiviruses/%s/enabled' % name, True)
         logging.getLogger().info("Unsuspended antivirus server. %s", {'name': name})
```

### Comparing `cterasdk-2.8.32/cterasdk/core/cli.py` & `cterasdk-2.9.0/cterasdk/edge/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
 
 from .base_command import BaseCommand
 
 
 class CLI(BaseCommand):
-    """ Portal CLI APIs """
+    """ Gateway CLI APIs """
 
     def run_command(self, cli_command):
         """
         Run a CLI command
 
         :param str cli_command: The CLI command to run on the gateway
-        :return str: The response of the Portal
+        :return str: The response of the gateway
         """
         logging.getLogger().info("Executing CLI command. %s", {'cli_command': cli_command})
-        response = self._portal.execute('', 'debugCmd', cli_command)
+
+        response = self._gateway.execute('/config/device', 'debugCmd', cli_command)
+
         logging.getLogger().info("CLI command executed. %s", {'cli_command': cli_command})
+
         return response
```

### Comparing `cterasdk-2.8.32/cterasdk/core/cloudfs.py` & `cterasdk-2.9.0/cterasdk/core/cloudfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from .base_command import BaseCommand
 from . import query
 from .enum import ListFilter
 from ..common import Object
 from ..common import union
-from ..exception import CTERAException, ObjectNotFoundException
+from ..exception import CTERAException
 
 
 class CloudFS(BaseCommand):
     """ CloudFS APIs """
 
     default = ['name', 'group', 'owner']
 
@@ -20,15 +20,15 @@
         :param str name: Name of the Folder Group to find
         :param str,optional include: List of fields to retrieve, defaults to ['name', 'owner']
         """
         include = union(include or [], ['name', 'owner'])
         include = ['/' + attr for attr in include]
         folder_group = self._portal.get_multi('/foldersGroups/' + name, include)
         if folder_group.name is None:
-            raise ObjectNotFoundException('Could not find folder group', f'/foldersGroups/{name}', name=name)
+            raise CTERAException('Could not find folder group', None, name=name)
         return folder_group
 
     def list_folder_groups(self, include=None, user=None):
         """
         List folder groups
 
         :param str,optional include: List of fields to retrieve, defaults to ['name', 'owner']
@@ -39,39 +39,34 @@
         builder = query.QueryParamBuilder().include(include)
         if user:
             uid = self._portal.users.get(user, ['uid']).uid
             builder.ownedBy(uid)
         param = builder.build()
         return query.iterator(self._portal, '/foldersGroups', param)
 
-    def mkfg(self, name, user=None, deduplication_method_type=None, storage_class=None):
+    def mkfg(self, name, user=None):
         """
         Create a new Folder Group
 
         :param str name: Name of the new folder group
         :param cterasdk.core.types.UserAccount user:
          User account, the user directory and name of the new folder group owner (default to None)
-        :param cterasdk.core.enum.DeduplicationMethodType deduplication_method_type: Deduplication-Method
-        :param str,optional storage_class: Storage class, defaults to the Default storage class
         """
 
         param = Object()
         param.name = name
         param.disabled = True
         param.owner = self._portal.users.get(user, ['baseObjectRef']).baseObjectRef if user is not None else None
-        param.deduplicationMethodType = deduplication_method_type
-        if storage_class:
-            param.storageClass = self._portal.storage_classes.get(storage_class).baseObjectRef
 
         try:
             response = self._portal.execute('', 'createFolderGroup', param)
             logging.getLogger().info('Folder group created. %s', {'name': name, 'owner': param.owner})
             return response
         except CTERAException as error:
-            logging.getLogger().error('Folder group creation failed. %s', {'name': name, 'owner': str(user)})
+            logging.getLogger().error('Folder group creation failed. %s', {'name': name, 'owner': user})
             raise error
 
     def rmfg(self, name):
         """
         Remove a Folder Group
 
         :param str name: Name of the folder group to remove
@@ -158,75 +153,32 @@
                 builder.addFilter(query_filter)
         if user:
             uid = self._portal.users.get(user, ['uid']).uid
             builder.ownedBy(uid)
         param = builder.build()
         return query.iterator(self._portal, '/cloudDrives', param)
 
-    def find(self, name, owner, include=None):
+    def find(self, name, owner, include):
         """
-        Find a Cloud Drive Folder
+        Find a  Cloud Drive Folder
 
         :param str name: Name of the Cloud Drive Folder to find
-        :param cterasdk.core.types.UserAccount owner: User account of the folder group owner
+        :param str owner: User name of the owner of the directory
         :param list[str] include: List of metadata fields to include in the response
-
-        :returns: A Cloud Drive Folder
         """
-
-        uid = self._portal.users.get(owner, ['uid']).uid
-        include = union(include or [], CloudFS.default)
-        builder = query.QueryParamBuilder().include(include).ownedBy(uid)
-        builder.addFilter(query.FilterBuilder('name').eq(name))
+        builder = query.QueryParamBuilder().include(include)
+        query_filter = query.FilterBuilder('name').eq(name)
+        builder.addFilter(query_filter)
         param = builder.build()
 
         iterator = query.iterator(self._portal, '/cloudDrives', param)
-        try:
-            return next(iterator)
-        except StopIteration:
-            logging.getLogger().info('Could not find cloud folder. %s', {'folder': name, 'owner': str(owner)})
-            raise CTERAException('Could not find cloud folder', None, folder=name, owner=str(owner))
+        for cloud_folder in iterator:
+            if cloud_folder.owner.endswith(owner):
+                return cloud_folder
+
+        logging.getLogger().info('Could not find cloud folder. %s', {'folder': name, 'owner': owner})
+        raise CTERAException('Could not find cloud folder', None, folder=name, owner=owner)
 
     def _dirpath(self, name, owner):
         owner = self._portal.users.get(owner, ['displayName']).displayName
         path = owner + '/' + name
         return path
-
-    def set_folders_acl(self, folders_path, sddl_string, is_recursive=False):
-        """
-        Changing the file or Folder ACLs
-
-        :param list folders_path: A list of paths
-        :param str sddl_string: The SDDL string with the ACL permissions
-        :param bool is_recursive: For path that is not a file but a folder
-        :return: execution response
-        """
-        param = Object()
-        param._classname = 'SDDLFoldersParam'  # pylint: disable=protected-access
-        param.foldersPath = folders_path
-        param.sddlString = sddl_string
-        param.isRecursive = is_recursive
-        try:
-            return self._portal.execute('', 'setFoldersACL', param)
-        except CTERAException as error:
-            logging.getLogger().error('setFoldersACL failed. %s', {'error': error})
-            raise CTERAException('Failed to setFoldersACL', error)
-
-    def set_owner_acl(self, folders_path, owner_sid, is_recursive=False):
-        """
-        Changing the File or Folder Owner SID or ACLs
-
-        :param list folders_path:  A list of paths
-        :param str owner_sid: The SID string that identifies the object's owner.
-        :param bool is_recursive: If the path is not a file but a folder
-        :return: execution response
-        """
-        param = Object()
-        param._classname = 'OwnerSidFoldersParam'  # pylint: disable=protected-access
-        param.foldersPath = folders_path
-        param.ownerSid = owner_sid
-        param.isRecursive = is_recursive
-        try:
-            return self._portal.execute('', 'setOwnerACL', param)
-        except CTERAException as error:
-            logging.getLogger().error('setOwnerACL failed. %s', {'error': error})
-            raise CTERAException('Failed to setOwnerACL', error)
```

### Comparing `cterasdk-2.8.32/cterasdk/core/decorator.py` & `cterasdk-2.9.0/cterasdk/core/decorator.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/devices.py` & `cterasdk-2.9.0/cterasdk/core/devices.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from .base_command import BaseCommand
 from .enum import DeviceType
 from . import remote, query
 from ..common import union
-from ..exception import CTERAException, ObjectNotFoundException
+from ..exception import CTERAException
 
 
 class Devices(BaseCommand):
     """ Portal Devices APIs """
 
     name_attr = 'name'
     type_attr = 'deviceType'
     default = ['name', 'portal', 'deviceType']
 
-    def _create_device_resource_uri(self, device_name, tenant):
-        session = self._portal.session()
-        if not tenant:
-            if not session.in_tenant_context():
-                raise CTERAException('You must specify a tenant name or browse the tenant first.')
-            tenant = self._portal.session().tenant()
-        if session.is_local_auth():
-            resource_uri = '/devices/' + device_name  # local auth: auto appends /portals/{tenant_name}
-        else:
-            resource_uri = f'/portals/{tenant}/devices/{device_name}'  # regular auth: support both tenant and Administration context
-        return resource_uri
-
     def device(self, device_name, tenant=None, include=None):
         """
         Get a Device by its name
 
         :param str device_name: Name of the device to retrieve
         :param str,optional tenant: Tenant of the device, defaults to the tenant in the current session
         :param list[str],optional include: List of fields to retrieve, defaults to ['name', 'portal', 'deviceType']
 
         :return: Managed Device
         :rtype: ctera.object.Gateway.Gateway or ctera.object.Agent.Agent
         """
         include = union(include or [], Devices.default)
         include = ['/' + attr for attr in include]
 
-        resource_uri = self._create_device_resource_uri(device_name, tenant)
+        session = self._portal.session()
+        if not tenant:
+            if not session.in_tenant_context():
+                raise CTERAException('You must specify a tenant name or browse the tenant first.')
+            tenant = self._portal.session().tenant()
+        if session.is_local_auth():
+            url = '/devices/' + device_name  # local auth: auto appends /portals/{tenant_name}
+        else:
+            url = '/portals/%s/devices/%s' % (tenant, device_name)  # regular auth: support both tenant and Administration context
 
-        dev = self._portal.get_multi(resource_uri, include)
+        dev = self._portal.get_multi(url, include)
         if dev.name is None:
-            raise ObjectNotFoundException('Device not found', resource_uri, tenant=tenant, name=device_name)
+            raise CTERAException('Device not found', None, tenant=tenant, device=device_name)
 
         return remote.remote_command(self._portal, dev)
 
     def filers(self, include=None, allPortals=False, deviceTypes=None):
         """
         Get Filers
 
@@ -139,26 +135,7 @@
             builder.ownedBy(uid)
         builder.orFilter((len(filters) > 1))
         param = builder.build()
         # Check if the _all attribute conflicts with the current tenant
         iterator = query.iterator(self._portal, '/devices', param)
         for dev in iterator:
             yield remote.remote_command(self._portal, dev)
-
-    def get_comment(self, device_name, tenant=None):
-        """
-        Get Portal device comment
-
-        :param str device: Device name
-        :returns: Comment
-        :rtype: str
-        """
-        return self._portal.get(f'{self._create_device_resource_uri(device_name, tenant)}/comment')
-
-    def set_comment(self, device_name, comment, tenant=None):
-        """
-        Set a comment to a Portal device
-
-        :param str device: Device name
-        :param str comment: Comment
-        """
-        return self._portal.put(f'{self._create_device_resource_uri(device_name, tenant)}/comment', comment)
```

### Comparing `cterasdk-2.8.32/cterasdk/core/directoryservice.py` & `cterasdk-2.9.0/cterasdk/edge/shares.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,276 +1,297 @@
 import logging
 
-from .base_command import BaseCommand
+from . import enum
+from .files import path
 from ..common import Object
-from ..exception import CTERAException
-from .enum import PortalAccountType, SearchType, DirectoryServiceType, DirectoryServiceFetchMode, Role, DirectorySearchEntityType
-from .types import AccessControlEntry, AccessControlRule, UserAccount, GroupAccount
-
-
-class DirectoryService(BaseCommand):
-    """
-    Portal Active Directory APIs
-    """
-
-    def _get_configuration(self):
-        return self._portal.get('/directoryConnector')
-
-    def connected(self):
-        directory_services_config = self._get_configuration()
-        if directory_services_config is None:
-            return False
-        try:
-            self._connect_to_directory_services(directory_services_config)
-            return True
-        except CTERAException:
-            return False
-
-    # pylint: disable=too-many-arguments
-    def connect(self, domain, username, password, directory=DirectoryServiceType.Microsoft,
-                domain_controllers=None, ou=None, ssl=False, krb=False, mapping=None, acl=None,
-                default=Role.Disabled, fetch=DirectoryServiceFetchMode.Lazy):
-        """
-        Connect a Portal tenant to directory services
-
-        :param str domain: The directory services domain to connect to
-        :param str username: The user name to use when connecting to the active directory services
-        :param str password: The password to use when connecting to the active directory services
-        :param str,optional ou: The OU path to use when connecting to the active directory services, defaults to `None`
-        :param cterasdk.core.enum.DirectoryServiceType,optional directory: The directory service type, deafults to `'ActiveDirectory'`
-        :param cterasdk.core.types.DomainControllers,optional domain_controllers:
-            Connect to a primary and a secondary domain controllers, defaults to `None`
-        :param bool,optional ssl: Connect using SSL, defaults to `False`
-        :param bool,optional krb: Connect using Kerberos, defaults to `False`
-        :param list[cterasdk.common.types.ADDomainIDMapping],optional: The directory services UID/GID mapping
-        :param list[cterasdk.core.types.AccessControlEntry],optional acl: List of access control entries and their associated roles
-        :param cterasdk.core.enum.Role default: Default role if no match applies, defaults to `None`
-        :param str,optional fetch: Configure identity fetching mode, defaults to `'Lazy'`
-        """
-        param = Object()
-        param._classname = 'ActiveDirectory'  # pylint: disable=protected-access
-        param.type = directory
-        param.domain = domain
-        param.useKerberos = krb
-        param.useSSL = ssl
-        param.username = username
-        param.password = password
-        param.ou = ou
-        param.noMatchRole = default
-        param.accessControlRules = None
-        param.idMapping = None
-        param.fetchMode = fetch
-        param.ipAddresses = None
-
-        if domain_controllers:
-            param.ipAddresses = Object()
-            param.ipAddresses._classname = 'DomainControlIPAddresses'  # pylint: disable=protected-access
-            param.ipAddresses.ipAddress1 = domain_controllers.primary
-            param.ipAddresses.ipAddress2 = domain_controllers.secondary
-
-        tenant = self._portal.session().user.tenant
-        logging.getLogger().info('Connecting Portal to directory services. %s', {
-            'tenant': tenant,
-            'type': type,
-            'domain': domain
-        })
-        self._connect_to_directory_services(param)
-        logging.getLogger().info('Connected Portal to directory services. %s', {'tennat': tenant, 'domain': domain})
-
-        if mapping:
-            self._configure_advanced_mapping(mapping)
-
-        if acl:
-            self._configure_access_control(acl, default)
-
-    def _connect_to_directory_services(self, param):
-        return self._portal.execute('', 'testAndSaveAD', param)
+from ..exception import CTERAException, InputError
+from .base_command import BaseCommand
+from .types import ShareAccessControlEntry, RemoveShareAccessControlEntry
 
-    def get_advanced_mapping(self):
-        """
-        Retrieve directory services advanced mapping configuration
 
-        :returns: A dictionary of domain mapping objects
-        :rtype: dict
-        """
-        return {map.domainFlatName: map for map in self._portal.get('/directoryConnector/idMapping/map')}
+class Shares(BaseCommand):
 
-    def set_advanced_mapping(self, mapping):
+    def get(self, name=None):
         """
-        Configure advanced mapping
-
-        :param list[cterasdk.common.types.ADDomainIDMapping] mapping: List of domains and their UID/GID mapping range
+        Get Share. If a share name was not passed as an argument, a list of all shares will be retrieved
+        :param str,optional name: Name of the share
+        """
+        return self._gateway.get('/config/fileservices/share' + ('' if name is None else ('/' + name)))
+
+    def add(self,
+            name,
+            directory,
+            acl=None,
+            access=enum.Acl.WindowsNT,
+            csc=enum.ClientSideCaching.Manual,
+            dir_permissions=777,
+            comment=None,
+            export_to_afp=False,
+            export_to_ftp=False,
+            export_to_nfs=False,
+            export_to_pc_agent=False,
+            export_to_rsync=False,
+            indexed=False,
+            trusted_nfs_clients=None
+            ):  # pylint: disable=too-many-arguments,too-many-locals,unused-argument
+        """
+        Add a network share.
+
+        :param str name: The share name
+        :param str directory: Full directory path
+        :param list[cterasdk.edge.types.ShareAccessControlEntry] acl: List of access control entries
+        :param cterasdk.edge.enum.Acl access: The Windows File Sharing authentication mode, defaults to ``winAclMode``
+        :param cterasdk.edge.enum.ClientSideCaching csc: The client side caching (offline files) configuration, defaults to ``manual``
+        :param int dir_permissions: Directory Permission, defaults to 777
+        :param str comment: Comment
+        :param bool export_to_afp: Whether to enable AFP access, defaults to ``False``
+        :param bool export_to_ftp: Whether to enable FTP access, defaults to ``False``
+        :param bool export_to_nfs: Whether to enable NFS access, defaults to ``False``
+        :param bool export_to_pc_agent: Whether to allow as a destination share for CTERA Backup Agents, defaults to ``False``
+        :param bool export_to_rsync: Whether to enable access over rsync, defaults to ``False``
+        :param bool indexed: Whether to enable indexing for search, defaults to ``False``
+        :param list[cterasdk.edge.types.NFSv3AccessControlEntry] trusted_nfs_clients: Trusted NFS v3 clients, defaults to ``None``
         """
-        if self._get_configuration() is None:
-            raise CTERAException('Failed to apply mapping. Not connected to directory services.')
+        acl = acl or []
 
-        return self._configure_advanced_mapping(mapping)
-
-    def _configure_advanced_mapping(self, mapping):
         param = Object()
-        param._classname = 'ADIDMapping'  # pylint: disable=protected-access
-        param.map = mapping
-        logging.getLogger().debug('Updating advanced mapping. %s', {
-            'domains': [mapping.domainFlatName for mapping in param.map]
-        })
-        response = self._portal.put('/directoryConnector/idMapping', param)
-        logging.getLogger().info('Updated advanced mapping.')
-        return response
-
-    def get_access_control(self):
-        """
-        Retrieve directory services access control list
-
-        :returns: List of access control entries
-        :rtype: list[cterasdk.core.types.AccessControlEntry]
-        """
-        acl = []
-        for ace in self._portal.get('/directoryConnector/accessControlRules'):
-            if ace.group.type == DirectorySearchEntityType.User:
-                acl.append(AccessControlEntry(UserAccount(ace.group.name, ace.group.domain), ace.role))
-            elif ace.group.type == DirectorySearchEntityType.Group:
-                acl.append(AccessControlEntry(GroupAccount(ace.group.name, ace.group.domain), ace.role))
-        return acl
-
-    def set_access_control(self, acl=None, default=None):
-        """
-        Configure directory services access control
-
-        :param list[cterasdk.core.types.AccessControlEntry],optional acl:
-            List of access control entries and their associated roles
-        :param cterasdk.core.enum.Role default: Default role if no match applies, defaults to `None`
-        """
-        directory_services_config = self._get_configuration()
-        if directory_services_config is None:
-            raise CTERAException('Failed to apply access control. Not connected to directory services.')
-
-        default = default if default is not None else directory_services_config.noMatchRole
-        return self._configure_access_control(acl, default)
-
-    def _configure_access_control(self, acl, default=None):
-
-        access_control_rules = []
-        for ace in acl:
-            account = None
-            if ace.account.account_type == PortalAccountType.User:
-                account = self._search_users(ace.account.directory, ace.account.name)
-            elif ace.account.account_type == PortalAccountType.Group:
-                account = self._search_groups(ace.account.directory, ace.account.name)
-            access_control_rules.append(AccessControlRule(account, ace.role))
-
-        logging.getLogger().info('Updating access control rules.')
-        response = self._portal.put('/directoryConnector/accessControlRules', access_control_rules)
-        logging.getLogger().info('Updated access control rules.')
-
-        if default is not None:
-            logging.getLogger().info('Updating default role.')
-            response = self._portal.put('/directoryConnector/noMatchRole', default)
-            logging.getLogger().info('Updated default role')
-
-        return response
-
-    def get_default_role(self):
-        """
-        Retrieve the default role assigned when no access control entry match was found
-        """
-        return self._portal.get('/directoryConnector/noMatchRole')
+        param.name = name
 
-    def get_connected_domain(self):
-        """
-        Get the connected domain information. Returns `None` if the Portal tenant is not connected to a domain
+        parts = path.CTERAPath(directory, '/').parts()
+        volume = parts[0]
+        self._validate_root_directory(volume)
+        param.volume = volume
+
+        directory = '/'.join(parts[1:])
+        param.directory = directory
+
+        param.access = access
+        param.clientSideCaching = csc
+        param.dirPermissions = dir_permissions
+        param.exportToAFP = export_to_afp
+        param.exportToFTP = export_to_ftp
+        param.exportToNFS = export_to_nfs
+        param.exportToPCAgent = export_to_pc_agent
+        param.exportToRSync = export_to_rsync
+        param.indexed = indexed
+        param.comment = comment
+        Shares._validate_acl(acl)
+        param.acl = [acl_entry.to_server_object() for acl_entry in acl]
+        param.trustedNFSClients = [client.to_server_object() for client in (trusted_nfs_clients or [])]
 
-        :return str: The connected domain
-        """
-        domain = None
         try:
-            domain = self._portal.get('/directoryConnector/domain')
-        except CTERAException:
-            pass
-        return domain
-
-    def domains(self):
-        """
-        Get domains
+            self._gateway.add('/config/fileservices/share', param)
+            logging.getLogger().info("Share created. %s", {'name': name})
+        except Exception as error:
+            logging.getLogger().error("Share creation failed.")
+            raise CTERAException('Share creation failed', error)
+
+    def set_share_winacls(self, name):
+        """
+        Set a network share to use Windows ACL Emulation Mode
+
+        :param str name: The share name
+        """
+        logging.getLogger().error("Updating Windows file sharing access mode. %s", {'share': name, 'access': enum.Acl.WindowsNT})
+        self._gateway.put('/config/fileservices/share/' + name + '/access', enum.Acl.WindowsNT)
+
+    def block_files(self, name, extensions):
+        """
+        Configure a share to block one or more file extensions
+
+        :param str name: The share name
+        :param list[str] extensions: List of file extensions to block
+        """
+        share = self.get(name)
+        if share.access != enum.Acl.WindowsNT:
+            raise CTERAException('Cannot block file types on non Windows-ACL enabled shares', None, share=share.name, access=share.access)
+        logging.getLogger().error("Updating the list of blocked file extensions. %s",
+                                  {'share': name, 'extensions': extensions, 'access': enum.Acl.WindowsNT})
+        self._gateway.put('/config/fileservices/share/' + share.name + '/screenedFileTypes', extensions)
+
+    def set_acl(self, name, acl):
+        """
+        Set a network share's access control entries.
+
+        :param str name: The share name
+        :param list[cterasdk.edge.types.ShareAccessControlEntry] acl: List of access control entries
+
+        .. warning:: this method will override the existing access control entries
+        """
+        Shares._validate_acl(acl)
+
+        param = [acl_entry.to_server_object() for acl_entry in acl]
+        self._gateway.put('/config/fileservices/share/' + name + '/acl', param)
+
+    def add_acl(self, name, acl):
+        """
+        Add one or more access control entries to an existing share.
+
+        :param str name: The share name
+        :param list[cterasdk.edge.types.ShareAccessControlEntry] acl: List of access control entries to add
+        """
+        Shares._validate_acl(acl)
+
+        current_acl = self._gateway.get('/config/fileservices/share/' + name + '/acl')
+
+        new_acl_dict = {
+            acl_entry.principal_type + '#' + acl_entry.name: acl_entry.to_server_object()
+            for acl_entry in acl
+        }
+
+        for entry in current_acl:
+            ace = ShareAccessControlEntry.from_server_object(entry)
+            entry_key = ace.principal_type + '#' + ace.name
+            if entry_key not in new_acl_dict:
+                new_acl_dict[entry_key] = entry
+
+        acls_array = [v for k, v in new_acl_dict.items()]
+        self._gateway.put('/config/fileservices/share/' + name + '/acl', acls_array)
+
+    def remove_acl(self, name, acl):
+        """
+        Remove one or more access control entries from an existing share.
+
+        :param str name: The share name
+        :param list[cterasdk.edge.types.RemoveShareAccessControlEntry] acl: List of access control entries to remove
+        """
+        Shares._validate_remove_acl(acl)
+
+        remove_acl_dict = {
+            acl_entry.principal_type + '#' + acl_entry.name: True
+            for acl_entry in acl
+        }
+
+        current_acl = self._gateway.get('/config/fileservices/share/' + name + '/acl')
+
+        new_acl = []
+        for entry in current_acl:
+            ace = ShareAccessControlEntry.from_server_object(entry)
+            if not remove_acl_dict.get(ace.principal_type + '#' + ace.name, False):
+                new_acl.append(entry)
+
+        self._gateway.put('/config/fileservices/share/' + name + '/acl', new_acl)
+
+    def modify(
+            self,
+            name,
+            directory=None,
+            acl=None,
+            access=None,
+            csc=None,
+            dir_permissions=None,
+            comment=None,
+            export_to_afp=None,
+            export_to_ftp=None,
+            export_to_nfs=None,
+            export_to_pc_agent=None,
+            export_to_rsync=None,
+            indexed=None,
+            trusted_nfs_clients=None
+                ):  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,unused-argument
+        """
+        Modify an existing network share. All parameters but name are optional and default to None
+
+        :param str name: The share name
+        :param str,optional directory: Full directory path
+        :param list[cterasdk.edge.types.ShareAccessControlEntry],optional acl: List of access control entries
+        :param cterasdk.edge.enum.Acl,optional access: The Windows File Sharing authentication mode
+        :param cterasdk.edge.enum.ClientSideCaching,optional csc: The client side caching (offline files) configuration
+        :param int,optional dir_permissions: Directory Permission
+        :param str,optional comment: Comment
+        :param bool,optional export_to_afp: Whether to enable AFP access
+        :param bool,optional export_to_ftp: Whether to enable FTP access
+        :param bool,optional export_to_nfs: Whether to enable NFS access
+        :param bool,optional export_to_pc_agent: Whether to allow as a destination share for CTERA Backup Agents
+        :param bool,optional export_to_rsync: Whether to enable access over rsync
+        :param bool,optional indexed: Whether to enable indexing for search
+        :param list[cterasdk.edge.types.NFSv3AccessControlEntry] trusted_nfs_clients: Trusted NFS v3 clients, defaults to ``None``
+        """
+        share = self.get(name=name)
+        if directory is not None:
+            parts = path.CTERAPath(directory, '/').parts()
+            volume = parts[0]
+            self._validate_root_directory(volume)
+            share.volume = volume
+            directory = '/'.join(parts[1:])
+            share.directory = directory
+        if access is not None:
+            share.access = access
+        if csc is not None:
+            share.clientSideCaching = csc
+        if dir_permissions is not None:
+            share.dirPermissions = dir_permissions
+        if export_to_afp is not None:
+            share.exportToAFP = export_to_afp
+        if export_to_ftp is not None:
+            share.exportToFTP = export_to_ftp
+        if export_to_nfs is not None:
+            share.exportToNFS = export_to_nfs
+        if export_to_pc_agent is not None:
+            share.exportToPCAgent = export_to_pc_agent
+        if export_to_rsync is not None:
+            share.exportToRSync = export_to_rsync
+        if indexed is not None:
+            share.indexed = indexed
+        if comment is not None:
+            share.comment = comment
+        if acl is not None:
+            Shares._validate_acl(acl)
+            share.acl = [acl_entry.to_server_object() for acl_entry in acl]
+        if trusted_nfs_clients is not None:
+            share.trustedNFSClients = [client.to_server_object() for client in trusted_nfs_clients]
 
-        :return list(str): List of names of all discovered domains
-        """
-        return self._portal.execute('', 'getADTrustedDomains', False)
+        try:
+            self._gateway.put('/config/fileservices/share/' + name, share)
+            logging.getLogger().info("Share modified. %s", {'name': name})
+        except Exception as error:
+            msg = 'Failed to modify the share %s' % name
+            logging.getLogger().error(msg)
+            raise CTERAException(msg, error)
 
-    def fetch(self, active_directory_accounts):
+    def delete(self, name):
         """
-        Instruct the Portal to fetch the provided Active Directory Accounts
-
-        :param list[cterasdk.core.types.PortalAccount] active_directory_accounts: List of Active Directory Accounts to fetch
+        Delete a share.
 
-        :return: Response Code
+        :param str name: The share name
         """
-        domains = self._portal.users.list_domains()
-        account_types = [v for k, v in PortalAccountType.__dict__.items() if not k.startswith('_')]
-
-        param = []
-        for active_directory_account in active_directory_accounts:
-            if active_directory_account.directory not in domains:
-                logging.getLogger().error('Invalid domain name. %s', {'domain': active_directory_account.directory})
-                raise CTERAException('Invalid domain', None, domain=active_directory_account.directory, domains=domains)
-
-            if active_directory_account.account_type not in account_types:
-                logging.getLogger().error('Invalid account type. %s', {'type': active_directory_account.account_type})
-                raise CTERAException('Invalid account type', None, type=active_directory_account.account_type, options=account_types)
-
-        for active_directory_account in active_directory_accounts:
-            if active_directory_account.account_type == PortalAccountType.User:
-                param.append(self._search_users(active_directory_account.directory, active_directory_account.name))
-            elif active_directory_account.account_type == PortalAccountType.Group:
-                param.append(self._search_groups(active_directory_account.directory, active_directory_account.name))
-
-        logging.getLogger().info('Starting to fetch users and groups.')
-        response = self._portal.execute('', 'syncAD', param)
-        logging.getLogger().info('Started fetching users and groups.')
-
-        return response
-
-    def _search_users(self, domain, user):
-        return self._search_directory_services(SearchType.Users, domain, user)
-
-    def _search_groups(self, domain, group):
-        return self._search_directory_services(SearchType.Groups, domain, group)
+        try:
+            self._gateway.delete('/config/fileservices/share/' + name)
+            logging.getLogger().info("Share deleted. %s", {'name': name})
+        except Exception as error:
+            logging.getLogger().error("Share deletion failed.")
+            raise CTERAException('Share deletion failed', error)
 
-    def _search_directory_services(self, search_type, domain, name):
+    def _validate_root_directory(self, name):
         param = Object()
-        param.mode = search_type
-        param.name = name
-        param.domain = domain
+        param.path = '/'
 
-        logging.getLogger().info(
-            'Searching %(search_type)s: %(info)s',
-            dict(search_type=search_type, info={'domain': domain, 'name': name})
-        )
-
-        objects = self._portal.execute('', 'searchAD', param)
-        if not objects:
-            logging.getLogger().info('Could not find results that match your search criteria. %s', {'domain': domain, 'name': name})
-            raise CTERAException(
-                'Could not find results that match your search criteria',
-                None,
-                domain=domain,
-                type=search_type,
-                account=name
-            )
-
-        for principal in objects:
-            if principal.name == name:
-                logging.getLogger().info('Found. %s', {'domain': domain, 'name': name})
-                return principal
-
-        raise CTERAException(
-            'Search returned multiple results, but none matches your search criteria',
-            None,
-            domain=domain,
-            type=search_type,
-            account=name
-        )
-
-    def disconnect(self):
-        """
-        Disconnect a Portal tenant from directory services
-        """
-        return self._portal.put('/directoryConnector', None)
+        response = self._gateway.execute('/status/fileManager', 'listPhysicalFolders', param)
+        for root in response:
+            if root.fullpath == ('/%s' % name):
+                logging.getLogger().debug("Found root directory. %s", {'name': root.name, 'type': root.type, 'fullpath': root.fullpath})
+                return name
+
+        logging.getLogger().error("Could not find root directory. %s", {'name': name})
+
+        options = [root.fullpath[1:] for root in response]
+        raise InputError('Invalid root directory.', name, options)
+
+    @staticmethod
+    def _validate_acl(acl):
+        if not isinstance(acl, list):
+            raise InputError('Invalid access control list format', repr(acl), '[cterasdk.edge.types.ShareAccessControlEntry, ...]')
+        for acl_entry in acl:
+            if not isinstance(acl_entry, ShareAccessControlEntry):
+                raise InputError('Invalid access control entry format', repr(acl_entry), 'cterasdk.edge.types.ShareAccessControlEntry')
+
+    @staticmethod
+    def _validate_remove_acl(acl):
+        if not isinstance(acl, list):
+            raise InputError('Invalid access control list format', repr(acl), '[cterasdk.edge.types.RemoveShareAccessControlEntry, ...]')
+        for acl_entry in acl:
+            if not isinstance(acl_entry, RemoveShareAccessControlEntry):
+                raise InputError(
+                    'Invalid access control entry format',
+                    repr(acl_entry),
+                    'cterasdk.edge.types.RemoveShareAccessControlEntry'
+                )
```

### Comparing `cterasdk-2.8.32/cterasdk/core/enum.py` & `cterasdk-2.9.0/cterasdk/core/enum.py`

 * *Files 27% similar despite different names*

```diff
@@ -358,195 +358,7 @@
     ICAP Services
 
     :ivar str Antivirus: Antivirus
     :ivar str DLP: Data Loss Prevention
     """
     Antivirus = "Antivirus"
     DLP = "DLP"
-
-
-class LocationType:
-    """
-    Location Type
-
-    :ivar str Azure: Azure Blob Storage
-    :ivar str S3: Amazon Web Services S3
-    :ivar str S3Compatible: S3 Compatible
-    :ivar str NetAppStorageGRID: NetApp StorageGRID WebScale (S3)
-    """
-    Azure = 'AzureLocation'
-    S3 = 'S3Location'
-    S3Compatible = 'S3Compatible'
-    NetAppStorageGRID = 'NetAppLocation'
-
-
-class BucketType:
-    """
-    Bucket Type
-
-    :ivar str Azure: Azure
-    :ivar str Scality: Scality
-    :ivar str AWS: Amazon Web Services S3
-    :ivar str ICOS: IBM Cloud Object Storage
-    :ivar str GenericS3: Generic S3
-    :ivar str Nutanix: Nutanix S3
-    :ivar str Wasabi: Wasabi S3
-    :ivar str Google: Google S3
-    :ivar str NetAppStorageGRID: NetApp StorageGRID WebScale (S3)
-    """
-    Azure = 'Azure'
-    Scality = 'ScalityS3'
-    AWS = 'S3'
-    ICOS = 'CleverSafeS3'
-    GenericS3 = 'GenericS3'
-    Nutanix = 'Nutanix'
-    Wasabi = 'WasabiS3'
-    Google = 'GoogleS3'
-    NetAppStorageGRID = 'NTAP'
-
-
-class EnvironmentVariables:
-    """
-    Environment Variables.\n
-    Some environment variables are applicable across platforms (i.e. Windows, Linux), while others are limited to a designated platform
-
-    :ivar str ALLUSERSPROFILE: All users profile
-    :ivar str WINDIR: Windows directory
-    :ivar str TEMP: Temp directory
-    :ivar str SYSTEMDRIVE: System drive
-    :ivar str PROGRAMFILES: Program files
-    :ivar str APPDATA: Application data
-    :ivar str USERPROFILE: Current user profile
-    :ivar str PRIMARYUSER: Primary user
-    :ivar str USERS: Users directory (CTERA Edge Filer)
-    :ivar str AGENTS: Agents directory (CTERA Edge Filer)
-    :ivar str SYNCS: Syncs directory (CTERA Edge Filer)
-    :ivar str PROJECTS: Projects directory (CTERA Edge Filer)
-    """
-    ALLUSERSPROFILE = '$ALLUSERSPROFILE'
-    WINDIR = '$WINDIR'
-    TEMP = '$TEMP'
-    SYSTEMDRIVE = '$SYSTEMDRIVE'
-    PROGRAMFILES = '$PROGRAMFILES'
-    APPDATA = '$APPDATA'
-    USERPROFILE = '$USERPROFILE'
-    USERS = '$USERS'
-    AGENTS = '$AGENTS'
-    SYNCS = '$SYNCS'
-    PROJECTS = '$PROJECTS'
-    PRIMARYUSER = '$PRIMARYUSER'
-
-
-class Platform:
-    """
-    CTERA Edge Platform Type.\n
-
-    :ivar str C200_Orion: All users profile
-    :ivar str C200_ARM: Windows directory
-    :ivar str C200_Kirkwood: Temp directory
-    :ivar str C400_C800: System drive
-    :ivar str Edge_6: CTERA 6.0 Edge Filer
-    :ivar str Edge_7: CTERA 7.0 Edge Filer
-    :ivar str Windows: Windows Agent (Drive App)
-    :ivar str Linux: Linux Agent (Drive App)
-    :ivar str OSX: Mac Agent (Drive App)
-    """
-    C200_Orion = 'Orion'
-    C200_ARM = 'ARM'
-    C200_Kirkwood = 'Kirkwood'
-    C400_C800 = 'X86'
-    Edge_6 = 'VBox'
-    Edge_7 = 'Genesis'
-    Linux = 'LinuxX86'
-    Windows = 'WindowsX86'
-    OSX = 'OSxX86'
-
-
-class TemplateCriteria:
-    """
-    Configuration Template Auto Assignment Rule Builder Criterias
-
-    :ivar str Type: Device type
-    :ivar str OperatingSystem: Operating system
-    :ivar str Version: Installed software version
-    :ivar str Hostname: Hostname
-    :ivar str Name: Device name
-    :ivar str Owner: Device owner username
-    :ivar str Plan: Plan name
-    :ivar str Groups: Device owner local or domain groups
-    """
-    Type = 'DeviceType'
-    OperatingSystem = 'OperatingSystem'
-    Version = 'InstalledSoftwareVersion'
-    Hostname = 'Hostname'
-    Name = 'DeviceName'
-    Owner = 'OwnerUsername'
-    Plan = 'Plan'
-    Groups = 'ownerGroups'
-
-
-class IPProtocol:
-    """
-    IP Protocol
-
-    :ivar str TCP: TCP Protocol
-    :ivar str UDP: UDP Protocol
-    """
-    TCP = "TCP"
-    UDP = "UDP"
-
-
-class Mode:
-    """
-    Enum for operational mode
-
-    :ivar str Enabled: Operational mode enabled
-    :ivar str Disabled: Operational mode diabled
-    """
-    Enabled = "enabled"
-    Disabled = "disabled"
-
-
-class DirectoryServiceType:
-    """
-    Directory Service Type
-
-    :ivar str Microsoft: Active Directory
-    :ivar str LDAP: LDAP
-    :ivar str Apple: Apple Open Directory
-    """
-    Microsoft = 'ActiveDirectory'
-    LDAP = 'LDAP'
-    Apple = 'AppleOpenDirectory'
-
-
-class DirectoryServiceFetchMode:
-    """
-    Directory Service Fetch Mode
-
-    :ivar str Eager: Eager
-    :ivar str Lazy: Lazy
-    """
-    Eager = 'Eager'
-    Lazy = 'Lazy'
-
-
-class DirectorySearchEntityType:
-    """
-    Directory Search Entity Type
-
-    :ivar str User: User
-    :ivar str Group: Group
-    """
-    User = 'user'
-    Group = 'group'
-
-
-class DeduplicationMethodType:
-    """
-    Folder Group Deduplication Method Type
-
-    :ivar str AverageBlockSize: AverageBlockSize
-    :ivar str FixedBlockSize: FixedBlockSize
-    """
-    AverageBlockSize = 'AverageBlockSize'
-    FixedBlockSize = 'FixedBlockSize'
```

### Comparing `cterasdk-2.8.32/cterasdk/core/files/browser.py` & `cterasdk-2.9.0/cterasdk/core/files/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import logging
 from .path import CTERAPath
 
-from ... import config
-from ...exception import CTERAException
 from ..base_command import BaseCommand
 from . import ls, directory, rename, rm, recover, mv, cp, ln, collaboration, file_access
 
 
+# pylint: disable=too-many-public-methods
 class FileBrowser(BaseCommand):
 
     """
     Portal File Browser APIs
     """
 
     def __init__(self, portal, base_path):
@@ -49,63 +47,29 @@
         Download a file
 
         :param str path: Path of the file to download
         :param str,optional destination:
          File destination, if it is a directory, the original filename will be kept, defaults to the default directory
         """
         path = self.mkpath(path)
-        return self._file_access.download(path, destination=destination)
+        self._file_access.download(path, destination=destination)
 
     def download_as_zip(self, cloud_directory, files, destination=None):
         """
         Download a list of files and/or directories from a cloud folder as a ZIP file
 
         .. warning:: The list of files is not validated. The ZIP file will include only the existing  files and directories
 
         :param str cloud_directory: Path to the cloud directory
         :param list[str] files: List of files and/or directories in the cloud folder to download
         :param str,optional destination:
          File destination, if it is a directory, the original filename will be kept, defaults to the default directory
         """
         self._file_access.download_as_zip(self.mkpath(cloud_directory), files, destination=destination)
 
-    def copy(self, src, dest):
-        """
-        Copy a file or directory
-
-        :param str src: The source path of the file or directory
-        :param str dst: The destination path of the file or directory
-        """
-        return cp.copy(self._portal, self.mkpath(src), self.mkpath(dest))
-
-    def copy_multi(self, src, dest):
-        return cp.copy_multi(self._portal, self.mkpath(src), self.mkpath(dest))
-
-    def mklink(self, path, access='RO', expire_in=30):
-        """
-        Create a link to a file
-
-        :param str path: The path of the file to create a link to
-        :param str,optional access: Access policy of the link, defaults to 'RO'
-        :param int,optional expire_in: Number of days until the link expires, defaults to 30
-        """
-        return ln.mklink(self._portal, self.mkpath(path), access, expire_in)
-
-    def mkpath(self, array):
-        if isinstance(array, list):
-            return [CTERAPath(item, self._base_path) for item in array]
-        return CTERAPath(array, self._base_path)
-
-
-class CloudDrive(FileBrowser):
-
-    """
-    Cloud Drive File Browser APIs
-    """
-
     def upload(self, file_path, server_path):
         """
         Upload a file
 
         :param str file_path: Path to the local file to upload
         :param str server_path: Path to the directory to upload the file to
         """
@@ -169,14 +133,36 @@
         :param str dst: The destination path of the file or directory
         """
         return mv.move(self._portal, self.mkpath(src), self.mkpath(dest))
 
     def move_multi(self, src, dest):
         return mv.move_multi(self._portal, self.mkpath(src), self.mkpath(dest))
 
+    def copy(self, src, dest):
+        """
+        Copy a file or directory
+
+        :param str src: The source path of the file or directory
+        :param str dst: The destination path of the file or directory
+        """
+        return cp.copy(self._portal, self.mkpath(src), self.mkpath(dest))
+
+    def copy_multi(self, src, dest):
+        return cp.copy_multi(self._portal, self.mkpath(src), self.mkpath(dest))
+
+    def mklink(self, path, access='RO', expire_in=30):
+        """
+        Create a link to a file
+
+        :param str path: The path of the file to create a link to
+        :param str,optional access: Access policy of the link, defaults to 'RO'
+        :param int,optional expire_in: Number of days until the link expires, defaults to 30
+        """
+        return ln.mklink(self._portal, self.mkpath(path), access, expire_in)
+
     def get_share_info(self, path):
         """
         Get share settings and recipients
         """
         return collaboration.get_share_info(self._portal, self.mkpath(path))
 
     def share(self, path, recipients, as_project=True, allow_reshare=True, allow_sync=True):
@@ -217,28 +203,11 @@
 
     def unshare(self, path):
         """
         Unshare a file or a folder
         """
         return collaboration.unshare(self._portal, self.mkpath(path))
 
-
-class Backups(FileBrowser):
-
-    """
-    Backups File Browser APIs
-    """
-
-    def device_config(self, device, destination=None):
-        """
-        Download a device configuration file
-
-        :param str device: The device name
-        :param str,optional destination:
-         File destination, if it is a directory, the original filename will be kept, defaults to the default directory
-        """
-        try:
-            destination = destination if destination is not None else f'{config.filesystem["dl"]}/{device}.xml'
-            return self.download(f'{device}/Device Configuration/db.xml', destination)
-        except CTERAException as error:
-            logging.getLogger().error('Failed downloading configuration file. %s', {'device': device, 'error': error.response.reason})
-            raise error
+    def mkpath(self, array):
+        if isinstance(array, list):
+            return [CTERAPath(item, self._base_path) for item in array]
+        return CTERAPath(array, self._base_path)
```

### Comparing `cterasdk-2.8.32/cterasdk/core/files/collaboration.py` & `cterasdk-2.9.0/cterasdk/core/files/collaboration.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/common.py` & `cterasdk-2.9.0/cterasdk/core/files/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,30 @@
         SrcDstParam(src, dest)
         return SrcDstParam.__instance
 
     def __init__(self, src, dest=None):
         self._classname = self.__class__.__name__
         self.src = src
         self.dest = dest
-        SrcDstParam.__instance = self  # pylint: disable=unused-private-member
+        SrcDstParam.__instance = self
 
 
 class ActionResourcesParam(Object):
 
     __instance = None
 
     @staticmethod
     def instance():
         ActionResourcesParam()
         return ActionResourcesParam.__instance
 
     def __init__(self):
         self._classname = self.__class__.__name__
         self.urls = []
-        ActionResourcesParam.__instance = self  # pylint: disable=unused-private-member
+        ActionResourcesParam.__instance = self
 
     def add(self, param):
         self.urls.append(param)
 
 
 class CreateShareParam(Object):
 
@@ -53,15 +53,15 @@
         self.share._classname = 'ShareConfig'
         self.share.accessMode = access
         self.share.protectionLevel = 'publicLink'
         self.share.expiration = expire_on
         self.share.invitee = Object()
         self.share.invitee._classname = 'Collaborator'
         self.share.invitee.type = 'external'
-        CreateShareParam.__instance = self  # pylint: disable=unused-private-member
+        CreateShareParam.__instance = self
 
 
 def get_resource_info(ctera_host, path):
     response = ls.ls(ctera_host, path, depth=0)
     if response.root is None:
         raise RemoteDirectoryNotFound(path.fullpath())
     return response.root
```

### Comparing `cterasdk-2.8.32/cterasdk/core/files/cp.py` & `cterasdk-2.9.0/cterasdk/core/files/cp.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/directory.py` & `cterasdk-2.9.0/cterasdk/core/files/directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         raise error
     except InvalidName as error:
         logging.getLogger().error('Directory name contains invalid characters. %s', {'name': path})
         raise error
     except ReservedName as error:
         logging.getLogger().error('Reserved directory name. %s', {'name': path})
         raise error
-    logging.getLogger().info('Directory created. %s', {'path': path})
+    else:
+        logging.getLogger().info('Directory created. %s', {'path': path})
 
 
 def _process_error(response, path):
     error = FileManagerTaskRC.get(response)
     if error is not None:
         error = error()
         error.path = path
```

### Comparing `cterasdk-2.8.32/cterasdk/core/files/fetch_resources_param.py` & `cterasdk-2.9.0/cterasdk/core/files/fetch_resources_param.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/file_access.py` & `cterasdk-2.9.0/cterasdk/core/files/file_access.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class FileAccess(FileAccessBase):
 
     def _get_single_file_url(self, path):
         return path.fullpath()
 
     def _get_multi_file_url(self, cloud_directory, files):
         folder_uid = self._get_cloud_folder_uid(cloud_directory)
-        return f'{self._ctera_host.context}/folders/folders/{folder_uid}'
+        return '%s/folders/folders/%s' % (self._ctera_host.context, folder_uid)
 
     @property
     def _use_file_url_for_multi_file_url(self):
         return True
 
     def _get_multi_file_object(self, cloud_directory, files):
         files_obj = Object()
@@ -27,15 +27,15 @@
         files_obj.password = None
         files_obj.portalName = None
         files_obj.showDeleted = False
         return files_obj
 
     def _get_upload_url(self, dest_path):
         folder_uid = self._get_cloud_folder_uid(dest_path)
-        return f'{self._ctera_host.context}/upload/folders/{folder_uid}'
+        return '%s/upload/folders/%s' % (self._ctera_host.context, folder_uid)
 
     def _get_upload_form(self, local_file_info, fd, dest_path):
         return dict(
             name=local_file_info['name'],
             Filename=local_file_info['name'],
             fullpath=urljoin(
                 self._ctera_host.base_file_url,
```

### Comparing `cterasdk-2.8.32/cterasdk/core/files/ln.py` & `cterasdk-2.9.0/cterasdk/core/files/ln.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/ls.py` & `cterasdk-2.9.0/cterasdk/core/files/ls.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/mv.py` & `cterasdk-2.9.0/cterasdk/core/files/mv.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/files/path.py` & `cterasdk-2.9.0/cterasdk/core/files/path.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/login.py` & `cterasdk-2.9.0/cterasdk/core/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,9 @@
         self._portal.form_data('/login', {'j_username': username, 'j_password': password})
         logging.getLogger().info("User logged in. %s", {'host': self._portal.host(), 'user': username})
 
     def logout(self):
         """
         Log out of the portal
         """
-        username = self._portal.session().user.name
         self._portal.form_data('/logout', {})
-        logging.getLogger().info("User logged out. %s", {'host': self._portal.host(), 'user': username})
+        logging.getLogger().info("User logged out. %s", {'host': self._portal.host()})
```

### Comparing `cterasdk-2.8.32/cterasdk/core/logs.py` & `cterasdk-2.9.0/cterasdk/core/users.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,178 @@
 import logging
-from datetime import datetime
 
 from .base_command import BaseCommand
-from ..lib import Iterator, Command
-from ..core import enum
-from ..common import Object
+from .types import UserAccount
+from ..exception import CTERAException
+from ..common import Object, DateTimeUtils
+from ..common import union
 from . import query
 
 
-class Logs(BaseCommand):
+class Users(BaseCommand):
     """
-    Portal Logs APIs
-
-    :ivar cterasdk.core.logs.Alerts alerts: Object holding the Portal Log Based Alerts APIs
+    Portal User Management APIs
     """
 
-    def __init__(self, portal):
-        super().__init__(portal)
-        self.alerts = Alerts(self._portal)
-
-    def device(self,
-               name,
-               topic=enum.LogTopic.System,
-               min_severity=enum.Severity.INFO,
-               before=None,
-               after=None,
-               filters=None):
-        """
-        Get device logs from the Portal
-
-        :param str name: Name of a device
-        :param cterasdk.core.enum.LogTopic,optional topic: Log topic to get, defaults to cterasdk.core.enum.LogTopic.System
-        :param cterasdk.core.enum.Severity,optional min_severity:
-         Minimun severity of logs to get, defaults to cterasdk.core.enum.Severity.INFO
-        :param str,optional before: Get logs before this date (in format "%m/%d/%Y %H:%M:%S"), defaults to None
-        :param str,optional after: Get logs after this date (in format "%m/%d/%Y %H:%M:%S"), defaults to None
-        :param list[cterasdk.core.query.FilterBuilder],optional filters: List of additional filters, defaults to None
-
-        :return: Iterator for all matching logs
-        :rtype: cterasdk.lib.iterator.Iterator[cterasdk.object.Object]
-        """
-        return self.get(topic, min_severity, enum.OriginType.Device, name, before, after, filters)
-
-    def get(self, topic=enum.LogTopic.System, min_severity=enum.Severity.INFO, origin_type=enum.OriginType.Portal, origin=None,
-            before=None, after=None, filters=None):
-        """
-        Get logs from the Portal
-
-        :param cterasdk.core.enum.LogTopic,optional topic: Log topic to get, defaults to cterasdk.core.enum.LogTopic.System
-        :param cterasdk.core.enum.Severity,optional min_severity:
-         Minimun severity of logs to get, defaults to cterasdk.core.enum.Severity.INFO
-        :param cterasdk.core.enum.OriginType,optional origin_type:
-         Origin type of the logs to get, defaults to cterasdk.core.enum.OriginType.Portal
-        :param str,optional origin: Log origin (e.g. device name, Portal server name), defaults to None
-        :param str,optional before: Get logs before this date (in format "%m/%d/%Y %H:%M:%S"), defaults to None
-        :param str,optional after: Get logs after this date (in format "%m/%d/%Y %H:%M:%S"), defaults to None
-        :param list[cterasdk.core.query.FilterBuilder],optional filters: List of additional filters, defaults to None
-
-        :return: Iterator for all matching logs
-        :rtype: cterasdk.lib.iterator.Iterator[cterasdk.object.Object]
-        """
-        builder = query.QueryParamBuilder().put('topic', topic).put('minSeverity', min_severity)
-
-        builder.addFilter(query.FilterBuilder('originType').eq(origin_type))
-
-        if before is not None:
-            builder.addFilter(query.FilterBuilder('time').before(self._strptime(before)))
-
-        if after is not None:
-            builder.addFilter(query.FilterBuilder('time').after(self._strptime(after)))
-
-        if origin is not None:
-            builder.addFilter(query.FilterBuilder.ref('origin').eq(origin))
-
-        if filters:
-            for user_filter in filters:
-                builder.addFilter(user_filter)
+    default = ['name']
 
-        param = builder.build()
-        function = Command(self._query_logs)
-
-        return Iterator(function, param)
-
-    def _query_logs(self, param):
-        response = self._portal.execute('', 'queryLogs', param)
-        return (response.hasMore, response.logs)
-
-    @staticmethod
-    def _strptime(datetime_str):
+    def _get_entire_object(self, user_account):
+        ref = '/users/%s' % user_account.name if user_account.is_local \
+            else '/domains/%s/adUsers/%s' % (user_account.directory, user_account.name)
         try:
-            return datetime.strptime(datetime_str, '%m/%d/%Y %H:%M:%S')
-        except ValueError as error:
-            raise error
-
+            return self._portal.get(ref)
+        except CTERAException as error:
+            raise CTERAException('Failed to get the user', error)
+
+    def get(self, user_account, include=None):
+        """
+        Get a user account
+
+        :param cterasdk.core.types.UserAccount user_account: User account, including the user directory and user name
+        :param list[str] include: List of fields to retrieve, defaults to ['name']
+        :return: The user account, including the requested fields
+        """
+        baseurl = '/users/%s' % user_account.name if user_account.is_local \
+            else '/domains/%s/adUsers/%s' % (user_account.directory, user_account.name)
+        include = union(include or [], Users.default)
+        include = ['/' + attr for attr in include]
+        user_object = self._portal.get_multi(baseurl, include)
+        if user_object.name is None:
+            raise CTERAException('Could not find user', None, user_directory=user_account.directory, username=user_account.name)
+        return user_object
+
+    def list_local_users(self, include=None):
+        """
+        List all local users
+
+        :param list[str] include: List of fields to retrieve, defaults to ['name']
+        :return: Iterator for all local users
+        :rtype: cterasdk.lib.iterator.Iterator
+        """
+        include = union(include or [], Users.default)
+        param = query.QueryParamBuilder().include(include).build()
+        return query.iterator(self._portal, '/users', param)
+
+    def list_domains(self):
+        """
+        List all domains
+
+        :return list: List of all domains
+        """
+        return self._portal.get('/domains')
+
+    def list_domain_users(self, domain, include=None):
+        """
+        List all the users in the domain
+
+        :param list[str] include: List of fields to retrieve, defaults to ['name']
+        :return: Iterator for all the domain users
+        :rtype: cterasdk.lib.iterator.Iterator
+        """
+        include = union(include or [], Users.default)
+        param = query.QueryParamBuilder().include(include).build()
+        return query.iterator(self._portal, '/domains/' + domain + '/adUsers', param)
+
+    def add(self, name, email, first_name, last_name, password, role, company=None, comment=None, password_change=False):
+        """
+        Create a local user account
+
+        :param str name: User name for the new user
+        :param str email: E-mail address of the new user
+        :param str first_name: The first name of the new user
+        :param str last_name: The last name of the new user
+        :param str password: Password for the new user
+        :param cterasdk.core.enum.Role role: User role of the new user
+        :param str,optional company: The name of the company of the new user, defaults to None
+        :param str,optional comment: Additional comment for the new user, defaults to None
+        :param variable,optional password_change:
+            Require the user to change the password on the first login.
+            Pass datetime.date for a specific date, integer for days from creation, or True for immediate , defaults to False
+        """
+        param = Object()
+        param._classname = "PortalUser"  # pylint: disable=protected-access
+        param.name = name
+        param.email = email
+        param.firstName = first_name
+        param.lastName = last_name
+        param.password = password
+        param.role = role
+        param.company = company
+        param.comment = comment
+        if password_change:
+            param.requirePasswordChangeOn = DateTimeUtils.get_expiration_date(password_change).strftime('%Y-%m-%d')
+
+        logging.getLogger().info('Creating user. %s', {'user': name})
+        response = self._portal.add('/users', param)
+        logging.getLogger().info('User created. %s', {'user': name, 'email': email, 'role': role})
 
-class Alerts(BaseCommand):
-    """
-    Portal Log Based Alerts APIs
-    """
-
-    def add(self, name, description=None, topic=None, log=None, min_severity=None, origin_type=None, content=None):
-        """
-        Add a Log Based Alert
-
-        :param str name: Alert name
-        :param str,optional description: Alert description
-        :param cterasdk.core.enum.LogTopic,optional topic: Log topic to get, defaults to any topic
-        :param str,optional log: Class name of the log
-        :param cterasdk.core.enum.Severity,optional min_severity: Minimun severity for triggering an alert, defaults to any severity
-        :param cterasdk.core.enum.OriginType,optional origin_type: Origin type of the log, defaults to any origin
-        :param str content: Content of the log message
-        :returns: A list of alerts
-        :rtype: list[cterasdk.common.object.Object]
-        """
-        alert = Object()
-        alert.id = name
-        alert._classname = 'AlertRule'  # pylint: disable=protected-access
-        if description:
-            alert.description = description
-        if log:
-            alert.logName = log
-        if content:
-            alert.messageContent = content
-        if min_severity:
-            alert.minSeverity = min_severity
-        if origin_type:
-            alert.originType = origin_type
-        if topic:
-            alert.topic = topic
-        alerts = self.get()
-        alerts.append(alert)
-        return self.put(alerts)
-
-    def put(self, alerts):
-        """
-        Set Log Based Alerts
-         Use :func:`cterasdk.core.types.AlertBuilder` to build log based alerts`
-
-        :param list[cterasdk.core.types.Alert] alerts: List of alerts
-        """
-        logging.getLogger().info('Updating log based alerts.')
-        response = self._portal.put(self._context, alerts)
-        logging.getLogger().info('Log based alerts updated.')
         return response
 
-    def get(self):
-        """
-        Get a List of Log Based Alerts
-
-        :returns: A list of alerts
-        :rtype: list[cterasdk.common.object.Object]
+    def modify(self, current_username, new_username=None, email=None, first_name=None,
+               last_name=None, password=None, role=None, company=None, comment=None):
         """
-        return self._portal.get(self._context)
+        Modify a local user account
 
-    def delete(self, name):
-        """
-        Remove a Log Based Alert
+        :param str current_username: The current user name
+        :param str,optional new_username: New name
+        :param str,optional email: E-mail address
+        :param str,optional first_name: First name
+        :param str,optional last_name: Last name
+        :param str,optional password: Password
+        :param cterasdk.core.enum.Role,optional role: User role
+        :param str,optional company: Company name
+        :param str,optional comment: Comment
+        """
+        user_account = UserAccount(current_username)
+        user = self._get_entire_object(user_account)
+        if new_username:
+            user.name = new_username
+        if email:
+            user.email = email
+        if first_name:
+            user.firstName = first_name
+        if last_name:
+            user.lastName = last_name
+        if password:
+            user.password = password
+        if role:
+            user.role = role
+        if company is not None:
+            user.company = company
+        if comment is not None:
+            user.comment = comment
 
-        :param str name: Alert name
-        """
-        alerts = [alert for alert in self.get() if alert.id != name]
-        self.put(alerts)
+        try:
+            response = self._portal.put('/users/' + current_username, user)
+            logging.getLogger().info("User modified. %s", {'username': user.name})
+            return response
+        except CTERAException as error:
+            logging.getLogger().error("Failed to modify user.")
+            raise CTERAException('Failed to modify user', error)
+
+    def apply_changes(self, wait=False):
+        """
+        Apply provisioning changes.\n
+
+        :param bool,optional wait: Wait for all changes to apply
+        """
+        param = Object()
+        param.objectId = None
+        param.type = 'users'
+        logging.getLogger().info('Applying provisioning changes.')
+        task = self._portal.execute('', 'updateAccounts', param)
+        if wait:
+            task = self._portal.tasks.wait(task)
+        return task
+
+    def delete(self, user):
+        """
+        Delete a user
+
+        :param cterasdk.core.types.UserAccount user: the user account
+        """
+        logging.getLogger().info('Deleting user. %s', {'user': str(user)})
+        baseurl = '/users/%s' % user.name if user.is_local else '/domains/%s/adUsers/%s' % (user.directory, user.name)
+        response = self._portal.execute(baseurl, 'delete', True)
+        logging.getLogger().info('User deleted. %s', {'user': str(user)})
 
-    @property
-    def _context(self):
-        return f'{"" if self._portal.session().in_tenant_context() else "/settings"}/alerts'
+        return response
```

### Comparing `cterasdk-2.8.32/cterasdk/core/plans.py` & `cterasdk-2.9.0/cterasdk/core/plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 from .base_command import BaseCommand
-from ..exception import CTERAException, InputError, ObjectNotFoundException
+from ..exception import CTERAException, InputError
 from .enum import PlanItem, PlanRetention
 from ..common import union, convert_size, DataUnit, PolicyRuleConverter
 from . import query
 
 
 class Plans(BaseCommand):
     """
-    Portal Plan APIs
-
-    :ivar cterasdk.core.plans.PlanAutoAssignPolicy auto_assign: Object holding the Portal subscription plan auto assignment rules APIs
+    Global Admin Plan APIs
     """
     default = ['name']
     _allowed_storage_size_units = [DataUnit.GB, DataUnit.TB, DataUnit.PB]
 
     def __init__(self, portal):
         super().__init__(portal)
         self.auto_assign = PlanAutoAssignPolicy(self._portal)
@@ -73,15 +71,15 @@
         :param list[str] include: List of fields to retrieve, defaults to ['name']
         :return: The subscription plan, including the requested fields
         """
         include = union(include or [], Plans.default)
         include = ['/' + attr for attr in include]
         plan = self._portal.get_multi('/plans/' + name, include)
         if plan.name is None:
-            raise ObjectNotFoundException('Could not find subscription plan', f'/plans/{name}', name=name)
+            raise CTERAException('Could not find subscription plan', None, name=name)
         return plan
 
     def add(self, name, retention=None, quotas=None):
         """
         Add a subscription plan
 
         :param dict,optional retention: The data retention policy
```

### Comparing `cterasdk-2.8.32/cterasdk/core/query.py` & `cterasdk-2.9.0/cterasdk/core/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from datetime import datetime
 
 from ..lib import Iterator, Command
 from ..common import Object
 from ..convert import tojsonstr
 
 
-def query(CTERAHost, path, name, param):
-    response = CTERAHost.execute(path, name, param) if name is not None else CTERAHost.db(path, 'query', param)
+def query(CTERAHost, path, param):
+    response = CTERAHost.db(path, 'query', param)
     return (response.hasMore, response.objects)
 
 
-def show(CTERAHost, path, name, param):
-    hasMore, objects = query(CTERAHost, path, name, param)
+def show(CTERAHost, path, param):
+    hasMore, objects = query(CTERAHost, path, param)
     print(tojsonstr(objects, no_log=False))
     return hasMore
 
 
-def iterator(CTERAHost, path, param, name=None):
-    function = Command(query, CTERAHost, path, name)
+def iterator(CTERAHost, path, param):
+    function = Command(query, CTERAHost, path)
     return Iterator(function, param)
 
 
 class Restriction:
     LIKE = "like"
     UNLIKE = "notLike"
     EQUALS = "eq"
```

### Comparing `cterasdk-2.8.32/cterasdk/core/remote.py` & `cterasdk-2.9.0/cterasdk/core/remote.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/reports.py` & `cterasdk-2.9.0/cterasdk/core/reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         """
         Retrieve the folder groups statistics report.\n
         To retrieve this report, you must first browse the Virtual Portal that contains the report, using: `GlobalAdmin.portals.browse()`
         """
         return self._get_report('folderGroupsStatisticsReport')
 
     def _get_report(self, report_name):
-        return self._portal.get(f'/reports/{report_name}')
+        return self._portal.get('/reports/%s' % report_name)
```

### Comparing `cterasdk-2.8.32/cterasdk/core/session.py` & `cterasdk-2.9.0/cterasdk/core/session.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/core/setup.py` & `cterasdk-2.9.0/cterasdk/core/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,25 +50,25 @@
             params.admin.firstName = first_name
             params.admin.lastName = last_name
             params.admin.password = password
 
             params.settings = Setup.default_settings()
             params.settings.dnsSuffix = domain
             logging.getLogger().info('Initializing Portal. %s', {'domain': domain, 'user': name})
-            self._portal.execute(f'/{self._portal.context}/public', 'init', params, use_file_url=True)
+            self._portal.execute('/%s/public' % (self._portal.context), 'init', params, use_file_url=True)
             SetupWizardStatusMonitor(self._portal).wait(SetupWizardStage.Portal)
             logging.getLogger().info('Portal initialized.')
         elif self.stage == SetupWizardStage.Finish:
             logging.getLogger().warning('Portal already initialized. %s', {'host': self._portal.host()})
         self._portal.startup.wait()
 
     def _init_slave(self, ipaddr, secret):
         self._get_current_stage()
 
-        response = self._portal.execute(f'/{self._portal.context}/setup/authenticaionMethod',
+        response = self._portal.execute('/%s/setup/authenticaionMethod' % (self._portal.context),
                                         'askMasterForSlaveAuthenticaionMethod', ipaddr, use_file_url=True)
 
         params = Setup._init_server_params(ServerMode.Slave)
         params.slaveSettings.masterIpAddr = ipaddr
         if response == SlaveAuthenticaionMethod.Password:
             params.slaveSettings.masterPassword = secret
         elif response == SlaveAuthenticaionMethod.PrivateKey:
@@ -76,15 +76,15 @@
         else:
             logging.getLogger().error('Unknown authentication method. %s', {'method': response})
 
         self._init_server(params, True)
 
     def _init_server(self, params, wait=False):
         if self.stage == SetupWizardStage.Server:
-            ref = f'/{self._portal.context}/setup'
+            ref = '/%s/setup' % (self._portal.context)
             form_data = {'inputXml': toxmlstr(params).decode('utf-8'), 'serverMode': params.serverMode}
 
             if params.serverMode == ServerMode.Slave:
                 form_data['masterIpAddr'] = params.slaveSettings.masterIpAddr
 
             logging.getLogger().info('Initializing server. %s', {'host': self._portal.host(), 'mode': params.serverMode})
             self._portal.multipart(ref, form_data, use_file_url=True)
@@ -105,32 +105,29 @@
         self._init_slave(ipaddr, secret)
         if self.stage == SetupWizardStage.Replication:
             logging.getLogger().info('Initializing an Application Server. %s', {'host': ipaddr})
             params = Setup._init_replication_param()
             self._init_role(params)
         self._portal.startup.wait()
 
-    def init_replication_server(self, ipaddr, secret, replicate_from=None):
+    def init_replication_server(self, ipaddr, secret, replicate_from):
         """
         Initialize a CTERA Portal Database Replication Server.
 
         :param str ipaddr: The CTERA Portal master server IP address
         :param str secret: A password or a PEM-encoded private key
-        :param str replicate_from: The name of a CTERA Portal server to replicate from
+        :param str replicate_from: The name of a CTERA Portal server replication source
         """
         self._init_slave(ipaddr, secret)
         if self.stage == SetupWizardStage.Replication:
             logging.getLogger().info('Initializing a Replication Database Server. %s', {'host': ipaddr, 'replicate_from': replicate_from})
             logging.getLogger().debug('Retrieving database replication candidates.')
             replication_candidates = {re.search('([^/]+$)', k).group(0): k for k in self.get_replication_candidates()}
             if replication_candidates:
-                if replicate_from is None and len(replication_candidates) == 1:
-                    server = next(iter(replication_candidates.values()))
-                else:
-                    server = replication_candidates.get(replicate_from)
+                server = replication_candidates.get(replicate_from)
                 if server:
                     logging.getLogger().debug('Found server in replication candidates. %s', {'server': replicate_from})
                     params = Setup._init_replication_param(server)
                     self._init_role(params)
                 else:
                     logging.getLogger().error('Could not find database replication target. %s', {
                         'target': replicate_from,
@@ -139,21 +136,21 @@
                     raise CTERAException('Could not find database replication target.',
                                          None, target=replicate_from, options=replication_candidates)
             else:
                 logging.getLogger().error('Could not find database replication candidates.')
         self._portal.startup.wait()
 
     def _init_role(self, params):
-        response = self._portal.execute(f'/{self._portal.context}/public/servers', 'setReplication', params, use_file_url=True)
+        response = self._portal.execute('/%s/public/servers' % (self._portal.context), 'setReplication', params, use_file_url=True)
         status = SetupWizardStatusMonitor(self._portal).wait(SetupWizardStage.Replication)
         self.stage = status.wizard
         return response
 
     def get_replication_candidates(self):
-        return self._portal.execute(f'/{self._portal.context}/public/servers', 'getReplicaitonCandidates', None, use_file_url=True)
+        return self._portal.execute('/%s/public/servers' % (self._portal.context), 'getReplicaitonCandidates', None, use_file_url=True)
 
     @staticmethod
     def _init_replication_param(replicate_from=None):
         params = Object()
         params._classname = 'SetReplicationParam'  # pylint: disable=protected-access
         if replicate_from:
             params.enabledReplicationParam = Object()
@@ -169,15 +166,15 @@
         params.serverMode = mode
         if mode == ServerMode.Slave:
             params.slaveSettings = Object()
             params.slaveSettings._classname = 'SlaveServerSettings'  # pylint: disable=protected-access
         return params
 
     def get_setup_status(self):
-        return self._portal.get(f'/{self._portal.context}/setup/status', use_file_url=True)
+        return self._portal.get('/%s/setup/status' % (self._portal.context), use_file_url=True)
 
     @staticmethod
     def default_settings():
         settings = Object()
         settings._classname = 'SystemSettings'  # pylint: disable=protected-access
         settings.smtpSettings = Object()
         settings.smtpSettings._classname = 'SMTPSettings'  # pylint: disable=protected-access
```

### Comparing `cterasdk-2.8.32/cterasdk/core/startup.py` & `cterasdk-2.9.0/cterasdk/core/startup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def status(self):
         """
         Get the server startup status
         """
         response = None
         try:
-            response = self._portal.get(f'/{self._portal.context}/startup', use_file_url=True)
+            response = self._portal.get('/%s/startup' % (self._portal.context), use_file_url=True)
         except CTERAClientException as error:
             return error.response.body.status
         return response.status
 
     def wait(self, retries=120, seconds=5):
         """
         Wait for server startup
```

### Comparing `cterasdk-2.8.32/cterasdk/core/syslog.py` & `cterasdk-2.9.0/cterasdk/edge/syslog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,77 @@
 import logging
 
-from .base_command import BaseCommand
-from ..common import Object
-from ..core.enum import Severity, Mode, IPProtocol
 from ..exception import CTERAException
+from ..common import Object
+from . import enum
+from .base_command import BaseCommand
 
 
 class Syslog(BaseCommand):
-    """
-    Portal Syslog Management APIs
-    """
-
-    # TODO: upload_ca_certificate  # pylint: disable=W0511
-    # TODO: upload_client_certificate  # pylint: disable=W0511
+    """ Gateway Syslog configuration APIs """
 
-    def is_enabled(self):
-        """
-        Check if forwarding log messages over syslog is enabled
+    def enable(self, server, port=514, proto=enum.IPProtocol.UDP, min_severity=enum.Severity.INFO):
         """
-        return self._portal.get('/settings/logsSettings/syslogConfig/mode') == Mode.Enabled
+        Enable Syslog
 
-    def get_configuration(self):
-        """
-        Retrieve the syslog server configuration
-        """
-        return self._portal.get('/settings/logsSettings/syslogConfig')
+        :param str server: Server address to send syslog logs
+        :param int,optional port: Syslog server communication port, defaults to 514
+        :param cterasdk.edge.enum.IPProtocol,optional proto:
+         Syslog server communication protocol, defaults to cterasdk.edge.enum.IPProtocol.UDP
+        :param cterasdk.edge.enum.Severity,optional min_severity:
+         Minimal log severity to fetch, defaults to cterasdk.edge.enum.Severity.INFO
+        """
+        obj = Object()
+        obj.mode = enum.Mode.Enabled
+        obj.server = server
+        obj.port = port
+        obj.proto = proto
+        obj.minSeverity = min_severity
 
-    def enable(self, server, port=514, protocol=IPProtocol.UDP, min_severity=Severity.INFO):
-        """
-        Enable Syslog
+        logging.getLogger().info("Configuring syslog server.")
+        self._gateway.put('/config/logging/syslog', obj)
+        logging.getLogger().info(
+            "Syslog server configured. %s",
+            {'server': server, 'port': port, 'protocol': proto, 'minSeverity': min_severity}
+        )
 
-        :param str server: Syslog server address
-        :param int,optional port: Syslog server port
-        :param cterasdk.core.enum.IPProtocol,optional protocol: Syslog server IP protocol
-        :param cterasdk.core.enum.Severity,optional min_severity: Minimum log severity to forward
-        """
-        param = Object()
-        param._classname = 'PortalSyslogConfig'  # pylint: disable=protected-access
-        param.mode = Mode.Enabled
-        param.server = server
-        param.minSeverity = min_severity
-        param.port = port
-        param.protocol = protocol
-        param.useClientCertificate = False
-        logging.getLogger().info('Enabling syslog.')
-        response = self._portal.put('/settings/logsSettings/syslogConfig', param)
-        logging.getLogger().info('Syslog enabled.')
-        return response
+    def disable(self):
+        """ Disable Syslog """
+        logging.getLogger().info("Disabling syslog server.")
+        self._gateway.put('/config/logging/syslog/mode', enum.Mode.Disabled)
+        logging.getLogger().info("Syslog server disabled.")
+
+    def get_configuration(self):
+        return self._gateway.get('/config/logging/syslog')
 
-    def modify(self, server=None, port=None, protocol=None, min_severity=None):
+    def modify(self, server=None, port=None, proto=None, min_severity=None):
         """
-        Modify Syslog log forwarding configuration
+        Modify current Syslog configuration. Only configurations that are not None will be changed. Syslog must be enabled
 
-        :param str server: Syslog server address
-        :param int,optional port: Syslog server port
-        :param cterasdk.core.enum.IPProtocol,optional protocol: Syslog server IP protocol
-        :param cterasdk.core.enum.Severity,optional min_severity: Minimum log severity to forward
+        :param str,optional server: Server address to send syslog logs
+        :param int,optional port: Syslog server communication port
+        :param cterasdk.edge.enum.IPProtocol,optional proto: Syslog server communication protocol
+        :param cterasdk.edge.enum.Severity,optional min_severity: Minimal log severity to fetch
         """
         current_config = self.get_configuration()
-        if current_config.mode == Mode.Disabled:
+        if current_config.mode == enum.Mode.Disabled:
             raise CTERAException("Syslog configuration cannot be modified when disabled")
         if server:
             current_config.server = server
         if port:
             current_config.port = port
-        if protocol:
-            current_config.protocol = protocol
+        if proto:
+            current_config.proto = proto
         if min_severity:
             current_config.minSeverity = min_severity
 
         logging.getLogger().info("Updating syslog server configuration.")
-        self._portal.put('/settings/logsSettings/syslogConfig', current_config)
+        self._gateway.put('/config/logging/syslog', current_config)
         logging.getLogger().info(
             "Syslog server configured. %s",
             {
                 'server': current_config.server,
                 'port': current_config.port,
-                'protocol': current_config.protocol,
+                'protocol': current_config.proto,
                 'minSeverity': current_config.minSeverity
             }
         )
-
-    def disable(self):
-        logging.getLogger().info('Disabling syslog.')
-        response = self._portal.put('/settings/logsSettings/syslogConfig/mode', Mode.Disabled)
-        logging.getLogger().info('Syslog disabled.')
-        return response
```

### Comparing `cterasdk-2.8.32/cterasdk/core/taskmgr.py` & `cterasdk-2.9.0/cterasdk/core/taskmgr.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,17 +29,15 @@
         Get background task status
 
         :param str ref: Task reference
         """
         task = Task(self._portal, ref)
         return task.status()
 
-    def wait(self, ref, retries=100, seconds=1):
+    def wait(self, ref):
         """
         Wait for background task to complete
 
         :param str ref: Task reference
-        :param int,optional retries: Number of retries when sampling the task status, defaults to 100
-        :param int,optional seconds: Number of seconds to wait between retries, defaults to 1
         """
-        task = Task(self._portal, ref, retries, seconds)
+        task = Task(self._portal, ref)
         return task.wait()
```

### Comparing `cterasdk-2.8.32/cterasdk/core/zones.py` & `cterasdk-2.9.0/cterasdk/core/zones.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 
 class Zones(BaseCommand):
     """
     Portal Zones APIs
     """
 
-    name_attr = 'name'
-
     def get(self, name):
         """
         Get zone by name
 
         :param str name: The name of the zone to get
         :return: The requested zone
         """
@@ -37,41 +35,14 @@
             logging.getLogger().error('Zone not found. %s', {'name': name})
             raise CTERAException('Zone not found', None, name=name)
 
         zone = objects[0]
         logging.getLogger().info('Zone found. %s', {'name': name, 'id': zone.zoneId})
         return zone
 
-    def list_zones(self, filters=None):
-        """
-        List Zones
-        :param list[],optional filters: List of additional filters, defaults to None
-
-        :return: Iterator for all Zones
-        :rtype: cterasdk.lib.iterator.Iterator
-        """
-        builder = query.QueryParamBuilder().include_classname().startFrom(0).countLimit(25)
-        filters = filters or []
-        for query_filter in filters:
-            builder.addFilter(query_filter)
-        builder.orFilter((len(filters) > 1))
-        param = builder.build()
-        return query.iterator(self._portal, '', param, 'getZonesDisplayInfo')
-
-    def search(self, name):
-        """
-        Search for Zones by name
-        :param str name: Search query
-
-        :return: Iterator for all matching Zones
-        :rtype: cterasdk.lib.iterator.Iterator
-        """
-        filters = [query.FilterBuilder(Zones.name_attr).like(name)]
-        return self.list_zones(filters)
-
     def add(self, name, policy_type=enum.PolicyType.SELECT, description=None):
         """
         Add a new zone
 
         :param str name: The name of the new zone
         :param cterasdk.core.enum.PolicyType,optional policy_type:
          Policy type of the new zone, defaults to cterasdk.core.enum.PolicyType.SELECT
@@ -80,18 +51,18 @@
         param = self._zone_param(name, policy_type, description)
 
         logging.getLogger().info('Adding zone. %s', {'name': name})
 
         response = self._portal.execute('', 'addZone', param)
         try:
             self._process_response(response)
-            logging.getLogger().info('Zone added. %s', {'name': name})
         except CTERAException as error:
             logging.getLogger().error('Zone creation failed. %s', {'rc': response.rc})
             raise error
+        logging.getLogger().info('Zone added. %s', {'name': name})
 
     def delete(self, name):
         """
         Delete a zone
 
         :param str name: The name of the zone to delete
         """
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/afp.py` & `cterasdk-2.9.0/cterasdk/edge/afp.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/aio.py` & `cterasdk-2.9.0/cterasdk/edge/aio.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/array.py` & `cterasdk-2.9.0/cterasdk/edge/array.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 
 class Array(BaseCommand):
     """ Gateway Array APIs """
 
     def get(self, name=None):
         """
         Get Array. If an array name was not passed as an argument, a list of all arrays will be retrieved
-
         :param str,optional name: Name of the array
         """
         return self._gateway.get('/config/storage/arrays' + ('' if name is None else ('/' + name)))
 
-    def add(self, array_name, level, members=None):
+    def add(self, array_name, level, members):
         """
         Add a new array
 
         :param str array_name: Name for the new array
         :param RAIDLevel level: RAID level
-        :param list(str) members: Members of the array. If not specified, the system will try to create an array using all available drives
+        :param list(str) members: Members of the array
         """
         param = Object()
         param.name = array_name
         param.level = level
-        param.members = [drive.name for drive in self._gateway.drive.get_status()] if members is None else members
+        param.members = members
 
         try:
             logging.getLogger().info("Creating a storage array.")
             response = self._gateway.add("/config/storage/arrays", param)
             logging.getLogger().info("Storage array created.")
             return response
         except CTERAException as error:
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/audit.py` & `cterasdk-2.9.0/cterasdk/edge/audit.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/backup.py` & `cterasdk-2.9.0/cterasdk/edge/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 
+from ..lib.task_manager_base import TaskError
 from ..common import Object
 from ..exception import CTERAException
 from .enum import BackupConfStatusID
 from .base_command import BaseCommand
 from .directorytree import DirectoryTree
 
 
@@ -211,16 +212,19 @@
         elif rc == CreateFolderRC.PermissionDenied:
             logging.getLogger().error('Backup folder creation failed. %s', {'rc': rc})
         elif rc == CreateFolderRC.FolderAlreadyExists:
             return None
         raise CTERAException('Failed to create backup folder', None, rc=rc)
 
     def _wait(self, task):
-        task = self._gateway.tasks.wait(task)
-        return task.result
+        try:
+            task = self._gateway.tasks.wait(task)
+            return task.result
+        except TaskError:
+            pass
 
     def _configure_backup_settings(self, param):
         backup_settings = self._gateway.get('/config/backup')
         if not backup_settings:
             backup_settings = self._gateway.get('/defaults/BackupSettings')
 
         backup_settings.encryptionMode = param.encryptionMode
@@ -253,8 +257,8 @@
                     logging.getLogger().info('Found backup config. %s', {'name': name})
                     return backup_config
             logging.getLogger().error('Could not find backup config. %s', {'name': name})
             raise CTERAException('Could not find backup config', None, name=name)
         return backup_configs
 
     def _update_backup_config(self, backup_config):
-        return self._gateway.put(f'/config/backup/backupPolicy/includeSets/{backup_config._uuid}', backup_config)  # pylint: disable=W0212
+        return self._gateway.put('/config/backup/backupPolicy/includeSets/%s' % backup_config._uuid, backup_config)  # pylint: disable=W0212
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/cache.py` & `cterasdk-2.9.0/cterasdk/edge/cache.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/decorator.py` & `cterasdk-2.9.0/cterasdk/edge/decorator.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/directoryservice.py` & `cterasdk-2.9.0/cterasdk/edge/directoryservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 import logging
 
 from ..common import Object
 from ..exception import CTERAException, CTERAConnectionError
 from .base_command import BaseCommand
 from .types import TCPService
 
@@ -14,26 +13,29 @@
 
     def connected(self):
         """
         Get the Active Directory join status
         """
         return self._gateway.get('/status/fileservices/cifs/joinStatus') == 0
 
-    def connect(self, domain, username, password, ou=None, check_connection=False):
+    def connect(self, domain, username, password, ou=None):
         """
         Connect the Gateway to an Active Directory
 
         :param str domain: The active directory domain to connect to
         :param str username: The user name to use when connecting to the active directory services
         :param str password: The password to use when connecting to the active directory services
         :param str,optional ou: The OU path to use when connecting to the active directory services, defaults to None
-        :param bool,optional check_connection: Check connectivity before attempting to connect to directory services, defaults to `False`
         """
-        if check_connection:
-            self._check_domain_connectivity(domain)
+        port = 389
+        tcp_connect_result = self._gateway.network.tcp_connect(TCPService(domain, port))
+        if not tcp_connect_result.is_open:
+            logging.getLogger().error("Connection failed. No traffic allowed over port %(port)s", dict(port=tcp_connect_result.port))
+            raise CTERAConnectionError('Unable to establish connection', None, host=tcp_connect_result.host,
+                                       port=tcp_connect_result.port, protocol='LDAP')
 
         cifs = self._gateway.get('/config/fileservices/cifs')
         cifs.type = "domain"
         cifs.domain = domain
         cifs.workgroup = None
         self._gateway.put('/config/fileservices/cifs', cifs)
 
@@ -47,25 +49,14 @@
         try:
             self._gateway.execute("/status/fileservices/cifs", "joinDomain", param)
         except CTERAException as error:
             logging.getLogger().error("Failed connecting to Active Directory.")
             raise error
         logging.getLogger().info("Connected to Active Directory.")
 
-    def _check_domain_connectivity(self, domain):
-        port = 389
-        domain_controllers = self.get_static_domain_controller()
-        domain_controllers = re.findall(r'\b(?:[0-9]{1,3}\.){3}[0-9]{1,3}\b', domain_controllers) if domain_controllers else [domain]
-        connection_results = self._gateway.network.diagnose([TCPService(host, port) for host in domain_controllers])
-        for connection_result in connection_results:
-            if not connection_result.is_open:
-                logging.getLogger().error("Connection failed. No traffic allowed over port %(port)s", dict(port=connection_result.port))
-                raise CTERAConnectionError('Unable to establish connection', None, host=connection_result.host,
-                                           port=connection_result.port, protocol='LDAP')
-
     def get_static_domain_controller(self):
         """
         Retrieve the static domain controller configuration
 
         :return: A FQDN, hostname or ip address of the domain controller
         :rtype: str
         """
@@ -83,48 +74,32 @@
 
     def remove_static_domain_controller(self):
         """
         Delete the static domain controller configuration
         """
         self._gateway.put('/config/fileservices/cifs/passwordServer', None)
 
-    def get_advanced_mapping(self):
-        """
-        Retrieve directory services advanced mapping configuration
-
-        :returns: A dictionary of domain mapping objects
-        :rtype: dict
-        """
-        return {mapping.domainFlatName: mapping for mapping in self._gateway.get('/config/fileservices/cifs/idMapping/map')}
-
-    def set_advanced_mapping(self, mappings):
+    def advanced_mapping(self, domain, start, end):
         """
         Configure advanced mapping
 
-        :param list[cterasdk.common.types.ADDomainIDMapping] mappings: List of domains and their UID/GID mapping range
+        :param str domain: The active directory domain
+        :param str start: The minimum id to use for mapping
+        :param str end: The maximum id to use for mapping
         """
-        if not self.connected():
-            raise CTERAException('Failed to configure advanced mapping. Not connected to directory services.')
-
-        domains = self.domains()
-        advanced_mapping = self._gateway.get('/config/fileservices/cifs/idMapping/map')
-        advanced_mapping = []
+        mappings = self._gateway.get('/config/fileservices/cifs/idMapping/map')
         for mapping in mappings:
-            if mapping.domainFlatName in domains:
-                advanced_mapping.append(mapping)
-            else:
-                logging.getLogger().warning('Invalid mapping. Could not find domain. %s', {'domain': mapping.domainFlatName})
-
-        logging.getLogger().debug('Updating advanced mapping. %s', {
-            'domains': [mapping.domainFlatName for mapping in advanced_mapping]
-        })
-        response = self._gateway.put('/config/fileservices/cifs/idMapping/map', advanced_mapping)
-        logging.getLogger().info('Updated advanced mapping.')
+            if domain == mapping.domainFlatName:
+                mapping.minID = start
+                mapping.maxID = end
+                logging.getLogger().debug('Configuring advanced mapping. %s', {'domain': domain, 'start': start, 'end': end})
+                return self._gateway.put('/config/fileservices/cifs/idMapping/map', mappings)
 
-        return response
+        logging.getLogger().error('Could not find domain name. %s', {'domain': domain})
+        raise CTERAException('Could not find domain name', None, domain=domain, domains=self.domains())
 
     def get_connected_domain(self):
         """
         Get the connected domain information
 
         :return cterasdk.common.object.Object:
         """
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/directorytree.py` & `cterasdk-2.9.0/cterasdk/edge/directorytree.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,42 +83,42 @@
                 break
         return (node, parts)
 
     @staticmethod
     def _is_dir(node):
         return getattr(node, '_classname', 'DirEntry') == 'DirEntry'
 
-    # pylint: disable=R6301
+    # pylint: disable=R0201
     def _has_children(self, node):
         return node.children is not None
 
     def _get_child(self, node, child_name):
         if self._has_children(node):
-            for child in node.children:
-                if child.name == child_name:
-                    return child
+            for i in range(0, len(node.children)):
+                if node.children[i].name == child_name:
+                    return node.children[i]
         return None
 
-    # pylint: disable=R6301
+    # pylint: disable=R0201
     def _add_child(self, parent, node):
         node._parent = parent  # pylint: disable=protected-access
         if parent.children is None:
             parent.children = []
         parent.children.append(node)
 
     def _remove_child(self, parent, child_name):
-        ret = None
+        child = None
         if self._has_children(parent):
-            for i, child in enumerate(parent.children):
-                if child.name == child_name:
-                    ret = parent.children.pop(i)
+            for i in range(0, len(parent.children)):
+                if parent.children[i].name == child_name:
+                    child = parent.children.pop(i)
                     if not parent.children:
                         parent.children = None
                     break
-        return ret
+        return child
 
     def _populate_selection(self, parent, parts, is_dir, include):
         descendant_name = parts.pop()
         descendant = self._get_dir_entry(descendant_name, include) if is_dir else self._get_file_entry(descendant_name, include)
         for part in parts:
             child_node = self._get_dir_entry(part, parent.isIncluded)
             self._add_child(parent, child_node)
@@ -127,15 +127,14 @@
 
     def _get_file_entry(self, name, include):
         return self._get_entry(False, name, include)
 
     def _get_dir_entry(self, name, include):
         return self._get_entry(True, name, include)
 
-    # pylint: disable=R6301
     def _get_entry(self, is_dir, name, include):
         param = Object()
         param.displayName = None
         param.name = name
         param.isIncluded = include
         if is_dir:
             param._classname = 'DirEntry'  # pylint: disable=protected-access
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/drive.py` & `cterasdk-2.9.0/cterasdk/edge/drive.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/enum.py` & `cterasdk-2.9.0/cterasdk/edge/enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     :ivar str RAID_6: Dual parity
     """
     JBOD = "linear"
     RAID_0 = "0"
     RAID_1 = "1"
     RAID_5 = "5"
     RAID_6 = "6"
-    LVM = 'LVM'
 
 
 class BackupConfStatusID:
     """
     Status of backup configuration
 
     :ivar str NotInitialized: Backup configuration was not initialized
@@ -352,77 +351,7 @@
     NoFolder = "NoFolder"
     WrongPassword = "WrongPassword"
     Failed = "Failed"
     Unsubscribed = "Unsubscribed"
     Unlicensed = "Unlicensed"
     ClocksOutOfSync = "ClocksOutOfSync"
     GetFoldersList = "GetFoldersList"
-
-
-class Traffic:
-    """
-    Traffic type
-
-    :ivar str Upload: Upload
-    :ivar str Download: Download
-    """
-    Upload = 'Upload'
-    Download = 'Download'
-
-
-class SMBProtocol:
-    """
-    SMB Protocol
-
-    :ivar str SMB1: SMB v1
-    :ivar str NT1: SMB v1
-    :ivar str SMB2_02: Vista, Server 2008
-    :ivar str SMB2_10: Windows 7, Server 2008 R2
-    :ivar str SMB3_00: Windows 8, Server 2012
-    :ivar str SMB3_02: Windows 8.1, Server 2012 R2
-    :ivar str SMB3_11: Windows 10, Server 2016
-    :ivar str SMB2: Windows 7, Server 2008
-    :ivar str SMB3: SMB 3.1.1
-    """
-    SMB1 = 'NT1'
-    NT1 = SMB1
-    SMB2_02 = 'SMB2_02'
-    SMB2_10 = 'SMB2_10'
-    SMB3_00 = 'SMB3_00'
-    SMB3_02 = 'SMB3_02'
-    SMB3_11 = 'SMB3_11'
-    SMB2 = 'SMB2'
-    SMB3 = 'SMB3'
-
-
-class SourceType:
-    """
-    Source Host Type
-
-    :ivar str Edge: This Edge Filer
-    :ivar str Windows: Windows Server
-    :ivar str ONTAP: NetApp ONTAP
-    :ivar str OneFS: Isilon OneFS
-    :ivar str Panzura: Panzura Freedom Filer
-    :ivar str SGRID9_SMB: NetApp StorageGRID 9
-    :ivar str SGRID11_SMB: NetApp StorageGRID 11
-    :ivar str StorSimple: Microsoft Azure StorSimple
-    """
-    Edge = 'currentDevice'
-    Windows = 'windowsServer'
-    ONTAP = 'netapp'
-    OneFS = 'isilon'
-    Panzura = 'panzura'
-    SGRID9_SMB = 'storageGrid9'
-    SGRID11_SMB = 'storageGrid11'
-    StorSimple = 'azureStorSimple'
-
-
-class TaskType:
-    """
-    Migration Tool Task Type
-
-    :ivar str Discovery: Discovery
-    :ivar str Migration: Migration
-    """
-    Discovery = 0
-    Migration = 1
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/files/browser.py` & `cterasdk-2.9.0/cterasdk/edge/files/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         .. warning:: The list of files is not validated. The ZIP file will include only the existing  files and directories
 
         :param str cloud_directory: Path to the cloud directory
         :param list[str] files: List of files and/or directories in the cloud folder to download
         :param str,optional destination:
          File destination, if it is a directory, the filename will be calculated, defaults to the default directory
         """
-        return self._file_access.download_as_zip(self.mkpath(cloud_directory), files, destination=destination)
+        self._file_access.download_as_zip(self.mkpath(cloud_directory), files, destination=destination)
 
     def upload(self, file_path, server_path):
         """
         Upload a file
 
         :param str file_path: Path to the local file to upload
         :param str server_path: Path to the directory to upload the file to
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/files/file_access.py` & `cterasdk-2.9.0/cterasdk/edge/files/file_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
     def _get_upload_url(self, dest_path):
         return '/actions/upload'
 
     def _get_upload_form(self, local_file_info, fd, dest_path):
         return dict(
             name=local_file_info['name'],
-            fullpath=f'{dest_path.fullpath()}/{local_file_info["name"]}',
+            fullpath='%s/%s' % (dest_path.fullpath(), local_file_info['name']),
             filedata=(local_file_info['name'], fd, local_file_info['mimetype'][0])
         )
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/files/mkdir.py` & `cterasdk-2.9.0/cterasdk/edge/files/mkdir.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/files/path.py` & `cterasdk-2.9.0/cterasdk/edge/files/path.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/firmware.py` & `cterasdk-2.9.0/cterasdk/edge/firmware.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,10 +46,10 @@
         while True:
             task_status = self._gateway.get(task_pointer)
             is_running = task_status.status == UploadTaskStatus.IN_PROGRESS
             if not is_running:
                 if task_status.status == UploadTaskStatus.COMPLETE:
                     return
                 raise CTERAException(
-                    message=f'Filer failed to receive the new firmware - {task_status.statusMessage}',
+                    message='Filer failed to receive the new firmware - %s' % task_status.statusMessage,
                     instance=task_status
                 )
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/ftp.py` & `cterasdk-2.9.0/cterasdk/edge/ftp.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/groups.py` & `cterasdk-2.9.0/cterasdk/edge/groups.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/login.py` & `cterasdk-2.9.0/cterasdk/edge/login.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,17 @@
         return self._gateway.get('/nosession/logininfo')
 
     def login(self, username, password):
         host = self._gateway.host()
         try:
             self._gateway.form_data('/login', {'username': username, 'password': password})
             logging.getLogger().info("User logged in. %s", {'host': host, 'user': username})
-            self._gateway.mtool.login()
         except CTERAException as error:
             logging.getLogger().error("Login failed. %s", {'host': host, 'user': username})
             raise error
 
     def logout(self):
-        host = self._gateway.host()
-        user = self._gateway.session().user
         try:
             self._gateway.form_data('/logout', {'foo': 'bar'})
-            logging.getLogger().info("User logged out. %s", {'host': self._gateway.host(), 'user': user})
+            logging.getLogger().info("User logged out. %s", {'host': self._gateway.host()})
         except CTERAException as error:
-            logging.getLogger().error("Logout failed. %s", {'host': host, 'user': user})
             raise error
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/logs.py` & `cterasdk-2.9.0/cterasdk/edge/logs.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/mail.py` & `cterasdk-2.9.0/cterasdk/edge/mail.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/ntp.py` & `cterasdk-2.9.0/cterasdk/edge/ntp.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 from .enum import Mode
 from .base_command import BaseCommand
 
 
 class NTP(BaseCommand):
     """ Gateway NTP configuration """
 
-    def get_configuration(self):
-        return self._gateway.get('/config/time')
-
-    @property
-    def servers(self):
-        return self._gateway.get('/config/time/NTPServer')
-
     def enable(self, servers=None):
         """
         Enable NTP
 
         :param list[str] servers: List of NTP servers address
         """
         logging.getLogger().info("Enabling time synchronization with ntp servers.")
+
         self._gateway.put('/config/time/NTPMode', Mode.Enabled)
+
         logging.getLogger().info("Time synchronization enabled.")
 
         if servers:
             logging.getLogger().info("Updating time servers. %s", {'servers': servers})
+
             self._gateway.put('/config/time/NTPServer', servers)
+
             logging.getLogger().info("Time servers updated. %s", {'servers': servers})
 
     def disable(self):
         """ Disable NTP """
         logging.getLogger().info("Disabling time synchronization with ntp servers.")
+
         self._gateway.put('/config/time/NTPMode', Mode.Disabled)
+
         logging.getLogger().info("Time synchronization disabled.")
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/power.py` & `cterasdk-2.9.0/cterasdk/edge/power.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 class Power(BaseCommand):
     """ Gateway Power APIs """
 
     def reboot(self, wait=False):
         """
         Reboot the Gateway
 
-        :param bool,optional wait: Wait for reboot to complete, defaults to False
+        :param bool,optional wait: Wait got the reboot to complete, defaults to False
         """
         logging.getLogger().info("Rebooting device. %s", {'host': self._gateway.host()})
         self._gateway.execute("/status/device", "reboot", None)
         if wait:
             Boot(self._gateway).wait()
 
     def shutdown(self):
         """ Shutdown the Gateway """
         self._gateway.execute("/status/device", "poweroff", None)
 
     def reset(self, wait=False):
         """
         Reset the Gateway setting
 
-        :param bool,optional wait: Wait for reset to complete, defaults to False
+        :param bool,optional wait: Wait got the reset to complete, defaults to False
         """
         self._gateway.execute("/status/device", "reset2default", None)
         logging.getLogger().info("Resetting device to default settings. %s", {'host': self._gateway.host()})
         if wait:
             Boot(self._gateway).wait()
 
 
@@ -48,15 +48,15 @@
             try:
                 self._increment()
                 logging.getLogger().debug('Checking if device is up and running. %s', {'attempt': self._attempt})
                 self._gateway.test()
                 logging.getLogger().info("Device is back up and running.")
                 break
             except (HostUnreachable, ExhaustedException) as e:
-                logging.getLogger().debug('Exception. %s', {'exception': e.__class__.__name__, 'message': e.message})
+                logging.getLogger().debug('Exception. %s', {'exception': e.classname, 'message': e.message})
 
     def _increment(self):
         self._attempt = self._attempt + 1
         if self._attempt >= self._retries:
             self._unreachable()
         logging.getLogger().debug('Sleep. %s', {'seconds': self._seconds})
         time.sleep(self._seconds)
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/query.py` & `cterasdk-2.9.0/cterasdk/edge/query.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/remote.py` & `cterasdk-2.9.0/cterasdk/edge/remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def login(Gateway, ticket):
     logging.getLogger().debug("Logging in using SSO ticket. %s", {'device': Gateway.host()})
     Gateway.get('/ssologin', {'ticket': ticket})
 
 
 def obtain_ticket(Portal, device_name):
     tenant = Portal.session().tenant()
-    url = f'/portals/{tenant}/devices/{device_name}'
+    url = '/portals/%s/devices/%s' % (tenant, device_name)
     logging.getLogger().debug("Obtaining SSO ticket. %s", {'tenant': tenant, 'device': device_name})
 
     ticket = Portal.execute(url, 'singleSignOn')
     if not ticket:
         logging.getLogger().error('Could not obtain SSO ticket. %s', {'tenant': tenant, 'device': device_name})
         raise CTERAException('Could not obtain SSO ticket.')
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/rsync.py` & `cterasdk-2.9.0/cterasdk/edge/rsync.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/services.py` & `cterasdk-2.9.0/cterasdk/edge/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def get_status(self):
         """
         Retrieve the cloud services connection status
         """
         status = self._gateway.get('/status/services')
         connection = Object()
-        connection.connected = status.CTERAPortal.connectionState == enum.ServicesConnectionState.Connected
+        connection.connected = (status.CTERAPortal.connectionState == enum.ServicesConnectionState.Connected)
         if connection.connected:
             connection.ipaddr = status.CTERAPortal.connectedAddress
             connection.user = status.userDisplayName
             connection.server_version = status.portalVersion
             connection.server_address = status.CTERAPortal.serverList[0].name
             connection.last_connected_at = status.CTERAPortal.establishedTime
         return connection
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/session.py` & `cterasdk-2.9.0/cterasdk/edge/session.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/shell.py` & `cterasdk-2.9.0/cterasdk/edge/shell.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/support.py` & `cterasdk-2.9.0/cterasdk/edge/support.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/taskmgr.py` & `cterasdk-2.9.0/cterasdk/edge/taskmgr.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         """
         Get background tasks by name
 
         :param str name: Task name
         """
         return self._gateway.query('/proc/bgtasks', 'name', name)
 
-    def wait(self, ref, retries=100, seconds=1):
+    def wait(self, ref):
         """
         Wait for background task to complete
 
         :param str ref: Task reference
-        :param int,optional retries: Number of retries when sampling the task status, defaults to 100
-        :param int,optional seconds: Number of seconds to wait between retries, defaults to 1
         """
-        task = Task(self._gateway, ref, retries, seconds)
+        task = Task(self._gateway, ref)
         return task.wait()
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/telnet.py` & `cterasdk-2.9.0/cterasdk/edge/telnet.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/timezone.py` & `cterasdk-2.9.0/cterasdk/edge/timezone.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/edge/uri.py` & `cterasdk-2.9.0/cterasdk/edge/uri.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,29 +19,29 @@
         return remote(baseurl, base_object_ref.name, device)  # remote, without a Gateway session
 
     logging.getLogger().error('Invalid connection type.')
     raise CTERAException('Invalid connection type', session)
 
 
 def local(baseurl):
-    return f'{baseurl}/admingui/api'
+    return '%s/admingui/api' % (baseurl)
 
 
 def remote(baseurl, tenant, device):
-    return f'{baseurl}/devicecmdnew/{tenant}/{device}/'
+    return '%s/devicecmdnew/%s/%s/' % (baseurl, tenant, device)
 
 
 def remote_access(baseurl, device):
-    return f'{baseurl}/devices/{device}/admingui/api'
+    return '%s/devices/%s/admingui/api' % (baseurl, device)
 
 
 def files(Gateway):
     session = Gateway.session()
     if session.local():
         return Gateway.baseurl()
 
     if session.remote():
         if session.remote_access():
             baseurl = Gateway._Portal.base_portal_url  # pylint: disable=protected-access
             device = Gateway.host()
-            return f'{baseurl}/devices/{device}'
+            return '%s/devices/%s' % (baseurl, device)
     raise CTERAException('Invalid connection type', session)
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/users.py` & `cterasdk-2.9.0/cterasdk/edge/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class Users(BaseCommand):
     """ Gateway Users configuration APIs """
 
     def get(self, name=None):
         """
         Get User. If a user name was not passed as an argument, a list of all local users will be retrieved
-
         :param str,optional name: Name of the user
         """
         return self._gateway.get('/config/auth/users' + ('' if name is None else ('/' + name)))
 
     def add_first_user(self, username, password, email=''):
         """
         Add the first user of the Gateway and login
```

### Comparing `cterasdk-2.8.32/cterasdk/edge/volumes.py` & `cterasdk-2.9.0/cterasdk/edge/volumes.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/exception.py` & `cterasdk-2.9.0/cterasdk/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .common import Object
 from .convert import tojsonstr
 
 
 class CTERAException(Exception):
 
     def __init__(self, message=None, instance=None, **kwargs):
         super().__init__()
@@ -24,26 +23,14 @@
         return tojsonstr(self)
 
 
 class CTERAClientException(CTERAException):
     pass
 
 
-class ObjectNotFoundException(CTERAException):
-
-    def __init__(self, message, object_ref, **kwargs):
-        super().__init__(message, None, **kwargs)
-        self.response = Object()
-        self.response.code = 404
-        self.response.reason = 'Not Found'
-        self.response.body = Object()
-        self.response.body.rc = 1
-        self.response.body.msg = f"Object '{object_ref}' not found"
-
-
 class CTERAConnectionError(CTERAException):
 
     def __init__(self, message, instance, host, port, protocol, **kwargs):
         super().__init__(message, instance, host=host, port=port, protocol=protocol, **kwargs)
 
 
 class ConnectionTimeout(CTERAException):
@@ -72,14 +59,20 @@
 
 class SSLException(CTERAConnectionError):
 
     def __init__(self, host, port, reason):
         super().__init__('Untrusted security certificate', None, host=host, port=port, protocol='TLS', reason=reason)
 
 
+class ParserException(CTERAException):
+
+    def __init__(self, fmt, payload):
+        CTERAException.__init__(self, 'Conversion falied', None, fmt=fmt, to='Python Object', payload=payload)
+
+
 class InputError(CTERAException):
 
     def __init__(self, message, expression, options):
         CTERAException.__init__(self, message, None, expression=expression, options=options)
 
 
 class ConsentException(CTERAException):
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/file_access_base.py` & `cterasdk-2.9.0/cterasdk/lib/file_access_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     def __init__(self, ctera_host):
         self._ctera_host = ctera_host
         self._filesystem = FileSystem.instance()
 
     def download(self, path, destination=None):
         directory, filename = self._split_destination(destination, path.name)
         handle = self._openfile(path)
-        return self._filesystem.save(directory, filename, handle)
+        self._filesystem.save(directory, filename, handle)
 
     def download_as_zip(self, cloud_directory, files, destination=None):
         files = files if isinstance(files, list) else [files]
         directory, filename = self._split_destination(
             destination,
             self._filesystem.compute_zip_file_name,
             cloud_directory=cloud_directory.fullpath(),
             files=files
         )
         handle = self._get_zip_file_handle(cloud_directory, files)
-        return self._filesystem.save(directory, filename, handle)
+        self._filesystem.save(directory, filename, handle)
 
     def upload(self, local_file, dest_path):
         local_file_info = self._filesystem.get_local_file_info(local_file)
         with open(local_file, 'rb') as fd:
             return self._ctera_host.upload(
                 self._get_upload_url(dest_path),
                 self._get_upload_form(local_file_info, fd, dest_path),
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/filesystem.py` & `cterasdk-2.9.0/cterasdk/lib/filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import mimetypes
-import shutil
 import os
 from pathlib import Path
 
 from .. import config
 from ..exception import RenameException, LocalDirectoryNotFound, LocalFileNotFound, LocalPathNotFound
 
 
-class FileSystem:  # pylint: disable=unused-private-member
+class FileSystem:
 
     __instance = None
 
     @staticmethod
     def instance():
         if FileSystem.__instance is None:
             FileSystem()
@@ -41,18 +40,14 @@
         raise RenameException(dirpath, src, dst)
 
     def validate_directory(self, dirpath):
         dirpath = os.path.expanduser(dirpath)
         if not self.exists(dirpath):
             raise LocalDirectoryNotFound(dirpath)
 
-    def copyfile(self, src, dst):
-        self.get_local_file_info(src)
-        return shutil.copyfile(src, dst)
-
     def save(self, dirpath, filename, handle):
         dirpath = os.path.expanduser(dirpath)
         if not self.exists(dirpath):
             raise LocalDirectoryNotFound(dirpath)
 
         tempfile = filename + '.Chopin3'
         filepath = os.path.join(dirpath, tempfile)
@@ -83,19 +78,16 @@
         else:
             name = filename
         return name + ' ' + '(' + str(version) + ')' + extension
 
     @staticmethod
     def write(filepath, handle):
         with open(filepath, 'w+b') as fd:
-            if isinstance(handle, bytes):
-                fd.write(handle)
-            else:
-                for chunk in handle.iter_content(chunk_size=8192):
-                    fd.write(chunk)
+            for chunk in handle.iter_content(chunk_size=8192):
+                fd.write(chunk)
         logging.getLogger().debug('Saved temporary file. %s', {'path': filepath})
 
     @staticmethod
     def get_local_file_info(local_file):
         path = Path(local_file)
         if not path.exists():
             logging.getLogger().error('The path %(local_file)s was not found', dict(local_file=local_file))
@@ -125,52 +117,25 @@
         except LocalDirectoryNotFound as error:
             dirpath = self.expanduser(dirpath)
             logging.getLogger().error('Download failed. Check the following directory exists. %s', {'path': dirpath})
             raise error
         return dirpath
 
     @staticmethod
-    def join(*paths):
-        return os.path.join(*paths)
-
-    @staticmethod
     def split_file_directory(path):
         # Exists and file -> directory=parent, filename=name
         # Exists and dir -> directory=current filename=None
         # Not Exists and parent Exists -> directory=parent filename=name
         # Not Exists and parent not Exists -> Error
-        path = os.path.expanduser(path)
         p = Path(path)
         if p.exists():
             if p.is_dir():
                 filename = None
             else:
                 filename = p.name
                 p = p.parent
         elif p.parent.exists():
             filename = p.name
             p = p.parent
         else:
             raise LocalPathNotFound(path)
         return str(p.resolve()), filename
-
-    @staticmethod
-    def split_file_directory_with_defaults(path=None, default_filename=None):
-        """
-        Compute the destination file path.
-
-        :param str path: A path to a file or a folder
-        :param str default_filename: The default file name to use unless `path` argument specifies a file path
-
-        :returns: A tuple including the destination directory and filename
-        :rtype: (string, string)
-        """
-        directory = filename = None
-        if path:
-            directory, filename = FileSystem.split_file_directory(path)
-        else:
-            directory = FileSystem.instance().get_dirpath()
-
-        if not filename:
-            filename = default_filename
-
-        return (directory, filename)
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/iterator.py` & `cterasdk-2.9.0/cterasdk/lib/iterator.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/lib/platform.py` & `cterasdk-2.9.0/cterasdk/lib/platform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import platform
 
 
-class Platform:  # pylint: disable=unused-private-member
+class Platform:
 
     __instance = None
 
     @staticmethod
     def instance():
         if Platform.__instance is None:
             Platform()
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/registry.py` & `cterasdk-2.9.0/cterasdk/lib/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class Registry:  # pylint: disable=unused-private-member
+class Registry:
 
     __instance = None
 
     @staticmethod
     def instance():
         if Registry.__instance is None:
             Registry()
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/session_base.py` & `cterasdk-2.9.0/cterasdk/lib/session_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,13 +46,9 @@
 
     def authenticated(self):
         return self.status == SessionStatus.Active
 
     def is_local_auth(self):
         return self.local_auth
 
-    @property
-    def active(self):
-        return self.status == SessionStatus.Active
-
     def whoami(self):
         print(self)
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/task_manager_base.py` & `cterasdk-2.9.0/cterasdk/lib/task_manager_base.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/lib/tempfile.py` & `cterasdk-2.9.0/cterasdk/lib/tempfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tempfile
 
 from .registry import Registry
 
 
 class TempfileServices:
 
-    __tempdir_prefix = 'cterasdk-'
+    __tempdir_prefix = 'chopin_core-'
 
     @staticmethod
     def mkdir():
         registry = Registry.instance()
         tempdir = registry.get('tempdir')
         if tempdir is None:
             logging.getLogger().debug('Creating temporary directory.')
```

### Comparing `cterasdk-2.8.32/cterasdk/lib/tracker.py` & `cterasdk-2.9.0/cterasdk/lib/tracker.py`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/lib/version.py` & `cterasdk-2.9.0/cterasdk/lib/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .platform import Platform
 
 
-class Version:  # pylint: disable=unused-private-member
+class Version:
 
     __instance = None
 
     @staticmethod
     def instance():
         if Version.__instance is None:
             Version()
@@ -15,14 +15,19 @@
         if Version.__instance is not None:
             raise Exception("Version is a singleton class.")
 
         self.product = 'Chopin'
         self.product_version = '3.0'
         self.system = Platform.instance().os()
         self.machine = Platform.instance().arch()
-        self.header = \
-            f"{self.product}/{self.product_version} ({self.system}; {self.machine}) Python-urllib/{Platform.instance().python_version()}"
+        self.header = "{product}/{version} ({system}; {machine}) Python-urllib/{python_version}".format(
+            product=self.product,
+            version=self.product_version,
+            system=self.system,
+            machine=self.machine,
+            python_version=Platform.instance().python_version()
+        )
         Version.__instance = self
 
     def as_header(self):
 
         return self.header
```

### Comparing `cterasdk-2.8.32/cterasdk/object/Gateway.py` & `cterasdk-2.9.0/cterasdk/object/Gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,26 @@
 from ..edge import aio
 from ..edge import array
 from ..edge import audit
 from ..edge import backup
 from ..edge import cache
 from ..edge import cli
 from ..edge import config
-from ..edge import dedup
 from ..edge import directoryservice
 from ..edge import drive
 from ..edge import ftp
 from ..edge import groups
-from ..edge import migration_tool
 from ..edge import licenses
 from ..edge import login
 from ..edge import logs
 from ..edge import mail
 from ..edge import network
 from ..edge import nfs
 from ..edge import ntp
-from ..edge import snmp
 from ..edge import ssl
-from ..edge import ssh
 from ..edge import power
 from ..edge import rsync
 from ..edge import services
 from ..edge import session
 from ..edge import shares
 from ..edge import shell
 from ..edge import smb
@@ -60,21 +56,18 @@
     :ivar cterasdk.edge.syslog.Syslog syslog: Object holding the Gateway Syslog APIs
     :ivar cterasdk.edge.taskmgr.Tasks tasks: Object holding the Gateway Background Tasks APIs
     :ivar cterasdk.edge.audit.Audit audit: Object holding the Gateway Audit APIs
     :ivar cterasdk.edge.mail.Mail mail: Object holding the Gateway Mail APIs
     :ivar cterasdk.edge.backup.Backup backup: Object holding the Gateway Backup APIs
     :ivar cterasdk.edge.sync.Sync sync: Object holding the Gateway Sync APIs
     :ivar cterasdk.edge.cache.Cache cache: Object holding the Gateway Cache APIs
-    :ivar cterasdk.edge.snmp.SNMP snmp: Object holding the Gateway SNMP APIs
     :ivar cterasdk.edge.ssl.SSL ssl: Object holding the Gateway SSL APIs
-    :ivar cterasdk.edge.ssl.SSH ssh: Object holding the Gateway SSH APIs
     :ivar cterasdk.edge.power.Power power: Object holding the Gateway Power APIs
     :ivar cterasdk.edge.users.Users users: Object holding the Gateway Users APIs
     :ivar cterasdk.edge.groups.Groups groups: Object holding the Gateway Groups APIs
-    :ivar cterasdk.edge.migration_tool.MigrationTool mtool: Object holding the Edge Filer's Migration Tool APIs
     :ivar cterasdk.edge.drive.Drive drive: Object holding the Gateway Drive APIs
     :ivar cterasdk.edge.volumes.Volumes volumes: Object holding the Gateway Volumes APIs
     :ivar cterasdk.edge.array.Array array: Object holding the Gateway Array APIs
     :ivar cterasdk.edge.shares.Shares shares: Object holding the Gateway Shares APIs
     :ivar cterasdk.edge.smb.SMB smb: Object holding the Gateway SMB APIs
     :ivar cterasdk.edge.aio.AIO aio: Object holding the Gateway AIO APIs
     :ivar cterasdk.edge.ftp.FTP ftp: Object holding the Gateway FTP APIs
@@ -82,18 +75,17 @@
     :ivar cterasdk.edge.nfs.NFS nfs: Object holding the Gateway NFS APIs
     :ivar cterasdk.edge.rsync.RSync rsync: Object holding the Gateway RSync APIs
     :ivar cterasdk.edge.timezone.Timezone timezone: Object holding the Gateway Timezone APIs
     :ivar cterasdk.edge.logs.Logs logs: Object holding the Gateway Logs APIs
     :ivar cterasdk.edge.ntp.NTP ntp: Object holding the Gateway NTP APIs
     :ivar cterasdk.edge.shell.Shell shell: Object holding the Gateway Shell APIs
     :ivar cterasdk.edge.cli.CLI cli: Object holding the Gateway CLI APIs
-    :ivar cterasdk.edge.dedup.Dedup dedup: Object holding the Gateway Local Deduplication APIs
     :ivar cterasdk.edge.support.Support support: Object holding the Gateway Support APIs
     :ivar cterasdk.edge.files.FileBrowser files: Object holding the Gateway File Browsing APIs
-    :ivar cterasdk.edge.firmware.Firmware firmware: Object holding the Gateway Firmware APIs
+    :ivar cterasdk.edge.firmware.Fireware firmware: Object holding the Gateway Firmware APIs
     """
 
     def __init__(self, host, port=None, https=False, Portal=None):
         """
         :param str host: The fully qualified domain name, hostname or an IPv4 address of the Gateway
         :param int,optional port: Set a custom port number (0 - 65535), If not set defaults to 80 for http and 443 for https
         :param bool,optional https: Set to True to require HTTPS, defaults to False
@@ -103,29 +95,26 @@
         self._remote_access = False
         self._session = session.Session(self.host())
         if Portal is not None:
             self._Portal = Portal
             self._ctera_client = Portal._ctera_client
             self._session.start_remote_session(self._Portal.session())
         self.config = config.Config(self)
-        self.dedup = dedup.Dedup(self)
         self.network = network.Network(self)
         self.licenses = licenses.Licenses(self)
         self.services = services.Services(self)
         self.directoryservice = directoryservice.DirectoryService(self)
         self.telnet = telnet.Telnet(self)
         self.syslog = syslog.Syslog(self)
         self.audit = audit.Audit(self)
         self.mail = mail.Mail(self)
         self.backup = backup.Backup(self)
         self.sync = sync.Sync(self)
         self.cache = cache.Cache(self)
-        self.snmp = snmp.SNMP(self)
         self.ssl = ssl.SSL(self)
-        self.ssh = ssh.SSH(self)
         self.power = power.Power(self)
         self.users = users.Users(self)
         self.groups = groups.Groups(self)
         self.drive = drive.Drive(self)
         self.volumes = volumes.Volumes(self)
         self.array = array.Array(self)
         self.shares = shares.Shares(self)
@@ -140,15 +129,14 @@
         self.ntp = ntp.NTP(self)
         self.shell = shell.Shell(self)
         self.cli = cli.CLI(self)
         self.support = support.Support(self)
         self.files = files.FileBrowser(self)
         self.firmware = firmware.Firmware(self)
         self.tasks = taskmgr.Tasks(self)
-        self.mtool = migration_tool.MigrationTool(self)
 
     @property
     def base_api_url(self):
         return uri.api(self)
 
     @property
     def base_file_url(self):
@@ -156,15 +144,15 @@
 
     @property
     def _session_id_key(self):
         return '_cteraSessionId_'
 
     @staticmethod
     def make_local_files_dir(full_path):
-        return f'localFiles/{full_path}'
+        return 'localFiles/%s' % full_path
 
     @property
     def _omit_fields(self):
         return super()._omit_fields + [
             'config',
             'network',
             'licenses',
@@ -173,17 +161,15 @@
             'telnet',
             'syslog',
             'audit',
             'mail',
             'backup',
             'sync',
             'cache',
-            'snmp',
             'ssl',
-            'ssh',
             'power',
             'users',
             'groups',
             'drive',
             'volumes',
             'array',
             'shares',
@@ -209,22 +195,18 @@
         return login.Login(self)
 
     @property
     def initialized(self):
         return not login.Login(self).info().isfirstlogin
 
     def _is_authenticated(self, function, *args, **kwargs):
-
         def is_nosession(path):
             return path.startswith('/nosession')
-
-        def is_migration_auth(path):
-            return path.startswith('/migration/rest/v1/auth/user')
         current_session = self.session()
-        return current_session.authenticated() or current_session.initializing() or is_nosession(args[0]) or is_migration_auth(args[0])
+        return current_session.authenticated() or current_session.initializing() or is_nosession(args[0])
 
     def test(self):
         """ Verification check to ensure the target host is a Gateway. """
         return connection.test(self)
 
     def remote_access(self):
         remote.remote_access(self, self._Portal)
```

### Comparing `cterasdk-2.8.32/cterasdk/object/Portal.py` & `cterasdk-2.9.0/cterasdk/object/Portal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,70 @@
 from ..client import CTERAHost, authenticated
-from ..core import connection, messaging
+from ..core import connection
 from ..core import activation
 from ..core import antivirus
-from ..core import buckets
-from ..core import cli
 from ..core import decorator
 from ..core import directoryservice
-from ..core import firmwares
 from ..core import login
 from ..core import query
 from ..core import logs
 from ..core import portals
 from ..core import plans
 from ..core import reports
 from ..core import servers
 from ..core import devices
 from ..core import session
-from ..core import storage_classes
 from ..core import users
 from ..core import cloudfs
 from ..core import zones
-from ..core import settings
 from ..core import setup
-from ..core import ssl
 from ..core import startup
-from ..core import syslog
 from ..core import taskmgr
-from ..core import templates
 from ..core import uri
 from ..core import files
-from ..core import admins
 
 
 class Portal(CTERAHost):  # pylint: disable=too-many-instance-attributes
     """
     Parent class for communicating with the Portal through either GlobalAdmin or ServicesPortal
 
     :ivar cterasdk.core.users.Users users: Object holding the Portal user APIs
-    :ivar cterasdk.core.admins.Administrators admins: Object holding the Portal GlobalAdmin users APIs
     :ivar cterasdk.core.plans.Plans plans: Object holding the Plan APIs
     :ivar cterasdk.core.reports.Reports reports: Object holding the Portal reports APIs
     :ivar cterasdk.core.devices.Devices devices: Object holding the Portal devices APIs
     :ivar cterasdk.core.directoryservice.DirectoryService directoryservice: Object holding the Portal Active Directory Service APIs
     :ivar cterasdk.core.zones.Zones zones: Object holding the Portal zones APIs
     :ivar cterasdk.core.activation.Activation activation: Object holding the Portal activation APIs
+    :ivar cterasdk.core.antivirus.Antivirus antivirus: Object holding the Portal Antivirus APIs
     :ivar cterasdk.core.logs.Logs logs: Object holding the Portal logs APIs
     :ivar cterasdk.core.cloudfs.CloudFS cloudfs: Object holding the Portal CloudFS APIs
-    :ivar cterasdk.core.settings.Settings settings: Object holding the Portal Settings APIs
-    :ivar cterasdk.core.settings.StorageClasses storage_classes: Object holding the Portal Storage Classes APIs
     :ivar cterasdk.core.taskmgr.Tasks tasks: Object holding the Portal Background Tasks APIs
-    :ivar cterasdk.core.templates.Templates templates: Object holding the Portal Configuration Templates APIs
-    :ivar cterasdk.core.firmwares.Firmwares firmwares: Object holding the Portal Firmware Repository APIs
     :ivar cterasdk.core.files.browser.FileBrowser files: Object holding the Portal File Browsing APIs
     """
 
     def __init__(self, host, port, https):
         """
         :param str host: The fully qualified domain name, hostname or an IPv4 address of the Gateway
         :param int port: Set a custom port number (0 - 65535)
         :param bool https: Set to True to require HTTPS
         """
         super().__init__(host, port, https)
         self._session = session.Session(self.host(), self.context)
         self.users = users.Users(self)
-        self.admins = admins.Administrators(self)
         self.reports = reports.Reports(self)
         self.plans = plans.Plans(self)
         self.devices = devices.Devices(self)
         self.directoryservice = directoryservice.DirectoryService(self)
         self.zones = zones.Zones(self)
         self.cloudfs = cloudfs.CloudFS(self)
         self.activation = activation.Activation(self)
-        self.files = files.CloudDrive(self, self.cloud_drive_base_path)
-        self.backups = files.Backups(self, self.backups_base_path)
+        self.antivirus = antivirus.Antivirus(self)
+        self.files = files.FileBrowser(self, self.file_browser_base_path)
         self.logs = logs.Logs(self)
-        self.settings = settings.Settings(self)
-        self.storage_classes = storage_classes.StorageClasses(self)
         self.tasks = taskmgr.Tasks(self)
-        self.templates = templates.Templates(self)
-        self.firmwares = firmwares.Firmwares(self)
 
     @property
     def base_api_url(self):
         return uri.api(self)
 
     @property
     def base_portal_url(self):
@@ -97,54 +79,47 @@
         return 'JSESSIONID'
 
     @property
     def context(self):
         raise NotImplementedError("Implementing class must implement the context property")
 
     @property
-    def cloud_drive_base_path(self):
-        raise NotImplementedError("Implementing class must implement the cloud_drive_base_path property")
-
-    @property
-    def backups_base_path(self):
-        raise NotImplementedError("Implementing class must implement the backups_base_path property")
+    def file_browser_base_path(self):
+        raise NotImplementedError("Implementing class must implement the file_browser_base_path property")
 
     @property
     def _omit_fields(self):
         return super()._omit_fields + [
-            'admins',
             'users',
             'reports',
             'plans',
             'devices',
             'directoryservice',
             'zones',
             'cloudfs',
             'activation',
+            'antivirus',
             'files',
             'logs',
-            'settings',
-            'tasks',
-            'templates',
-            'firmwares'
+            'tasks'
         ]
 
     @property
     def _login_object(self):
         return login.Login(self)
 
     def _is_authenticated(self, function, *args, **kwargs):
         def is_public(path):
-            return path.startswith(f'/{self.context}/public')
+            return path.startswith('/%s/public' % self.context)
 
         def is_setup(path):
-            return path.startswith(f'/{self.context}/setup')
+            return path.startswith('/%s/setup' % self.context)
 
         def is_startup(path):
-            return path.startswith(f'/{self.context}/startup')
+            return path.startswith('/%s/startup' % self.context)
         current_session = self.session()
         return current_session.authenticated() or current_session.initializing() or \
             is_public(args[0]) or is_setup(args[0]) or is_startup(args[0]) or \
             current_session.is_local_auth()
 
     def test(self):
         """ Verification check to ensure the target host is a Portal. """
@@ -156,76 +131,59 @@
         return self.get('/' + self.context + '/public/publicInfo', params={}, use_file_url=True)
 
     @decorator.update_current_tenant
     def put(self, path, value, use_file_url=False):
         return super().put(path, value, use_file_url=use_file_url)
 
     @authenticated
-    def query(self, path, name, param):
-        return query.query(self, path, name, param)
+    def query(self, path, param):
+        return query.query(self, path, param)
 
     @authenticated
-    def show_query(self, path, name, param):
-        return query.show(self, path, name, param)
+    def show_query(self, path, param):
+        return query.show(self, path, param)
 
     def iterator(self, path, param):
         return query.iterator(self, path, param)
 
 
-class GlobalAdmin(Portal):  # pylint: disable=too-many-instance-attributes
+class GlobalAdmin(Portal):
     """
     Main class for Global Admin operations on a Portal
 
     :ivar cterasdk.core.portals.Portals portals: Object holding the Portals Management APIs
-    :ivar cterasdk.core.cli.CLI cli: Object holding the Portal GlobalAdmin CLI APIs
     :ivar cterasdk.core.servers.Servers servers: Object holding the Servers Management APIs
     :ivar cterasdk.core.setup.Setup setup: Object holding the Portal setup APIs
-    :ivar cterasdk.core.ssl.SSL ssl: Object holding the Portal SSL Certificate APIs
     :ivar cterasdk.core.startup.Startup startup: Object holding the Portal startup APIs
-    :ivar cterasdk.core.syslog.Syslog syslog: Object holding the Portal syslog APIs
-    :ivar cterasdk.core.antivirus.Antivirus antivirus: Object holding the Portal Antivirus APIs
-    :ivar cterasdk.core.buckets.Buckets buckets: Object holding the Portal Storage Node APIs
-    :ivar cterasdk.core.messaging.Messaging messaging: Object holding the Portal Messaging Service Management APIs
-
     """
 
     def __init__(self, host, port=None, https=True):
         """
         :param str host: The fully qualified domain name, hostname or an IPv4 address of the Portal
         :param int,optional port: Set a custom port number (0 - 65535), If not set defaults to 80 for http and 443 for https
         :param bool,optional https: Set to True to require HTTPS, defaults to True
         """
         super().__init__(host, port, https)
         self.portals = portals.Portals(self)
         self.servers = servers.Servers(self)
-        self.cli = cli.CLI(self)
         self.setup = setup.Setup(self)
-        self.ssl = ssl.SSL(self)
         self.startup = startup.Startup(self)
-        self.syslog = syslog.Syslog(self)
-        self.antivirus = antivirus.Antivirus(self)
-        self.buckets = buckets.Buckets(self)
-        self.messaging = messaging.Messaging(self)
 
     @property
     def _omit_fields(self):
-        return super()._omit_fields + ['portals', 'servers', 'setup', 'ssl', 'startup', 'syslog', 'antivirus', 'buckets', 'messaging']
+        return super()._omit_fields + ['portals', 'servers', 'setup', 'startup']
 
     @property
     def context(self):
         return 'admin'
 
     @property
-    def cloud_drive_base_path(self):
+    def file_browser_base_path(self):
         return '/admin/webdav/Users'
 
-    @property
-    def backups_base_path(self):
-        return '/admin/webdav/backupFolders'
-
 
 class ServicesPortal(Portal):
     """
     Main class for Service operations on a Portal
     """
 
     def __init__(self, host, port=None, https=True):
@@ -237,13 +195,9 @@
         super().__init__(host, port, https)
 
     @property
     def context(self):
         return 'ServicesPortal'
 
     @property
-    def cloud_drive_base_path(self):
+    def file_browser_base_path(self):
         return '/ServicesPortal/webdav'
-
-    @property
-    def backups_base_path(self):
-        return '/ServicesPortal/webdav/backups'
```

### Comparing `cterasdk-2.8.32/cterasdk/transcript/apidoc.template` & `cterasdk-2.9.0/cterasdk/transcript/apidoc.template`

 * *Files identical despite different names*

### Comparing `cterasdk-2.8.32/cterasdk/transcript/transcribe.py` & `cterasdk-2.9.0/cterasdk/transcript/transcribe.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,21 +67,21 @@
         if reply:
             response_content_array.append("<br/><p class=\"h6\">Response body:</p>")
             response_content_array.append('<pre>' + cls._prettify(reply) + '</pre>')
         return ''.join(response_content_array)
 
     def _append_content(self, content):
         header, footer = self._get_header_footer()
-        with open(self._filename, 'w', encoding='utf-8') as f:
+        with open(self._filename, 'w') as f:
             f.write(header + content + Transcribe.COMMENT + footer)
 
     def _get_header_footer(self):
         filename = self._filename if os.path.exists(self._filename) else \
             os.path.join(pathlib.Path(__file__).parent.absolute(), 'apidoc.template')
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, 'r') as f:
             content = f.read()
         array = content.split(Transcribe.COMMENT)
         return array[0], array[1]
 
     @staticmethod
     def _prettify(data):
         try:
```

### Comparing `cterasdk-2.8.32/cterasdk.egg-info/PKG-INFO` & `cterasdk-2.9.0/cterasdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,95 @@
 Metadata-Version: 2.1
 Name: cterasdk
-Version: 2.8.32
+Version: 2.9.0
 Summary: CTERA Python SDK
 Home-page: https://pypi.org/project/cterasdk/
 Author: CTERA Networks
 Author-email: support@ctera.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ctera/ctera-python-sdk/issues
 Project-URL: Documentation, https://ctera-python-sdk.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ctera/ctera-python-sdk
+Description: ****************
+        CTERA for Python
+        ****************
+        .. image:: https://travis-ci.com/ctera/ctera-python-sdk.svg?branch=master
+           :target: https://travis-ci.com/ctera/ctera-python-sdk
+        .. image:: https://github.com/ctera/ctera-python-sdk/workflows/CI/badge.svg
+           :target: https://github.com/ctera/ctera-python-sdk/actions?query=workflow%3ACI
+        .. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=stable
+           :target: https://ctera-python-sdk.readthedocs.io/en/stable
+           :alt: [Latest Release Documentation]
+        .. image:: https://snyk.io/test/github/ctera/ctera-python-sdk/badge.svg
+           :target: https://snyk.io/test/github/ctera/ctera-python-sdk
+        .. image:: https://img.shields.io/pypi/v/cterasdk
+           :target: https://pypi.org/pypi/cterasdk
+           :alt: [Latest Release Version]
+        .. image:: https://img.shields.io/pypi/wheel/cterasdk
+           :target: https://pypi.org/pypi/cterasdk
+           :alt: PyPI - Wheel
+        .. image:: https://img.shields.io/pypi/l/cterasdk
+           :target: https://opensource.org/licenses/Apache-2.0
+           :alt: [Latest Release License]
+        .. image:: https://img.shields.io/pypi/pyversions/cterasdk
+            :target: https://pypi.org/pypi/cterasdk
+            :alt: [Latest Release Supported Python Versions]
+        .. image:: https://img.shields.io/pypi/status/cterasdk
+            :target: https://pypi.org/pypi/cterasdk
+            :alt: [Latest Release Development Stage]
+        
+        A Python SDK for integrating with the CTERA Global File System API. Compatible with Python
+        3.5+. 
+        
+        Documentation
+        -------------
+        User documentation is available on `Read the Docs <http://ctera-python-sdk.readthedocs.org/>`_.
+        
+        Installation
+        ------------
+        Installing via `pip <https://pip.pypa.io/>`_:
+        
+        .. code-block:: console
+        
+            $ pip install cterasdk
+        
+        Install from source:
+        
+        .. code-block:: console
+        
+           $ git clone https://github.com/ctera/ctera-python-sdk.git
+           $ cd ctera-python-sdk
+           $ python setup.py install
+        
+        Importing the Library
+        ---------------------
+        After installation, to get started, open a Python console:
+        
+        .. code-block:: pycon
+        
+            >>> from cterasdk import *
+        
+        Building Documentation
+        -------------------------
+        Documentation can be compiled by running ``make html`` from the ``docs``
+        folder. After compilation, open ``docs/build/html/index.html``. 
+        
+        Testing
+        -------
+        We use the `tox <https://tox.readthedocs.org/>`_ package to run tests in Python
+        3. To install, use :code:`pip install tox`. Once installed, run `tox` from the
+        root directory.
+        
+        .. code-block:: console
+        
+           $ tox
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
 Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
-
-****************
-CTERA for Python
-****************
-.. image:: https://travis-ci.com/ctera/ctera-python-sdk.svg?branch=master
-   :target: https://travis-ci.com/ctera/ctera-python-sdk
-.. image:: https://github.com/ctera/ctera-python-sdk/workflows/CI/badge.svg
-   :target: https://github.com/ctera/ctera-python-sdk/actions?query=workflow%3ACI
-.. image:: https://readthedocs.org/projects/ctera-python-sdk/badge/?version=latest
-   :target: https://ctera-python-sdk.readthedocs.io/en/latest
-   :alt: [Latest Release Documentation]
-.. image:: https://snyk.io/test/github/ctera/ctera-python-sdk/badge.svg
-   :target: https://snyk.io/test/github/ctera/ctera-python-sdk
-.. image:: https://img.shields.io/pypi/v/cterasdk
-   :target: https://pypi.org/pypi/cterasdk
-   :alt: [Latest Release Version]
-.. image:: https://img.shields.io/pypi/wheel/cterasdk
-   :target: https://pypi.org/pypi/cterasdk
-   :alt: PyPI - Wheel
-.. image:: https://img.shields.io/pypi/l/cterasdk
-   :target: https://opensource.org/licenses/Apache-2.0
-   :alt: [Latest Release License]
-.. image:: https://img.shields.io/pypi/pyversions/cterasdk
-    :target: https://pypi.org/pypi/cterasdk
-    :alt: [Latest Release Supported Python Versions]
-.. image:: https://img.shields.io/pypi/status/cterasdk
-    :target: https://pypi.org/pypi/cterasdk
-    :alt: [Latest Release Development Stage]
-
-A Python SDK for integrating with the CTERA Global File System API. Compatible with Python
-3.5+.
-
-Documentation
--------------
-User documentation is available on `Read the Docs <http://ctera-python-sdk.readthedocs.org/>`_.
-
-Installation
-------------
-Installing via `pip <https://pip.pypa.io/>`_:
-
-.. code-block:: console
-
-    $ pip install cterasdk
-
-..
-
-If you receive a certificate error, add the following trusted hosts:
-
-.. code-block:: console
-
-    $ pip install cterasdk --trusted-host pypi.org --trusted-host files.pythonhosted.org  # [SSL: CERTIFICATE_VERIFY_FAILED]
-
-..
-
-Installation via proxy:
-
-.. code-block:: console
-
-    $ pip install cterasdk --proxy http://user:password@proxyserver:port  # use proxy
-
-..
-
-Install from source:
-
-.. code-block:: console
-
-   $ git clone https://github.com/ctera/ctera-python-sdk.git
-   $ cd ctera-python-sdk
-   $ python setup.py install
-
-Importing the Library
----------------------
-After installation, to get started, open a Python console:
-
-.. code-block:: python
-
-    >>> from cterasdk import *
-
-Building Documentation
--------------------------
-Documentation can be compiled by running ``make html`` from the ``docs``
-folder. After compilation, open ``docs/build/html/index.html``.
-
-Testing
--------
-We use the `tox <https://tox.readthedocs.org/>`_ package to run tests in Python
-3. To install, use :code:`pip install tox`. Once installed, run `tox` from the
-root directory.
-
-.. code-block:: console
-
-   $ tox
-
```

### Comparing `cterasdk-2.8.32/cterasdk.egg-info/SOURCES.txt` & `cterasdk-2.9.0/cterasdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,44 +33,34 @@
 cterasdk/convert/__init__.py
 cterasdk/convert/exception.py
 cterasdk/convert/format.py
 cterasdk/convert/parse.py
 cterasdk/convert/xml_types.py
 cterasdk/core/__init__.py
 cterasdk/core/activation.py
-cterasdk/core/admins.py
 cterasdk/core/antivirus.py
 cterasdk/core/base_command.py
-cterasdk/core/buckets.py
-cterasdk/core/cli.py
 cterasdk/core/cloudfs.py
 cterasdk/core/connection.py
 cterasdk/core/decorator.py
 cterasdk/core/devices.py
 cterasdk/core/directoryservice.py
 cterasdk/core/enum.py
-cterasdk/core/firmwares.py
 cterasdk/core/login.py
 cterasdk/core/logs.py
-cterasdk/core/messaging.py
 cterasdk/core/plans.py
 cterasdk/core/portals.py
 cterasdk/core/query.py
 cterasdk/core/remote.py
 cterasdk/core/reports.py
 cterasdk/core/servers.py
 cterasdk/core/session.py
-cterasdk/core/settings.py
 cterasdk/core/setup.py
-cterasdk/core/ssl.py
 cterasdk/core/startup.py
-cterasdk/core/storage_classes.py
-cterasdk/core/syslog.py
 cterasdk/core/taskmgr.py
-cterasdk/core/templates.py
 cterasdk/core/types.py
 cterasdk/core/uri.py
 cterasdk/core/users.py
 cterasdk/core/zones.py
 cterasdk/core/files/__init__.py
 cterasdk/core/files/browser.py
 cterasdk/core/files/collaboration.py
@@ -94,41 +84,37 @@
 cterasdk/edge/backup.py
 cterasdk/edge/base_command.py
 cterasdk/edge/cache.py
 cterasdk/edge/cli.py
 cterasdk/edge/config.py
 cterasdk/edge/connection.py
 cterasdk/edge/decorator.py
-cterasdk/edge/dedup.py
 cterasdk/edge/directoryservice.py
 cterasdk/edge/directorytree.py
 cterasdk/edge/drive.py
 cterasdk/edge/enum.py
 cterasdk/edge/firmware.py
 cterasdk/edge/ftp.py
 cterasdk/edge/groups.py
 cterasdk/edge/licenses.py
 cterasdk/edge/login.py
 cterasdk/edge/logs.py
 cterasdk/edge/mail.py
-cterasdk/edge/migration_tool.py
 cterasdk/edge/network.py
 cterasdk/edge/nfs.py
 cterasdk/edge/ntp.py
 cterasdk/edge/power.py
 cterasdk/edge/query.py
 cterasdk/edge/remote.py
 cterasdk/edge/rsync.py
 cterasdk/edge/services.py
 cterasdk/edge/session.py
 cterasdk/edge/shares.py
 cterasdk/edge/shell.py
 cterasdk/edge/smb.py
-cterasdk/edge/snmp.py
-cterasdk/edge/ssh.py
 cterasdk/edge/ssl.py
 cterasdk/edge/support.py
 cterasdk/edge/sync.py
 cterasdk/edge/syslog.py
 cterasdk/edge/taskmgr.py
 cterasdk/edge/telnet.py
 cterasdk/edge/timezone.py
@@ -144,15 +130,14 @@
 cterasdk/edge/files/move.py
 cterasdk/edge/files/open.py
 cterasdk/edge/files/path.py
 cterasdk/edge/files/rm.py
 cterasdk/lib/__init__.py
 cterasdk/lib/cmd.py
 cterasdk/lib/consent.py
-cterasdk/lib/crypto.py
 cterasdk/lib/file_access_base.py
 cterasdk/lib/filesystem.py
 cterasdk/lib/iterator.py
 cterasdk/lib/platform.py
 cterasdk/lib/registry.py
 cterasdk/lib/session_base.py
 cterasdk/lib/task_manager_base.py
```

### Comparing `cterasdk-2.8.32/setup.cfg` & `cterasdk-2.9.0/setup.cfg`

 * *Files identical despite different names*

