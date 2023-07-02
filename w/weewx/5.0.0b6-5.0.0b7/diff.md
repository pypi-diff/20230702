# Comparing `tmp/weewx-5.0.0b6.tar.gz` & `tmp/weewx-5.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weewx-5.0.0b6.tar", max compression
+gzip compressed data, was "weewx-5.0.0b7.tar", max compression
```

## Comparing `weewx-5.0.0b6.tar` & `weewx-5.0.0b7.tar`

### file list

```diff
@@ -1,478 +1,478 @@
--rw-r--r--   0        0        0    32472 2023-05-30 12:01:49.265499 weewx-5.0.0b6/LICENSE.txt
--rw-r--r--   0        0        0     3725 2023-06-22 18:50:33.745869 weewx-5.0.0b6/README.md
--rw-r--r--   0        0        0      230 2023-05-30 12:01:49.265499 weewx-5.0.0b6/bin/schemas/__init__.py
--rw-r--r--   0        0        0     3448 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/schemas/wview.py
--rw-r--r--   0        0        0     5953 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/schemas/wview_extended.py
--rw-r--r--   0        0        0     2105 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/schemas/wview_small.py
--rwxr-xr-x   0        0        0    52292 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/wee_database.py
--rwxr-xr-x   0        0        0    16172 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/wee_debug.py
--rwxr-xr-x   0        0        0     2187 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/wee_device.py
--rwxr-xr-x   0        0        0    38942 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/wee_import.py
--rwxr-xr-x   0        0        0     5630 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/wee_reports.py
--rw-r--r--   0        0        0        0 2023-07-02 01:40:06.556500 weewx-5.0.0b6/bin/wee_resources/__init__.py
--rw-r--r--   0        0        0      306 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/wee_resources/bin/user/__init__.py
--rw-r--r--   0        0        0      324 2023-06-26 17:07:40.592701 weewx-5.0.0b6/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      398 2023-06-26 17:07:40.592701 weewx-5.0.0b6/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
--rw-r--r--   0        0        0      541 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/wee_resources/bin/user/extensions.py
--rw-r--r--   0        0        0    33173 2023-06-30 14:55:56.834551 weewx-5.0.0b6/bin/wee_resources/docs/404.html
--rw-r--r--   0        0        0     1870 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113489 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js
--rw-r--r--   0        0        0   954781 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map
--rw-r--r--   0        0        0    17074 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0   113455 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css
--rw-r--r--   0        0        0    38958 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map
--rw-r--r--   0        0        0    12227 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css
--rw-r--r--   0        0        0     3628 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map
--rw-r--r--   0        0        0   195059 2023-06-30 14:55:56.878550 weewx-5.0.0b6/bin/wee_resources/docs/changes/index.html
--rw-r--r--   0        0        0    35875 2023-06-30 14:55:56.878550 weewx-5.0.0b6/bin/wee_resources/docs/copyright/index.html
--rw-r--r--   0        0        0      565 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/css/tocbot-4.12.0.css
--rw-r--r--   0        0        0      565 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/css/tocbot-4.3.1.css
--rw-r--r--   0        0        0    12148 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/css/weewx_ui.css
--rw-r--r--   0        0        0    62945 2023-06-30 14:55:56.958550 weewx-5.0.0b6/bin/wee_resources/docs/custom/appendix/index.html
--rw-r--r--   0        0        0   141082 2023-06-30 14:55:56.998550 weewx-5.0.0b6/bin/wee_resources/docs/custom/cheetah/index.html
--rw-r--r--   0        0        0    72678 2023-06-30 14:55:57.014550 weewx-5.0.0b6/bin/wee_resources/docs/custom/custom-reports/index.html
--rw-r--r--   0        0        0    60357 2023-06-30 14:55:57.022549 weewx-5.0.0b6/bin/wee_resources/docs/custom/database/index.html
--rw-r--r--   0        0        0    34898 2023-06-30 14:55:57.026549 weewx-5.0.0b6/bin/wee_resources/docs/custom/derived/index.html
--rw-r--r--   0        0        0    49193 2023-06-30 14:55:57.030549 weewx-5.0.0b6/bin/wee_resources/docs/custom/drivers/index.html
--rw-r--r--   0        0        0    40560 2023-06-30 14:55:57.034549 weewx-5.0.0b6/bin/wee_resources/docs/custom/extensions/index.html
--rw-r--r--   0        0        0    61818 2023-06-30 14:55:57.042549 weewx-5.0.0b6/bin/wee_resources/docs/custom/image-generator/index.html
--rw-r--r--   0        0        0    71102 2023-06-30 14:55:56.946550 weewx-5.0.0b6/bin/wee_resources/docs/custom/index.html
--rw-r--r--   0        0        0    65111 2023-06-30 14:55:57.058549 weewx-5.0.0b6/bin/wee_resources/docs/custom/localization/index.html
--rw-r--r--   0        0        0    48063 2023-06-30 14:55:57.062549 weewx-5.0.0b6/bin/wee_resources/docs/custom/multiple-bindings/index.html
--rw-r--r--   0        0        0   119836 2023-06-30 14:55:57.086549 weewx-5.0.0b6/bin/wee_resources/docs/custom/report-options/index.html
--rw-r--r--   0        0        0    51200 2023-06-30 14:55:57.090549 weewx-5.0.0b6/bin/wee_resources/docs/custom/report-scheduling/index.html
--rw-r--r--   0        0        0    83633 2023-06-30 14:55:57.114549 weewx-5.0.0b6/bin/wee_resources/docs/custom/service-engine/index.html
--rw-r--r--   0        0        0    45932 2023-06-30 14:55:57.122549 weewx-5.0.0b6/bin/wee_resources/docs/custom/units/index.html
--rw-r--r--   0        0        0    71286 2023-06-30 14:55:56.890550 weewx-5.0.0b6/bin/wee_resources/docs/devnotes/index.html
--rw-r--r--   0        0        0     2747 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/examples/tag.htm
--rw-r--r--   0        0        0    40976 2023-06-30 14:55:57.126549 weewx-5.0.0b6/bin/wee_resources/docs/hardware/acurite/index.html
--rw-r--r--   0        0        0    62045 2023-06-30 14:55:57.134549 weewx-5.0.0b6/bin/wee_resources/docs/hardware/cc3000/index.html
--rw-r--r--   0        0        0    56652 2023-06-30 14:55:57.150549 weewx-5.0.0b6/bin/wee_resources/docs/hardware/drivers/index.html
--rw-r--r--   0        0        0    48664 2023-06-30 14:55:57.158548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/fousb/index.html
--rw-r--r--   0        0        0    47333 2023-06-30 14:55:57.162549 weewx-5.0.0b6/bin/wee_resources/docs/hardware/te923/index.html
--rw-r--r--   0        0        0    38960 2023-06-30 14:55:57.166549 weewx-5.0.0b6/bin/wee_resources/docs/hardware/ultimeter/index.html
--rw-r--r--   0        0        0    69205 2023-06-30 14:55:57.178548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/vantage/index.html
--rw-r--r--   0        0        0    43515 2023-06-30 14:55:57.182548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr100/index.html
--rw-r--r--   0        0        0    43628 2023-06-30 14:55:57.190548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr300/index.html
--rw-r--r--   0        0        0    43159 2023-06-30 14:55:57.198548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr9x8/index.html
--rw-r--r--   0        0        0    38243 2023-06-30 14:55:57.198548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws1/index.html
--rw-r--r--   0        0        0    45030 2023-06-30 14:55:57.202548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws23xx/index.html
--rw-r--r--   0        0        0    50646 2023-06-30 14:55:57.206548 weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws28xx/index.html
--rw-r--r--   0        0        0    54196 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/antialias.gif
--rw-r--r--   0        0        0     3145 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/day-gap-not-shown.png
--rw-r--r--   0        0        0     3269 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/day-gap-showing.png
--rw-r--r--   0        0        0     7579 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/daycompare.png
--rw-r--r--   0        0        0     8705 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/daytemp_with_avg.png
--rw-r--r--   0        0        0     7803 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/dayvaporp.png
--rw-r--r--   0        0        0     7663 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/daywindvec.png
--rw-r--r--   0        0        0     1026 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/favicon.png
--rw-r--r--   0        0        0    38406 2023-06-30 14:55:56.730551 weewx-5.0.0b6/bin/wee_resources/docs/images/ferrites.jpg
--rw-r--r--   0        0        0     3638 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/funky_degree.png
--rw-r--r--   0        0        0    19123 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/image_parts.png
--rw-r--r--   0        0        0    86388 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/image_parts.xcf
--rw-r--r--   0        0        0     2136 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-apple.png
--rw-r--r--   0        0        0     4734 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-centos.png
--rw-r--r--   0        0        0    14541 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-debian.png
--rw-r--r--   0        0        0    24662 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-fedora.png
--rw-r--r--   0        0        0    12046 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-linux.png
--rw-r--r--   0        0        0    27245 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-mint.png
--rw-r--r--   0        0        0    15980 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-opensuse.png
--rw-r--r--   0        0        0    14374 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-pypi.svg
--rw-r--r--   0        0        0     1192 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-redhat.png
--rw-r--r--   0        0        0     3926 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-rpi.png
--rw-r--r--   0        0        0     7877 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-suse.png
--rw-r--r--   0        0        0    13954 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-ubuntu.png
--rw-r--r--   0        0        0    12208 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/logo-weewx.png
--rw-r--r--   0        0        0    35496 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/pipeline.png
--rw-r--r--   0        0        0     6709 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/sample_monthrain.png
--rw-r--r--   0        0        0    10107 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/sample_monthtempdew.png
--rw-r--r--   0        0        0    10649 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/weekgustoverlay.png
--rw-r--r--   0        0        0     8468 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/weektempdew.png
--rw-r--r--   0        0        0     6602 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/yeardiff.png
--rw-r--r--   0        0        0     7286 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/images/yearhilow.png
--rw-r--r--   0        0        0    39555 2023-06-30 14:55:56.850551 weewx-5.0.0b6/bin/wee_resources/docs/index.html
--rw-r--r--   0        0        0    32611 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/cash.js
--rw-r--r--   0        0        0    14828 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/cash.min.js
--rw-r--r--   0        0        0    11422 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.12.0.js
--rw-r--r--   0        0        0    11422 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
--rw-r--r--   0        0        0     8892 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
--rw-r--r--   0        0        0     4640 2023-06-30 14:55:56.734551 weewx-5.0.0b6/bin/wee_resources/docs/js/weewx.js
--rw-r--r--   0        0        0    44042 2023-06-30 14:55:57.214548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/debian/index.html
--rw-r--r--   0        0        0    44892 2023-06-30 14:55:57.218548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/git/index.html
--rw-r--r--   0        0        0    34859 2023-06-30 14:55:57.210548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/index.html
--rw-r--r--   0        0        0    61186 2023-06-30 14:55:57.230548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/pip/index.html
--rw-r--r--   0        0        0    42835 2023-06-30 14:55:57.234548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/redhat/index.html
--rw-r--r--   0        0        0    41774 2023-06-30 14:55:57.238548 weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/suse/index.html
--rw-r--r--   0        0        0  1039833 2023-06-30 14:55:57.418547 weewx-5.0.0b6/bin/wee_resources/docs/search/search_index.json
--rw-r--r--   0        0        0    12605 2023-06-30 14:55:56.738551 weewx-5.0.0b6/bin/wee_resources/docs/sitemap.xml
--rw-r--r--   0        0        0      750 2023-06-30 14:55:56.742551 weewx-5.0.0b6/bin/wee_resources/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    95313 2023-06-30 14:55:56.914550 weewx-5.0.0b6/bin/wee_resources/docs/sle/index.html
--rw-r--r--   0        0        0    38042 2023-06-30 14:55:57.254548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
--rw-r--r--   0        0        0    34819 2023-06-30 14:55:57.250548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/index.html
--rw-r--r--   0        0        0    41075 2023-06-30 14:55:57.258548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/installing-weewx/index.html
--rw-r--r--   0        0        0    39324 2023-06-30 14:55:57.262548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
--rw-r--r--   0        0        0    38374 2023-06-30 14:55:57.266548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/running-weewx/index.html
--rw-r--r--   0        0        0    38405 2023-06-30 14:55:57.266548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/system-requirements/index.html
--rw-r--r--   0        0        0    41481 2023-06-30 14:55:57.286548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html
--rw-r--r--   0        0        0    34943 2023-06-30 14:55:57.282548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/index.html
--rw-r--r--   0        0        0    41997 2023-06-30 14:55:57.286548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html
--rw-r--r--   0        0        0    62539 2023-06-30 14:55:57.298548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html
--rw-r--r--   0        0        0    41816 2023-06-30 14:55:57.274548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/webserver-integration/index.html
--rw-r--r--   0        0        0    38891 2023-06-30 14:55:57.302548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
--rw-r--r--   0        0        0    38398 2023-06-30 14:55:57.306547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
--rw-r--r--   0        0        0    41822 2023-06-30 14:55:57.310547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
--rw-r--r--   0        0        0    42451 2023-06-30 14:55:57.314548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
--rw-r--r--   0        0        0    39419 2023-06-30 14:55:57.318548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
--rw-r--r--   0        0        0    37700 2023-06-30 14:55:57.298548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
--rw-r--r--   0        0        0    84111 2023-06-30 14:55:57.330547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
--rw-r--r--   0        0        0    40224 2023-06-30 14:55:57.334547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
--rw-r--r--   0        0        0    36761 2023-06-30 14:55:57.334547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
--rw-r--r--   0        0        0    37346 2023-06-30 14:55:57.338547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
--rw-r--r--   0        0        0    37554 2023-06-30 14:55:57.342547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
--rw-r--r--   0        0        0    60169 2023-06-30 14:55:57.346547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
--rw-r--r--   0        0        0    70287 2023-06-30 14:55:57.358547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
--rw-r--r--   0        0        0    35735 2023-06-30 14:55:57.358547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
--rw-r--r--   0        0        0    56824 2023-06-30 14:55:57.366547 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
--rw-r--r--   0        0        0    42668 2023-06-30 14:55:57.278548 weewx-5.0.0b6/bin/wee_resources/docs/usersguide/where/index.html
--rw-r--r--   0        0        0    57266 2023-06-30 14:55:57.374547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_database/index.html
--rw-r--r--   0        0        0    46043 2023-06-30 14:55:57.378547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_debug/index.html
--rw-r--r--   0        0        0    36328 2023-06-30 14:55:57.378547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_device/index.html
--rw-r--r--   0        0        0   254677 2023-06-30 14:55:57.398547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_import/index.html
--rw-r--r--   0        0        0    38640 2023-06-30 14:55:57.402547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_reports/index.html
--rw-r--r--   0        0        0    49036 2023-06-30 14:55:57.406547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/weectl-extension/index.html
--rw-r--r--   0        0        0    63373 2023-06-30 14:55:57.414547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/weectl-station/index.html
--rw-r--r--   0        0        0    35546 2023-06-30 14:55:57.414547 weewx-5.0.0b6/bin/wee_resources/docs/utilities/weewxd/index.html
--rw-r--r--   0        0        0   150560 2023-06-30 14:55:56.934550 weewx-5.0.0b6/bin/wee_resources/docs/versions/index.html
--rw-r--r--   0        0        0     3097 2023-06-26 17:07:40.352703 weewx-5.0.0b6/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
--rw-r--r--   0        0        0    10729 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/alarm.py
--rw-r--r--   0        0        0      179 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/basic/changelog
--rw-r--r--   0        0        0     1563 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/basic/install.py
--rw-r--r--   0        0        0     1243 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/basic/readme.md
--rw-r--r--   0        0        0     1510 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/basic.css
--rw-r--r--   0        0        0     6451 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/current.inc
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/favicon.ico
--rw-r--r--   0        0        0    11292 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/hilo.inc
--rw-r--r--   0        0        0     1665 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
--rw-r--r--   0        0        0     2216 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
--rw-r--r--   0        0        0     2408 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
--rw-r--r--   0        0        0     3173 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/skin.conf
--rw-r--r--   0        0        0     2080 2023-06-26 17:07:37.972717 weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
--rw-r--r--   0        0        0     2255 2023-06-26 17:07:37.992717 weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
--rw-r--r--   0        0        0     3290 2023-06-26 17:07:37.992717 weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
--rw-r--r--   0        0        0     2128 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_1.py
--rw-r--r--   0        0        0     2617 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_2.py
--rw-r--r--   0        0        0     4001 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_3.py
--rw-r--r--   0        0        0     4180 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
--rw-r--r--   0        0        0      269 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/fileparse/changelog
--rw-r--r--   0        0        0      835 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/fileparse/install.py
--rw-r--r--   0        0        0     2086 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/fileparse/readme.md
--rw-r--r--   0        0        0    10792 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/lowBattery.py
--rw-r--r--   0        0        0     1108 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/mem.py
--rw-r--r--   0        0        0     5986 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/pmon/bin/user/pmon.py
--rw-r--r--   0        0        0      341 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/pmon/changelog
--rw-r--r--   0        0        0     1511 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/pmon/install.py
--rw-r--r--   0        0        0     2628 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/pmon/readme.md
--rw-r--r--   0        0        0      507 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
--rw-r--r--   0        0        0     1234 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
--rw-r--r--   0        0        0     4334 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/tests/test_vaporpressure.py
--rw-r--r--   0        0        0     4285 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/examples/vaporpressure.py
--rw-r--r--   0        0        0     3034 2023-06-26 17:07:38.004717 weewx-5.0.0b6/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
--rw-r--r--   0        0        0     5662 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/bin/user/xstats.py
--rw-r--r--   0        0        0      146 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/changelog
--rw-r--r--   0        0        0      850 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/install.py
--rw-r--r--   0        0        0     2923 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/readme.txt
--rw-r--r--   0        0        0     2138 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
--rw-r--r--   0        0        0      591 2023-06-22 18:50:24.485903 weewx-5.0.0b6/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
--rw-r--r--   0        0        0      676 2023-07-02 01:39:52.980626 weewx-5.0.0b6/bin/wee_resources/skins/Ftp/skin.conf
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/favicon.ico
--rw-r--r--   0        0        0     2573 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/index.html.tmpl
--rw-r--r--   0        0        0     1021 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/de.conf
--rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/en.conf
--rw-r--r--   0        0        0     1101 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/nl.conf
--rw-r--r--   0        0        0     2940 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/no.conf
--rw-r--r--   0        0        0      671 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/mobile.css
--rw-r--r--   0        0        0     5171 2023-07-02 01:39:52.984626 weewx-5.0.0b6/bin/wee_resources/skins/Mobile/skin.conf
--rw-r--r--   0        0        0      760 2023-07-02 01:39:52.988626 weewx-5.0.0b6/bin/wee_resources/skins/Rsync/skin.conf
--rw-r--r--   0        0        0     2667 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5460 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     1482 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/about.inc
--rw-r--r--   0        0        0      674 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/analytics.inc
--rw-r--r--   0        0        0     1137 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/celestial.html.tmpl
--rw-r--r--   0        0        0     6214 2023-06-22 18:50:24.489903 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/celestial.inc
--rw-r--r--   0        0        0     1291 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/current.inc
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/favicon.ico
--rw-r--r--   0        0        0   172876 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
--rw-r--r--   0        0        0   169744 2023-05-30 12:01:49.289499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
--rw-r--r--   0        0        0     4383 2023-06-22 18:50:24.489903 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OFL.txt
--rw-r--r--   0        0        0   224592 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   217360 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    20248 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans.woff
--rw-r--r--   0        0        0    10352 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
--rw-r--r--   0        0        0     4348 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/license.txt
--rw-r--r--   0        0        0     4360 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/hilo.inc
--rw-r--r--   0        0        0      858 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/identifier.inc
--rw-r--r--   0        0        0     2787 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/index.html.tmpl
--rw-r--r--   0        0        0     9216 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/cn.conf
--rw-r--r--   0        0        0     9844 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/cz.conf
--rw-r--r--   0        0        0     9745 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/de.conf
--rw-r--r--   0        0        0     9459 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/en.conf
--rw-r--r--   0        0        0    10702 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/es.conf
--rw-r--r--   0        0        0    10673 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/fr.conf
--rw-r--r--   0        0        0    11838 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/gr.conf
--rw-r--r--   0        0        0     9947 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/it.conf
--rw-r--r--   0        0        0     9548 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/nl.conf
--rw-r--r--   0        0        0    10705 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/no.conf
--rw-r--r--   0        0        0    15356 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/th.conf
--rw-r--r--   0        0        0      920 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/map.inc
--rw-r--r--   0        0        0      572 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/radar.inc
--rw-r--r--   0        0        0     4373 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/rss.xml.tmpl
--rw-r--r--   0        0        0      642 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/satellite.inc
--rw-r--r--   0        0        0     5406 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/seasons.css
--rw-r--r--   0        0        0     6404 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/seasons.js
--rw-r--r--   0        0        0     3947 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/sensors.inc
--rw-r--r--   0        0        0    27402 2023-07-02 01:39:52.992626 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/skin.conf
--rw-r--r--   0        0        0     1294 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/statistics.html.tmpl
--rw-r--r--   0        0        0     3971 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/statistics.inc
--rw-r--r--   0        0        0     2771 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/sunmoon.inc
--rw-r--r--   0        0        0      987 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/tabular.html.tmpl
--rw-r--r--   0        0        0     2450 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
--rw-r--r--   0        0        0     1115 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Seasons/titlebar.inc
--rw-r--r--   0        0        0     1804 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/custom.js
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/favicon.ico
--rw-r--r--   0        0        0     1043 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     2457 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1639 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/de.conf
--rw-r--r--   0        0        0     1554 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/en.conf
--rw-r--r--   0        0        0     1594 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/nl.conf
--rw-r--r--   0        0        0     3530 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/no.conf
--rw-r--r--   0        0        0     1502 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     7806 2023-07-02 01:39:52.992626 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/skin.conf
--rw-r--r--   0        0        0     1588 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/temp.html.tmpl
--rw-r--r--   0        0        0     1681 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/wind.html.tmpl
--rw-r--r--   0        0        0     2591 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5364 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     8546 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
--rw-r--r--   0        0        0       76 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/band.gif
--rw-r--r--   0        0        0     2593 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
--rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/drops.gif
--rw-r--r--   0        0        0     1386 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
--rw-r--r--   0        0        0     2277 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
--rw-r--r--   0        0        0     8609 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/night.gif
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/favicon.ico
--rw-r--r--   0        0        0   313856 2023-06-22 18:50:24.493903 weewx-5.0.0b6/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
--rw-r--r--   0        0        0    20739 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/index.html.tmpl
--rw-r--r--   0        0        0     9390 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/de.conf
--rw-r--r--   0        0        0     9264 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/en.conf
--rw-r--r--   0        0        0     9765 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/fr.conf
--rw-r--r--   0        0        0     9356 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/nl.conf
--rw-r--r--   0        0        0    10875 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/no.conf
--rw-r--r--   0        0        0    15140 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/month.html.tmpl
--rw-r--r--   0        0        0    16429 2023-07-02 01:39:52.992626 weewx-5.0.0b6/bin/wee_resources/skins/Standard/skin.conf
--rw-r--r--   0        0        0     1456 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/custom.js
--rw-r--r--   0        0        0     1012 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     1918 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
--rw-r--r--   0        0        0     1394 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     1441 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
--rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
--rw-r--r--   0        0        0    15057 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/week.html.tmpl
--rw-r--r--   0        0        0     3533 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/weewx.css
--rw-r--r--   0        0        0     9990 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/skins/Standard/year.html.tmpl
--rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-06-22 18:50:24.493903 weewx-5.0.0b6/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0      526 2023-06-24 20:56:10.599627 weewx-5.0.0b6/bin/wee_resources/util/systemd/weewx.service
--rw-r--r--   0        0        0    18375 2023-07-02 01:39:52.976626 weewx-5.0.0b6/bin/wee_resources/weewx.conf
--rw-r--r--   0        0        0    25898 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weecfg/__init__.py
--rw-r--r--   0        0        0    26461 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weecfg/database.py
--rw-r--r--   0        0        0    24020 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weecfg/extension.py
--rw-r--r--   0        0        0    33749 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weecfg/station_config.py
--rw-r--r--   0        0        0    45364 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weecfg/update_config.py
--rwxr-xr-x   0        0        0     1473 2023-07-02 01:39:33.428810 weewx-5.0.0b6/bin/weectl.py
--rw-r--r--   0        0        0     1831 2023-07-02 01:39:33.428810 weewx-5.0.0b6/bin/weectllib/__init__.py
--rw-r--r--   0        0        0    18865 2023-07-02 01:39:33.428810 weewx-5.0.0b6/bin/weectllib/database_cmd.py
--rw-r--r--   0        0        0    18055 2023-07-02 01:39:33.428810 weewx-5.0.0b6/bin/weectllib/db_actions.py
--rw-r--r--   0        0        0     6768 2023-06-30 12:11:26.893320 weewx-5.0.0b6/bin/weectllib/extension_cmd.py
--rw-r--r--   0        0        0    17231 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weectllib/station_cmd.py
--rw-r--r--   0        0        0     4538 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/weedb/NOTES.md
--rw-r--r--   0        0        0     6717 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weedb/__init__.py
--rw-r--r--   0        0        0    11213 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weedb/mysql.py
--rw-r--r--   0        0        0    11161 2023-06-22 18:50:24.453903 weewx-5.0.0b6/bin/weedb/sqlite.py
--rw-r--r--   0        0        0      255 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/weeimport/__init__.py
--rw-r--r--   0        0        0    11110 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/weeimport/csvimport.py
--rw-r--r--   0        0        0    20265 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/weeimport/cumulusimport.py
--rw-r--r--   0        0        0    35701 2023-05-30 12:01:49.269499 weewx-5.0.0b6/bin/weeimport/wdimport.py
--rw-r--r--   0        0        0    18225 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeimport/weathercatimport.py
--rw-r--r--   0        0        0    69526 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeimport/weeimport.py
--rw-r--r--   0        0        0    17222 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeimport/wuimport.py
--rw-r--r--   0        0        0      367 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeplot/__init__.py
--rw-r--r--   0        0        0    33267 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeplot/genplot.py
--rw-r--r--   0        0        0    24811 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeplot/utilities.py
--rw-r--r--   0        0        0     1633 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeutil/Moon.py
--rw-r--r--   0        0        0    18296 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeutil/Sun.py
--rw-r--r--   0        0        0      142 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeutil/__init__.py
--rw-r--r--   0        0        0     9408 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeutil/config.py
--rw-r--r--   0        0        0    12986 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeutil/ftpupload.py
--rw-r--r--   0        0        0     3150 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeutil/log.py
--rw-r--r--   0        0        0     5896 2023-06-22 18:50:24.457903 weewx-5.0.0b6/bin/weeutil/logger.py
--rw-r--r--   0        0        0     6593 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeutil/rsyncupload.py
--rw-r--r--   0        0        0     2224 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weeutil/timediff.py
--rw-r--r--   0        0        0    65551 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weeutil/weeutil.py
--rw-r--r--   0        0        0     5929 2023-07-02 01:39:52.996626 weewx-5.0.0b6/bin/weewx/__init__.py
--rw-r--r--   0        0        0    26063 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/accum.py
--rw-r--r--   0        0        0    25229 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/almanac.py
--rw-r--r--   0        0        0    33390 2023-06-26 15:33:43.623098 weewx-5.0.0b6/bin/weewx/cheetahgenerator.py
--rw-r--r--   0        0        0     3393 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/crc16.py
--rw-r--r--   0        0        0     2888 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/daemon.py
--rw-r--r--   0        0        0    11955 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/defaults.py
--rw-r--r--   0        0        0     5148 2023-06-26 23:49:37.357451 weewx-5.0.0b6/bin/weewx/drivers/__init__.py
--rw-r--r--   0        0        0    38987 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/acurite.py
--rw-r--r--   0        0        0    64005 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/drivers/cc3000.py
--rw-r--r--   0        0        0    78592 2023-06-22 18:50:24.461903 weewx-5.0.0b6/bin/weewx/drivers/fousb.py
--rw-r--r--   0        0        0    14931 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/simulator.py
--rw-r--r--   0        0        0    99881 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/te923.py
--rw-r--r--   0        0        0    15797 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/ultimeter.py
--rw-r--r--   0        0        0   139716 2023-06-27 00:08:59.518408 weewx-5.0.0b6/bin/weewx/drivers/vantage.py
--rw-r--r--   0        0        0    17795 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/wmr100.py
--rw-r--r--   0        0        0    72747 2023-05-30 12:01:49.273499 weewx-5.0.0b6/bin/weewx/drivers/wmr300.py
--rw-r--r--   0        0        0    29536 2023-06-22 18:50:24.465903 weewx-5.0.0b6/bin/weewx/drivers/wmr9x8.py
--rw-r--r--   0        0        0    18843 2023-06-22 18:50:24.465903 weewx-5.0.0b6/bin/weewx/drivers/ws1.py
--rw-r--r--   0        0        0    79489 2023-06-22 18:50:24.465903 weewx-5.0.0b6/bin/weewx/drivers/ws23xx.py
--rw-r--r--   0        0        0   173578 2023-05-30 12:01:49.277499 weewx-5.0.0b6/bin/weewx/drivers/ws28xx.py
--rw-r--r--   0        0        0    37475 2023-06-22 18:50:24.465903 weewx-5.0.0b6/bin/weewx/engine.py
--rw-r--r--   0        0        0      276 2023-05-30 12:01:49.277499 weewx-5.0.0b6/bin/weewx/filegenerator.py
--rw-r--r--   0        0        0    18278 2023-06-22 18:50:24.465903 weewx-5.0.0b6/bin/weewx/imagegenerator.py
--rw-r--r--   0        0        0    73115 2023-06-30 19:01:08.594144 weewx-5.0.0b6/bin/weewx/manager.py
--rw-r--r--   0        0        0     3187 2023-05-30 12:01:49.277499 weewx-5.0.0b6/bin/weewx/qc.py
--rw-r--r--   0        0        0    37780 2023-06-22 18:50:24.469903 weewx-5.0.0b6/bin/weewx/reportengine.py
--rw-r--r--   0        0        0    79730 2023-06-22 18:50:24.469903 weewx-5.0.0b6/bin/weewx/restx.py
--rw-r--r--   0        0        0     7207 2023-05-30 12:01:49.277499 weewx-5.0.0b6/bin/weewx/station.py
--rw-r--r--   0        0        0    31690 2023-06-22 18:50:24.469903 weewx-5.0.0b6/bin/weewx/tags.py
--rw-r--r--   0        0        0    71594 2023-06-22 18:50:24.473903 weewx-5.0.0b6/bin/weewx/units.py
--rw-r--r--   0        0        0    25248 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/uwxutils.py
--rw-r--r--   0        0        0      246 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/wxengine.py
--rw-r--r--   0        0        0    30034 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/wxformulas.py
--rw-r--r--   0        0        0      367 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/wxmanager.py
--rw-r--r--   0        0        0     7270 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/wxservices.py
--rw-r--r--   0        0        0    34292 2023-05-30 12:01:49.281499 weewx-5.0.0b6/bin/weewx/wxxtypes.py
--rw-r--r--   0        0        0    55988 2023-06-22 18:50:24.473903 weewx-5.0.0b6/bin/weewx/xtypes.py
--rwxr-xr-x   0        0        0     9648 2023-06-22 18:50:24.473903 weewx-5.0.0b6/bin/weewxd.py
--rw-r--r--   0        0        0    12175 2023-06-22 18:50:24.485903 weewx-5.0.0b6/pkg/changelog.el
--rw-r--r--   0        0        0    12070 2023-06-22 18:50:24.485903 weewx-5.0.0b6/pkg/changelog.suse
--rw-r--r--   0        0        0     2731 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/debian/README
--rw-r--r--   0        0        0    21471 2023-06-22 18:50:24.485903 weewx-5.0.0b6/pkg/debian/changelog
--rw-r--r--   0        0        0        3 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/compat
--rw-r--r--   0        0        0       36 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/debian/conffiles
--rwxr-xr-x   0        0        0     3398 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/config
--rw-r--r--   0        0        0      724 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/control
--rw-r--r--   0        0        0      926 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/copyright
--rwxr-xr-x   0        0        0     8937 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/postinst
--rwxr-xr-x   0        0        0      906 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/debian/postrm
--rwxr-xr-x   0        0        0      410 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/debian/preinst
--rwxr-xr-x   0        0        0      693 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/prerm
--rwxr-xr-x   0        0        0     2985 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/rules
--rw-r--r--   0        0        0       12 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/debian/source/format
--rw-r--r--   0        0        0     5501 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/debian/templates
--rw-r--r--   0        0        0     1708 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/index-apt.html
--rw-r--r--   0        0        0     1728 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/index-suse.html
--rw-r--r--   0        0        0     1714 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/index-yum.html
--rwxr-xr-x   0        0        0     9874 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/mkchangelog.pl
--rw-r--r--   0        0        0       79 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx-el8.repo
--rw-r--r--   0        0        0       57 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx-python2.list
--rw-r--r--   0        0        0       56 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx-python3.list
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx-suse12.repo
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx-suse15.repo
--rw-r--r--   0        0        0     2201 2023-05-30 12:01:49.289499 weewx-5.0.0b6/pkg/weewx.smf
--rw-r--r--   0        0        0     7144 2023-06-22 18:50:24.489903 weewx-5.0.0b6/pkg/weewx.spec.in
--rw-r--r--   0        0        0     2796 2023-07-02 01:39:46.020692 weewx-5.0.0b6/pyproject.toml
--rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/apache/conf-available/weewx.conf
--rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/apache/conf.d/weewx.conf
--rw-r--r--   0        0        0      136 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/default/weewx
--rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/i18n/i18n-report
--rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/import/csv-example.conf
--rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/import/cumulus-example.conf
--rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/import/wd-example.conf
--rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/import/weathercat-example.conf
--rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/import/wu-example.conf
--rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/logrotate.d/weewx
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/logwatch/conf/logfiles/weewx.conf
--rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/logwatch/conf/services/weewx.conf
--rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/logwatch/scripts/services/weewx
--rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/newsyslog.d/weewx.conf
--rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/rsyslog.d/weewx.conf
--rwxr-xr-x   0        0        0      319 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/wee_database
--rwxr-xr-x   0        0        0      316 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/wee_debug
--rwxr-xr-x   0        0        0      317 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/wee_device
--rwxr-xr-x   0        0        0      317 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/wee_import
--rwxr-xr-x   0        0        0      318 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/wee_reports
--rwxr-xr-x   0        0        0      313 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/weectl
--rwxr-xr-x   0        0        0      313 2023-06-22 18:50:24.493903 weewx-5.0.0b6/util/scripts/weewxd
--rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/solaris/weewx-smf.xml
--rw-r--r--   0        0        0      526 2023-06-24 20:56:10.599627 weewx-5.0.0b6/util/systemd/weewx.service
--rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/tmpfiles.d/weewx.conf
--rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/acurite.rules
--rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/cc3000.rules
--rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/fousb.rules
--rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/te923.rules
--rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/vantage.rules
--rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/weewx.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/wmr100.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/wmr300.rules
--rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b6/util/udev/rules.d/ws28xx.rules
--rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 weewx-5.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-05-30 12:01:49.265499 weewx-5.0.0b7/LICENSE.txt
+-rw-r--r--   0        0        0     3725 2023-06-22 18:50:33.745869 weewx-5.0.0b7/README.md
+-rw-r--r--   0        0        0      230 2023-05-30 12:01:49.265499 weewx-5.0.0b7/bin/schemas/__init__.py
+-rw-r--r--   0        0        0     3448 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/schemas/wview.py
+-rw-r--r--   0        0        0     5953 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/schemas/wview_extended.py
+-rw-r--r--   0        0        0     2105 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/schemas/wview_small.py
+-rwxr-xr-x   0        0        0    52292 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/wee_database.py
+-rwxr-xr-x   0        0        0    16172 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/wee_debug.py
+-rwxr-xr-x   0        0        0     2187 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/wee_device.py
+-rwxr-xr-x   0        0        0    38942 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/wee_import.py
+-rwxr-xr-x   0        0        0     5630 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/wee_reports.py
+-rw-r--r--   0        0        0        0 2023-07-02 01:40:06.556500 weewx-5.0.0b7/bin/wee_resources/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/wee_resources/bin/user/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-26 17:07:40.592701 weewx-5.0.0b7/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      398 2023-06-26 17:07:40.592701 weewx-5.0.0b7/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
+-rw-r--r--   0        0        0      541 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/wee_resources/bin/user/extensions.py
+-rw-r--r--   0        0        0    33173 2023-06-30 14:55:56.834551 weewx-5.0.0b7/bin/wee_resources/docs/404.html
+-rw-r--r--   0        0        0     1870 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0   113455 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css
+-rw-r--r--   0        0        0    38958 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map
+-rw-r--r--   0        0        0    12227 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css
+-rw-r--r--   0        0        0     3628 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map
+-rw-r--r--   0        0        0   195059 2023-06-30 14:55:56.878550 weewx-5.0.0b7/bin/wee_resources/docs/changes/index.html
+-rw-r--r--   0        0        0    35875 2023-06-30 14:55:56.878550 weewx-5.0.0b7/bin/wee_resources/docs/copyright/index.html
+-rw-r--r--   0        0        0      565 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/css/tocbot-4.12.0.css
+-rw-r--r--   0        0        0      565 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/css/tocbot-4.3.1.css
+-rw-r--r--   0        0        0    12148 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/css/weewx_ui.css
+-rw-r--r--   0        0        0    62945 2023-06-30 14:55:56.958550 weewx-5.0.0b7/bin/wee_resources/docs/custom/appendix/index.html
+-rw-r--r--   0        0        0   141082 2023-06-30 14:55:56.998550 weewx-5.0.0b7/bin/wee_resources/docs/custom/cheetah/index.html
+-rw-r--r--   0        0        0    72678 2023-06-30 14:55:57.014550 weewx-5.0.0b7/bin/wee_resources/docs/custom/custom-reports/index.html
+-rw-r--r--   0        0        0    60357 2023-06-30 14:55:57.022549 weewx-5.0.0b7/bin/wee_resources/docs/custom/database/index.html
+-rw-r--r--   0        0        0    34898 2023-06-30 14:55:57.026549 weewx-5.0.0b7/bin/wee_resources/docs/custom/derived/index.html
+-rw-r--r--   0        0        0    49193 2023-06-30 14:55:57.030549 weewx-5.0.0b7/bin/wee_resources/docs/custom/drivers/index.html
+-rw-r--r--   0        0        0    40560 2023-06-30 14:55:57.034549 weewx-5.0.0b7/bin/wee_resources/docs/custom/extensions/index.html
+-rw-r--r--   0        0        0    61818 2023-06-30 14:55:57.042549 weewx-5.0.0b7/bin/wee_resources/docs/custom/image-generator/index.html
+-rw-r--r--   0        0        0    71102 2023-06-30 14:55:56.946550 weewx-5.0.0b7/bin/wee_resources/docs/custom/index.html
+-rw-r--r--   0        0        0    65111 2023-06-30 14:55:57.058549 weewx-5.0.0b7/bin/wee_resources/docs/custom/localization/index.html
+-rw-r--r--   0        0        0    48063 2023-06-30 14:55:57.062549 weewx-5.0.0b7/bin/wee_resources/docs/custom/multiple-bindings/index.html
+-rw-r--r--   0        0        0   119836 2023-06-30 14:55:57.086549 weewx-5.0.0b7/bin/wee_resources/docs/custom/report-options/index.html
+-rw-r--r--   0        0        0    51200 2023-06-30 14:55:57.090549 weewx-5.0.0b7/bin/wee_resources/docs/custom/report-scheduling/index.html
+-rw-r--r--   0        0        0    83633 2023-06-30 14:55:57.114549 weewx-5.0.0b7/bin/wee_resources/docs/custom/service-engine/index.html
+-rw-r--r--   0        0        0    45932 2023-06-30 14:55:57.122549 weewx-5.0.0b7/bin/wee_resources/docs/custom/units/index.html
+-rw-r--r--   0        0        0    71286 2023-06-30 14:55:56.890550 weewx-5.0.0b7/bin/wee_resources/docs/devnotes/index.html
+-rw-r--r--   0        0        0     2747 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/examples/tag.htm
+-rw-r--r--   0        0        0    40976 2023-06-30 14:55:57.126549 weewx-5.0.0b7/bin/wee_resources/docs/hardware/acurite/index.html
+-rw-r--r--   0        0        0    62045 2023-06-30 14:55:57.134549 weewx-5.0.0b7/bin/wee_resources/docs/hardware/cc3000/index.html
+-rw-r--r--   0        0        0    56652 2023-06-30 14:55:57.150549 weewx-5.0.0b7/bin/wee_resources/docs/hardware/drivers/index.html
+-rw-r--r--   0        0        0    48664 2023-06-30 14:55:57.158548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/fousb/index.html
+-rw-r--r--   0        0        0    47333 2023-06-30 14:55:57.162549 weewx-5.0.0b7/bin/wee_resources/docs/hardware/te923/index.html
+-rw-r--r--   0        0        0    38960 2023-06-30 14:55:57.166549 weewx-5.0.0b7/bin/wee_resources/docs/hardware/ultimeter/index.html
+-rw-r--r--   0        0        0    69205 2023-06-30 14:55:57.178548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/vantage/index.html
+-rw-r--r--   0        0        0    43515 2023-06-30 14:55:57.182548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr100/index.html
+-rw-r--r--   0        0        0    43628 2023-06-30 14:55:57.190548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr300/index.html
+-rw-r--r--   0        0        0    43159 2023-06-30 14:55:57.198548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr9x8/index.html
+-rw-r--r--   0        0        0    38243 2023-06-30 14:55:57.198548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws1/index.html
+-rw-r--r--   0        0        0    45030 2023-06-30 14:55:57.202548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws23xx/index.html
+-rw-r--r--   0        0        0    50646 2023-06-30 14:55:57.206548 weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws28xx/index.html
+-rw-r--r--   0        0        0    54196 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/antialias.gif
+-rw-r--r--   0        0        0     3145 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/day-gap-not-shown.png
+-rw-r--r--   0        0        0     3269 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/day-gap-showing.png
+-rw-r--r--   0        0        0     7579 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/daycompare.png
+-rw-r--r--   0        0        0     8705 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/daytemp_with_avg.png
+-rw-r--r--   0        0        0     7803 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/dayvaporp.png
+-rw-r--r--   0        0        0     7663 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/daywindvec.png
+-rw-r--r--   0        0        0     1026 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/favicon.png
+-rw-r--r--   0        0        0    38406 2023-06-30 14:55:56.730551 weewx-5.0.0b7/bin/wee_resources/docs/images/ferrites.jpg
+-rw-r--r--   0        0        0     3638 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/funky_degree.png
+-rw-r--r--   0        0        0    19123 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/image_parts.png
+-rw-r--r--   0        0        0    86388 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/image_parts.xcf
+-rw-r--r--   0        0        0     2136 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-apple.png
+-rw-r--r--   0        0        0     4734 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-centos.png
+-rw-r--r--   0        0        0    14541 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-debian.png
+-rw-r--r--   0        0        0    24662 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-fedora.png
+-rw-r--r--   0        0        0    12046 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-linux.png
+-rw-r--r--   0        0        0    27245 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-mint.png
+-rw-r--r--   0        0        0    15980 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-opensuse.png
+-rw-r--r--   0        0        0    14374 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-pypi.svg
+-rw-r--r--   0        0        0     1192 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-redhat.png
+-rw-r--r--   0        0        0     3926 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-rpi.png
+-rw-r--r--   0        0        0     7877 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-suse.png
+-rw-r--r--   0        0        0    13954 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-ubuntu.png
+-rw-r--r--   0        0        0    12208 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/logo-weewx.png
+-rw-r--r--   0        0        0    35496 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/pipeline.png
+-rw-r--r--   0        0        0     6709 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/sample_monthrain.png
+-rw-r--r--   0        0        0    10107 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/sample_monthtempdew.png
+-rw-r--r--   0        0        0    10649 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/weekgustoverlay.png
+-rw-r--r--   0        0        0     8468 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/weektempdew.png
+-rw-r--r--   0        0        0     6602 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/yeardiff.png
+-rw-r--r--   0        0        0     7286 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/images/yearhilow.png
+-rw-r--r--   0        0        0    39555 2023-06-30 14:55:56.850551 weewx-5.0.0b7/bin/wee_resources/docs/index.html
+-rw-r--r--   0        0        0    32611 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/cash.js
+-rw-r--r--   0        0        0    14828 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/cash.min.js
+-rw-r--r--   0        0        0    11422 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.12.0.js
+-rw-r--r--   0        0        0    11422 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
+-rw-r--r--   0        0        0     8892 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
+-rw-r--r--   0        0        0     4640 2023-06-30 14:55:56.734551 weewx-5.0.0b7/bin/wee_resources/docs/js/weewx.js
+-rw-r--r--   0        0        0    44042 2023-06-30 14:55:57.214548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/debian/index.html
+-rw-r--r--   0        0        0    44892 2023-06-30 14:55:57.218548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/git/index.html
+-rw-r--r--   0        0        0    34859 2023-06-30 14:55:57.210548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/index.html
+-rw-r--r--   0        0        0    61186 2023-06-30 14:55:57.230548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/pip/index.html
+-rw-r--r--   0        0        0    42835 2023-06-30 14:55:57.234548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/redhat/index.html
+-rw-r--r--   0        0        0    41774 2023-06-30 14:55:57.238548 weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/suse/index.html
+-rw-r--r--   0        0        0  1039833 2023-06-30 14:55:57.418547 weewx-5.0.0b7/bin/wee_resources/docs/search/search_index.json
+-rw-r--r--   0        0        0    12605 2023-06-30 14:55:56.738551 weewx-5.0.0b7/bin/wee_resources/docs/sitemap.xml
+-rw-r--r--   0        0        0      750 2023-06-30 14:55:56.742551 weewx-5.0.0b7/bin/wee_resources/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    95313 2023-06-30 14:55:56.914550 weewx-5.0.0b7/bin/wee_resources/docs/sle/index.html
+-rw-r--r--   0        0        0    38042 2023-06-30 14:55:57.254548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
+-rw-r--r--   0        0        0    34819 2023-06-30 14:55:57.250548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/index.html
+-rw-r--r--   0        0        0    41075 2023-06-30 14:55:57.258548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/installing-weewx/index.html
+-rw-r--r--   0        0        0    39324 2023-06-30 14:55:57.262548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
+-rw-r--r--   0        0        0    38374 2023-06-30 14:55:57.266548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/running-weewx/index.html
+-rw-r--r--   0        0        0    38405 2023-06-30 14:55:57.266548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/system-requirements/index.html
+-rw-r--r--   0        0        0    41481 2023-06-30 14:55:57.286548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html
+-rw-r--r--   0        0        0    34943 2023-06-30 14:55:57.282548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/index.html
+-rw-r--r--   0        0        0    41997 2023-06-30 14:55:57.286548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html
+-rw-r--r--   0        0        0    62539 2023-06-30 14:55:57.298548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html
+-rw-r--r--   0        0        0    41816 2023-06-30 14:55:57.274548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/webserver-integration/index.html
+-rw-r--r--   0        0        0    38891 2023-06-30 14:55:57.302548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
+-rw-r--r--   0        0        0    38398 2023-06-30 14:55:57.306547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
+-rw-r--r--   0        0        0    41822 2023-06-30 14:55:57.310547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
+-rw-r--r--   0        0        0    42451 2023-06-30 14:55:57.314548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
+-rw-r--r--   0        0        0    39419 2023-06-30 14:55:57.318548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
+-rw-r--r--   0        0        0    37700 2023-06-30 14:55:57.298548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
+-rw-r--r--   0        0        0    84111 2023-06-30 14:55:57.330547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
+-rw-r--r--   0        0        0    40224 2023-06-30 14:55:57.334547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
+-rw-r--r--   0        0        0    36761 2023-06-30 14:55:57.334547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
+-rw-r--r--   0        0        0    37346 2023-06-30 14:55:57.338547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
+-rw-r--r--   0        0        0    37554 2023-06-30 14:55:57.342547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
+-rw-r--r--   0        0        0    60169 2023-06-30 14:55:57.346547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
+-rw-r--r--   0        0        0    70287 2023-06-30 14:55:57.358547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
+-rw-r--r--   0        0        0    35735 2023-06-30 14:55:57.358547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
+-rw-r--r--   0        0        0    56824 2023-06-30 14:55:57.366547 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
+-rw-r--r--   0        0        0    42668 2023-06-30 14:55:57.278548 weewx-5.0.0b7/bin/wee_resources/docs/usersguide/where/index.html
+-rw-r--r--   0        0        0    57266 2023-06-30 14:55:57.374547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_database/index.html
+-rw-r--r--   0        0        0    46043 2023-06-30 14:55:57.378547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_debug/index.html
+-rw-r--r--   0        0        0    36328 2023-06-30 14:55:57.378547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_device/index.html
+-rw-r--r--   0        0        0   254677 2023-06-30 14:55:57.398547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_import/index.html
+-rw-r--r--   0        0        0    38640 2023-06-30 14:55:57.402547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_reports/index.html
+-rw-r--r--   0        0        0    49036 2023-06-30 14:55:57.406547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/weectl-extension/index.html
+-rw-r--r--   0        0        0    63373 2023-06-30 14:55:57.414547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/weectl-station/index.html
+-rw-r--r--   0        0        0    35546 2023-06-30 14:55:57.414547 weewx-5.0.0b7/bin/wee_resources/docs/utilities/weewxd/index.html
+-rw-r--r--   0        0        0   150560 2023-06-30 14:55:56.934550 weewx-5.0.0b7/bin/wee_resources/docs/versions/index.html
+-rw-r--r--   0        0        0     3097 2023-06-26 17:07:40.352703 weewx-5.0.0b7/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
+-rw-r--r--   0        0        0    10729 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/alarm.py
+-rw-r--r--   0        0        0      179 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/basic/changelog
+-rw-r--r--   0        0        0     1563 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/basic/install.py
+-rw-r--r--   0        0        0     1243 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/basic/readme.md
+-rw-r--r--   0        0        0     1510 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/basic.css
+-rw-r--r--   0        0        0     6451 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/current.inc
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/favicon.ico
+-rw-r--r--   0        0        0    11292 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/hilo.inc
+-rw-r--r--   0        0        0     1665 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
+-rw-r--r--   0        0        0     2216 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
+-rw-r--r--   0        0        0     2408 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
+-rw-r--r--   0        0        0     3173 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/skin.conf
+-rw-r--r--   0        0        0     2080 2023-06-26 17:07:37.972717 weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
+-rw-r--r--   0        0        0     2255 2023-06-26 17:07:37.992717 weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
+-rw-r--r--   0        0        0     3290 2023-06-26 17:07:37.992717 weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
+-rw-r--r--   0        0        0     2128 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_1.py
+-rw-r--r--   0        0        0     2617 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_2.py
+-rw-r--r--   0        0        0     4001 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_3.py
+-rw-r--r--   0        0        0     4180 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
+-rw-r--r--   0        0        0      269 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/fileparse/changelog
+-rw-r--r--   0        0        0      835 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/fileparse/install.py
+-rw-r--r--   0        0        0     2086 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/fileparse/readme.md
+-rw-r--r--   0        0        0    10792 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/lowBattery.py
+-rw-r--r--   0        0        0     1108 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/mem.py
+-rw-r--r--   0        0        0     5986 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/pmon/bin/user/pmon.py
+-rw-r--r--   0        0        0      341 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/pmon/changelog
+-rw-r--r--   0        0        0     1511 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/pmon/install.py
+-rw-r--r--   0        0        0     2628 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/pmon/readme.md
+-rw-r--r--   0        0        0      507 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
+-rw-r--r--   0        0        0     1234 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
+-rw-r--r--   0        0        0     4334 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/tests/test_vaporpressure.py
+-rw-r--r--   0        0        0     4285 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/examples/vaporpressure.py
+-rw-r--r--   0        0        0     3034 2023-06-26 17:07:38.004717 weewx-5.0.0b7/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
+-rw-r--r--   0        0        0     5662 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/bin/user/xstats.py
+-rw-r--r--   0        0        0      146 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/changelog
+-rw-r--r--   0        0        0      850 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/install.py
+-rw-r--r--   0        0        0     2923 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/readme.txt
+-rw-r--r--   0        0        0     2138 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
+-rw-r--r--   0        0        0      591 2023-06-22 18:50:24.485903 weewx-5.0.0b7/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
+-rw-r--r--   0        0        0      676 2023-07-02 01:39:52.980626 weewx-5.0.0b7/bin/wee_resources/skins/Ftp/skin.conf
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/favicon.ico
+-rw-r--r--   0        0        0     2573 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/index.html.tmpl
+-rw-r--r--   0        0        0     1021 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/de.conf
+-rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/en.conf
+-rw-r--r--   0        0        0     1101 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/nl.conf
+-rw-r--r--   0        0        0     2940 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/no.conf
+-rw-r--r--   0        0        0      671 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/mobile.css
+-rw-r--r--   0        0        0     5171 2023-07-02 01:39:52.984626 weewx-5.0.0b7/bin/wee_resources/skins/Mobile/skin.conf
+-rw-r--r--   0        0        0      760 2023-07-02 01:39:52.988626 weewx-5.0.0b7/bin/wee_resources/skins/Rsync/skin.conf
+-rw-r--r--   0        0        0     2667 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5460 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     1482 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/about.inc
+-rw-r--r--   0        0        0      674 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/analytics.inc
+-rw-r--r--   0        0        0     1137 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/celestial.html.tmpl
+-rw-r--r--   0        0        0     6214 2023-06-22 18:50:24.489903 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/celestial.inc
+-rw-r--r--   0        0        0     1291 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/current.inc
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/favicon.ico
+-rw-r--r--   0        0        0   172876 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
+-rw-r--r--   0        0        0   169744 2023-05-30 12:01:49.289499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
+-rw-r--r--   0        0        0     4383 2023-06-22 18:50:24.489903 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OFL.txt
+-rw-r--r--   0        0        0   224592 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   217360 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    20248 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans.woff
+-rw-r--r--   0        0        0    10352 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
+-rw-r--r--   0        0        0     4348 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/license.txt
+-rw-r--r--   0        0        0     4360 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/hilo.inc
+-rw-r--r--   0        0        0      858 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/identifier.inc
+-rw-r--r--   0        0        0     2787 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/index.html.tmpl
+-rw-r--r--   0        0        0     9216 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/cn.conf
+-rw-r--r--   0        0        0     9844 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/cz.conf
+-rw-r--r--   0        0        0     9745 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/de.conf
+-rw-r--r--   0        0        0     9459 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/en.conf
+-rw-r--r--   0        0        0    10702 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/es.conf
+-rw-r--r--   0        0        0    10673 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/fr.conf
+-rw-r--r--   0        0        0    11838 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/gr.conf
+-rw-r--r--   0        0        0     9947 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/it.conf
+-rw-r--r--   0        0        0     9548 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/nl.conf
+-rw-r--r--   0        0        0    10705 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/no.conf
+-rw-r--r--   0        0        0    15356 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/th.conf
+-rw-r--r--   0        0        0      920 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/map.inc
+-rw-r--r--   0        0        0      572 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/radar.inc
+-rw-r--r--   0        0        0     4373 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/rss.xml.tmpl
+-rw-r--r--   0        0        0      642 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/satellite.inc
+-rw-r--r--   0        0        0     5406 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/seasons.css
+-rw-r--r--   0        0        0     6404 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/seasons.js
+-rw-r--r--   0        0        0     3947 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/sensors.inc
+-rw-r--r--   0        0        0    27402 2023-07-02 01:39:52.992626 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/skin.conf
+-rw-r--r--   0        0        0     1294 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/statistics.html.tmpl
+-rw-r--r--   0        0        0     3971 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/statistics.inc
+-rw-r--r--   0        0        0     2771 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/sunmoon.inc
+-rw-r--r--   0        0        0      987 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/tabular.html.tmpl
+-rw-r--r--   0        0        0     2450 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
+-rw-r--r--   0        0        0     1115 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Seasons/titlebar.inc
+-rw-r--r--   0        0        0     1804 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/custom.js
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/favicon.ico
+-rw-r--r--   0        0        0     1043 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     2457 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1639 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/de.conf
+-rw-r--r--   0        0        0     1554 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/en.conf
+-rw-r--r--   0        0        0     1594 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/nl.conf
+-rw-r--r--   0        0        0     3530 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/no.conf
+-rw-r--r--   0        0        0     1502 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     7806 2023-07-02 01:39:52.992626 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/skin.conf
+-rw-r--r--   0        0        0     1588 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/temp.html.tmpl
+-rw-r--r--   0        0        0     1681 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0     2591 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5364 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     8546 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
+-rw-r--r--   0        0        0       76 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/band.gif
+-rw-r--r--   0        0        0     2593 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
+-rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/drops.gif
+-rw-r--r--   0        0        0     1386 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
+-rw-r--r--   0        0        0     2277 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
+-rw-r--r--   0        0        0     8609 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/night.gif
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/favicon.ico
+-rw-r--r--   0        0        0   313856 2023-06-22 18:50:24.493903 weewx-5.0.0b7/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0        0        0    20739 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/index.html.tmpl
+-rw-r--r--   0        0        0     9390 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/de.conf
+-rw-r--r--   0        0        0     9264 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/en.conf
+-rw-r--r--   0        0        0     9765 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/fr.conf
+-rw-r--r--   0        0        0     9356 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/nl.conf
+-rw-r--r--   0        0        0    10875 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/no.conf
+-rw-r--r--   0        0        0    15140 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/month.html.tmpl
+-rw-r--r--   0        0        0    16429 2023-07-02 01:39:52.992626 weewx-5.0.0b7/bin/wee_resources/skins/Standard/skin.conf
+-rw-r--r--   0        0        0     1456 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/custom.js
+-rw-r--r--   0        0        0     1012 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     1918 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
+-rw-r--r--   0        0        0     1394 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     1441 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
+-rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0    15057 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/week.html.tmpl
+-rw-r--r--   0        0        0     3533 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/weewx.css
+-rw-r--r--   0        0        0     9990 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/skins/Standard/year.html.tmpl
+-rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-06-22 18:50:24.493903 weewx-5.0.0b7/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0      526 2023-06-24 20:56:10.599627 weewx-5.0.0b7/bin/wee_resources/util/systemd/weewx.service
+-rw-r--r--   0        0        0    18375 2023-07-02 01:39:52.976626 weewx-5.0.0b7/bin/wee_resources/weewx.conf
+-rw-r--r--   0        0        0    25898 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weecfg/__init__.py
+-rw-r--r--   0        0        0    26461 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weecfg/database.py
+-rw-r--r--   0        0        0    24020 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weecfg/extension.py
+-rw-r--r--   0        0        0    33749 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weecfg/station_config.py
+-rw-r--r--   0        0        0    45364 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weecfg/update_config.py
+-rwxr-xr-x   0        0        0     1473 2023-07-02 01:39:33.428810 weewx-5.0.0b7/bin/weectl.py
+-rw-r--r--   0        0        0     1831 2023-07-02 01:39:33.428810 weewx-5.0.0b7/bin/weectllib/__init__.py
+-rw-r--r--   0        0        0    18865 2023-07-02 01:39:33.428810 weewx-5.0.0b7/bin/weectllib/database_cmd.py
+-rw-r--r--   0        0        0    18055 2023-07-02 01:39:33.428810 weewx-5.0.0b7/bin/weectllib/db_actions.py
+-rw-r--r--   0        0        0     6768 2023-06-30 12:11:26.893320 weewx-5.0.0b7/bin/weectllib/extension_cmd.py
+-rw-r--r--   0        0        0    17231 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weectllib/station_cmd.py
+-rw-r--r--   0        0        0     4538 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/weedb/NOTES.md
+-rw-r--r--   0        0        0     6717 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weedb/__init__.py
+-rw-r--r--   0        0        0    11213 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weedb/mysql.py
+-rw-r--r--   0        0        0    11161 2023-06-22 18:50:24.453903 weewx-5.0.0b7/bin/weedb/sqlite.py
+-rw-r--r--   0        0        0      255 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/weeimport/__init__.py
+-rw-r--r--   0        0        0    11110 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/weeimport/csvimport.py
+-rw-r--r--   0        0        0    20265 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/weeimport/cumulusimport.py
+-rw-r--r--   0        0        0    35701 2023-05-30 12:01:49.269499 weewx-5.0.0b7/bin/weeimport/wdimport.py
+-rw-r--r--   0        0        0    18225 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeimport/weathercatimport.py
+-rw-r--r--   0        0        0    69526 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeimport/weeimport.py
+-rw-r--r--   0        0        0    17222 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeimport/wuimport.py
+-rw-r--r--   0        0        0      367 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeplot/__init__.py
+-rw-r--r--   0        0        0    33267 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeplot/genplot.py
+-rw-r--r--   0        0        0    25533 2023-07-02 15:55:57.217087 weewx-5.0.0b7/bin/weeplot/utilities.py
+-rw-r--r--   0        0        0     1633 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeutil/Moon.py
+-rw-r--r--   0        0        0    18296 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeutil/Sun.py
+-rw-r--r--   0        0        0      142 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeutil/__init__.py
+-rw-r--r--   0        0        0     9408 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeutil/config.py
+-rw-r--r--   0        0        0    12986 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeutil/ftpupload.py
+-rw-r--r--   0        0        0     3150 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeutil/log.py
+-rw-r--r--   0        0        0     5896 2023-06-22 18:50:24.457903 weewx-5.0.0b7/bin/weeutil/logger.py
+-rw-r--r--   0        0        0     6593 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeutil/rsyncupload.py
+-rw-r--r--   0        0        0     2224 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weeutil/timediff.py
+-rw-r--r--   0        0        0    65551 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weeutil/weeutil.py
+-rw-r--r--   0        0        0     5929 2023-07-02 01:39:52.996626 weewx-5.0.0b7/bin/weewx/__init__.py
+-rw-r--r--   0        0        0    26063 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/accum.py
+-rw-r--r--   0        0        0    25229 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/almanac.py
+-rw-r--r--   0        0        0    33390 2023-06-26 15:33:43.623098 weewx-5.0.0b7/bin/weewx/cheetahgenerator.py
+-rw-r--r--   0        0        0     3393 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/crc16.py
+-rw-r--r--   0        0        0     2888 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/daemon.py
+-rw-r--r--   0        0        0    11955 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/defaults.py
+-rw-r--r--   0        0        0     5148 2023-06-26 23:49:37.357451 weewx-5.0.0b7/bin/weewx/drivers/__init__.py
+-rw-r--r--   0        0        0    38987 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/acurite.py
+-rw-r--r--   0        0        0    64005 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/drivers/cc3000.py
+-rw-r--r--   0        0        0    78592 2023-06-22 18:50:24.461903 weewx-5.0.0b7/bin/weewx/drivers/fousb.py
+-rw-r--r--   0        0        0    14931 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/simulator.py
+-rw-r--r--   0        0        0    99881 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/te923.py
+-rw-r--r--   0        0        0    15797 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/ultimeter.py
+-rw-r--r--   0        0        0   139716 2023-06-27 00:08:59.518408 weewx-5.0.0b7/bin/weewx/drivers/vantage.py
+-rw-r--r--   0        0        0    17795 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/wmr100.py
+-rw-r--r--   0        0        0    72747 2023-05-30 12:01:49.273499 weewx-5.0.0b7/bin/weewx/drivers/wmr300.py
+-rw-r--r--   0        0        0    29536 2023-06-22 18:50:24.465903 weewx-5.0.0b7/bin/weewx/drivers/wmr9x8.py
+-rw-r--r--   0        0        0    18843 2023-06-22 18:50:24.465903 weewx-5.0.0b7/bin/weewx/drivers/ws1.py
+-rw-r--r--   0        0        0    79489 2023-06-22 18:50:24.465903 weewx-5.0.0b7/bin/weewx/drivers/ws23xx.py
+-rw-r--r--   0        0        0   173578 2023-05-30 12:01:49.277499 weewx-5.0.0b7/bin/weewx/drivers/ws28xx.py
+-rw-r--r--   0        0        0    37475 2023-06-22 18:50:24.465903 weewx-5.0.0b7/bin/weewx/engine.py
+-rw-r--r--   0        0        0      276 2023-05-30 12:01:49.277499 weewx-5.0.0b7/bin/weewx/filegenerator.py
+-rw-r--r--   0        0        0    18278 2023-06-22 18:50:24.465903 weewx-5.0.0b7/bin/weewx/imagegenerator.py
+-rw-r--r--   0        0        0    73115 2023-06-30 19:01:08.594144 weewx-5.0.0b7/bin/weewx/manager.py
+-rw-r--r--   0        0        0     3187 2023-05-30 12:01:49.277499 weewx-5.0.0b7/bin/weewx/qc.py
+-rw-r--r--   0        0        0    37780 2023-06-22 18:50:24.469903 weewx-5.0.0b7/bin/weewx/reportengine.py
+-rw-r--r--   0        0        0    79730 2023-06-22 18:50:24.469903 weewx-5.0.0b7/bin/weewx/restx.py
+-rw-r--r--   0        0        0     7207 2023-05-30 12:01:49.277499 weewx-5.0.0b7/bin/weewx/station.py
+-rw-r--r--   0        0        0    31690 2023-06-22 18:50:24.469903 weewx-5.0.0b7/bin/weewx/tags.py
+-rw-r--r--   0        0        0    71594 2023-06-22 18:50:24.473903 weewx-5.0.0b7/bin/weewx/units.py
+-rw-r--r--   0        0        0    25248 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/uwxutils.py
+-rw-r--r--   0        0        0      246 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/wxengine.py
+-rw-r--r--   0        0        0    30034 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/wxformulas.py
+-rw-r--r--   0        0        0      367 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/wxmanager.py
+-rw-r--r--   0        0        0     7270 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/wxservices.py
+-rw-r--r--   0        0        0    34292 2023-05-30 12:01:49.281499 weewx-5.0.0b7/bin/weewx/wxxtypes.py
+-rw-r--r--   0        0        0    55988 2023-06-22 18:50:24.473903 weewx-5.0.0b7/bin/weewx/xtypes.py
+-rwxr-xr-x   0        0        0     9648 2023-06-22 18:50:24.473903 weewx-5.0.0b7/bin/weewxd.py
+-rw-r--r--   0        0        0    12175 2023-06-22 18:50:24.485903 weewx-5.0.0b7/pkg/changelog.el
+-rw-r--r--   0        0        0    12070 2023-06-22 18:50:24.485903 weewx-5.0.0b7/pkg/changelog.suse
+-rw-r--r--   0        0        0     2731 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/debian/README
+-rw-r--r--   0        0        0    21471 2023-06-22 18:50:24.485903 weewx-5.0.0b7/pkg/debian/changelog
+-rw-r--r--   0        0        0        3 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/compat
+-rw-r--r--   0        0        0       36 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/debian/conffiles
+-rwxr-xr-x   0        0        0     3398 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/config
+-rw-r--r--   0        0        0      724 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/control
+-rw-r--r--   0        0        0      926 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/copyright
+-rwxr-xr-x   0        0        0     8937 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/postinst
+-rwxr-xr-x   0        0        0      906 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/debian/postrm
+-rwxr-xr-x   0        0        0      410 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/debian/preinst
+-rwxr-xr-x   0        0        0      693 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/prerm
+-rwxr-xr-x   0        0        0     2985 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/rules
+-rw-r--r--   0        0        0       12 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/debian/source/format
+-rw-r--r--   0        0        0     5501 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/debian/templates
+-rw-r--r--   0        0        0     1708 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/index-apt.html
+-rw-r--r--   0        0        0     1728 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/index-suse.html
+-rw-r--r--   0        0        0     1714 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/index-yum.html
+-rwxr-xr-x   0        0        0     9874 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/mkchangelog.pl
+-rw-r--r--   0        0        0       79 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx-el8.repo
+-rw-r--r--   0        0        0       57 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx-python2.list
+-rw-r--r--   0        0        0       56 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx-python3.list
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx-suse12.repo
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx-suse15.repo
+-rw-r--r--   0        0        0     2201 2023-05-30 12:01:49.289499 weewx-5.0.0b7/pkg/weewx.smf
+-rw-r--r--   0        0        0     7144 2023-06-22 18:50:24.489903 weewx-5.0.0b7/pkg/weewx.spec.in
+-rw-r--r--   0        0        0     2829 2023-07-02 15:58:22.008000 weewx-5.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/apache/conf-available/weewx.conf
+-rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/apache/conf.d/weewx.conf
+-rw-r--r--   0        0        0      136 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/default/weewx
+-rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/i18n/i18n-report
+-rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/import/csv-example.conf
+-rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/import/cumulus-example.conf
+-rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/import/wd-example.conf
+-rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/import/weathercat-example.conf
+-rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/import/wu-example.conf
+-rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/logrotate.d/weewx
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/logwatch/conf/logfiles/weewx.conf
+-rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/logwatch/conf/services/weewx.conf
+-rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/logwatch/scripts/services/weewx
+-rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/newsyslog.d/weewx.conf
+-rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/rsyslog.d/weewx.conf
+-rwxr-xr-x   0        0        0      319 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/wee_database
+-rwxr-xr-x   0        0        0      316 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/wee_debug
+-rwxr-xr-x   0        0        0      317 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/wee_device
+-rwxr-xr-x   0        0        0      317 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/wee_import
+-rwxr-xr-x   0        0        0      318 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/wee_reports
+-rwxr-xr-x   0        0        0      313 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/weectl
+-rwxr-xr-x   0        0        0      313 2023-06-22 18:50:24.493903 weewx-5.0.0b7/util/scripts/weewxd
+-rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/solaris/weewx-smf.xml
+-rw-r--r--   0        0        0      526 2023-06-24 20:56:10.599627 weewx-5.0.0b7/util/systemd/weewx.service
+-rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/tmpfiles.d/weewx.conf
+-rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/acurite.rules
+-rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/cc3000.rules
+-rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/fousb.rules
+-rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/te923.rules
+-rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/vantage.rules
+-rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/weewx.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/wmr100.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/wmr300.rules
+-rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b7/util/udev/rules.d/ws28xx.rules
+-rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 weewx-5.0.0b7/PKG-INFO
```

### Comparing `weewx-5.0.0b6/LICENSE.txt` & `weewx-5.0.0b7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/README.md` & `weewx-5.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/schemas/wview.py` & `weewx-5.0.0b7/bin/schemas/wview.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/schemas/wview_extended.py` & `weewx-5.0.0b7/bin/schemas/wview_extended.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/schemas/wview_small.py` & `weewx-5.0.0b7/bin/schemas/wview_small.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_database.py` & `weewx-5.0.0b7/bin/wee_database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_debug.py` & `weewx-5.0.0b7/bin/wee_debug.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_device.py` & `weewx-5.0.0b7/bin/wee_device.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_import.py` & `weewx-5.0.0b7/bin/wee_import.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_reports.py` & `weewx-5.0.0b7/bin/wee_reports.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/bin/user/extensions.py` & `weewx-5.0.0b7/bin/wee_resources/bin/user/extensions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/404.html` & `weewx-5.0.0b7/bin/wee_resources/docs/404.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/images/favicon.png` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map` & `weewx-5.0.0b7/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/changes/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/changes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/copyright/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/copyright/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/css/tocbot-4.12.0.css` & `weewx-5.0.0b7/bin/wee_resources/docs/css/tocbot-4.12.0.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/css/tocbot-4.3.1.css` & `weewx-5.0.0b7/bin/wee_resources/docs/css/tocbot-4.3.1.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/css/weewx_ui.css` & `weewx-5.0.0b7/bin/wee_resources/docs/css/weewx_ui.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/appendix/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/appendix/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/cheetah/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/cheetah/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/custom-reports/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/custom-reports/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/database/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/derived/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/derived/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/drivers/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/drivers/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/extensions/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/extensions/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/image-generator/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/image-generator/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/localization/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/localization/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/multiple-bindings/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/multiple-bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/report-options/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/report-options/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/report-scheduling/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/report-scheduling/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/service-engine/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/service-engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/custom/units/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/custom/units/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/devnotes/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/devnotes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/examples/tag.htm` & `weewx-5.0.0b7/bin/wee_resources/docs/examples/tag.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/acurite/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/acurite/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/cc3000/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/cc3000/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/drivers/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/drivers/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/fousb/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/fousb/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/te923/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/te923/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/ultimeter/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/ultimeter/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/vantage/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/vantage/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr100/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr100/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr300/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr300/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/wmr9x8/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/wmr9x8/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws1/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws1/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws23xx/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws23xx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/hardware/ws28xx/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/hardware/ws28xx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/antialias.gif` & `weewx-5.0.0b7/bin/wee_resources/docs/images/antialias.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/day-gap-not-shown.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/day-gap-not-shown.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/day-gap-showing.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/day-gap-showing.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/daycompare.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/daycompare.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/daytemp_with_avg.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/daytemp_with_avg.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/dayvaporp.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/dayvaporp.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/daywindvec.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/daywindvec.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/favicon.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/ferrites.jpg` & `weewx-5.0.0b7/bin/wee_resources/docs/images/ferrites.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/funky_degree.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/funky_degree.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/image_parts.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/image_parts.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/image_parts.xcf` & `weewx-5.0.0b7/bin/wee_resources/docs/images/image_parts.xcf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-apple.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-apple.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-centos.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-centos.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-debian.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-debian.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-fedora.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-fedora.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-linux.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-linux.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-mint.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-mint.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-opensuse.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-opensuse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-pypi.svg` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-redhat.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-redhat.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-rpi.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-rpi.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-suse.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-suse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-ubuntu.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-ubuntu.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/logo-weewx.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/logo-weewx.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/pipeline.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/sample_monthrain.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/sample_monthrain.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/sample_monthtempdew.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/sample_monthtempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/weekgustoverlay.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/weekgustoverlay.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/weektempdew.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/weektempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/yeardiff.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/yeardiff.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/images/yearhilow.png` & `weewx-5.0.0b7/bin/wee_resources/docs/images/yearhilow.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/cash.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/cash.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/cash.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/cash.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.12.0.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.12.0.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.12.0.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.12.0.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/tocbot-4.3.1.min.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/tocbot-4.3.1.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/js/weewx.js` & `weewx-5.0.0b7/bin/wee_resources/docs/js/weewx.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/debian/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/debian/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/git/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/git/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/pip/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/pip/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/redhat/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/redhat/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/quickstarts/suse/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/quickstarts/suse/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/search/search_index.json` & `weewx-5.0.0b7/bin/wee_resources/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b7/bin/wee_resources/docs/sitemap.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/sitemap.xml.gz` & `weewx-5.0.0b7/bin/wee_resources/docs/sitemap.xml.gz`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/sle/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/sle/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/installing-weewx/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/installing-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/running-weewx/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/running-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/system-requirements/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/system-requirements/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/webserver-integration/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/webserver-integration/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/usersguide/where/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/usersguide/where/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_database/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_debug/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_debug/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_device/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_device/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_import/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_import/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/wee_reports/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/wee_reports/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/weectl-extension/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/weectl-extension/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/weectl-station/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/weectl-station/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/utilities/weewxd/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/utilities/weewxd/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/docs/versions/index.html` & `weewx-5.0.0b7/bin/wee_resources/docs/versions/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc` & `weewx-5.0.0b7/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/alarm.py` & `weewx-5.0.0b7/bin/wee_resources/examples/alarm.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/install.py` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/readme.md` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/basic.css` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/basic.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/current.inc` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/favicon.ico` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/hilo.inc` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/lang/en.conf` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/basic/skins/basic/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/examples/basic/skins/basic/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_1.py` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_2.py` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_2.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/colorize/colorize_3.py` & `weewx-5.0.0b7/bin/wee_resources/examples/colorize/colorize_3.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/fileparse/bin/user/fileparse.py` & `weewx-5.0.0b7/bin/wee_resources/examples/fileparse/bin/user/fileparse.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/fileparse/install.py` & `weewx-5.0.0b7/bin/wee_resources/examples/fileparse/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/fileparse/readme.md` & `weewx-5.0.0b7/bin/wee_resources/examples/fileparse/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/lowBattery.py` & `weewx-5.0.0b7/bin/wee_resources/examples/lowBattery.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/mem.py` & `weewx-5.0.0b7/bin/wee_resources/examples/mem.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/pmon/bin/user/pmon.py` & `weewx-5.0.0b7/bin/wee_resources/examples/pmon/bin/user/pmon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/pmon/install.py` & `weewx-5.0.0b7/bin/wee_resources/examples/pmon/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/pmon/readme.md` & `weewx-5.0.0b7/bin/wee_resources/examples/pmon/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/pmon/skins/pmon/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/examples/pmon/skins/pmon/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/tests/test_vaporpressure.py` & `weewx-5.0.0b7/bin/wee_resources/examples/tests/test_vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/vaporpressure.py` & `weewx-5.0.0b7/bin/wee_resources/examples/vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/bin/user/xstats.py` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/bin/user/xstats.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/install.py` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/readme.txt` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/readme.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/examples/xstats/skins/xstats/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/examples/xstats/skins/xstats/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Ftp/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Ftp/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/favicon.ico` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/de.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/en.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/nl.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/lang/no.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/mobile.css` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/mobile.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Mobile/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Mobile/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Rsync/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Rsync/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/about.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/about.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/analytics.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/analytics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/celestial.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/celestial.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/celestial.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/celestial.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/current.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/favicon.ico` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OFL.txt` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans.woff` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans.woff`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/OpenSans.woff2` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/OpenSans.woff2`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/font/license.txt` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/font/license.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/hilo.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/identifier.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/identifier.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/cn.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/cn.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/cz.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/cz.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/de.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/en.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/es.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/es.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/fr.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/gr.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/gr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/it.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/it.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/nl.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/no.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/lang/th.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/lang/th.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/map.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/map.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/radar.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/radar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/rss.xml.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/satellite.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/satellite.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/seasons.css` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/seasons.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/seasons.js` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/seasons.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/sensors.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/sensors.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/statistics.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/statistics.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/statistics.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/statistics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/sunmoon.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/sunmoon.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/tabular.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/tabular.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/telemetry.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/telemetry.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Seasons/titlebar.inc` & `weewx-5.0.0b7/bin/wee_resources/skins/Seasons/titlebar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/barometer.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/favicon.ico` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/humidity.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/de.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/en.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/nl.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/lang/no.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/rain.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/temp.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/temp.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Smartphone/wind.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/drops.gif` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/drops.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/flower.jpg` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/flower.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/backgrounds/night.gif` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/backgrounds/night.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/favicon.ico` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/de.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/en.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/fr.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/nl.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/lang/no.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/month.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/month.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/skin.conf` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/week.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/week.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/weewx.css` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/weewx.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/skins/Standard/year.html.tmpl` & `weewx-5.0.0b7/bin/wee_resources/skins/Standard/year.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx-multi` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.bsd` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.debian` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.freebsd` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.lsb` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.redhat` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/init.d/weewx.suse` & `weewx-5.0.0b7/bin/wee_resources/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b7/bin/wee_resources/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/util/systemd/weewx.service` & `weewx-5.0.0b7/bin/wee_resources/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/wee_resources/weewx.conf` & `weewx-5.0.0b7/bin/wee_resources/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weecfg/__init__.py` & `weewx-5.0.0b7/bin/weecfg/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weecfg/database.py` & `weewx-5.0.0b7/bin/weecfg/database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weecfg/extension.py` & `weewx-5.0.0b7/bin/weecfg/extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weecfg/station_config.py` & `weewx-5.0.0b7/bin/weecfg/station_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weecfg/update_config.py` & `weewx-5.0.0b7/bin/weecfg/update_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectl.py` & `weewx-5.0.0b7/bin/weectl.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectllib/__init__.py` & `weewx-5.0.0b7/bin/weectllib/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectllib/database_cmd.py` & `weewx-5.0.0b7/bin/weectllib/database_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectllib/db_actions.py` & `weewx-5.0.0b7/bin/weectllib/db_actions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectllib/extension_cmd.py` & `weewx-5.0.0b7/bin/weectllib/extension_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weectllib/station_cmd.py` & `weewx-5.0.0b7/bin/weectllib/station_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weedb/NOTES.md` & `weewx-5.0.0b7/bin/weedb/NOTES.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weedb/__init__.py` & `weewx-5.0.0b7/bin/weedb/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weedb/mysql.py` & `weewx-5.0.0b7/bin/weedb/mysql.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weedb/sqlite.py` & `weewx-5.0.0b7/bin/weedb/sqlite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/csvimport.py` & `weewx-5.0.0b7/bin/weeimport/csvimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/cumulusimport.py` & `weewx-5.0.0b7/bin/weeimport/cumulusimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/wdimport.py` & `weewx-5.0.0b7/bin/weeimport/wdimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/weathercatimport.py` & `weewx-5.0.0b7/bin/weeimport/weathercatimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/weeimport.py` & `weewx-5.0.0b7/bin/weeimport/weeimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeimport/wuimport.py` & `weewx-5.0.0b7/bin/weeimport/wuimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeplot/genplot.py` & `weewx-5.0.0b7/bin/weeplot/genplot.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeplot/utilities.py` & `weewx-5.0.0b7/bin/weeplot/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -573,17 +573,27 @@
         try:
             if fontpath_str.endswith('.ttf'):
                 # 1. Nice feature of Pillow: if fontpath_str is an absolute path, and it cannot be
                 #    found, then Pillow will search for the font in system resources as well.
                 # 2. Specifying the basic layout engine is necessary to avoid a segmentation
                 #    fault in Pillow versions earlier than 8.2.
                 #    See https://github.com/python-pillow/Pillow/issues/3066
-                font = ImageFont.truetype(fontpath_str,                         # See note 1 above
-                                          layout_engine=ImageFont.LAYOUT_BASIC, # See note 2 above
-                                          *args)
+                # 3. But, unfortunately, the means for specifying the Layout engine changed
+                #    with Pillow V9.1. The old way was deprecated in Pillow 10.0,
+                #    so if we want to support versions older than 9.1, we have to try it both ways
+                try:
+                    # First, try it the modern way (see note 3 above)
+                    font = ImageFont.truetype(fontpath_str,                         # See note 1
+                                              layout_engine=ImageFont.Layout.BASIC, # See note 2
+                                              *args)
+                except AttributeError:
+                    # That didn't work. Try it the old way (see note 3)
+                    font = ImageFont.truetype(fontpath_str,                         # See note 1
+                                              layout_engine=ImageFont.LAYOUT_BASIC, # See note 2
+                                              *args)
             else:
                 font = ImageFont.load_path(fontpath_str)
         except IOError:
             pass
 
     if font is None:
         font = ImageFont.load_default()
```

### Comparing `weewx-5.0.0b6/bin/weeutil/Moon.py` & `weewx-5.0.0b7/bin/weeutil/Moon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/Sun.py` & `weewx-5.0.0b7/bin/weeutil/Sun.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/config.py` & `weewx-5.0.0b7/bin/weeutil/config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/ftpupload.py` & `weewx-5.0.0b7/bin/weeutil/ftpupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/log.py` & `weewx-5.0.0b7/bin/weeutil/log.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/logger.py` & `weewx-5.0.0b7/bin/weeutil/logger.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/rsyncupload.py` & `weewx-5.0.0b7/bin/weeutil/rsyncupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/timediff.py` & `weewx-5.0.0b7/bin/weeutil/timediff.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weeutil/weeutil.py` & `weewx-5.0.0b7/bin/weeutil/weeutil.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/__init__.py` & `weewx-5.0.0b7/bin/weewx/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/accum.py` & `weewx-5.0.0b7/bin/weewx/accum.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/almanac.py` & `weewx-5.0.0b7/bin/weewx/almanac.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/cheetahgenerator.py` & `weewx-5.0.0b7/bin/weewx/cheetahgenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/crc16.py` & `weewx-5.0.0b7/bin/weewx/crc16.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/daemon.py` & `weewx-5.0.0b7/bin/weewx/daemon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/defaults.py` & `weewx-5.0.0b7/bin/weewx/defaults.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/__init__.py` & `weewx-5.0.0b7/bin/weewx/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/acurite.py` & `weewx-5.0.0b7/bin/weewx/drivers/acurite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/cc3000.py` & `weewx-5.0.0b7/bin/weewx/drivers/cc3000.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/fousb.py` & `weewx-5.0.0b7/bin/weewx/drivers/fousb.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/simulator.py` & `weewx-5.0.0b7/bin/weewx/drivers/simulator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/te923.py` & `weewx-5.0.0b7/bin/weewx/drivers/te923.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/ultimeter.py` & `weewx-5.0.0b7/bin/weewx/drivers/ultimeter.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/vantage.py` & `weewx-5.0.0b7/bin/weewx/drivers/vantage.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/wmr100.py` & `weewx-5.0.0b7/bin/weewx/drivers/wmr100.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/wmr300.py` & `weewx-5.0.0b7/bin/weewx/drivers/wmr300.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/wmr9x8.py` & `weewx-5.0.0b7/bin/weewx/drivers/wmr9x8.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/ws1.py` & `weewx-5.0.0b7/bin/weewx/drivers/ws1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/ws23xx.py` & `weewx-5.0.0b7/bin/weewx/drivers/ws23xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/drivers/ws28xx.py` & `weewx-5.0.0b7/bin/weewx/drivers/ws28xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/engine.py` & `weewx-5.0.0b7/bin/weewx/engine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/imagegenerator.py` & `weewx-5.0.0b7/bin/weewx/imagegenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/manager.py` & `weewx-5.0.0b7/bin/weewx/manager.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/qc.py` & `weewx-5.0.0b7/bin/weewx/qc.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/reportengine.py` & `weewx-5.0.0b7/bin/weewx/reportengine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/restx.py` & `weewx-5.0.0b7/bin/weewx/restx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/station.py` & `weewx-5.0.0b7/bin/weewx/station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/tags.py` & `weewx-5.0.0b7/bin/weewx/tags.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/units.py` & `weewx-5.0.0b7/bin/weewx/units.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/uwxutils.py` & `weewx-5.0.0b7/bin/weewx/uwxutils.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/wxformulas.py` & `weewx-5.0.0b7/bin/weewx/wxformulas.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/wxservices.py` & `weewx-5.0.0b7/bin/weewx/wxservices.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/wxxtypes.py` & `weewx-5.0.0b7/bin/weewx/wxxtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewx/xtypes.py` & `weewx-5.0.0b7/bin/weewx/xtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/bin/weewxd.py` & `weewx-5.0.0b7/bin/weewxd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/changelog.el` & `weewx-5.0.0b7/pkg/changelog.el`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/changelog.suse` & `weewx-5.0.0b7/pkg/changelog.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/README` & `weewx-5.0.0b7/pkg/debian/README`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/changelog` & `weewx-5.0.0b7/pkg/debian/changelog`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/config` & `weewx-5.0.0b7/pkg/debian/config`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/control` & `weewx-5.0.0b7/pkg/debian/control`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/copyright` & `weewx-5.0.0b7/pkg/debian/copyright`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/postinst` & `weewx-5.0.0b7/pkg/debian/postinst`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/postrm` & `weewx-5.0.0b7/pkg/debian/postrm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/prerm` & `weewx-5.0.0b7/pkg/debian/prerm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/rules` & `weewx-5.0.0b7/pkg/debian/rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/debian/templates` & `weewx-5.0.0b7/pkg/debian/templates`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/index-apt.html` & `weewx-5.0.0b7/pkg/index-apt.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/index-suse.html` & `weewx-5.0.0b7/pkg/index-suse.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/index-yum.html` & `weewx-5.0.0b7/pkg/index-yum.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/mkchangelog.pl` & `weewx-5.0.0b7/pkg/mkchangelog.pl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/weewx.smf` & `weewx-5.0.0b7/pkg/weewx.smf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pkg/weewx.spec.in` & `weewx-5.0.0b7/pkg/weewx.spec.in`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/pyproject.toml` & `weewx-5.0.0b7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "weewx"
-version = "5.0.0b6"
+version = "5.0.0b7"
 description = "The WeeWX weather software system. This is an BETA release, and may have many bugs!"
 authors = ["Tom Keffer <tkeffer@gmail.com>"]
 license = "GPL3"
 readme = 'README.md'
 repository = "https://github.com/weewx/weewx"
 homepage = "https://weewx.com"
 documentation = "https://weewx.com/docs"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Operating System :: POSIX :: Linux',
     'Operating System :: Unix',
+    'Operating System :: MacOS',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
```

### Comparing `weewx-5.0.0b6/util/i18n/i18n-report` & `weewx-5.0.0b7/util/i18n/i18n-report`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/import/csv-example.conf` & `weewx-5.0.0b7/util/import/csv-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/import/cumulus-example.conf` & `weewx-5.0.0b7/util/import/cumulus-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/import/wd-example.conf` & `weewx-5.0.0b7/util/import/wd-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/import/weathercat-example.conf` & `weewx-5.0.0b7/util/import/weathercat-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/import/wu-example.conf` & `weewx-5.0.0b7/util/import/wu-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx-multi` & `weewx-5.0.0b7/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.bsd` & `weewx-5.0.0b7/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.debian` & `weewx-5.0.0b7/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.freebsd` & `weewx-5.0.0b7/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.lsb` & `weewx-5.0.0b7/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.redhat` & `weewx-5.0.0b7/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/init.d/weewx.suse` & `weewx-5.0.0b7/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b7/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/logrotate.d/weewx` & `weewx-5.0.0b7/util/logrotate.d/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/logwatch/scripts/services/weewx` & `weewx-5.0.0b7/util/logwatch/scripts/services/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/rsyslog.d/weewx.conf` & `weewx-5.0.0b7/util/rsyslog.d/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/solaris/weewx-smf.xml` & `weewx-5.0.0b7/util/solaris/weewx-smf.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/systemd/weewx.service` & `weewx-5.0.0b7/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/udev/rules.d/vantage.rules` & `weewx-5.0.0b7/util/udev/rules.d/vantage.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/util/udev/rules.d/weewx.rules` & `weewx-5.0.0b7/util/udev/rules.d/weewx.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b6/PKG-INFO` & `weewx-5.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: weewx
-Version: 5.0.0b6
+Version: 5.0.0b7
 Summary: The WeeWX weather software system. This is an BETA release, and may have many bugs!
 Home-page: https://weewx.com
 License: GPL3
 Author: Tom Keffer
 Author-email: tkeffer@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

