# Comparing `tmp/osxphotos-0.60.5.tar.gz` & `tmp/osxphotos-0.60.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.5.tar", last modified: Sat Jun 24 17:51:35 2023, max compression
+gzip compressed data, was "osxphotos-0.60.6.tar", last modified: Sun Jul  2 16:42:00 2023, max compression
```

## Comparing `osxphotos-0.60.5.tar` & `osxphotos-0.60.6.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.337727 osxphotos-0.60.5/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.5/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.5/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-24 17:51:35.337484 osxphotos-0.60.5/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   225895 2023-06-24 17:51:20.000000 osxphotos-0.60.5/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.5/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.275203 osxphotos-0.60.5/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1955 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.5/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-24 17:51:14.000000 osxphotos-0.60.5/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.5/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.5/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.291701 osxphotos-0.60.5/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.5/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3805 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.5/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   107303 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61930 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.5/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.5/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.5/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.5/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.5/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.5/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.292938 osxphotos-0.60.5/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.5/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1471826 2023-06-24 17:51:29.000000 osxphotos-0.60.5/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.5/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.5/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.5/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.5/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    91553 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    84853 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.313659 osxphotos-0.60.5/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.5/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.5/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-24 17:51:20.000000 osxphotos-0.60.5/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.5/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.5/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21821 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/platform.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.5/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.315739 osxphotos-0.60.5/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.5/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.5/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.5/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.5/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.5/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.5/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.5/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.317221 osxphotos-0.60.5/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.5/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.277108 osxphotos-0.60.5/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-24 17:51:35.337768 osxphotos-0.60.5/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.5/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.336849 osxphotos-0.60.5/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.337211 osxphotos-0.60.5/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.5/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.5/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   274105 2023-06-24 17:50:43.000000 osxphotos-0.60.5/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.5/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.5/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.5/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.5/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.5/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.5/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.5/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.5/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.5/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.5/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.5/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_photosalbum_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.5/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.5/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.5/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.5/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.5/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.5/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.5/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.5/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.5/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.5/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.898076 osxphotos-0.60.6/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.6/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.6/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-02 16:42:00.897889 osxphotos-0.60.6/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   225720 2023-07-02 16:41:50.000000 osxphotos-0.60.6/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.6/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.868539 osxphotos-0.60.6/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.6/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-02 16:41:47.000000 osxphotos-0.60.6/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.6/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.6/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.876378 osxphotos-0.60.6/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.6/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.6/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   107303 2023-07-02 15:42:46.000000 osxphotos-0.60.6/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.6/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.6/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.6/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.6/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.6/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.6/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.876870 osxphotos-0.60.6/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.6/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1465082 2023-07-02 16:41:57.000000 osxphotos-0.60.6/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.6/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.6/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.6/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.6/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    91553 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    84853 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.879356 osxphotos-0.60.6/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.6/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.6/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-02 16:41:49.000000 osxphotos-0.60.6/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.6/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.6/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    25682 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.6/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.884201 osxphotos-0.60.6/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.6/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.6/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.6/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.6/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.6/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.6/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.6/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.885216 osxphotos-0.60.6/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.6/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.869423 osxphotos-0.60.6/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-02 16:42:00.898118 osxphotos-0.60.6/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.6/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.897412 osxphotos-0.60.6/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.897677 osxphotos-0.60.6/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.6/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.6/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   274105 2023-06-24 17:50:43.000000 osxphotos-0.60.6/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.6/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.6/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.6/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.6/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.6/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.6/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.6/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.6/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.6/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.6/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.6/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.6/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.6/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.6/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.6/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.6/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.6/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.6/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.6/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.6/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.6/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.5/LICENSE` & `osxphotos-0.60.6/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/PKG-INFO` & `osxphotos-0.60.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.5
+Version: 0.60.6
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.5/README.md` & `osxphotos-0.60.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osxphotos)
 [![Downloads](https://static.pepy.tech/personalized-badge/osxphotos?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/osxphotos)
 [![subreddit](https://img.shields.io/reddit/subreddit-subscribers/osxphotos?style=social)](https://www.reddit.com/r/osxphotos/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-61-orange.svg?style=flat)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-62-orange.svg?style=flat)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS and Linux. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
 
 <p align="center"><img src="docs/screencast/demo.gif?raw=true" width="713" height="430"/></p>
 
 # Table of Contents
@@ -136,23 +136,16 @@
 ]]] -->
 ```
 Usage: osxphotos [OPTIONS] COMMAND [ARGS]...
 
   osxphotos: the multi-tool for your Photos library
 
 Options:
-  -v, --version                   Show the version and exit.
-  --library, --db PHOTOS_LIBRARY_PATH
-                                  Specify path to Photos library. If not
-                                  provided, will attempt to find the library to
-                                  use in the following order: 1. last opened
-                                  library, 2. system library, 3.
-                                  ~/Pictures/Photos Library.photoslibrary
-  --json                          Print output in JSON format.
-  -h, --help                      Show this message and exit.
+  -v, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
 Commands:
   about          Print information about osxphotos including license.
   add-locations  Add missing location data to photos in Photos.app using...
   albums         Print out albums found in the Photos library.
   batch-edit     Batch edit photo metadata such as title, description,...
   diff           Compare two Photos databases and print out differences
@@ -2113,15 +2106,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.5'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.6'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2600,15 +2593,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.5'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.6'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2729,14 +2722,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wernerzj"><img src="https://avatars.githubusercontent.com/u/130370930?v=4?s=75" width="75px;" alt="wernerzj"/><br /><sub><b>wernerzj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Awernerzj" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=rajscode" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/MaxLyt"><img src="https://avatars.githubusercontent.com/u/136200430?v=4?s=75" width="75px;" alt="MaxLyt"/><br /><sub><b>MaxLyt</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3AMaxLyt" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ces3001"><img src="https://avatars.githubusercontent.com/u/23762610?v=4?s=75" width="75px;" alt="ces3001"/><br /><sub><b>ces3001</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aces3001" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/msolo"><img src="https://avatars.githubusercontent.com/u/5078276?v=4?s=75" width="75px;" alt="msolo"/><br /><sub><b>msolo</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Amsolo" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `osxphotos-0.60.5/README.rst` & `osxphotos-0.60.6/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/__init__.py` & `osxphotos-0.60.6/osxphotos/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .albuminfo import AlbumInfo, FolderInfo, ImportInfo, ProjectInfo
 from .debug import is_debug, set_debug
 from .exifinfo import ExifInfo
 from .exiftool import ExifTool
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil, FileUtilNoOp
 from .momentinfo import MomentInfo
-from .personinfo import PersonInfo
+from .personinfo import FaceInfo, PersonInfo
 from .photoexporter import ExportOptions, ExportResults, PhotoExporter
 from .photoinfo import PhotoInfo
 from .photosdb import PhotosDB
 from .photosdb._photosdb_process_comments import CommentInfo, LikeInfo
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate
 from .placeinfo import PlaceInfo
@@ -44,14 +44,15 @@
     "CommentInfo",
     "ExifInfo",
     "ExifTool",
     "ExportDB",
     "ExportDBTemp",
     "ExportOptions",
     "ExportResults",
+    "FaceInfo",
     "FileUtil",
     "FileUtilNoOp",
     "FolderInfo",
     "ImportInfo",
     "LikeInfo",
     "MomentInfo",
     "PersonInfo",
```

### Comparing `osxphotos-0.60.5/osxphotos/_constants.py` & `osxphotos-0.60.6/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.6/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/albuminfo.py` & `osxphotos-0.60.6/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/__init__.py` & `osxphotos-0.60.6/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/about.py` & `osxphotos-0.60.6/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/add_locations.py` & `osxphotos-0.60.6/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/albums.py` & `osxphotos-0.60.6/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.6/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/cli.py` & `osxphotos-0.60.6/osxphotos/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from osxphotos._constants import PROFILE_SORT_KEYS
 from osxphotos._version import __version__
 from osxphotos.platform import is_macos
 
 from .about import about
 from .albums import albums
-from .cli_params import DB_OPTION, DEBUG_OPTIONS, JSON_OPTION, VERSION_OPTION
+from .cli_params import DEBUG_OPTIONS, VERSION_OPTION
 from .common import OSXPHOTOS_HIDDEN
 from .debug_dump import debug_dump
 from .docs import docs_command
 from .dump import dump
 from .exiftool_cli import exiftool
 from .export import export
 from .exportdb import exportdb
@@ -58,16 +58,14 @@
 
 
 CTX_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.group(context_settings=CTX_SETTINGS)
 @VERSION_OPTION
-@DB_OPTION
-@JSON_OPTION
 @DEBUG_OPTIONS
 @click.option(
     "--profile", is_flag=True, hidden=OSXPHOTOS_HIDDEN, help="Enable profiling"
 )
 @click.option(
     "--profile-sort",
     default=None,
@@ -79,20 +77,20 @@
         case_sensitive=True,
     ),
     help="Sort profiler output by SORT_KEY as specified at https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats. "
     f"Can be specified multiple times. Valid options are: {PROFILE_SORT_KEYS}. "
     "Default = 'cumulative'.",
 )
 @click.pass_context
-def cli_main(ctx, db, json_, profile, profile_sort, **kwargs):
+def cli_main(ctx, profile, profile_sort, **kwargs):
     """osxphotos: the multi-tool for your Photos library"""
     # Note: kwargs is used to catch any debug options passed in
     # the debug options are handled in cli/__init__.py
     # before this function is called
-    ctx.obj = CLI_Obj(db=db, json=json_, group=cli_main)
+    ctx.obj = CLI_Obj(group=cli_main)
     if profile:
         click.echo("Profiling...")
         profile_sort = profile_sort or ["cumulative"]
         click.echo(f"Profile sort_stats order: {profile_sort}")
         pr = cProfile.Profile()
         pr.enable()
```

### Comparing `osxphotos-0.60.5/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.6/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/cli_params.py` & `osxphotos-0.60.6/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.6/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/color_themes.py` & `osxphotos-0.60.6/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/common.py` & `osxphotos-0.60.6/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/darkmode.py` & `osxphotos-0.60.6/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.6/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/docs.py` & `osxphotos-0.60.6/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/dump.py` & `osxphotos-0.60.6/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.6/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/export.py` & `osxphotos-0.60.6/osxphotos/cli/export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/exportdb.py` & `osxphotos-0.60.6/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/grep.py` & `osxphotos-0.60.6/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/help.py` & `osxphotos-0.60.6/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/import_cli.py` & `osxphotos-0.60.6/osxphotos/cli/import_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1418,15 +1418,21 @@
     split_folder,
     theme,
     timestamp,
     title,
     verbose_flag,
     walk,
 ):
-    """Import photos and videos into Photos."""
+    """Import photos and videos into Photos. Photos will be imported into the
+    most recently opened Photos library.
+
+    Photos are imported one at a time thus the "Imports" album in Photos will show
+    a new import group for each photo imported. Batch import into a single import
+    group will be added in a future release.
+    """
 
     verbose = verbose_print(verbose=verbose_flag, timestamp=timestamp, theme=theme)
 
     if not files:
         echo("Nothing to import", err=True)
         return
```

### Comparing `osxphotos-0.60.5/osxphotos/cli/info.py` & `osxphotos-0.60.6/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.6/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/keywords.py` & `osxphotos-0.60.6/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/kvstore.py` & `osxphotos-0.60.6/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/labels.py` & `osxphotos-0.60.6/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/list.py` & `osxphotos-0.60.6/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/orphans.py` & `osxphotos-0.60.6/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/param_types.py` & `osxphotos-0.60.6/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/persons.py` & `osxphotos-0.60.6/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.6/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/places.py` & `osxphotos-0.60.6/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.6/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/query.py` & `osxphotos-0.60.6/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/repl.py` & `osxphotos-0.60.6/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/report_writer.py` & `osxphotos-0.60.6/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.6/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/show_command.py` & `osxphotos-0.60.6/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.6/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/sync.py` & `osxphotos-0.60.6/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/sync_results.py` & `osxphotos-0.60.6/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/theme.py` & `osxphotos-0.60.6/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/timewarp.py` & `osxphotos-0.60.6/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/tutorial.py` & `osxphotos-0.60.6/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/uuid.py` & `osxphotos-0.60.6/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/verbose.py` & `osxphotos-0.60.6/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/cli/version.py` & `osxphotos-0.60.6/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/compare_exif.py` & `osxphotos-0.60.6/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/configoptions.py` & `osxphotos-0.60.6/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/crash_reporter.py` & `osxphotos-0.60.6/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/datetime_formatter.py` & `osxphotos-0.60.6/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/datetime_utils.py` & `osxphotos-0.60.6/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/debug.py` & `osxphotos-0.60.6/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/docs/docs.zip` & `osxphotos-0.60.6/osxphotos/docs/docs.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1471826 bytes, number of entries: 99
+Zip file size: 1465082 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jun-24 17:51 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jul-02 16:41 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   324897 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
@@ -17,85 +17,85 @@
 -rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
 -rw-r--r--  3.0 unx   313931 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
 -rw-r--r--  3.0 unx   526465 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
--rw-r--r--  3.0 unx    92670 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/placeinfo.html
+-rw-r--r--  3.0 unx    98734 tx defN 23-Jul-02 16:33 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    61579 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    61830 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jun-24 17:51 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jul-02 16:35 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jun-24 17:51 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jul-02 16:41 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jun-24 17:51 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jul-02 16:41 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jun-24 17:51 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jul-02 16:41 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jun-24 17:51 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jul-02 16:41 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jun-24 17:51 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jul-02 16:41 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   424076 tx defN 23-Jun-24 17:51 docs/cli.html
+-rw-r--r--  3.0 unx   423177 tx defN 23-Jul-02 16:35 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   249787 tx defN 23-Jun-24 17:51 docs/genindex.html
--rw-r--r--  3.0 unx   105318 tx defN 23-Jun-24 17:51 docs/index.html
+-rw-r--r--  3.0 unx   251521 tx defN 23-Jul-02 16:41 docs/genindex.html
+-rw-r--r--  3.0 unx   109432 tx defN 23-Jul-02 16:41 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9617 bx stor 23-Jun-24 17:51 docs/objects.inv
+-rw-r--r--  3.0 unx     9745 bx stor 23-Jul-02 16:41 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jun-24 17:51 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jun-24 17:51 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jun-24 17:51 docs/py-modindex.html
--rw-r--r--  3.0 unx   446001 tx defN 23-Jun-24 17:51 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jul-02 16:35 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jul-02 16:35 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jul-02 16:41 docs/py-modindex.html
+-rw-r--r--  3.0 unx   466218 tx defN 23-Jul-02 16:35 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jun-24 17:51 docs/search.html
--rw-r--r--  3.0 unx   220745 tx defN 23-Jun-24 17:51 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jun-24 17:51 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jun-24 17:51 docs/tutorial.html
-99 files, 6962292 bytes uncompressed, 1453094 bytes compressed:  79.1%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jul-02 16:41 docs/search.html
+-rw-r--r--  3.0 unx   114256 tx defN 23-Jul-02 16:41 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jul-02 16:41 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jul-02 16:41 docs/tutorial.html
+99 files, 6887161 bytes uncompressed, 1446350 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.5 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/placeinfo.html

```diff
@@ -198,14 +198,17 @@
 <span></span><span class="sd">&quot;&quot;&quot; </span>
 <span class="sd">    PlaceInfo class</span>
 <span class="sd">    Provides reverse geolocation info for photos </span>
 <span class="sd">    </span>
 <span class="sd">    See https://developer.apple.com/documentation/corelocation/clplacemark</span>
 <span class="sd">    for additional documentation on reverse geolocation data</span>
 <span class="sd">&quot;&quot;&quot;</span>
+
+<span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">annotations</span>
+
 <span class="kn">from</span> <span class="nn">abc</span> <span class="kn">import</span> <span class="n">ABC</span><span class="p">,</span> <span class="n">abstractmethod</span>
 <span class="kn">from</span> <span class="nn">collections</span> <span class="kn">import</span> <span class="n">namedtuple</span>  <span class="c1"># pylint: disable=syntax-error</span>
 
 <span class="kn">import</span> <span class="nn">yaml</span>
 <span class="kn">from</span> <span class="nn">bpylist2</span> <span class="kn">import</span> <span class="n">archiver</span>
 
 <span class="kn">from</span> <span class="nn">.unicode</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
@@ -524,43 +527,107 @@
 <span class="n">archiver</span><span class="o">.</span><span class="n">update_class_map</span><span class="p">(</span>
     <span class="p">{</span><span class="s2">&quot;PLRevGeoMapItemAdditionalPlaceInfo&quot;</span><span class="p">:</span> <span class="n">PLRevGeoMapItemAdditionalPlaceInfo</span><span class="p">}</span>
 <span class="p">)</span>
 <span class="n">archiver</span><span class="o">.</span><span class="n">update_class_map</span><span class="p">({</span><span class="s2">&quot;PLRevGeoMapItem&quot;</span><span class="p">:</span> <span class="n">PLRevGeoMapItem</span><span class="p">})</span>
 <span class="n">archiver</span><span class="o">.</span><span class="n">update_class_map</span><span class="p">({</span><span class="s2">&quot;PLRevGeoLocationInfo&quot;</span><span class="p">:</span> <span class="n">PLRevGeoLocationInfo</span><span class="p">})</span>
 
 
-<div class="viewcode-block" id="PlaceInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.PlaceInfo">[docs]</a><span class="k">class</span> <span class="nc">PlaceInfo</span><span class="p">(</span><span class="n">ABC</span><span class="p">):</span>
+<span class="c1"># PlaceInfo is really an abstract base class but defining it as such</span>
+<span class="c1"># means it doesn&#39;t get picked up by the doc generation tools</span>
+<span class="c1"># so we define it as a regular class and then subclass it</span>
+<span class="c1"># TODO: right fix is probably have PlaceInfo as the only class that</span>
+<span class="c1"># is used and then have PlaceInfo4 and PlaceInfo5 called by PlaceInfo</span>
+<span class="c1"># as needed to return the properties (and make them private classes)</span>
+
+
+<div class="viewcode-block" id="PlaceInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.PlaceInfo">[docs]</a><span class="k">class</span> <span class="nc">PlaceInfo</span><span class="p">:</span>
+    <span class="sd">&quot;&quot;&quot;Reverse geolocation place info for a photo.&quot;&quot;&quot;</span>
+
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
-    <span class="k">def</span> <span class="nf">address_str</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">address_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns the full postal address as a string if defined, otherwise `None`.&quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
-    <span class="k">def</span> <span class="nf">country_code</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">country_code</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns the country_code of place, for example &quot;GB&quot;.</span>
+<span class="sd">        Returns `None` if PhotoInfo contains no country code.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
-    <span class="k">def</span> <span class="nf">ishome</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">ishome</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns `True` if photo place is user&#39;s home address, otherwise `False`.&quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
-    <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns the name of the local place as str.</span>
+<span class="sd">        This is what Photos displays in the Info window.</span>
+<span class="sd">        **Note** Photos 5 uses a different algorithm to determine the name than earlier versions which means the same Photo may have a different place name in Photos 4 and Photos 5.</span>
+<span class="sd">        `PhotoInfo.name` will return the name Photos would have shown depending on the version of the library being processed.</span>
+<span class="sd">        Returns `None` if photo does not contain a name.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
-    <span class="k">def</span> <span class="nf">names</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">PlaceNames</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns a `PlaceNames` namedtuple with the following fields.</span>
+<span class="sd">        Each field is a list with zero or more values, sorted by area in ascending order.</span>
+<span class="sd">        E.g. `names.area_of_interest` could be [&#39;Gulf Islands National Seashore&#39;, &#39;Santa Rosa Island&#39;], [&quot;Knott&#39;s Berry Farm&quot;], or [] if `area_of_interest` not defined.</span>
+<span class="sd">        The value shown in Photos is the first value in the list. With the exception of `body_of_water` each of these field corresponds to an attribute of</span>
+<span class="sd">        a [CLPlacemark](https://developer.apple.com/documentation/corelocation/clplacemark) object.</span>
+
+
+<span class="sd">        * `country`; the name of the country associated with the placemark.</span>
+<span class="sd">        * `state_province`; administrativeArea, The state or province associated with the placemark.</span>
+<span class="sd">        * `sub_administrative_area`; additional administrative area information for the placemark.</span>
+<span class="sd">        * `city`; locality; the city associated with the placemark.</span>
+<span class="sd">        * `additional_city_info`; subLocality, Additional city-level information for the placemark.</span>
+<span class="sd">        * `ocean`; the name of the ocean associated with the placemark.</span>
+<span class="sd">        * `area_of_interest`; areasOfInterest, The relevant areas of interest associated with the placemark.</span>
+<span class="sd">        * `inland_water`; the name of the inland water body associated with the placemark.</span>
+<span class="sd">        * `region`; the geographic region associated with the placemark.</span>
+<span class="sd">        * `sub_throughfare`; additional street-level information for the placemark.</span>
+<span class="sd">        * `postal_code`; the postal code associated with the placemark.</span>
+<span class="sd">        * `street_address`; throughfare, The street address associated with the placemark.</span>
+<span class="sd">        * `body_of_water`; in Photos 4, any body of water; in Photos 5 contains the union of ocean and inland_water</span>
+
+<span class="sd">        **Note**: In Photos &lt;= 4.0, only the following fields are defined; all others are set to empty list:</span>
+
+<span class="sd">        * `country`</span>
+<span class="sd">        * `state_province`</span>
+<span class="sd">        * `sub_administrative_area`</span>
+<span class="sd">        * `city`</span>
+<span class="sd">        * `additional_city_info`</span>
+<span class="sd">        * `area_of_interest`</span>
+<span class="sd">        * `body_of_water`</span>
+
+<span class="sd">        Note:</span>
+<span class="sd">            The `PlaceNames` namedtuple contains reserved fields not listed below (see implementation for details),</span>
+<span class="sd">            thus it should be referenced only by name (e.g. `names.city`) and not by index.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
     <span class="nd">@property</span>
-    <span class="nd">@abstractmethod</span>
     <span class="k">def</span> <span class="nf">address</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Returns a `PostalAddress` namedtuple with details of the postal address containing the following fields:</span>
+
+<span class="sd">        * `city`</span>
+<span class="sd">        * `country`</span>
+<span class="sd">        * `postal_code`</span>
+<span class="sd">        * `state`</span>
+<span class="sd">        * `street`</span>
+<span class="sd">        * `sub_administrative_area`</span>
+<span class="sd">        * `sub_locality`</span>
+<span class="sd">        * `iso_country_code`</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">pass</span>
+
+    <span class="k">def</span> <span class="nf">asdict</span><span class="p">():</span>
         <span class="k">pass</span></div>
 
 
 <span class="k">class</span> <span class="nc">PlaceInfo4</span><span class="p">(</span><span class="n">PlaceInfo</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;Reverse geolocation place info for a photo (Photos &lt;= 4)&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">place_names</span><span class="p">,</span> <span class="n">country_code</span><span class="p">):</span>
```

##### html2text {}

```diff
@@ -39,14 +39,17 @@
 """
     PlaceInfo class
     Provides reverse geolocation info for photos
 
     See https://developer.apple.com/documentation/corelocation/clplacemark
     for additional documentation on reverse geolocation data
 """
+
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from collections import namedtuple  # pylint: disable=syntax-error
 
 import yaml
 from bpylist2 import archiver
 
 from .unicode import normalize_unicode
@@ -379,43 +382,129 @@
 archiver.update_class_map(
     {"PLRevGeoMapItemAdditionalPlaceInfo": PLRevGeoMapItemAdditionalPlaceInfo}
 )
 archiver.update_class_map({"PLRevGeoMapItem": PLRevGeoMapItem})
 archiver.update_class_map({"PLRevGeoLocationInfo": PLRevGeoLocationInfo})
 
 
-[docs]class PlaceInfo(ABC):
+# PlaceInfo is really an abstract base class but defining it as such
+# means it doesn't get picked up by the doc generation tools
+# so we define it as a regular class and then subclass it
+# TODO: right fix is probably have PlaceInfo as the only class that
+# is used and then have PlaceInfo4 and PlaceInfo5 called by PlaceInfo
+# as needed to return the properties (and make them private classes)
+
+
+[docs]class PlaceInfo:
+    """Reverse geolocation place info for a photo."""
+
     @property
-    @abstractmethod
-    def address_str(self):
+    def address_str(self) -> str | None:
+        """Returns the full postal address as a string if defined, otherwise
+`None`."""
         pass
 
     @property
-    @abstractmethod
-    def country_code(self):
+    def country_code(self) -> str | None:
+        """Returns the country_code of place, for example "GB".
+        Returns `None` if PhotoInfo contains no country code.
+        """
         pass
 
     @property
-    @abstractmethod
-    def ishome(self):
+    def ishome(self) -> bool:
+        """Returns `True` if photo place is user's home address, otherwise
+`False`."""
         pass
 
     @property
-    @abstractmethod
-    def name(self):
+    def name(self) -> str | None:
+        """Returns the name of the local place as str.
+        This is what Photos displays in the Info window.
+        **Note** Photos 5 uses a different algorithm to determine the name than
+earlier versions which means the same Photo may have a different place name in
+Photos 4 and Photos 5.
+        `PhotoInfo.name` will return the name Photos would have shown depending
+on the version of the library being processed.
+        Returns `None` if photo does not contain a name.
+        """
         pass
 
     @property
-    @abstractmethod
-    def names(self):
+    def names(self) -> PlaceNames | None:
+        """Returns a `PlaceNames` namedtuple with the following fields.
+        Each field is a list with zero or more values, sorted by area in
+ascending order.
+        E.g. `names.area_of_interest` could be ['Gulf Islands National
+Seashore', 'Santa Rosa Island'], ["Knott's Berry Farm"], or [] if
+`area_of_interest` not defined.
+        The value shown in Photos is the first value in the list. With the
+exception of `body_of_water` each of these field corresponds to an attribute of
+        a [CLPlacemark](https://developer.apple.com/documentation/corelocation/
+clplacemark) object.
+
+
+        * `country`; the name of the country associated with the placemark.
+        * `state_province`; administrativeArea, The state or province
+associated with the placemark.
+        * `sub_administrative_area`; additional administrative area information
+for the placemark.
+        * `city`; locality; the city associated with the placemark.
+        * `additional_city_info`; subLocality, Additional city-level
+information for the placemark.
+        * `ocean`; the name of the ocean associated with the placemark.
+        * `area_of_interest`; areasOfInterest, The relevant areas of interest
+associated with the placemark.
+        * `inland_water`; the name of the inland water body associated with the
+placemark.
+        * `region`; the geographic region associated with the placemark.
+        * `sub_throughfare`; additional street-level information for the
+placemark.
+        * `postal_code`; the postal code associated with the placemark.
+        * `street_address`; throughfare, The street address associated with the
+placemark.
+        * `body_of_water`; in Photos 4, any body of water; in Photos 5 contains
+the union of ocean and inland_water
+
+        **Note**: In Photos <= 4.0, only the following fields are defined; all
+others are set to empty list:
+
+        * `country`
+        * `state_province`
+        * `sub_administrative_area`
+        * `city`
+        * `additional_city_info`
+        * `area_of_interest`
+        * `body_of_water`
+
+        Note:
+            The `PlaceNames` namedtuple contains reserved fields not listed
+below (see implementation for details),
+            thus it should be referenced only by name (e.g. `names.city`) and
+not by index.
+        """
         pass
 
     @property
-    @abstractmethod
     def address(self):
+        """Returns a `PostalAddress` namedtuple with details of the postal
+address containing the following fields:
+
+        * `city`
+        * `country`
+        * `postal_code`
+        * `state`
+        * `street`
+        * `sub_administrative_area`
+        * `sub_locality`
+        * `iso_country_code`
+        """
+        pass
+
+    def asdict():
         pass
 
 
 
 class PlaceInfo4(PlaceInfo):
     """Reverse geolocation place info for a photo (Photos <= 4)"""
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.5'
+     - The osxphotos version, e.g. '0.60.6'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.5',
+    VERSION: '0.60.6',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -207,26 +207,14 @@
 <p class="rubric">Options</p>
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-v">
 <span id="cmdoption-osxphotos-version"></span><span class="sig-name descname"><span class="pre">-v</span></span><span class="sig-prename descclassname"></span><span class="sig-prename descclassname"><span class="pre">,</span> </span><span class="sig-name descname"><span class="pre">--version</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-v" title="Permalink to this definition">#</a></dt>
 <dd><p>Show the version and exit.</p>
 </dd></dl>
 
-<dl class="std option">
-<dt class="sig sig-object std" id="cmdoption-osxphotos-library">
-<span id="cmdoption-osxphotos-db"></span><span class="sig-name descname"><span class="pre">--library</span></span><span class="sig-prename descclassname"></span><span class="sig-prename descclassname"><span class="pre">,</span> </span><span class="sig-name descname"><span class="pre">--db</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;PHOTOS_LIBRARY_PATH&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-library" title="Permalink to this definition">#</a></dt>
-<dd><p>Specify path to Photos library. If not provided, will attempt to find the library to use in the following order: 1. last opened library, 2. system library, 3. ~/Pictures/Photos Library.photoslibrary</p>
-</dd></dl>
-
-<dl class="std option">
-<dt class="sig sig-object std" id="cmdoption-osxphotos-json">
-<span class="sig-name descname"><span class="pre">--json</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-json" title="Permalink to this definition">#</a></dt>
-<dd><p>Print output in JSON format.</p>
-</dd></dl>
-
 <section id="osxphotos-about">
 <h3>about<a class="headerlink" href="#osxphotos-about" title="Permalink to this heading">#</a></h3>
 <p>Print information about osxphotos including license.</p>
 <div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>osxphotos about <span class="o">[</span>OPTIONS<span class="o">]</span>
 </pre></div>
 </div>
 </section>
@@ -2376,15 +2364,19 @@
 <span id="cmdoption-osxphotos-help-arg-subtopic"></span><span class="sig-name descname"><span class="pre">SUBTOPIC</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-help-arg-SUBTOPIC" title="Permalink to this definition">#</a></dt>
 <dd><p>Optional argument</p>
 </dd></dl>
 
 </section>
 <section id="osxphotos-import">
 <h3>import<a class="headerlink" href="#osxphotos-import" title="Permalink to this heading">#</a></h3>
-<p>Import photos and videos into Photos.</p>
+<p>Import photos and videos into Photos. Photos will be imported into the
+most recently opened Photos library.</p>
+<p>Photos are imported one at a time thus the “Imports” album in Photos will show
+a new import group for each photo imported. Batch import into a single import
+group will be added in a future release.</p>
 <div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>osxphotos import <span class="o">[</span>OPTIONS<span class="o">]</span> <span class="o">[</span>FILES<span class="o">]</span>...
 </pre></div>
 </div>
 <p class="rubric">Options</p>
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-import-a">
 <span id="cmdoption-osxphotos-import-album"></span><span class="sig-name descname"><span class="pre">-a</span></span><span class="sig-prename descclassname"></span><span class="sig-prename descclassname"><span class="pre">,</span> </span><span class="sig-name descname"><span class="pre">--album</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;ALBUM_TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-import-a" title="Permalink to this definition">#</a></dt>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -40,20 +40,14 @@
 ****** OSXPhotos Command Line Interface (CLI)# ******
 ***** osxphotos# *****
 osxphotos: the multi-tool for your Photos library
 osxphotos [OPTIONS] COMMAND [ARGS]...
 Options
   -v, --version#
       Show the version and exit.
-  --library, --db <PHOTOS_LIBRARY_PATH>#
-      Specify path to Photos library. If not provided, will attempt to find the
-      library to use in the following order: 1. last opened library, 2. system
-      library, 3. ~/Pictures/Photos Library.photoslibrary
-  --json#
-      Print output in JSON format.
 **** about# ****
 Print information about osxphotos including license.
 osxphotos about [OPTIONS]
 
 **** add-locations# ****
 Add missing location data to photos in Photos.app using nearest neighbor.
 This command will search for photos that are missing location data and look for
@@ -1340,15 +1334,19 @@
 Arguments
   TOPIC#
       Optional argument
   SUBTOPIC#
       Optional argument
 
 **** import# ****
-Import photos and videos into Photos.
+Import photos and videos into Photos. Photos will be imported into the most
+recently opened Photos library.
+Photos are imported one at a time thus the âImportsâ album in Photos will
+show a new import group for each photo imported. Batch import into a single
+import group will be added in a future release.
 osxphotos import [OPTIONS] [FILES]...
 Options
   -a, --album <ALBUM_TEMPLATE>#
       Import photos into album ALBUM_TEMPLATE. ALBUM_TEMPLATE is an osxphotos
       template string. Photos may be imported into more than one album by
       repeating âalbum. See Template System in help for additional
       information.
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.5 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.6 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -467,16 +467,14 @@
           <li><a href="cli.html#cmdoption-osxphotos-timewarp-D">osxphotos-timewarp command line option</a>
 </li>
         </ul></li>
         <li>
     --db
 
         <ul>
-          <li><a href="cli.html#cmdoption-osxphotos-library">osxphotos command line option</a>
-</li>
           <li><a href="cli.html#cmdoption-osxphotos-albums-library">osxphotos-albums command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-batch-edit-library">osxphotos-batch-edit command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-diff-library">osxphotos-diff command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-dump-library">osxphotos-dump command line option</a>
@@ -1140,16 +1138,14 @@
           <li><a href="cli.html#cmdoption-osxphotos-export-jpeg-quality">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
     --json
 
         <ul>
-          <li><a href="cli.html#cmdoption-osxphotos-json">osxphotos command line option</a>
-</li>
           <li><a href="cli.html#cmdoption-osxphotos-albums-json">osxphotos-albums command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-dump-json">osxphotos-dump command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-info-json">osxphotos-info command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-keywords-json">osxphotos-keywords command line option</a>
@@ -1229,16 +1225,14 @@
           <li><a href="cli.html#cmdoption-osxphotos-exportdb-last-run">osxphotos-exportdb command line option</a>
 </li>
         </ul></li>
         <li>
     --library
 
         <ul>
-          <li><a href="cli.html#cmdoption-osxphotos-library">osxphotos command line option</a>
-</li>
           <li><a href="cli.html#cmdoption-osxphotos-albums-library">osxphotos-albums command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-batch-edit-library">osxphotos-batch-edit command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-diff-library">osxphotos-diff command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-dump-library">osxphotos-dump command line option</a>
@@ -3030,14 +3024,18 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.added_after">added_after (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.added_before">added_before (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.added_in_last">added_in_last (osxphotos.QueryOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.PlaceInfo.address">address (osxphotos.PlaceInfo property)</a>
+</li>
+        <li><a href="reference.html#osxphotos.PlaceInfo.address_str">address_str (osxphotos.PlaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.ExifTool.addvalues">addvalues() (osxphotos.ExifTool method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.adjustments">adjustments (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.album">album (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.FolderInfo.album_info">album_info (osxphotos.FolderInfo property)</a>
@@ -3056,18 +3054,18 @@
 
         <ul>
           <li><a href="reference.html#osxphotos.PhotosDB.albums">(osxphotos.PhotosDB property)</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.PhotosDB.albums_as_dict">albums_as_dict (osxphotos.PhotosDB property)</a>
 </li>
-        <li><a href="reference.html#osxphotos.PhotosDB.albums_shared">albums_shared (osxphotos.PhotosDB property)</a>
-</li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.PhotosDB.albums_shared">albums_shared (osxphotos.PhotosDB property)</a>
+</li>
         <li><a href="reference.html#osxphotos.PhotosDB.albums_shared_as_dict">albums_shared_as_dict (osxphotos.PhotosDB property)</a>
 </li>
         <li><a href="reference.html#osxphotos.AlbumSortOrder">AlbumSortOrder (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.SearchInfo.all">all (osxphotos.SearchInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportResults.all_files">all_files() (osxphotos.ExportResults method)</a>
@@ -3080,14 +3078,16 @@
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.AlbumInfo.asdict">asdict() (osxphotos.AlbumInfo method)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.ExifTool.asdict">(osxphotos.ExifTool method)</a>
 </li>
+          <li><a href="reference.html#osxphotos.FaceInfo.asdict">(osxphotos.FaceInfo method)</a>
+</li>
           <li><a href="reference.html#osxphotos.FolderInfo.asdict">(osxphotos.FolderInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.ImportInfo.asdict">(osxphotos.ImportInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.MomentInfo.asdict">(osxphotos.MomentInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.PersonInfo.asdict">(osxphotos.PersonInfo method)</a>
@@ -3143,14 +3143,16 @@
 
 <section id="C" class="genindex-section">
   <h2>C</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.SearchInfo.camera">camera (osxphotos.SearchInfo property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.center">center (osxphotos.FaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.SearchInfo.city">city (osxphotos.SearchInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportDB.close">close() (osxphotos.ExportDB method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.cloud_guid">cloud_guid (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.cloud_metadata">cloud_metadata (osxphotos.PhotoInfo property)</a>
@@ -3171,14 +3173,16 @@
 </li>
         <li><a href="reference.html#osxphotos.FileUtilNoOp.convert_to_jpeg">convert_to_jpeg() (osxphotos.FileUtilNoOp class method)</a>
 </li>
         <li><a href="reference.html#osxphotos.FileUtilNoOp.copy">copy() (osxphotos.FileUtilNoOp class method)</a>
 </li>
         <li><a href="reference.html#osxphotos.SearchInfo.country">country (osxphotos.SearchInfo property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.PlaceInfo.country_code">country_code (osxphotos.PlaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.ExportDB.create_file_record">create_file_record() (osxphotos.ExportDB method)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportDB.create_or_get_file_record">create_or_get_file_record() (osxphotos.ExportDB method)</a>
 </li>
     </ul></td>
   </tr></table>
 </section>
@@ -3341,16 +3345,20 @@
     <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.PersonInfo.face_info">face_info (osxphotos.PersonInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.PhotoInfo.face_info">(osxphotos.PhotoInfo property)</a>
 </li>
         </ul></li>
+        <li><a href="reference.html#osxphotos.FaceInfo.face_rect">face_rect() (osxphotos.FaceInfo method)</a>
+</li>
         <li><a href="reference.html#osxphotos.ExportOptions.face_regions">face_regions (osxphotos.ExportOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo">FaceInfo (class in osxphotos)</a>
+</li>
         <li><a href="reference.html#osxphotos.PersonInfo.favorite">favorite (osxphotos.PersonInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.PhotoInfo.favorite">(osxphotos.PhotoInfo property)</a>
 </li>
           <li><a href="reference.html#osxphotos.QueryOptions.favorite">(osxphotos.QueryOptions attribute)</a>
 </li>
@@ -3368,18 +3376,18 @@
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-import-arg-FILES">osxphotos-import command line option</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.FileUtil">FileUtil (class in osxphotos)</a>
 </li>
-        <li><a href="reference.html#osxphotos.ExportOptions.fileutil">fileutil (osxphotos.ExportOptions attribute)</a>
-</li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.ExportOptions.fileutil">fileutil (osxphotos.ExportOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.FileUtilNoOp">FileUtilNoOp (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate.filter_predicate">filter_predicate() (osxphotos.PhotoTemplate method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.fingerprint">fingerprint (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.folder">folder (osxphotos.QueryOptions attribute)</a>
@@ -3530,26 +3538,28 @@
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.incloud">incloud (osxphotos.PhotoInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.QueryOptions.incloud">(osxphotos.QueryOptions attribute)</a>
 </li>
         </ul></li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExportOptions.increment">increment (osxphotos.ExportOptions attribute)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.PhotoInfo.intrash">intrash (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.is_debug">is_debug() (in module osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.is_reference">is_reference (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.iscloudasset">iscloudasset (osxphotos.PhotoInfo property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.PlaceInfo.ishome">ishome (osxphotos.PlaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.PhotoInfo.ismissing">ismissing (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.ismovie">ismovie (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.isphoto">isphoto (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.israw">israw (osxphotos.PhotoInfo property)</a>
@@ -3564,19 +3574,19 @@
   <h2>J</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExportOptions.jpeg_ext">jpeg_ext (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.jpeg_quality">jpeg_quality (osxphotos.ExportOptions attribute)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExifTool.json">json() (osxphotos.ExifTool method)</a>
 
         <ul>
+          <li><a href="reference.html#osxphotos.FaceInfo.json">(osxphotos.FaceInfo method)</a>
+</li>
           <li><a href="reference.html#osxphotos.PersonInfo.json">(osxphotos.PersonInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.PhotoInfo.json">(osxphotos.PhotoInfo method)</a>
 </li>
         </ul></li>
     </ul></td>
   </tr></table>
@@ -3674,18 +3684,18 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.min_size">min_size (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.missing">missing (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.missing_bursts">missing_bursts (osxphotos.QueryOptions attribute)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.MomentInfo.modification_date">modification_date (osxphotos.MomentInfo property)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     module
 
         <ul>
           <li><a href="reference.html#module-osxphotos">osxphotos</a>
 </li>
         </ul></li>
@@ -3693,23 +3703,33 @@
 </li>
         <li><a href="reference.html#osxphotos.MomentInfo">MomentInfo (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.SearchInfo.month">month (osxphotos.SearchInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.movies">movies (osxphotos.QueryOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.mpri_reg_rect">mpri_reg_rect (osxphotos.FaceInfo property)</a>
+</li>
+        <li><a href="reference.html#osxphotos.FaceInfo.mwg_rs_area">mwg_rs_area (osxphotos.FaceInfo property)</a>
+</li>
     </ul></td>
   </tr></table>
 </section>
 
 <section id="N" class="genindex-section">
   <h2>N</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
-        <li><a href="reference.html#osxphotos.QueryOptions.name">name (osxphotos.QueryOptions attribute)</a>
+        <li><a href="reference.html#osxphotos.PlaceInfo.name">name (osxphotos.PlaceInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.QueryOptions.name">(osxphotos.QueryOptions attribute)</a>
+</li>
+        </ul></li>
+        <li><a href="reference.html#osxphotos.PlaceInfo.names">names (osxphotos.PlaceInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.SearchInfo.neighborhoods">neighborhoods (osxphotos.SearchInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.no_comment">no_comment (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.no_description">no_description (osxphotos.QueryOptions attribute)</a>
 </li>
@@ -3727,18 +3747,18 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_cloudasset">not_cloudasset (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_edited">not_edited (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_favorite">not_favorite (osxphotos.QueryOptions attribute)</a>
 </li>
-        <li><a href="reference.html#osxphotos.QueryOptions.not_hdr">not_hdr (osxphotos.QueryOptions attribute)</a>
-</li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.QueryOptions.not_hdr">not_hdr (osxphotos.QueryOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_hidden">not_hidden (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_in_album">not_in_album (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_incloud">not_incloud (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_live">not_live (osxphotos.QueryOptions attribute)</a>
@@ -3792,20 +3812,14 @@
           <li><a href="reference.html#module-osxphotos">module</a>
 </li>
         </ul></li>
         <li>
     osxphotos command line option
 
         <ul>
-          <li><a href="cli.html#cmdoption-osxphotos-library">--db</a>
-</li>
-          <li><a href="cli.html#cmdoption-osxphotos-json">--json</a>
-</li>
-          <li><a href="cli.html#cmdoption-osxphotos-library">--library</a>
-</li>
           <li><a href="cli.html#cmdoption-osxphotos-v">--version</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-v">-v</a>
 </li>
         </ul></li>
         <li>
     osxphotos-add-locations command line option
@@ -4625,29 +4639,29 @@
           <li><a href="cli.html#cmdoption-osxphotos-import-V">-V</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-import-w">-w</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-import-arg-FILES">FILES</a>
 </li>
         </ul></li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     osxphotos-info command line option
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-info-library">--db</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-info-json">--json</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-info-library">--library</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY">PHOTOS_LIBRARY</a>
 </li>
         </ul></li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     osxphotos-inspect command line option
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-inspect-library">--db</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-inspect-t">--detect-text</a>
@@ -5559,17 +5573,19 @@
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.path_live_photo">path_live_photo (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.path_raw">path_raw (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.person">person (osxphotos.QueryOptions attribute)</a>
 </li>
-        <li><a href="reference.html#osxphotos.PhotoInfo.person_info">person_info (osxphotos.PhotoInfo property)</a>
+        <li><a href="reference.html#osxphotos.FaceInfo.person_info">person_info (osxphotos.FaceInfo property)</a>
 
         <ul>
+          <li><a href="reference.html#osxphotos.PhotoInfo.person_info">(osxphotos.PhotoInfo property)</a>
+</li>
           <li><a href="reference.html#osxphotos.PhotosDB.person_info">(osxphotos.PhotosDB property)</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.PersonInfo">PersonInfo (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.persons">persons (osxphotos.ExportOptions attribute)</a>
 
@@ -5577,14 +5593,16 @@
           <li><a href="reference.html#osxphotos.PhotoInfo.persons">(osxphotos.PhotoInfo property)</a>
 </li>
           <li><a href="reference.html#osxphotos.PhotosDB.persons">(osxphotos.PhotosDB property)</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.PhotosDB.persons_as_dict">persons_as_dict (osxphotos.PhotosDB property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.photo">photo (osxphotos.FaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.AlbumInfo.photo_index">photo_index() (osxphotos.AlbumInfo method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoExporter">PhotoExporter (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo">PhotoInfo (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.AlbumInfo.photos">photos (osxphotos.AlbumInfo property)</a>
@@ -5595,18 +5613,18 @@
           <li><a href="reference.html#osxphotos.MomentInfo.photos">(osxphotos.MomentInfo property)</a>
 </li>
           <li><a href="reference.html#osxphotos.PersonInfo.photos">(osxphotos.PersonInfo property)</a>
 </li>
           <li><a href="reference.html#osxphotos.QueryOptions.photos">(osxphotos.QueryOptions attribute)</a>
 </li>
         </ul></li>
-        <li><a href="reference.html#osxphotos.PhotosDB.photos">photos() (osxphotos.PhotosDB method)</a>
-</li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.PhotosDB.photos">photos() (osxphotos.PhotosDB method)</a>
+</li>
         <li><a href="reference.html#osxphotos.PhotosDB.photos_by_uuid">photos_by_uuid() (osxphotos.PhotosDB method)</a>
 </li>
         <li>
     PHOTOS_LIBRARY
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY">osxphotos-albums command line option</a>
@@ -5636,14 +5654,16 @@
 </li>
         <li><a href="reference.html#osxphotos.PhotosDB">PhotosDB (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate">PhotoTemplate (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExifTool.pid">pid (osxphotos.ExifTool property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.pitch">pitch (osxphotos.FaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.MomentInfo.pk">pk (osxphotos.MomentInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.place">place (osxphotos.PhotoInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.QueryOptions.place">(osxphotos.QueryOptions attribute)</a>
 </li>
@@ -5707,26 +5727,30 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.regex">regex (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.FileUtilNoOp.rename">rename() (osxphotos.FileUtilNoOp class method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate.render">render() (osxphotos.PhotoTemplate method)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExportOptions.render_options">render_options (osxphotos.ExportOptions attribute)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.PhotoInfo.render_template">render_template() (osxphotos.PhotoInfo method)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.replace_keywords">replace_keywords (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.rich">rich (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.FileUtilNoOp.rmdir">rmdir() (osxphotos.FileUtilNoOp class method)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.roll">roll (osxphotos.FaceInfo property)</a>
+</li>
+        <li><a href="reference.html#osxphotos.FaceInfo.roll_pitch_yaw">roll_pitch_yaw() (osxphotos.FaceInfo method)</a>
+</li>
         <li><a href="reference.html#osxphotos.ExifTool.run_commands">run_commands() (osxphotos.ExifTool method)</a>
 </li>
     </ul></td>
   </tr></table>
 </section>
 
 <section id="S" class="genindex-section">
@@ -5783,14 +5807,16 @@
         </ul></li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExportOptions.sidecar">sidecar (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.sidecar_drop_ext">sidecar_drop_ext (osxphotos.ExportOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.FaceInfo.size_pixels">size_pixels (osxphotos.FaceInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.PhotoInfo.slow_mo">slow_mo (osxphotos.PhotoInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.QueryOptions.slow_mo">(osxphotos.QueryOptions attribute)</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.AlbumInfo.sort_order">sort_order (osxphotos.AlbumInfo property)</a>
@@ -5979,14 +6005,18 @@
   </tr></table>
 </section>
 
 <section id="Y" class="genindex-section">
   <h2>Y</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.FaceInfo.yaw">yaw (osxphotos.FaceInfo property)</a>
+</li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.QueryOptions.year">year (osxphotos.QueryOptions attribute)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.SearchInfo.year">(osxphotos.SearchInfo property)</a>
 </li>
         </ul></li>
     </ul></td>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -41,940 +41,936 @@
 | S | T | U | V | W | Y
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
-          o osxphotos-export_command
-            line_option
-    * --add-skipped-to-album
           o osxphotos-export_command        * --not-hdr
             line_option                           o osxphotos-add-locations
-    * --add-to-album                                command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-timewarp_command            o osxphotos-query_command
+    * --add-skipped-to-album                        command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --added-after                               o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --not-hidden
-          o osxphotos-query_command               o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-query_command
-            option                                  line_option
-    * --added-before                              o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --not-in-album
-          o osxphotos-query_command               o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-query_command
-            option                                  line_option
-    * --added-in-last                             o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --not-incloud
-          o osxphotos-query_command               o osxphotos-add-locations
+    * --add-to-album                              o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-timewarp_command              option
+            line_option                           o osxphotos-sync_command_line
+    * --added-after                                 option
+          o osxphotos-add-locations         * --not-hidden
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --added-before                                option
+          o osxphotos-add-locations         * --not-in-album
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --added-in-last                               option
+          o osxphotos-add-locations         * --not-incloud
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --album                                       option
+          o osxphotos-add-locations         * --not-live
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-repl_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
+            option                          * --not-missing
+    * --album-keyword                             o osxphotos-add-locations
+          o osxphotos-exiftool_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+    * --alt-copy                                    line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --append                                    o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
+            line_option                     * --not-panorama
+          o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-query_command
-            option                                  line_option
-    * --album                                     o osxphotos-repl_command_line
+          o osxphotos-exportdb_command            o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-import_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --burst                                     o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --not-live
-          o osxphotos-import_command              o osxphotos-add-locations
+            command_line_option             * --not-portrait
+          o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --album-keyword                             o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --not-missing
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --alt-copy                                  o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --append                                      line_option
-          o osxphotos-exiftool_command            o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-exportdb_command      * --not-panorama
-            line_option                           o osxphotos-add-locations
-          o osxphotos-import_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --burst                                       line_option
-          o osxphotos-add-locations               o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-query_command         * --not-portrait
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --check-signatures                            line_option
-          o osxphotos-exportdb_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --check-templates                           o osxphotos-sync_command_line
-          o osxphotos-import_command                option
+    * --check-signatures                          o osxphotos-sync_command_line
+          o osxphotos-exportdb_command              option
             line_option                     * --not-reference
-    * --cleanup                                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
+    * --check-templates                           o osxphotos-add-locations
+          o osxphotos-import_command                command_line_option
             line_option                           o osxphotos-export_command
-    * --clear-location                              line_option
-          o osxphotos-import_command              o osxphotos-query_command
+    * --cleanup                                     line_option
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --clear-metadata                            o osxphotos-repl_command_line
+    * --clear-location                            o osxphotos-repl_command_line
           o osxphotos-import_command                option
             line_option                           o osxphotos-sync_command_line
-    * --clone                                       option
-          o osxphotos-theme_command         * --not-saved-to-library
+    * --clear-metadata                              option
+          o osxphotos-import_command        * --not-saved-to-library
             line_option                           o osxphotos-add-locations
-    * --cloudasset                                  command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-sync_command_line     * --not-screenshot
-            option                                o osxphotos-add-locations
-    * --compare-exif                                command_line_option
-          o osxphotos-timewarp_command            o osxphotos-export_command
+    * --clone                                       command_line_option
+          o osxphotos-theme_command               o osxphotos-export_command
             line_option                             line_option
-    * --config                                    o osxphotos-query_command
-          o osxphotos-theme_command                 line_option
+    * --cloudasset                                o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --not-screenshot
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --compare-exif                              o osxphotos-query_command
+          o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-repl_command_line
-    * --config-only                                 option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+    * --config                                      option
+          o osxphotos-theme_command               o osxphotos-sync_command_line
             line_option                             option
-    * --convert-to-jpeg                     * --not-selfie
+    * --config-only                         * --not-selfie
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-    * --count                                     o osxphotos-export_command
-          o osxphotos-query_command                 line_option
+    * --convert-to-jpeg                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-    * --current-name                                line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+    * --count                                       line_option
+          o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
-    * --date                                      o osxphotos-sync_command_line
-          o osxphotos-timewarp_command              option
+    * --current-name                              o osxphotos-sync_command_line
+          o osxphotos-export_command                option
             line_option                     * --not-shared
-    * --date-added                                o osxphotos-add-locations
+    * --date                                      o osxphotos-add-locations
           o osxphotos-timewarp_command              command_line_option
             line_option                           o osxphotos-export_command
-    * --date-added-from-photo                       line_option
+    * --date-added                                  line_option
           o osxphotos-timewarp_command            o osxphotos-query_command
             line_option                             line_option
-    * --date-delta                                o osxphotos-repl_command_line
+    * --date-added-from-photo                     o osxphotos-repl_command_line
           o osxphotos-timewarp_command              option
             line_option                     * --not-slow-mo
-    * --db                                        o osxphotos-add-locations
-          o osxphotos_command_line                  command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-albums_command                line_option
+    * --date-delta                                o osxphotos-add-locations
+          o osxphotos-timewarp_command              command_line_option
+            line_option                           o osxphotos-export_command
+    * --db                                          line_option
+          o osxphotos-albums_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-batch-edit                  o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-diff_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-dump_command_line     * --not-syndicated
+            option                                o osxphotos-add-locations
+          o osxphotos-exiftool_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option                   o osxphotos-repl_command_line
-          o osxphotos-diff_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-dump_command_line             option
-            option                          * --not-syndicated
-          o osxphotos-exiftool_command            o osxphotos-add-locations
+          o osxphotos-info_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-inspect_command               option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-keywords_command              option
+            line_option                     * --not-time-lapse
+          o osxphotos-labels_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-orphans_command             o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-info_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-inspect_command             o osxphotos-repl_command_line
+          o osxphotos-persons_command             o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-places_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-keywords_command            o osxphotos-sync_command_line
+          o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-labels_command        * --not-time-lapse
-            line_option                           o osxphotos-add-locations
-          o osxphotos-orphans_command               command_line_option
+          o osxphotos-repl_command_line     * --only-movies
+            option                                o osxphotos-add-locations
+          o osxphotos-show_command_line             command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-snap_command_line             line_option
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --db-config                                   option
+          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+            line_option                             option
+    * --default                             * --only-new
+          o osxphotos-theme_command               o osxphotos-export_command
+            line_option                             line_option
+    * --delete                              * --only-photos
+          o osxphotos-theme_command               o osxphotos-add-locations
+            line_option                             command_line_option
+    * --delete-file                               o osxphotos-export_command
+          o osxphotos-exportdb_command              line_option
+            line_option                           o osxphotos-query_command
+    * --delete-uuid                                 line_option
+          o osxphotos-exportdb_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --deleted                                   o osxphotos-sync_command_line
+          o osxphotos-dump_command_line             option
+            option                          * --original-suffix
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command         * --overwrite
             line_option                           o osxphotos-export_command
-          o osxphotos-persons_command               line_option
+          o osxphotos-repl_command_line             line_option
+            option                          * --panorama
+    * --deleted-only                              o osxphotos-add-locations
+          o osxphotos-dump_command_line             command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-places_command                line_option
+          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
-            option                          * --only-movies
-          o osxphotos-show_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-snap_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                o osxphotos-sync_command_line
+    * --description                                 option
+          o osxphotos-add-locations         * --parse-date
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --person
+          o osxphotos-import_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
-    * --db-config                                 o osxphotos-repl_command_line
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --description-template                      o osxphotos-sync_command_line
           o osxphotos-exiftool_command              option
-            line_option                           o osxphotos-sync_command_line
-    * --default                                     option
-          o osxphotos-theme_command         * --only-new
+            line_option                     * --person-keyword
+          o osxphotos-export_command              o osxphotos-exiftool_command
+            line_option                             line_option
+    * --detect-text                               o osxphotos-export_command
+          o osxphotos-inspect_command               line_option
+            line_option                     * --place
+    * --directory                                 o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-    * --delete                                      line_option
-          o osxphotos-theme_command         * --only-photos
+    * --download-missing                            line_option
+          o osxphotos-export_command              o osxphotos-query_command
+            line_option                             line_option
+    * --dry-run                                   o osxphotos-repl_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-batch-edit                    option
+            command_line_option             * --plain
+          o osxphotos-exiftool_command            o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-export_command        * --portrait
             line_option                           o osxphotos-add-locations
-    * --delete-file                                 command_line_option
-          o osxphotos-exportdb_command            o osxphotos-export_command
+          o osxphotos-exportdb_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-query_command
+    * --dup-check                                   line_option
+          o osxphotos-import_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --duplicate                                 o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --post-command
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --delete-uuid                               o osxphotos-query_command
-          o osxphotos-exportdb_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --deleted                                     option
-          o osxphotos-dump_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-export_command        * --original-suffix
+          o osxphotos-query_command         * --post-function
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --overwrite
-          o osxphotos-repl_command_line           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --preview
+    * --edit                                      o osxphotos-export_command
+          o osxphotos-theme_command                 line_option
+            line_option                           o osxphotos-theme_command
+    * --edited                                      line_option
+          o osxphotos-add-locations         * --preview-if-missing
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                     * --preview-suffix
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --print
+            option                                o osxphotos-dump_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-export_command
+    * --edited-suffix                               line_option
+          o osxphotos-export_command              o osxphotos-query_command
+            line_option                             line_option
+    * --emacs                               * --pull-exif
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --deleted-only                        * --panorama
-          o osxphotos-dump_command_line           o osxphotos-add-locations
-            option                                  command_line_option
+    * --errors                              * --push-exif
+          o osxphotos-exportdb_command            o osxphotos-timewarp_command
+            line_option                             line_option
+    * --exif                                * --query-eval
+          o osxphotos-add-locations               o osxphotos-add-locations
+            command_line_option                     command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --description                               o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --parse-date
-          o osxphotos-batch-edit                  o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-import_command        * --person
-            line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --description-template                        option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-export_command        * --person-keyword
-            line_option                           o osxphotos-exiftool_command
-    * --detect-text                                 line_option
-          o osxphotos-inspect_command             o osxphotos-export_command
-            line_option                             line_option
-    * --directory                           * --place
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --exiftool                            * --query-function
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-    * --download-missing                          o osxphotos-export_command
-          o osxphotos-export_command                line_option
+          o osxphotos-import_command              o osxphotos-export_command
+            line_option                             line_option
+    * --exiftool-merge-keywords                   o osxphotos-query_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+    * --exiftool-merge-persons                      option
+          o osxphotos-exiftool_command      * --quiet
             line_option                           o osxphotos-query_command
-    * --dry-run                                     line_option
-          o osxphotos-add-locations               o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-batch-edit                  o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-exiftool_command      * --plain
-            line_option                           o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option                     * --portrait
-          o osxphotos-exportdb_command            o osxphotos-add-locations
+            line_option                     * --ramdb
+    * --exiftool-option                           o osxphotos-export_command
+          o osxphotos-exiftool_command              line_option
+            line_option                     * --raw-output
+          o osxphotos-export_command              o osxphotos-diff_command_line
+            line_option                             option
+    * --exiftool-path                       * --regex
+          o osxphotos-exiftool_command            o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-sync_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --dup-check                                 o osxphotos-query_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --duplicate                                   option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --post-command
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --post-function
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-import_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --export                                    o osxphotos-sync_command_line
+          o osxphotos-orphans_command               option
+            line_option                     * --relative-to
           o osxphotos-sync_command_line           o osxphotos-import_command
             option                                  line_option
-    * --edit                                * --preview
-          o osxphotos-theme_command               o osxphotos-export_command
+    * --export-as-hardlink                  * --replace-keywords
+          o osxphotos-export_command              o osxphotos-batch-edit
+            line_option                             command_line_option
+    * --export-by-date                            o osxphotos-exiftool_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-export_command
+    * --export-dir                                  line_option
+          o osxphotos-exportdb_command      * --report
+            line_option                           o osxphotos-exiftool_command
+    * --exportdb                                    line_option
+          o osxphotos-exiftool_command            o osxphotos-export_command
             line_option                             line_option
-    * --edited                                    o osxphotos-theme_command
+          o osxphotos-export_command              o osxphotos-exportdb_command
+            line_option                             line_option
+    * --external-edit                             o osxphotos-import_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --resume
+          o osxphotos-query_command               o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --retry
+            option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --run
+    * --favorite                                  o osxphotos-version_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * --preview-if-missing
+            command_line_option             * --save-config
+          o osxphotos-export_command              o osxphotos-exiftool_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-exportdb_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --saved-to-library
+            option                                o osxphotos-add-locations
+    * --favorite-rating                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --preview-suffix
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --print
-          o osxphotos-sync_command_line           o osxphotos-dump_command_line
-            option                                  option
-    * --edited-suffix                             o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --emacs                                       line_option
-          o osxphotos-repl_command_line     * --pull-exif
-            option                                o osxphotos-timewarp_command
-    * --errors                                      line_option
-          o osxphotos-exportdb_command      * --push-exif
-            line_option                           o osxphotos-timewarp_command
-    * --exif                                        line_option
-          o osxphotos-add-locations         * --query-eval
+    * --field                                     o osxphotos-query_command
+          o osxphotos-dump_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+    * --filename                                    option
+          o osxphotos-export_command        * --screenshot
+            line_option                           o osxphotos-add-locations
+          o osxphotos-uuid_command_line             command_line_option
+            option                                o osxphotos-export_command
+    * --finder-tag-keywords                         line_option
+          o osxphotos-export_command              o osxphotos-query_command
+            line_option                             line_option
+    * --finder-tag-template                       o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+    * --folder                                      option
+          o osxphotos-add-locations         * --selected
             command_line_option                   o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-query_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-repl_command_line
           o osxphotos-sync_command_line             option
             option                                o osxphotos-sync_command_line
-    * --exiftool                                    option
-          o osxphotos-export_command        * --query-function
+    * --force                                       option
+          o osxphotos-timewarp_command      * --selfie
             line_option                           o osxphotos-add-locations
-          o osxphotos-import_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --exiftool-merge-keywords                     line_option
-          o osxphotos-exiftool_command            o osxphotos-query_command
+    * --force-update                                command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-    * --exiftool-merge-persons                    o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --quiet
+    * --from-date                                 o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --set
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-sync_command_line     * --shared
+            option                                o osxphotos-add-locations
+    * --from-time                                   command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --exiftool-option                     * --ramdb
-          o osxphotos-exiftool_command            o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-export_command        * --raw-output
-            line_option                           o osxphotos-diff_command_line
-    * --exiftool-path                               option
-          o osxphotos-exiftool_command      * --regex
-            line_option                           o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --export                                      option
-          o osxphotos-orphans_command             o osxphotos-sync_command_line
+          o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-sync_command_line     * --relative-to
-            option                                o osxphotos-import_command
-    * --export-as-hardlink                          line_option
-          o osxphotos-export_command        * --replace-keywords
-            line_option                           o osxphotos-batch-edit
-    * --export-by-date                              command_line_option
-          o osxphotos-export_command              o osxphotos-exiftool_command
+          o osxphotos-repl_command_line     * --sidecar
+            option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --sidecar-drop-ext
+    * --function                                  o osxphotos-export_command
+          o osxphotos-timewarp_command              line_option
+            line_option                     * --skip-bursts
+    * --glob                                      o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                     * --skip-edited
+    * --has-comment                               o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --skip-live
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --export-dir                                o osxphotos-export_command
-          o osxphotos-exportdb_command              line_option
-            line_option                     * --report
-    * --exportdb                                  o osxphotos-exiftool_command
-          o osxphotos-exiftool_command              line_option
+          o osxphotos-query_command         * --skip-original-if-edited
             line_option                           o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-exportdb_command
-    * --external-edit                               line_option
-          o osxphotos-add-locations               o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-query_command         * --resume
-            line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
-            option                          * --retry
+            option                          * --skip-raw
           o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-    * --favorite                            * --run
-          o osxphotos-add-locations               o osxphotos-version_command
+    * --has-likes                           * --skip-uuid
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command        * --save-config
-            line_option                           o osxphotos-exiftool_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-export_command        * --skip-uuid-from-file
             line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-exportdb_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --saved-to-library
-    * --favorite-rating                           o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --field                                       line_option
-          o osxphotos-dump_command_line           o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --slow-mo
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
-            line_option                             option
-    * --filename                                  o osxphotos-sync_command_line
+    * --has-raw                                   o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
           o osxphotos-export_command                option
-            line_option                     * --screenshot
-          o osxphotos-uuid_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --finder-tag-keywords                       o osxphotos-export_command
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --split-folder
+          o osxphotos-repl_command_line           o osxphotos-import_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --sql
+            option                                o osxphotos-exportdb_command
+    * --hdr                                         line_option
+          o osxphotos-add-locations         * --strip
+            command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --finder-tag-template                         line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                     * --style
+          o osxphotos-query_command               o osxphotos-diff_command_line
             line_option                             option
-    * --folder                                    o osxphotos-sync_command_line
+          o osxphotos-repl_command_line     * --syndicated
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-export_command
+    * --help                                        line_option
+          o osxphotos-run_command_line            o osxphotos-query_command
+            option                                  line_option
+    * --hidden                                    o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --selected
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --template
+          o osxphotos-query_command               o osxphotos-inspect_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
+          o osxphotos-repl_command_line     * --theme
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-batch-edit
+    * --ignore-case                                 command_line_option
+          o osxphotos-add-locations               o osxphotos-exiftool_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --force                                     o osxphotos-sync_command_line
-          o osxphotos-timewarp_command              option
-            line_option                     * --selfie
-    * --force-update                              o osxphotos-add-locations
+          o osxphotos-sync_command_line           o osxphotos-inspect_command
+            option                                  line_option
+    * --ignore-date-modified                      o osxphotos-orphans_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-timewarp_command
+    * --ignore-signature                            line_option
+          o osxphotos-export_command        * --time
+            line_option                           o osxphotos-timewarp_command
+    * --import                                      line_option
+          o osxphotos-sync_command_line     * --time-delta
+            option                                o osxphotos-timewarp_command
+    * --in-album                                    line_option
+          o osxphotos-add-locations         * --time-lapse
+            command_line_option                   o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-    * --from-date                                   line_option
-          o osxphotos-add-locations               o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-repl_command_line     * --set
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --shared
-    * --from-time                                 o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
           o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --incloud                                     option
+          o osxphotos-add-locations         * --timestamp
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-diff_command_line
           o osxphotos-repl_command_line             option
-            option                          * --sidecar
-          o osxphotos-sync_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --function                            * --sidecar-drop-ext
-          o osxphotos-timewarp_command            o osxphotos-export_command
-            line_option                             line_option
-    * --glob                                * --skip-bursts
-          o osxphotos-import_command              o osxphotos-export_command
+            option                                o osxphotos-exiftool_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-export_command
+    * --info                                        line_option
+          o osxphotos-exportdb_command            o osxphotos-exportdb_command
             line_option                             line_option
-    * --has-comment                         * --skip-edited
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --skip-live
+    * --inspect                                   o osxphotos-import_command
+          o osxphotos-timewarp_command              line_option
+            line_option                           o osxphotos-orphans_command
+    * --is-reference                                line_option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option, [1]
+          o osxphotos-query_command         * --timezone
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line             line_option
+            option                          * --title
+          o osxphotos-sync_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --jpeg-ext                                  o osxphotos-batch-edit
+          o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --skip-original-if-edited
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --skip-raw
-            option                                o osxphotos-export_command
-    * --has-likes                                   line_option
-          o osxphotos-add-locations         * --skip-uuid
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                     * --skip-uuid-from-file
-          o osxphotos-query_command               o osxphotos-export_command
+    * --jpeg-quality                                line_option
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --slow-mo
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
+    * --json                                      o osxphotos-query_command
+          o osxphotos-albums_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-dump_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-info_command_line             option
+            option                          * --tmpdir
+          o osxphotos-keywords_command            o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-labels_command        * --to-date
+            line_option                           o osxphotos-add-locations
+          o osxphotos-list_command_line             command_line_option
             option                                o osxphotos-export_command
-    * --has-raw                                     line_option
-          o osxphotos-add-locations               o osxphotos-query_command
+          o osxphotos-persons_command               line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-places_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+    * --keep                                        option
+          o osxphotos-export_command        * --to-time
+            line_option                           o osxphotos-add-locations
+    * --keyword                                     command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-batch-edit                  o osxphotos-query_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-query_command               o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-repl_command_line     * --split-folder
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --sql
-    * --hdr                                       o osxphotos-exportdb_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --strip
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command         * --style
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-repl_command_line             option
-            option                          * --syndicated
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --help                                      o osxphotos-export_command
-          o osxphotos-run_command_line              line_option
-            option                                o osxphotos-query_command
-    * --hidden                                      line_option
-          o osxphotos-add-locations               o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+          o osxphotos-import_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-query_command         * --template
-            line_option                           o osxphotos-inspect_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --theme
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --ignore-case                               o osxphotos-batch-edit
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-exiftool_command
-          o osxphotos-export_command                line_option
+          o osxphotos-query_command         * --touch-file
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-exportdb_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-import_command
+            option                                o osxphotos-exportdb_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-inspect_command
-    * --ignore-date-modified                        line_option
-          o osxphotos-exiftool_command            o osxphotos-orphans_command
-            line_option                             line_option
+            option                          * --undo
+    * --keyword-template                          o osxphotos-batch-edit
+          o osxphotos-exiftool_command              command_line_option
+            line_option                     * --unmatched
           o osxphotos-export_command              o osxphotos-sync_command_line
             line_option                             option
-    * --ignore-signature                          o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * --time
-    * --import                                    o osxphotos-timewarp_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --time-delta
-    * --in-album                                  o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --time-lapse
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --incloud                                   o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --timestamp
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-batch-edit
-            line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-diff_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-exiftool_command
+    * --label                               * --update
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * --update-errors
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --update-signatures
+          o osxphotos-repl_command_line           o osxphotos-exportdb_command
             option                                  line_option
-    * --info                                      o osxphotos-export_command
-          o osxphotos-exportdb_command              line_option
-            line_option                           o osxphotos-exportdb_command
-    * --inspect                                     line_option
-          o osxphotos-timewarp_command            o osxphotos-import_command
-            line_option                             line_option
-    * --is-reference                              o osxphotos-orphans_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
+          o osxphotos-sync_command_line     * --upgrade
+            option                                o osxphotos-install_command
+    * --last-errors                                 line_option
+          o osxphotos-exportdb_command      * --use-file-time
             line_option                           o osxphotos-timewarp_command
-          o osxphotos-query_command                 line_option, [1]
-            line_option                     * --timezone
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --title
-            option                                o osxphotos-add-locations
-    * --jpeg-ext                                    command_line_option
-          o osxphotos-export_command              o osxphotos-batch-edit
-            line_option                             command_line_option
-    * --jpeg-quality                              o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-import_command
-    * --json                                        line_option
-          o osxphotos_command_line                o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-albums_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-dump_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-info_command_line     * --tmpdir
-            option                                o osxphotos-export_command
-          o osxphotos-keywords_command              line_option
-            line_option                     * --to-date
-          o osxphotos-labels_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-list_command_line           o osxphotos-export_command
+    * --last-run                                    line_option
+          o osxphotos-exportdb_command      * --use-photokit
+            line_option                           o osxphotos-export_command
+    * --library                                     line_option
+          o osxphotos-albums_command        * --use-photos-export
+            line_option                           o osxphotos-export_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option             * --uti
+          o osxphotos-diff_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-dump_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-persons_command             o osxphotos-query_command
+          o osxphotos-exiftool_command            o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-places_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-sync_command_line
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-    * --keep                                * --to-time
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --keyword                                   o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-query_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option                   o osxphotos-repl_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-import_command                option
-            line_option                     * --touch-file
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-exportdb_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --undo
-            option                                o osxphotos-batch-edit
-    * --keyword-template                            command_line_option
-          o osxphotos-exiftool_command      * --unmatched
+          o osxphotos-info_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-inspect_command       * --uuid
+            line_option                           o osxphotos-add-locations
+          o osxphotos-keywords_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-labels_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-orphans_command               line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-persons_command               option
             line_option                           o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --update
-    * --label                                     o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --update-errors
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-places_command                option
+            line_option                     * --uuid-files
+          o osxphotos-query_command               o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-query_command         * --update-signatures
-            line_option                           o osxphotos-exportdb_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --upgrade
-          o osxphotos-sync_command_line           o osxphotos-install_command
-            option                                  line_option
-    * --last-errors                         * --use-file-time
-          o osxphotos-exportdb_command            o osxphotos-timewarp_command
-            line_option                             line_option
-    * --last-run                            * --use-photokit
-          o osxphotos-exportdb_command            o osxphotos-export_command
-            line_option                             line_option
-    * --library                             * --use-photos-export
-          o osxphotos_command_line                o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-albums_command        * --uti
-            line_option                           o osxphotos-add-locations
-          o osxphotos-batch-edit                    command_line_option
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-diff_command_line             line_option
+          o osxphotos-repl_command_line     * --uuid-from-file
+            option                                o osxphotos-add-locations
+          o osxphotos-show_command_line             command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-snap_command_line             line_option
             option                                o osxphotos-query_command
-          o osxphotos-dump_command_line             line_option
+          o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
-          o osxphotos-exiftool_command              option
+          o osxphotos-timewarp_command              option
             line_option                           o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --uuid
-          o osxphotos-info_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-inspect_command             o osxphotos-export_command
+    * --limit                                       option
+          o osxphotos-export_command        * --uuid-info
+            line_option                           o osxphotos-exportdb_command
+    * --list                                        line_option
+          o osxphotos-theme_command         * --vacuum
+            line_option                           o osxphotos-exportdb_command
+    * --live                                        line_option
+          o osxphotos-add-locations         * --verbose
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-diff_command_line
+          o osxphotos-repl_command_line             option
+            option                                o osxphotos-exiftool_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-export_command
+    * --load-config                                 line_option
+          o osxphotos-exiftool_command            o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-keywords_command            o osxphotos-query_command
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-labels_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-orphans_command             o osxphotos-sync_command_line
+    * --location                                  o osxphotos-orphans_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-batch-edit                    option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --version
+          o osxphotos-import_command              o osxphotos_command_line
             line_option                             option
-          o osxphotos-persons_command       * --uuid-files
-            line_option                           o osxphotos-exportdb_command
-          o osxphotos-places_command                line_option
-            line_option                     * --uuid-from-file
-          o osxphotos-query_command               o osxphotos-add-locations
+          o osxphotos-query_command               o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --walk
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --window
+    * --match-time                                o osxphotos-add-locations
+          o osxphotos-timewarp_command              command_line_option
+            line_option                     * --xattr-template
+    * --max-size                                  o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --year
+          o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-show_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-snap_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-timewarp_command      * --uuid-info
-            line_option                           o osxphotos-exportdb_command
-    * --limit                                       line_option
-          o osxphotos-export_command        * --vacuum
-            line_option                           o osxphotos-exportdb_command
-    * --list                                        line_option
-          o osxphotos-theme_command         * --verbose
-            line_option                           o osxphotos-add-locations
-    * --live                                        command_line_option
-          o osxphotos-add-locations               o osxphotos-batch-edit
-            command_line_option                     command_line_option
-          o osxphotos-export_command              o osxphotos-diff_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-exiftool_command
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-exportdb_command
+          o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
-    * --load-config                               o osxphotos-import_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-orphans_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-sync_command_line
-    * --location                                    option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-batch-edit            * --version
-            command_line_option                   o osxphotos_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-exportdb_command
-          o osxphotos-import_command                line_option
-            line_option                     * --walk
-          o osxphotos-query_command               o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --window
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
-            option                          * --xattr-template
-    * --match-time                                o osxphotos-export_command
-          o osxphotos-timewarp_command              line_option
-            line_option                     * --year
-    * --max-size                                  o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --merge                                     o osxphotos-sync_command_line
           o osxphotos-sync_command_line             option
             option                          * --yes
-    * --merge                                     o osxphotos-uninstall_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -A
-    * --merge-keywords                            o osxphotos-sync_command_line
-          o osxphotos-import_command                option
+    * --merge-keywords                            o osxphotos-uninstall_command
+          o osxphotos-import_command                line_option
+            line_option                     * -A
+    * --migrate                                   o osxphotos-sync_command_line
+          o osxphotos-exportdb_command              option
             line_option                     * -a
-    * --migrate                                   o osxphotos-import_command
+    * --migrate-photos-library                    o osxphotos-import_command
           o osxphotos-exportdb_command              line_option
             line_option                           o osxphotos-timewarp_command
-    * --migrate-photos-library                      line_option
-          o osxphotos-exportdb_command      * -C
-            line_option                           o osxphotos-import_command
     * --min-size                                    line_option
-          o osxphotos-add-locations         * -c
-            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-add-locations         * -C
+            command_line_option                   o osxphotos-import_command
           o osxphotos-export_command                line_option
-            line_option                     * -D
-          o osxphotos-query_command               o osxphotos-import_command
+            line_option                     * -c
+          o osxphotos-query_command               o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * -d
+          o osxphotos-repl_command_line     * -D
             option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-timewarp_command
     * --missing                                     line_option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -e
-            line_option                           o osxphotos-import_command
+          o osxphotos-add-locations         * -d
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-timewarp_command
           o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-timewarp_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -F
+            line_option                     * -e
+          o osxphotos-repl_command_line           o osxphotos-import_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
     * --name                                      o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -f
-          o osxphotos-export_command              o osxphotos-dump_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-    * --no-comment                                o osxphotos-uuid_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * -g
-          o osxphotos-export_command              o osxphotos-import_command
+            command_line_option             * -F
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-query_command         * -h
-            line_option                           o osxphotos-run_command_line
+          o osxphotos-query_command         * -f
+            line_option                           o osxphotos-dump_command_line
           o osxphotos-repl_command_line             option
-            option                          * -i
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --no-description                            o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-query_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-repl_command_line             option, [1]
-            option                                o osxphotos-timewarp_command
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                          * -k
-    * --no-keyword                                o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -L
-          o osxphotos-export_command              o osxphotos-import_command
+            option                                o osxphotos-query_command
+    * --no-comment                                  line_option
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-uuid_command_line
+            line_option                             option
+          o osxphotos-query_command         * -g
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                          * -h
+          o osxphotos-sync_command_line           o osxphotos-run_command_line
+            option                                  option
+    * --no-description                      * -i
+          o osxphotos-add-locations               o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-timewarp_command
+          o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * -l
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -M
-    * --no-likes                                  o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option, [1]
+    * --no-keyword                                o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -m
+            command_line_option             * -k
           o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * -P
-            option                                o osxphotos-import_command
-    * --no-location                                 line_option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -p
+          o osxphotos-query_command         * -L
             line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-timewarp_command
           o osxphotos-repl_command_line             line_option
-            option                          * -R
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --no-place                                  o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * -r
-          o osxphotos-export_command              o osxphotos-diff_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-import_command
+            option                                o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -l
+    * --no-likes                                  o osxphotos-import_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -M
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * -s
-            option                                o osxphotos-diff_command_line
-          o osxphotos-sync_command_line             option
+          o osxphotos-query_command         * -m
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-sync_command_line
-    * --no-progress                                 option
-          o osxphotos-export_command        * -T
-            line_option                           o osxphotos-inspect_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-timewarp_command
-    * --no-title                                    line_option
-          o osxphotos-add-locations         * -t
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-timewarp_command
+    * --no-location                                 line_option
+          o osxphotos-add-locations         * -P
             command_line_option                   o osxphotos-import_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-inspect_command
-          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-timewarp_command
-          o osxphotos-repl_command_line             line_option
-            option                          * -U
-          o osxphotos-sync_command_line           o osxphotos-install_command
+          o osxphotos-query_command                 line_option
+            line_option                     * -p
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-    * --not-burst                                 o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * -V
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-batch-edit
-            line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-diff_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-exiftool_command
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --not-cloudasset                            o osxphotos-export_command
+    * --no-place                            * -R
+          o osxphotos-add-locations               o osxphotos-import_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * -r
+            line_option                           o osxphotos-diff_command_line
+          o osxphotos-repl_command_line             option
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -s
+    * --no-progress                               o osxphotos-diff_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-import_command                option
+            line_option                     * -T
+    * --no-title                                  o osxphotos-inspect_command
           o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-exportdb_command
+            command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-orphans_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-timewarp_command
-    * --not-edited                                  line_option
-          o osxphotos-add-locations         * -v
-            command_line_option                   o osxphotos_command_line
-          o osxphotos-export_command                option
-            line_option                     * -w
-          o osxphotos-query_command               o osxphotos-add-locations
-            line_option                             command_line_option
+            line_option                     * -t
+          o osxphotos-query_command               o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-inspect_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --not-burst                           * -U
+          o osxphotos-add-locations               o osxphotos-install_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * -V
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-batch-edit
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-diff_command_line
+    * --not-cloudasset                              option
+          o osxphotos-add-locations               o osxphotos-exiftool_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-exportdb_command
+            line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-          o osxphotos-sync_command_line     * -y
-            option                                o osxphotos-uninstall_command
-    * --not-favorite                                line_option
-          o osxphotos-add-locations         * -z
+          o osxphotos-sync_command_line           o osxphotos-orphans_command
+            option                                  line_option
+    * --not-edited                                o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option
-          o osxphotos-query_command
-            line_option
+            line_option                     * -v
+          o osxphotos-query_command               o osxphotos_command_line
+            line_option                             option
+          o osxphotos-repl_command_line     * -w
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-import_command
+    * --not-favorite                                line_option
+          o osxphotos-add-locations         * -y
+            command_line_option                   o osxphotos-uninstall_command
+          o osxphotos-export_command                line_option
+            line_option                     * -z
+          o osxphotos-query_command               o osxphotos-timewarp_command
+            line_option                             line_option
           o osxphotos-repl_command_line
             option
           o osxphotos-sync_command_line
             option
 
 ***** A *****
     * activities_(osxphotos.SearchInfo
-      property)                             * albums_shared_as_dict_
-    * added_after_                            (osxphotos.PhotosDB_property)
-      (osxphotos.QueryOptions               * AlbumSortOrder_(class_in
-      attribute)                              osxphotos)
-    * added_before_                         * all_(osxphotos.SearchInfo
-      (osxphotos.QueryOptions                 property)
-      attribute)                            * all_files()_
-    * added_in_last_                          (osxphotos.ExportResults_method)
-      (osxphotos.QueryOptions               * ARGS
-      attribute)                                  o osxphotos-run_command_line
-    * addvalues()_(osxphotos.ExifTool               option
-      method)                               * asdict()_(osxphotos.AlbumInfo
-    * adjustments_(osxphotos.PhotoInfo        method)
-      property)                                   o (osxphotos.ExifTool_method)
-    * album_(osxphotos.QueryOptions               o (osxphotos.FolderInfo
-      attribute)                                    method)
-    * album_info_(osxphotos.FolderInfo            o (osxphotos.ImportInfo
-      property)                                     method)
-          o (osxphotos.PhotoInfo                  o (osxphotos.MomentInfo
-            property)                               method)
-          o (osxphotos.PhotosDB                   o (osxphotos.PersonInfo
-            property)                               method)
-    * album_info_shared_                          o (osxphotos.PhotoInfo
-      (osxphotos.PhotosDB_property)                 method)
-    * AlbumInfo_(class_in_osxphotos)              o (osxphotos.ScoreInfo
-    * albums_(osxphotos.PhotoInfo                   method)
-      property)                                   o (osxphotos.SearchInfo
-          o (osxphotos.PhotosDB                     method)
-            property)                       * attributes_
-    * albums_as_dict_                         (osxphotos.ExportResults
-      (osxphotos.PhotosDB_property)           property)
-    * albums_shared_(osxphotos.PhotosDB
       property)
+    * added_after_                         * albums_shared_(osxphotos.PhotosDB
+      (osxphotos.QueryOptions                property)
+      attribute)                           * albums_shared_as_dict_
+    * added_before_                          (osxphotos.PhotosDB_property)
+      (osxphotos.QueryOptions              * AlbumSortOrder_(class_in
+      attribute)                             osxphotos)
+    * added_in_last_                       * all_(osxphotos.SearchInfo
+      (osxphotos.QueryOptions                property)
+      attribute)                           * all_files()_
+    * address_(osxphotos.PlaceInfo           (osxphotos.ExportResults_method)
+      property)                            * ARGS
+    * address_str_(osxphotos.PlaceInfo           o osxphotos-run_command_line
+      property)                                    option
+    * addvalues()_(osxphotos.ExifTool      * asdict()_(osxphotos.AlbumInfo
+      method)                                method)
+    * adjustments_(osxphotos.PhotoInfo           o (osxphotos.ExifTool_method)
+      property)                                  o (osxphotos.FaceInfo_method)
+    * album_(osxphotos.QueryOptions              o (osxphotos.FolderInfo
+      attribute)                                   method)
+    * album_info_(osxphotos.FolderInfo           o (osxphotos.ImportInfo
+      property)                                    method)
+          o (osxphotos.PhotoInfo                 o (osxphotos.MomentInfo
+            property)                              method)
+          o (osxphotos.PhotosDB                  o (osxphotos.PersonInfo
+            property)                              method)
+    * album_info_shared_                         o (osxphotos.PhotoInfo_method)
+      (osxphotos.PhotosDB_property)              o (osxphotos.ScoreInfo_method)
+    * AlbumInfo_(class_in_osxphotos)             o (osxphotos.SearchInfo
+    * albums_(osxphotos.PhotoInfo                  method)
+      property)                            * attributes_
+          o (osxphotos.PhotosDB              (osxphotos.ExportResults_property)
+            property)
+    * albums_as_dict_
+      (osxphotos.PhotosDB_property)
 
 ***** B *****
     * bit_flags_                          * burst_albums_(osxphotos.PhotoInfo
       (osxphotos.ExportOptions              property)
       property)                           * burst_default_pick_
     * bodies_of_water_                      (osxphotos.PhotoInfo_property)
       (osxphotos.SearchInfo_property)     * burst_key_(osxphotos.PhotoInfo
@@ -983,32 +979,34 @@
           o (osxphotos.QueryOptions         property)
             attribute)                          o (osxphotos.QueryOptions
     * burst_album_info_                           attribute)
       (osxphotos.PhotoInfo_property)      * burst_selected_
                                             (osxphotos.PhotoInfo_property)
 
 ***** C *****
-                                             * comments_(osxphotos.PhotoInfo
-    * camera_(osxphotos.SearchInfo             property)
-      property)                              * connection_(osxphotos.ExportDB
-    * city_(osxphotos.SearchInfo               property)
-      property)                              * convert_to_jpeg_
-    * close()_(osxphotos.ExportDB              (osxphotos.ExportOptions
-      method)                                  attribute)
-    * cloud_guid_(osxphotos.PhotoInfo        * convert_to_jpeg()_
-      property)                                (osxphotos.FileUtilNoOp_class
-    * cloud_metadata_                          method)
-      (osxphotos.PhotoInfo_property)         * copy()_(osxphotos.FileUtilNoOp
-    * cloud_owner_hashed_id_                   class_method)
-      (osxphotos.PhotoInfo_property)         * country_(osxphotos.SearchInfo
-    * cloudasset_(osxphotos.QueryOptions       property)
-      attribute)                             * create_file_record()_
-    * CommentInfo_(class_in_osxphotos)         (osxphotos.ExportDB_method)
-                                             * create_or_get_file_record()_
-                                               (osxphotos.ExportDB_method)
+                                           * comments_(osxphotos.PhotoInfo
+    * camera_(osxphotos.SearchInfo           property)
+      property)                            * connection_(osxphotos.ExportDB
+    * center_(osxphotos.FaceInfo             property)
+      property)                            * convert_to_jpeg_
+    * city_(osxphotos.SearchInfo             (osxphotos.ExportOptions
+      property)                              attribute)
+    * close()_(osxphotos.ExportDB          * convert_to_jpeg()_
+      method)                                (osxphotos.FileUtilNoOp_class
+    * cloud_guid_(osxphotos.PhotoInfo        method)
+      property)                            * copy()_(osxphotos.FileUtilNoOp
+    * cloud_metadata_                        class_method)
+      (osxphotos.PhotoInfo_property)       * country_(osxphotos.SearchInfo
+    * cloud_owner_hashed_id_                 property)
+      (osxphotos.PhotoInfo_property)       * country_code_(osxphotos.PlaceInfo
+    * cloudasset_                            property)
+      (osxphotos.QueryOptions              * create_file_record()_
+      attribute)                             (osxphotos.ExportDB_method)
+    * CommentInfo_(class_in_osxphotos)     * create_or_get_file_record()_
+                                             (osxphotos.ExportDB_method)
 
 ***** D *****
                                             * deleted_(osxphotos.QueryOptions
                                               attribute)
     * date_(osxphotos.MomentInfo            * deleted_only_
       property)                               (osxphotos.QueryOptions
           o (osxphotos.PhotoInfo              attribute)
@@ -1063,43 +1061,44 @@
     * expand_variables()_                     osxphotos)
       (osxphotos.PhotoTemplate_method)      * external_edit_
     * expand_variables_to_str()_              (osxphotos.PhotoInfo_property)
       (osxphotos.PhotoTemplate_method)            o (osxphotos.QueryOptions
                                                     attribute)
 
 ***** F *****
-    * face_info_(osxphotos.PersonInfo
-      property)                             * FileUtilNoOp_(class_in_osxphotos)
-          o (osxphotos.PhotoInfo            * filter_predicate()_
-            property)                         (osxphotos.PhotoTemplate_method)
-    * face_regions_                         * fingerprint_(osxphotos.PhotoInfo
-      (osxphotos.ExportOptions                property)
-      attribute)                            * folder_(osxphotos.QueryOptions
-    * favorite_(osxphotos.PersonInfo          attribute)
-      property)                             * folder_info_(osxphotos.PhotosDB
-          o (osxphotos.PhotoInfo              property)
-            property)                       * folder_list_(osxphotos.AlbumInfo
-          o (osxphotos.QueryOptions           property)
-            attribute)                            o (osxphotos.ProjectInfo
-    * favorite_rating_                              property)
-      (osxphotos.ExportOptions              * folder_names_(osxphotos.AlbumInfo
-      attribute)                              property)
-    * feature_less_                               o (osxphotos.ProjectInfo
-      (osxphotos.PersonInfo_property)               property)
-    * file_sig()_                           * FolderInfo_(class_in_osxphotos)
-      (osxphotos.FileUtilNoOp_class         * folders_(osxphotos.PhotosDB
-      method)                                 property)
-    * filename_(osxphotos.PhotoInfo         * force_update_
-      property)                               (osxphotos.ExportOptions
-    * FILES                                   attribute)
-          o osxphotos-import_command        * from_date_(osxphotos.QueryOptions
-            line_option                       attribute)
-    * FileUtil_(class_in_osxphotos)         * function_(osxphotos.QueryOptions
-    * fileutil_(osxphotos.ExportOptions       attribute)
-      attribute)
+    * face_info_(osxphotos.PersonInfo     * fileutil_(osxphotos.ExportOptions
+      property)                             attribute)
+          o (osxphotos.PhotoInfo          * FileUtilNoOp_(class_in_osxphotos)
+            property)                     * filter_predicate()_
+    * face_rect()_(osxphotos.FaceInfo       (osxphotos.PhotoTemplate_method)
+      method)                             * fingerprint_(osxphotos.PhotoInfo
+    * face_regions_                         property)
+      (osxphotos.ExportOptions            * folder_(osxphotos.QueryOptions
+      attribute)                            attribute)
+    * FaceInfo_(class_in_osxphotos)       * folder_info_(osxphotos.PhotosDB
+    * favorite_(osxphotos.PersonInfo        property)
+      property)                           * folder_list_(osxphotos.AlbumInfo
+          o (osxphotos.PhotoInfo            property)
+            property)                           o (osxphotos.ProjectInfo
+          o (osxphotos.QueryOptions               property)
+            attribute)                    * folder_names_(osxphotos.AlbumInfo
+    * favorite_rating_                      property)
+      (osxphotos.ExportOptions                  o (osxphotos.ProjectInfo
+      attribute)                                  property)
+    * feature_less_                       * FolderInfo_(class_in_osxphotos)
+      (osxphotos.PersonInfo_property)     * folders_(osxphotos.PhotosDB
+    * file_sig()_                           property)
+      (osxphotos.FileUtilNoOp_class       * force_update_
+      method)                               (osxphotos.ExportOptions
+    * filename_(osxphotos.PhotoInfo         attribute)
+      property)                           * from_date_(osxphotos.QueryOptions
+    * FILES                                 attribute)
+          o osxphotos-import_command      * function_(osxphotos.QueryOptions
+            line_option                     attribute)
+    * FileUtil_(class_in_osxphotos)
 
 ***** G *****
     * get_db_connection()_                 * get_photo_video_type()_
       (osxphotos.PhotosDB_method)            (osxphotos.PhotoTemplate_method)
     * get_export_results()_                * get_photoinfo_for_uuid()_
       (osxphotos.ExportDB_method)            (osxphotos.ExportDB_method)
     * get_exported_files()_                * get_previous_uuids()_
@@ -1135,42 +1134,45 @@
       property)                               property)
           o (osxphotos.QueryOptions               o (osxphotos.QueryOptions
             attribute)                              attribute)
     * hasadjustments_                       * holidays_(osxphotos.SearchInfo
       (osxphotos.PhotoInfo_property)          property)
 
 ***** I *****
-    * ignore_case_                         * increment_(osxphotos.ExportOptions
-      (osxphotos.QueryOptions                attribute)
+    * ignore_case_
+      (osxphotos.QueryOptions
       attribute)                           * intrash_(osxphotos.PhotoInfo
     * ignore_date_modified_                  property)
       (osxphotos.ExportOptions             * is_debug()_(in_module_osxphotos)
       attribute)                           * is_reference_
     * ignore_signature_                      (osxphotos.QueryOptions_attribute)
       (osxphotos.ExportOptions             * iscloudasset_(osxphotos.PhotoInfo
       attribute)                             property)
-    * import_info_(osxphotos.PhotoInfo     * ismissing_(osxphotos.PhotoInfo
+    * import_info_(osxphotos.PhotoInfo     * ishome_(osxphotos.PlaceInfo
       property)                              property)
-          o (osxphotos.PhotosDB            * ismovie_(osxphotos.PhotoInfo
+          o (osxphotos.PhotosDB            * ismissing_(osxphotos.PhotoInfo
             property)                        property)
-    * ImportInfo_(class_in_osxphotos)      * isphoto_(osxphotos.PhotoInfo
+    * ImportInfo_(class_in_osxphotos)      * ismovie_(osxphotos.PhotoInfo
     * in_album_(osxphotos.QueryOptions       property)
-      attribute)                           * israw_(osxphotos.PhotoInfo
+      attribute)                           * isphoto_(osxphotos.PhotoInfo
     * incloud_(osxphotos.PhotoInfo           property)
-      property)                            * isreference_(osxphotos.PhotoInfo
+      property)                            * israw_(osxphotos.PhotoInfo
           o (osxphotos.QueryOptions          property)
-            attribute)
+            attribute)                     * isreference_(osxphotos.PhotoInfo
+    * increment_                             property)
+      (osxphotos.ExportOptions
+      attribute)
 
 ***** J *****
-    * jpeg_ext_(osxphotos.ExportOptions     * json()_(osxphotos.ExifTool
-      attribute)                              method)
-    * jpeg_quality_                               o (osxphotos.PersonInfo
-      (osxphotos.ExportOptions                      method)
-      attribute)                                  o (osxphotos.PhotoInfo
-                                                    method)
+    * jpeg_ext_(osxphotos.ExportOptions_attribute)
+    * jpeg_quality_(osxphotos.ExportOptions_attribute)
+    * json()_(osxphotos.ExifTool_method)
+          o (osxphotos.FaceInfo_method)
+          o (osxphotos.PersonInfo_method)
+          o (osxphotos.PhotoInfo_method)
 
 ***** K *****
     * keyword_(osxphotos.QueryOptions     * keywords_(osxphotos.PhotoInfo
       attribute)                            property)
     * keyword_template_                         o (osxphotos.PhotosDB_property)
       (osxphotos.ExportOptions            * keywords_as_dict_
       attribute)                            (osxphotos.PhotosDB_property)
@@ -1196,631 +1198,635 @@
     * library_path_(osxphotos.PhotosDB             property)
       property)                                  o (osxphotos.QueryOptions
                                                    attribute)
 
 ***** M *****
     * max_size_(osxphotos.QueryOptions
       attribute)
-    * media_types_(osxphotos.SearchInfo      * modification_date_
-      property)                                (osxphotos.MomentInfo_property)
-    * merge_exif_keywords_                   * module
-      (osxphotos.ExportOptions                     o osxphotos
-      attribute)                             * moment_info_(osxphotos.PhotoInfo
-    * merge_exif_persons_                      property)
-      (osxphotos.ExportOptions               * MomentInfo_(class_in_osxphotos)
-      attribute)                             * month_(osxphotos.SearchInfo
-    * min_size_(osxphotos.QueryOptions         property)
-      attribute)                             * movies_(osxphotos.QueryOptions
-    * missing_(osxphotos.QueryOptions          attribute)
+    * media_types_(osxphotos.SearchInfo
+      property)                             * module
+    * merge_exif_keywords_                        o osxphotos
+      (osxphotos.ExportOptions              * moment_info_(osxphotos.PhotoInfo
+      attribute)                              property)
+    * merge_exif_persons_                   * MomentInfo_(class_in_osxphotos)
+      (osxphotos.ExportOptions              * month_(osxphotos.SearchInfo
+      attribute)                              property)
+    * min_size_(osxphotos.QueryOptions      * movies_(osxphotos.QueryOptions
+      attribute)                              attribute)
+    * missing_(osxphotos.QueryOptions       * mpri_reg_rect_(osxphotos.FaceInfo
+      attribute)                              property)
+    * missing_bursts_                       * mwg_rs_area_(osxphotos.FaceInfo
+      (osxphotos.QueryOptions                 property)
       attribute)
-    * missing_bursts_
-      (osxphotos.QueryOptions_attribute)
+    * modification_date_
+      (osxphotos.MomentInfo_property)
 
 ***** N *****
+                                            * not_hdr_(osxphotos.QueryOptions
+                                              attribute)
                                             * not_hidden_
                                               (osxphotos.QueryOptions
-                                              attribute)
-                                            * not_in_album_
-    * name_(osxphotos.QueryOptions            (osxphotos.QueryOptions
-      attribute)                              attribute)
-    * neighborhoods_                        * not_incloud_
-      (osxphotos.SearchInfo_property)         (osxphotos.QueryOptions
+    * name_(osxphotos.PlaceInfo               attribute)
+      property)                             * not_in_album_
+          o (osxphotos.QueryOptions           (osxphotos.QueryOptions
+            attribute)                        attribute)
+    * names_(osxphotos.PlaceInfo            * not_incloud_
+      property)                               (osxphotos.QueryOptions
+    * neighborhoods_                          attribute)
+      (osxphotos.SearchInfo_property)       * not_live_(osxphotos.QueryOptions
     * no_comment_                             attribute)
-      (osxphotos.QueryOptions               * not_live_(osxphotos.QueryOptions
-      attribute)                              attribute)
-    * no_description_                       * not_missing_
-      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
-      attribute)                              attribute)
-    * no_keyword_                           * not_panorama_
-      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
-      attribute)                              attribute)
-    * no_likes_(osxphotos.QueryOptions      * not_portrait_
+      (osxphotos.QueryOptions               * not_missing_
+      attribute)                              (osxphotos.QueryOptions
+    * no_description_                         attribute)
+      (osxphotos.QueryOptions               * not_panorama_
       attribute)                              (osxphotos.QueryOptions
-    * no_location_                            attribute)
-      (osxphotos.QueryOptions               * not_reference_
+    * no_keyword_                             attribute)
+      (osxphotos.QueryOptions               * not_portrait_
       attribute)                              (osxphotos.QueryOptions
-    * no_place_(osxphotos.QueryOptions        attribute)
+    * no_likes_(osxphotos.QueryOptions        attribute)
+      attribute)                            * not_reference_
+    * no_location_                            (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
       attribute)                            * not_saved_to_library_
-    * no_title_(osxphotos.QueryOptions        (osxphotos.QueryOptions
+    * no_place_(osxphotos.QueryOptions        (osxphotos.QueryOptions
       attribute)                              attribute)
-    * not_burst_(osxphotos.QueryOptions     * not_screenshot_
-      attribute)                              (osxphotos.QueryOptions
-    * not_cloudasset_                         attribute)
-      (osxphotos.QueryOptions               * not_selfie_
+    * no_title_(osxphotos.QueryOptions      * not_screenshot_
       attribute)                              (osxphotos.QueryOptions
-    * not_edited_                             attribute)
-      (osxphotos.QueryOptions               * not_shared_
-      attribute)                              (osxphotos.QueryOptions
-    * not_favorite_                           attribute)
-      (osxphotos.QueryOptions               * not_slow_mo_
-      attribute)                              (osxphotos.QueryOptions
-    * not_hdr_(osxphotos.QueryOptions         attribute)
+    * not_burst_(osxphotos.QueryOptions       attribute)
+      attribute)                            * not_selfie_
+    * not_cloudasset_                         (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
+      attribute)                            * not_shared_
+    * not_edited_                             (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
+      attribute)                            * not_slow_mo_
+    * not_favorite_                           (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
       attribute)                            * not_syndicated_
                                               (osxphotos.QueryOptions
                                               attribute)
                                             * not_time_lapse_
                                               (osxphotos.QueryOptions
                                               attribute)
 
 ***** O *****
-                                            * osxphotos-info command line
-                                              option
-                                                  o --db
-                                                  o --json
-    * orientation_(osxphotos.PhotoInfo            o --library
-      property)                                   o PHOTOS_LIBRARY
-    * original_filename_                    * osxphotos-inspect command line
-      (osxphotos.PhotoInfo_property)          option
-    * original_filesize_                          o --db
+    * orientation_(osxphotos.PhotoInfo      * osxphotos-inspect command line
+      property)                               option
+    * original_filename_                          o --db
       (osxphotos.PhotoInfo_property)              o --detect-text
-    * original_height_                            o --library
+    * original_filesize_                          o --library
       (osxphotos.PhotoInfo_property)              o --template
-    * original_orientation_                       o --theme
+    * original_height_                            o --theme
       (osxphotos.PhotoInfo_property)              o -t
-    * original_width_                             o -T
+    * original_orientation_                       o -T
       (osxphotos.PhotoInfo_property)        * osxphotos-install command line
-    * osxphotos                               option
-          o module                                o --upgrade
-    * osxphotos command line option               o -U
-          o --db                                  o PACKAGES
-          o --json                          * osxphotos-keywords command line
+    * original_width_                         option
+      (osxphotos.PhotoInfo_property)              o --upgrade
+    * osxphotos                                   o -U
+          o module                                o PACKAGES
+    * osxphotos command line option         * osxphotos-keywords command line
+          o --version                         option
+          o -v                                    o --db
+    * osxphotos-add-locations command             o --json
+      line option                                 o --library
+          o --added-after                         o PHOTOS_LIBRARY
+          o --added-before                  * osxphotos-labels command line
+          o --added-in-last                   option
+          o --album                               o --db
+          o --burst                               o --json
+          o --cloudasset                          o --library
+          o --description                         o PHOTOS_LIBRARY
+          o --dry-run                       * osxphotos-list command line
+          o --duplicate                       option
+          o --edited                              o --json
+          o --exif                          * osxphotos-orphans command line
+          o --external-edit                   option
+          o --favorite                            o --db
+          o --folder                              o --export
+          o --from-date                           o --library
+          o --from-time                           o --theme
+          o --has-comment                         o --timestamp
+          o --has-likes                           o --verbose
+          o --has-raw                             o -V
+          o --hdr                           * osxphotos-persons command line
+          o --hidden                          option
+          o --ignore-case                         o --db
+          o --in-album                            o --json
+          o --incloud                             o --library
+          o --is-reference                        o PHOTOS_LIBRARY
+          o --keyword                       * osxphotos-places command line
+          o --label                           option
+          o --live                                o --db
+          o --location                            o --json
+          o --max-size                            o --library
+          o --min-size                            o PHOTOS_LIBRARY
+          o --missing                       * osxphotos-query command line
+          o --name                            option
+          o --no-comment                          o --add-to-album
+          o --no-description                      o --added-after
+          o --no-keyword                          o --added-before
+          o --no-likes                            o --added-in-last
+          o --no-location                         o --album
+          o --no-place                            o --burst
+          o --no-title                            o --cloudasset
+          o --not-burst                           o --count
+          o --not-cloudasset                      o --db
+          o --not-edited                          o --deleted
+          o --not-favorite                        o --deleted-only
+          o --not-hdr                             o --description
+          o --not-hidden                          o --duplicate
+          o --not-in-album                        o --edited
+          o --not-incloud                         o --exif
+          o --not-live                            o --external-edit
+          o --not-missing                         o --favorite
+          o --not-panorama                        o --field
+          o --not-portrait                        o --folder
+          o --not-reference                       o --from-date
+          o --not-saved-to-library                o --from-time
+          o --not-screenshot                      o --has-comment
+          o --not-selfie                          o --has-likes
+          o --not-shared                          o --has-raw
+          o --not-slow-mo                         o --hdr
+          o --not-syndicated                      o --hidden
+          o --not-time-lapse                      o --ignore-case
+          o --only-movies                         o --in-album
+          o --only-photos                         o --incloud
+          o --panorama                            o --is-reference
+          o --person                              o --json
+          o --place                               o --keyword
+          o --portrait                            o --label
+          o --query-eval                          o --library
+          o --query-function                      o --live
+          o --regex                               o --location
+          o --saved-to-library                    o --max-size
+          o --screenshot                          o --min-size
+          o --selected                            o --missing
+          o --selfie                              o --name
+          o --shared                              o --no-comment
+          o --slow-mo                             o --no-description
+          o --syndicated                          o --no-keyword
+          o --theme                               o --no-likes
+          o --time-lapse                          o --no-location
+          o --timestamp                           o --no-place
+          o --title                               o --no-title
+          o --to-date                             o --not-burst
+          o --to-time                             o --not-cloudasset
+          o --uti                                 o --not-edited
+          o --uuid                                o --not-favorite
+          o --uuid-from-file                      o --not-hdr
+          o --verbose                             o --not-hidden
+          o --window                              o --not-in-album
+          o --year                                o --not-incloud
+          o -i                                    o --not-live
+          o -V                                    o --not-missing
+          o -w                                    o --not-panorama
+    * osxphotos-albums command line               o --not-portrait
+      option                                      o --not-reference
+          o --db                                  o --not-saved-to-library
+          o --json                                o --not-screenshot
+          o --library                             o --not-selfie
+          o PHOTOS_LIBRARY                        o --not-shared
+    * osxphotos-batch-edit command line           o --not-slow-mo
+      option                                      o --not-syndicated
+          o --db                                  o --not-time-lapse
+          o --description                         o --only-movies
+          o --dry-run                             o --only-photos
+          o --keyword                             o --panorama
+          o --library                             o --person
+          o --location                            o --place
+          o --replace-keywords                    o --portrait
+          o --theme                               o --print
+          o --timestamp                           o --query-eval
+          o --title                               o --query-function
+          o --undo                                o --quiet
+          o --verbose                             o --regex
+          o -V                                    o --saved-to-library
+    * osxphotos-diff command line                 o --screenshot
+      option                                      o --selected
+          o --db                                  o --selfie
+          o --library                             o --shared
+          o --raw-output                          o --slow-mo
+          o --style                               o --syndicated
+          o --timestamp                           o --time-lapse
+          o --verbose                             o --title
+          o -r                                    o --to-date
+          o -s                                    o --to-time
+          o -V                                    o --uti
+          o DB2                                   o --uuid
+    * osxphotos-dump command line                 o --uuid-from-file
+      option                                      o --year
+          o --db                                  o -f
+          o --deleted                             o -i
+          o --deleted-only                        o PHOTOS_LIBRARY
+          o --field                         * osxphotos-repl command line
+          o --json                            option
+          o --library                             o --added-after
+          o --print                               o --added-before
+          o -f                                    o --added-in-last
+          o PHOTOS_LIBRARY                        o --album
+    * osxphotos-exiftool command line             o --burst
+      option                                      o --cloudasset
+          o --album-keyword                       o --db
+          o --append                              o --deleted
+          o --db                                  o --deleted-only
+          o --db-config                           o --description
+          o --description-template                o --duplicate
+          o --dry-run                             o --edited
+          o --exiftool-merge-keywords             o --emacs
+          o --exiftool-merge-persons              o --exif
+          o --exiftool-option                     o --external-edit
+          o --exiftool-path                       o --favorite
+          o --exportdb                            o --folder
+          o --ignore-date-modified                o --from-date
+          o --keyword-template                    o --from-time
+          o --library                             o --has-comment
+          o --load-config                         o --has-likes
+          o --person-keyword                      o --has-raw
+          o --replace-keywords                    o --hdr
+          o --report                              o --hidden
+          o --save-config                         o --ignore-case
+          o --theme                               o --in-album
+          o --timestamp                           o --incloud
+          o --verbose                             o --is-reference
+          o -V                                    o --keyword
+          o EXPORT_DIRECTORY                      o --label
+    * osxphotos-export command line               o --library
+      option                                      o --live
+          o --add-exported-to-album               o --location
+          o --add-missing-to-album                o --max-size
+          o --add-skipped-to-album                o --min-size
+          o --added-after                         o --missing
+          o --added-before                        o --name
+          o --added-in-last                       o --no-comment
+          o --album                               o --no-description
+          o --album-keyword                       o --no-keyword
+          o --alt-copy                            o --no-likes
+          o --append                              o --no-location
+          o --burst                               o --no-place
+          o --cleanup                             o --no-title
+          o --cloudasset                          o --not-burst
+          o --config-only                         o --not-cloudasset
+          o --convert-to-jpeg                     o --not-edited
+          o --current-name                        o --not-favorite
+          o --db                                  o --not-hdr
+          o --deleted                             o --not-hidden
+          o --deleted-only                        o --not-in-album
+          o --description                         o --not-incloud
+          o --description-template                o --not-live
+          o --directory                           o --not-missing
+          o --download-missing                    o --not-panorama
+          o --dry-run                             o --not-portrait
+          o --duplicate                           o --not-reference
+          o --edited                              o --not-saved-to-library
+          o --edited-suffix                       o --not-screenshot
+          o --exif                                o --not-selfie
+          o --exiftool                            o --not-shared
+          o --exiftool-merge-keywords             o --not-slow-mo
+          o --exiftool-merge-persons              o --not-syndicated
+          o --exiftool-option                     o --not-time-lapse
+          o --exiftool-path                       o --only-movies
+          o --export-as-hardlink                  o --only-photos
+          o --export-by-date                      o --panorama
+          o --exportdb                            o --person
+          o --external-edit                       o --place
+          o --favorite                            o --portrait
+          o --favorite-rating                     o --query-eval
+          o --filename                            o --query-function
+          o --finder-tag-keywords                 o --regex
+          o --finder-tag-template                 o --saved-to-library
+          o --folder                              o --screenshot
+          o --force-update                        o --selected
+          o --from-date                           o --selfie
+          o --from-time                           o --shared
+          o --has-comment                         o --slow-mo
+          o --has-likes                           o --syndicated
+          o --has-raw                             o --time-lapse
+          o --hdr                                 o --title
+          o --hidden                              o --to-date
+          o --ignore-case                         o --to-time
+          o --ignore-date-modified                o --uti
+          o --ignore-signature                    o --uuid
+          o --in-album                            o --uuid-from-file
+          o --incloud                             o --year
+          o --is-reference                        o -i
+          o --jpeg-ext                      * osxphotos-run command line option
+          o --jpeg-quality                        o --help
+          o --keep                                o -h
+          o --keyword                             o ARGS
+          o --keyword-template                    o PYTHON_FILE
+          o --label                         * osxphotos-show command line
           o --library                         option
-          o --version                             o --db
-          o -v                                    o --json
-    * osxphotos-add-locations command             o --library
-      line option                                 o PHOTOS_LIBRARY
-          o --added-after                   * osxphotos-labels command line
-          o --added-before                    option
-          o --added-in-last                       o --db
-          o --album                               o --json
-          o --burst                               o --library
-          o --cloudasset                          o PHOTOS_LIBRARY
-          o --description                   * osxphotos-list command line
-          o --dry-run                         option
-          o --duplicate                           o --json
-          o --edited                        * osxphotos-orphans command line
-          o --exif                            option
-          o --external-edit                       o --db
-          o --favorite                            o --export
-          o --folder                              o --library
-          o --from-date                           o --theme
-          o --from-time                           o --timestamp
-          o --has-comment                         o --verbose
-          o --has-likes                           o -V
-          o --has-raw                       * osxphotos-persons command line
-          o --hdr                             option
-          o --hidden                              o --db
-          o --ignore-case                         o --json
-          o --in-album                            o --library
-          o --incloud                             o PHOTOS_LIBRARY
-          o --is-reference                  * osxphotos-places command line
-          o --keyword                         option
-          o --label                               o --db
-          o --live                                o --json
-          o --location                            o --library
-          o --max-size                            o PHOTOS_LIBRARY
-          o --min-size                      * osxphotos-query command line
-          o --missing                         option
-          o --name                                o --add-to-album
-          o --no-comment                          o --added-after
-          o --no-description                      o --added-before
-          o --no-keyword                          o --added-in-last
-          o --no-likes                            o --album
-          o --no-location                         o --burst
-          o --no-place                            o --cloudasset
-          o --no-title                            o --count
+          o --limit                               o --db
+          o --live                                o --library
+          o --load-config                         o UUID_OR_NAME
+          o --location                      * osxphotos-snap command line
+          o --max-size                        option
+          o --min-size                            o --db
+          o --missing                             o --library
+          o --name                          * osxphotos-sync command line
+          o --no-comment                      option
+          o --no-description                      o --added-after
+          o --no-keyword                          o --added-before
+          o --no-likes                            o --added-in-last
+          o --no-location                         o --album
+          o --no-place                            o --append
+          o --no-progress                         o --burst
+          o --no-title                            o --cloudasset
           o --not-burst                           o --db
-          o --not-cloudasset                      o --deleted
-          o --not-edited                          o --deleted-only
-          o --not-favorite                        o --description
-          o --not-hdr                             o --duplicate
-          o --not-hidden                          o --edited
-          o --not-in-album                        o --exif
+          o --not-cloudasset                      o --description
+          o --not-edited                          o --dry-run
+          o --not-favorite                        o --duplicate
+          o --not-hdr                             o --edited
+          o --not-hidden                          o --exif
+          o --not-in-album                        o --export
           o --not-incloud                         o --external-edit
           o --not-live                            o --favorite
-          o --not-missing                         o --field
-          o --not-panorama                        o --folder
-          o --not-portrait                        o --from-date
-          o --not-reference                       o --from-time
-          o --not-saved-to-library                o --has-comment
-          o --not-screenshot                      o --has-likes
-          o --not-selfie                          o --has-raw
-          o --not-shared                          o --hdr
-          o --not-slow-mo                         o --hidden
-          o --not-syndicated                      o --ignore-case
+          o --not-missing                         o --folder
+          o --not-panorama                        o --from-date
+          o --not-portrait                        o --from-time
+          o --not-reference                       o --has-comment
+          o --not-saved-to-library                o --has-likes
+          o --not-screenshot                      o --has-raw
+          o --not-selfie                          o --hdr
+          o --not-shared                          o --hidden
+          o --not-slow-mo                         o --ignore-case
+          o --not-syndicated                      o --import
           o --not-time-lapse                      o --in-album
           o --only-movies                         o --incloud
-          o --only-photos                         o --is-reference
-          o --panorama                            o --json
-          o --person                              o --keyword
-          o --place                               o --label
-          o --portrait                            o --library
-          o --query-eval                          o --live
-          o --query-function                      o --location
-          o --regex                               o --max-size
-          o --saved-to-library                    o --min-size
-          o --screenshot                          o --missing
-          o --selected                            o --name
-          o --selfie                              o --no-comment
-          o --shared                              o --no-description
-          o --slow-mo                             o --no-keyword
-          o --syndicated                          o --no-likes
-          o --theme                               o --no-location
-          o --time-lapse                          o --no-place
-          o --timestamp                           o --no-title
-          o --title                               o --not-burst
-          o --to-date                             o --not-cloudasset
-          o --to-time                             o --not-edited
-          o --uti                                 o --not-favorite
-          o --uuid                                o --not-hdr
-          o --uuid-from-file                      o --not-hidden
-          o --verbose                             o --not-in-album
-          o --window                              o --not-incloud
-          o --year                                o --not-live
-          o -i                                    o --not-missing
-          o -V                                    o --not-panorama
-          o -w                                    o --not-portrait
-    * osxphotos-albums command line               o --not-reference
-      option                                      o --not-saved-to-library
-          o --db                                  o --not-screenshot
-          o --json                                o --not-selfie
-          o --library                             o --not-shared
-          o PHOTOS_LIBRARY                        o --not-slow-mo
-    * osxphotos-batch-edit command line           o --not-syndicated
-      option                                      o --not-time-lapse
-          o --db                                  o --only-movies
-          o --description                         o --only-photos
-          o --dry-run                             o --panorama
-          o --keyword                             o --person
-          o --library                             o --place
-          o --location                            o --portrait
-          o --replace-keywords                    o --print
-          o --theme                               o --query-eval
-          o --timestamp                           o --query-function
-          o --title                               o --quiet
-          o --undo                                o --regex
-          o --verbose                             o --saved-to-library
-          o -V                                    o --screenshot
-    * osxphotos-diff command line                 o --selected
-      option                                      o --selfie
-          o --db                                  o --shared
-          o --library                             o --slow-mo
-          o --raw-output                          o --syndicated
-          o --style                               o --time-lapse
-          o --timestamp                           o --title
-          o --verbose                             o --to-date
-          o -r                                    o --to-time
-          o -s                                    o --uti
-          o -V                                    o --uuid
-          o DB2                                   o --uuid-from-file
-    * osxphotos-dump command line                 o --year
-      option                                      o -f
-          o --db                                  o -i
-          o --deleted                             o PHOTOS_LIBRARY
-          o --deleted-only                  * osxphotos-repl command line
-          o --field                           option
-          o --json                                o --added-after
-          o --library                             o --added-before
-          o --print                               o --added-in-last
-          o -f                                    o --album
-          o PHOTOS_LIBRARY                        o --burst
-    * osxphotos-exiftool command line             o --cloudasset
-      option                                      o --db
-          o --album-keyword                       o --deleted
-          o --append                              o --deleted-only
-          o --db                                  o --description
-          o --db-config                           o --duplicate
-          o --description-template                o --edited
-          o --dry-run                             o --emacs
-          o --exiftool-merge-keywords             o --exif
-          o --exiftool-merge-persons              o --external-edit
-          o --exiftool-option                     o --favorite
-          o --exiftool-path                       o --folder
-          o --exportdb                            o --from-date
-          o --ignore-date-modified                o --from-time
-          o --keyword-template                    o --has-comment
-          o --library                             o --has-likes
-          o --load-config                         o --has-raw
-          o --person-keyword                      o --hdr
-          o --replace-keywords                    o --hidden
-          o --report                              o --ignore-case
-          o --save-config                         o --in-album
-          o --theme                               o --incloud
-          o --timestamp                           o --is-reference
-          o --verbose                             o --keyword
-          o -V                                    o --label
-          o EXPORT_DIRECTORY                      o --library
-    * osxphotos-export command line               o --live
-      option                                      o --location
-          o --add-exported-to-album               o --max-size
-          o --add-missing-to-album                o --min-size
-          o --add-skipped-to-album                o --missing
-          o --added-after                         o --name
-          o --added-before                        o --no-comment
-          o --added-in-last                       o --no-description
-          o --album                               o --no-keyword
-          o --album-keyword                       o --no-likes
-          o --alt-copy                            o --no-location
-          o --append                              o --no-place
-          o --burst                               o --no-title
-          o --cleanup                             o --not-burst
-          o --cloudasset                          o --not-cloudasset
-          o --config-only                         o --not-edited
-          o --convert-to-jpeg                     o --not-favorite
-          o --current-name                        o --not-hdr
-          o --db                                  o --not-hidden
-          o --deleted                             o --not-in-album
-          o --deleted-only                        o --not-incloud
-          o --description                         o --not-live
-          o --description-template                o --not-missing
-          o --directory                           o --not-panorama
-          o --download-missing                    o --not-portrait
-          o --dry-run                             o --not-reference
-          o --duplicate                           o --not-saved-to-library
-          o --edited                              o --not-screenshot
-          o --edited-suffix                       o --not-selfie
-          o --exif                                o --not-shared
-          o --exiftool                            o --not-slow-mo
-          o --exiftool-merge-keywords             o --not-syndicated
-          o --exiftool-merge-persons              o --not-time-lapse
-          o --exiftool-option                     o --only-movies
-          o --exiftool-path                       o --only-photos
-          o --export-as-hardlink                  o --panorama
-          o --export-by-date                      o --person
-          o --exportdb                            o --place
-          o --external-edit                       o --portrait
-          o --favorite                            o --query-eval
-          o --favorite-rating                     o --query-function
-          o --filename                            o --regex
-          o --finder-tag-keywords                 o --saved-to-library
-          o --finder-tag-template                 o --screenshot
-          o --folder                              o --selected
-          o --force-update                        o --selfie
-          o --from-date                           o --shared
-          o --from-time                           o --slow-mo
-          o --has-comment                         o --syndicated
-          o --has-likes                           o --time-lapse
-          o --has-raw                             o --title
-          o --hdr                                 o --to-date
-          o --hidden                              o --to-time
-          o --ignore-case                         o --uti
-          o --ignore-date-modified                o --uuid
-          o --ignore-signature                    o --uuid-from-file
-          o --in-album                            o --year
-          o --incloud                             o -i
-          o --is-reference                  * osxphotos-run command line option
-          o --jpeg-ext                            o --help
-          o --jpeg-quality                        o -h
-          o --keep                                o ARGS
-          o --keyword                             o PYTHON_FILE
-          o --keyword-template              * osxphotos-show command line
-          o --label                           option
-          o --library                             o --db
-          o --limit                               o --library
-          o --live                                o UUID_OR_NAME
-          o --load-config                   * osxphotos-snap command line
-          o --location                        option
-          o --max-size                            o --db
-          o --min-size                            o --library
-          o --missing                       * osxphotos-sync command line
-          o --name                            option
-          o --no-comment                          o --added-after
-          o --no-description                      o --added-before
-          o --no-keyword                          o --added-in-last
-          o --no-likes                            o --album
-          o --no-location                         o --append
-          o --no-place                            o --burst
-          o --no-progress                         o --cloudasset
-          o --no-title                            o --db
-          o --not-burst                           o --description
-          o --not-cloudasset                      o --dry-run
-          o --not-edited                          o --duplicate
-          o --not-favorite                        o --edited
-          o --not-hdr                             o --exif
-          o --not-hidden                          o --export
-          o --not-in-album                        o --external-edit
-          o --not-incloud                         o --favorite
-          o --not-live                            o --folder
-          o --not-missing                         o --from-date
-          o --not-panorama                        o --from-time
-          o --not-portrait                        o --has-comment
-          o --not-reference                       o --has-likes
-          o --not-saved-to-library                o --has-raw
-          o --not-screenshot                      o --hdr
-          o --not-selfie                          o --hidden
-          o --not-shared                          o --ignore-case
-          o --not-slow-mo                         o --import
-          o --not-syndicated                      o --in-album
-          o --not-time-lapse                      o --incloud
-          o --only-movies                         o --is-reference
-          o --only-new                            o --keyword
-          o --only-photos                         o --label
-          o --original-suffix                     o --library
-          o --overwrite                           o --live
-          o --panorama                            o --location
-          o --person                              o --max-size
-          o --person-keyword                      o --merge
-          o --place                               o --min-size
-          o --portrait                            o --missing
-          o --post-command                        o --name
-          o --post-function                       o --no-comment
-          o --preview                             o --no-description
-          o --preview-if-missing                  o --no-keyword
-          o --preview-suffix                      o --no-likes
-          o --print                               o --no-location
-          o --query-eval                          o --no-place
-          o --query-function                      o --no-title
-          o --ramdb                               o --not-burst
-          o --regex                               o --not-cloudasset
-          o --replace-keywords                    o --not-edited
-          o --report                              o --not-favorite
-          o --retry                               o --not-hdr
-          o --save-config                         o --not-hidden
-          o --saved-to-library                    o --not-in-album
-          o --screenshot                          o --not-incloud
-          o --selected                            o --not-live
-          o --selfie                              o --not-missing
-          o --shared                              o --not-panorama
-          o --sidecar                             o --not-portrait
-          o --sidecar-drop-ext                    o --not-reference
-          o --skip-bursts                         o --not-saved-to-library
-          o --skip-edited                         o --not-screenshot
-          o --skip-live                           o --not-selfie
-          o --skip-original-if-edited             o --not-slow-mo
-          o --skip-raw                            o --not-syndicated
-          o --skip-uuid                           o --not-time-lapse
-          o --skip-uuid-from-file                 o --only-movies
-          o --slow-mo                             o --only-photos
-          o --strip                               o --panorama
-          o --syndicated                          o --person
-          o --theme                               o --place
-          o --time-lapse                          o --portrait
-          o --timestamp                           o --query-eval
-          o --title                               o --query-function
-          o --tmpdir                              o --regex
-          o --to-date                             o --report
-          o --to-time                             o --saved-to-library
-          o --touch-file                          o --screenshot
-          o --update                              o --selected
-          o --update-errors                       o --selfie
-          o --use-photokit                        o --set
-          o --use-photos-export                   o --slow-mo
-          o --uti                                 o --syndicated
-          o --uuid                                o --theme
-          o --uuid-from-file                      o --time-lapse
-          o --verbose                             o --timestamp
-          o --xattr-template                      o --title
-          o --year                                o --to-date
-          o -i                                    o --to-time
-          o -V                                    o --unmatched
-          o DEST                                  o --uti
-          o PHOTOS_LIBRARY                        o --uuid
-    * osxphotos-exportdb command line             o --uuid-from-file
-      option                                      o --verbose
-          o --append                              o --year
-          o --check-signatures                    o -A
-          o --delete-file                         o -e
-          o --delete-uuid                         o -i, [1]
-          o --dry-run                             o -m
-          o --errors                              o -R
-          o --export-dir                          o -s
-          o --info                                o -U
-          o --last-errors                         o -V
-          o --last-run                      * osxphotos-theme command line
-          o --migrate                         option
-          o --migrate-photos-library              o --clone
-          o --report                              o --config
-          o --save-config                         o --default
-          o --sql                                 o --delete
-          o --theme                               o --edit
-          o --timestamp                           o --list
-          o --touch-file                          o --preview
-          o --update-signatures             * osxphotos-timewarp command line
-          o --uuid-files                      option
-          o --uuid-info                           o --add-to-album
-          o --vacuum                              o --compare-exif
-          o --verbose                             o --date
-          o --version                             o --date-added
-          o -V                                    o --date-added-from-photo
-          o EXPORT_DATABASE                       o --date-delta
-    * osxphotos-help command line                 o --exiftool-path
-      option                                      o --force
-          o SUBTOPIC                              o --function
-          o TOPIC                                 o --inspect
-    * osxphotos-import command line               o --library
-      option                                      o --match-time
-          o --album                               o --parse-date
-          o --append                              o --plain
-          o --check-templates                     o --pull-exif
-          o --clear-location                      o --push-exif
-          o --clear-metadata                      o --theme
-          o --description                         o --time
-          o --dup-check                           o --time-delta
-          o --exiftool                            o --timestamp, [1]
-          o --exiftool-path                       o --timezone
-          o --glob                                o --use-file-time
-          o --keyword                             o --verbose
-          o --location                            o -a
-          o --merge-keywords                      o -c
-          o --no-progress                         o -d
-          o --parse-date                          o -D
-          o --post-function                       o -e
-          o --relative-to                         o -F
-          o --report                              o -f
-          o --resume                              o -i
-          o --split-folder                        o -L
-          o --theme                               o -M
-          o --timestamp                           o -m
-          o --title                               o -p
-          o --verbose                             o -P
-          o --walk                                o -t
-          o -a                                    o -T
-          o -C                                    o -V
-          o -d                                    o -z
-          o -D                              * osxphotos-tutorial command line
-          o -e                                option
-          o -f                                    o WIDTH
-          o -g                              * osxphotos-uninstall command line
-          o -k                                option
-          o -l                                    o --yes
-          o -L                                    o -y
-          o -m                                    o PACKAGES
-          o -P                              * osxphotos-uuid command line
-          o -p                                option
-          o -r                                    o --filename
-          o -R                                    o -f
-          o -t                              * osxphotos-version command line
-          o -V                                option
-          o -w                                    o --run
-          o FILES                           * overwrite_
-                                              (osxphotos.ExportOptions
-                                              attribute)
-                                            * owner_(osxphotos.PhotoInfo
-                                              property)
+          o --only-new                            o --is-reference
+          o --only-photos                         o --keyword
+          o --original-suffix                     o --label
+          o --overwrite                           o --library
+          o --panorama                            o --live
+          o --person                              o --location
+          o --person-keyword                      o --max-size
+          o --place                               o --merge
+          o --portrait                            o --min-size
+          o --post-command                        o --missing
+          o --post-function                       o --name
+          o --preview                             o --no-comment
+          o --preview-if-missing                  o --no-description
+          o --preview-suffix                      o --no-keyword
+          o --print                               o --no-likes
+          o --query-eval                          o --no-location
+          o --query-function                      o --no-place
+          o --ramdb                               o --no-title
+          o --regex                               o --not-burst
+          o --replace-keywords                    o --not-cloudasset
+          o --report                              o --not-edited
+          o --retry                               o --not-favorite
+          o --save-config                         o --not-hdr
+          o --saved-to-library                    o --not-hidden
+          o --screenshot                          o --not-in-album
+          o --selected                            o --not-incloud
+          o --selfie                              o --not-live
+          o --shared                              o --not-missing
+          o --sidecar                             o --not-panorama
+          o --sidecar-drop-ext                    o --not-portrait
+          o --skip-bursts                         o --not-reference
+          o --skip-edited                         o --not-saved-to-library
+          o --skip-live                           o --not-screenshot
+          o --skip-original-if-edited             o --not-selfie
+          o --skip-raw                            o --not-slow-mo
+          o --skip-uuid                           o --not-syndicated
+          o --skip-uuid-from-file                 o --not-time-lapse
+          o --slow-mo                             o --only-movies
+          o --strip                               o --only-photos
+          o --syndicated                          o --panorama
+          o --theme                               o --person
+          o --time-lapse                          o --place
+          o --timestamp                           o --portrait
+          o --title                               o --query-eval
+          o --tmpdir                              o --query-function
+          o --to-date                             o --regex
+          o --to-time                             o --report
+          o --touch-file                          o --saved-to-library
+          o --update                              o --screenshot
+          o --update-errors                       o --selected
+          o --use-photokit                        o --selfie
+          o --use-photos-export                   o --set
+          o --uti                                 o --slow-mo
+          o --uuid                                o --syndicated
+          o --uuid-from-file                      o --theme
+          o --verbose                             o --time-lapse
+          o --xattr-template                      o --timestamp
+          o --year                                o --title
+          o -i                                    o --to-date
+          o -V                                    o --to-time
+          o DEST                                  o --unmatched
+          o PHOTOS_LIBRARY                        o --uti
+    * osxphotos-exportdb command line             o --uuid
+      option                                      o --uuid-from-file
+          o --append                              o --verbose
+          o --check-signatures                    o --year
+          o --delete-file                         o -A
+          o --delete-uuid                         o -e
+          o --dry-run                             o -i, [1]
+          o --errors                              o -m
+          o --export-dir                          o -R
+          o --info                                o -s
+          o --last-errors                         o -U
+          o --last-run                            o -V
+          o --migrate                       * osxphotos-theme command line
+          o --migrate-photos-library          option
+          o --report                              o --clone
+          o --save-config                         o --config
+          o --sql                                 o --default
+          o --theme                               o --delete
+          o --timestamp                           o --edit
+          o --touch-file                          o --list
+          o --update-signatures                   o --preview
+          o --uuid-files                    * osxphotos-timewarp command line
+          o --uuid-info                       option
+          o --vacuum                              o --add-to-album
+          o --verbose                             o --compare-exif
+          o --version                             o --date
+          o -V                                    o --date-added
+          o EXPORT_DATABASE                       o --date-added-from-photo
+    * osxphotos-help command line                 o --date-delta
+      option                                      o --exiftool-path
+          o SUBTOPIC                              o --force
+          o TOPIC                                 o --function
+    * osxphotos-import command line               o --inspect
+      option                                      o --library
+          o --album                               o --match-time
+          o --append                              o --parse-date
+          o --check-templates                     o --plain
+          o --clear-location                      o --pull-exif
+          o --clear-metadata                      o --push-exif
+          o --description                         o --theme
+          o --dup-check                           o --time
+          o --exiftool                            o --time-delta
+          o --exiftool-path                       o --timestamp, [1]
+          o --glob                                o --timezone
+          o --keyword                             o --use-file-time
+          o --location                            o --verbose
+          o --merge-keywords                      o -a
+          o --no-progress                         o -c
+          o --parse-date                          o -d
+          o --post-function                       o -D
+          o --relative-to                         o -e
+          o --report                              o -F
+          o --resume                              o -f
+          o --split-folder                        o -i
+          o --theme                               o -L
+          o --timestamp                           o -M
+          o --title                               o -m
+          o --verbose                             o -p
+          o --walk                                o -P
+          o -a                                    o -t
+          o -C                                    o -T
+          o -d                                    o -V
+          o -D                                    o -z
+          o -e                              * osxphotos-tutorial command line
+          o -f                                option
+          o -g                                    o WIDTH
+          o -k                              * osxphotos-uninstall command line
+          o -l                                option
+          o -L                                    o --yes
+          o -m                                    o -y
+          o -P                                    o PACKAGES
+          o -p                              * osxphotos-uuid command line
+          o -r                                option
+          o -R                                    o --filename
+          o -t                                    o -f
+          o -V                              * osxphotos-version command line
+          o -w                                option
+          o FILES                                 o --run
+    * osxphotos-info command line           * overwrite_
+      option                                  (osxphotos.ExportOptions
+          o --db                              attribute)
+          o --json                          * owner_(osxphotos.PhotoInfo
+          o --library                         property)
+          o PHOTOS_LIBRARY
 
 ***** P *****
-    * PACKAGES
-          o osxphotos-install_command       * photos_by_uuid()_
-            line_option                       (osxphotos.PhotosDB_method)
-          o osxphotos-uninstall_command     * PHOTOS_LIBRARY
-            line_option                           o osxphotos-albums_command
-    * panorama_(osxphotos.PhotoInfo                 line_option
-      property)                                   o osxphotos-dump_command_line
-          o (osxphotos.QueryOptions                 option
-            attribute)                            o osxphotos-export_command
-    * parent_(osxphotos.AlbumInfo                   line_option
-      property)                                   o osxphotos-info_command_line
-          o (osxphotos.FolderInfo                   option
-            property)                             o osxphotos-keywords_command
-    * path_(osxphotos.ExportDB                      line_option
-      property)                                   o osxphotos-labels_command
-          o (osxphotos.PhotoInfo                    line_option
-            property)                             o osxphotos-persons_command
-    * path_derivatives_                             line_option
-      (osxphotos.PhotoInfo_property)              o osxphotos-places_command
-    * path_edited_(osxphotos.PhotoInfo              line_option
-      property)                                   o osxphotos-query_command
-    * path_edited_live_photo_                       line_option
-      (osxphotos.PhotoInfo_property)        * photos_version_
-    * path_live_photo_                        (osxphotos.PhotosDB_property)
-      (osxphotos.PhotoInfo_property)        * PhotosAlbum_(class_in_osxphotos)
-    * path_raw_(osxphotos.PhotoInfo         * PhotosAlbumPhotoScript_(class_in
+    * PACKAGES                              * photos()_(osxphotos.PhotosDB
+          o osxphotos-install_command         method)
+            line_option                     * photos_by_uuid()_
+          o osxphotos-uninstall_command       (osxphotos.PhotosDB_method)
+            line_option                     * PHOTOS_LIBRARY
+    * panorama_(osxphotos.PhotoInfo               o osxphotos-albums_command
+      property)                                     line_option
+          o (osxphotos.QueryOptions               o osxphotos-dump_command_line
+            attribute)                              option
+    * parent_(osxphotos.AlbumInfo                 o osxphotos-export_command
+      property)                                     line_option
+          o (osxphotos.FolderInfo                 o osxphotos-info_command_line
+            property)                               option
+    * path_(osxphotos.ExportDB                    o osxphotos-keywords_command
+      property)                                     line_option
+          o (osxphotos.PhotoInfo                  o osxphotos-labels_command
+            property)                               line_option
+    * path_derivatives_                           o osxphotos-persons_command
+      (osxphotos.PhotoInfo_property)                line_option
+    * path_edited_(osxphotos.PhotoInfo            o osxphotos-places_command
+      property)                                     line_option
+    * path_edited_live_photo_                     o osxphotos-query_command
+      (osxphotos.PhotoInfo_property)                line_option
+    * path_live_photo_                      * photos_version_
+      (osxphotos.PhotoInfo_property)          (osxphotos.PhotosDB_property)
+    * path_raw_(osxphotos.PhotoInfo         * PhotosAlbum_(class_in_osxphotos)
+      property)                             * PhotosAlbumPhotoScript_(class_in
+    * person_(osxphotos.QueryOptions          osxphotos)
+      attribute)                            * PhotosDB_(class_in_osxphotos)
+    * person_info_(osxphotos.FaceInfo       * PhotoTemplate_(class_in
       property)                               osxphotos)
-    * person_(osxphotos.QueryOptions        * PhotosDB_(class_in_osxphotos)
-      attribute)                            * PhotoTemplate_(class_in
-    * person_info_(osxphotos.PhotoInfo        osxphotos)
-      property)                             * pid_(osxphotos.ExifTool_property)
-          o (osxphotos.PhotosDB             * pk_(osxphotos.MomentInfo
-            property)                         property)
-    * PersonInfo_(class_in_osxphotos)       * place_(osxphotos.PhotoInfo
-    * persons_(osxphotos.ExportOptions        property)
-      attribute)                                  o (osxphotos.QueryOptions
-          o (osxphotos.PhotoInfo                    attribute)
-            property)                       * place_names_(osxphotos.SearchInfo
+          o (osxphotos.PhotoInfo            * pid_(osxphotos.ExifTool_property)
+            property)                       * pitch_(osxphotos.FaceInfo
           o (osxphotos.PhotosDB               property)
-            property)                       * PlaceInfo_(class_in_osxphotos)
-    * persons_as_dict_                      * portrait_(osxphotos.PhotoInfo
-      (osxphotos.PhotosDB_property)           property)
-    * photo_index()_                              o (osxphotos.QueryOptions
-      (osxphotos.AlbumInfo_method)                  attribute)
-    * PhotoExporter_(class_in               * preview_(osxphotos.ExportOptions
-      osxphotos)                              attribute)
-    * PhotoInfo_(class_in_osxphotos)        * preview_suffix_
-    * photos_(osxphotos.AlbumInfo             (osxphotos.ExportOptions
-      property)                               attribute)
-          o (osxphotos.ImportInfo           * project_info_(osxphotos.PhotoInfo
+            property)                       * pk_(osxphotos.MomentInfo
+    * PersonInfo_(class_in_osxphotos)         property)
+    * persons_(osxphotos.ExportOptions      * place_(osxphotos.PhotoInfo
+      attribute)                              property)
+          o (osxphotos.PhotoInfo                  o (osxphotos.QueryOptions
+            property)                               attribute)
+          o (osxphotos.PhotosDB             * place_names_(osxphotos.SearchInfo
             property)                         property)
-          o (osxphotos.MomentInfo                 o (osxphotos.PhotosDB
-            property)                               property)
-          o (osxphotos.PersonInfo           * ProjectInfo_(class_in_osxphotos)
-            property)                       * PYTHON_FILE
-          o (osxphotos.QueryOptions               o osxphotos-run_command_line
-            attribute)                              option
-    * photos()_(osxphotos.PhotosDB
-      method)
+    * persons_as_dict_                      * PlaceInfo_(class_in_osxphotos)
+      (osxphotos.PhotosDB_property)         * portrait_(osxphotos.PhotoInfo
+    * photo_(osxphotos.FaceInfo               property)
+      property)                                   o (osxphotos.QueryOptions
+    * photo_index()_                                attribute)
+      (osxphotos.AlbumInfo_method)          * preview_(osxphotos.ExportOptions
+    * PhotoExporter_(class_in                 attribute)
+      osxphotos)                            * preview_suffix_
+    * PhotoInfo_(class_in_osxphotos)          (osxphotos.ExportOptions
+    * photos_(osxphotos.AlbumInfo             attribute)
+      property)                             * project_info_(osxphotos.PhotoInfo
+          o (osxphotos.ImportInfo             property)
+            property)                             o (osxphotos.PhotosDB
+          o (osxphotos.MomentInfo                   property)
+            property)                       * ProjectInfo_(class_in_osxphotos)
+          o (osxphotos.PersonInfo           * PYTHON_FILE
+            property)                             o osxphotos-run_command_line
+          o (osxphotos.QueryOptions                 option
+            attribute)
 
 ***** Q *****
     * query()_(osxphotos.PhotosDB     * query_eval_(osxphotos.QueryOptions
       method)                           attribute)
                                       * QueryOptions_(class_in_osxphotos)
 
 ***** R *****
-                                            * render_options_
-    * raw_original_(osxphotos.PhotoInfo       (osxphotos.ExportOptions
-      property)                               attribute)
-    * raw_photo_                            * render_template()_
-      (osxphotos.ExportOptions                (osxphotos.PhotoInfo_method)
-      attribute)                            * replace_keywords_
-    * regex_(osxphotos.QueryOptions           (osxphotos.ExportOptions
+    * raw_original_(osxphotos.PhotoInfo     * render_template()_
+      property)                               (osxphotos.PhotoInfo_method)
+    * raw_photo_                            * replace_keywords_
+      (osxphotos.ExportOptions                (osxphotos.ExportOptions
       attribute)                              attribute)
-    * rename()_(osxphotos.FileUtilNoOp      * rich_(osxphotos.ExportOptions
-      class_method)                           attribute)
-    * render()_(osxphotos.PhotoTemplate     * rmdir()_(osxphotos.FileUtilNoOp
-      method)                                 class_method)
-                                            * run_commands()_
+    * regex_(osxphotos.QueryOptions         * rich_(osxphotos.ExportOptions
+      attribute)                              attribute)
+    * rename()_(osxphotos.FileUtilNoOp      * rmdir()_(osxphotos.FileUtilNoOp
+      class_method)                           class_method)
+    * render()_(osxphotos.PhotoTemplate     * roll_(osxphotos.FaceInfo
+      method)                                 property)
+    * render_options_                       * roll_pitch_yaw()_
+      (osxphotos.ExportOptions                (osxphotos.FaceInfo_method)
+      attribute)                            * run_commands()_
                                               (osxphotos.ExifTool_method)
 
 ***** S *****
     * saved_to_library_                     * sidecar_(osxphotos.ExportOptions
       (osxphotos.PhotoInfo_property)          attribute)
           o (osxphotos.QueryOptions         * sidecar_drop_ext_
             attribute)                        (osxphotos.ExportOptions
     * score_(osxphotos.PhotoInfo              attribute)
-      property)                             * slow_mo_(osxphotos.PhotoInfo
+      property)                             * size_pixels_(osxphotos.FaceInfo
     * ScoreInfo_(class_in_osxphotos)          property)
-    * screenshot_(osxphotos.PhotoInfo             o (osxphotos.QueryOptions
-      property)                                     attribute)
-          o (osxphotos.QueryOptions         * sort_order_(osxphotos.AlbumInfo
-            attribute)                        property)
-    * search_info_(osxphotos.PhotoInfo            o (osxphotos.PersonInfo
-      property)                                     property)
-    * search_info_normalized_               * source_(osxphotos.SearchInfo
-      (osxphotos.PhotoInfo_property)          property)
-    * SearchInfo_(class_in_osxphotos)       * start_date_(osxphotos.MomentInfo
+    * screenshot_(osxphotos.PhotoInfo       * slow_mo_(osxphotos.PhotoInfo
+      property)                               property)
+          o (osxphotos.QueryOptions               o (osxphotos.QueryOptions
+            attribute)                              attribute)
+    * search_info_(osxphotos.PhotoInfo      * sort_order_(osxphotos.AlbumInfo
+      property)                               property)
+    * search_info_normalized_                     o (osxphotos.PersonInfo
+      (osxphotos.PhotoInfo_property)                property)
+    * SearchInfo_(class_in_osxphotos)       * source_(osxphotos.SearchInfo
     * season_(osxphotos.SearchInfo            property)
-      property)                             * state_(osxphotos.SearchInfo
+      property)                             * start_date_(osxphotos.MomentInfo
     * selected_(osxphotos.QueryOptions        property)
-      attribute)                            * state_abbreviation_
-    * selfie_(osxphotos.PhotoInfo             (osxphotos.SearchInfo_property)
-      property)                             * streets_(osxphotos.SearchInfo
-          o (osxphotos.QueryOptions           property)
-            attribute)                      * strip_(osxphotos.ExportOptions
-    * set_config()_(osxphotos.ExportDB        attribute)
-      method)                               * subfolders_(osxphotos.FolderInfo
-    * set_debug()_(in_module_osxphotos)       property)
-    * set_export_results()_                 * subtitle_(osxphotos.MomentInfo
+      attribute)                            * state_(osxphotos.SearchInfo
+    * selfie_(osxphotos.PhotoInfo             property)
+      property)                             * state_abbreviation_
+          o (osxphotos.QueryOptions           (osxphotos.SearchInfo_property)
+            attribute)                      * streets_(osxphotos.SearchInfo
+    * set_config()_(osxphotos.ExportDB        property)
+      method)                               * strip_(osxphotos.ExportOptions
+    * set_debug()_(in_module_osxphotos)       attribute)
+    * set_export_results()_                 * subfolders_(osxphotos.FolderInfo
       (osxphotos.ExportDB_method)             property)
-    * set_photoinfo_for_uuid()_             * SUBTOPIC
-      (osxphotos.ExportDB_method)                 o osxphotos-help_command_line
-    * setvalue()_(osxphotos.ExifTool                option
-      method)                               * syndicated_(osxphotos.PhotoInfo
-    * shared_(osxphotos.PhotoInfo             property)
-      property)                                   o (osxphotos.QueryOptions
-          o (osxphotos.QueryOptions                 attribute)
-            attribute)
+    * set_photoinfo_for_uuid()_             * subtitle_(osxphotos.MomentInfo
+      (osxphotos.ExportDB_method)             property)
+    * setvalue()_(osxphotos.ExifTool        * SUBTOPIC
+      method)                                     o osxphotos-help_command_line
+    * shared_(osxphotos.PhotoInfo                   option
+      property)                             * syndicated_(osxphotos.PhotoInfo
+          o (osxphotos.QueryOptions           property)
+            attribute)                            o (osxphotos.QueryOptions
+                                                    attribute)
 
 ***** T *****
     * tables()_(osxphotos.PhotoInfo
       method)
     * text_found_(osxphotos.SearchInfo
       property)
     * time_lapse_(osxphotos.PhotoInfo      * tmpdir_(osxphotos.ExportOptions
@@ -1878,13 +1884,15 @@
 ***** W *****
     * WIDTH                                * width_(osxphotos.PhotoInfo
           o osxphotos-tutorial_command       property)
             line_option                    * write_exiftool_metadata_to_file()_
                                              (osxphotos.PhotoExporter_method)
 
 ***** Y *****
-    * year_(osxphotos.QueryOptions_attribute)
-          o (osxphotos.SearchInfo_property)
+                                            * year_(osxphotos.QueryOptions
+    * yaw_(osxphotos.FaceInfo_property)       attribute)
+                                                  o (osxphotos.SearchInfo
+                                                    property)
 
 Copyright © 2021, Rhet Turnbull
 Made with Sphinx and @pradyunsg's Furo
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.5 documentation</title>
+        <title>osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -380,14 +380,30 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ExportResults"><code class="docutils literal notranslate"><span class="pre">ExportResults</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportResults.all_files"><code class="docutils literal notranslate"><span class="pre">ExportResults.all_files()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportResults.attributes"><code class="docutils literal notranslate"><span class="pre">ExportResults.attributes</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportResults.datetime"><code class="docutils literal notranslate"><span class="pre">ExportResults.datetime</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.FaceInfo"><code class="docutils literal notranslate"><span class="pre">FaceInfo</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.asdict"><code class="docutils literal notranslate"><span class="pre">FaceInfo.asdict()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.center"><code class="docutils literal notranslate"><span class="pre">FaceInfo.center</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.face_rect"><code class="docutils literal notranslate"><span class="pre">FaceInfo.face_rect()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.json"><code class="docutils literal notranslate"><span class="pre">FaceInfo.json()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.mpri_reg_rect"><code class="docutils literal notranslate"><span class="pre">FaceInfo.mpri_reg_rect</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.mwg_rs_area"><code class="docutils literal notranslate"><span class="pre">FaceInfo.mwg_rs_area</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.person_info"><code class="docutils literal notranslate"><span class="pre">FaceInfo.person_info</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.photo"><code class="docutils literal notranslate"><span class="pre">FaceInfo.photo</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.pitch"><code class="docutils literal notranslate"><span class="pre">FaceInfo.pitch</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.roll"><code class="docutils literal notranslate"><span class="pre">FaceInfo.roll</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.roll_pitch_yaw"><code class="docutils literal notranslate"><span class="pre">FaceInfo.roll_pitch_yaw()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.size_pixels"><code class="docutils literal notranslate"><span class="pre">FaceInfo.size_pixels</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FaceInfo.yaw"><code class="docutils literal notranslate"><span class="pre">FaceInfo.yaw</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.FileUtil"><code class="docutils literal notranslate"><span class="pre">FileUtil</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp.convert_to_jpeg"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.convert_to_jpeg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp.copy"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.copy()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp.file_sig"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.file_sig()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp.hardlink"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.hardlink()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.FileUtilNoOp.rename"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.rename()</span></code></a></li>
@@ -588,15 +604,23 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.photos"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.photos_by_uuid"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_by_uuid()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.photos_version"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_version</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
-<li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.address"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.address_str"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address_str</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.country_code"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.country_code</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.ishome"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.ishome</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.name"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.name</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.names"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.names</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo.folder_list"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_list</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo.folder_names"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_names</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.QueryOptions"><code class="docutils literal notranslate"><span class="pre">QueryOptions</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.added_after"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_after</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -196,14 +196,28 @@
                 # ExportOptions.tmpdir
                 # ExportOptions.favorite_rating
                 # ExportOptions.bit_flags
           o ExportResults
                 # ExportResults.all_files()
                 # ExportResults.attributes
                 # ExportResults.datetime
+          o FaceInfo
+                # FaceInfo.asdict()
+                # FaceInfo.center
+                # FaceInfo.face_rect()
+                # FaceInfo.json()
+                # FaceInfo.mpri_reg_rect
+                # FaceInfo.mwg_rs_area
+                # FaceInfo.person_info
+                # FaceInfo.photo
+                # FaceInfo.pitch
+                # FaceInfo.roll
+                # FaceInfo.roll_pitch_yaw()
+                # FaceInfo.size_pixels
+                # FaceInfo.yaw
           o FileUtil
           o FileUtilNoOp
                 # FileUtilNoOp.convert_to_jpeg()
                 # FileUtilNoOp.copy()
                 # FileUtilNoOp.file_sig()
                 # FileUtilNoOp.hardlink()
                 # FileUtilNoOp.rename()
@@ -387,14 +401,20 @@
                 # PhotosDB.persons_as_dict
                 # PhotosDB.photos()
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
+                # PlaceInfo.address
+                # PlaceInfo.address_str
+                # PlaceInfo.country_code
+                # PlaceInfo.ishome
+                # PlaceInfo.name
+                # PlaceInfo.names
           o ProjectInfo
                 # ProjectInfo.folder_list
                 # ProjectInfo.folder_names
           o QueryOptions
                 # QueryOptions.added_after
                 # QueryOptions.added_before
                 # QueryOptions.added_in_last
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -91,14 +91,28 @@
 osxphotos.ExportOptions.use_photokit py:attribute 1 reference.html#$ -
 osxphotos.ExportOptions.use_photos_export py:attribute 1 reference.html#$ -
 osxphotos.ExportOptions.verbose py:attribute 1 reference.html#$ -
 osxphotos.ExportResults py:class 1 reference.html#$ -
 osxphotos.ExportResults.all_files py:method 1 reference.html#$ -
 osxphotos.ExportResults.attributes py:property 1 reference.html#$ -
 osxphotos.ExportResults.datetime py:property 1 reference.html#$ -
+osxphotos.FaceInfo py:class 1 reference.html#$ -
+osxphotos.FaceInfo.asdict py:method 1 reference.html#$ -
+osxphotos.FaceInfo.center py:property 1 reference.html#$ -
+osxphotos.FaceInfo.face_rect py:method 1 reference.html#$ -
+osxphotos.FaceInfo.json py:method 1 reference.html#$ -
+osxphotos.FaceInfo.mpri_reg_rect py:property 1 reference.html#$ -
+osxphotos.FaceInfo.mwg_rs_area py:property 1 reference.html#$ -
+osxphotos.FaceInfo.person_info py:property 1 reference.html#$ -
+osxphotos.FaceInfo.photo py:property 1 reference.html#$ -
+osxphotos.FaceInfo.pitch py:property 1 reference.html#$ -
+osxphotos.FaceInfo.roll py:property 1 reference.html#$ -
+osxphotos.FaceInfo.roll_pitch_yaw py:method 1 reference.html#$ -
+osxphotos.FaceInfo.size_pixels py:property 1 reference.html#$ -
+osxphotos.FaceInfo.yaw py:property 1 reference.html#$ -
 osxphotos.FileUtil py:class 1 reference.html#$ -
 osxphotos.FileUtilNoOp py:class 1 reference.html#$ -
 osxphotos.FileUtilNoOp.convert_to_jpeg py:method 1 reference.html#$ -
 osxphotos.FileUtilNoOp.copy py:method 1 reference.html#$ -
 osxphotos.FileUtilNoOp.file_sig py:method 1 reference.html#$ -
 osxphotos.FileUtilNoOp.hardlink py:method 1 reference.html#$ -
 osxphotos.FileUtilNoOp.rename py:method 1 reference.html#$ -
@@ -282,14 +296,20 @@
 osxphotos.PhotosDB.persons_as_dict py:property 1 reference.html#$ -
 osxphotos.PhotosDB.photos py:method 1 reference.html#$ -
 osxphotos.PhotosDB.photos_by_uuid py:method 1 reference.html#$ -
 osxphotos.PhotosDB.photos_version py:property 1 reference.html#$ -
 osxphotos.PhotosDB.project_info py:property 1 reference.html#$ -
 osxphotos.PhotosDB.query py:method 1 reference.html#$ -
 osxphotos.PlaceInfo py:class 1 reference.html#$ -
+osxphotos.PlaceInfo.address py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.address_str py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.country_code py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.ishome py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.name py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.names py:property 1 reference.html#$ -
 osxphotos.ProjectInfo py:class 1 reference.html#$ -
 osxphotos.ProjectInfo.folder_list py:property 1 reference.html#$ -
 osxphotos.ProjectInfo.folder_names py:property 1 reference.html#$ -
 osxphotos.QueryOptions py:class 1 reference.html#$ -
 osxphotos.QueryOptions.added_after py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.added_before py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.added_in_last py:attribute 1 reference.html#$ -
@@ -410,14 +430,15 @@
 osxphotos.exiftool.ExifTool py:class -1 reference.html#osxphotos.ExifTool -
 osxphotos.export_db.ExportDB py:class -1 reference.html#osxphotos.ExportDB -
 osxphotos.export_db.ExportDBTemp py:class -1 reference.html#osxphotos.ExportDBTemp -
 osxphotos.fileutil.FileUtil py:class -1 reference.html#osxphotos.FileUtil -
 osxphotos.fileutil.FileUtilNoOp py:class -1 reference.html#osxphotos.FileUtilNoOp -
 osxphotos.is_debug py:function 1 reference.html#$ -
 osxphotos.momentinfo.MomentInfo py:class -1 reference.html#osxphotos.MomentInfo -
+osxphotos.personinfo.FaceInfo py:class -1 reference.html#osxphotos.FaceInfo -
 osxphotos.personinfo.PersonInfo py:class -1 reference.html#osxphotos.PersonInfo -
 osxphotos.photoexporter.ExportOptions py:class -1 reference.html#osxphotos.ExportOptions -
 osxphotos.photoexporter.ExportResults py:class -1 reference.html#osxphotos.ExportResults -
 osxphotos.photoexporter.PhotoExporter py:class -1 reference.html#osxphotos.PhotoExporter -
 osxphotos.photoinfo.PhotoInfo py:class -1 reference.html#osxphotos.PhotoInfo -
 osxphotos.photosalbum.PhotosAlbum py:class -1 reference.html#osxphotos.PhotosAlbum -
 osxphotos.photosalbum.PhotosAlbumPhotoScript py:class -1 reference.html#osxphotos.PhotosAlbumPhotoScript -
@@ -1204,17 +1225,14 @@
 osxphotos-tutorial.WIDTH std:cmdoption 1 cli.html#cmdoption-osxphotos-tutorial-arg-WIDTH -
 osxphotos-uninstall.--yes std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
 osxphotos-uninstall.-y std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
 osxphotos-uninstall.PACKAGES std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-arg-PACKAGES -
 osxphotos-uuid.--filename std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
 osxphotos-uuid.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
 osxphotos-version.--run std:cmdoption 1 cli.html#cmdoption-osxphotos-version-run -
-osxphotos.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-library -
-osxphotos.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-json -
-osxphotos.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-library -
 osxphotos.--version std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
 osxphotos.-v std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
 overview std:doc -1 overview.html OSXPhotos
 package_overview std:doc -1 package_overview.html OSXPhotos Python Package Overview
 py-modindex std:label -1 py-modindex.html Python Module Index
 reference std:doc -1 reference.html OSXPhotos Python Reference
 search std:label -1 search.html Search Page
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.5 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.6 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1063,14 +1063,147 @@
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">datetime</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span></em><a class="headerlink" href="#osxphotos.ExportResults.datetime" title="Permalink to this definition">#</a></dt>
 <dd><p>Return datetime when ExportResults was created</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">FaceInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pk</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/personinfo.html#FaceInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FaceInfo" title="Permalink to this definition">#</a></dt>
+<dd><p>Info about a face in the Photos library</p>
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.asdict">
+<span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/personinfo.html#FaceInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FaceInfo.asdict" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns dict representation of class instance</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.center">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">center</span></span><a class="headerlink" href="#osxphotos.FaceInfo.center" title="Permalink to this definition">#</a></dt>
+<dd><p>Coordinates, in PIL format, for center of face</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>tuple of coordinates in form (x, y)</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.face_rect">
+<span class="sig-name descname"><span class="pre">face_rect</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/personinfo.html#FaceInfo.face_rect"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FaceInfo.face_rect" title="Permalink to this definition">#</a></dt>
+<dd><dl class="simple">
+<dt>Get face rectangle coordinates for current version of the associated image</dt><dd><p>If image has been edited, rectangle applies to edited version, otherwise original version
+Coordinates in format and reference frame used by PIL</p>
+</dd>
+</dl>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>list [(x0, x1), (y0, y1)] of coordinates in reference frame used by PIL</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.json">
+<span class="sig-name descname"><span class="pre">json</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/personinfo.html#FaceInfo.json"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FaceInfo.json" title="Permalink to this definition">#</a></dt>
+<dd><p>Return JSON representation of FaceInfo instance</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.mpri_reg_rect">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">mpri_reg_rect</span></span><a class="headerlink" href="#osxphotos.FaceInfo.mpri_reg_rect" title="Permalink to this definition">#</a></dt>
+<dd><p>Get coordinates for Microsoft Photo Region Rectangle.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>x = x coordinate of top left corner of rectangle
+y = y coordinate of top left corner of rectangle
+h = height of rectangle
+w = width of rectangle</p>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p>MPRI_Reg_Rect named tuple with x, y, h, w where</p>
+</dd>
+</dl>
+<dl class="simple">
+<dt>Reference:</dt><dd><p><a class="reference external" href="https://docs.microsoft.com/en-us/windows/win32/wic/-wic-people-tagging">https://docs.microsoft.com/en-us/windows/win32/wic/-wic-people-tagging</a></p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.mwg_rs_area">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">mwg_rs_area</span></span><a class="headerlink" href="#osxphotos.FaceInfo.mwg_rs_area" title="Permalink to this definition">#</a></dt>
+<dd><p>Get coordinates for Metadata Working Group Region Area.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>x = stArea:x
+y = stArea:y
+h = stArea:h
+w = stArea:w</p>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p>MWG_RS_Area named tuple with x, y, h, w where</p>
+</dd>
+</dl>
+<dl class="simple">
+<dt>Reference:</dt><dd><p><a class="reference external" href="https://photo.stackexchange.com/questions/106410/how-does-xmp-define-the-face-region">https://photo.stackexchange.com/questions/106410/how-does-xmp-define-the-face-region</a></p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.person_info">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">person_info</span></span><a class="headerlink" href="#osxphotos.FaceInfo.person_info" title="Permalink to this definition">#</a></dt>
+<dd><p>PersonInfo instance for person associated with this face</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.photo">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">photo</span></span><a class="headerlink" href="#osxphotos.FaceInfo.photo" title="Permalink to this definition">#</a></dt>
+<dd><p>PhotoInfo instance associated with this face</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.pitch">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">pitch</span></span><a class="headerlink" href="#osxphotos.FaceInfo.pitch" title="Permalink to this definition">#</a></dt>
+<dd><p>Return pitch angle in radians of the face region</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.roll">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">roll</span></span><a class="headerlink" href="#osxphotos.FaceInfo.roll" title="Permalink to this definition">#</a></dt>
+<dd><p>Return roll angle in radians of the face region</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.roll_pitch_yaw">
+<span class="sig-name descname"><span class="pre">roll_pitch_yaw</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/personinfo.html#FaceInfo.roll_pitch_yaw"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FaceInfo.roll_pitch_yaw" title="Permalink to this definition">#</a></dt>
+<dd><p>Roll, pitch, yaw of face in radians as tuple</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.size_pixels">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">size_pixels</span></span><a class="headerlink" href="#osxphotos.FaceInfo.size_pixels" title="Permalink to this definition">#</a></dt>
+<dd><p>Size of face in pixels (centered around center_x, center_y)</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>size, in int pixels, of a circle drawn around the center of the face</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.FaceInfo.yaw">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">yaw</span></span><a class="headerlink" href="#osxphotos.FaceInfo.yaw" title="Permalink to this definition">#</a></dt>
+<dd><p>Return yaw angle in radians of the face region</p>
+</dd></dl>
+
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.FileUtil">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">FileUtil</span></span><a class="reference internal" href="_modules/osxphotos/fileutil.html#FileUtil"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.FileUtil" title="Permalink to this definition">#</a></dt>
 <dd><p>Various file utilities</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.FileUtilNoOp">
@@ -2615,15 +2748,101 @@
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.PlaceInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">PlaceInfo</span></span><a class="reference internal" href="_modules/osxphotos/placeinfo.html#PlaceInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PlaceInfo" title="Permalink to this definition">#</a></dt>
-<dd></dd></dl>
+<dd><p>Reverse geolocation place info for a photo.</p>
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.address">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">address</span></span><a class="headerlink" href="#osxphotos.PlaceInfo.address" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns a <cite>PostalAddress</cite> namedtuple with details of the postal address containing the following fields:</p>
+<ul class="simple">
+<li><p><cite>city</cite></p></li>
+<li><p><cite>country</cite></p></li>
+<li><p><cite>postal_code</cite></p></li>
+<li><p><cite>state</cite></p></li>
+<li><p><cite>street</cite></p></li>
+<li><p><cite>sub_administrative_area</cite></p></li>
+<li><p><cite>sub_locality</cite></p></li>
+<li><p><cite>iso_country_code</cite></p></li>
+</ul>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.address_str">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">address_str</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.address_str" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns the full postal address as a string if defined, otherwise <cite>None</cite>.</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.country_code">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">country_code</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.country_code" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns the country_code of place, for example “GB”.
+Returns <cite>None</cite> if PhotoInfo contains no country code.</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.ishome">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">ishome</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.ishome" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns <cite>True</cite> if photo place is user’s home address, otherwise <cite>False</cite>.</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.name">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">name</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.name" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns the name of the local place as str.
+This is what Photos displays in the Info window.
+<strong>Note</strong> Photos 5 uses a different algorithm to determine the name than earlier versions which means the same Photo may have a different place name in Photos 4 and Photos 5.
+<cite>PhotoInfo.name</cite> will return the name Photos would have shown depending on the version of the library being processed.
+Returns <cite>None</cite> if photo does not contain a name.</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.names">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">names</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">osxphotos.placeinfo.PlaceNames</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.names" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns a <cite>PlaceNames</cite> namedtuple with the following fields.
+Each field is a list with zero or more values, sorted by area in ascending order.
+E.g. <cite>names.area_of_interest</cite> could be [‘Gulf Islands National Seashore’, ‘Santa Rosa Island’], [“Knott’s Berry Farm”], or [] if <cite>area_of_interest</cite> not defined.
+The value shown in Photos is the first value in the list. With the exception of <cite>body_of_water</cite> each of these field corresponds to an attribute of
+a [CLPlacemark](<a class="reference external" href="https://developer.apple.com/documentation/corelocation/clplacemark">https://developer.apple.com/documentation/corelocation/clplacemark</a>) object.</p>
+<ul class="simple">
+<li><p><cite>country</cite>; the name of the country associated with the placemark.</p></li>
+<li><p><cite>state_province</cite>; administrativeArea, The state or province associated with the placemark.</p></li>
+<li><p><cite>sub_administrative_area</cite>; additional administrative area information for the placemark.</p></li>
+<li><p><cite>city</cite>; locality; the city associated with the placemark.</p></li>
+<li><p><cite>additional_city_info</cite>; subLocality, Additional city-level information for the placemark.</p></li>
+<li><p><cite>ocean</cite>; the name of the ocean associated with the placemark.</p></li>
+<li><p><cite>area_of_interest</cite>; areasOfInterest, The relevant areas of interest associated with the placemark.</p></li>
+<li><p><cite>inland_water</cite>; the name of the inland water body associated with the placemark.</p></li>
+<li><p><cite>region</cite>; the geographic region associated with the placemark.</p></li>
+<li><p><cite>sub_throughfare</cite>; additional street-level information for the placemark.</p></li>
+<li><p><cite>postal_code</cite>; the postal code associated with the placemark.</p></li>
+<li><p><cite>street_address</cite>; throughfare, The street address associated with the placemark.</p></li>
+<li><p><cite>body_of_water</cite>; in Photos 4, any body of water; in Photos 5 contains the union of ocean and inland_water</p></li>
+</ul>
+<p><strong>Note</strong>: In Photos &lt;= 4.0, only the following fields are defined; all others are set to empty list:</p>
+<ul class="simple">
+<li><p><cite>country</cite></p></li>
+<li><p><cite>state_province</cite></p></li>
+<li><p><cite>sub_administrative_area</cite></p></li>
+<li><p><cite>city</cite></p></li>
+<li><p><cite>additional_city_info</cite></p></li>
+<li><p><cite>area_of_interest</cite></p></li>
+<li><p><cite>body_of_water</cite></p></li>
+</ul>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>The <cite>PlaceNames</cite> namedtuple contains reserved fields not listed below (see implementation for details),
+thus it should be referenced only by name (e.g. <cite>names.city</cite>) and not by index.</p>
+</div>
+</dd></dl>
+
+</dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ProjectInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ProjectInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#ProjectInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ProjectInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>ProjectInfo with info about projects
 Projects are cards, calendars, slideshows, etc.</p>
 <dl class="py property">
@@ -3897,14 +4116,30 @@
 </li>
 <li><a class="reference internal" href="#osxphotos.ExportResults"><code class="docutils literal notranslate"><span class="pre">ExportResults</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.ExportResults.all_files"><code class="docutils literal notranslate"><span class="pre">ExportResults.all_files()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportResults.attributes"><code class="docutils literal notranslate"><span class="pre">ExportResults.attributes</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportResults.datetime"><code class="docutils literal notranslate"><span class="pre">ExportResults.datetime</span></code></a></li>
 </ul>
 </li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo"><code class="docutils literal notranslate"><span class="pre">FaceInfo</span></code></a><ul>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.asdict"><code class="docutils literal notranslate"><span class="pre">FaceInfo.asdict()</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.center"><code class="docutils literal notranslate"><span class="pre">FaceInfo.center</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.face_rect"><code class="docutils literal notranslate"><span class="pre">FaceInfo.face_rect()</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.json"><code class="docutils literal notranslate"><span class="pre">FaceInfo.json()</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.mpri_reg_rect"><code class="docutils literal notranslate"><span class="pre">FaceInfo.mpri_reg_rect</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.mwg_rs_area"><code class="docutils literal notranslate"><span class="pre">FaceInfo.mwg_rs_area</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.person_info"><code class="docutils literal notranslate"><span class="pre">FaceInfo.person_info</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.photo"><code class="docutils literal notranslate"><span class="pre">FaceInfo.photo</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.pitch"><code class="docutils literal notranslate"><span class="pre">FaceInfo.pitch</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.roll"><code class="docutils literal notranslate"><span class="pre">FaceInfo.roll</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.roll_pitch_yaw"><code class="docutils literal notranslate"><span class="pre">FaceInfo.roll_pitch_yaw()</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.size_pixels"><code class="docutils literal notranslate"><span class="pre">FaceInfo.size_pixels</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.FaceInfo.yaw"><code class="docutils literal notranslate"><span class="pre">FaceInfo.yaw</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#osxphotos.FileUtil"><code class="docutils literal notranslate"><span class="pre">FileUtil</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp.convert_to_jpeg"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.convert_to_jpeg()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp.copy"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.copy()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp.file_sig"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.file_sig()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp.hardlink"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.hardlink()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.FileUtilNoOp.rename"><code class="docutils literal notranslate"><span class="pre">FileUtilNoOp.rename()</span></code></a></li>
@@ -4105,15 +4340,23 @@
 <li><a class="reference internal" href="#osxphotos.PhotosDB.photos"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.photos_by_uuid"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_by_uuid()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.photos_version"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_version</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
-<li><a class="reference internal" href="#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a><ul>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.address"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.address_str"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address_str</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.country_code"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.country_code</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.ishome"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.ishome</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.name"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.name</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.names"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.names</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.ProjectInfo.folder_list"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_list</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ProjectInfo.folder_names"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_names</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions"><code class="docutils literal notranslate"><span class="pre">QueryOptions</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.added_after"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_after</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -450,14 +450,70 @@
       Results class which holds export results for export
         all_files() &#x2192; List[str][source]#
             return all filenames contained in results
         propertyattributes: List[str]#
             Return list of attributes tracked by ExportResults
         propertydatetime: str#
             Return datetime when ExportResults was created
+  classosxphotos.FaceInfo(db=None, pk=None)[source]#
+      Info about a face in the Photos library
+        asdict()[source]#
+            Returns dict representation of class instance
+        propertycenter#
+            Coordinates, in PIL format, for center of face
+              Returns:
+                  tuple of coordinates in form (x, y)
+        face_rect()[source]#
+              Get face rectangle coordinates for current version of the
+              associated image
+                  If image has been edited, rectangle applies to edited
+                  version, otherwise original version Coordinates in format and
+                  reference frame used by PIL
+              Returns:
+                  list [(x0, x1), (y0, y1)] of coordinates in reference frame
+                  used by PIL
+        json()[source]#
+            Return JSON representation of FaceInfo instance
+        propertympri_reg_rect#
+            Get coordinates for Microsoft Photo Region Rectangle.
+              Returns:
+                  x = x coordinate of top left corner of rectangle y = y
+                  coordinate of top left corner of rectangle h = height of
+                  rectangle w = width of rectangle
+              Return type:
+                  MPRI_Reg_Rect named tuple with x, y, h, w where
+              Reference:
+                  https://docs.microsoft.com/en-us/windows/win32/wic/-wic-
+                  people-tagging
+        propertymwg_rs_area#
+            Get coordinates for Metadata Working Group Region Area.
+              Returns:
+                  x = stArea:x y = stArea:y h = stArea:h w = stArea:w
+              Return type:
+                  MWG_RS_Area named tuple with x, y, h, w where
+              Reference:
+                  https://photo.stackexchange.com/questions/106410/how-does-
+                  xmp-define-the-face-region
+        propertyperson_info#
+            PersonInfo instance for person associated with this face
+        propertyphoto#
+            PhotoInfo instance associated with this face
+        propertypitch#
+            Return pitch angle in radians of the face region
+        propertyroll#
+            Return roll angle in radians of the face region
+        roll_pitch_yaw()[source]#
+            Roll, pitch, yaw of face in radians as tuple
+        propertysize_pixels#
+            Size of face in pixels (centered around center_x, center_y)
+              Returns:
+                  size, in int pixels, of a circle drawn around the center of
+                  the face
+        propertyyaw#
+            Return yaw angle in radians of the face region
   classosxphotos.FileUtil[source]#
       Various file utilities
   classosxphotos.FileUtilNoOp(verbose=None)[source]#
       No-Op implementation of FileUtil for testing / dry-run mode all methods
       with exception of tmpdir, cmp, cmp_file_sig and file_cmp are no-op cmp
       and cmp_file_sig functions as FileUtil methods do file_cmp returns mock
       data
@@ -1251,14 +1307,87 @@
             return list of AlbumInfo projects for each project in the database
         query(options: QueryOptions) &#x2192; List[PhotoInfo][source]#
             Run a query against PhotosDB to extract the photos based on user
             supplied options
               Parameters:
                   options â a QueryOptions instance
   classosxphotos.PlaceInfo[source]#
+      Reverse geolocation place info for a photo.
+        propertyaddress#
+            Returns aPostalAddressnamedtuple with details of the postal address
+            containing the following fields:
+                * city
+                * country
+                * postal_code
+                * state
+                * street
+                * sub_administrative_area
+                * sub_locality
+                * iso_country_code
+        propertyaddress_str: str | None#
+            Returns the full postal address as a string if defined,
+            otherwiseNone.
+        propertycountry_code: str | None#
+            Returns the country_code of place, for example âGBâ.
+            ReturnsNoneif PhotoInfo contains no country code.
+        propertyishome: bool#
+            ReturnsTrueif photo place is userâs home address, otherwiseFalse.
+        propertyname: str | None#
+            Returns the name of the local place as str. This is what Photos
+            displays in the Info window. Note Photos 5 uses a different
+            algorithm to determine the name than earlier versions which means
+            the same Photo may have a different place name in Photos 4 and
+            Photos 5.PhotoInfo.namewill return the name Photos would have shown
+            depending on the version of the library being processed.
+            ReturnsNoneif photo does not contain a name.
+        propertynames: osxphotos.placeinfo.PlaceNames | None#
+            Returns aPlaceNamesnamedtuple with the following fields. Each field
+            is a list with zero or more values, sorted by area in ascending
+            order. E.g.names.area_of_interestcould be [âGulf Islands National
+            Seashoreâ, âSanta Rosa Islandâ], [âKnottâs Berry
+            Farmâ], or [] ifarea_of_interestnot defined. The value shown in
+            Photos is the first value in the list. With the exception
+            ofbody_of_watereach of these field corresponds to an attribute of a
+            [CLPlacemark](https://developer.apple.com/documentation/
+            corelocation/clplacemark) object.
+                * country; the name of the country associated with the
+                  placemark.
+                * state_province; administrativeArea, The state or province
+                  associated with the placemark.
+                * sub_administrative_area; additional administrative area
+                  information for the placemark.
+                * city; locality; the city associated with the placemark.
+                * additional_city_info; subLocality, Additional city-level
+                  information for the placemark.
+                * ocean; the name of the ocean associated with the placemark.
+                * area_of_interest; areasOfInterest, The relevant areas of
+                  interest associated with the placemark.
+                * inland_water; the name of the inland water body associated
+                  with the placemark.
+                * region; the geographic region associated with the placemark.
+                * sub_throughfare; additional street-level information for the
+                  placemark.
+                * postal_code; the postal code associated with the placemark.
+                * street_address; throughfare, The street address associated
+                  with the placemark.
+                * body_of_water; in Photos 4, any body of water; in Photos 5
+                  contains the union of ocean and inland_water
+            Note: In Photos <= 4.0, only the following fields are defined; all
+            others are set to empty list:
+                * country
+                * state_province
+                * sub_administrative_area
+                * city
+                * additional_city_info
+                * area_of_interest
+                * body_of_water
+            Note
+            ThePlaceNamesnamedtuple contains reserved fields not listed below
+            (see implementation for details), thus it should be referenced only
+            by name (e.g.names.city) and not by index.
   classosxphotos.ProjectInfo(db, uuid)[source]#
       ProjectInfo with info about projects Projects are cards, calendars,
       slideshows, etc.
         propertyfolder_list#
             Returns list of FolderInfo objects for each folder the album is
             contained in or empty list if album is not in any folders
         propertyfolder_names#
@@ -1817,14 +1946,28 @@
                 # ExportOptions.tmpdir
                 # ExportOptions.favorite_rating
                 # ExportOptions.bit_flags
           o ExportResults
                 # ExportResults.all_files()
                 # ExportResults.attributes
                 # ExportResults.datetime
+          o FaceInfo
+                # FaceInfo.asdict()
+                # FaceInfo.center
+                # FaceInfo.face_rect()
+                # FaceInfo.json()
+                # FaceInfo.mpri_reg_rect
+                # FaceInfo.mwg_rs_area
+                # FaceInfo.person_info
+                # FaceInfo.photo
+                # FaceInfo.pitch
+                # FaceInfo.roll
+                # FaceInfo.roll_pitch_yaw()
+                # FaceInfo.size_pixels
+                # FaceInfo.yaw
           o FileUtil
           o FileUtilNoOp
                 # FileUtilNoOp.convert_to_jpeg()
                 # FileUtilNoOp.copy()
                 # FileUtilNoOp.file_sig()
                 # FileUtilNoOp.hardlink()
                 # FileUtilNoOp.rename()
@@ -2008,14 +2151,20 @@
                 # PhotosDB.persons_as_dict
                 # PhotosDB.photos()
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
+                # PlaceInfo.address
+                # PlaceInfo.address_str
+                # PlaceInfo.country_code
+                # PlaceInfo.ishome
+                # PlaceInfo.name
+                # PlaceInfo.names
           o ProjectInfo
                 # ProjectInfo.folder_list
                 # ProjectInfo.folder_names
           o QueryOptions
                 # QueryOptions.added_after
                 # QueryOptions.added_before
                 # QueryOptions.added_in_last
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.5 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.6 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -98,15 +98,15 @@
         "ani": [0, 2, 3, 4, 5, 6],
         "valid": [0, 3, 4, 5, 6],
         "pygment": 0,
         "org": [0, 4, 5, 6],
         "default": [0, 3, 4, 5, 6],
         "monokai": 0,
         "verbos": [0, 1, 4, 6],
-        "document": [0, 2, 5],
+        "document": [0, 2, 4, 5],
         "browser": [0, 2],
         "all": [0, 1, 2, 3, 4, 5],
         "associ": [0, 2, 4, 5, 6],
         "from": [0, 1, 2, 3, 4, 5],
         "delet": [0, 1, 4],
         "folder": [0, 1, 3, 4, 5, 6],
         "f": [0, 3, 4, 5],
@@ -155,15 +155,15 @@
         "load": [0, 1, 3],
         "configur": [0, 6],
         "match": [0, 4, 5, 6],
         "other": [0, 4, 5, 6],
         "conjunct": [0, 6],
         "thei": [0, 4, 6],
         "overrid": [0, 5],
-        "correspond": 0,
+        "correspond": [0, 4],
         "config_fil": 0,
         "written": [0, 4, 5, 6],
         "save": [0, 1, 4],
         "toml": [0, 6],
         "exiftool_path": [0, 4],
         "look": [0, 2, 4, 6],
         "flag": [0, 4],
@@ -187,23 +187,23 @@
         "date": [0, 1, 2, 3, 4, 5],
         "modifi": [0, 4, 5, 6],
         "modif": [0, 4, 5, 6],
         "exif": [0, 1, 3, 4, 5],
         "modifyd": [0, 4],
         "datetimeorigin": [0, 4],
         "consist": 0,
-        "how": [0, 5, 6],
+        "how": [0, 4, 5, 6],
         "handl": [0, 6],
         "tag": [0, 2, 4, 5, 6],
         "imag": [0, 1, 2, 4, 5],
         "form": [0, 4, 5, 6],
         "same": [0, 2, 3, 4, 5, 6],
         "add": [1, 4, 5, 6],
         "contain": [0, 3, 4, 5, 6],
-        "could": [0, 3, 5, 6],
+        "could": [0, 3, 4, 5, 6],
         "folder_album": [0, 4, 5, 6],
         "year": [0, 1, 4, 5, 6],
         "replac": [0, 4, 5, 6],
         "below": [0, 4],
         "By": [0, 6],
         "exist": [0, 3, 4, 6],
         "instead": [0, 4, 5, 6],
@@ -234,43 +234,43 @@
         "actual": [0, 1, 4, 5],
         "signatur": [0, 4, 6],
         "color": [0, 1, 2],
         "dark": [0, 6],
         "light": 0,
         "mono": 0,
         "plain": [0, 6],
-        "depend": [0, 5],
+        "depend": [0, 4, 5],
         "requir": [0, 2, 4, 5, 6],
         "dest": [0, 4],
         "search": [0, 1, 2, 4, 6],
         "treat": [0, 4, 5, 6],
         "AND": [0, 4],
         "edit": [1, 2, 3, 4, 5],
         "live": [0, 1, 4, 5, 6],
         "movi": [0, 1, 4, 6],
         "burst": [0, 1, 4, 5],
         "skip": [0, 3, 4, 6],
         "behavior": [0, 4],
         "progress": 0,
-        "displai": [0, 2, 5],
+        "displai": [0, 2, 4, 5],
         "bar": [0, 3, 5],
         "dure": [0, 1, 4],
         "OR": [0, 4],
         "top": [0, 4, 6],
         "level": [0, 4, 6],
         "doe": [0, 3, 4, 5, 6],
         "subfold": [0, 1, 4, 5],
         "singl": [0, 4, 5, 6],
         "per": 0,
         "preced": [0, 5, 6],
         "desc": 0,
         "revers": [0, 4, 5, 6],
         "geoloc": [0, 4, 5, 6],
         "gp": [0, 6],
-        "coordin": [0, 6],
+        "coordin": [0, 4, 6],
         "classif": [0, 2, 6],
         "5": [0, 2, 3, 4, 5],
         "uti": [0, 1, 4],
         "whose": 0,
         "uniform": [0, 4],
         "type": [0, 2, 3, 4, 5, 6],
         "identifi": [0, 4, 5, 6],
@@ -327,15 +327,15 @@
         "to_tim": [0, 4],
         "specif": [0, 2, 4, 6],
         "2022": [0, 3],
         "befor": [0, 4, 5, 6],
         "after": [0, 4, 5, 6],
         "librai": 0,
         "time_delta": 0,
-        "where": [0, 5, 6],
+        "where": [0, 4, 5, 6],
         "like": [0, 1, 3, 4, 5, 6],
         "hr": 0,
         "1d": 0,
         "week": [0, 5, 6],
         "2week": 0,
         "month": [0, 1, 4, 5, 6],
         "7d": 0,
@@ -361,15 +361,15 @@
         "size": [0, 4, 5, 6],
         "height": [0, 1, 4],
         "width": [0, 1, 4],
         "statu": [0, 4],
         "byte": [0, 4],
         "nor": 0,
         "hash": [0, 4],
-        "should": [0, 2, 5, 6],
+        "should": [0, 2, 4, 5, 6],
         "within": [0, 5],
         "integ": [0, 5],
         "si": 0,
         "nist": 0,
         "unit": [0, 5],
         "1048576": 0,
         "048576mb": 0,
@@ -471,15 +471,15 @@
         "non": [0, 4, 6],
         "heic": 0,
         "png": 0,
         "qualiti": [0, 4, 6],
         "ext": [0, 4, 6],
         "mac": [0, 2, 6],
         "gpu": 0,
-        "thu": [0, 6],
+        "thu": [0, 4, 6],
         "virtual": [0, 3],
         "machin": [0, 2, 4, 5, 6],
         "jpeg_qual": [0, 1, 4],
         "0": [0, 2, 3, 4, 5, 6],
         "A": [0, 5, 6],
         "best": [0, 4, 6],
         "maximum": [0, 4],
@@ -508,15 +508,15 @@
         "digikam": [0, 6],
         "lightroom": [0, 6],
         "subject": [0, 4],
         "personinimag": [0, 4],
         "created": [0, 4],
         "gpslongitud": [0, 4],
         "region": [0, 4],
-        "microsoft": [0, 6],
+        "microsoft": [0, 4, 6],
         "useabl": 0,
         "appli": [0, 4, 5, 6],
         "j": [0, 4],
         "compat": [0, 6],
         "drop": [0, 4, 6],
         "photo_filenam": 0,
         "photo_ext": 0,
@@ -698,15 +698,15 @@
         "relative_to_path": 0,
         "comput": [0, 3, 4],
         "dup": 0,
         "split": [0, 5],
         "split_fold": [0, 4],
         "hierarch": [0, 4, 6],
         "charact": [0, 3, 5, 6],
-        "w": 0,
+        "w": [0, 4],
         "walk": 0,
         "recurs": 0,
         "through": [0, 2, 6],
         "glob": 0,
         "unix": 0,
         "pattern": [0, 6],
         "resum": [0, 6],
@@ -722,15 +722,15 @@
         "As": [0, 6],
         "press": 0,
         "ctrl": 0,
         "modern": 0,
         "kitti": 0,
         "text": [0, 4, 5, 6],
         "packag": [0, 1, 2],
-        "u": [0, 5],
+        "u": [0, 4, 5],
         "upgrad": 0,
         "latest": 0,
         "export_path": [0, 3],
         "present": [0, 5],
         "cloudasset": [0, 1, 4],
         "incloud": [0, 1, 4],
         "quiet": 0,
@@ -740,18 +740,18 @@
         "launch": 0,
         "keybind": 0,
         "vi": 0,
         "bind": 0,
         "made": [0, 5],
         "avail": [0, 4, 5, 6],
         "python_fil": 0,
-        "h": [0, 2, 5],
+        "h": [0, 2, 4, 5],
         "messag": [0, 2, 4],
         "entir": [0, 4, 6],
-        "defin": [0, 3, 5, 6],
+        "defin": [0, 3, 4, 5, 6],
         "new_them": 0,
         "adjust": [0, 1, 2, 4, 5, 6],
         "oper": [0, 1, 5, 6],
         "smart": [0, 6],
         "view": 0,
         "overview": [0, 1],
         "yyyi": 0,
@@ -774,15 +774,15 @@
         "02": [0, 5, 6],
         "ahead": [0, 4],
         "13": [0, 4],
         "old": 0,
         "exhibit": 0,
         "manual": [0, 6],
         "get": [0, 2, 3, 4, 5, 6],
-        "window": 0,
+        "window": [0, 4],
         "push": 0,
         "pull": 0,
         "It": [0, 4, 5, 6],
         "might": [0, 4, 6],
         "thusli": 0,
         "unless": [0, 4, 5],
         "naiv": [0, 4],
@@ -798,15 +798,15 @@
         "those": [0, 3, 4, 6],
         "o": [2, 3, 4],
         "output_fil": [],
         "rich": [0, 1, 4, 6],
         "bypass": 0,
         "confirm": 0,
         "prompt": 0,
-        "y": [0, 5],
+        "y": [0, 4, 5],
         "ye": 0,
         "ask": 0,
         "uniqu": [0, 2, 4, 5],
         "id": [0, 2, 4, 5],
         "suitabl": [0, 5],
         "usag": [0, 1, 3, 5],
         "instal": [1, 3, 4, 5, 6],
@@ -820,15 +820,15 @@
         "theme": [1, 2],
         "conclus": 1,
         "interfac": [1, 2, 3, 4, 6],
         "cli": [1, 2],
         "about": [1, 2, 3, 4, 6],
         "album": [1, 2, 3, 4, 5, 6],
         "diff": [1, 2],
-        "doc": [1, 2],
+        "doc": [1, 2, 4],
         "dump": [1, 2],
         "exiftool": [1, 3, 4, 5, 6],
         "exportdb": [1, 4, 6],
         "help": [1, 2, 3, 5, 6],
         "import": [1, 3, 4, 5, 6],
         "info": [1, 2, 4],
         "inspect": [1, 3],
@@ -841,15 +841,15 @@
         "repl": [1, 2],
         "snap": [1, 2],
         "timewarp": [1, 2],
         "uninstal": [1, 2, 3],
         "uuid": [1, 2, 3, 4, 5],
         "version": [1, 2, 3, 4, 5, 6],
         "substitut": [1, 4],
-        "code": [1, 2, 5],
+        "code": [1, 2, 4, 5],
         "api": [],
         "albuminfo": [1, 3, 4],
         "folder_list": [1, 4],
         "folder_nam": [1, 4],
         "photo_index": [1, 4],
         "sort_ord": [1, 4],
         "albumsortord": [1, 4],
@@ -1127,15 +1127,15 @@
         "dest_dir": 3,
         "join": [3, 5, 6],
         "isdir": 3,
         "makedir": 3,
         "edited_nam": 3,
         "unedit": [3, 6],
         "loop": 3,
-        "develop": 3,
+        "develop": [3, 4],
         "feb": 3,
         "36": [3, 5],
         "clang": 3,
         "1200": 3,
         "32": 3,
         "29": 3,
         "47": 3,
@@ -1211,15 +1211,15 @@
         "dictionari": 4,
         "dict": 4,
         "kei": [4, 5, 6],
         "no_fil": 4,
         "errror": 4,
         "dbfile": 4,
         "sqlite3": 4,
-        "union": [],
+        "union": 4,
         "exportrecord": 4,
         "record": 4,
         "given": [0, 4],
         "retriev": [4, 6],
         "tupl": 4,
         "track": [4, 6],
         "struct": [],
@@ -1291,15 +1291,15 @@
         "its": [4, 5, 6],
         "content": 4,
         "filesystem": [0, 4, 6],
         "access": [4, 5, 6],
         "moment_pk": 4,
         "stop": [4, 5],
         "represent": [4, 5],
-        "faceinfo": 4,
+        "faceinfo": [1, 4],
         "highest": 4,
         "lowest": 4,
         "n": [4, 5, 6],
         "build": 4,
         "send": 4,
         "captionabstract": 4,
         "objectnam": 4,
@@ -1521,55 +1521,55 @@
         "190738": 5,
         "vid\u00e9o": 5,
         "vid\u00e9o_acc\u00e9l\u00e9r\u00e9": 5,
         "openbrac": 5,
         "closebrac": 5,
         "var": 5,
         "prohibit": 5,
-        "around": 5,
+        "around": [4, 5],
         "kati": 5,
         "percent": 5,
         "sign": 5,
         "escap": 5,
         "photo_or_video": 5,
         "foto": 5,
         "value_if_tru": 5,
         "value_if_fals": 5,
         "edited_vers": 5,
         "03": 5,
         "22": 5,
         "digit": [5, 6],
         "yy": 5,
-        "zero": 5,
+        "zero": [4, 5],
         "pad": 5,
         "mon": 5,
         "dow": 5,
         "doi": 5,
         "julian": 5,
         "23": [0, 5],
         "null": [5, 6],
-        "country_cod": 5,
-        "state_provinc": 5,
-        "provinc": 5,
-        "area_of_interest": 5,
-        "area": 5,
-        "interest": [5, 6],
+        "country_cod": [1, 4, 5],
+        "state_provinc": [4, 5],
+        "provinc": [4, 5],
+        "area_of_interest": [4, 5],
+        "area": [4, 5],
+        "interest": [4, 5, 6],
         "landmark": 5,
-        "address": 5,
-        "postal": 5,
+        "address": [1, 4, 5],
+        "postal": [4, 5],
         "2007": 5,
         "18th": 5,
         "st": 5,
         "nw": 5,
         "washington": 5,
         "dc": 5,
         "20009": 5,
-        "postal_cod": 5,
+        "postal_cod": [4, 5],
         "summer": [5, 6],
-        "algorithm": [5, 6],
+        "algorithm": [4, 5, 6],
         "iphon": [0, 5, 6],
         "15mm": 5,
         "intern": [4, 5, 6],
         "univers": 5,
         "128fb4c6": 5,
         "0b16": 5,
         "4e7d": 5,
@@ -1588,15 +1588,15 @@
         "sequenc": 5,
         "seq": 5,
         "starting_valu": 5,
         "00000": 5,
         "0001": 5,
         "folder_album_seq": 5,
         "questionmark": 5,
-        "question": 5,
+        "question": [4, 5],
         "openparen": 5,
         "closeparen": 5,
         "openbracket": 5,
         "closebracket": 5,
         "newlin": [5, 6],
         "lf": 5,
         "feed": 5,
@@ -1642,15 +1642,15 @@
         "sever": 6,
         "focu": 6,
         "probabl": 6,
         "thousand": 6,
         "isn": 6,
         "2021": 6,
         "21": 6,
-        "With": 6,
+        "With": [4, 6],
         "2015": 6,
         "05": 6,
         "prefer": 6,
         "wide": 6,
         "throughout": 6,
         "worth": 6,
         "interpret": 6,
@@ -1694,15 +1694,15 @@
         "na": [0, 6],
         "devic": [0, 6],
         "unreli": 6,
         "flaki": 6,
         "decreas": 6,
         "dbpath": 6,
         "put": 6,
-        "home": 6,
+        "home": [4, 6],
         "rememb": 6,
         "ram": 6,
         "much": 6,
         "offer": 6,
         "signific": 6,
         "boost": 6,
         "tremend": 6,
@@ -1777,24 +1777,24 @@
         "bin": 6,
         "integr": 6,
         "concept": 6,
         "discuss": 6,
         "thank": 6,
         "philipp": 6,
         "contribut": 6,
-        "roll": 6,
+        "roll": [1, 4, 6],
         "basi": 6,
         "ot": 6,
         "rise": 6,
         "nevertheless": 6,
         "good": 6,
         "cut": 6,
         "pro": 6,
         "pick": 6,
-        "left": 6,
+        "left": [4, 6],
         "chose": 6,
         "quik": 6,
         "spot": 6,
         "gopro": 6,
         "popul": 6,
         "enabl": 6,
         "desktop": 6,
@@ -1960,15 +1960,15 @@
         "19393": [],
         "shared_movi": [],
         "keyword_dict": [],
         "ie": [],
         "persons_dict": [],
         "albums_dict": [],
         "albums_shared_dict": [],
-        "peopl": [],
+        "peopl": 4,
         "dog": [],
         "easier": [],
         "conn": [],
         "zuuid": [],
         "zgenericasset": [],
         "zfavorit": [],
         "fetchal": [],
@@ -2074,58 +2074,58 @@
         "enum": [],
         "unknown": [],
         "newest_first": [],
         "oldest_first": [],
         "effect": [],
         "children": [],
         "0x10fcc0160": [],
-        "shown": [],
+        "shown": 4,
         "mayfair": [],
         "shop": [],
         "centr": [],
         "victoria": [],
         "canada": [],
         "vancouv": [],
-        "island": [],
+        "island": 4,
         "british": [],
         "columbia": [],
-        "placenam": [],
-        "namedtupl": [],
-        "ascend": [],
-        "gulf": [],
-        "nation": [],
-        "seashor": [],
-        "santa": [],
-        "rosa": [],
-        "knott": [],
-        "berri": [],
-        "farm": [],
-        "body_of_wat": [],
-        "clplacemark": [],
-        "reserv": [],
-        "placemark": [],
-        "administrativearea": [],
-        "sub_administrative_area": [],
-        "administr": [],
-        "additional_city_info": [],
-        "subloc": [],
-        "ocean": [],
-        "areasofinterest": [],
-        "relev": [],
-        "inland_wat": [],
-        "inland": [],
-        "geograph": [],
-        "sub_throughfar": [],
-        "street_address": [],
-        "throughfar": [],
-        "gb": [],
+        "placenam": 4,
+        "namedtupl": 4,
+        "ascend": 4,
+        "gulf": 4,
+        "nation": 4,
+        "seashor": 4,
+        "santa": 4,
+        "rosa": 4,
+        "knott": 4,
+        "berri": 4,
+        "farm": 4,
+        "body_of_wat": 4,
+        "clplacemark": 4,
+        "reserv": 4,
+        "placemark": 4,
+        "administrativearea": 4,
+        "sub_administrative_area": 4,
+        "administr": 4,
+        "additional_city_info": 4,
+        "subloc": 4,
+        "ocean": 4,
+        "areasofinterest": 4,
+        "relev": 4,
+        "inland_wat": 4,
+        "inland": 4,
+        "geograph": 4,
+        "sub_throughfar": 4,
+        "street_address": 4,
+        "throughfar": 4,
+        "gb": 4,
         "2038": [],
-        "postaladdress": [],
-        "sub_loc": [],
-        "iso_country_cod": [],
+        "postaladdress": 4,
+        "sub_loc": 4,
+        "iso_country_cod": 4,
         "3700": [],
         "wailea": [],
         "alanui": [],
         "dr": [],
         "kihei": [],
         "maui": [],
         "hi": [],
@@ -2137,30 +2137,30 @@
         "municip": [],
         "witht": [],
         "photoo": [],
         "thumbnail": [],
         "shortcut": [],
         "metdata": [],
         "mwg": [],
-        "starea": [],
-        "rectangl": [],
+        "starea": 4,
+        "rectangl": 4,
         "mpri": [],
-        "corner": [],
-        "x0": [],
-        "y0": [],
-        "x1": [],
-        "y1": [],
+        "corner": 4,
+        "x0": 4,
+        "y0": 4,
+        "x1": 4,
+        "y1": 4,
         "rectangular": [],
-        "frame": [],
+        "frame": 4,
         "pillow": [],
         "pathedit": [],
         "diamet": [],
-        "radian": [],
-        "center_x": [],
-        "center_i": [],
+        "radian": 4,
+        "center_x": 4,
+        "center_i": 4,
         "measur": [],
         "source_width": [],
         "source_height": [],
         "has_smil": [],
         "face_typ": [],
         "age_typ": [],
         "eye_makeup_typ": [],
@@ -2209,28 +2209,28 @@
         "singleton": [],
         "tmpfile": [],
         "avoid": [],
         "unnecessari": [],
         "osxmetadata": [],
         "xarg": [],
         "creation_d": [],
-        "ishom": [],
-        "address_str": [],
+        "ishom": [1, 4],
+        "address_str": [1, 4],
         "display_nam": [],
         "keyphoto": [],
         "facecount": [],
         "asset_uuid": [],
-        "mwg_rs_area": [],
-        "mpri_reg_rect": [],
-        "face_rect": [],
-        "center": [],
-        "size_pixel": [],
-        "roll_pitch_yaw": [],
-        "pitch": [],
-        "yaw": [],
+        "mwg_rs_area": [1, 4],
+        "mpri_reg_rect": [1, 4],
+        "face_rect": [1, 4],
+        "center": [1, 4],
+        "size_pixel": [1, 4],
+        "roll_pitch_yaw": [1, 4],
+        "pitch": [1, 4],
+        "yaw": [1, 4],
         "get_system_library_path": [],
         "get_last_library_path": [],
         "list_photo_librari": [],
         "cloud_guid": [1, 4],
         "cloud_owner_hashed_id": [1, 4],
         "guid": 4,
         "root": 0,
@@ -2252,15 +2252,25 @@
         "shallow": 4,
         "shutil": 4,
         "photot": 4,
         "60": 5,
         "syndic": [0, 1, 4],
         "saved_to_librari": [1, 4],
         "not_synd": [1, 4],
-        "not_saved_to_librari": [1, 4]
+        "not_saved_to_librari": [1, 4],
+        "pil": 4,
+        "en": 4,
+        "win32": 4,
+        "wic": 4,
+        "stackexchang": 4,
+        "106410": 4,
+        "angl": 4,
+        "circl": 4,
+        "drawn": 4,
+        "coreloc": 4
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2268,14 +2278,15 @@
             [4, 1, 1, "", "CommentInfo"],
             [4, 1, 1, "", "ExifInfo"],
             [4, 1, 1, "", "ExifTool"],
             [4, 1, 1, "", "ExportDB"],
             [4, 1, 1, "", "ExportDBTemp"],
             [4, 1, 1, "", "ExportOptions"],
             [4, 1, 1, "", "ExportResults"],
+            [4, 1, 1, "", "FaceInfo"],
             [4, 1, 1, "", "FileUtil"],
             [4, 1, 1, "", "FileUtilNoOp"],
             [4, 1, 1, "", "FolderInfo"],
             [4, 1, 1, "", "ImportInfo"],
             [4, 1, 1, "", "LikeInfo"],
             [4, 1, 1, "", "MomentInfo"],
             [4, 1, 1, "", "PersonInfo"],
@@ -2288,17 +2299,14 @@
             [4, 1, 1, "", "PlaceInfo"],
             [4, 1, 1, "", "ProjectInfo"],
             [4, 1, 1, "", "QueryOptions"],
             [4, 1, 1, "", "ScoreInfo"],
             [4, 1, 1, "", "SearchInfo"],
             [4, 5, 1, "", "is_debug"],
             [4, 5, 1, "", "set_debug"],
-            [0, 6, 1, "cmdoption-osxphotos-library", "--db"],
-            [0, 6, 1, "cmdoption-osxphotos-json", "--json"],
-            [0, 6, 1, "cmdoption-osxphotos-library", "--library"],
             [0, 6, 1, "cmdoption-osxphotos-v", "--version"],
             [0, 6, 1, "cmdoption-osxphotos-v", "-v"]
         ],
         "osxphotos.AlbumInfo": [
             [4, 2, 1, "", "asdict"],
             [4, 3, 1, "", "folder_list"],
             [4, 3, 1, "", "folder_names"],
@@ -2386,14 +2394,29 @@
             [4, 4, 1, "", "verbose"]
         ],
         "osxphotos.ExportResults": [
             [4, 2, 1, "", "all_files"],
             [4, 3, 1, "", "attributes"],
             [4, 3, 1, "", "datetime"]
         ],
+        "osxphotos.FaceInfo": [
+            [4, 2, 1, "", "asdict"],
+            [4, 3, 1, "", "center"],
+            [4, 2, 1, "", "face_rect"],
+            [4, 2, 1, "", "json"],
+            [4, 3, 1, "", "mpri_reg_rect"],
+            [4, 3, 1, "", "mwg_rs_area"],
+            [4, 3, 1, "", "person_info"],
+            [4, 3, 1, "", "photo"],
+            [4, 3, 1, "", "pitch"],
+            [4, 3, 1, "", "roll"],
+            [4, 2, 1, "", "roll_pitch_yaw"],
+            [4, 3, 1, "", "size_pixels"],
+            [4, 3, 1, "", "yaw"]
+        ],
         "osxphotos.FileUtilNoOp": [
             [4, 2, 1, "", "convert_to_jpeg"],
             [4, 2, 1, "", "copy"],
             [4, 2, 1, "", "file_sig"],
             [4, 2, 1, "", "hardlink"],
             [4, 2, 1, "", "rename"],
             [4, 2, 1, "", "rmdir"],
@@ -2581,14 +2604,22 @@
             [4, 3, 1, "", "persons_as_dict"],
             [4, 2, 1, "", "photos"],
             [4, 2, 1, "", "photos_by_uuid"],
             [4, 3, 1, "", "photos_version"],
             [4, 3, 1, "", "project_info"],
             [4, 2, 1, "", "query"]
         ],
+        "osxphotos.PlaceInfo": [
+            [4, 3, 1, "", "address"],
+            [4, 3, 1, "", "address_str"],
+            [4, 3, 1, "", "country_code"],
+            [4, 3, 1, "", "ishome"],
+            [4, 3, 1, "", "name"],
+            [4, 3, 1, "", "names"]
+        ],
         "osxphotos.ProjectInfo": [
             [4, 3, 1, "", "folder_list"],
             [4, 3, 1, "", "folder_names"]
         ],
         "osxphotos.QueryOptions": [
             [4, 4, 1, "", "added_after"],
             [4, 4, 1, "", "added_before"],
@@ -4112,3279 +4143,9 @@
         "Color Themes": [
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
-    "indexentries": {
-        "--add-exported-to-album": [
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
-        ],
-        "--add-missing-to-album": [
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
-        ],
-        "--add-skipped-to-album": [
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
-        ],
-        "--add-to-album": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "--added-after": [
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-after"]
-        ],
-        "--added-before": [
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-before"]
-        ],
-        "--added-in-last": [
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"]
-        ],
-        "--album": [
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-sync-album"]
-        ],
-        "--album-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-export-album-keyword"]
-        ],
-        "--alt-copy": [
-            [0, "cmdoption-osxphotos-export-alt-copy"]
-        ],
-        "--append": [
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-sync-A"]
-        ],
-        "--burst": [
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-sync-burst"]
-        ],
-        "--check-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
-        ],
-        "--check-templates": [
-            [0, "cmdoption-osxphotos-import-check-templates"]
-        ],
-        "--cleanup": [
-            [0, "cmdoption-osxphotos-export-cleanup"]
-        ],
-        "--clear-location": [
-            [0, "cmdoption-osxphotos-import-L"]
-        ],
-        "--clear-metadata": [
-            [0, "cmdoption-osxphotos-import-C"]
-        ],
-        "--clone": [
-            [0, "cmdoption-osxphotos-theme-clone"]
-        ],
-        "--cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"]
-        ],
-        "--compare-exif": [
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "--config": [
-            [0, "cmdoption-osxphotos-theme-config"]
-        ],
-        "--config-only": [
-            [0, "cmdoption-osxphotos-export-config-only"]
-        ],
-        "--convert-to-jpeg": [
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
-        ],
-        "--count": [
-            [0, "cmdoption-osxphotos-query-count"]
-        ],
-        "--current-name": [
-            [0, "cmdoption-osxphotos-export-current-name"]
-        ],
-        "--date": [
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "--date-added": [
-            [0, "cmdoption-osxphotos-timewarp-date-added"]
-        ],
-        "--date-added-from-photo": [
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
-        ],
-        "--date-delta": [
-            [0, "cmdoption-osxphotos-timewarp-D"]
-        ],
-        "--db": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"]
-        ],
-        "--db-config": [
-            [0, "cmdoption-osxphotos-exiftool-db-config"]
-        ],
-        "--default": [
-            [0, "cmdoption-osxphotos-theme-default"]
-        ],
-        "--delete": [
-            [0, "cmdoption-osxphotos-theme-delete"]
-        ],
-        "--delete-file": [
-            [0, "cmdoption-osxphotos-exportdb-delete-file"]
-        ],
-        "--delete-uuid": [
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
-        ],
-        "--deleted": [
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted"]
-        ],
-        "--deleted-only": [
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"]
-        ],
-        "--description": [
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-sync-description"]
-        ],
-        "--description-template": [
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-export-description-template"]
-        ],
-        "--detect-text": [
-            [0, "cmdoption-osxphotos-inspect-t"]
-        ],
-        "--directory": [
-            [0, "cmdoption-osxphotos-export-directory"]
-        ],
-        "--download-missing": [
-            [0, "cmdoption-osxphotos-export-download-missing"]
-        ],
-        "--dry-run": [
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-sync-dry-run"]
-        ],
-        "--dup-check": [
-            [0, "cmdoption-osxphotos-import-D"]
-        ],
-        "--duplicate": [
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-sync-duplicate"]
-        ],
-        "--edit": [
-            [0, "cmdoption-osxphotos-theme-edit"]
-        ],
-        "--edited": [
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-sync-edited"]
-        ],
-        "--edited-suffix": [
-            [0, "cmdoption-osxphotos-export-edited-suffix"]
-        ],
-        "--emacs": [
-            [0, "cmdoption-osxphotos-repl-emacs"]
-        ],
-        "--errors": [
-            [0, "cmdoption-osxphotos-exportdb-errors"]
-        ],
-        "--exif": [
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-sync-exif"]
-        ],
-        "--exiftool": [
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-import-e"]
-        ],
-        "--exiftool-merge-keywords": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
-        ],
-        "--exiftool-merge-persons": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
-        ],
-        "--exiftool-option": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"]
-        ],
-        "--exiftool-path": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "--export": [
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-sync-e"]
-        ],
-        "--export-as-hardlink": [
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
-        ],
-        "--export-by-date": [
-            [0, "cmdoption-osxphotos-export-export-by-date"]
-        ],
-        "--export-dir": [
-            [0, "cmdoption-osxphotos-exportdb-export-dir"]
-        ],
-        "--exportdb": [
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-export-exportdb"]
-        ],
-        "--external-edit": [
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-sync-external-edit"]
-        ],
-        "--favorite": [
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-sync-favorite"]
-        ],
-        "--favorite-rating": [
-            [0, "cmdoption-osxphotos-export-favorite-rating"]
-        ],
-        "--field": [
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-query-f"]
-        ],
-        "--filename": [
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "--finder-tag-keywords": [
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
-        ],
-        "--finder-tag-template": [
-            [0, "cmdoption-osxphotos-export-finder-tag-template"]
-        ],
-        "--folder": [
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-sync-folder"]
-        ],
-        "--force": [
-            [0, "cmdoption-osxphotos-timewarp-force"]
-        ],
-        "--force-update": [
-            [0, "cmdoption-osxphotos-export-force-update"]
-        ],
-        "--from-date": [
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-date"]
-        ],
-        "--from-time": [
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-sync-from-time"]
-        ],
-        "--function": [
-            [0, "cmdoption-osxphotos-timewarp-F"]
-        ],
-        "--glob": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "--has-comment": [
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-comment"]
-        ],
-        "--has-likes": [
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-likes"]
-        ],
-        "--has-raw": [
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-sync-has-raw"]
-        ],
-        "--hdr": [
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-sync-hdr"]
-        ],
-        "--help": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "--hidden": [
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-sync-hidden"]
-        ],
-        "--ignore-case": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"]
-        ],
-        "--ignore-date-modified": [
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
-        ],
-        "--ignore-signature": [
-            [0, "cmdoption-osxphotos-export-ignore-signature"]
-        ],
-        "--import": [
-            [0, "cmdoption-osxphotos-sync-i"]
-        ],
-        "--in-album": [
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-sync-in-album"]
-        ],
-        "--incloud": [
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-sync-incloud"]
-        ],
-        "--info": [
-            [0, "cmdoption-osxphotos-exportdb-info"]
-        ],
-        "--inspect": [
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "--is-reference": [
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-sync-is-reference"]
-        ],
-        "--jpeg-ext": [
-            [0, "cmdoption-osxphotos-export-jpeg-ext"]
-        ],
-        "--jpeg-quality": [
-            [0, "cmdoption-osxphotos-export-jpeg-quality"]
-        ],
-        "--json": [
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-list-json"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-query-json"]
-        ],
-        "--keep": [
-            [0, "cmdoption-osxphotos-export-keep"]
-        ],
-        "--keyword": [
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-sync-keyword"]
-        ],
-        "--keyword-template": [
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-export-keyword-template"]
-        ],
-        "--label": [
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-sync-label"]
-        ],
-        "--last-errors": [
-            [0, "cmdoption-osxphotos-exportdb-last-errors"]
-        ],
-        "--last-run": [
-            [0, "cmdoption-osxphotos-exportdb-last-run"]
-        ],
-        "--library": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-timewarp-L"]
-        ],
-        "--limit": [
-            [0, "cmdoption-osxphotos-export-limit"]
-        ],
-        "--list": [
-            [0, "cmdoption-osxphotos-theme-list"]
-        ],
-        "--live": [
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-sync-live"]
-        ],
-        "--load-config": [
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-export-load-config"]
-        ],
-        "--location": [
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-sync-location"]
-        ],
-        "--match-time": [
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "--max-size": [
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-sync-max-size"]
-        ],
-        "--merge": [
-            [0, "cmdoption-osxphotos-sync-m"]
-        ],
-        "--merge-keywords": [
-            [0, "cmdoption-osxphotos-import-m"]
-        ],
-        "--migrate": [
-            [0, "cmdoption-osxphotos-exportdb-migrate"]
-        ],
-        "--migrate-photos-library": [
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
-        ],
-        "--min-size": [
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"]
-        ],
-        "--missing": [
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-sync-missing"]
-        ],
-        "--name": [
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-sync-name"]
-        ],
-        "--no-comment": [
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-comment"]
-        ],
-        "--no-description": [
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-description"]
-        ],
-        "--no-keyword": [
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"]
-        ],
-        "--no-likes": [
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-likes"]
-        ],
-        "--no-location": [
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-location"]
-        ],
-        "--no-place": [
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-place"]
-        ],
-        "--no-progress": [
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-import-no-progress"]
-        ],
-        "--no-title": [
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-sync-no-title"]
-        ],
-        "--not-burst": [
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-burst"]
-        ],
-        "--not-cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
-        ],
-        "--not-edited": [
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-edited"]
-        ],
-        "--not-favorite": [
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"]
-        ],
-        "--not-hdr": [
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"]
-        ],
-        "--not-hidden": [
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"]
-        ],
-        "--not-in-album": [
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"]
-        ],
-        "--not-incloud": [
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"]
-        ],
-        "--not-live": [
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-live"]
-        ],
-        "--not-missing": [
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-missing"]
-        ],
-        "--not-panorama": [
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"]
-        ],
-        "--not-portrait": [
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"]
-        ],
-        "--not-reference": [
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-reference"]
-        ],
-        "--not-saved-to-library": [
-            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-not-saved-to-library"]
-        ],
-        "--not-screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"]
-        ],
-        "--not-selfie": [
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"]
-        ],
-        "--not-shared": [
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-shared"]
-        ],
-        "--not-slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
-        ],
-        "--not-syndicated": [
-            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
-            [0, "cmdoption-osxphotos-export-not-syndicated"],
-            [0, "cmdoption-osxphotos-query-not-syndicated"],
-            [0, "cmdoption-osxphotos-repl-not-syndicated"],
-            [0, "cmdoption-osxphotos-sync-not-syndicated"]
-        ],
-        "--not-time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
-        ],
-        "--only-movies": [
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-movies"]
-        ],
-        "--only-new": [
-            [0, "cmdoption-osxphotos-export-only-new"]
-        ],
-        "--only-photos": [
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-sync-only-photos"]
-        ],
-        "--original-suffix": [
-            [0, "cmdoption-osxphotos-export-original-suffix"]
-        ],
-        "--overwrite": [
-            [0, "cmdoption-osxphotos-export-overwrite"]
-        ],
-        "--panorama": [
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-sync-panorama"]
-        ],
-        "--parse-date": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-M"]
-        ],
-        "--person": [
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-sync-person"]
-        ],
-        "--person-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-export-person-keyword"]
-        ],
-        "--place": [
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-sync-place"]
-        ],
-        "--plain": [
-            [0, "cmdoption-osxphotos-timewarp-plain"]
-        ],
-        "--portrait": [
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-sync-portrait"]
-        ],
-        "--post-command": [
-            [0, "cmdoption-osxphotos-export-post-command"]
-        ],
-        "--post-function": [
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-import-post-function"]
-        ],
-        "--preview": [
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "--preview-if-missing": [
-            [0, "cmdoption-osxphotos-export-preview-if-missing"]
-        ],
-        "--preview-suffix": [
-            [0, "cmdoption-osxphotos-export-preview-suffix"]
-        ],
-        "--print": [
-            [0, "cmdoption-osxphotos-dump-print"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-query-print"]
-        ],
-        "--pull-exif": [
-            [0, "cmdoption-osxphotos-timewarp-P"]
-        ],
-        "--push-exif": [
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "--query-eval": [
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-eval"]
-        ],
-        "--query-function": [
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-sync-query-function"]
-        ],
-        "--quiet": [
-            [0, "cmdoption-osxphotos-query-quiet"]
-        ],
-        "--ramdb": [
-            [0, "cmdoption-osxphotos-export-ramdb"]
-        ],
-        "--raw-output": [
-            [0, "cmdoption-osxphotos-diff-r"]
-        ],
-        "--regex": [
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-sync-regex"]
-        ],
-        "--relative-to": [
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "--replace-keywords": [
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"]
-        ],
-        "--report": [
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-sync-R"]
-        ],
-        "--resume": [
-            [0, "cmdoption-osxphotos-import-R"]
-        ],
-        "--retry": [
-            [0, "cmdoption-osxphotos-export-retry"]
-        ],
-        "--run": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
-        "--save-config": [
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"]
-        ],
-        "--saved-to-library": [
-            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-saved-to-library"]
-        ],
-        "--screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-sync-screenshot"]
-        ],
-        "--selected": [
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-sync-selected"]
-        ],
-        "--selfie": [
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-sync-selfie"]
-        ],
-        "--set": [
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "--shared": [
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-repl-shared"]
-        ],
-        "--sidecar": [
-            [0, "cmdoption-osxphotos-export-sidecar"]
-        ],
-        "--sidecar-drop-ext": [
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
-        ],
-        "--skip-bursts": [
-            [0, "cmdoption-osxphotos-export-skip-bursts"]
-        ],
-        "--skip-edited": [
-            [0, "cmdoption-osxphotos-export-skip-edited"]
-        ],
-        "--skip-live": [
-            [0, "cmdoption-osxphotos-export-skip-live"]
-        ],
-        "--skip-original-if-edited": [
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
-        ],
-        "--skip-raw": [
-            [0, "cmdoption-osxphotos-export-skip-raw"]
-        ],
-        "--skip-uuid": [
-            [0, "cmdoption-osxphotos-export-skip-uuid"]
-        ],
-        "--skip-uuid-from-file": [
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
-        ],
-        "--slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"]
-        ],
-        "--split-folder": [
-            [0, "cmdoption-osxphotos-import-f"]
-        ],
-        "--sql": [
-            [0, "cmdoption-osxphotos-exportdb-sql"]
-        ],
-        "--strip": [
-            [0, "cmdoption-osxphotos-export-strip"]
-        ],
-        "--style": [
-            [0, "cmdoption-osxphotos-diff-s"]
-        ],
-        "--syndicated": [
-            [0, "cmdoption-osxphotos-add-locations-syndicated"],
-            [0, "cmdoption-osxphotos-export-syndicated"],
-            [0, "cmdoption-osxphotos-query-syndicated"],
-            [0, "cmdoption-osxphotos-repl-syndicated"],
-            [0, "cmdoption-osxphotos-sync-syndicated"]
-        ],
-        "--template": [
-            [0, "cmdoption-osxphotos-inspect-T"]
-        ],
-        "--theme": [
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-inspect-theme"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-timewarp-theme"]
-        ],
-        "--time": [
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "--time-delta": [
-            [0, "cmdoption-osxphotos-timewarp-T"]
-        ],
-        "--time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"]
-        ],
-        "--timestamp": [
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-diff-timestamp"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"]
-        ],
-        "--timezone": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "--title": [
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-sync-title"]
-        ],
-        "--tmpdir": [
-            [0, "cmdoption-osxphotos-export-tmpdir"]
-        ],
-        "--to-date": [
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-date"]
-        ],
-        "--to-time": [
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-sync-to-time"]
-        ],
-        "--touch-file": [
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"]
-        ],
-        "--undo": [
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "--unmatched": [
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "--update": [
-            [0, "cmdoption-osxphotos-export-update"]
-        ],
-        "--update-errors": [
-            [0, "cmdoption-osxphotos-export-update-errors"]
-        ],
-        "--update-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
-        ],
-        "--upgrade": [
-            [0, "cmdoption-osxphotos-install-U"]
-        ],
-        "--use-file-time": [
-            [0, "cmdoption-osxphotos-timewarp-1"]
-        ],
-        "--use-photokit": [
-            [0, "cmdoption-osxphotos-export-use-photokit"]
-        ],
-        "--use-photos-export": [
-            [0, "cmdoption-osxphotos-export-use-photos-export"]
-        ],
-        "--uti": [
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-sync-uti"]
-        ],
-        "--uuid": [
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid"]
-        ],
-        "--uuid-files": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
-        ],
-        "--uuid-from-file": [
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
-        ],
-        "--uuid-info": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
-        ],
-        "--vacuum": [
-            [0, "cmdoption-osxphotos-exportdb-vacuum"]
-        ],
-        "--verbose": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"]
-        ],
-        "--version": [
-            [0, "cmdoption-osxphotos-exportdb-version"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "--walk": [
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "--window": [
-            [0, "cmdoption-osxphotos-add-locations-w"]
-        ],
-        "--xattr-template": [
-            [0, "cmdoption-osxphotos-export-xattr-template"]
-        ],
-        "--year": [
-            [0, "cmdoption-osxphotos-add-locations-year"],
-            [0, "cmdoption-osxphotos-export-year"],
-            [0, "cmdoption-osxphotos-query-year"],
-            [0, "cmdoption-osxphotos-repl-year"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "--yes": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-a": [
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "-c": [
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "-d": [
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "-f": [
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "-l": [
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-import-l"]
-        ],
-        "-m": [
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "-p": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "-r": [
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "-t": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "-u": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "-v": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "-e": [
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "-g": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "-h": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "-i": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "-k": [
-            [0, "cmdoption-osxphotos-import-k"]
-        ],
-        "-s": [
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "-w": [
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "-y": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-z": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "args": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"]
-        ],
-        "db2": [
-            [0, "cmdoption-osxphotos-diff-arg-DB2"]
-        ],
-        "dest": [
-            [0, "cmdoption-osxphotos-export-arg-DEST"]
-        ],
-        "export_database": [
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
-        ],
-        "export_directory": [
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
-        ],
-        "files": [
-            [0, "cmdoption-osxphotos-import-arg-FILES"]
-        ],
-        "packages": [
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
-        ],
-        "photos_library": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
-        ],
-        "python_file": [
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
-        ],
-        "subtopic": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
-        ],
-        "topic": [
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "uuid_or_name": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
-        ],
-        "width": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos command line option": [
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "osxphotos-add-locations command line option": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-syndicated"],
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-add-locations-year"]
-        ],
-        "osxphotos-albums command line option": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-albums-library"]
-        ],
-        "osxphotos-batch-edit command line option": [
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "osxphotos-diff command line option": [
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-diff-arg-DB2"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-diff-timestamp"]
-        ],
-        "osxphotos-dump command line option": [
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-dump-print"]
-        ],
-        "osxphotos-exiftool command line option": [
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
-            [0, "cmdoption-osxphotos-exiftool-db-config"],
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"]
-        ],
-        "osxphotos-export command line option": [
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-export-album-keyword"],
-            [0, "cmdoption-osxphotos-export-alt-copy"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-export-arg-DEST"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-export-cleanup"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-export-config-only"],
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
-            [0, "cmdoption-osxphotos-export-current-name"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-export-description-template"],
-            [0, "cmdoption-osxphotos-export-directory"],
-            [0, "cmdoption-osxphotos-export-download-missing"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-export-edited-suffix"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
-            [0, "cmdoption-osxphotos-export-export-by-date"],
-            [0, "cmdoption-osxphotos-export-exportdb"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite-rating"],
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
-            [0, "cmdoption-osxphotos-export-finder-tag-template"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-export-force-update"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-signature"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-export-jpeg-ext"],
-            [0, "cmdoption-osxphotos-export-jpeg-quality"],
-            [0, "cmdoption-osxphotos-export-keep"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword-template"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-export-limit"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-export-load-config"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-syndicated"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-new"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-export-original-suffix"],
-            [0, "cmdoption-osxphotos-export-overwrite"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-export-person-keyword"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-export-post-command"],
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-export-preview-if-missing"],
-            [0, "cmdoption-osxphotos-export-preview-suffix"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-export-ramdb"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-export-retry"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-export-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-export-sidecar"],
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
-            [0, "cmdoption-osxphotos-export-skip-bursts"],
-            [0, "cmdoption-osxphotos-export-skip-edited"],
-            [0, "cmdoption-osxphotos-export-skip-live"],
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
-            [0, "cmdoption-osxphotos-export-skip-raw"],
-            [0, "cmdoption-osxphotos-export-skip-uuid"],
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-export-strip"],
-            [0, "cmdoption-osxphotos-export-syndicated"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-export-tmpdir"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-export-update"],
-            [0, "cmdoption-osxphotos-export-update-errors"],
-            [0, "cmdoption-osxphotos-export-use-photokit"],
-            [0, "cmdoption-osxphotos-export-use-photos-export"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-xattr-template"],
-            [0, "cmdoption-osxphotos-export-year"]
-        ],
-        "osxphotos-exportdb command line option": [
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-delete-file"],
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-errors"],
-            [0, "cmdoption-osxphotos-exportdb-export-dir"],
-            [0, "cmdoption-osxphotos-exportdb-info"],
-            [0, "cmdoption-osxphotos-exportdb-last-errors"],
-            [0, "cmdoption-osxphotos-exportdb-last-run"],
-            [0, "cmdoption-osxphotos-exportdb-migrate"],
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-sql"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
-            [0, "cmdoption-osxphotos-exportdb-vacuum"],
-            [0, "cmdoption-osxphotos-exportdb-version"]
-        ],
-        "osxphotos-help command line option": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "osxphotos-import command line option": [
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-import-arg-FILES"],
-            [0, "cmdoption-osxphotos-import-check-templates"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-import-g"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-import-no-progress"],
-            [0, "cmdoption-osxphotos-import-post-function"],
-            [0, "cmdoption-osxphotos-import-r"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "osxphotos-info command line option": [
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-info-library"]
-        ],
-        "osxphotos-inspect command line option": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-inspect-theme"]
-        ],
-        "osxphotos-install command line option": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
-        ],
-        "osxphotos-keywords command line option": [
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-keywords-library"]
-        ],
-        "osxphotos-labels command line option": [
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-labels-library"]
-        ],
-        "osxphotos-list command line option": [
-            [0, "cmdoption-osxphotos-list-json"]
-        ],
-        "osxphotos-orphans command line option": [
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"]
-        ],
-        "osxphotos-persons command line option": [
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-persons-library"]
-        ],
-        "osxphotos-places command line option": [
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-places-library"]
-        ],
-        "osxphotos-query command line option": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-query-count"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-query-json"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-syndicated"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-query-print"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-query-quiet"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-query-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-query-syndicated"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-year"]
-        ],
-        "osxphotos-repl command line option": [
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-repl-emacs"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-syndicated"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-repl-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-repl-shared"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-syndicated"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-year"]
-        ],
-        "osxphotos-run command line option": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"],
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "osxphotos-show command line option": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
-            [0, "cmdoption-osxphotos-show-library"]
-        ],
-        "osxphotos-snap command line option": [
-            [0, "cmdoption-osxphotos-snap-library"]
-        ],
-        "osxphotos-sync command line option": [
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-sync-U"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-sync-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-album"],
-            [0, "cmdoption-osxphotos-sync-burst"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-description"],
-            [0, "cmdoption-osxphotos-sync-dry-run"],
-            [0, "cmdoption-osxphotos-sync-duplicate"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-sync-edited"],
-            [0, "cmdoption-osxphotos-sync-exif"],
-            [0, "cmdoption-osxphotos-sync-external-edit"],
-            [0, "cmdoption-osxphotos-sync-favorite"],
-            [0, "cmdoption-osxphotos-sync-folder"],
-            [0, "cmdoption-osxphotos-sync-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-time"],
-            [0, "cmdoption-osxphotos-sync-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-raw"],
-            [0, "cmdoption-osxphotos-sync-hdr"],
-            [0, "cmdoption-osxphotos-sync-hidden"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-sync-in-album"],
-            [0, "cmdoption-osxphotos-sync-incloud"],
-            [0, "cmdoption-osxphotos-sync-is-reference"],
-            [0, "cmdoption-osxphotos-sync-keyword"],
-            [0, "cmdoption-osxphotos-sync-label"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-sync-live"],
-            [0, "cmdoption-osxphotos-sync-location"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-sync-max-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"],
-            [0, "cmdoption-osxphotos-sync-missing"],
-            [0, "cmdoption-osxphotos-sync-name"],
-            [0, "cmdoption-osxphotos-sync-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-title"],
-            [0, "cmdoption-osxphotos-sync-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-syndicated"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-photos"],
-            [0, "cmdoption-osxphotos-sync-panorama"],
-            [0, "cmdoption-osxphotos-sync-person"],
-            [0, "cmdoption-osxphotos-sync-place"],
-            [0, "cmdoption-osxphotos-sync-portrait"],
-            [0, "cmdoption-osxphotos-sync-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-function"],
-            [0, "cmdoption-osxphotos-sync-regex"],
-            [0, "cmdoption-osxphotos-sync-s"],
-            [0, "cmdoption-osxphotos-sync-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-screenshot"],
-            [0, "cmdoption-osxphotos-sync-selected"],
-            [0, "cmdoption-osxphotos-sync-selfie"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-syndicated"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-sync-title"],
-            [0, "cmdoption-osxphotos-sync-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-time"],
-            [0, "cmdoption-osxphotos-sync-uti"],
-            [0, "cmdoption-osxphotos-sync-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "osxphotos-theme command line option": [
-            [0, "cmdoption-osxphotos-theme-clone"],
-            [0, "cmdoption-osxphotos-theme-config"],
-            [0, "cmdoption-osxphotos-theme-default"],
-            [0, "cmdoption-osxphotos-theme-delete"],
-            [0, "cmdoption-osxphotos-theme-edit"],
-            [0, "cmdoption-osxphotos-theme-list"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "osxphotos-timewarp command line option": [
-            [0, "cmdoption-osxphotos-timewarp-0"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-timewarp-a"],
-            [0, "cmdoption-osxphotos-timewarp-c"],
-            [0, "cmdoption-osxphotos-timewarp-d"],
-            [0, "cmdoption-osxphotos-timewarp-date-added"],
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
-            [0, "cmdoption-osxphotos-timewarp-e"],
-            [0, "cmdoption-osxphotos-timewarp-force"],
-            [0, "cmdoption-osxphotos-timewarp-i"],
-            [0, "cmdoption-osxphotos-timewarp-p"],
-            [0, "cmdoption-osxphotos-timewarp-plain"],
-            [0, "cmdoption-osxphotos-timewarp-t"],
-            [0, "cmdoption-osxphotos-timewarp-theme"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "osxphotos-tutorial command line option": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos-uninstall command line option": [
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "osxphotos-uuid command line option": [
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "osxphotos-version command line option": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
-        "albuminfo (class in osxphotos)": [
-            [4, "osxphotos.AlbumInfo"]
-        ],
-        "albumsortorder (class in osxphotos)": [
-            [4, "osxphotos.AlbumSortOrder"]
-        ],
-        "commentinfo (class in osxphotos)": [
-            [4, "osxphotos.CommentInfo"]
-        ],
-        "exifinfo (class in osxphotos)": [
-            [4, "osxphotos.ExifInfo"]
-        ],
-        "exiftool (class in osxphotos)": [
-            [4, "osxphotos.ExifTool"]
-        ],
-        "exportdb (class in osxphotos)": [
-            [4, "osxphotos.ExportDB"]
-        ],
-        "exportdbtemp (class in osxphotos)": [
-            [4, "osxphotos.ExportDBTemp"]
-        ],
-        "exportoptions (class in osxphotos)": [
-            [4, "osxphotos.ExportOptions"]
-        ],
-        "exportresults (class in osxphotos)": [
-            [4, "osxphotos.ExportResults"]
-        ],
-        "fileutil (class in osxphotos)": [
-            [4, "osxphotos.FileUtil"]
-        ],
-        "fileutilnoop (class in osxphotos)": [
-            [4, "osxphotos.FileUtilNoOp"]
-        ],
-        "folderinfo (class in osxphotos)": [
-            [4, "osxphotos.FolderInfo"]
-        ],
-        "importinfo (class in osxphotos)": [
-            [4, "osxphotos.ImportInfo"]
-        ],
-        "likeinfo (class in osxphotos)": [
-            [4, "osxphotos.LikeInfo"]
-        ],
-        "momentinfo (class in osxphotos)": [
-            [4, "osxphotos.MomentInfo"]
-        ],
-        "personinfo (class in osxphotos)": [
-            [4, "osxphotos.PersonInfo"]
-        ],
-        "photoexporter (class in osxphotos)": [
-            [4, "osxphotos.PhotoExporter"]
-        ],
-        "photoinfo (class in osxphotos)": [
-            [4, "osxphotos.PhotoInfo"]
-        ],
-        "phototemplate (class in osxphotos)": [
-            [4, "osxphotos.PhotoTemplate"]
-        ],
-        "photosalbum (class in osxphotos)": [
-            [4, "osxphotos.PhotosAlbum"]
-        ],
-        "photosalbumphotoscript (class in osxphotos)": [
-            [4, "osxphotos.PhotosAlbumPhotoScript"]
-        ],
-        "photosdb (class in osxphotos)": [
-            [4, "osxphotos.PhotosDB"]
-        ],
-        "placeinfo (class in osxphotos)": [
-            [4, "osxphotos.PlaceInfo"]
-        ],
-        "projectinfo (class in osxphotos)": [
-            [4, "osxphotos.ProjectInfo"]
-        ],
-        "queryoptions (class in osxphotos)": [
-            [4, "osxphotos.QueryOptions"]
-        ],
-        "scoreinfo (class in osxphotos)": [
-            [4, "osxphotos.ScoreInfo"]
-        ],
-        "searchinfo (class in osxphotos)": [
-            [4, "osxphotos.SearchInfo"]
-        ],
-        "activities (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.activities"]
-        ],
-        "added_after (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_after"]
-        ],
-        "added_before (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_before"]
-        ],
-        "added_in_last (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_in_last"]
-        ],
-        "addvalues() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.addvalues"]
-        ],
-        "adjustments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.adjustments"]
-        ],
-        "album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.album"]
-        ],
-        "album_info (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.album_info"]
-        ],
-        "album_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.album_info"]
-        ],
-        "album_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.album_info"]
-        ],
-        "album_info_shared (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.album_info_shared"]
-        ],
-        "albums (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.albums"]
-        ],
-        "albums (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums"]
-        ],
-        "albums_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_as_dict"]
-        ],
-        "albums_shared (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_shared"]
-        ],
-        "albums_shared_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_shared_as_dict"]
-        ],
-        "all (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.all"]
-        ],
-        "all_files() (osxphotos.exportresults method)": [
-            [4, "osxphotos.ExportResults.all_files"]
-        ],
-        "asdict() (osxphotos.albuminfo method)": [
-            [4, "osxphotos.AlbumInfo.asdict"]
-        ],
-        "asdict() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.asdict"]
-        ],
-        "asdict() (osxphotos.folderinfo method)": [
-            [4, "osxphotos.FolderInfo.asdict"]
-        ],
-        "asdict() (osxphotos.importinfo method)": [
-            [4, "osxphotos.ImportInfo.asdict"]
-        ],
-        "asdict() (osxphotos.momentinfo method)": [
-            [4, "osxphotos.MomentInfo.asdict"]
-        ],
-        "asdict() (osxphotos.personinfo method)": [
-            [4, "osxphotos.PersonInfo.asdict"]
-        ],
-        "asdict() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.asdict"]
-        ],
-        "asdict() (osxphotos.scoreinfo method)": [
-            [4, "osxphotos.ScoreInfo.asdict"]
-        ],
-        "asdict() (osxphotos.searchinfo method)": [
-            [4, "osxphotos.SearchInfo.asdict"]
-        ],
-        "attributes (osxphotos.exportresults property)": [
-            [4, "osxphotos.ExportResults.attributes"]
-        ],
-        "bit_flags (osxphotos.exportoptions property)": [
-            [4, "osxphotos.ExportOptions.bit_flags"]
-        ],
-        "bodies_of_water (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.bodies_of_water"]
-        ],
-        "burst (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst"]
-        ],
-        "burst (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.burst"]
-        ],
-        "burst_album_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_album_info"]
-        ],
-        "burst_albums (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_albums"]
-        ],
-        "burst_default_pick (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_default_pick"]
-        ],
-        "burst_key (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_key"]
-        ],
-        "burst_photos (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_photos"]
-        ],
-        "burst_photos (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.burst_photos"]
-        ],
-        "burst_selected (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_selected"]
-        ],
-        "camera (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.camera"]
-        ],
-        "city (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.city"]
-        ],
-        "close() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.close"]
-        ],
-        "cloud_guid (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_guid"]
-        ],
-        "cloud_metadata (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_metadata"]
-        ],
-        "cloud_owner_hashed_id (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_owner_hashed_id"]
-        ],
-        "cloudasset (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.cloudasset"]
-        ],
-        "comments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.comments"]
-        ],
-        "connection (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.connection"]
-        ],
-        "convert_to_jpeg (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.convert_to_jpeg"]
-        ],
-        "convert_to_jpeg() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.convert_to_jpeg"]
-        ],
-        "copy() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.copy"]
-        ],
-        "country (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.country"]
-        ],
-        "create_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.create_file_record"]
-        ],
-        "create_or_get_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.create_or_get_file_record"]
-        ],
-        "date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.date"]
-        ],
-        "date (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date"]
-        ],
-        "date_added (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_added"]
-        ],
-        "date_modified (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_modified"]
-        ],
-        "date_trashed (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_trashed"]
-        ],
-        "datetime (osxphotos.exportresults property)": [
-            [4, "osxphotos.ExportResults.datetime"]
-        ],
-        "db_path (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.db_path"]
-        ],
-        "db_version (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.db_version"]
-        ],
-        "delete_data_for_filepath() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.delete_data_for_filepath"]
-        ],
-        "delete_data_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.delete_data_for_uuid"]
-        ],
-        "deleted (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.deleted"]
-        ],
-        "deleted_only (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.deleted_only"]
-        ],
-        "description (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.description"]
-        ],
-        "description (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.description"]
-        ],
-        "description_template (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.description_template"]
-        ],
-        "detected_text (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.detected_text"]
-        ],
-        "detected_text() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.detected_text"]
-        ],
-        "download_missing (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.download_missing"]
-        ],
-        "dry_run (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.dry_run"]
-        ],
-        "duplicate (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.duplicate"]
-        ],
-        "duplicates (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.duplicates"]
-        ],
-        "edited (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.edited"]
-        ],
-        "edited (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.edited"]
-        ],
-        "end_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.end_date"]
-        ],
-        "execute() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.execute"]
-        ],
-        "exif (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.exif"]
-        ],
-        "exif_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.exif_info"]
-        ],
-        "exiftool (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.exiftool"]
-        ],
-        "exiftool (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.exiftool"]
-        ],
-        "exiftool_flags (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.exiftool_flags"]
-        ],
-        "exiftool_json_sidecar() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.exiftool_json_sidecar"]
-        ],
-        "expand_variables() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.expand_variables"]
-        ],
-        "expand_variables_to_str() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.expand_variables_to_str"]
-        ],
-        "export() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.export"]
-        ],
-        "export() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.export"]
-        ],
-        "export_as_hardlink (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.export_as_hardlink"]
-        ],
-        "export_db (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.export_db"]
-        ],
-        "export_dir (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.export_dir"]
-        ],
-        "external_edit (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.external_edit"]
-        ],
-        "external_edit (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.external_edit"]
-        ],
-        "face_info (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.face_info"]
-        ],
-        "face_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.face_info"]
-        ],
-        "face_regions (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.face_regions"]
-        ],
-        "favorite (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.favorite"]
-        ],
-        "favorite (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.favorite"]
-        ],
-        "favorite (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.favorite"]
-        ],
-        "favorite_rating (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.favorite_rating"]
-        ],
-        "feature_less (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.feature_less"]
-        ],
-        "file_sig() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.file_sig"]
-        ],
-        "filename (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.filename"]
-        ],
-        "fileutil (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.fileutil"]
-        ],
-        "filter_predicate() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.filter_predicate"]
-        ],
-        "fingerprint (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.fingerprint"]
-        ],
-        "folder (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.folder"]
-        ],
-        "folder_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.folder_info"]
-        ],
-        "folder_list (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.folder_list"]
-        ],
-        "folder_list (osxphotos.projectinfo property)": [
-            [4, "osxphotos.ProjectInfo.folder_list"]
-        ],
-        "folder_names (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.folder_names"]
-        ],
-        "folder_names (osxphotos.projectinfo property)": [
-            [4, "osxphotos.ProjectInfo.folder_names"]
-        ],
-        "folders (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.folders"]
-        ],
-        "force_update (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.force_update"]
-        ],
-        "from_date (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.from_date"]
-        ],
-        "function (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.function"]
-        ],
-        "get_db_connection() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.get_db_connection"]
-        ],
-        "get_export_results() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_export_results"]
-        ],
-        "get_exported_files() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_exported_files"]
-        ],
-        "get_field_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_field_values"]
-        ],
-        "get_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_file_record"]
-        ],
-        "get_files_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_files_for_uuid"]
-        ],
-        "get_filter_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_filter_values"]
-        ],
-        "get_format_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_format_values"]
-        ],
-        "get_media_type() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_media_type"]
-        ],
-        "get_photo() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.get_photo"]
-        ],
-        "get_photo_bool_attribute() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_photo_bool_attribute"]
-        ],
-        "get_photo_video_type() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_photo_video_type"]
-        ],
-        "get_photoinfo_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_photoinfo_for_uuid"]
-        ],
-        "get_previous_uuids() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_previous_uuids"]
-        ],
-        "get_target_for_file() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_target_for_file"]
-        ],
-        "get_template_value() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value"]
-        ],
-        "get_template_value_exiftool() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_exiftool"]
-        ],
-        "get_template_value_filter_function() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_filter_function"]
-        ],
-        "get_template_value_function() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_function"]
-        ],
-        "get_template_value_multi() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_multi"]
-        ],
-        "get_template_value_pathlib() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_pathlib"]
-        ],
-        "get_uuid_for_file() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_uuid_for_file"]
-        ],
-        "hardlink() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.hardlink"]
-        ],
-        "has_comment (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_comment"]
-        ],
-        "has_likes (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_likes"]
-        ],
-        "has_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.has_raw"]
-        ],
-        "has_raw (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_raw"]
-        ],
-        "hasadjustments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hasadjustments"]
-        ],
-        "hdr (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hdr"]
-        ],
-        "hdr (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.hdr"]
-        ],
-        "height (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.height"]
-        ],
-        "hexdigest (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hexdigest"]
-        ],
-        "hidden (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hidden"]
-        ],
-        "hidden (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.hidden"]
-        ],
-        "holidays (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.holidays"]
-        ],
-        "ignore_case (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.ignore_case"]
-        ],
-        "ignore_date_modified (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.ignore_date_modified"]
-        ],
-        "ignore_signature (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.ignore_signature"]
-        ],
-        "import_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.import_info"]
-        ],
-        "import_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.import_info"]
-        ],
-        "in_album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.in_album"]
-        ],
-        "incloud (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.incloud"]
-        ],
-        "incloud (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.incloud"]
-        ],
-        "increment (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.increment"]
-        ],
-        "intrash (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.intrash"]
-        ],
-        "is_debug() (in module osxphotos)": [
-            [4, "osxphotos.is_debug"]
-        ],
-        "is_reference (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.is_reference"]
-        ],
-        "iscloudasset (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.iscloudasset"]
-        ],
-        "ismissing (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.ismissing"]
-        ],
-        "ismovie (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.ismovie"]
-        ],
-        "isphoto (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.isphoto"]
-        ],
-        "israw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.israw"]
-        ],
-        "isreference (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.isreference"]
-        ],
-        "jpeg_ext (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.jpeg_ext"]
-        ],
-        "jpeg_quality (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.jpeg_quality"]
-        ],
-        "json() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.json"]
-        ],
-        "json() (osxphotos.personinfo method)": [
-            [4, "osxphotos.PersonInfo.json"]
-        ],
-        "json() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.json"]
-        ],
-        "keyword (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.keyword"]
-        ],
-        "keyword_template (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.keyword_template"]
-        ],
-        "keywords (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.keywords"]
-        ],
-        "keywords (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.keywords"]
-        ],
-        "keywords_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.keywords_as_dict"]
-        ],
-        "label (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.label"]
-        ],
-        "labels (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.labels"]
-        ],
-        "labels (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels"]
-        ],
-        "labels (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.labels"]
-        ],
-        "labels_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_as_dict"]
-        ],
-        "labels_normalized (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.labels_normalized"]
-        ],
-        "labels_normalized (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_normalized"]
-        ],
-        "labels_normalized_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_normalized_as_dict"]
-        ],
-        "library_path (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.library_path"]
-        ],
-        "likes (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.likes"]
-        ],
-        "live (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.live"]
-        ],
-        "live_photo (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.live_photo"]
-        ],
-        "live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.live_photo"]
-        ],
-        "locality_names (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.locality_names"]
-        ],
-        "location (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.location"]
-        ],
-        "location (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.location"]
-        ],
-        "location (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.location"]
-        ],
-        "location (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.location"]
-        ],
-        "max_size (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.max_size"]
-        ],
-        "media_types (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.media_types"]
-        ],
-        "merge_exif_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.merge_exif_keywords"]
-        ],
-        "merge_exif_persons (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.merge_exif_persons"]
-        ],
-        "min_size (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.min_size"]
-        ],
-        "missing (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.missing"]
-        ],
-        "missing_bursts (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.missing_bursts"]
-        ],
-        "modification_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.modification_date"]
-        ],
-        "module": [
-            [4, "module-osxphotos"]
-        ],
-        "moment_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.moment_info"]
-        ],
-        "month (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.month"]
-        ],
-        "movies (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.movies"]
-        ],
-        "name (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.name"]
-        ],
-        "neighborhoods (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.neighborhoods"]
-        ],
-        "no_comment (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_comment"]
-        ],
-        "no_description (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_description"]
-        ],
-        "no_keyword (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_keyword"]
-        ],
-        "no_likes (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_likes"]
-        ],
-        "no_location (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_location"]
-        ],
-        "no_place (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_place"]
-        ],
-        "no_title (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_title"]
-        ],
-        "not_burst (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_burst"]
-        ],
-        "not_cloudasset (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_cloudasset"]
-        ],
-        "not_edited (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_edited"]
-        ],
-        "not_favorite (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_favorite"]
-        ],
-        "not_hdr (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_hdr"]
-        ],
-        "not_hidden (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_hidden"]
-        ],
-        "not_in_album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_in_album"]
-        ],
-        "not_incloud (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_incloud"]
-        ],
-        "not_live (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_live"]
-        ],
-        "not_missing (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_missing"]
-        ],
-        "not_panorama (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_panorama"]
-        ],
-        "not_portrait (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_portrait"]
-        ],
-        "not_reference (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_reference"]
-        ],
-        "not_saved_to_library (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_saved_to_library"]
-        ],
-        "not_screenshot (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_screenshot"]
-        ],
-        "not_selfie (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_selfie"]
-        ],
-        "not_shared (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_shared"]
-        ],
-        "not_slow_mo (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_slow_mo"]
-        ],
-        "not_syndicated (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_syndicated"]
-        ],
-        "not_time_lapse (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_time_lapse"]
-        ],
-        "orientation (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.orientation"]
-        ],
-        "original_filename (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_filename"]
-        ],
-        "original_filesize (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_filesize"]
-        ],
-        "original_height (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_height"]
-        ],
-        "original_orientation (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_orientation"]
-        ],
-        "original_width (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_width"]
-        ],
-        "osxphotos": [
-            [4, "module-osxphotos"]
-        ],
-        "overwrite (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.overwrite"]
-        ],
-        "owner (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.owner"]
-        ],
-        "panorama (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.panorama"]
-        ],
-        "panorama (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.panorama"]
-        ],
-        "parent (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.parent"]
-        ],
-        "parent (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.parent"]
-        ],
-        "path (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.path"]
-        ],
-        "path (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path"]
-        ],
-        "path_derivatives (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_derivatives"]
-        ],
-        "path_edited (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_edited"]
-        ],
-        "path_edited_live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_edited_live_photo"]
-        ],
-        "path_live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_live_photo"]
-        ],
-        "path_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_raw"]
-        ],
-        "person (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.person"]
-        ],
-        "person_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.person_info"]
-        ],
-        "person_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.person_info"]
-        ],
-        "persons (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.persons"]
-        ],
-        "persons (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.persons"]
-        ],
-        "persons (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.persons"]
-        ],
-        "persons_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.persons_as_dict"]
-        ],
-        "photo_index() (osxphotos.albuminfo method)": [
-            [4, "osxphotos.AlbumInfo.photo_index"]
-        ],
-        "photos (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.photos"]
-        ],
-        "photos (osxphotos.importinfo property)": [
-            [4, "osxphotos.ImportInfo.photos"]
-        ],
-        "photos (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.photos"]
-        ],
-        "photos (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.photos"]
-        ],
-        "photos (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.photos"]
-        ],
-        "photos() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.photos"]
-        ],
-        "photos_by_uuid() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.photos_by_uuid"]
-        ],
-        "photos_version (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.photos_version"]
-        ],
-        "pid (osxphotos.exiftool property)": [
-            [4, "osxphotos.ExifTool.pid"]
-        ],
-        "pk (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.pk"]
-        ],
-        "place (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.place"]
-        ],
-        "place (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.place"]
-        ],
-        "place_names (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.place_names"]
-        ],
-        "portrait (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.portrait"]
-        ],
-        "portrait (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.portrait"]
-        ],
-        "preview (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.preview"]
-        ],
-        "preview_suffix (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.preview_suffix"]
-        ],
-        "project_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.project_info"]
-        ],
-        "project_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.project_info"]
-        ],
-        "query() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.query"]
-        ],
-        "query_eval (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.query_eval"]
-        ],
-        "raw_original (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.raw_original"]
-        ],
-        "raw_photo (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.raw_photo"]
-        ],
-        "regex (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.regex"]
-        ],
-        "rename() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.rename"]
-        ],
-        "render() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.render"]
-        ],
-        "render_options (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.render_options"]
-        ],
-        "render_template() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.render_template"]
-        ],
-        "replace_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.replace_keywords"]
-        ],
-        "rich (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.rich"]
-        ],
-        "rmdir() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.rmdir"]
-        ],
-        "run_commands() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.run_commands"]
-        ],
-        "saved_to_library (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.saved_to_library"]
-        ],
-        "saved_to_library (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.saved_to_library"]
-        ],
-        "score (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.score"]
-        ],
-        "screenshot (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.screenshot"]
-        ],
-        "screenshot (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.screenshot"]
-        ],
-        "search_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.search_info"]
-        ],
-        "search_info_normalized (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.search_info_normalized"]
-        ],
-        "season (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.season"]
-        ],
-        "selected (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.selected"]
-        ],
-        "selfie (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.selfie"]
-        ],
-        "selfie (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.selfie"]
-        ],
-        "set_config() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_config"]
-        ],
-        "set_debug() (in module osxphotos)": [
-            [4, "osxphotos.set_debug"]
-        ],
-        "set_export_results() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_export_results"]
-        ],
-        "set_photoinfo_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_photoinfo_for_uuid"]
-        ],
-        "setvalue() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.setvalue"]
-        ],
-        "shared (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.shared"]
-        ],
-        "shared (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.shared"]
-        ],
-        "sidecar (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.sidecar"]
-        ],
-        "sidecar_drop_ext (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.sidecar_drop_ext"]
-        ],
-        "slow_mo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.slow_mo"]
-        ],
-        "slow_mo (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.slow_mo"]
-        ],
-        "sort_order (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.sort_order"]
-        ],
-        "sort_order (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.sort_order"]
-        ],
-        "source (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.source"]
-        ],
-        "start_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.start_date"]
-        ],
-        "state (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.state"]
-        ],
-        "state_abbreviation (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.state_abbreviation"]
-        ],
-        "streets (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.streets"]
-        ],
-        "strip (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.strip"]
-        ],
-        "subfolders (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.subfolders"]
-        ],
-        "subtitle (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.subtitle"]
-        ],
-        "syndicated (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.syndicated"]
-        ],
-        "syndicated (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.syndicated"]
-        ],
-        "tables() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.tables"]
-        ],
-        "text_found (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.text_found"]
-        ],
-        "time_lapse (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.time_lapse"]
-        ],
-        "time_lapse (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.time_lapse"]
-        ],
-        "timeout (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.timeout"]
-        ],
-        "title (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.title"]
-        ],
-        "title (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.title"]
-        ],
-        "title (osxphotos.importinfo property)": [
-            [4, "osxphotos.ImportInfo.title"]
-        ],
-        "title (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.title"]
-        ],
-        "title (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.title"]
-        ],
-        "title (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.title"]
-        ],
-        "tmpdir (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.tmpdir"]
-        ],
-        "tmpdir() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.tmpdir"]
-        ],
-        "to_date (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.to_date"]
-        ],
-        "touch_file (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.touch_file"]
-        ],
-        "tzoffset (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.tzoffset"]
-        ],
-        "unlink() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.unlink"]
-        ],
-        "update (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.update"]
-        ],
-        "update_errors (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.update_errors"]
-        ],
-        "use_albums_as_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_albums_as_keywords"]
-        ],
-        "use_persons_as_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_persons_as_keywords"]
-        ],
-        "use_photokit (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_photokit"]
-        ],
-        "use_photos_export (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_photos_export"]
-        ],
-        "uti (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti"]
-        ],
-        "uti (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.uti"]
-        ],
-        "uti_edited (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_edited"]
-        ],
-        "uti_original (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_original"]
-        ],
-        "uti_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_raw"]
-        ],
-        "utime() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.utime"]
-        ],
-        "uuid (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.uuid"]
-        ],
-        "uuid (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uuid"]
-        ],
-        "uuid (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.uuid"]
-        ],
-        "venue_types (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.venue_types"]
-        ],
-        "venues (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.venues"]
-        ],
-        "verbose (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.verbose"]
-        ],
-        "version (osxphotos.exiftool property)": [
-            [4, "osxphotos.ExifTool.version"]
-        ],
-        "visible (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.visible"]
-        ],
-        "width (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.width"]
-        ],
-        "write_exiftool_metadata_to_file() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.write_exiftool_metadata_to_file"]
-        ],
-        "year (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.year"]
-        ],
-        "year (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.year"]
-        ]
-    }
+    "indexentries": {}
 })
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.5’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.6’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.5â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.6â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.5 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.6 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.6_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.5/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.6/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/exifinfo.py` & `osxphotos-0.60.6/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/exiftool.py` & `osxphotos-0.60.6/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.6/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/export_db.py` & `osxphotos-0.60.6/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/export_db_utils.py` & `osxphotos-0.60.6/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/fileutil.py` & `osxphotos-0.60.6/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.6/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/imageconverter.py` & `osxphotos-0.60.6/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/momentinfo.py` & `osxphotos-0.60.6/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/path_utils.py` & `osxphotos-0.60.6/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/personinfo.py` & `osxphotos-0.60.6/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photodates.py` & `osxphotos-0.60.6/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photoexporter.py` & `osxphotos-0.60.6/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photoinfo.py` & `osxphotos-0.60.6/osxphotos/photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photokit.py` & `osxphotos-0.60.6/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosalbum.py` & `osxphotos-0.60.6/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photoscript_utils.py` & `osxphotos-0.60.6/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.6/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.6/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototables.py` & `osxphotos-0.60.6/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.6/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototemplate.md` & `osxphotos-0.60.6/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototemplate.py` & `osxphotos-0.60.6/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototemplate.tx` & `osxphotos-0.60.6/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/phototz.py` & `osxphotos-0.60.6/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/placeinfo.py` & `osxphotos-0.60.6/osxphotos/placeinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ 
     PlaceInfo class
     Provides reverse geolocation info for photos 
     
     See https://developer.apple.com/documentation/corelocation/clplacemark
     for additional documentation on reverse geolocation data
 """
+
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from collections import namedtuple  # pylint: disable=syntax-error
 
 import yaml
 from bpylist2 import archiver
 
 from .unicode import normalize_unicode
@@ -327,43 +330,107 @@
 archiver.update_class_map(
     {"PLRevGeoMapItemAdditionalPlaceInfo": PLRevGeoMapItemAdditionalPlaceInfo}
 )
 archiver.update_class_map({"PLRevGeoMapItem": PLRevGeoMapItem})
 archiver.update_class_map({"PLRevGeoLocationInfo": PLRevGeoLocationInfo})
 
 
-class PlaceInfo(ABC):
+# PlaceInfo is really an abstract base class but defining it as such
+# means it doesn't get picked up by the doc generation tools
+# so we define it as a regular class and then subclass it
+# TODO: right fix is probably have PlaceInfo as the only class that
+# is used and then have PlaceInfo4 and PlaceInfo5 called by PlaceInfo
+# as needed to return the properties (and make them private classes)
+
+
+class PlaceInfo:
+    """Reverse geolocation place info for a photo."""
+
     @property
-    @abstractmethod
-    def address_str(self):
+    def address_str(self) -> str | None:
+        """Returns the full postal address as a string if defined, otherwise `None`."""
         pass
 
     @property
-    @abstractmethod
-    def country_code(self):
+    def country_code(self) -> str | None:
+        """Returns the country_code of place, for example "GB".
+        Returns `None` if PhotoInfo contains no country code.
+        """
         pass
 
     @property
-    @abstractmethod
-    def ishome(self):
+    def ishome(self) -> bool:
+        """Returns `True` if photo place is user's home address, otherwise `False`."""
         pass
 
     @property
-    @abstractmethod
-    def name(self):
+    def name(self) -> str | None:
+        """Returns the name of the local place as str.
+        This is what Photos displays in the Info window.
+        **Note** Photos 5 uses a different algorithm to determine the name than earlier versions which means the same Photo may have a different place name in Photos 4 and Photos 5.
+        `PhotoInfo.name` will return the name Photos would have shown depending on the version of the library being processed.
+        Returns `None` if photo does not contain a name.
+        """
         pass
 
     @property
-    @abstractmethod
-    def names(self):
+    def names(self) -> PlaceNames | None:
+        """Returns a `PlaceNames` namedtuple with the following fields.
+        Each field is a list with zero or more values, sorted by area in ascending order.
+        E.g. `names.area_of_interest` could be ['Gulf Islands National Seashore', 'Santa Rosa Island'], ["Knott's Berry Farm"], or [] if `area_of_interest` not defined.
+        The value shown in Photos is the first value in the list. With the exception of `body_of_water` each of these field corresponds to an attribute of
+        a [CLPlacemark](https://developer.apple.com/documentation/corelocation/clplacemark) object.
+
+
+        * `country`; the name of the country associated with the placemark.
+        * `state_province`; administrativeArea, The state or province associated with the placemark.
+        * `sub_administrative_area`; additional administrative area information for the placemark.
+        * `city`; locality; the city associated with the placemark.
+        * `additional_city_info`; subLocality, Additional city-level information for the placemark.
+        * `ocean`; the name of the ocean associated with the placemark.
+        * `area_of_interest`; areasOfInterest, The relevant areas of interest associated with the placemark.
+        * `inland_water`; the name of the inland water body associated with the placemark.
+        * `region`; the geographic region associated with the placemark.
+        * `sub_throughfare`; additional street-level information for the placemark.
+        * `postal_code`; the postal code associated with the placemark.
+        * `street_address`; throughfare, The street address associated with the placemark.
+        * `body_of_water`; in Photos 4, any body of water; in Photos 5 contains the union of ocean and inland_water
+
+        **Note**: In Photos <= 4.0, only the following fields are defined; all others are set to empty list:
+
+        * `country`
+        * `state_province`
+        * `sub_administrative_area`
+        * `city`
+        * `additional_city_info`
+        * `area_of_interest`
+        * `body_of_water`
+
+        Note:
+            The `PlaceNames` namedtuple contains reserved fields not listed below (see implementation for details),
+            thus it should be referenced only by name (e.g. `names.city`) and not by index.
+        """
         pass
 
     @property
-    @abstractmethod
     def address(self):
+        """Returns a `PostalAddress` namedtuple with details of the postal address containing the following fields:
+
+        * `city`
+        * `country`
+        * `postal_code`
+        * `state`
+        * `street`
+        * `sub_administrative_area`
+        * `sub_locality`
+        * `iso_country_code`
+        """
+        pass
+
+    def asdict():
         pass
 
 
 class PlaceInfo4(PlaceInfo):
     """Reverse geolocation place info for a photo (Photos <= 4)"""
 
     def __init__(self, place_names, country_code):
```

### Comparing `osxphotos-0.60.5/osxphotos/platform.py` & `osxphotos-0.60.6/osxphotos/platform.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/pyrepl.py` & `osxphotos-0.60.6/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.6/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/query_builder.py` & `osxphotos-0.60.6/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/queryoptions.py` & `osxphotos-0.60.6/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/scoreinfo.py` & `osxphotos-0.60.6/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/searchinfo.py` & `osxphotos-0.60.6/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/sqlgrep.py` & `osxphotos-0.60.6/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/sqlite_utils.py` & `osxphotos-0.60.6/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.6/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/template_counter.py` & `osxphotos-0.60.6/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.6/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.6/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/text_detection.py` & `osxphotos-0.60.6/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/timeutils.py` & `osxphotos-0.60.6/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/timezones.py` & `osxphotos-0.60.6/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/tutorial.md` & `osxphotos-0.60.6/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/unicode.py` & `osxphotos-0.60.6/osxphotos/unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/uti.py` & `osxphotos-0.60.6/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos/utils.py` & `osxphotos-0.60.6/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.6/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.5
+Version: 0.60.6
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.5/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.6/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.6/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/setup.py` & `osxphotos-0.60.6/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_10_12_6.py` & `osxphotos-0.60.6/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.6/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.6/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.6/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.6/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli.py` & `osxphotos-0.60.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_add_locations.py` & `osxphotos-0.60.6/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_add_to_album.py` & `osxphotos-0.60.6/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_all_commands.py` & `osxphotos-0.60.6/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_batch_edit.py` & `osxphotos-0.60.6/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_dump.py` & `osxphotos-0.60.6/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_exiftool.py` & `osxphotos-0.60.6/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_export_cloud.py` & `osxphotos-0.60.6/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_export_projects.py` & `osxphotos-0.60.6/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_exportdb.py` & `osxphotos-0.60.6/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_import.py` & `osxphotos-0.60.6/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_orphans.py` & `osxphotos-0.60.6/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_param_types.py` & `osxphotos-0.60.6/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_sync.py` & `osxphotos-0.60.6/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_timewarp.py` & `osxphotos-0.60.6/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_utils.py` & `osxphotos-0.60.6/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cli_verbose.py` & `osxphotos-0.60.6/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.6/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_comments.py` & `osxphotos-0.60.6/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_concurrent_export.py` & `osxphotos-0.60.6/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_configoptions.py` & `osxphotos-0.60.6/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_datetime_formatter.py` & `osxphotos-0.60.6/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_datetime_utils.py` & `osxphotos-0.60.6/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_debug.py` & `osxphotos-0.60.6/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_empty_library_4_0.py` & `osxphotos-0.60.6/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_exif_info.py` & `osxphotos-0.60.6/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_exiftool.py` & `osxphotos-0.60.6/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_exiftool_caching.py` & `osxphotos-0.60.6/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.6/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.6/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.6/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_db.py` & `osxphotos-0.60.6/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_exportresults.py` & `osxphotos-0.60.6/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_faceinfo.py` & `osxphotos-0.60.6/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_fileutil.py` & `osxphotos-0.60.6/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_highsierra.py` & `osxphotos-0.60.6/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_image_converter.py` & `osxphotos-0.60.6/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.6/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.6/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.6/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.6/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.6/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.6/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_movies_4_0.py` & `osxphotos-0.60.6/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_movies_5_0.py` & `osxphotos-0.60.6/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_path_utils.py` & `osxphotos-0.60.6/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_personinfo.py` & `osxphotos-0.60.6/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_photokit.py` & `osxphotos-0.60.6/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_photosalbum_unicode.py` & `osxphotos-0.60.6/tests/test_photosalbum_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_photosdb_utils.py` & `osxphotos-0.60.6/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_placeinfo.py` & `osxphotos-0.60.6/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.6/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_projects_catalina.py` & `osxphotos-0.60.6/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_projects_sierra.py` & `osxphotos-0.60.6/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_score_info.py` & `osxphotos-0.60.6/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.6/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.6/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.6/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.6/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_sidecar_xmp.py` & `osxphotos-0.60.6/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.6/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.6/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.6/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.6/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_sqlitekvstore.py` & `osxphotos-0.60.6/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_template.py` & `osxphotos-0.60.6/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_template_counter.py` & `osxphotos-0.60.6/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_template_today.py` & `osxphotos-0.60.6/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_unicode.py` & `osxphotos-0.60.6/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_uti.py` & `osxphotos-0.60.6/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_utils.py` & `osxphotos-0.60.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.6/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.5/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.6/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

