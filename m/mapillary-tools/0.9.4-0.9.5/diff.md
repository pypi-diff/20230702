# Comparing `tmp/mapillary_tools-0.9.4.tar.gz` & `tmp/mapillary_tools-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapillary_tools-0.9.4.tar", last modified: Tue Oct 11 05:21:34 2022, max compression
+gzip compressed data, was "mapillary_tools-0.9.5.tar", last modified: Wed Nov  9 03:29:09 2022, max compression
```

## Comparing `mapillary_tools-0.9.4.tar` & `mapillary_tools-0.9.5.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.699657 mapillary_tools-0.9.4/
--rw-r--r--   0 taopeng    (501) staff       (20)     1292 2022-04-11 23:18:10.000000 mapillary_tools-0.9.4/LICENSE
--rw-r--r--   0 taopeng    (501) staff       (20)       47 2022-10-07 21:07:56.000000 mapillary_tools-0.9.4/MANIFEST.in
--rw-r--r--   0 taopeng    (501) staff       (20)    20050 2022-10-11 05:21:34.699813 mapillary_tools-0.9.4/PKG-INFO
--rw-r--r--   0 taopeng    (501) staff       (20)    19771 2022-10-07 21:07:56.000000 mapillary_tools-0.9.4/README.md
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.674766 mapillary_tools-0.9.4/mapillary_tools/
--rw-r--r--   0 taopeng    (501) staff       (20)       18 2022-10-11 04:58:59.000000 mapillary_tools-0.9.4/mapillary_tools/__init__.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1880 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/api_v4.py
--rw-r--r--   0 taopeng    (501) staff       (20)     3255 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/authenticate.py
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.687507 mapillary_tools-0.9.4/mapillary_tools/commands/
--rw-r--r--   0 taopeng    (501) staff       (20)      169 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/__init__.py
--rw-r--r--   0 taopeng    (501) staff       (20)     4160 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/__main__.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1136 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/authenticate.py
--rw-r--r--   0 taopeng    (501) staff       (20)    11405 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/process.py
--rw-r--r--   0 taopeng    (501) staff       (20)      644 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/process_and_upload.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2828 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/sample_video.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2069 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/upload.py
--rw-r--r--   0 taopeng    (501) staff       (20)      911 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/upload_blackvue.py
--rw-r--r--   0 taopeng    (501) staff       (20)      895 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/upload_camm.py
--rw-r--r--   0 taopeng    (501) staff       (20)      886 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/commands/upload_zip.py
--rw-r--r--   0 taopeng    (501) staff       (20)      453 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/video_process.py
--rw-r--r--   0 taopeng    (501) staff       (20)      817 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/video_process_and_upload.py
--rw-r--r--   0 taopeng    (501) staff       (20)      991 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/commands/zip.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2061 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/config.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1624 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/constants.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1631 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/exceptions.py
--rw-r--r--   0 taopeng    (501) staff       (20)    10807 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/exif_read.py
--rw-r--r--   0 taopeng    (501) staff       (20)     6158 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/exif_write.py
--rw-r--r--   0 taopeng    (501) staff       (20)     6253 2022-10-11 04:58:48.000000 mapillary_tools-0.9.4/mapillary_tools/ffmpeg.py
--rw-r--r--   0 taopeng    (501) staff       (20)     5350 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geo.py
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.698358 mapillary_tools-0.9.4/mapillary_tools/geotag/
--rw-r--r--   0 taopeng    (501) staff       (20)       19 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/__init__.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2580 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/blackvue_parser.py
--rw-r--r--   0 taopeng    (501) staff       (20)     8676 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/camm_builder.py
--rw-r--r--   0 taopeng    (501) staff       (20)     5765 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/camm_parser.py
--rw-r--r--   0 taopeng    (501) staff       (20)     3249 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_blackvue.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2758 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_camm.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2819 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_exif.py
--rw-r--r--   0 taopeng    (501) staff       (20)      207 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_generic.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2812 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gopro.py
--rw-r--r--   0 taopeng    (501) staff       (20)     6814 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gpx.py
--rw-r--r--   0 taopeng    (501) staff       (20)     3439 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gpx_file.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1499 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_nmea_file.py
--rw-r--r--   0 taopeng    (501) staff       (20)     2591 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/gpmf_gps_filter.py
--rw-r--r--   0 taopeng    (501) staff       (20)    12374 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/gpmf_parser.py
--rw-r--r--   0 taopeng    (501) staff       (20)     3766 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/gps_filter.py
--rw-r--r--   0 taopeng    (501) staff       (20)     5454 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/io_utils.py
--rw-r--r--   0 taopeng    (501) staff       (20)       23 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/mp4_optimizer.py
--rw-r--r--   0 taopeng    (501) staff       (20)    15062 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/simple_mp4_builder.py
--rw-r--r--   0 taopeng    (501) staff       (20)    20948 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/simple_mp4_parser.py
--rw-r--r--   0 taopeng    (501) staff       (20)      634 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/geotag/utils.py
--rw-r--r--   0 taopeng    (501) staff       (20)     1089 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/ipc.py
--rw-r--r--   0 taopeng    (501) staff       (20)    14755 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/process_geotag_properties.py
--rw-r--r--   0 taopeng    (501) staff       (20)     3663 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/process_import_meta_properties.py
--rw-r--r--   0 taopeng    (501) staff       (20)     7498 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/process_sequence_properties.py
--rw-r--r--   0 taopeng    (501) staff       (20)     4748 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/sample_video.py
--rw-r--r--   0 taopeng    (501) staff       (20)     7412 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/types.py
--rw-r--r--   0 taopeng    (501) staff       (20)    26164 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/upload.py
--rw-r--r--   0 taopeng    (501) staff       (20)     9199 2022-10-11 04:58:48.000000 mapillary_tools-0.9.4/mapillary_tools/upload_api_v4.py
--rw-r--r--   0 taopeng    (501) staff       (20)    16591 2022-10-11 04:29:27.000000 mapillary_tools-0.9.4/mapillary_tools/uploader.py
--rw-r--r--   0 taopeng    (501) staff       (20)     4584 2022-10-11 04:29:26.000000 mapillary_tools-0.9.4/mapillary_tools/utils.py
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.679988 mapillary_tools-0.9.4/mapillary_tools.egg-info/
--rw-r--r--   0 taopeng    (501) staff       (20)    20050 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/PKG-INFO
--rw-r--r--   0 taopeng    (501) staff       (20)     2302 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 taopeng    (501) staff       (20)        1 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 taopeng    (501) staff       (20)       75 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/entry_points.txt
--rw-r--r--   0 taopeng    (501) staff       (20)      214 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/requires.txt
--rw-r--r--   0 taopeng    (501) staff       (20)       16 2022-10-11 05:21:34.000000 mapillary_tools-0.9.4/mapillary_tools.egg-info/top_level.txt
--rw-r--r--   0 taopeng    (501) staff       (20)      209 2022-10-04 07:43:06.000000 mapillary_tools-0.9.4/requirements.txt
-drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-10-11 05:21:34.698896 mapillary_tools-0.9.4/schema/
--rw-r--r--   0 taopeng    (501) staff       (20)     2185 2022-09-11 11:36:20.000000 mapillary_tools-0.9.4/schema/image_description_schema.json
--rw-r--r--   0 taopeng    (501) staff       (20)      109 2022-10-11 05:21:34.700364 mapillary_tools-0.9.4/setup.cfg
--rw-r--r--   0 taopeng    (501) staff       (20)     1009 2022-10-07 21:07:56.000000 mapillary_tools-0.9.4/setup.py
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.540807 mapillary_tools-0.9.5/
+-rw-r--r--   0 taopeng    (501) staff       (20)     1292 2022-04-11 23:18:10.000000 mapillary_tools-0.9.5/LICENSE
+-rw-r--r--   0 taopeng    (501) staff       (20)       47 2022-10-07 21:07:56.000000 mapillary_tools-0.9.5/MANIFEST.in
+-rw-r--r--   0 taopeng    (501) staff       (20)    20050 2022-11-09 03:29:09.540947 mapillary_tools-0.9.5/PKG-INFO
+-rw-r--r--   0 taopeng    (501) staff       (20)    19771 2022-11-09 02:40:28.000000 mapillary_tools-0.9.5/README.md
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.515052 mapillary_tools-0.9.5/mapillary_tools/
+-rw-r--r--   0 taopeng    (501) staff       (20)       18 2022-11-09 02:23:37.000000 mapillary_tools-0.9.5/mapillary_tools/__init__.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1880 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/api_v4.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2957 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/authenticate.py
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.524336 mapillary_tools-0.9.5/mapillary_tools/commands/
+-rw-r--r--   0 taopeng    (501) staff       (20)      169 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/__init__.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     4160 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/__main__.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1136 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/authenticate.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    11405 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/commands/process.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      644 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/process_and_upload.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2828 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/sample_video.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2069 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/upload.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      911 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/commands/upload_blackvue.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      895 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/commands/upload_camm.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      886 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/commands/upload_zip.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      453 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/video_process.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      817 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/video_process_and_upload.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      991 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/commands/zip.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2103 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/config.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1788 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/constants.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1631 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/exceptions.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    10807 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/exif_read.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     6158 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/exif_write.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     7865 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/ffmpeg.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     5350 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geo.py
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.538358 mapillary_tools-0.9.5/mapillary_tools/geotag/
+-rw-r--r--   0 taopeng    (501) staff       (20)       19 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/__init__.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2983 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/blackvue_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    10408 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/camm_builder.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     8618 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/camm_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    14436 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/construct_mp4_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3297 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_blackvue.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3263 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_camm.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2819 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_exif.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      207 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_generic.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3351 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gopro.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     6814 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gpx.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3439 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gpx_file.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1499 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_nmea_file.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     2591 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/gpmf_gps_filter.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    14808 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/gpmf_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3766 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/gps_filter.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     5454 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/io_utils.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     7220 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/mp4_sample_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    11331 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/simple_mp4_builder.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     6671 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/simple_mp4_parser.py
+-rw-r--r--   0 taopeng    (501) staff       (20)      651 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/geotag/utils.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     1089 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/ipc.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    14755 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/process_geotag_properties.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     3663 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/process_import_meta_properties.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     7498 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/process_sequence_properties.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     4847 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/sample_video.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     7412 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/types.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    27167 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/upload.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     8670 2022-11-09 02:21:04.000000 mapillary_tools-0.9.5/mapillary_tools/upload_api_v4.py
+-rw-r--r--   0 taopeng    (501) staff       (20)    14729 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/uploader.py
+-rw-r--r--   0 taopeng    (501) staff       (20)     4584 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/mapillary_tools/utils.py
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.517710 mapillary_tools-0.9.5/mapillary_tools.egg-info/
+-rw-r--r--   0 taopeng    (501) staff       (20)    20050 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 taopeng    (501) staff       (20)     2353 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 taopeng    (501) staff       (20)        1 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 taopeng    (501) staff       (20)       75 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 taopeng    (501) staff       (20)      214 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/requires.txt
+-rw-r--r--   0 taopeng    (501) staff       (20)       16 2022-11-09 03:29:09.000000 mapillary_tools-0.9.5/mapillary_tools.egg-info/top_level.txt
+-rw-r--r--   0 taopeng    (501) staff       (20)      209 2022-10-04 07:43:06.000000 mapillary_tools-0.9.5/requirements.txt
+drwxr-xr-x   0 taopeng    (501) staff       (20)        0 2022-11-09 03:29:09.539935 mapillary_tools-0.9.5/schema/
+-rw-r--r--   0 taopeng    (501) staff       (20)     2185 2022-11-09 02:40:32.000000 mapillary_tools-0.9.5/schema/image_description_schema.json
+-rw-r--r--   0 taopeng    (501) staff       (20)      109 2022-11-09 03:29:09.541539 mapillary_tools-0.9.5/setup.cfg
+-rw-r--r--   0 taopeng    (501) staff       (20)     1009 2022-10-07 21:07:56.000000 mapillary_tools-0.9.5/setup.py
```

### Comparing `mapillary_tools-0.9.4/LICENSE` & `mapillary_tools-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/PKG-INFO` & `mapillary_tools-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapillary_tools
-Version: 0.9.4
+Version: 0.9.5
 Summary: Mapillary Image/Video Import Pipeline
 Home-page: https://github.com/mapillary/mapillary_tools
 Author: Mapillary
 License: BSD
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapillary_tools Version: 0.9.4 Summary: Mapillary
+Metadata-Version: 2.1 Name: mapillary_tools Version: 0.9.5 Summary: Mapillary
 Image/Video Import Pipeline Home-page: https://github.com/mapillary/
 mapillary_tools Author: Mapillary License: BSD Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
 [https://raw.githubusercontent.com/mapillary/mapillary_tools/main/docs/images/
                                    logo.png]
                ***** Process and upload Mapillary imagery *****
       [PyPI] [Actions_Status] [GitHub_license] [GitHub_stars] [Downloads]
```

### Comparing `mapillary_tools-0.9.4/README.md` & `mapillary_tools-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/api_v4.py` & `mapillary_tools-0.9.5/mapillary_tools/api_v4.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/authenticate.py` & `mapillary_tools-0.9.5/mapillary_tools/authenticate.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from . import api_v4, config, types
 
 
 LOG = logging.getLogger(__name__)
 
 
 def authenticate(
-    user_name: str = None,
-    user_email: str = None,
-    user_password: str = None,
-    jwt: str = None,
+    user_name: T.Optional[str] = None,
+    user_email: T.Optional[str] = None,
+    user_password: T.Optional[str] = None,
+    jwt: T.Optional[str] = None,
 ):
     if user_name:
         user_name = user_name.strip()
 
     while not user_name:
         user_name = input(
             "Enter the Mapillary username you would like to (re)authenticate: "
@@ -39,48 +39,34 @@
         }
     else:
         user_items = prompt_user_for_user_items(user_name)
 
     config.update_config(user_name, user_items)
 
 
-class HTTPError(requests.HTTPError):
-    pass
-
-
-def wrap_http_exception(ex: requests.HTTPError):
-    resp = ex.response
-    lines = [
-        f"{ex.request.method} {resp.url}",
-        f"> HTTP Status: {ex.response.status_code}",
-        f"{ex.response.text}",
-    ]
-    return HTTPError("\n".join(lines))
-
-
 def prompt_user_for_user_items(user_name: str) -> types.UserItem:
     print(f"Sign in for user {user_name}")
     user_email = input("Enter your Mapillary user email: ")
     user_password = getpass.getpass("Enter Mapillary user password: ")
 
     try:
         resp = api_v4.get_upload_token(user_email, user_password)
     except requests.HTTPError as ex:
         if 400 <= ex.response.status_code < 500:
             r = ex.response.json()
             subcode = r.get("error", {}).get("error_subcode")
             if subcode in [1348028, 1348092, 3404005, 1348131]:
                 title = r.get("error", {}).get("error_user_title")
                 message = r.get("error", {}).get("error_user_msg")
-                LOG.error(f"{title}: {message}")
+                LOG.error(f"%s: %s", title, message)
                 return prompt_user_for_user_items(user_name)
             else:
-                raise wrap_http_exception(ex)
+                raise ex
         else:
-            raise wrap_http_exception(ex)
+            raise ex
 
     data = resp.json()
     upload_token = T.cast(str, data.get("access_token"))
     user_key = T.cast(str, data.get("user_id"))
     if not isinstance(upload_token, str) or not isinstance(user_key, (str, int)):
         raise RuntimeError(
             f"Error extracting user_key or token from the login response: {data}"
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/__main__.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/__main__.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/authenticate.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/authenticate.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/process.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/process.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/process_and_upload.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/process_and_upload.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/sample_video.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/sample_video.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/upload.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/upload.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/upload_blackvue.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/upload_blackvue.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/upload_camm.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/upload_camm.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/upload_zip.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/upload_zip.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/video_process_and_upload.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/video_process_and_upload.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/commands/zip.py` & `mapillary_tools-0.9.5/mapillary_tools/commands/zip.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/config.py` & `mapillary_tools-0.9.5/mapillary_tools/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,36 +30,38 @@
     # Override to not change option names (by default it will lower them)
     config.optionxform = str  # type: ignore
     # If path not found, then config will be empty
     config.read(config_path)
     return config
 
 
-def load_user(user_name: str, config_path: str = None) -> T.Optional[types.UserItem]:
+def load_user(
+    user_name: str, config_path: T.Optional[str] = None
+) -> T.Optional[types.UserItem]:
     if config_path is None:
         config_path = MAPILLARY_CONFIG_PATH
     config = _load_config(config_path)
     if not config.has_section(user_name):
         return None
     user_items = dict(config.items(user_name))
     return T.cast(types.UserItem, user_items)
 
 
-def list_all_users(config_path: str = None) -> T.List[types.UserItem]:
+def list_all_users(config_path: T.Optional[str] = None) -> T.List[types.UserItem]:
     if config_path is None:
         config_path = MAPILLARY_CONFIG_PATH
     cp = _load_config(config_path)
     users = [
         load_user(user_name, config_path=config_path) for user_name in cp.sections()
     ]
     return [item for item in users if item is not None]
 
 
 def update_config(
-    user_name: str, user_items: types.UserItem, config_path: str = None
+    user_name: str, user_items: types.UserItem, config_path: T.Optional[str] = None
 ) -> None:
     if config_path is None:
         config_path = MAPILLARY_CONFIG_PATH
     config = _load_config(config_path)
     if not config.has_section(user_name):
         config.add_section(user_name)
     for key, val in user_items.items():
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/constants.py` & `mapillary_tools-0.9.5/mapillary_tools/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     _ENV_PREFIX + "IMAGE_DESCRIPTION_FILENAME", "mapillary_image_description.json"
 )
 SAMPLED_VIDEO_FRAMES_FILENAME = os.getenv(
     _ENV_PREFIX + "SAMPLED_VIDEO_FRAMES_FILENAME", "mapillary_sampled_video_frames"
 )
 MAX_SEQUENCE_LENGTH = int(os.getenv(_ENV_PREFIX + "MAX_SEQUENCE_LENGTH", 500))
 USER_DATA_DIR = appdirs.user_data_dir(appname="mapillary_tools", appauthor="Mapillary")
+UPLOAD_CHUNK_SIZE_MB = float(os.getenv(_ENV_PREFIX + "UPLOAD_CHUNK_SIZE_MB", 16))
 
 # DoP value, the lower the better
 # See https://github.com/gopro/gpmf-parser#hero5-black-with-gps-enabled-adds
 # It is used to filter out noisy points
 GOPRO_MAX_DOP100 = int(os.getenv(_ENV_PREFIX + "GOPRO_MAX_DOP100", 1000))
 GOPRO_GPS_FIXES: T.Set[int] = set(
     int(fix) for fix in os.getenv(_ENV_PREFIX + "GOPRO_GPS_FIXES", "2,3").split(",")
 )
+MAX_UPLOAD_RETRIES: int = int(os.getenv(_ENV_PREFIX + "MAX_UPLOAD_RETRIES", 200))
 
 # GPS precision, in meters, is used to filter outliers
 GOPRO_GPS_PRECISION = float(os.getenv(_ENV_PREFIX + "GOPRO_GPS_PRECISION", 15))
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/exceptions.py` & `mapillary_tools-0.9.5/mapillary_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/exif_read.py` & `mapillary_tools-0.9.5/mapillary_tools/exif_read.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/exif_write.py` & `mapillary_tools-0.9.5/mapillary_tools/exif_write.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/ffmpeg.py` & `mapillary_tools-0.9.5/mapillary_tools/ffmpeg.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,88 +30,135 @@
     duration: str
     height: int
     index: int
     tags: StreamTag
     width: int
 
 
-class ProbeFormat(TypedDict):
-    filename: str
-    duration: str
-
-
 class ProbeOutput(TypedDict):
     streams: T.List[Stream]
-    format: T.Dict
 
 
 class FFmpegNotFoundError(Exception):
     pass
 
 
+_MAX_STDERR_LENGTH = 2048
+
+
+def _truncate_begin(s: str) -> str:
+    if _MAX_STDERR_LENGTH < len(s):
+        return "..." + s[-_MAX_STDERR_LENGTH:]
+    else:
+        return s
+
+
+def _truncate_end(s: str) -> str:
+    if _MAX_STDERR_LENGTH < len(s):
+        return s[:_MAX_STDERR_LENGTH] + "..."
+    else:
+        return s
+
+
+class FFmpegCalledProcessError(Exception):
+    def __init__(self, ex: subprocess.CalledProcessError):
+        self.inner_ex = ex
+
+    def __str__(self) -> str:
+        msg = str(self.inner_ex)
+        if self.inner_ex.stderr is not None:
+            try:
+                stderr = self.inner_ex.stderr.decode("utf-8")
+            except UnicodeDecodeError:
+                stderr = str(self.inner_ex.stderr)
+            msg += f"\nSTDERR: {_truncate_begin(stderr)}"
+        return msg
+
+
 class FFMPEG:
     def __init__(
-        self, ffmpeg_path: str = "ffmpeg", ffprobe_path: str = "ffprobe"
+        self,
+        ffmpeg_path: str = "ffmpeg",
+        ffprobe_path: str = "ffprobe",
+        stderr: T.Optional[int] = None,
     ) -> None:
+        """
+        ffmpeg_path: path to ffmpeg binary
+        ffprobe_path: path to ffprobe binary
+        stderr: param passed to subprocess.run to control whether to capture stderr
+        """
         self.ffmpeg_path = ffmpeg_path
         self.ffprobe_path = ffprobe_path
+        self.stderr = stderr
 
     def _run_ffprobe_json(self, cmd: T.List[str]) -> T.Dict:
         full_cmd = [self.ffprobe_path, "-print_format", "json", *cmd]
         LOG.info(f"Extracting video information: {' '.join(full_cmd)}")
         try:
-            output = subprocess.check_output(full_cmd)
+            completed = subprocess.run(
+                full_cmd,
+                check=True,
+                stdout=subprocess.PIPE,
+                stderr=self.stderr,
+            )
         except FileNotFoundError:
             raise FFmpegNotFoundError(
                 f'The ffprobe command "{self.ffprobe_path}" not found'
             )
+        except subprocess.CalledProcessError as ex:
+            raise FFmpegCalledProcessError(ex) from ex
+
         try:
-            return json.loads(output)
+            stdout = completed.stdout.decode("utf-8")
+        except UnicodeDecodeError:
+            raise RuntimeError(
+                f"Error decoding ffprobe output as unicode: {_truncate_end(str(completed.stdout))}"
+            )
+
+        try:
+            output = json.loads(stdout)
         except json.JSONDecodeError:
             raise RuntimeError(
-                f"Error JSON decoding ffprobe output: {output.decode('utf-8')}"
+                f"Error JSON decoding ffprobe output: {_truncate_end(stdout)}"
+            )
+
+        # This check is for macOS:
+        # ffprobe -hide_banner -print_format json not_exists
+        # you will get exit code == 0 with the following stdout and stderr:
+        # {
+        # }
+        # not_exists: No such file or directory
+        if not output:
+            raise RuntimeError(
+                f"Empty JSON ffprobe output with STDERR: {_truncate_begin(str(completed.stderr))}"
             )
 
+        return output
+
     def _run_ffmpeg(self, cmd: T.List[str]) -> None:
         full_cmd = [self.ffmpeg_path, *cmd]
         LOG.info(f"Extracting frames: {' '.join(full_cmd)}")
         try:
-            subprocess.check_call(full_cmd)
+            subprocess.run(full_cmd, check=True, stderr=self.stderr)
         except FileNotFoundError:
             raise FFmpegNotFoundError(
                 f'The ffmpeg command "{self.ffmpeg_path}" not found'
             )
+        except subprocess.CalledProcessError as ex:
+            raise FFmpegCalledProcessError(ex) from ex
 
     def probe_format_and_streams(self, video_path: Path) -> ProbeOutput:
         cmd = [
             "-hide_banner",
             "-show_format",
             "-show_streams",
             str(video_path),
         ]
         return T.cast(ProbeOutput, self._run_ffprobe_json(cmd))
 
-    def extract_stream(self, source: Path, dest: Path, stream_id: int) -> None:
-        cmd = [
-            "-hide_banner",
-            "-i",
-            str(source),
-            "-y",  # overwrite - potentially dangerous
-            "-nostats",
-            "-codec",
-            "copy",
-            "-map",
-            f"0:{stream_id}",
-            "-f",
-            "rawvideo",
-            str(dest),
-        ]
-
-        self._run_ffmpeg(cmd)
-
     def extract_frames(
         self,
         video_path: Path,
         sample_dir: Path,
         sample_interval: float,
     ) -> None:
         sample_prefix = sample_dir.joinpath(video_path.stem)
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geo.py` & `mapillary_tools-0.9.5/mapillary_tools/geo.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/blackvue_parser.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/blackvue_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import pathlib
 import re
 import typing as T
 
 import pynmea2
 
@@ -48,36 +49,53 @@
                 lat=nmea.latitude,
                 lon=nmea.longitude,
                 alt=nmea.altitude,
                 angle=None,
             )
 
 
-# TODO: what it failed to parse free/cprt
-def find_camera_model(path: pathlib.Path) -> str:
-    with path.open("rb") as fp:
-        cprt_data = simple_mp4_parser.parse_data_first(fp, [b"free", b"cprt"])
-        if cprt_data is None:
-            return ""
-        fields = cprt_data.split(b";")
-        if 2 <= len(fields):
-            model: bytes = fields[1]
-            if model:
-                try:
-                    return model.decode("utf8")
-                except UnicodeDecodeError:
-                    return ""
+def extract_camera_model(fp: T.BinaryIO) -> str:
+    try:
+        cprt_bytes = simple_mp4_parser.parse_mp4_data_first(fp, [b"free", b"cprt"])
+    except simple_mp4_parser.ParsingError:
+        return ""
+
+    if cprt_bytes is None:
+        return ""
+
+    # examples: b' {"model":"DR900X Plus","ver":0.918,"lang":"English","direct":1,"psn":"","temp":34,"GPS":1}\x00'
+    #           b' Pittasoft Co., Ltd.;DR900S-1CH;1.008;English;1;D90SS1HAE00661;T69;\x00'
+    cprt_bytes = cprt_bytes.strip().strip(b"\x00")
+
+    try:
+        cprt_str = cprt_bytes.decode("utf8")
+    except UnicodeDecodeError:
+        return ""
+
+    try:
+        cprt_json = json.loads(cprt_str)
+    except json.JSONDecodeError:
+        cprt_json = None
+
+    if cprt_json is not None:
+        return str(cprt_json.get("model", "")).strip()
+
+    fields = cprt_str.split(";")
+    if 2 <= len(fields):
+        model = fields[1]
+        if model:
+            return model.strip()
         else:
             return ""
-    return ""
+    else:
+        return ""
 
 
 def extract_points(fp: T.BinaryIO) -> T.Optional[T.List[geo.Point]]:
-    # TODO: what it failed to parse free/gps
-    gps_data = simple_mp4_parser.parse_data_first(fp, [b"free", b"gps "])
+    gps_data = simple_mp4_parser.parse_mp4_data_first(fp, [b"free", b"gps "])
     if gps_data is None:
         return None
 
     points = list(_parse_gps_box(gps_data))
     if not points:
         return points
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/camm_builder.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/camm_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import dataclasses
 import io
 import typing as T
 
 from .. import geo, utils
 
 from . import (
     blackvue_parser,
     camm_parser,
+    construct_mp4_parser as cparser,
     gpmf_parser,
+    mp4_sample_parser as sample_parser,
     simple_mp4_builder as builder,
     simple_mp4_parser as parser,
 )
 from .simple_mp4_builder import BoxDict
 
 
 def build_camm_sample(point: geo.Point) -> bytes:
@@ -82,92 +85,79 @@
             "entries": entries,
         },
     }
 
 
 def convert_points_to_raw_samples(
     points: T.Sequence[geo.Point], timescale: int
-) -> T.Generator[parser.RawSample, None, None]:
+) -> T.Generator[sample_parser.RawSample, None, None]:
     for idx, point in enumerate(points):
         camm_sample_data = build_camm_sample(point)
 
         if idx + 1 < len(points):
             timedelta = int((points[idx + 1].time - point.time) * timescale)
         else:
             timedelta = 0
         assert (
             0 <= timedelta <= builder.UINT32_MAX
         ), f"expected timedelta {timedelta} between {points[idx]} and {points[idx + 1]} with timescale {timescale} to be <= UINT32_MAX"
 
-        yield parser.RawSample(
+        yield sample_parser.RawSample(
             # will update later
             description_idx=1,
             # will update later
             offset=0,
             size=len(camm_sample_data),
             timedelta=timedelta,
             is_sync=True,
         )
 
 
-def _create_camm_stbl(raw_samples: T.Iterable[parser.RawSample]) -> BoxDict:
+_STBLChildrenBuilderConstruct = cparser.Box32ConstructBuilder(
+    T.cast(cparser.SwitchMapType, cparser.CMAP[b"stbl"])
+)
+
+
+def _create_camm_stbl(raw_samples: T.Iterable[sample_parser.RawSample]) -> BoxDict:
     descriptions = [
         {
             "format": b"camm",
             "data_reference_index": 1,
             "data": b"",
         }
     ]
 
     stbl_children_boxes = builder.build_stbl_from_raw_samples(descriptions, raw_samples)
 
-    stbl_data = builder.FullBoxStruct32.BoxList.build(stbl_children_boxes)
+    stbl_data = _STBLChildrenBuilderConstruct.build_boxlist(stbl_children_boxes)
     return {
         "type": b"stbl",
         "data": stbl_data,
     }
 
 
-_SELF_REFERENCE_DREF_BOX_DATA: bytes = builder.FullBoxStruct32.Box.build(
-    {
-        "type": b"dref",
-        "data": {
-            "entries": [
-                {
-                    "type": b"url ",
-                    "data": {
-                        "flags": 1,
-                        "data": b"",
-                    },
-                }
-            ],
-        },
-    }
-)
-
-
 def create_camm_trak(
-    raw_samples: T.Sequence[parser.RawSample],
+    raw_samples: T.Sequence[sample_parser.RawSample],
     media_timescale: int,
 ) -> BoxDict:
     stbl = _create_camm_stbl(raw_samples)
 
-    hdlr = {
+    hdlr: BoxDict = {
         "type": b"hdlr",
         "data": {
             "handler_type": b"camm",
             "name": "CameraMetadataMotionHandler",
         },
     }
 
     media_duration = sum(s.timedelta for s in raw_samples)
     assert media_timescale <= builder.UINT64_MAX
 
     # Media Header Box
-    mdhd = {
+    mdhd: BoxDict = {
         "type": b"mdhd",
         "data": {
             # use 64-bit version
             "version": 1,
             # TODO: find timestamps from mvhd?
             # do not set dynamic timestamps (e.g. time.time()) here because we'd like to
             # make sure the md5 of the new mp4 file unchanged
@@ -177,15 +167,31 @@
             "duration": media_duration,
             "language": 21956,
         },
     }
 
     dinf: BoxDict = {
         "type": b"dinf",
-        "data": _SELF_REFERENCE_DREF_BOX_DATA,
+        "data": [
+            # self reference dref box
+            {
+                "type": b"dref",
+                "data": {
+                    "entries": [
+                        {
+                            "type": b"url ",
+                            "data": {
+                                "flags": 1,
+                                "data": b"",
+                            },
+                        }
+                    ],
+                },
+            }
+        ],
     }
 
     minf: BoxDict = {
         "type": b"minf",
         "data": [
             dinf,
             stbl,
@@ -224,78 +230,125 @@
         "data": [
             tkhd,
             mdia,
         ],
     }
 
 
-def extract_points(
+@dataclasses.dataclass
+class VideoMetadata:
+    file_type: utils.FileType
+    points: T.List[geo.Point]
+    make: str
+    model: str
+
+
+def extract_video_metadata(
     fp: T.BinaryIO,
     file_types: T.Optional[T.Set[utils.FileType]] = None,
-) -> T.Tuple[T.Optional[utils.FileType], T.List[geo.Point]]:
+) -> T.Optional[VideoMetadata]:
     start_offset = fp.tell()
 
     if file_types is None or utils.FileType.CAMM in file_types:
+        fp.seek(start_offset, io.SEEK_SET)
         try:
             points = camm_parser.extract_points(fp)
-        except (parser.BoxNotFoundError, parser.RangeError):
+        except parser.ParsingError:
             points = []
         if points:
-            return utils.FileType.CAMM, points
+            fp.seek(start_offset, io.SEEK_SET)
+            make, model = camm_parser.extract_camera_make_and_model(fp)
+            return VideoMetadata(utils.FileType.CAMM, points, make, model)
 
     if file_types is None or utils.FileType.GOPRO in file_types:
-        fp.seek(start_offset)
+        fp.seek(start_offset, io.SEEK_SET)
         try:
             points_with_fix = gpmf_parser.extract_points(fp)
-        except (parser.BoxNotFoundError, parser.RangeError):
-            points = []
+        except parser.ParsingError:
+            points_with_fix = []
         if points_with_fix:
-            return utils.FileType.GOPRO, T.cast(T.List[geo.Point], points_with_fix)
+            fp.seek(start_offset, io.SEEK_SET)
+            make, model = "GoPro", gpmf_parser.extract_camera_model(fp)
+            return VideoMetadata(
+                utils.FileType.GOPRO,
+                T.cast(T.List[geo.Point], points_with_fix),
+                make,
+                model,
+            )
 
     if file_types is None or utils.FileType.BLACKVUE in file_types:
-        fp.seek(start_offset)
+        fp.seek(start_offset, io.SEEK_SET)
         try:
             points = blackvue_parser.extract_points(fp)
-        except (parser.BoxNotFoundError, parser.RangeError):
+        except parser.ParsingError:
             points = []
         if points:
-            return utils.FileType.BLACKVUE, points
+            fp.seek(start_offset, io.SEEK_SET)
+            make, model = "BlackVue", blackvue_parser.extract_camera_model(fp)
+            return VideoMetadata(utils.FileType.BLACKVUE, points, make, model)
 
-    return None, []
+    return None
 
 
-def camm_sample_generator2(points: T.Sequence[geo.Point]):
+def camm_sample_generator2(video_metadata: VideoMetadata):
     def _f(
         fp: T.BinaryIO,
         moov_children: T.List[BoxDict],
     ) -> T.Generator[io.IOBase, None, None]:
         movie_timescale = builder.find_movie_timescale(moov_children)
         # make sure the precision of timedeltas not lower than 0.001 (1ms)
         media_timescale = max(1000, movie_timescale)
-        camm_samples = list(convert_points_to_raw_samples(points, media_timescale))
+        camm_samples = list(
+            convert_points_to_raw_samples(video_metadata.points, media_timescale)
+        )
         camm_trak = create_camm_trak(camm_samples, media_timescale)
-        elst = _create_edit_list([points], movie_timescale, media_timescale)
+        elst = _create_edit_list(
+            [video_metadata.points], movie_timescale, media_timescale
+        )
         if T.cast(T.Dict, elst["data"])["entries"]:
             T.cast(T.List[BoxDict], camm_trak["data"]).append(
                 {
                     "type": b"edts",
                     "data": [elst],
                 }
             )
         moov_children.append(camm_trak)
 
+        udta_data: T.List[BoxDict] = []
+        if video_metadata.make:
+            udta_data.append(
+                {
+                    "type": b"@mak",
+                    "data": video_metadata.make.encode("utf-8"),
+                }
+            )
+        if video_metadata.model:
+            udta_data.append(
+                {
+                    "type": b"@mod",
+                    "data": video_metadata.model.encode("utf-8"),
+                }
+            )
+        if udta_data:
+            moov_children.append(
+                {
+                    "type": b"udta",
+                    "data": udta_data,
+                }
+            )
+
         # if yield, the moov_children will not be modified
-        return (io.BytesIO(build_camm_sample(point)) for point in points)
+        return (io.BytesIO(build_camm_sample(point)) for point in video_metadata.points)
 
     return _f
 
 
 def camm_sample_generator(
     fp: T.BinaryIO,
     moov_children: T.List[BoxDict],
 ) -> T.Iterator[io.IOBase]:
-    fp.seek(0)
-    _, points = extract_points(fp)
-    if not points:
+    fp.seek(0, io.SEEK_SET)
+    metadata = extract_video_metadata(fp)
+    if not metadata:
         raise ValueError("no points found")
 
-    return camm_sample_generator2(points)(fp, moov_children)
+    return camm_sample_generator2(metadata)(fp, moov_children)
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_blackvue.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_blackvue.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,73 +21,73 @@
     ):
         self.image_paths = image_paths
         self.video_paths = video_paths
         self.offset_time = offset_time
         super().__init__()
 
     def to_description(self) -> T.List[types.ImageDescriptionFileOrError]:
-        descs: T.List[types.ImageDescriptionFileOrError] = []
+        all_descs: T.List[types.ImageDescriptionFileOrError] = []
 
         for video_path in self.video_paths:
             LOG.debug("Processing BlackVue video: %s", video_path)
 
-            sample_images = list(
+            sample_image_paths = list(
                 utils.filter_video_samples(self.image_paths, video_path)
             )
             LOG.debug(
                 "Found %d sample images from video %s",
-                len(sample_images),
+                len(sample_image_paths),
                 video_path,
             )
 
-            if not sample_images:
+            if not sample_image_paths:
                 continue
 
             points = blackvue_parser.parse_gps_points(video_path)
 
             # bypass empty points to raise MapillaryGPXEmptyError
             if points and geotag_utils.is_video_stationary(
                 geo.get_max_distance_from_start([(p.lat, p.lon) for p in points])
             ):
                 LOG.warning(
                     "Fail %d sample images due to stationary video %s",
-                    len(sample_images),
+                    len(sample_image_paths),
                     video_path,
                 )
-                for image_path in sample_images:
+                for image_path in sample_image_paths:
                     err_desc = types.describe_error(
                         exceptions.MapillaryStationaryVideoError(
                             "Stationary BlackVue video"
                         ),
                         str(image_path),
                     )
-                    descs.append(err_desc)
+                    all_descs.append(err_desc)
                 continue
 
-            model = blackvue_parser.find_camera_model(video_path)
-            LOG.debug(
-                f"Found BlackVue camera model %s from video %s", model, video_path
-            )
-
             with tqdm(
-                total=len(sample_images),
+                total=len(sample_image_paths),
                 desc=f"Interpolating {video_path.name}",
                 unit="images",
                 disable=LOG.getEffectiveLevel() <= logging.DEBUG,
             ) as pbar:
                 geotag = GeotagFromGPXWithProgress(
-                    sample_images,
+                    sample_image_paths,
                     points,
                     use_gpx_start_time=False,
                     use_image_start_time=True,
                     offset_time=self.offset_time,
                     progress_bar=pbar,
                 )
-                for desc in geotag.to_description():
-                    if not types.is_error(desc):
-                        desc = T.cast(types.ImageDescriptionFile, desc)
-                        desc["MAPDeviceMake"] = "Blackvue"
-                        if model:
-                            desc["MAPDeviceModel"] = model
-                    descs.append(desc)
+                this_descs = geotag.to_description()
+                all_descs.extend(this_descs)
+
+            # update make and model
+            with video_path.open("rb") as fp:
+                make, model = "BlackVue", blackvue_parser.extract_camera_model(fp)
+            LOG.debug(f'Found camera make "%s" and model "%s"', make, model)
+            for desc in types.filter_out_errors(this_descs):
+                if make:
+                    desc["MAPDeviceMake"] = make
+                if model:
+                    desc["MAPDeviceModel"] = model
 
-        return descs
+        return all_descs
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_camm.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_camm.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ):
         self.image_paths = image_paths
         self.video_paths = video_paths
         self.offset_time = offset_time
         super().__init__()
 
     def to_description(self) -> T.List[types.ImageDescriptionFileOrError]:
-        descs: T.List[types.ImageDescriptionFileOrError] = []
+        all_descs: T.List[types.ImageDescriptionFileOrError] = []
         for video_path in self.video_paths:
             LOG.debug("Processing CAMM video: %s", video_path)
 
             sample_image_paths = list(
                 utils.filter_video_samples(self.image_paths, video_path)
             )
             LOG.debug(
@@ -56,15 +56,15 @@
                 for image_path in sample_image_paths:
                     err_desc = types.describe_error(
                         exceptions.MapillaryStationaryVideoError(
                             "Stationary CAMM video"
                         ),
                         str(image_path),
                     )
-                    descs.append(err_desc)
+                    all_descs.append(err_desc)
                 continue
 
             with tqdm(
                 total=len(sample_image_paths),
                 desc=f"Interpolating {video_path.name}",
                 unit="images",
                 disable=LOG.getEffectiveLevel() <= logging.DEBUG,
@@ -73,9 +73,21 @@
                     sample_image_paths,
                     points,
                     use_gpx_start_time=False,
                     use_image_start_time=True,
                     offset_time=self.offset_time,
                     progress_bar=pbar,
                 )
-                descs.extend(geotag.to_description())
-        return descs
+                this_descs = geotag.to_description()
+                all_descs.extend(this_descs)
+
+            # update make and model
+            with video_path.open("rb") as fp:
+                make, model = camm_parser.extract_camera_make_and_model(fp)
+            LOG.debug(f'Found camera make "%s" and model "%s"', make, model)
+            for desc in types.filter_out_errors(this_descs):
+                if make:
+                    desc["MAPDeviceMake"] = make
+                if model:
+                    desc["MAPDeviceModel"] = model
+
+        return all_descs
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_exif.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_exif.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gopro.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gopro.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,64 +22,75 @@
     ):
         self.image_paths = image_paths
         self.video_paths = video_paths
         self.offset_time = offset_time
         super().__init__()
 
     def to_description(self) -> T.List[types.ImageDescriptionFileOrError]:
-        descs: T.List[types.ImageDescriptionFileOrError] = []
+        all_descs: T.List[types.ImageDescriptionFileOrError] = []
 
         for video_path in self.video_paths:
             LOG.debug("Processing GoPro video: %s", video_path)
 
-            sample_images = list(
+            sample_image_paths = list(
                 utils.filter_video_samples(self.image_paths, video_path)
             )
             LOG.debug(
                 "Found %d sample images from video %s",
-                len(sample_images),
+                len(sample_image_paths),
                 video_path,
             )
 
-            if not sample_images:
+            if not sample_image_paths:
                 continue
 
             points = gpmf_gps_filter.filter_noisy_points(
                 gpmf_parser.parse_gpx(video_path)
             )
 
             # bypass empty points to raise MapillaryGPXEmptyError
             if points and geotag_utils.is_video_stationary(
                 geo.get_max_distance_from_start([(p.lat, p.lon) for p in points])
             ):
                 LOG.warning(
                     "Fail %d sample images due to stationary video %s",
-                    len(sample_images),
+                    len(sample_image_paths),
                     video_path,
                 )
-                for image_path in sample_images:
+                for image_path in sample_image_paths:
                     err_desc = types.describe_error(
                         exceptions.MapillaryStationaryVideoError(
                             "Stationary GoPro video"
                         ),
                         str(image_path),
                     )
-                    descs.append(err_desc)
+                    all_descs.append(err_desc)
                 continue
 
             with tqdm(
-                total=len(sample_images),
+                total=len(sample_image_paths),
                 desc=f"Interpolating {video_path.name}",
                 unit="images",
                 disable=LOG.getEffectiveLevel() <= logging.DEBUG,
             ) as pbar:
                 geotag = GeotagFromGPXWithProgress(
-                    sample_images,
+                    sample_image_paths,
                     points,
                     use_gpx_start_time=False,
                     use_image_start_time=True,
                     offset_time=self.offset_time,
                     progress_bar=pbar,
                 )
-                descs.extend(geotag.to_description())
+                this_descs = geotag.to_description()
+                all_descs.extend(this_descs)
 
-        return descs
+            # update make and model
+            with video_path.open("rb") as fp:
+                make, model = "GoPro", gpmf_parser.extract_camera_model(fp)
+            LOG.debug(f'Found camera make "%s" and model "%s"', make, model)
+            for desc in types.filter_out_errors(this_descs):
+                if make:
+                    desc["MAPDeviceMake"] = make
+                if model:
+                    desc["MAPDeviceModel"] = model
+
+        return all_descs
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gpx.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gpx.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_gpx_file.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_gpx_file.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/geotag_from_nmea_file.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/geotag_from_nmea_file.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/gpmf_gps_filter.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/gpmf_gps_filter.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/gps_filter.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/gps_filter.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/io_utils.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/io_utils.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/geotag/utils.py` & `mapillary_tools-0.9.5/mapillary_tools/geotag/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import typing as T
 
 import gpxpy
+import gpxpy.gpx
 
 from .. import geo
 
 
 def is_video_stationary(max_distance_from_start: float) -> bool:
     radius_threshold = 10
     return max_distance_from_start < radius_threshold
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/ipc.py` & `mapillary_tools-0.9.5/mapillary_tools/ipc.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/process_geotag_properties.py` & `mapillary_tools-0.9.5/mapillary_tools/process_geotag_properties.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/process_import_meta_properties.py` & `mapillary_tools-0.9.5/mapillary_tools/process_import_meta_properties.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/process_sequence_properties.py` & `mapillary_tools-0.9.5/mapillary_tools/process_sequence_properties.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/sample_video.py` & `mapillary_tools-0.9.5/mapillary_tools/sample_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,24 @@
     skip_sample_errors: bool = False,
     rerun: bool = False,
 ) -> None:
     if video_import_path.is_dir():
         video_list = utils.find_videos(
             [video_import_path], skip_subfolders=skip_subfolders
         )
-        video_dir = video_import_path
+        video_dir = video_import_path.resolve()
         LOG.debug(f"Found %d videos in %s", len(video_list), video_dir)
     elif video_import_path.is_file():
         video_list = [video_import_path]
         video_dir = video_import_path.resolve().parent
     else:
         raise exceptions.MapillaryFileNotFoundError(
             f"Video file or directory not found: {video_import_path}"
         )
+    assert video_dir.is_absolute(), f"video_dir must be absolute here: {str(video_dir)}"
 
     video_start_time_dt: T.Optional[datetime.datetime] = None
     if video_start_time is not None:
         try:
             video_start_time_dt = types.map_capture_time_to_datetime(video_start_time)
         except ValueError as ex:
             raise exceptions.MapillaryBadParameterError(str(ex))
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/types.py` & `mapillary_tools-0.9.5/mapillary_tools/types.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools/upload.py` & `mapillary_tools-0.9.5/mapillary_tools/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,28 @@
 
 class UploadError(Exception):
     def __init__(self, inner_ex) -> None:
         self.inner_ex = inner_ex
         super().__init__(str(inner_ex))
 
 
+class UploadHTTPError(Exception):
+    pass
+
+
+def wrap_http_exception(ex: requests.HTTPError):
+    resp = ex.response
+    lines = [
+        f"{ex.request.method} {resp.url}",
+        f"> HTTP Status: {ex.response.status_code}",
+        f"{resp.content}",
+    ]
+    return UploadHTTPError("\n".join(lines))
+
+
 def read_image_descriptions(desc_path: str) -> T.List[types.ImageDescriptionFile]:
     descs: T.List[types.ImageDescriptionFile] = []
 
     if desc_path == "-":
         try:
             descs = json.load(sys.stdin)
         except json.JSONDecodeError as ex:
@@ -125,23 +139,26 @@
         if len(all_user_items) == 1:
             user_items = all_user_items[0]
         else:
             raise exceptions.MapillaryBadParameterError(
                 f"Found multiple Mapillary accounts. Please specify one with --user_name"
             )
     else:
-        user_items = authenticate.authenticate_user(user_name)
+        try:
+            user_items = authenticate.authenticate_user(user_name)
+        except requests.HTTPError as exc:
+            raise wrap_http_exception(exc) from exc
 
     if organization_key is not None:
         try:
             resp = api_v4.fetch_organization(
                 user_items["user_upload_token"], organization_key
             )
         except requests.HTTPError as ex:
-            raise authenticate.wrap_http_exception(ex) from ex
+            raise wrap_http_exception(ex) from ex
         org = resp.json()
         LOG.info("Uploading to organization: %s", json.dumps(org))
         user_items = T.cast(
             types.UserItem, {**user_items, "MAPOrganizationKey": organization_key}
         )
     return user_items
 
@@ -436,15 +453,15 @@
             action,
             summary,
         )
     except requests.HTTPError as exc:
         LOG.warning(
             "Error from API Logging for action %s",
             action,
-            exc_info=uploader.upload_api_v4.wrap_http_exception(exc),
+            exc_info=wrap_http_exception(exc),
         )
     except:
         LOG.warning("Error from API Logging for action %s", action, exc_info=True)
 
 
 def _api_logging_failed(user_items: types.UserItem, payload: T.Dict, exc: Exception):
     if MAPILLARY_DISABLE_API_LOGGING:
@@ -456,15 +473,15 @@
     try:
         api_v4.logging(
             user_items["user_upload_token"],
             action,
             payload_with_reason,
         )
     except requests.HTTPError as exc:
-        wrapped_exc = uploader.upload_api_v4.wrap_http_exception(exc)
+        wrapped_exc = wrap_http_exception(exc)
         LOG.warning(
             "Error from API Logging for action %s",
             action,
             exc_info=wrapped_exc,
         )
     except:
         LOG.warning("Error from API Logging for action %s", action, exc_info=True)
@@ -580,15 +597,20 @@
         "user_key": user_items.get("MAPSettingsUserKey"),
         "organization_key": user_items.get("MAPOrganizationKey"),
     }
 
     if enable_history:
         _setup_write_upload_history(emitter, params, descs)
 
-    mly_uploader = uploader.Uploader(user_items, emitter=emitter, dry_run=dry_run)
+    mly_uploader = uploader.Uploader(
+        user_items,
+        emitter=emitter,
+        dry_run=dry_run,
+        chunk_size=int(constants.UPLOAD_CHUNK_SIZE_MB * 1024 * 1024),
+    )
 
     image_paths = utils.find_images(import_paths, skip_subfolders=skip_subfolders)
     video_paths = utils.find_videos(import_paths, skip_subfolders=skip_subfolders)
     zip_paths = utils.find_zipfiles(import_paths, skip_subfolders=skip_subfolders)
 
     try:
         if FileType.IMAGE in file_types:
@@ -616,15 +638,18 @@
 
         if FileType.ZIP in file_types:
             _upload_zipfiles(mly_uploader, zip_paths)
 
     except UploadError as ex:
         if not dry_run:
             _api_logging_failed(mly_uploader.user_items, _summarize(stats), ex.inner_ex)
-        raise ex
+        if isinstance(ex.inner_ex, requests.HTTPError):
+            raise wrap_http_exception(ex.inner_ex) from ex.inner_ex
+        else:
+            raise ex
 
     if stats:
         if not dry_run:
             _api_logging_finished(user_items, _summarize(stats))
         _show_upload_summary(stats)
     else:
         LOG.info("Nothing uploaded. Bye.")
@@ -634,52 +659,58 @@
     mly_uploader: uploader.Uploader,
     video_paths: T.Sequence[Path],
     file_types: T.Set[FileType],
 ) -> None:
     for idx, video_path in enumerate(video_paths):
         LOG.debug("Converting and uploading %s", video_path)
         with open(video_path, "rb") as src_fp:
-            file_type, points = camm_builder.extract_points(src_fp, file_types)
-            if file_type is None:
+            metadata = camm_builder.extract_video_metadata(src_fp, file_types)
+            if metadata is None:
                 LOG.warning(
                     f"Skipping %s due to: No GPS found in the video",
                     video_path.name,
                 )
                 continue
 
-            if file_type == FileType.GOPRO:
-                new_points = gpmf_gps_filter.filter_noisy_points(
-                    T.cast(T.List[gpmf_parser.PointWithFix], points)
+            if metadata.file_type == FileType.GOPRO:
+                metadata.points = T.cast(
+                    T.List[geo.Point],
+                    gpmf_gps_filter.filter_noisy_points(
+                        T.cast(T.List[gpmf_parser.PointWithFix], metadata.points)
+                    ),
                 )
-                points = T.cast(T.List[geo.Point], new_points)
 
             stationary = video_utils.is_video_stationary(
-                geo.get_max_distance_from_start([(p.lat, p.lon) for p in points])
+                geo.get_max_distance_from_start(
+                    [(p.lat, p.lon) for p in metadata.points]
+                )
             )
             if stationary:
                 LOG.warning(
                     f"Skipping %s %s due to: Stationary video",
-                    file_type.value.upper(),
+                    metadata.file_type.value.upper(),
                     video_path.name,
                 )
                 continue
 
-            generator = camm_builder.camm_sample_generator2(points)
+            generator = camm_builder.camm_sample_generator2(metadata)
             camm_fp = simple_mp4_builder.transform_mp4(src_fp, generator)
             event_payload: uploader.Progress = {
                 "total_sequence_count": len(video_paths),
                 "sequence_idx": idx,
-                "file_type": file_type.value,
+                "file_type": metadata.file_type.value,
+                "import_path": str(video_path),
             }
             try:
                 cluster_id = mly_uploader.upload_camm_fp(
-                    T.cast(T.BinaryIO, camm_fp), video_path, event_payload=event_payload
+                    T.cast(T.BinaryIO, camm_fp), event_payload=event_payload
                 )
             except Exception as ex:
                 raise UploadError(ex) from ex
+
         LOG.debug(f"Uploaded to cluster: %s", cluster_id)
 
 
 def _check_blackvue(video_path: Path) -> None:
     # Skip in tests only because we don't have valid sample blackvue for tests
     if os.getenv("MAPILLARY__DISABLE_BLACKVUE_CHECK") == "YES":
         return
@@ -700,33 +731,35 @@
     video_paths: T.Sequence[Path],
 ) -> None:
     for idx, video_path in enumerate(video_paths):
         event_payload: uploader.Progress = {
             "total_sequence_count": len(video_paths),
             "sequence_idx": idx,
             "file_type": FileType.RAW_BLACKVUE.value,
+            "import_path": str(video_path),
         }
 
         try:
             _check_blackvue(video_path)
         except Exception as ex:
             LOG.warning(
                 f"Skipping %s %s due to: %s",
                 FileType.RAW_BLACKVUE.value.upper(),
                 video_path.name,
                 ex,
             )
             continue
 
-        try:
-            cluster_id = mly_uploader.upload_blackvue(
-                video_path, event_payload=event_payload
-            )
-        except Exception as ex:
-            raise UploadError(ex) from ex
+        with video_path.open("rb") as fp:
+            try:
+                cluster_id = mly_uploader.upload_blackvue_fp(
+                    fp, event_payload=event_payload
+                )
+            except Exception as ex:
+                raise UploadError(ex) from ex
         LOG.debug(f"Uploaded to cluster: %s", cluster_id)
 
 
 def _check_camm(video_path: Path) -> None:
     # Skip in tests only because we don't have valid sample CAMM for tests
     if os.getenv("MAPILLARY__DISABLE_CAMM_CHECK") == "YES":
         return
@@ -747,43 +780,47 @@
     video_paths: T.Sequence[Path],
 ) -> None:
     for idx, video_path in enumerate(video_paths):
         event_payload: uploader.Progress = {
             "total_sequence_count": len(video_paths),
             "sequence_idx": idx,
             "file_type": FileType.RAW_CAMM.value,
+            "import_path": str(video_path),
         }
         try:
             _check_camm(video_path)
         except Exception as ex:
             LOG.warning(
                 f"Skipping %s %s due to: %s",
                 FileType.RAW_CAMM.value.upper(),
                 video_path.name,
                 ex,
             )
             continue
         try:
-            cluster_id = mly_uploader.upload_camm(
-                video_path, event_payload=event_payload
-            )
+            with video_path.open("rb") as fp:
+                cluster_id = mly_uploader.upload_camm_fp(
+                    fp, event_payload=event_payload
+                )
         except Exception as ex:
             raise UploadError(ex) from ex
+
         LOG.debug(f"Uploaded to cluster: %s", cluster_id)
 
 
 def _upload_zipfiles(
     mly_uploader: uploader.Uploader,
     zip_paths: T.Sequence[Path],
 ) -> None:
     for idx, zip_path in enumerate(zip_paths):
         event_payload: uploader.Progress = {
             "total_sequence_count": len(zip_paths),
             "sequence_idx": idx,
             "file_type": FileType.ZIP.value,
+            "import_path": str(zip_path),
         }
         try:
             cluster_id = mly_uploader.upload_zipfile(
                 zip_path, event_payload=event_payload
             )
         except Exception as ex:
             raise UploadError(ex) from ex
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/upload_api_v4.py` & `mapillary_tools-0.9.5/mapillary_tools/upload_api_v4.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,155 @@
 import io
+import json
+import logging
 import os
+import random
 import sys
 import typing as T
 
 import requests
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module
 else:
     from typing_extensions import Literal
 
 from .api_v4 import MAPILLARY_GRAPH_API_ENDPOINT
 
+LOG = logging.getLogger(__name__)
 MAPILLARY_UPLOAD_ENDPOINT = os.getenv(
     "MAPILLARY_UPLOAD_ENDPOINT", "https://rupload.facebook.com/mapillary_public_uploads"
 )
-DEFAULT_CHUNK_SIZE = 1024 * 1024 * 16
-REQUESTS_TIMEOUT = 60  # 1 minutes
-# According to the docs, UPLOAD_REQUESTS_TIMEOUT sets both the "connection timeout"
-# and "read timeout": https://docs.python-requests.org/en/latest/user/advanced/#timeouts
-# In my test, however, the connection timeout does not only include the time for connection,
-# but also the time for uploading the actual data.
-# i.e. if your data uploading can't finish in this timeout, it will throw:
+DEFAULT_CHUNK_SIZE = 1024 * 1024 * 16  # 16MB
+# According to the docs, UPLOAD_REQUESTS_TIMEOUT can be a tuple of
+# (connection_timeout, read_timeout): https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
+# In my test, however, the connection_timeout rules both connection timeout and read timeout.
+# i.e. if your the server does not respond within this timeout, it will throw:
 # ConnectionError: ('Connection aborted.', timeout('The write operation timed out'))
-# so make sure the largest possible chunks can be uploaded before this timeout
-UPLOAD_REQUESTS_TIMEOUT = 10 * 60  # 10 minutes
+# So let us make sure the largest possible chunks can be uploaded before this timeout for now,
+REQUESTS_TIMEOUT = (20, 20)  # 20 seconds
+UPLOAD_REQUESTS_TIMEOUT = (30 * 60, 30 * 60)  # 30 minutes
 
 
 FileType = Literal["zip", "mly_blackvue_video", "mly_camm_video"]
 
 
-class UploadHTTPError(Exception):
-    pass
-
-
-def wrap_http_exception(ex: requests.HTTPError):
-    resp = ex.response
-    lines = [
-        f"{ex.request.method} {resp.url}",
-        f"> HTTP Status: {ex.response.status_code}",
-        f"{ex.response.text}",
-    ]
-    return UploadHTTPError("\n".join(lines))
+def _sanitize_headers(headers: T.Dict):
+    return {
+        k: v
+        for k, v in headers.items()
+        if k.lower() not in ["authorization", "cookie", "x-fb-access-token"]
+    }
+
+
+def _truncate_end(s: bytes) -> bytes:
+    MAX_LENGTH = 512
+    if MAX_LENGTH < len(s):
+        if isinstance(s, bytes):
+            return s[:MAX_LENGTH] + b"..."
+        else:
+            return str(s[:MAX_LENGTH]) + "..."
+    else:
+        return s
 
 
 class UploadService:
     user_access_token: str
     entity_size: int
     session_key: str
     callbacks: T.List[T.Callable[[bytes, T.Optional[requests.Response]], None]]
     file_type: FileType
     organization_id: T.Optional[T.Union[str, int]]
+    chunk_size: int
 
     def __init__(
         self,
         user_access_token: str,
         session_key: str,
         entity_size: int,
         organization_id: T.Optional[T.Union[str, int]] = None,
         file_type: FileType = "zip",
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
     ):
         if entity_size <= 0:
             raise ValueError(f"Expect positive entity size but got {entity_size}")
 
         if file_type.lower() not in ["zip", "mly_blackvue_video", "mly_camm_video"]:
             raise ValueError(f"Invalid file type {file_type}")
 
+        if chunk_size <= 0:
+            raise ValueError("Expect positive chunk size")
+
         self.user_access_token = user_access_token
         self.session_key = session_key
         self.entity_size = entity_size
         self.organization_id = organization_id
         self.file_type = T.cast(FileType, file_type.lower())
         self.callbacks = []
+        self.chunk_size = chunk_size
 
     def fetch_offset(self) -> int:
         headers = {
             "Authorization": f"OAuth {self.user_access_token}",
         }
+        url = f"{MAPILLARY_UPLOAD_ENDPOINT}/{self.session_key}"
+        LOG.debug("GET %s", url)
         resp = requests.get(
-            f"{MAPILLARY_UPLOAD_ENDPOINT}/{self.session_key}",
+            url,
             headers=headers,
             timeout=REQUESTS_TIMEOUT,
         )
+        LOG.debug("HTTP response %s: %s", resp.status_code, resp.content)
         resp.raise_for_status()
         data = resp.json()
         return data["offset"]
 
     def upload(
         self,
         data: T.IO[bytes],
         offset: T.Optional[int] = None,
-        chunk_size: int = DEFAULT_CHUNK_SIZE,
     ) -> str:
-        if chunk_size <= 0:
-            raise ValueError("Expect positive chunk size")
-
         if offset is None:
             offset = self.fetch_offset()
 
         entity_type_map: T.Dict[FileType, str] = {
             "zip": "application/zip",
             "mly_blackvue_video": "video/mp4",
             "mly_camm_video": "video/mp4",
         }
 
         entity_type = entity_type_map[self.file_type]
 
         data.seek(offset, io.SEEK_CUR)
 
         while True:
-            chunk = data.read(chunk_size)
+            chunk = data.read(self.chunk_size)
             # it is possible to upload an empty chunk here
             # in order to return the handle
             headers = {
                 "Authorization": f"OAuth {self.user_access_token}",
                 "Offset": f"{offset}",
                 "X-Entity-Length": str(self.entity_size),
                 "X-Entity-Name": self.session_key,
                 "X-Entity-Type": entity_type,
             }
+            url = f"{MAPILLARY_UPLOAD_ENDPOINT}/{self.session_key}"
+            LOG.debug("POST %s HEADERS %s", url, json.dumps(_sanitize_headers(headers)))
             resp = requests.post(
-                f"{MAPILLARY_UPLOAD_ENDPOINT}/{self.session_key}",
+                url,
                 headers=headers,
                 data=chunk,
                 timeout=UPLOAD_REQUESTS_TIMEOUT,
             )
+            LOG.debug(
+                "HTTP response %s: %s", resp.status_code, _truncate_end(resp.content)
+            )
             resp.raise_for_status()
             offset += len(chunk)
+            LOG.debug("The next offset will be: %s", offset)
             for callback in self.callbacks:
                 callback(chunk, resp)
             # we can assert that offset == self.fetch_offset(session_key)
             # otherwise, server will throw
 
             if not chunk:
                 break
@@ -154,37 +173,38 @@
         data: T.Dict[str, T.Union[str, int]] = {
             "file_handle": file_handle,
             "file_type": self.file_type,
         }
         if self.organization_id is not None:
             data["organization_id"] = self.organization_id
 
+        url = f"{MAPILLARY_GRAPH_API_ENDPOINT}/finish_upload"
+
+        LOG.debug("POST %s HEADERS %s", url, json.dumps(_sanitize_headers(headers)))
         resp = requests.post(
-            f"{MAPILLARY_GRAPH_API_ENDPOINT}/finish_upload",
+            url,
             headers=headers,
             json=data,
             timeout=REQUESTS_TIMEOUT,
         )
+        LOG.debug("HTTP response %s: %s", resp.status_code, _truncate_end(resp.content))
 
         resp.raise_for_status()
 
         data = resp.json()
 
         cluster_id = data.get("cluster_id")
         if cluster_id is None:
             raise RuntimeError(
                 f"Upload server error: failed to create the cluster {resp.text}"
             )
 
         return T.cast(str, cluster_id)
 
 
-import random
-
-
 # A mock class for testing only
 class FakeUploadService(UploadService):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._upload_path = os.getenv(
             "MAPILLARY_UPLOAD_PATH", "mapillary_public_uploads"
         )
@@ -231,53 +251,7 @@
             )
         filename = os.path.join(self._upload_path, self.session_key)
         if not os.path.exists(filename):
             return 0
         with open(filename, "rb") as fp:
             fp.seek(0, io.SEEK_END)
             return fp.tell()
-
-
-def _file_stats(fp: T.IO[bytes]):
-    md5 = hashlib.md5()
-    while True:
-        buf = fp.read(DEFAULT_CHUNK_SIZE)
-        if not buf:
-            break
-        md5.update(buf)
-    fp.seek(0, os.SEEK_END)
-    return md5.hexdigest(), fp.tell()
-
-
-if __name__ == "__main__":
-    import hashlib, os, sys
-
-    import tqdm
-
-    user_access_token = os.getenv("MAPILLARY_TOOLS_USER_ACCESS_TOKEN")
-    if not user_access_token:
-        raise RuntimeError("MAPILLARY_TOOLS_USER_ACCESS_TOKEN is required")
-
-    path = sys.argv[1]
-    with open(path, "rb") as fp:
-        md5sum, entity_size = _file_stats(fp)
-    session_key = sys.argv[2] if sys.argv[2:] else f"mly_tools_test_{md5sum}"
-    service = UploadService(user_access_token, session_key, entity_size)
-
-    print(f"session key: {session_key}")
-    print(f"entity size: {entity_size}")
-    print(f"initial offset: {service.fetch_offset()}")
-
-    with open(path, "rb") as fp:
-        with tqdm.tqdm(
-            total=entity_size,
-            initial=service.fetch_offset(),
-            unit="B",
-            unit_scale=True,
-            unit_divisor=1024,
-        ) as pbar:
-            service.callbacks.append(lambda chunk, resp: pbar.update(len(chunk)))
-            try:
-                file_handle = service.upload(fp)
-            except requests.HTTPError as ex:
-                raise wrap_http_exception(ex)
-    print(file_handle)
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/uploader.py` & `mapillary_tools-0.9.5/mapillary_tools/uploader.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import requests
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module
 else:
     from typing_extensions import Literal
 
-from . import exif_write, types, upload_api_v4, utils
+from . import constants, exif_write, types, upload_api_v4, utils
 
 
-MIN_CHUNK_SIZE = 1024 * 1024  # 1MB
-MAX_CHUNK_SIZE = 1024 * 1024 * 16  # 16MB
 LOG = logging.getLogger(__name__)
 
 
 def _group_sequences_by_uuid(
     descs: T.Sequence[types.ImageDescriptionFile],
 ) -> T.Dict[str, T.Dict[str, types.ImageDescriptionFile]]:
     sequences: T.Dict[str, T.Dict[str, types.ImageDescriptionFile]] = {}
@@ -106,144 +104,179 @@
     def emit(self, event: EventName, *args, **kwargs):
         for callback in self.events.get(event, []):
             callback(*args, **kwargs)
 
 
 class Uploader:
     def __init__(
-        self, user_items: types.UserItem, emitter: EventEmitter = None, dry_run=False
+        self,
+        user_items: types.UserItem,
+        emitter: T.Optional[EventEmitter] = None,
+        chunk_size: int = upload_api_v4.DEFAULT_CHUNK_SIZE,
+        dry_run=False,
     ):
         jsonschema.validate(instance=user_items, schema=types.UserItemSchema)
         self.user_items = user_items
-        self.dry_run = dry_run
         self.emitter = emitter
+        self.chunk_size = chunk_size
+        self.dry_run = dry_run
 
     def upload_zipfile(
         self, zip_path: Path, event_payload: T.Optional[Progress] = None
     ) -> T.Optional[str]:
+        if event_payload is None:
+            event_payload = {}
+
         with zipfile.ZipFile(zip_path) as ziph:
             namelist = ziph.namelist()
             if not namelist:
                 LOG.warning(f"Skipping empty zipfile: %s", zip_path)
                 return None
             upload_md5sum = _hash_zipfile(ziph)
 
-        if event_payload is None:
-            event_payload = {}
-
-        new_event_payload: Progress = {
-            "import_path": str(zip_path),
+        final_event_payload: Progress = {
+            **event_payload,  # type: ignore
             "sequence_image_count": len(namelist),
         }
 
         with zip_path.open("rb") as fp:
             try:
-                return _upload_zipfile_fp(
+                return self._upload_fp(
                     fp,
                     upload_md5sum,
-                    len(namelist),
-                    self.user_items,
-                    event_payload=T.cast(
-                        Progress, {**event_payload, **new_event_payload}
-                    ),
-                    emitter=self.emitter,
-                    dry_run=self.dry_run,
+                    "zip",
+                    event_payload=final_event_payload,
                 )
             except UploadCancelled:
                 return None
 
-    def upload_blackvue(
-        self, blackvue_path: Path, event_payload: T.Optional[Progress] = None
+    def upload_blackvue_fp(
+        self, fp: T.IO[bytes], event_payload: T.Optional[Progress] = None
     ) -> T.Optional[str]:
-        try:
-            with blackvue_path.open("rb") as fp:
-                return _upload_video_fp(
-                    fp,
-                    blackvue_path,
-                    self.user_items,
-                    "mly_blackvue_video",
-                    event_payload=event_payload,
-                    emitter=self.emitter,
-                    dry_run=self.dry_run,
-                )
-        except UploadCancelled:
-            return None
+        if event_payload is None:
+            event_payload = {}
 
-    def upload_camm(
-        self, camm_path: Path, event_payload: T.Optional[Progress] = None
-    ) -> T.Optional[str]:
+        upload_md5sum = utils.md5sum_fp(fp)
         try:
-            with camm_path.open("rb") as fp:
-                return _upload_video_fp(
-                    fp,
-                    camm_path,
-                    self.user_items,
-                    "mly_camm_video",
-                    event_payload=event_payload,
-                    emitter=self.emitter,
-                    dry_run=self.dry_run,
-                )
+            return self._upload_fp(
+                fp,
+                upload_md5sum,
+                "mly_blackvue_video",
+                event_payload=event_payload,
+            )
         except UploadCancelled:
             return None
 
     def upload_camm_fp(
         self,
         fp: T.IO[bytes],
-        camm_path: Path,
         event_payload: T.Optional[Progress] = None,
     ) -> T.Optional[str]:
+        if event_payload is None:
+            event_payload = {}
+
+        upload_md5sum = utils.md5sum_fp(fp)
         try:
-            return _upload_video_fp(
+            return self._upload_fp(
                 fp,
-                camm_path,
-                self.user_items,
+                upload_md5sum,
                 "mly_camm_video",
                 event_payload=event_payload,
-                emitter=self.emitter,
-                dry_run=self.dry_run,
             )
         except UploadCancelled:
             return None
 
     def upload_images(
         self,
         descs: T.Sequence[types.ImageDescriptionFile],
         event_payload: T.Optional[Progress] = None,
     ) -> T.Dict[str, str]:
         if event_payload is None:
             event_payload = {}
+
         _validate_descs(descs)
         sequences = _group_sequences_by_uuid(descs)
         ret: T.Dict[str, str] = {}
         for sequence_idx, (sequence_uuid, images) in enumerate(sequences.items()):
             final_event_payload: Progress = {
+                **event_payload,  # type: ignore
                 "sequence_idx": sequence_idx,
                 "total_sequence_count": len(sequences),
                 "sequence_image_count": len(images),
                 "sequence_uuid": sequence_uuid,
             }
-            final_event_payload.update(event_payload)
             with tempfile.NamedTemporaryFile() as fp:
                 upload_md5sum = _zip_sequence_fp(images, fp)
                 try:
-                    cluster_id: T.Optional[str] = _upload_zipfile_fp(
+                    cluster_id: T.Optional[str] = self._upload_fp(
                         fp,
                         upload_md5sum,
-                        len(images),
-                        self.user_items,
-                        emitter=self.emitter,
-                        event_payload=final_event_payload,
-                        dry_run=self.dry_run,
+                        "zip",
+                        final_event_payload,
                     )
                 except UploadCancelled:
                     cluster_id = None
             if cluster_id is not None:
                 ret[sequence_uuid] = cluster_id
         return ret
 
+    def _upload_fp(
+        self,
+        fp: T.IO[bytes],
+        upload_md5sum: str,
+        file_type: upload_api_v4.FileType,
+        event_payload: T.Optional[Progress] = None,
+    ) -> str:
+        if event_payload is None:
+            event_payload = {}
+
+        fp.seek(0, io.SEEK_END)
+        entity_size = fp.tell()
+
+        SUFFIX_MAP: T.Dict[upload_api_v4.FileType, str] = {
+            "zip": ".zip",
+            "mly_camm_video": ".mp4",
+            "mly_blackvue_video": ".mp4",
+        }
+        session_key = f"mly_tools_{upload_md5sum}{SUFFIX_MAP[file_type]}"
+
+        if self.dry_run:
+            upload_service: upload_api_v4.UploadService = (
+                upload_api_v4.FakeUploadService(
+                    user_access_token=self.user_items["user_upload_token"],
+                    session_key=session_key,
+                    entity_size=entity_size,
+                    organization_id=self.user_items.get("MAPOrganizationKey"),
+                    file_type=file_type,
+                    chunk_size=self.chunk_size,
+                )
+            )
+        else:
+            upload_service = upload_api_v4.UploadService(
+                user_access_token=self.user_items["user_upload_token"],
+                session_key=session_key,
+                entity_size=entity_size,
+                organization_id=self.user_items.get("MAPOrganizationKey"),
+                file_type=file_type,
+                chunk_size=self.chunk_size,
+            )
+
+        final_event_payload: Progress = {
+            **event_payload,  # type: ignore
+            "entity_size": entity_size,
+            "md5sum": upload_md5sum,
+        }
+
+        return _upload_fp(
+            upload_service,
+            fp,
+            event_payload=final_event_payload,
+            emitter=self.emitter,
+        )
+
 
 def desc_file_to_exif(
     desc: types.ImageDescriptionFile,
 ) -> types.ImageDescriptionEXIF:
     not_needed = ["MAPPhotoUUID", "MAPSequenceUUID"]
     removed = {
         key: value
@@ -313,116 +346,22 @@
             arcname = f"{md5sum}{ext.lower()}"
             zipinfo = zipfile.ZipInfo(arcname, date_time=(1980, 1, 1, 0, 0, 0))
             ziph.writestr(zipinfo, image_bytes)
 
         return _hash_zipfile(ziph)
 
 
-def _upload_zipfile_fp(
-    fp: T.IO[bytes],
-    upload_md5sum: str,
-    image_count: int,
-    user_items: types.UserItem,
-    event_payload: T.Optional[Progress] = None,
-    emitter: T.Optional[EventEmitter] = None,
-    dry_run=False,
-) -> str:
-    if event_payload is None:
-        event_payload = {
-            "sequence_idx": 0,
-            "total_sequence_count": 1,
-        }
-
-    fp.seek(0, io.SEEK_END)
-    entity_size = fp.tell()
-
-    # chunk size
-    avg_image_size = int(entity_size / image_count)
-    chunk_size = min(max(avg_image_size, MIN_CHUNK_SIZE), MAX_CHUNK_SIZE)
-
-    if dry_run:
-        upload_service: upload_api_v4.UploadService = upload_api_v4.FakeUploadService(
-            user_access_token=user_items["user_upload_token"],
-            session_key=f"mly_tools_{upload_md5sum}.zip",
-            entity_size=entity_size,
-            organization_id=user_items.get("MAPOrganizationKey"),
-        )
-    else:
-        upload_service = upload_api_v4.UploadService(
-            user_access_token=user_items["user_upload_token"],
-            session_key=f"mly_tools_{upload_md5sum}.zip",
-            entity_size=entity_size,
-            organization_id=user_items.get("MAPOrganizationKey"),
-        )
-
-    new_event_payload: Progress = {
-        "entity_size": entity_size,
-        "md5sum": upload_md5sum,
-    }
-
-    return _upload_fp(
-        upload_service,
-        fp,
-        chunk_size,
-        event_payload=T.cast(Progress, {**event_payload, **new_event_payload}),
-        emitter=emitter,
-    )
-
-
-def _upload_video_fp(
-    fp: T.IO[bytes],
-    video_path: Path,
-    user_items: types.UserItem,
-    file_type: upload_api_v4.FileType,
-    event_payload: T.Optional[Progress] = None,
-    emitter: EventEmitter = None,
-    dry_run=False,
-) -> str:
-    upload_md5sum = utils.md5sum_fp(fp)
-
-    fp.seek(0, io.SEEK_END)
-    entity_size = fp.tell()
-
-    # chunk size
-    avg_image_size = entity_size
-    chunk_size = min(max(avg_image_size, MIN_CHUNK_SIZE), MAX_CHUNK_SIZE)
-
-    if dry_run:
-        upload_service: upload_api_v4.UploadService = upload_api_v4.FakeUploadService(
-            user_access_token=user_items["user_upload_token"],
-            session_key=f"mly_tools_{upload_md5sum}.mp4",
-            entity_size=entity_size,
-            organization_id=user_items.get("MAPOrganizationKey"),
-            file_type=file_type,
-        )
-    else:
-        upload_service = upload_api_v4.UploadService(
-            user_access_token=user_items["user_upload_token"],
-            session_key=f"mly_tools_{upload_md5sum}.mp4",
-            entity_size=entity_size,
-            organization_id=user_items.get("MAPOrganizationKey"),
-            file_type=file_type,
-        )
-
-    if event_payload is None:
-        event_payload = {}
-
-    new_event_payload: Progress = {
-        "entity_size": entity_size,
-        "import_path": str(video_path),
-        "md5sum": upload_md5sum,
-    }
-
-    return _upload_fp(
-        upload_service,
-        fp,
-        chunk_size,
-        event_payload=T.cast(Progress, {**event_payload, **new_event_payload}),
-        emitter=emitter,
-    )
+def is_immediate_retry(ex: Exception):
+    if isinstance(ex, requests.HTTPError) and ex.response.status_code == 412:
+        try:
+            resp = ex.response.json()
+        except json.JSONDecodeError:
+            return False
+        # resp: {"debug_info":{"retriable":true,"type":"OffsetInvalidError","message":"Request starting offset is invalid"}}
+        return resp.get("debug_info", {}).get("retriable", False)
 
 
 def is_retriable_exception(ex: Exception):
     if isinstance(ex, (requests.ConnectionError, requests.Timeout)):
         return True
 
     if isinstance(ex, requests.HTTPError):
@@ -447,17 +386,16 @@
 
     return _callback
 
 
 def _upload_fp(
     upload_service: upload_api_v4.UploadService,
     fp: T.IO[bytes],
-    chunk_size: int,
-    event_payload: Progress = None,
-    emitter: EventEmitter = None,
+    event_payload: T.Optional[Progress] = None,
+    emitter: T.Optional[EventEmitter] = None,
 ) -> str:
     retries = 0
 
     if event_payload is None:
         event_payload = {}
 
     mutable_payload = T.cast(Progress, {**event_payload})
@@ -466,66 +404,62 @@
     def _reset_retries(_, __):
         nonlocal retries
         retries = 0
 
     if emitter:
         emitter.emit("upload_start", mutable_payload)
 
-    MAX_RETRIES = 200
-
-    offset = None
-
     while True:
         fp.seek(0, io.SEEK_SET)
+        begin_offset: T.Optional[int] = None
         try:
-            offset = upload_service.fetch_offset()
+            begin_offset = upload_service.fetch_offset()
             upload_service.callbacks = [_reset_retries]
             if emitter:
-                mutable_payload["offset"] = offset
+                mutable_payload["offset"] = begin_offset
                 mutable_payload["retries"] = retries
                 emitter.emit("upload_fetch_offset", mutable_payload)
                 upload_service.callbacks.append(
                     _setup_callback(emitter, mutable_payload)
                 )
-            file_handle = upload_service.upload(
-                fp, chunk_size=chunk_size, offset=offset
-            )
+            file_handle = upload_service.upload(fp, offset=begin_offset)
         except Exception as ex:
-            if retries < MAX_RETRIES and is_retriable_exception(ex):
+            if retries < constants.MAX_UPLOAD_RETRIES and is_retriable_exception(ex):
                 if emitter:
                     emitter.emit("upload_interrupted", mutable_payload)
-                retries += 1
-                sleep_for = min(2**retries, 16)
                 LOG.warning(
                     # use %s instead of %d because offset could be None
-                    f"Error uploading chunk_size %d at offset %s: %s: %s",
-                    chunk_size,
-                    offset,
+                    f"Error uploading chunk_size %d at begin_offset %s: %s: %s",
+                    upload_service.chunk_size,
+                    begin_offset,
                     ex.__class__.__name__,
                     str(ex),
                 )
+                retries += 1
+                if is_immediate_retry(ex):
+                    sleep_for = 0
+                else:
+                    sleep_for = min(2**retries, 16)
                 LOG.info(
-                    "Retrying in %d seconds (%d/%d)", sleep_for, retries, MAX_RETRIES
+                    "Retrying in %d seconds (%d/%d)",
+                    sleep_for,
+                    retries,
+                    constants.MAX_UPLOAD_RETRIES,
                 )
-                time.sleep(sleep_for)
+                if sleep_for:
+                    time.sleep(sleep_for)
             else:
-                if isinstance(ex, requests.HTTPError):
-                    raise upload_api_v4.wrap_http_exception(ex) from ex
-                else:
-                    raise ex
+                raise ex
         else:
             break
 
     if emitter:
         emitter.emit("upload_end", mutable_payload)
 
     # TODO: retry here
-    try:
-        cluster_id = upload_service.finish(file_handle)
-    except requests.HTTPError as ex:
-        raise upload_api_v4.wrap_http_exception(ex) from ex
+    cluster_id = upload_service.finish(file_handle)
 
     if emitter:
         mutable_payload["cluster_id"] = cluster_id
         emitter.emit("upload_finished", mutable_payload)
 
     return cluster_id
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools/utils.py` & `mapillary_tools-0.9.5/mapillary_tools/utils.py`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/mapillary_tools.egg-info/PKG-INFO` & `mapillary_tools-0.9.5/mapillary_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapillary-tools
-Version: 0.9.4
+Version: 0.9.5
 Summary: Mapillary Image/Video Import Pipeline
 Home-page: https://github.com/mapillary/mapillary_tools
 Author: Mapillary
 License: BSD
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapillary-tools Version: 0.9.4 Summary: Mapillary
+Metadata-Version: 2.1 Name: mapillary-tools Version: 0.9.5 Summary: Mapillary
 Image/Video Import Pipeline Home-page: https://github.com/mapillary/
 mapillary_tools Author: Mapillary License: BSD Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
 [https://raw.githubusercontent.com/mapillary/mapillary_tools/main/docs/images/
                                    logo.png]
                ***** Process and upload Mapillary imagery *****
       [PyPI] [Actions_Status] [GitHub_license] [GitHub_stars] [Downloads]
```

### Comparing `mapillary_tools-0.9.4/mapillary_tools.egg-info/SOURCES.txt` & `mapillary_tools-0.9.5/mapillary_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,24 +43,25 @@
 mapillary_tools/commands/video_process.py
 mapillary_tools/commands/video_process_and_upload.py
 mapillary_tools/commands/zip.py
 mapillary_tools/geotag/__init__.py
 mapillary_tools/geotag/blackvue_parser.py
 mapillary_tools/geotag/camm_builder.py
 mapillary_tools/geotag/camm_parser.py
+mapillary_tools/geotag/construct_mp4_parser.py
 mapillary_tools/geotag/geotag_from_blackvue.py
 mapillary_tools/geotag/geotag_from_camm.py
 mapillary_tools/geotag/geotag_from_exif.py
 mapillary_tools/geotag/geotag_from_generic.py
 mapillary_tools/geotag/geotag_from_gopro.py
 mapillary_tools/geotag/geotag_from_gpx.py
 mapillary_tools/geotag/geotag_from_gpx_file.py
 mapillary_tools/geotag/geotag_from_nmea_file.py
 mapillary_tools/geotag/gpmf_gps_filter.py
 mapillary_tools/geotag/gpmf_parser.py
 mapillary_tools/geotag/gps_filter.py
 mapillary_tools/geotag/io_utils.py
-mapillary_tools/geotag/mp4_optimizer.py
+mapillary_tools/geotag/mp4_sample_parser.py
 mapillary_tools/geotag/simple_mp4_builder.py
 mapillary_tools/geotag/simple_mp4_parser.py
 mapillary_tools/geotag/utils.py
 schema/image_description_schema.json
```

### Comparing `mapillary_tools-0.9.4/schema/image_description_schema.json` & `mapillary_tools-0.9.5/schema/image_description_schema.json`

 * *Files identical despite different names*

### Comparing `mapillary_tools-0.9.4/setup.py` & `mapillary_tools-0.9.5/setup.py`

 * *Files identical despite different names*

