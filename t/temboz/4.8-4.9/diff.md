# Comparing `tmp/temboz-4.8.tar.gz` & `tmp/temboz-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temboz-4.8.tar", last modified: Thu May 11 12:34:45 2023, max compression
+gzip compressed data, was "temboz-4.9.tar", last modified: Sat May 20 14:55:59 2023, max compression
```

## Comparing `temboz-4.8.tar` & `temboz-4.9.tar`

### file list

```diff
@@ -1,551 +1,551 @@
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.426349 temboz-4.8/
--rw-r--r--   0 majid     (1001) engineers    (11)       87 2017-10-20 17:55:01.000000 temboz-4.8/.codebeatignore
--rw-r--r--   0 majid     (1001) engineers    (11)      102 2020-11-09 18:38:13.000000 temboz-4.8/.gitignore
--rw-r--r--   0 majid     (1001) engineers    (11)      575 2019-10-15 15:39:31.000000 temboz-4.8/Dockerfile
--rw-r--r--   0 majid     (1001) engineers    (11)     1054 2017-06-09 12:18:20.000000 temboz-4.8/LICENSE
--rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.8/MANIFEST.in
--rw-r--r--   0 majid     (1001) engineers    (11)     1775 2021-05-07 18:02:43.000000 temboz-4.8/Makefile
--rw-r--r--   0 majid     (1001) engineers    (11)     4880 2023-05-11 12:34:45.426349 temboz-4.8/PKG-INFO
--rw-r--r--   0 majid     (1001) engineers    (11)     4314 2020-10-26 23:24:50.000000 temboz-4.8/README.md
--rw-r--r--   0 majid     (1001) engineers    (11)      886 2016-07-20 04:47:16.000000 temboz-4.8/UPGRADE
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.349682 temboz-4.8/bugfeed/
--rw-r--r--   0 majid     (1001) engineers    (11)    62524 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/DigitalOutbackPhoto_News.xml
--rw-r--r--   0 majid     (1001) engineers    (11)   215624 2020-02-01 21:07:52.000000 temboz-4.8/bugfeed/PetaPixel
--rw-r--r--   0 majid     (1001) engineers    (11)    76181 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/QuantifiedSelf
--rw-r--r--   0 majid     (1001) engineers    (11)    31209 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/barnett
--rw-r--r--   0 majid     (1001) engineers    (11)    86626 2020-11-09 17:41:27.000000 temboz-4.8/bugfeed/boingboing
--rw-r--r--   0 majid     (1001) engineers    (11)   136355 2020-08-26 21:32:47.000000 temboz-4.8/bugfeed/calmatters
--rw-r--r--   0 majid     (1001) engineers    (11)    71401 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/case1
--rw-r--r--   0 majid     (1001) engineers    (11)   175269 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/case2
--rw-r--r--   0 majid     (1001) engineers    (11)    10798 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/case3
--rw-r--r--   0 majid     (1001) engineers    (11)    38530 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/cooltools
--rw-r--r--   0 majid     (1001) engineers    (11)    85842 2020-10-29 20:21:22.000000 temboz-4.8/bugfeed/greenwald
--rw-r--r--   0 majid     (1001) engineers    (11)   159523 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/nettuts
--rw-r--r--   0 majid     (1001) engineers    (11)    61492 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/russellbeattieweblog
--rw-r--r--   0 majid     (1001) engineers    (11)    38305 2017-02-23 02:16:15.000000 temboz-4.8/bugfeed/tokyo
--rw-r--r--   0 majid     (1001) engineers    (11)    98458 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/tychay
--rw-r--r--   0 majid     (1001) engineers    (11)    41930 2016-07-20 04:47:17.000000 temboz-4.8/bugfeed/typographica
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.349682 temboz-4.8/etc/
--rw-r--r--   0 majid     (1001) engineers    (11)     2735 2016-07-20 04:47:16.000000 temboz-4.8/etc/db_0.5.sh
--rwxr-xr-x   0 majid     (1001) engineers    (11)     1089 2019-10-15 15:39:31.000000 temboz-4.8/etc/norm_url.py
--rw-r--r--   0 majid     (1001) engineers    (11)      887 2019-10-15 15:39:31.000000 temboz-4.8/etc/resolveguid.py
--rw-r--r--   0 majid     (1001) engineers    (11)   115785 2017-02-26 12:29:31.000000 temboz-4.8/me.opml
--rw-r--r--   0 majid     (1001) engineers    (11)       13 2020-04-27 13:16:50.000000 temboz-4.8/pyproject.toml
--rw-r--r--   0 majid     (1001) engineers    (11)      696 2022-08-05 10:46:43.000000 temboz-4.8/sanity.py
--rw-r--r--   0 majid     (1001) engineers    (11)       38 2023-05-11 12:34:45.426349 temboz-4.8/setup.cfg
--rw-r--r--   0 majid     (1001) engineers    (11)     1050 2023-05-11 12:25:10.000000 temboz-4.8/setup.py
--rwxr-xr-x   0 majid     (1001) engineers    (11)     2926 2022-03-16 15:08:42.000000 temboz-4.8/temboz
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.349682 temboz-4.8/temboz.egg-info/
--rw-r--r--   0 majid     (1001) engineers    (11)     4880 2023-05-11 12:34:45.000000 temboz-4.8/temboz.egg-info/PKG-INFO
--rw-r--r--   0 majid     (1001) engineers    (11)    23015 2023-05-11 12:34:45.000000 temboz-4.8/temboz.egg-info/SOURCES.txt
--rw-r--r--   0 majid     (1001) engineers    (11)        1 2023-05-11 12:34:45.000000 temboz-4.8/temboz.egg-info/dependency_links.txt
--rw-r--r--   0 majid     (1001) engineers    (11)      128 2023-05-11 12:34:45.000000 temboz-4.8/temboz.egg-info/requires.txt
--rw-r--r--   0 majid     (1001) engineers    (11)       10 2023-05-11 12:34:45.000000 temboz-4.8/temboz.egg-info/top_level.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.356349 temboz-4.8/tembozapp/
--rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/__init__.py
--rw-r--r--   0 majid     (1001) engineers    (11)     1247 2022-09-22 19:02:31.000000 temboz-4.8/tembozapp/aia.py
--rw-r--r--   0 majid     (1001) engineers    (11)     1589 2020-11-18 12:30:40.000000 temboz-4.8/tembozapp/autodiscovery.py
--rw-r--r--   0 majid     (1001) engineers    (11)     3595 2019-10-15 15:39:31.000000 temboz-4.8/tembozapp/bootstrap.py
--rw-r--r--   0 majid     (1001) engineers    (11)    18039 2022-06-08 21:41:43.000000 temboz-4.8/tembozapp/dbop.py
--rw-r--r--   0 majid     (1001) engineers    (11)     3142 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/ddl.sql
--rw-r--r--   0 majid     (1001) engineers    (11)     5409 2022-06-08 17:34:16.000000 temboz-4.8/tembozapp/degunk.py
--rw-r--r--   0 majid     (1001) engineers    (11)     2481 2020-10-29 20:48:27.000000 temboz-4.8/tembozapp/feedfix.py
--rw-r--r--   0 majid     (1001) engineers    (11)    12795 2022-06-08 20:29:22.000000 temboz-4.8/tembozapp/filters.py
--rw-r--r--   0 majid     (1001) engineers    (11)     2838 2023-01-11 20:20:56.000000 temboz-4.8/tembozapp/fts5.py
--rw-r--r--   0 majid     (1001) engineers    (11)    33022 2022-07-26 00:38:50.000000 temboz-4.8/tembozapp/normalize.py
--rw-r--r--   0 majid     (1001) engineers    (11)     2633 2022-03-16 15:08:42.000000 temboz-4.8/tembozapp/opml.py
--rw-r--r--   0 majid     (1001) engineers    (11)     2795 2020-06-03 04:24:13.000000 temboz-4.8/tembozapp/param.py
--rw-r--r--   0 majid     (1001) engineers    (11)     8455 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/porter2.py
--rw-r--r--   0 majid     (1001) engineers    (11)    30480 2023-05-11 12:23:43.000000 temboz-4.8/tembozapp/server.py
--rw-r--r--   0 majid     (1001) engineers    (11)     1098 2020-03-31 11:12:59.000000 temboz-4.8/tembozapp/sop.py
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.356349 temboz-4.8/tembozapp/static/
--rw-r--r--   0 majid     (1001) engineers    (11)       52 2018-08-08 18:25:00.000000 temboz-4.8/tembozapp/static/add.js
--rw-r--r--   0 majid     (1001) engineers    (11)   136091 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/dygraph-combined.js
--rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/iphone.css
--rw-r--r--   0 majid     (1001) engineers    (11)     1076 2018-05-05 07:28:18.000000 temboz-4.8/tembozapp/static/item.mst
--rw-r--r--   0 majid     (1001) engineers    (11)    23522 2021-09-22 09:25:31.000000 temboz-4.8/tembozapp/static/mustache.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3035 2021-09-22 09:23:47.000000 temboz-4.8/tembozapp/static/specific.js
--rw-r--r--   0 majid     (1001) engineers    (11)    10392 2021-05-07 18:03:17.000000 temboz-4.8/tembozapp/static/temboz.css
--rw-r--r--   0 majid     (1001) engineers    (11)   478942 2021-09-22 09:25:31.000000 temboz-4.8/tembozapp/static/temboz.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/
--rw-r--r--   0 majid     (1001) engineers    (11)      213 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/blank.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     1650 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)      304 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/langs/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)    23672 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/license.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/
--rw-r--r--   0 majid     (1001) engineers    (11)     2039 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     8563 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/images/
--rw-r--r--   0 majid     (1001) engineers    (11)       87 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/images/template.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      240 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1524 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/popup.htm
--rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.359682 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      299 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/css/advhr.css
--rw-r--r--   0 majid     (1001) engineers    (11)     2128 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3024 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      153 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/images/advhr.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)     1128 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/jscripts/rule.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      192 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)     2721 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/rule.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      835 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/css/advimage.css
--rw-r--r--   0 majid     (1001) engineers    (11)     3264 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     4603 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)    10595 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/image.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/images/
--rw-r--r--   0 majid     (1001) engineers    (11)     1624 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/images/sample.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)    16256 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/jscripts/functions.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      931 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      594 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/css/advlink.css
--rw-r--r--   0 majid     (1001) engineers    (11)     1978 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2742 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)    18473 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/jscripts/functions.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.363016 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     1434 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)    14866 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/link.htm
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/
--rw-r--r--   0 majid     (1001) engineers    (11)      802 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1263 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      149 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/cleanup/
--rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/cleanup/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)      383 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/cleanup/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)       52 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/cleanup/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/css/
--rw-r--r--   0 majid     (1001) engineers    (11)     1226 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/css/contextmenu.css
--rw-r--r--   0 majid     (1001) engineers    (11)    11005 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)    14711 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/images/
--rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/images/spacer.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/
--rw-r--r--   0 majid     (1001) engineers    (11)     2099 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2837 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.366349 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      155 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/images/ltr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      153 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/images/rtl.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.369682 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      160 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.369682 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/
--rw-r--r--   0 majid     (1001) engineers    (11)     1105 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1881 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)     4409 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/emotions.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      319 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/emotions.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      150 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)      354 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-cool.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      329 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-cry.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      331 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-embarassed.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      344 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-foot-in-mouth.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      340 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-frown.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      336 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-innocent.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      338 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-kiss.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      344 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-laughing.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      321 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-money-mouth.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      325 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-sealed.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      345 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-smile.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      342 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-surprised.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      328 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-tongue-out.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      337 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-undecided.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      351 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-wink.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      336 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-yell.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)      666 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/jscripts/functions.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      461 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      190 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/css/content.css
--rw-r--r--   0 majid     (1001) engineers    (11)      119 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/css/flash.css
--rw-r--r--   0 majid     (1001) engineers    (11)     7030 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     9871 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2800 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/flash.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      241 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/images/flash.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)     3437 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/jscripts/flash.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.373016 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      251 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/
--rw-r--r--   0 majid     (1001) engineers    (11)      229 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/blank.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/css/
--rw-r--r--   0 majid     (1001) engineers    (11)     2876 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/css/fullpage.css
--rw-r--r--   0 majid     (1001) engineers    (11)     5072 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     7372 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)    26164 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/fullpage.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      893 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/add.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      632 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/fullpage.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      194 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/move_down.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      200 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/move_up.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      180 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/remove.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)    18594 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/fullpage.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     2744 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/langs/en.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/
--rw-r--r--   0 majid     (1001) engineers    (11)     1538 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2160 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3268 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/fullscreen.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      198 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/images/fullscreen.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.376349 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      136 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/
--rw-r--r--   0 majid     (1001) engineers    (11)     1195 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1916 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      124 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/images/iespell.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/css/
--rw-r--r--   0 majid     (1001) engineers    (11)     1030 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/css/inlinepopup.css
--rw-r--r--   0 majid     (1001) engineers    (11)    15998 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)    20815 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/
--rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/spacer.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_close.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_maximize.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_minimize.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       74 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_resize.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)    14517 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/mcwindows.js
--rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.379683 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/
--rw-r--r--   0 majid     (1001) engineers    (11)     2744 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3766 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      287 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/images/insertdate.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      239 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/images/inserttime.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      682 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/
--rw-r--r--   0 majid     (1001) engineers    (11)     5031 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     6897 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      209 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/images/absolute.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      360 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/images/backward.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      358 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/images/forward.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      264 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/images/insert_layer.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      238 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.383016 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      395 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/css/noneditable.css
--rw-r--r--   0 majid     (1001) engineers    (11)     3339 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     5127 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/
--rw-r--r--   0 majid     (1001) engineers    (11)      496 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/blank.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      395 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/css/blank.css
--rw-r--r--   0 majid     (1001) engineers    (11)       49 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/css/pasteword.css
--rw-r--r--   0 majid     (1001) engineers    (11)     9320 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)    13678 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      294 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/images/pastetext.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      299 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/images/pasteword.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      205 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/images/selectall.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)      816 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/jscripts/pastetext.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1282 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/jscripts/pasteword.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      380 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1454 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/pastetext.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1135 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/pasteword.htm
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/
--rw-r--r--   0 majid     (1001) engineers    (11)     2159 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3107 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)      314 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/example.html
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      286 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/images/preview.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.386349 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/
--rw-r--r--   0 majid     (1001) engineers    (11)      811 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1344 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      211 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/images/print.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/print/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)       49 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/
--rw-r--r--   0 majid     (1001) engineers    (11)     2066 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3313 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      285 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/images/save.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/save/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/
--rw-r--r--   0 majid     (1001) engineers    (11)     4444 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     6177 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      125 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/images/replace.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      191 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/images/search.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)     1306 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/replace.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1082 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/search.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.389683 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)      827 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)     2585 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/replace.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     2029 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/search.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/css/
--rw-r--r--   0 majid     (1001) engineers    (11)     1173 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/css/props.css
--rw-r--r--   0 majid     (1001) engineers    (11)     1335 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2033 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/images/
--rw-r--r--   0 majid     (1001) engineers    (11)     1096 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/images/apply_button_bg.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      562 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/images/style_info.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)    29556 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/jscripts/props.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     1550 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)    28854 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/props.htm
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/style/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/
--rw-r--r--   0 majid     (1001) engineers    (11)     6960 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/cell.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.393016 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      205 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/css/cell.css
--rw-r--r--   0 majid     (1001) engineers    (11)      306 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/css/row.css
--rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/css/table.css
--rw-r--r--   0 majid     (1001) engineers    (11)    20104 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)    30559 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/editor_plugin_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.396349 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/
--rw-r--r--   0 majid     (1001) engineers    (11)     1356 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/buttons.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      287 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      189 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_cell_props.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      372 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_delete.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      163 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_delete_col.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      171 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_delete_row.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      165 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_insert_col_after.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      165 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_insert_col_before.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      163 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_insert_row_after.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      159 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_insert_row_before.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      198 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_merge_cells.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      187 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_row_props.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      210 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/table_split_cells.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.396349 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)     7901 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/cell.js
--rw-r--r--   0 majid     (1001) engineers    (11)      489 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/merge_cells.js
--rw-r--r--   0 majid     (1001) engineers    (11)     6395 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/row.js
--rw-r--r--   0 majid     (1001) engineers    (11)    11734 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/table.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.396349 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     2593 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1410 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/merge_cells.htm
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/readme.txt
--rw-r--r--   0 majid     (1001) engineers    (11)     6016 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/row.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     6812 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/table/table.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.396349 temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/
--rw-r--r--   0 majid     (1001) engineers    (11)     1173 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1789 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/readme.txt
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.339682 temboz-4.8/tembozapp/static/tiny_mce/themes/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.399683 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/
--rw-r--r--   0 majid     (1001) engineers    (11)     2411 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/about.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1142 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/anchor.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     2591 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/charmap.htm
--rw-r--r--   0 majid     (1001) engineers    (11)      554 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/color_picker.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.399683 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/
--rw-r--r--   0 majid     (1001) engineers    (11)     1263 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_content.css
--rw-r--r--   0 majid     (1001) engineers    (11)     5536 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_popup.css
--rw-r--r--   0 majid     (1001) engineers    (11)     7017 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_ui.css
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.339682 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.403016 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/
--rw-r--r--   0 majid     (1001) engineers    (11)      977 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/about.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     6769 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/common_buttons.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     3401 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/create_accessible_content.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.403016 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/
--rw-r--r--   0 majid     (1001) engineers    (11)     5189 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_anchor_window.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     7195 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_image_window.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     5658 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_link_window.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     7094 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_table_window.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     1104 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/index.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1061 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_anchor_button.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1964 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_image_button.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1082 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_link_button.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1946 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_table_button.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1320 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/style.css
--rw-r--r--   0 majid     (1001) engineers    (11)    40216 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/editor_template.js
--rw-r--r--   0 majid     (1001) engineers    (11)    53294 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/editor_template_src.js
--rw-r--r--   0 majid     (1001) engineers    (11)     4891 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/image.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.413016 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/
--rw-r--r--   0 majid     (1001) engineers    (11)      171 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/anchor.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/anchor_symbol.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      174 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/backcolor.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold_de_se.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       80 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold_es.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold_fr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      207 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bold_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      113 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/browse.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      108 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/bullist.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/button_menu.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     8399 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/buttons.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      677 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/cancel_button_bg.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/charmap.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      256 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/cleanup.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      102 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/close.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/code.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      125 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/color.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      263 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/copy.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/custom_1.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      187 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/cut.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      272 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/forecolor.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      295 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/help.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       63 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/hr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      194 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/image.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/indent.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      703 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/insert_button_bg.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/italic.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/italic_de_se.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       74 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/italic_es.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/italic_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      274 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/italic_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/justifycenter.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       71 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/justifyfull.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       71 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/justifyleft.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/justifyright.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/link.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       51 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/menu_check.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/newdocument.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/numlist.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      147 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/opacity.png
--rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/outdent.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      286 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/paste.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/redo.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      168 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/removeformat.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/separator.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/spacer.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/statusbar_resize.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       83 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/strikethrough.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      148 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/sub.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      147 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/sup.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/underline.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/underline_es.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/underline_fr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/underline_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/underline_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/undo.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      190 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/unlink.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      206 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/visualaid.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.413016 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/
--rw-r--r--   0 majid     (1001) engineers    (11)      694 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_bg.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_end.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      428 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_sel_bg.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      101 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_sel_end.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       48 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tabs_bg.gif
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.416349 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/
--rw-r--r--   0 majid     (1001) engineers    (11)     2616 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/about.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1992 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/anchor.js
--rw-r--r--   0 majid     (1001) engineers    (11)    15097 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/charmap.js
--rw-r--r--   0 majid     (1001) engineers    (11)     5030 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/color_picker.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3003 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/image.js
--rw-r--r--   0 majid     (1001) engineers    (11)     2459 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/link.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1909 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/source_editor.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.416349 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/langs/
--rw-r--r--   0 majid     (1001) engineers    (11)     2862 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/langs/en.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3901 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/link.htm
--rw-r--r--   0 majid     (1001) engineers    (11)     1334 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/source_editor.htm
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.416349 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.416349 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/
--rw-r--r--   0 majid     (1001) engineers    (11)      513 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_content.css
--rw-r--r--   0 majid     (1001) engineers    (11)      805 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_popup.css
--rw-r--r--   0 majid     (1001) engineers    (11)     2296 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_ui.css
--rw-r--r--   0 majid     (1001) engineers    (11)     2840 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/editor_template.js
--rw-r--r--   0 majid     (1001) engineers    (11)     3582 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/editor_template_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.419683 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/
--rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bold.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bold_de_se.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bold_fr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bold_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      207 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bold_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      108 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/bullist.gif
--rw-r--r--   0 majid     (1001) engineers    (11)     1054 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/buttons.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      256 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/cleanup.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/italic.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/italic_de_se.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/italic_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      274 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/italic_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/numlist.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/redo.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/separator.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/spacer.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       83 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/strikethrough.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/underline.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/underline_fr.gif
--rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/underline_ru.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/underline_tw.gif
--rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/undo.gif
--rw-r--r--   0 majid     (1001) engineers    (11)   136939 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/tiny_mce.js
--rw-r--r--   0 majid     (1001) engineers    (11)     7364 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/tiny_mce_popup.js
--rw-r--r--   0 majid     (1001) engineers    (11)   194076 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/tiny_mce_src.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.419683 temboz-4.8/tembozapp/static/tiny_mce/utils/
--rw-r--r--   0 majid     (1001) engineers    (11)     1801 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/utils/editable_selects.js
--rw-r--r--   0 majid     (1001) engineers    (11)     6329 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/utils/form_utils.js
--rw-r--r--   0 majid     (1001) engineers    (11)     4357 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/utils/mclayer.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1841 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/utils/mctabs.js
--rw-r--r--   0 majid     (1001) engineers    (11)     1724 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/static/tiny_mce/utils/validate.js
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.423016 temboz-4.8/tembozapp/templates/
--rw-r--r--   0 majid     (1001) engineers    (11)     1186 2020-08-31 19:52:31.000000 temboz-4.8/tembozapp/templates/_share.atom
--rw-r--r--   0 majid     (1001) engineers    (11)     1085 2018-08-08 18:25:33.000000 temboz-4.8/tembozapp/templates/add.html
--rw-r--r--   0 majid     (1001) engineers    (11)     1361 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/templates/edit.html
--rw-r--r--   0 majid     (1001) engineers    (11)     6173 2023-03-07 13:54:33.000000 temboz-4.8/tembozapp/templates/feed.html
--rw-r--r--   0 majid     (1001) engineers    (11)      683 2019-10-28 12:30:01.000000 temboz-4.8/tembozapp/templates/feed_debug.html
--rw-r--r--   0 majid     (1001) engineers    (11)     3569 2021-01-28 01:11:49.000000 temboz-4.8/tembozapp/templates/feeds.html
--rw-r--r--   0 majid     (1001) engineers    (11)     1617 2019-09-24 22:46:49.000000 temboz-4.8/tembozapp/templates/login.html
--rw-r--r--   0 majid     (1001) engineers    (11)     2308 2020-10-14 18:12:17.000000 temboz-4.8/tembozapp/templates/menubar.html
--rw-r--r--   0 majid     (1001) engineers    (11)     3156 2018-05-06 10:21:59.000000 temboz-4.8/tembozapp/templates/offline.html
--rw-r--r--   0 majid     (1001) engineers    (11)      549 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/templates/opml.opml
--rw-r--r--   0 majid     (1001) engineers    (11)      472 2017-02-26 12:29:31.000000 temboz-4.8/tembozapp/templates/rules.html
--rw-r--r--   0 majid     (1001) engineers    (11)     6957 2020-12-30 12:28:01.000000 temboz-4.8/tembozapp/templates/rules_common.html
--rw-r--r--   0 majid     (1001) engineers    (11)    12280 2022-06-08 21:05:10.000000 temboz-4.8/tembozapp/templates/settings.html
--rw-r--r--   0 majid     (1001) engineers    (11)     1037 2020-05-26 09:58:27.000000 temboz-4.8/tembozapp/templates/threads.html
--rw-r--r--   0 majid     (1001) engineers    (11)    11961 2023-01-27 12:39:27.000000 temboz-4.8/tembozapp/templates/view.html
--rw-r--r--   0 majid     (1001) engineers    (11)    12124 2022-06-08 17:13:28.000000 temboz-4.8/tembozapp/transform.py
--rw-r--r--   0 majid     (1001) engineers    (11)    26737 2023-03-07 14:13:13.000000 temboz-4.8/tembozapp/update.py
--rw-r--r--   0 majid     (1001) engineers    (11)      908 2022-03-16 15:08:42.000000 temboz-4.8/tembozapp/urldedup.py
--rw-r--r--   0 majid     (1001) engineers    (11)     1203 2019-10-15 15:39:31.000000 temboz-4.8/tembozapp/util.py
-drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-11 12:34:45.426349 temboz-4.8/test/
--rw-r--r--   0 majid     (1001) engineers    (11)      376 2016-07-20 04:47:17.000000 temboz-4.8/test/category.opml
--rw-r--r--   0 majid     (1001) engineers    (11)     1634 2016-07-20 04:47:17.000000 temboz-4.8/test/directory.opml
--rw-r--r--   0 majid     (1001) engineers    (11)     1343 2016-07-20 04:47:17.000000 temboz-4.8/test/placesLived.opml
--rw-r--r--   0 majid     (1001) engineers    (11)     1390 2016-07-20 04:47:17.000000 temboz-4.8/test/simpleScript.opml
--rw-r--r--   0 majid     (1001) engineers    (11)     2837 2016-07-20 04:47:17.000000 temboz-4.8/test/states.opml
--rw-r--r--   0 majid     (1001) engineers    (11)     4687 2016-07-20 04:47:17.000000 temboz-4.8/test/subscriptionList.opml
--rwxr-xr-x   0 majid     (1001) engineers    (11)     2194 2023-02-09 19:18:28.000000 temboz-4.8/test.py
--rw-r--r--   0 majid     (1001) engineers    (11)      368 2020-08-27 11:56:31.000000 temboz-4.8/unit_test.py
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.883499 temboz-4.9/
+-rw-r--r--   0 majid     (1001) engineers    (11)       87 2017-10-20 17:55:01.000000 temboz-4.9/.codebeatignore
+-rw-r--r--   0 majid     (1001) engineers    (11)      102 2020-11-09 18:38:13.000000 temboz-4.9/.gitignore
+-rw-r--r--   0 majid     (1001) engineers    (11)      575 2019-10-15 15:39:31.000000 temboz-4.9/Dockerfile
+-rw-r--r--   0 majid     (1001) engineers    (11)     1054 2017-06-09 12:18:20.000000 temboz-4.9/LICENSE
+-rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.9/MANIFEST.in
+-rw-r--r--   0 majid     (1001) engineers    (11)     1775 2021-05-07 18:02:43.000000 temboz-4.9/Makefile
+-rw-r--r--   0 majid     (1001) engineers    (11)     4880 2023-05-20 14:55:59.883499 temboz-4.9/PKG-INFO
+-rw-r--r--   0 majid     (1001) engineers    (11)     4314 2020-10-26 23:24:50.000000 temboz-4.9/README.md
+-rw-r--r--   0 majid     (1001) engineers    (11)      886 2016-07-20 04:47:16.000000 temboz-4.9/UPGRADE
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.803498 temboz-4.9/bugfeed/
+-rw-r--r--   0 majid     (1001) engineers    (11)    62524 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/DigitalOutbackPhoto_News.xml
+-rw-r--r--   0 majid     (1001) engineers    (11)   215624 2020-02-01 21:07:52.000000 temboz-4.9/bugfeed/PetaPixel
+-rw-r--r--   0 majid     (1001) engineers    (11)    76181 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/QuantifiedSelf
+-rw-r--r--   0 majid     (1001) engineers    (11)    31209 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/barnett
+-rw-r--r--   0 majid     (1001) engineers    (11)    86626 2020-11-09 17:41:27.000000 temboz-4.9/bugfeed/boingboing
+-rw-r--r--   0 majid     (1001) engineers    (11)   136355 2020-08-26 21:32:47.000000 temboz-4.9/bugfeed/calmatters
+-rw-r--r--   0 majid     (1001) engineers    (11)    71401 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/case1
+-rw-r--r--   0 majid     (1001) engineers    (11)   175269 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/case2
+-rw-r--r--   0 majid     (1001) engineers    (11)    10798 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/case3
+-rw-r--r--   0 majid     (1001) engineers    (11)    38530 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/cooltools
+-rw-r--r--   0 majid     (1001) engineers    (11)    85842 2020-10-29 20:21:22.000000 temboz-4.9/bugfeed/greenwald
+-rw-r--r--   0 majid     (1001) engineers    (11)   159523 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/nettuts
+-rw-r--r--   0 majid     (1001) engineers    (11)    61492 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/russellbeattieweblog
+-rw-r--r--   0 majid     (1001) engineers    (11)    38305 2017-02-23 02:16:15.000000 temboz-4.9/bugfeed/tokyo
+-rw-r--r--   0 majid     (1001) engineers    (11)    98458 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/tychay
+-rw-r--r--   0 majid     (1001) engineers    (11)    41930 2016-07-20 04:47:17.000000 temboz-4.9/bugfeed/typographica
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.806832 temboz-4.9/etc/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2735 2016-07-20 04:47:16.000000 temboz-4.9/etc/db_0.5.sh
+-rwxr-xr-x   0 majid     (1001) engineers    (11)     1089 2019-10-15 15:39:31.000000 temboz-4.9/etc/norm_url.py
+-rw-r--r--   0 majid     (1001) engineers    (11)      887 2019-10-15 15:39:31.000000 temboz-4.9/etc/resolveguid.py
+-rw-r--r--   0 majid     (1001) engineers    (11)   115785 2017-02-26 12:29:31.000000 temboz-4.9/me.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)       13 2020-04-27 13:16:50.000000 temboz-4.9/pyproject.toml
+-rw-r--r--   0 majid     (1001) engineers    (11)      696 2022-08-05 10:46:43.000000 temboz-4.9/sanity.py
+-rw-r--r--   0 majid     (1001) engineers    (11)       38 2023-05-20 14:55:59.883499 temboz-4.9/setup.cfg
+-rw-r--r--   0 majid     (1001) engineers    (11)     1050 2023-05-20 14:55:07.000000 temboz-4.9/setup.py
+-rwxr-xr-x   0 majid     (1001) engineers    (11)     2926 2022-03-16 15:08:42.000000 temboz-4.9/temboz
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.806832 temboz-4.9/temboz.egg-info/
+-rw-r--r--   0 majid     (1001) engineers    (11)     4880 2023-05-20 14:55:59.000000 temboz-4.9/temboz.egg-info/PKG-INFO
+-rw-r--r--   0 majid     (1001) engineers    (11)    23015 2023-05-20 14:55:59.000000 temboz-4.9/temboz.egg-info/SOURCES.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)        1 2023-05-20 14:55:59.000000 temboz-4.9/temboz.egg-info/dependency_links.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)      128 2023-05-20 14:55:59.000000 temboz-4.9/temboz.egg-info/requires.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)       10 2023-05-20 14:55:59.000000 temboz-4.9/temboz.egg-info/top_level.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.810165 temboz-4.9/tembozapp/
+-rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/__init__.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     1247 2022-09-22 19:02:31.000000 temboz-4.9/tembozapp/aia.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     1631 2023-05-20 11:01:05.000000 temboz-4.9/tembozapp/autodiscovery.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     3595 2019-10-15 15:39:31.000000 temboz-4.9/tembozapp/bootstrap.py
+-rw-r--r--   0 majid     (1001) engineers    (11)    18039 2022-06-08 21:41:43.000000 temboz-4.9/tembozapp/dbop.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     3142 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/ddl.sql
+-rw-r--r--   0 majid     (1001) engineers    (11)     5488 2023-05-20 10:59:59.000000 temboz-4.9/tembozapp/degunk.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     2481 2020-10-29 20:48:27.000000 temboz-4.9/tembozapp/feedfix.py
+-rw-r--r--   0 majid     (1001) engineers    (11)    12857 2023-05-20 10:58:34.000000 temboz-4.9/tembozapp/filters.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     2838 2023-01-11 20:20:56.000000 temboz-4.9/tembozapp/fts5.py
+-rw-r--r--   0 majid     (1001) engineers    (11)    33120 2023-05-20 11:27:03.000000 temboz-4.9/tembozapp/normalize.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     2633 2022-03-16 15:08:42.000000 temboz-4.9/tembozapp/opml.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     2795 2020-06-03 04:24:13.000000 temboz-4.9/tembozapp/param.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     8455 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/porter2.py
+-rw-r--r--   0 majid     (1001) engineers    (11)    30480 2023-05-11 12:23:43.000000 temboz-4.9/tembozapp/server.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     1098 2020-03-31 11:12:59.000000 temboz-4.9/tembozapp/sop.py
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.813499 temboz-4.9/tembozapp/static/
+-rw-r--r--   0 majid     (1001) engineers    (11)       52 2018-08-08 18:25:00.000000 temboz-4.9/tembozapp/static/add.js
+-rw-r--r--   0 majid     (1001) engineers    (11)   136091 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/dygraph-combined.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/iphone.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     1076 2018-05-05 07:28:18.000000 temboz-4.9/tembozapp/static/item.mst
+-rw-r--r--   0 majid     (1001) engineers    (11)    23522 2021-09-22 09:25:31.000000 temboz-4.9/tembozapp/static/mustache.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3035 2021-09-22 09:23:47.000000 temboz-4.9/tembozapp/static/specific.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    10392 2021-05-07 18:03:17.000000 temboz-4.9/tembozapp/static/temboz.css
+-rw-r--r--   0 majid     (1001) engineers    (11)   478942 2021-09-22 09:25:31.000000 temboz-4.9/tembozapp/static/temboz.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.813499 temboz-4.9/tembozapp/static/tiny_mce/
+-rw-r--r--   0 majid     (1001) engineers    (11)      213 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/blank.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.813499 temboz-4.9/tembozapp/static/tiny_mce/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1650 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)      304 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/langs/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)    23672 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/license.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2039 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     8563 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)       87 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/images/template.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      240 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1524 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/popup.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      299 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/css/advhr.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     2128 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3024 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      153 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/images/advhr.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1128 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/jscripts/rule.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.816832 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      192 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)     2721 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/rule.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      835 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/css/advimage.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     3264 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     4603 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    10595 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/image.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1624 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/images/sample.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)    16256 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/jscripts/functions.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      931 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      594 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/css/advlink.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     1978 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2742 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)    18473 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/jscripts/functions.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1434 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    14866 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/link.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.820165 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/
+-rw-r--r--   0 majid     (1001) engineers    (11)      802 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1263 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      149 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/cleanup/
+-rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/cleanup/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)      383 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/cleanup/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       52 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/cleanup/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1226 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/css/contextmenu.css
+-rw-r--r--   0 majid     (1001) engineers    (11)    11005 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    14711 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/images/spacer.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2099 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2837 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      155 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/images/ltr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      153 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/images/rtl.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.823499 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      160 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.826832 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1105 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1881 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     4409 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/emotions.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      319 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/emotions.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      150 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)      354 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-cool.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      329 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-cry.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      331 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-embarassed.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      344 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-foot-in-mouth.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      340 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-frown.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      336 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-innocent.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      338 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-kiss.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      344 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-laughing.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      321 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-money-mouth.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      325 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-sealed.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      345 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-smile.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      342 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-surprised.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      328 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-tongue-out.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      337 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-undecided.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      351 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-wink.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      336 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/images/smiley-yell.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)      666 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/jscripts/functions.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      461 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      190 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/css/content.css
+-rw-r--r--   0 majid     (1001) engineers    (11)      119 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/css/flash.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     7030 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     9871 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2800 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/flash.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      241 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/images/flash.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)     3437 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/jscripts/flash.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      251 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.830165 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/
+-rw-r--r--   0 majid     (1001) engineers    (11)      229 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/blank.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2876 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/css/fullpage.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     5072 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     7372 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    26164 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/fullpage.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      893 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/add.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      632 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/fullpage.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      194 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/move_down.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      200 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/move_up.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      180 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/remove.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)    18594 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/fullpage.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2744 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/langs/en.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1538 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2160 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3268 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/fullscreen.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      198 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/images/fullscreen.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      136 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.833499 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1195 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1916 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      124 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/images/iespell.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1030 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/css/inlinepopup.css
+-rw-r--r--   0 majid     (1001) engineers    (11)    15998 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    20815 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/spacer.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_close.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_maximize.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_minimize.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       74 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/images/window_resize.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)    14517 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/mcwindows.js
+-rw-r--r--   0 majid     (1001) engineers    (11)        0 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.836832 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2744 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3766 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      287 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/images/insertdate.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      239 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/images/inserttime.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      682 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/
+-rw-r--r--   0 majid     (1001) engineers    (11)     5031 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     6897 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      209 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/images/absolute.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      360 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/images/backward.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      358 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/images/forward.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      264 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/images/insert_layer.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      238 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.840165 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      395 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/css/noneditable.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     3339 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     5127 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/
+-rw-r--r--   0 majid     (1001) engineers    (11)      496 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/blank.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      395 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/css/blank.css
+-rw-r--r--   0 majid     (1001) engineers    (11)       49 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/css/pasteword.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     9320 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    13678 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      294 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/images/pastetext.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      299 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/images/pasteword.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      205 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/images/selectall.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)      816 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/jscripts/pastetext.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1282 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/jscripts/pasteword.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      380 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1454 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/pastetext.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1135 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/pasteword.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2159 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3107 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)      314 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/example.html
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.843499 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      286 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/images/preview.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/
+-rw-r--r--   0 majid     (1001) engineers    (11)      811 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1344 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      211 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/images/print.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/print/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)       49 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2066 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3313 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      285 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/images/save.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/save/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/
+-rw-r--r--   0 majid     (1001) engineers    (11)     4444 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     6177 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      125 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/images/replace.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      191 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/images/search.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.846832 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1306 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/replace.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1082 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/search.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)      827 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)     2585 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/replace.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     2029 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/search.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1173 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/css/props.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     1335 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2033 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1096 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/images/apply_button_bg.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      562 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/images/style_info.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)    29556 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/jscripts/props.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1550 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    28854 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/props.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/style/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/
+-rw-r--r--   0 majid     (1001) engineers    (11)     6960 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/cell.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.850165 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      205 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/css/cell.css
+-rw-r--r--   0 majid     (1001) engineers    (11)      306 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/css/row.css
+-rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/css/table.css
+-rw-r--r--   0 majid     (1001) engineers    (11)    20104 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    30559 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/editor_plugin_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.853499 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1356 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/buttons.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      287 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      189 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_cell_props.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      372 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_delete.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      163 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_delete_col.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      171 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_delete_row.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      165 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_insert_col_after.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      165 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_insert_col_before.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      163 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_insert_row_after.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      159 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_insert_row_before.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      198 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_merge_cells.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      187 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_row_props.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      210 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/table_split_cells.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.853499 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)     7901 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/cell.js
+-rw-r--r--   0 majid     (1001) engineers    (11)      489 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/merge_cells.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     6395 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/row.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    11734 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/table.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.853499 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2593 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1410 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/merge_cells.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/readme.txt
+-rw-r--r--   0 majid     (1001) engineers    (11)     6016 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/row.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     6812 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/table/table.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.856832 temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1173 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1789 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)       61 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/readme.txt
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.796832 temboz-4.9/tembozapp/static/tiny_mce/themes/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.856832 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2411 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/about.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1142 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/anchor.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     2591 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/charmap.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)      554 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/color_picker.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.856832 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1263 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_content.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     5536 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_popup.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     7017 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_ui.css
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.796832 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.860165 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/
+-rw-r--r--   0 majid     (1001) engineers    (11)      977 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/about.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     6769 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/common_buttons.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     3401 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/create_accessible_content.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.860165 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)     5189 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_anchor_window.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     7195 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_image_window.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     5658 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_link_window.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     7094 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_table_window.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     1104 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/index.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1061 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_anchor_button.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1964 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_image_button.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1082 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_link_button.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1946 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_table_button.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1320 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/style.css
+-rw-r--r--   0 majid     (1001) engineers    (11)    40216 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/editor_template.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    53294 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/editor_template_src.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     4891 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/image.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.870165 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)      171 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/anchor.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/anchor_symbol.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      174 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/backcolor.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold_de_se.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       80 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold_es.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold_fr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      207 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bold_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      113 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/browse.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      108 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/bullist.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/button_menu.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     8399 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/buttons.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      677 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/cancel_button_bg.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/charmap.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      256 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/cleanup.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      102 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/close.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/code.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      125 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/color.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      263 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/copy.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/custom_1.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      187 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/cut.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      272 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/forecolor.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      295 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/help.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       63 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/hr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      194 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/image.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      112 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/indent.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      703 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/insert_button_bg.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/italic.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/italic_de_se.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       74 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/italic_es.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/italic_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      274 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/italic_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/justifycenter.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       71 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/justifyfull.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       71 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/justifyleft.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       70 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/justifyright.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/link.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       51 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/menu_check.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      170 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/newdocument.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/numlist.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      147 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/opacity.png
+-rw-r--r--   0 majid     (1001) engineers    (11)      110 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/outdent.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      286 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/paste.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/redo.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      168 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/removeformat.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/separator.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/spacer.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/statusbar_resize.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       83 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/strikethrough.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      148 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/sub.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      147 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/sup.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/underline.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/underline_es.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/underline_fr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/underline_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/underline_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/undo.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      190 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/unlink.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      206 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/visualaid.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.870165 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/
+-rw-r--r--   0 majid     (1001) engineers    (11)      694 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_bg.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_end.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      428 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_sel_bg.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      101 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_sel_end.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       48 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tabs_bg.gif
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.873499 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2616 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/about.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1992 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/anchor.js
+-rw-r--r--   0 majid     (1001) engineers    (11)    15097 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/charmap.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     5030 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/color_picker.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3003 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/image.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     2459 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/link.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1909 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/source_editor.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.873499 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/langs/
+-rw-r--r--   0 majid     (1001) engineers    (11)     2862 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/langs/en.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3901 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/link.htm
+-rw-r--r--   0 majid     (1001) engineers    (11)     1334 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/source_editor.htm
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.873499 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.873499 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/
+-rw-r--r--   0 majid     (1001) engineers    (11)      513 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_content.css
+-rw-r--r--   0 majid     (1001) engineers    (11)      805 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_popup.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     2296 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_ui.css
+-rw-r--r--   0 majid     (1001) engineers    (11)     2840 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/editor_template.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     3582 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/editor_template_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.876832 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/
+-rw-r--r--   0 majid     (1001) engineers    (11)       76 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bold.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       73 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bold_de_se.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bold_fr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bold_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      207 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bold_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      108 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/bullist.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)     1054 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/buttons.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      256 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/cleanup.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/italic.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       75 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/italic_de_se.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       78 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/italic_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      274 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/italic_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      111 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/numlist.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      169 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/redo.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       57 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/separator.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       43 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/spacer.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       83 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/strikethrough.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       88 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/underline.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       79 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/underline_fr.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)       77 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/underline_ru.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      245 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/underline_tw.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)      175 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/undo.gif
+-rw-r--r--   0 majid     (1001) engineers    (11)   136939 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/tiny_mce.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     7364 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/tiny_mce_popup.js
+-rw-r--r--   0 majid     (1001) engineers    (11)   194076 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/tiny_mce_src.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.880165 temboz-4.9/tembozapp/static/tiny_mce/utils/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1801 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/utils/editable_selects.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     6329 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/utils/form_utils.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     4357 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/utils/mclayer.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1841 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/utils/mctabs.js
+-rw-r--r--   0 majid     (1001) engineers    (11)     1724 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/static/tiny_mce/utils/validate.js
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.880165 temboz-4.9/tembozapp/templates/
+-rw-r--r--   0 majid     (1001) engineers    (11)     1186 2020-08-31 19:52:31.000000 temboz-4.9/tembozapp/templates/_share.atom
+-rw-r--r--   0 majid     (1001) engineers    (11)     1085 2018-08-08 18:25:33.000000 temboz-4.9/tembozapp/templates/add.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     1361 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/templates/edit.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     6173 2023-03-07 13:54:33.000000 temboz-4.9/tembozapp/templates/feed.html
+-rw-r--r--   0 majid     (1001) engineers    (11)      683 2019-10-28 12:30:01.000000 temboz-4.9/tembozapp/templates/feed_debug.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     3569 2021-01-28 01:11:49.000000 temboz-4.9/tembozapp/templates/feeds.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     1617 2019-09-24 22:46:49.000000 temboz-4.9/tembozapp/templates/login.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     2308 2020-10-14 18:12:17.000000 temboz-4.9/tembozapp/templates/menubar.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     3156 2018-05-06 10:21:59.000000 temboz-4.9/tembozapp/templates/offline.html
+-rw-r--r--   0 majid     (1001) engineers    (11)      549 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/templates/opml.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)      472 2017-02-26 12:29:31.000000 temboz-4.9/tembozapp/templates/rules.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     6957 2020-12-30 12:28:01.000000 temboz-4.9/tembozapp/templates/rules_common.html
+-rw-r--r--   0 majid     (1001) engineers    (11)    12280 2022-06-08 21:05:10.000000 temboz-4.9/tembozapp/templates/settings.html
+-rw-r--r--   0 majid     (1001) engineers    (11)     1037 2020-05-26 09:58:27.000000 temboz-4.9/tembozapp/templates/threads.html
+-rw-r--r--   0 majid     (1001) engineers    (11)    11961 2023-01-27 12:39:27.000000 temboz-4.9/tembozapp/templates/view.html
+-rw-r--r--   0 majid     (1001) engineers    (11)    12124 2022-06-08 17:13:28.000000 temboz-4.9/tembozapp/transform.py
+-rw-r--r--   0 majid     (1001) engineers    (11)    27202 2023-05-20 11:22:25.000000 temboz-4.9/tembozapp/update.py
+-rw-r--r--   0 majid     (1001) engineers    (11)      908 2022-03-16 15:08:42.000000 temboz-4.9/tembozapp/urldedup.py
+-rw-r--r--   0 majid     (1001) engineers    (11)     1203 2019-10-15 15:39:31.000000 temboz-4.9/tembozapp/util.py
+drwxr-xr-x   0 majid     (1001) engineers    (11)        0 2023-05-20 14:55:59.883499 temboz-4.9/test/
+-rw-r--r--   0 majid     (1001) engineers    (11)      376 2016-07-20 04:47:17.000000 temboz-4.9/test/category.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)     1634 2016-07-20 04:47:17.000000 temboz-4.9/test/directory.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)     1343 2016-07-20 04:47:17.000000 temboz-4.9/test/placesLived.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)     1390 2016-07-20 04:47:17.000000 temboz-4.9/test/simpleScript.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)     2837 2016-07-20 04:47:17.000000 temboz-4.9/test/states.opml
+-rw-r--r--   0 majid     (1001) engineers    (11)     4687 2016-07-20 04:47:17.000000 temboz-4.9/test/subscriptionList.opml
+-rwxr-xr-x   0 majid     (1001) engineers    (11)     2194 2023-02-09 19:18:28.000000 temboz-4.9/test.py
+-rw-r--r--   0 majid     (1001) engineers    (11)      368 2020-08-27 11:56:31.000000 temboz-4.9/unit_test.py
```

### Comparing `temboz-4.8/Dockerfile` & `temboz-4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `temboz-4.8/LICENSE` & `temboz-4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `temboz-4.8/Makefile` & `temboz-4.9/Makefile`

 * *Files identical despite different names*

### Comparing `temboz-4.8/PKG-INFO` & `temboz-4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboz
-Version: 4.8
+Version: 4.9
 Summary: The Temboz RSS/Atom feed reader and aggregator.
 Home-page: https://github.com/fazalmajid/temboz
 Author: Fazal Majid
 Author-email: python@sentfrom.com
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `temboz-4.8/README.md` & `temboz-4.9/README.md`

 * *Files identical despite different names*

### Comparing `temboz-4.8/UPGRADE` & `temboz-4.9/UPGRADE`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/DigitalOutbackPhoto_News.xml` & `temboz-4.9/bugfeed/DigitalOutbackPhoto_News.xml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/PetaPixel` & `temboz-4.9/bugfeed/PetaPixel`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/QuantifiedSelf` & `temboz-4.9/bugfeed/QuantifiedSelf`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/barnett` & `temboz-4.9/bugfeed/barnett`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/boingboing` & `temboz-4.9/bugfeed/boingboing`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/calmatters` & `temboz-4.9/bugfeed/calmatters`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/case1` & `temboz-4.9/bugfeed/case1`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/case2` & `temboz-4.9/bugfeed/case2`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/case3` & `temboz-4.9/bugfeed/case3`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/cooltools` & `temboz-4.9/bugfeed/cooltools`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/greenwald` & `temboz-4.9/bugfeed/greenwald`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/nettuts` & `temboz-4.9/bugfeed/nettuts`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/russellbeattieweblog` & `temboz-4.9/bugfeed/russellbeattieweblog`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/tokyo` & `temboz-4.9/bugfeed/tokyo`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/tychay` & `temboz-4.9/bugfeed/tychay`

 * *Files identical despite different names*

### Comparing `temboz-4.8/bugfeed/typographica` & `temboz-4.9/bugfeed/typographica`

 * *Files identical despite different names*

### Comparing `temboz-4.8/etc/db_0.5.sh` & `temboz-4.9/etc/db_0.5.sh`

 * *Files identical despite different names*

### Comparing `temboz-4.8/etc/norm_url.py` & `temboz-4.9/etc/norm_url.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/etc/resolveguid.py` & `temboz-4.9/etc/resolveguid.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/me.opml` & `temboz-4.9/me.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/sanity.py` & `temboz-4.9/sanity.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/setup.py` & `temboz-4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name='temboz',
   author='Fazal Majid',
   author_email='python@sentfrom.com',
-  version='4.8',
+  version='4.9',
   url='https://github.com/fazalmajid/temboz',
   #package_dir={'': 'src'},
   packages=['tembozapp'] + setuptools.find_packages(),
   include_package_data=True,
   scripts=['temboz'],
   install_requires=[
     'flask',
```

### Comparing `temboz-4.8/temboz` & `temboz-4.9/temboz`

 * *Files identical despite different names*

### Comparing `temboz-4.8/temboz.egg-info/PKG-INFO` & `temboz-4.9/temboz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboz
-Version: 4.8
+Version: 4.9
 Summary: The Temboz RSS/Atom feed reader and aggregator.
 Home-page: https://github.com/fazalmajid/temboz
 Author: Fazal Majid
 Author-email: python@sentfrom.com
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `temboz-4.8/temboz.egg-info/SOURCES.txt` & `temboz-4.9/temboz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/aia.py` & `temboz-4.9/tembozapp/aia.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/autodiscovery.py` & `temboz-4.9/tembozapp/autodiscovery.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import urllib.parse
 import requests, html5lib, feedparser
 from . import param
 
 def find(url):
-  html = requests.get(url,
-                      headers={'user-agent': param.user_agent},
-                      timeout=param.http_timeout).content
+  s = requests.Session()
+  try:
+    html = s.get(url,
+                 headers={'user-agent': param.user_agent},
+                 timeout=param.http_timeout).content
+  finally:
+    s.close()
   tree = html5lib.parse(html, namespaceHTMLElements=False)
   # base for relative URLs
   base = tree.findall('.//base')
   if base and 'href' in base[0].attrib:
     base = base[0].attrib
   else:
     base = url
```

### Comparing `temboz-4.8/tembozapp/bootstrap.py` & `temboz-4.9/tembozapp/bootstrap.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/dbop.py` & `temboz-4.9/tembozapp/dbop.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/ddl.sql` & `temboz-4.9/tembozapp/ddl.sql`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/degunk.py` & `temboz-4.9/tembozapp/degunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,19 @@
           link = c.fetchone()
           c.close()
           if link:
             print('not dereferencing', guid, '->', link[0], file=param.log)
             item['link'] = link[0]
             return content
           # we haven't seen this article before, buck up and load it
-          deref = requests.get(item['link'],
-                               timeout=param.http_timeout).content
+          s = requests.Session()
+          try:
+            deref = s.get(item['link'],
+                          timeout=param.http_timeout).content
+          finally:
+            s.close()
           m = self.re.search(deref)
           if m and m.groups():
             item['link'] = m.groups()[0]
       except:
         util.print_stack()
     return content
```

### Comparing `temboz-4.8/tembozapp/feedfix.py` & `temboz-4.9/tembozapp/feedfix.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/filters.py` & `temboz-4.9/tembozapp/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,20 @@
   try:
     return candidates[0].attrib['href']
   except:
     return 'NOT MATCHED'
 
 def dereference_content(url):
   try:
-    r = requests.get(url, timeout=param.http_timeout)
-    return r.content
+    s = requests.Session()
+    try:
+      r = s.get(url, timeout=param.http_timeout)
+      return r.content
+    finally:
+      s.close()
   except:
     return ''
 
 # shades of LISP...
 def curry(fn, obj):
   return lambda *args: fn(obj, *args)
```

### Comparing `temboz-4.8/tembozapp/fts5.py` & `temboz-4.9/tembozapp/fts5.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/normalize.py` & `temboz-4.9/tembozapp/normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,34 +545,38 @@
     seen.add(url)
   if jar is None:
     jar = requests.cookies.RequestsCookieJar()
   # stop recursion if it is too deep
   if level > 16:
     return url
   try:
-    r = requests.get(url, allow_redirects=False, timeout=param.http_timeout,
-                     cookies=jar)
-    if not r.is_redirect:
-      return url
-    else:
-      jar.update(r.cookies)
-      # break a redirection loop if it occurs
-      redir = r.headers.get('Location')
-      if True not in [redir.startswith(p)
-                      for p in ['http://', 'https://', 'ftp://']]:
+    s = requests.Session()
+    try:
+      r = s.get(url, allow_redirects=False, timeout=param.http_timeout,
+                       cookies=jar)
+      if not r.is_redirect:
         return url
-      if redir in seen:
-        return url
-      # some servers redirect to Unicode URLs, which are not legal
-      try:
-        str(redir)
-      except UnicodeDecodeError:
-        return url
-      # there might be several levels of redirection
-      return dereference(redir, seen, level + 1, jar)
+      else:
+        jar.update(r.cookies)
+        # break a redirection loop if it occurs
+        redir = r.headers.get('Location')
+        if True not in [redir.startswith(p)
+                        for p in ['http://', 'https://', 'ftp://']]:
+          return url
+        if redir in seen:
+          return url
+        # some servers redirect to Unicode URLs, which are not legal
+        try:
+          str(redir)
+        except UnicodeDecodeError:
+          return url
+        # there might be several levels of redirection
+        return dereference(redir, seen, level + 1, jar)
+    finally:
+      s.close()
   except (requests.exceptions.RequestException, ValueError, socket.error):
     return url
   except:
     util.print_stack()
     return url
   
 url_re = re.compile('(?:href|src)="([^"]*)"', re.IGNORECASE)
```

### Comparing `temboz-4.8/tembozapp/opml.py` & `temboz-4.9/tembozapp/opml.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/param.py` & `temboz-4.9/tembozapp/param.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/porter2.py` & `temboz-4.9/tembozapp/porter2.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/server.py` & `temboz-4.9/tembozapp/server.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/sop.py` & `temboz-4.9/tembozapp/sop.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/dygraph-combined.js` & `temboz-4.9/tembozapp/static/dygraph-combined.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/item.mst` & `temboz-4.9/tembozapp/static/item.mst`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/mustache.js` & `temboz-4.9/tembozapp/static/mustache.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/specific.js` & `temboz-4.9/tembozapp/static/specific.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/temboz.css` & `temboz-4.9/tembozapp/static/temboz.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/temboz.js` & `temboz-4.9/tembozapp/static/temboz.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/license.txt` & `temboz-4.9/tembozapp/static/tiny_mce/license.txt`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/_template/popup.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/_template/popup.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/jscripts/rule.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/jscripts/rule.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advhr/rule.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advhr/rule.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/css/advimage.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/css/advimage.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/image.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/image.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/images/sample.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/images/sample.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/jscripts/functions.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/jscripts/functions.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advimage/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advimage/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/css/advlink.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/css/advlink.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/jscripts/functions.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/jscripts/functions.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/advlink/link.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/advlink/link.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/autosave/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/css/contextmenu.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/css/contextmenu.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/contextmenu/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/directionality/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/emotions.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/emotions.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/emotions/jscripts/functions.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/emotions/jscripts/functions.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/flash.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/flash.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/flash/jscripts/flash.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/flash/jscripts/flash.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/css/fullpage.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/css/fullpage.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/fullpage.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/fullpage.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/add.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/add.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/images/fullpage.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/images/fullpage.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/fullpage.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/jscripts/fullpage.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullpage/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullpage/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/fullscreen/fullscreen.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/fullscreen/fullscreen.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/iespell/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/css/inlinepopup.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/css/inlinepopup.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/mcwindows.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/inlinepopups/jscripts/mcwindows.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/insertdatetime/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/layer/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/layer/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/noneditable/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/jscripts/pastetext.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/jscripts/pastetext.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/jscripts/pasteword.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/jscripts/pasteword.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/pastetext.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/pastetext.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/paste/pasteword.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/paste/pasteword.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/preview/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/preview/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/print/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/print/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/print/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/print/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/save/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/save/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/save/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/save/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/replace.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/replace.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/search.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/jscripts/search.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/replace.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/replace.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/searchreplace/search.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/searchreplace/search.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/css/props.css` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/css/props.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/images/apply_button_bg.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/images/apply_button_bg.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/images/style_info.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/images/style_info.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/jscripts/props.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/jscripts/props.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/style/props.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/style/props.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/cell.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/cell.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/images/buttons.gif` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/images/buttons.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/cell.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/cell.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/row.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/row.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/jscripts/table.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/jscripts/table.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/merge_cells.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/merge_cells.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/row.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/row.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/table/table.htm` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/table/table.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/plugins/zoom/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/about.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/about.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/anchor.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/anchor.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/charmap.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/charmap.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/color_picker.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/color_picker.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_content.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_content.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_popup.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_popup.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/css/editor_ui.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/css/editor_ui.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/about.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/about.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/common_buttons.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/common_buttons.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/create_accessible_content.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/create_accessible_content.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_anchor_window.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_anchor_window.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_image_window.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_image_window.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_link_window.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_link_window.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_table_window.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/images/insert_table_window.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/index.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/index.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_anchor_button.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_anchor_button.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_image_button.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_image_button.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_link_button.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_link_button.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_table_button.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/insert_table_button.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/docs/en/style.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/docs/en/style.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/editor_template.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/editor_template.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/editor_template_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/editor_template_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/image.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/image.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/buttons.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/buttons.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/cancel_button_bg.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/cancel_button_bg.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/insert_button_bg.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/insert_button_bg.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_bg.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/images/xp/tab_bg.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/about.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/about.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/anchor.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/anchor.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/charmap.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/charmap.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/color_picker.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/color_picker.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/image.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/image.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/link.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/link.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/jscripts/source_editor.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/jscripts/source_editor.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/langs/en.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/langs/en.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/link.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/link.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/advanced/source_editor.htm` & `temboz-4.9/tembozapp/static/tiny_mce/themes/advanced/source_editor.htm`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_content.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_content.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_popup.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_popup.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/css/editor_ui.css` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/css/editor_ui.css`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/editor_template.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/editor_template.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/editor_template_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/editor_template_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/themes/simple/images/buttons.gif` & `temboz-4.9/tembozapp/static/tiny_mce/themes/simple/images/buttons.gif`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/tiny_mce.js` & `temboz-4.9/tembozapp/static/tiny_mce/tiny_mce.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/tiny_mce_popup.js` & `temboz-4.9/tembozapp/static/tiny_mce/tiny_mce_popup.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/tiny_mce_src.js` & `temboz-4.9/tembozapp/static/tiny_mce/tiny_mce_src.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/utils/editable_selects.js` & `temboz-4.9/tembozapp/static/tiny_mce/utils/editable_selects.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/utils/form_utils.js` & `temboz-4.9/tembozapp/static/tiny_mce/utils/form_utils.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/utils/mclayer.js` & `temboz-4.9/tembozapp/static/tiny_mce/utils/mclayer.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/utils/mctabs.js` & `temboz-4.9/tembozapp/static/tiny_mce/utils/mctabs.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/static/tiny_mce/utils/validate.js` & `temboz-4.9/tembozapp/static/tiny_mce/utils/validate.js`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/_share.atom` & `temboz-4.9/tembozapp/templates/_share.atom`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/add.html` & `temboz-4.9/tembozapp/templates/add.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/edit.html` & `temboz-4.9/tembozapp/templates/edit.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/feed.html` & `temboz-4.9/tembozapp/templates/feed.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/feed_debug.html` & `temboz-4.9/tembozapp/templates/feed_debug.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/feeds.html` & `temboz-4.9/tembozapp/templates/feeds.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/login.html` & `temboz-4.9/tembozapp/templates/login.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/menubar.html` & `temboz-4.9/tembozapp/templates/menubar.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/offline.html` & `temboz-4.9/tembozapp/templates/offline.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/opml.opml` & `temboz-4.9/tembozapp/templates/opml.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/rules_common.html` & `temboz-4.9/tembozapp/templates/rules_common.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/settings.html` & `temboz-4.9/tembozapp/templates/settings.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/threads.html` & `temboz-4.9/tembozapp/templates/threads.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/templates/view.html` & `temboz-4.9/tembozapp/templates/view.html`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/transform.py` & `temboz-4.9/tembozapp/transform.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/update.py` & `temboz-4.9/tembozapp/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,37 +46,49 @@
 
 def add_feed(feed_xml):
   """Try to add a feed. Returns a tuple (feed_uid, num_added, num_filtered)"""
   with dbop.db() as db:
     c = db.cursor()
     feed_xml = feed_xml.replace('feed://', 'http://')
     # verify the feed
-    r = requests.get(feed_xml, timeout=param.http_timeout)
-    f = feedparser.parse(r.content)
+    s = requests.Session()
+    try:
+      r = s.get(feed_xml, timeout=param.http_timeout)
+      content = r.content
+      etag = r.headers.get('Etag')
+    finally:
+      s.close()
+    f = feedparser.parse(content)
     normalize.basic(f, feed_xml)
     if not f.feed or ('link' not in f.feed or 'title' not in f.feed):
       original = feed_xml
       feed_xml = autodiscovery.find(original)
       if not feed_xml:
         raise AutoDiscoveryError
       print('add_feed:autodiscovery of', original, 'found', feed_xml,
             file=param.log)
-      r = requests.get(feed_xml, timeout=param.http_timeout)
-      f = feedparser.parse(r.text)
+      s = requests.Session()
+      try:
+        r = s.get(feed_xml, timeout=param.http_timeout)
+        text = r.text
+        etag = r.headers.get('Etag')
+      finally:
+        s.close()
+      f = feedparser.parse(text)
       normalize.basic(f, feed_xml)
       if not f.feed or 'url' not in f:
-        print('add_feed:autodiscovery failed %r %r' % (r.text, f.__dict__),
+        print('add_feed:autodiscovery failed %r %r' % (text, f.__dict__),
               file=param.log)
         raise ParseError
     # we have a valid feed, normalize it
     normalize.normalize_feed(f)
     feed = {
       'xmlUrl': f['url'],
       'htmlUrl': str(f.feed['link']),
-      'etag': r.headers.get('Etag'),
+      'etag': etag,
       'title': f.feed['title'],
       'desc': f.feed['description']
     }
     for key, value in list(feed.items()):
       if type(value) == str:
         feed[key] = value
     filters.load_rules(c)
@@ -96,16 +108,21 @@
         db.rollback()
         raise UnknownError(str(e))
 
 def update_feed_xml(feed_uid, feed_xml):
   """Update a feed URL and fetch the feed. Returns the number of new items"""
   feed_uid = int(feed_uid)
 
-  r = requests.get(feed_xml, timeout=param.http_timeout)
-  f = feedparser.parse(r.content)
+  s = requests.Session()
+  try:
+    r = s.get(feed_xml, timeout=param.http_timeout)
+    content = r.content
+  finally:
+    s.close()
+  f = feedparser.parse(content)
   if not f.feed:
     raise ParseError
   normalize.normalize_feed(f)
 
   with dbop.db() as db:
     c = db.cursor()
     clear_errors(db, c, feed_uid, f)
@@ -275,15 +292,15 @@
   with dbop.db() as db:
     c = db.cursor()
     c.execute("""update fm_items set item_rating=-1
     where item_feed_uid=? and item_rating=0 and exists (
       select * from fm_items i2
       where i2.item_feed_uid=fm_items.item_feed_uid
         and i2.item_uid<>fm_items.item_uid
-        and i2.item_title=fm_items.item_title and i2.item_rating<>0
+        and i2.item_title=fm_items.item_title
     )""", [feed_uid])
     modified = c.rowcount
     db.commit()
     c.close()
   return modified
 
 def purge_items(c, feed_uid):
@@ -302,16 +319,21 @@
     purge_items(c, feed_uid)
     c.execute("""update fm_feeds set feed_modified=NULL, feed_etag=NULL
     where feed_uid=?""", [feed_uid])
     c.execute("""select feed_xml from fm_feeds
     where feed_uid=?""", [feed_uid])
     feed_xml = c.fetchone()[0]
     db.commit()
-    r = requests.get(feed_xml, timeout=param.http_timeout)
-    f = feedparser.parse(r.content)
+    s = requests.Session()
+    try:
+      r = s.get(feed_xml, timeout=param.http_timeout)
+      content = r.content
+    finally:
+      s.close()
+    f = feedparser.parse(content)
     if not f.feed:
       raise ParseError
     normalize.normalize_feed(f)
     clear_errors(db, c, feed_uid, f)
     filters.load_rules(c)
     num_added = process_parsed_feed(db, c, f, feed_uid)
     db.commit()
@@ -356,20 +378,26 @@
 
 def fetch_feed(feed_uid, feed_xml, feed_etag, feed_modified):
   if not feed_etag:
     feed_etag = None
   if not feed_modified:
     feed_modified = None
   try:
-    r = requests.get(feed_xml, headers={
-      'If-None-Match': feed_etag
-    }, timeout=param.http_timeout)
-    if r.content == '':
+    s = requests.Session()
+    try:
+      r = s.get(feed_xml, headers={
+        'If-None-Match': feed_etag
+      }, timeout=param.http_timeout)
+      content = r.content
+      etag = r.headers.get('Etag')
+    finally:
+      s.close()
+    if content == '':
       return {'channel': {}, 'items': [], 'why': 'no change since Etag'}
-    f = feedparser.parse(r.content, etag=r.headers.get('Etag'),
+    f = feedparser.parse(content, etag=etag,
                          modified=feed_modified)
   except (socket.timeout, requests.exceptions.RequestException) as e:
     if param.debug:
       print('EEEEE error fetching feed', feed_xml, e, file=param.log)
     f = {'channel': {}, 'items': [], 'why': repr(e)}
   except:
     if param.debug:
```

### Comparing `temboz-4.8/tembozapp/urldedup.py` & `temboz-4.9/tembozapp/urldedup.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/tembozapp/util.py` & `temboz-4.9/tembozapp/util.py`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test/directory.opml` & `temboz-4.9/test/directory.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test/placesLived.opml` & `temboz-4.9/test/placesLived.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test/simpleScript.opml` & `temboz-4.9/test/simpleScript.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test/states.opml` & `temboz-4.9/test/states.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test/subscriptionList.opml` & `temboz-4.9/test/subscriptionList.opml`

 * *Files identical despite different names*

### Comparing `temboz-4.8/test.py` & `temboz-4.9/test.py`

 * *Files identical despite different names*

