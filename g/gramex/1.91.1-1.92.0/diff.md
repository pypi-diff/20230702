# Comparing `tmp/gramex-1.91.1.tar.gz` & `tmp/gramex-1.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.91.1.tar", last modified: Mon Jun 19 14:24:51 2023, max compression
+gzip compressed data, was "gramex-1.92.0.tar", last modified: Sun Jul  2 06:18:29 2023, max compression
```

## Comparing `gramex-1.91.1.tar` & `gramex-1.92.0.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:51.393066 gramex-1.91.1/
--rw-rw-rw-   0        0        0     1968 2023-06-17 00:40:29.000000 gramex-1.91.1/.gitignore
--rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.91.1/LICENSE
--rw-rw-rw-   0        0        0      641 2023-05-13 04:30:57.000000 gramex-1.91.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2956 2023-06-19 14:24:51.395075 gramex-1.91.1/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.91.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.053350 gramex-1.91.1/gramex/
--rw-rw-rw-   0        0        0    15366 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.91.1/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.108780 gramex-1.91.1/gramex/apps/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.91.1/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.113302 gramex-1.91.1/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.91.1/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.134590 gramex-1.91.1/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      226 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/admin2/.snyk
--rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.91.1/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12257 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.91.1/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0     5216 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/admin2/schedule.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.154911 gramex-1.91.1/gramex/apps/capture/
--rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12051 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0   142301 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.187959 gramex-1.91.1/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.91.1/gramex/apps/filemanager/.snyk
--rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.91.1/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.91.1/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.91.1/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.91.1/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:49.843956 gramex-1.91.1/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.226481 gramex-1.91.1/gramex/apps/init/default/
--rw-rw-rw-   0        0        0      578 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/.eslintrc.yml
--rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      756 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.91.1/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.91.1/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.229585 gramex-1.91.1/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/init/default/assets/README.template.md
--rw-rw-rw-   0        0        0     1756 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0      694 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.236136 gramex-1.91.1/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2608 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      352 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       80 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     3499 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.244651 gramex-1.91.1/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      378 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      244 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.253526 gramex-1.91.1/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      247 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      757 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.258884 gramex-1.91.1/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.91.1/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.316295 gramex-1.91.1/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.91.1/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.91.1/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.91.1/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.91.1/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.91.1/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.91.1/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.91.1/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.91.1/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.91.1/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      775 2023-06-19 13:55:51.000000 gramex-1.91.1/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.91.1/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.327225 gramex-1.91.1/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.91.1/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.91.1/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.331185 gramex-1.91.1/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.91.1/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.345742 gramex-1.91.1/gramex/apps/pynode/
--rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.91.1/gramex/apps/pynode/.snyk
--rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.91.1/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     2953 2023-06-19 13:55:55.000000 gramex-1.91.1/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.91.1/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.356295 gramex-1.91.1/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.91.1/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.91.1/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.388592 gramex-1.91.1/gramex/apps/ui/
--rw-rw-rw-   0        0        0     1019 2023-06-19 13:54:33.000000 gramex-1.91.1/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    13288 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.91.1/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.91.1/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0   607863 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      339 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.91.1/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.404421 gramex-1.91.1/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.569310 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.91.1/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.91.1/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.675403 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.91.1/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.735369 gramex-1.91.1/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.91.1/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.740419 gramex-1.91.1/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.756566 gramex-1.91.1/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.91.1/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.772125 gramex-1.91.1/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.91.1/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.91.1/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.91.1/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.91.1/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.790378 gramex-1.91.1/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.806162 gramex-1.91.1/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     5781 2023-06-19 13:56:49.000000 gramex-1.91.1/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.91.1/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.809520 gramex-1.91.1/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.815055 gramex-1.91.1/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.820052 gramex-1.91.1/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.825567 gramex-1.91.1/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.829782 gramex-1.91.1/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.833303 gramex-1.91.1/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.836793 gramex-1.91.1/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.838817 gramex-1.91.1/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.842395 gramex-1.91.1/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.844343 gramex-1.91.1/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.851872 gramex-1.91.1/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.853884 gramex-1.91.1/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.856228 gramex-1.91.1/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.859385 gramex-1.91.1/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1815 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.91.1/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.874921 gramex-1.91.1/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.91.1/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.91.1/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.91.1/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      277 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/apps.yaml
--rw-rw-rw-   0        0        0    56842 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/cache.py
--rw-rw-rw-   0        0        0    35221 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/config.py
--rw-rw-rw-   0        0        0    93430 2023-05-27 08:02:09.000000 gramex-1.91.1/gramex/data.py
--rw-rw-rw-   0        0        0     6408 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.91.1/gramex/favicon.ico
--rw-rw-rw-   0        0        0    15661 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/gramex.yaml
--rw-rw-rw-   0        0        0     6262 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/gramexfeatures.csv
--rw-rw-rw-   0        0        0    14390 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/gramexsize.csv
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.969903 gramex-1.91.1/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2483 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     3085 2023-06-19 14:23:48.000000 gramex-1.91.1/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0     3862 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17341 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    65366 2023-06-19 14:23:49.000000 gramex-1.91.1/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    15771 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     6643 2023-06-19 14:23:49.000000 gramex-1.91.1/gramex/handlers/chatgpthandler.py
--rw-rw-rw-   0        0        0     1477 2023-06-08 09:04:46.000000 gramex-1.91.1/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0     8904 2023-06-17 00:11:07.000000 gramex-1.91.1/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14924 2023-06-19 13:54:33.000000 gramex-1.91.1/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.91.1/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13125 2023-06-19 14:23:49.000000 gramex-1.91.1/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2023-06-08 09:04:46.000000 gramex-1.91.1/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6706 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0     6838 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/handlers/messagehandler.py
--rw-rw-rw-   0        0        0    16154 2023-06-02 05:59:12.000000 gramex-1.91.1/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2023-06-08 09:04:46.000000 gramex-1.91.1/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7193 2023-06-08 09:04:46.000000 gramex-1.91.1/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2023-06-08 09:04:46.000000 gramex-1.91.1/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     5145 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7882 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.91.1/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11338 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9434 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.91.1/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/http.py
--rw-rw-rw-   0        0        0    35069 2023-06-17 00:40:29.000000 gramex-1.91.1/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.91.1/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/migrate.py
--rw-rw-rw-   0        0        0    18629 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.989390 gramex-1.91.1/gramex/pptgen/
--rw-rw-rw-   0        0        0     9967 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18868 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.91.1/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.91.1/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.91.1/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26250 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.994847 gramex-1.91.1/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23438 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34432 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4278 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/pynode.py
--rw-rw-rw-   0        0        0     2979 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:51.019134 gramex-1.91.1/gramex/services/
--rw-rw-rw-   0        0        0    39443 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    11176 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3681 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3684 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2023-05-13 04:30:57.000000 gramex-1.91.1/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4521 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5822 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.91.1/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:51.036212 gramex-1.91.1/gramex/transforms/
--rw-rw-rw-   0        0        0      803 2023-06-19 14:23:49.000000 gramex-1.91.1/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.91.1/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3542 2023-06-19 13:54:33.000000 gramex-1.91.1/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32960 2023-06-19 14:23:49.000000 gramex-1.91.1/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10095 2023-06-08 09:27:24.000000 gramex-1.91.1/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.91.1/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:50.106795 gramex-1.91.1/gramex.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-06-19 14:24:46.000000 gramex-1.91.1/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12004 2023-06-19 14:24:49.000000 gramex-1.91.1/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 14:24:46.000000 gramex-1.91.1/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-19 14:24:46.000000 gramex-1.91.1/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      953 2023-06-19 14:24:46.000000 gramex-1.91.1/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 14:24:46.000000 gramex-1.91.1/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6171 2023-06-19 14:23:49.000000 gramex-1.91.1/pyproject.toml
--rw-rw-rw-   0        0        0      503 2023-06-19 14:24:51.424337 gramex-1.91.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 14:24:51.390538 gramex-1.91.1/tests/
--rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.91.1/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.91.1/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.91.1/tests/test_args.py
--rw-rw-rw-   0        0        0    39128 2023-06-19 14:23:49.000000 gramex-1.91.1/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.91.1/tests/test_cache.py
--rw-rw-rw-   0        0        0    15062 2023-05-13 04:30:57.000000 gramex-1.91.1/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.91.1/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    12571 2023-06-19 14:23:49.000000 gramex-1.91.1/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17857 2023-06-19 14:23:49.000000 gramex-1.91.1/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2023-05-13 04:30:57.000000 gramex-1.91.1/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-05-27 08:02:33.000000 gramex-1.91.1/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.91.1/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.91.1/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    19008 2023-06-19 14:23:49.000000 gramex-1.91.1/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2023-05-13 04:30:57.000000 gramex-1.91.1/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.91.1/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.91.1/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.91.1/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2023-05-13 04:30:57.000000 gramex-1.91.1/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.91.1/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.91.1/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.91.1/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.91.1/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.91.1/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.91.1/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.91.1/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.91.1/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.91.1/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.91.1/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.91.1/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.158016 gramex-1.92.0/
+-rw-rw-rw-   0        0        0     1968 2023-06-17 00:40:29.000000 gramex-1.92.0/.gitignore
+-rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.92.0/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-05-13 04:30:57.000000 gramex-1.92.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2956 2023-07-02 06:18:29.158016 gramex-1.92.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.92.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.067998 gramex-1.92.0/gramex/
+-rw-rw-rw-   0        0        0    15366 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.92.0/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.116576 gramex-1.92.0/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.92.0/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.120596 gramex-1.92.0/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.92.0/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.136304 gramex-1.92.0/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      226 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/.snyk
+-rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.92.0/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12257 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.92.0/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0     5216 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/schedule.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.153805 gramex-1.92.0/gramex/apps/capture/
+-rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12051 2023-06-25 01:52:25.000000 gramex-1.92.0/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0   142301 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.177013 gramex-1.92.0/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.92.0/gramex/apps/filemanager/.snyk
+-rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:27.910952 gramex-1.92.0/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.207254 gramex-1.92.0/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0      578 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/.eslintrc.yml
+-rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/.flake8
+-rw-rw-rw-   0        0        0      756 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.92.0/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.92.0/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.209444 gramex-1.92.0/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/assets/README.template.md
+-rw-rw-rw-   0        0        0     1756 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0      694 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.212767 gramex-1.92.0/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2608 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      352 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       80 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     3499 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.222248 gramex-1.92.0/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      378 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      244 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.226244 gramex-1.92.0/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      247 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      757 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.235256 gramex-1.92.0/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.92.0/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.288576 gramex-1.92.0/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.92.0/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13287 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.92.0/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.92.0/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      775 2023-07-02 04:13:13.000000 gramex-1.92.0/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.92.0/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.293578 gramex-1.92.0/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.92.0/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.92.0/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.296572 gramex-1.92.0/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.92.0/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.311128 gramex-1.92.0/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/pynode/.snyk
+-rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.92.0/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     2953 2023-07-02 04:13:17.000000 gramex-1.92.0/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.92.0/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.317128 gramex-1.92.0/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.92.0/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.92.0/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.341135 gramex-1.92.0/gramex/apps/ui/
+-rw-rw-rw-   0        0        0      667 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    13165 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.92.0/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.92.0/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0   163730 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      265 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.92.0/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.362659 gramex-1.92.0/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.471892 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.552981 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.92.0/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.686688 gramex-1.92.0/gramex/apps/uifactory/
+-rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/uifactory/.eslintrc.js
+-rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/.gitattributes
+-rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.688688 gramex-1.92.0/gramex/apps/uifactory/assets/
+-rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/assets/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.690688 gramex-1.92.0/gramex/apps/uifactory/assets/data/
+-rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/apps/uifactory/assets/data/input.json
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.704039 gramex-1.92.0/gramex/apps/uifactory/assets/img/
+-rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/arrows-move.svg
+-rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/clipboard.svg
+-rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
+-rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/trash.svg
+-rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/create.html
+-rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/edit.html
+-rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/field-actions.html
+-rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.92.0/gramex/apps/uifactory/form_builder.py
+-rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/gramex.yaml
+-rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/index.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.730191 gramex-1.92.0/gramex/apps/uifactory/js/
+-rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/README.md
+-rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/embed.js
+-rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/fields.js
+-rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/fork-form.js
+-rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/index.js
+-rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/script.js
+-rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/utils.js
+-rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/viewform.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.751263 gramex-1.92.0/gramex/apps/uifactory/modals/
+-rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/add-field.html
+-rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/embed.html
+-rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/remove.html
+-rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/rename.html
+-rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/themes.html
+-rw-rw-rw-   0        0        0     5781 2023-07-02 04:14:00.000000 gramex-1.92.0/gramex/apps/uifactory/package-lock.json
+-rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.92.0/gramex/apps/uifactory/package.json
+-rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/popover-form.html
+-rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/sample.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.766205 gramex-1.92.0/gramex/apps/uifactory/snippets/
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.768989 gramex-1.92.0/gramex/apps/uifactory/snippets/button/
+-rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/button/bs4-button.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.772555 gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/
+-rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.775554 gramex-1.92.0/gramex/apps/uifactory/snippets/email/
+-rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/email/bs4-email.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.781701 gramex-1.92.0/gramex/apps/uifactory/snippets/hidden/
+-rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.785738 gramex-1.92.0/gramex/apps/uifactory/snippets/html/
+-rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/html/bs4-html.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.788725 gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/
+-rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.790873 gramex-1.92.0/gramex/apps/uifactory/snippets/number/
+-rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/number/bs4-number.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.796521 gramex-1.92.0/gramex/apps/uifactory/snippets/password/
+-rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/password/bs4-password.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.800032 gramex-1.92.0/gramex/apps/uifactory/snippets/radio/
+-rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.802042 gramex-1.92.0/gramex/apps/uifactory/snippets/range/
+-rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/range/bs4-range.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.805032 gramex-1.92.0/gramex/apps/uifactory/snippets/select/
+-rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/select/bs4-select.js
+-rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/setup.js
+-rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/snippets.json
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.808040 gramex-1.92.0/gramex/apps/uifactory/snippets/text/
+-rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/text/bs4-text.js
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.812032 gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/
+-rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
+-rw-rw-rw-   0        0        0     1815 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/uifactory/style.scss
+-rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/template-navbar-view-form.html
+-rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/template-navbar.html
+-rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/toast.html
+-rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/viewform.html
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.823142 gramex-1.92.0/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.92.0/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.92.0/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.92.0/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      277 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    58478 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/cache.py
+-rw-rw-rw-   0        0        0    35221 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/config.py
+-rw-rw-rw-   0        0        0    93430 2023-05-27 08:02:09.000000 gramex-1.92.0/gramex/data.py
+-rw-rw-rw-   0        0        0     6408 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.92.0/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    15621 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/gramex.yaml
+-rw-rw-rw-   0        0        0     6262 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/gramexfeatures.csv
+-rw-rw-rw-   0        0        0    14340 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/gramexsize.csv
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.951295 gramex-1.92.0/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2483 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     3085 2023-06-19 14:23:48.000000 gramex-1.92.0/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0     3862 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17347 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    65374 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    15771 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     6643 2023-07-02 04:09:20.000000 gramex-1.92.0/gramex/handlers/chatgpthandler.py
+-rw-rw-rw-   0        0        0     1477 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0     8904 2023-06-17 00:11:07.000000 gramex-1.92.0/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14917 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.92.0/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13125 2023-06-19 14:23:49.000000 gramex-1.92.0/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6706 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0     6838 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/messagehandler.py
+-rw-rw-rw-   0        0        0    16154 2023-06-02 05:59:12.000000 gramex-1.92.0/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7326 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     5145 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7882 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11338 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9434 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.92.0/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/http.py
+-rw-rw-rw-   0        0        0    35069 2023-06-17 00:40:29.000000 gramex-1.92.0/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18629 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.969316 gramex-1.92.0/gramex/pptgen/
+-rw-rw-rw-   0        0        0     9967 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18868 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.92.0/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.92.0/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26250 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.978185 gramex-1.92.0/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23438 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34432 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4278 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2979 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.000893 gramex-1.92.0/gramex/services/
+-rw-rw-rw-   0        0        0    39783 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    11451 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3724 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3684 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4521 2023-06-27 08:54:47.000000 gramex-1.92.0/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5822 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.018509 gramex-1.92.0/gramex/transforms/
+-rw-rw-rw-   0        0        0      787 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3022 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32960 2023-06-19 14:23:49.000000 gramex-1.92.0/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10095 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.92.0/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.114595 gramex-1.92.0/gramex.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12004 2023-07-02 06:18:27.000000 gramex-1.92.0/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      953 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6171 2023-07-02 06:16:31.000000 gramex-1.92.0/pyproject.toml
+-rw-rw-rw-   0        0        0      503 2023-07-02 06:18:29.178968 gramex-1.92.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.156018 gramex-1.92.0/tests/
+-rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.92.0/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_args.py
+-rw-rw-rw-   0        0        0    39128 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15062 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.92.0/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    12571 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17308 2023-07-02 06:16:31.000000 gramex-1.92.0/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-05-27 08:02:33.000000 gramex-1.92.0/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.92.0/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.92.0/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    19008 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.92.0/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.92.0/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.92.0/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.92.0/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.92.0/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.92.0/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.92.0/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.92.0/tests/test_websockethandler.py
```

### Comparing `gramex-1.91.1/.gitignore` & `gramex-1.92.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/LICENSE` & `gramex-1.92.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/MANIFEST.in` & `gramex-1.92.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/PKG-INFO` & `gramex-1.92.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.91.1
+Version: 1.92.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.91.1/README.md` & `gramex-1.92.0/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/__init__.py` & `gramex-1.92.0/gramex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 gramex install                Install an app
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
 '''
 
-__version__ = '1.91.1'
+__version__ = '1.92.0'
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
 paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
```

### Comparing `gramex-1.91.1/gramex/apps/admin2/gramex.yaml` & `gramex-1.92.0/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/admin2/gramexadmin.py` & `gramex-1.92.0/gramex/apps/admin2/gramexadmin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/admin2/index.html` & `gramex-1.92.0/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/admin2/schedule.js` & `gramex-1.92.0/gramex/apps/admin2/schedule.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/capture/README.md` & `gramex-1.92.0/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/capture/capture.js` & `gramex-1.92.0/gramex/apps/capture/capture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/capture/chromecapture.js` & `gramex-1.92.0/gramex/apps/capture/chromecapture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/capture/index.html` & `gramex-1.92.0/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/capture/package-lock.json` & `gramex-1.92.0/gramex/apps/capture/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998337438423645%*

 * *Differences: {"'dependencies'": "{'@types/node': {'version': '20.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/node/-/node-20.3.3.tgz', 'integrity': "*

 * *                   "'sha512-wheIYdr4NYML61AjC8MKj/2jrR/kDQri/CIpVoZwldwhnIrD/j9jIU5bJ8yBKuB2VhpFV7Ab6G2XkBjv9r9Zzw=='}}",*

 * * "'packages'": "{'node_modules/@types/node': {'version': '20.3.3', 'resolved': "*

 * *               "'https://registry.npmjs.org/@types/node/-/node-20.3.3.tgz', 'integrity': "*

 * *               "'sha512-wheIYdr4NYML61AjC8MKj/2jrR/ […]*

```diff
@@ -50,18 +50,18 @@
                 "unbzip2-stream": "1.4.3",
                 "yargs": "17.7.1"
             },
             "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.5.0.tgz",
             "version": "0.5.0"
         },
         "@types/node": {
-            "integrity": "sha512-EhcH/wvidPy1WeML3TtYFGR83UzjxeWRen9V402T8aUGYsCHOmfoisV3ZSg03gAFIbLq8TnWOJ0f4cALtnSEUg==",
+            "integrity": "sha512-wheIYdr4NYML61AjC8MKj/2jrR/kDQri/CIpVoZwldwhnIrD/j9jIU5bJ8yBKuB2VhpFV7Ab6G2XkBjv9r9Zzw==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.1.tgz",
-            "version": "20.3.1"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.3.tgz",
+            "version": "20.3.3"
         },
         "@types/yauzl": {
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
             "requires": {
                 "@types/node": "*"
             },
@@ -1632,18 +1632,18 @@
         },
         "node_modules/@puppeteer/browsers/node_modules/ms": {
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-EhcH/wvidPy1WeML3TtYFGR83UzjxeWRen9V402T8aUGYsCHOmfoisV3ZSg03gAFIbLq8TnWOJ0f4cALtnSEUg==",
+            "integrity": "sha512-wheIYdr4NYML61AjC8MKj/2jrR/kDQri/CIpVoZwldwhnIrD/j9jIU5bJ8yBKuB2VhpFV7Ab6G2XkBjv9r9Zzw==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.1.tgz",
-            "version": "20.3.1"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.3.tgz",
+            "version": "20.3.3"
         },
         "node_modules/@types/yauzl": {
             "dependencies": {
                 "@types/node": "*"
             },
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
```

### Comparing `gramex-1.91.1/gramex/apps/capture/package.json` & `gramex-1.92.0/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/README.html` & `gramex-1.92.0/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.92.0/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.92.0/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/filemanager.html` & `gramex-1.92.0/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/filemanager.js` & `gramex-1.92.0/gramex/apps/filemanager/filemanager.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/filemanager.py` & `gramex-1.92.0/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/gramex.yaml` & `gramex-1.92.0/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/index.html` & `gramex-1.92.0/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/filemanager/navbar.html` & `gramex-1.92.0/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/.eslintrc.yml` & `gramex-1.92.0/gramex/apps/init/default/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/.gitlab-ci.yml` & `gramex-1.92.0/gramex/apps/init/default/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/.template.gitignore` & `gramex-1.92.0/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/assets/README.template.md` & `gramex-1.92.0/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.92.0/gramex/apps/init/default/gramex.template.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/index.template.html` & `gramex-1.92.0/gramex/apps/init/default/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/js/README.template.md` & `gramex-1.92.0/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/login.template.html` & `gramex-1.92.0/gramex/apps/init/default/login.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.92.0/gramex/apps/init/default/template-navbar.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/ide/index.template.html` & `gramex-1.92.0/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/init/minimal/index.template.html` & `gramex-1.92.0/gramex/apps/init/minimal/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/languagetool/README.md` & `gramex-1.92.0/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/languagetool/gramex.yaml` & `gramex-1.92.0/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/config.yaml` & `gramex-1.92.0/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/gramex.yaml` & `gramex-1.92.0/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/index.html` & `gramex-1.92.0/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/logviewer.py` & `gramex-1.92.0/gramex/apps/logviewer/logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.92.0/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/package-lock.json` & `gramex-1.92.0/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/render.js` & `gramex-1.92.0/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/logviewer/script.js` & `gramex-1.92.0/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/mail/index.html` & `gramex-1.92.0/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/mlhandler/template.html` & `gramex-1.92.0/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/pynode/index.js` & `gramex-1.92.0/gramex/apps/pynode/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/pynode/package-lock.json` & `gramex-1.92.0/gramex/apps/pynode/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/.snyk` & `gramex-1.92.0/gramex/apps/ui/.snyk`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,14 @@
   # get-google-fonts impacts only the installation of comicgen. No runtime impact.
   SNYK-JS-REQUEST-3361831:
     - '*':
         reason: No fix. Await get-google-fonts upgrade
         expires: 2030-01-01T00:00:00.000Z
         created: 2021-07-24T00:00:00.000Z
 
-  # @vue/cli-service has vulnerabilities that only affects projects using Vue. Known risk.
-  # Since this only impacts developer-controlled code, it's acceptable
-  SNYK-JS-ANSIREGEX-1583908:
-    - '*':
-        reason: No fix available. Await @vue/cli-service upgrade
-        expires: 2022-06-30T00:00:00.000Z
-        created: 2021-10-01T00:00:00.000Z
-
   # We need D3 v4 for old projects. Just retain this forever -- but newer projects won't use this
   SNYK-JS-D3COLOR-1076592:
     - '*':
         reason: Retained for backward compatibility for old projects
         expires: 2030-01-01T00:00:00.000Z
         created: 2021-07-24T00:00:00.000Z
```

### Comparing `gramex-1.91.1/gramex/apps/ui/__init__.py` & `gramex-1.92.0/gramex/apps/ui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''Main UI application'''
 import io
 import re
 import os
 import gramex
 import gramex.cache
 import gramex.handlers
-import string
 
 # B404:import_subprocess only for JS compilation
 import subprocess  # nosec B404
 from hashlib import md5
 from tornado.gen import coroutine, Return
 from functools import partial
 from gramex.config import variables, app_log, merge
@@ -20,19 +19,27 @@
     return os.path.normpath(os.path.join(*args))
 
 
 ui_dir = os.path.dirname(os.path.abspath(__file__))
 config_file = _join(ui_dir, 'config.yaml')
 cache_dir = _join(variables['GRAMEXDATA'], 'apps', 'ui')
 sass_bin = _join(ui_dir, 'node_modules', 'sass', 'sass.js')
-ts_path = _join(ui_dir, 'node_modules', 'esbuild', 'bin', 'esbuild')
-vue_path = _join(ui_dir, 'node_modules', '@vue', 'cli-service', 'bin', 'vue-cli-service')
 if not os.path.exists(cache_dir):
     os.makedirs(cache_dir)
 
+esbuild_path = _join(ui_dir, 'node_modules', 'esbuild', 'bin', 'esbuild')
+# if esbuild is a shell script, run the base script
+esbuild_cmd = [esbuild_path]
+try:
+    with open(esbuild_path, 'rb') as handle:
+        if handle.read(2) == b'#!':
+            esbuild_cmd = ['node', esbuild_path]
+except OSError:
+    pass
+
 
 def cdn_redirect(handler, folder_map={}):
     '''Redirect /ui/... to cdn.jsdelivr.net/npm/...
 
     Before Gramex 1.84, specific npm libraries were included in Gramex. Now, we encourage projects
     to specify their own npm dependencies. This redirection makes apps backward compatible.
 
@@ -223,83 +230,83 @@
 
 
 @coroutine
 def jscompiler(
     handler: gramex.handlers.FileHandler,
     path: str,
     target_ext: str,
-    exe: str,
     cmd: str,
     options: dict = {},
 ) -> bytes:
-    '''Compile a file (Vue, TypeScript), etc into a JS file using Node.js
+    '''Compile a file (e.g. TypeScript) into a JS file using Node.js
 
     Examples:
         >>> jscompiler(
         ...     handler, path='x.ts', target_ext='.js', exe='/path/to/esbuild',
-        ...     cmd='node $exe $filename --outDir $targetDir --sourceMap')
+        ...     cmd=lambda filename, target_dir, options: ...)
 
     Parameters:
         handler: the[FileHandler][gramex.handlers.FileHandler] serving this file
         path: absolute path of input file to compile into JavaScript
         target_ext: extension of output file (e.g. `.js`, `.min.js`)
-        exe: path to the compiler's JS executable (e.g. `/path/to/esbuild`)
         cmd: command line to run. This substitutes 3 variables:
             - `$exe` for the `exe` parameter
             - `$filename` for the absolute path to the input file
             - `$targetDir` for the absolute path to the output directory
 
     Returns:
         compiled JS file or source map if ?_map is specified
     '''
     # Get valid variables from URL query parameters
     # Create cache key based on state = path. Output to <cache-key>.js
     path = os.path.normpath(path).replace('\\', '/')
     ext = os.path.splitext(path)[-1]
-    options = ' '.join(f'--{key}={handler.get_arg(key, val)}' for key, val in options.items())
-    cache_key = _get_cache_key([path, options])
+    options = [f'--{key}={handler.get_arg(key, val)}' for key, val in options.items()]
+    cache_key = _get_cache_key([path] + options)
     target_dir = _join(cache_dir, f'{ext}-{cache_key}')
     target = os.path.join(target_dir, os.path.basename(path[: -len(ext)] + target_ext))
 
     # Recompile if output target is missing, or path has been updated
     if not os.path.exists(target) or os.stat(path).st_mtime > os.stat(target).st_mtime:
         cwd, filename = os.path.split(path)
-        subs = {'exe': exe, 'filename': filename, 'targetDir': target_dir}
-        cmd = [string.Template(x).substitute(subs) for x in cmd.format(OPTIONS=options).split()]
-        app_log.debug(f'Compiling .{ext}: {" ".join(cmd)}')
+        cmd_to_run = cmd(filename=filename, target_dir=target_dir, options=options)
+        app_log.debug(f'Compiling {ext}: {cmd_to_run}')
         proc = yield gramex.service.threadpool.submit(
-            subprocess.run, cmd, cwd=cwd, capture_output=True, encoding='utf-8'
+            subprocess.run,
+            cmd_to_run,
+            cwd=cwd,
+            capture_output=True,
+            encoding='utf-8',
         )
         if proc.returncode:
             raise RuntimeError(f'.{ext} compilation failure:\n{proc.stderr}\n{proc.stdout}')
 
     return _sourcemap(handler, target, 'text/javascript')
 
 
 ts = partial(
     jscompiler,
     target_ext='.js',
-    exe=ts_path,
     options={
         'format': 'iife',
         'bundle': 'true',
         'minify': 'true',
         'target': 'esnext',
         'charset': 'utf8',
         'global-name': '',
         'keep-names': 'false',
     },
-    cmd='node $exe {OPTIONS} --allow-overwrite --sourcemap --outdir=$targetDir $filename',
-)
-vue = partial(
-    jscompiler,
-    target_ext='.min.js',
-    exe=vue_path,
-    options={'target': 'wc'},
-    cmd='node --unhandled-rejections=strict $exe build {OPTIONS} $filename --dest $targetDir',
+    cmd=lambda options, filename, target_dir: [
+        *esbuild_cmd,
+        *options,
+        '--allow-overwrite',
+        '--sourcemap',
+        f'--outdir={target_dir}',
+        filename,
+    ],
 )
 
 
 def _sourcemap(handler: gramex.handlers.FileHandler, target: str, mime: str) -> bytes:
     '''Returns the compiled target file OR the source map if ?_map is set.
 
     Examples:
@@ -309,15 +316,15 @@
         handler: the [FileHandler][gramex.handlers.FileHandler] serving this file
         target: absolute path of compiled output
         mime: MIME type of compiled output
 
     Returns:
         source map or target file contents
 
-    This is used by FileHandlers compiling Vue, TS, SASS, etc.
+    This is used by FileHandlers compiling TS, SASS, etc.
 
     If the URL has a ?_map, it serves `{target}.map` as a JSON file.
     Else it serves the `{target}` as `mime` type,
     replacing `sourceMappingURL` with the current URL + `?_map`.
     '''
     if '_map' in handler.args:
         # Serve JSON source map if requested
```

### Comparing `gramex-1.91.1/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.92.0/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/config.yaml` & `gramex-1.92.0/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/gramex.yaml` & `gramex-1.92.0/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/gramexui.scss` & `gramex-1.92.0/gramex/apps/ui/gramexui.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/setup.js` & `gramex-1.92.0/gramex/apps/ui/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.92.0/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/default.png` & `gramex-1.92.0/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/index.html` & `gramex-1.92.0/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/sample.html` & `gramex-1.92.0/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/ui/theme/themes.json` & `gramex-1.92.0/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/.eslintrc.js` & `gramex-1.92.0/gramex/apps/uifactory/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/assets/data/input.json` & `gramex-1.92.0/gramex/apps/uifactory/assets/data/input.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/assets/img/arrows-move.svg` & `gramex-1.92.0/gramex/apps/uifactory/assets/img/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png` & `gramex-1.92.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/assets/img/trash.svg` & `gramex-1.92.0/gramex/apps/uifactory/assets/img/trash.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/create.html` & `gramex-1.92.0/gramex/apps/uifactory/create.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/edit.html` & `gramex-1.92.0/gramex/apps/uifactory/edit.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/field-actions.html` & `gramex-1.92.0/gramex/apps/uifactory/field-actions.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/form_builder.py` & `gramex-1.92.0/gramex/apps/uifactory/form_builder.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/gramex.yaml` & `gramex-1.92.0/gramex/apps/uifactory/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/index.html` & `gramex-1.92.0/gramex/apps/uifactory/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/README.md` & `gramex-1.92.0/gramex/apps/uifactory/js/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/fields.js` & `gramex-1.92.0/gramex/apps/uifactory/js/fields.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/fork-form.js` & `gramex-1.92.0/gramex/apps/uifactory/js/fork-form.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/index.js` & `gramex-1.92.0/gramex/apps/uifactory/js/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/script.js` & `gramex-1.92.0/gramex/apps/uifactory/js/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/utils.js` & `gramex-1.92.0/gramex/apps/uifactory/js/utils.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/js/viewform.js` & `gramex-1.92.0/gramex/apps/uifactory/js/viewform.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/modals/add-field.html` & `gramex-1.92.0/gramex/apps/uifactory/modals/add-field.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/modals/embed.html` & `gramex-1.92.0/gramex/apps/uifactory/modals/embed.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/modals/remove.html` & `gramex-1.92.0/gramex/apps/uifactory/modals/remove.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/modals/rename.html` & `gramex-1.92.0/gramex/apps/uifactory/modals/rename.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/modals/themes.html` & `gramex-1.92.0/gramex/apps/uifactory/modals/themes.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/package-lock.json` & `gramex-1.92.0/gramex/apps/uifactory/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/popover-form.html` & `gramex-1.92.0/gramex/apps/uifactory/popover-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/sample.html` & `gramex-1.92.0/gramex/apps/uifactory/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/button/bs4-button.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/button/bs4-button.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/email/bs4-email.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/email/bs4-email.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/number/bs4-number.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/number/bs4-number.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/range/bs4-range.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/range/bs4-range.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/select/bs4-select.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/select/bs4-select.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/setup.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/text/bs4-text.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/text/bs4-text.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js` & `gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/style.scss` & `gramex-1.92.0/gramex/apps/uifactory/style.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/template-navbar-view-form.html` & `gramex-1.92.0/gramex/apps/uifactory/template-navbar-view-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/template-navbar.html` & `gramex-1.92.0/gramex/apps/uifactory/template-navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/uifactory/viewform.html` & `gramex-1.92.0/gramex/apps/uifactory/viewform.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/update/README.md` & `gramex-1.92.0/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/update/gramex.yaml` & `gramex-1.92.0/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/update/gramexupdate.py` & `gramex-1.92.0/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/apps/update/index.html` & `gramex-1.92.0/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/cache.py` & `gramex-1.92.0/gramex/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 
 def read_excel(
     io: Union[str, BinaryIO],
     sheet_name: Union[str, int] = 0,
     table: str = None,
     name: str = None,
     range: str = None,
+    links: Union[Dict[str, str], bool] = None,
     header: Union[None, int, List[int]] = ...,
     **kwargs: dict,
 ) -> pd.DataFrame:
     '''Read data from an XLSX as a DataFrame using `openpyxl`.
 
     Examples:
         >>> gramex.cache.read_excel('data.xlsx', sheet_name='Sheet1')
@@ -236,23 +237,26 @@
         sheet_name: sheet to load data from. Sheet names are specified as strings.
             Integers pick zero-indexed sheet position. default: 0
         table: Worksheet table to load from sheet, e.g. `'Table1'`
         name: Defined name to load from sheet, e.g. `'MyNamedRange'`
         range: Cell range to load from sheet, e.g. `'A1:C10'`
         header: Row (0-indexed) to use for the column labels. A list of integers is combined into
             a MultiIndex. Use None if there is no header.
+        links: optional dictionary to extract hyperlinks from column names into a new column, e.g.
+            `{'issue': 'issue_link'}` extracts the URL from the `issue` column into `issue_link`.
+            Set to True to extract all available hyperlinks into a new column `{col}_link`.
         **kwargs: If neither `table`, nor `name`, nor `range` is specified, loads entire
             sheet via `pd.read_excel`, passing the remaining kwargs.
 
     Returns:
         The loaded DataFrame
 
     Note: `table` takes priority over `name` takes priority over `range`.
     '''
-    if not any((range, name, table)):
+    if not any((range, name, table, links)):
         # Pandas defaults to xlrd, but we prefer openpyxl
         kwargs.setdefault('engine', 'openpyxl')
         return pd.read_excel(
             io, sheet_name=sheet_name, header=0 if header is ... else header, **kwargs
         )
 
     import openpyxl
@@ -275,33 +279,61 @@
         # Raise an error if we can't find it
         if defined_name is None:
             raise ValueError(f'{io}: missing name {name} in sheet {sheet_name}')
         # Note: This only works if it's a cell range. If we create a named range inside a table,
         # Excel may store this as =Table[[#All],[Col1]:[Col5]], which isn't a valid range.
         # Currently, we ignore that, and assumed that the name is like Sheet1!A1:C10
         range = defined_name.attr_text.split('!')[-1]
+    elif not range:
+        range = ws.dimensions
 
-    vals = ws[range]
-    if isinstance(vals, tuple):
-        data = pd.DataFrame([[cell.value for cell in row] for row in vals])
-    else:
-        data = pd.DataFrame([[vals.value]])
+    # If range is a single cell, ws[range] returns the value. cells ensures it's a 2D tuple
+    cells = ws[range] if isinstance(ws[range], tuple) else ((ws[range],),)
+    data = pd.DataFrame([[cell.value for cell in row] for row in cells])
     # Header defaults to 0 if undefined. If it's not None, apply the header
     header = 0 if header is ... else header
     if header is not None:
-        data = (
-            data.T.set_index(header)
-            .T.reset_index(  # Set header rows as column names
-                drop=True
-            )  # Drop index with "holes" where headers were
-            .rename_axis(  # Column name has header index (e.g. 0). Drop it
-                [None] * len(header) if isinstance(header, (list, tuple)) else None, axis=1
+        # Set header rows as column names
+        data = data.T.set_index(header).T
+        # The index will now have numbers 0 .. n SKIPPING for headers. Fix that
+        data = data.reset_index(drop=True)
+        # Column name has header index (e.g. 0). Drop it
+        cols = [None] * len(header) if isinstance(header, (list, tuple)) else None
+        data = data.rename_axis(cols, axis=1)
+    # Convert data types
+    data = data.infer_objects()
+    # Add link columns
+    header_set = set(header) if isinstance(header, (list, tuple)) else {header}
+    if isinstance(links, dict):
+        for col_name, col_link in (links or {}).items():
+            if col_name not in data.columns:
+                app_log.warning('gramex.cache.open: column %s not found in %s', col_name, io)
+                continue
+            col = data.columns.get_loc(col_name)
+            data[col_link] = [
+                getattr(row[col].hyperlink, 'target', None)
+                for i, row in enumerate(cells)
+                if i not in header_set
+            ]
+    elif links is True:
+        for col_name in data.columns:
+            col = data.columns.get_loc(col_name)
+            col_link = (
+                tuple(f'{c}_link' for c in data.columns[col])
+                if isinstance(header, (list, tuple)) and len(header) > 1
+                else f'{col_name}_link'
             )
-        )
-    return data.infer_objects()  # Convert data types
+            links = [
+                getattr(row[col].hyperlink, 'target', None)
+                for i, row in enumerate(cells)
+                if i not in header_set
+            ]
+            if any(links):
+                data[col_link] = links
+    return data
 
 
 def save(
     data: pd.DataFrame,
     url: str,
     rel: bool = False,
     callback: Union[str, Callable] = None,
```

### Comparing `gramex-1.91.1/gramex/config.py` & `gramex-1.92.0/gramex/config.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/data.py` & `gramex-1.92.0/gramex/data.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/debug.py` & `gramex-1.92.0/gramex/debug.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/deploy.yaml` & `gramex-1.92.0/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/download.vega.js` & `gramex-1.92.0/gramex/download.vega.js`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/favicon.ico` & `gramex-1.92.0/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/gramex.yaml` & `gramex-1.92.0/gramex/gramex.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,14 @@
       default_filename: # Choose default file for a directory from
         - default.template.html #   Template files, else
         - default.tmpl.html
         - index.html #   HTML file, else
       index: true # Display directory indices
       sass: ["*.scss", "*.sass"] # Handle SASS files
       ts: ["*.ts"] # Handle TypeScript files
-      vue: ["*.vue"] # Handle Vue files
       template: # Handle template files
         - "*.template.html"
         - "*.tmpl.html"
       headers:
         Cache-Control: max-age=60 # By default, cache for a minute
         # Standard libraries won't ever change. Cache for 10 years
         "node_modules/**":
```

### Comparing `gramex-1.91.1/gramex/gramexfeatures.csv` & `gramex-1.92.0/gramex/gramexfeatures.csv`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/gramexsize.csv` & `gramex-1.92.0/gramex/gramexsize.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 codepath,yamlpath,complexity
 gramex.cache._delete_temp_files,*,3
 gramex.cache.open,*,13
-gramex.cache.*,cache,49
+gramex.cache.*,cache,55
 gramex.cache.save,url.*.handler=FormHandler|FilterHandler|MLHandler|DriverHandler,4
 gramex.cache.query,url.*.handler=FormHandler|FilterHandler|MLHandler|DriverHandler,9
 gramex.cache.stat,*,2
 gramex.cache.reload_module,*,5
 gramex.cache.urlfetch,alert,6
 gramex.cache.Subprocess.*,url.*.handler=ProcessHandler|Process,25
 gramex.cache.daemon,url.*.handler=ComicHandler|Comic,24
@@ -49,15 +49,15 @@
 gramex.transformers.*,url.*.handler=MLHandler|ML,31
 gramex.winservice.*,TODO - if app is deployed on Windows server,22
 gramex.__init__.*,*,49
 gramex.apps.admin2.*,import.*.path=$GRAMEXAPPS/admin2/gramex.yaml,53
 gramex.apps.filemanager.*,import.*.path=$GRAMEXAPPS/filemanager/gramex.yaml,7
 gramex.apps.logviewer.*,import.*.path=$GRAMEXAPPS/logviewer/gramex.yaml,61
 gramex.apps.mail.*,import.*.path=$GRAMEXAPPS/mail/gramex.yaml,2
-gramex.apps.ui.*,import.*.path=$GRAMEXAPPS/ui/gramex.yaml,28
+gramex.apps.ui.*,import.*.path=$GRAMEXAPPS/ui/gramex.yaml,32
 gramex.apps.uifactory.*,import.*.path=$GRAMEXAPPS/uifactory/gramex.yaml,21
 gramex.apps.update.*,import.*.path=$GRAMEXAPPS/update/gramex.yaml,14
 gramex.handlers.authhandler.AuthHandler.*,url.*.handler=GoogleAuth|SimpleAuth|OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,35
 gramex.handlers.authhandler.LogoutHandler.*,url.*.handler=LogoutHandler,4
 gramex.handlers.authhandler.GoogleAuth.*,url.*.handler=GoogleAuth,5
 gramex.handlers.authhandler.SimpleAuth.*,url.*.handler=SimpleAuth,5
 gramex.handlers.basehandler.BaseMixin.setup,url,2
@@ -139,16 +139,16 @@
 gramex.handlers.socialhandler.TwitterRESTHandler.*,url.*.handler=TwitterRESTHandler|Twitter,8
 gramex.handlers.socialhandler.FacebookGraphHandler.*,url.*.handler=FacebookGraphHandler|Facebook,6
 gramex.handlers.uploadhandler.*,url.*.handler=UploadHandler|Upload,44
 gramex.handlers.websockethandler.*,url.*.handler=WebSocketHandler|Websocket,7
 gramex.handlers.__init__.*,url.*.handler=OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,7
 gramex.pptgen.*,url.*.handler=PPTXHandler,363
 gramex.pptgen2.*,url.*.handler=PPTXHandler,244
-gramex.services.emailer.*,email,34
-gramex.services.rediscache.*,cache.*.type=redis,23
+gramex.services.emailer.*,email,35
+gramex.services.rediscache.*,cache.*.type=redis,24
 gramex.services.scheduler.*,schedule,26
 gramex.services.sms.*,sms,10
 gramex.services.ttlcache.*,cache.*.type=memory,46
 gramex.services.urlcache.get_cachefile,cache,4
 gramex.services.urlcache.CacheFile.*,cache,3
 gramex.services.urlcache.MemoryCacheFile.*,cache.*.type=memory,4
 gramex.services.urlcache.MemoryCacheFile.*,cache.*.type=disk,4
@@ -159,15 +159,15 @@
 gramex.services.__init__.app,app,21
 gramex.services.__init__.schedule,schedule,5
 gramex.services.__init__.alert,alert,7
 gramex.services.__init__.threadpool,threadpool,2
 gramex.services.__init__.url,url,16
 gramex.services.__init__.mime,mime,2
 gramex.services.__init__.watch,watch,9
-gramex.services.__init__.cache,cache,10
+gramex.services.__init__.cache,cache,13
 gramex.services.__init__.eventlog,eventlog,6
 gramex.services.__init__.email,email,3
 gramex.services.__init__.sms,sms,6
 gramex.services.__init__.handlers,handlers,1
 gramex.services.__init__.encrypt,encrypt,1
 gramex.services.__init__.test,test,1
 gramex.services.__init__.gramexlog,gramexlog,11
@@ -184,15 +184,14 @@
 gramex.services.__init__._url_normalize,url.*.pattern,2
 gramex.services.__init__._get_cache_key,url.*.cache,10
 gramex.services.__init__._cache_generator,url.*.cache,5
 gramex.transforms.auth.ensure_single_session,url.*.handlers.kwargs.action.function:ensure_single_session,7
 gramex.transforms.template.template,url.*.kwargs.template,4
 gramex.transforms.template.scss,url.*.kwargs.scss,1
 gramex.transforms.template.ts,url.*.kwargs.ts,1
-gramex.transforms.template.vue,url.*.kwargs.vue,1
 gramex.transforms.template.CacheLoader.*,url.*.kwargs.template,3
 gramex.transforms.transforms.identity,TODO - if any PY code uses @handler,1
 gramex.transforms.transforms._arg_repr,TODO - same as build_transform (maybe always),4
 gramex.transforms.transforms._full_name,TODO - same as build_transform (maybe always),3
 gramex.transforms.transforms.module_names,TODO - same as build_transform (maybe always),11
 gramex.transforms.transforms.build_transform,TODO - same as build_transform (maybe always),15
 gramex.transforms.transforms.build_pipeline,TODO - same as build_transform (maybe always),15
```

### Comparing `gramex-1.91.1/gramex/handlers/400.html` & `gramex-1.92.0/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/401.html` & `gramex-1.92.0/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/403.html` & `gramex-1.92.0/gramex/handlers/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/404.html` & `gramex-1.92.0/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/500.html` & `gramex-1.92.0/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/__init__.py` & `gramex-1.92.0/gramex/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.92.0/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/auth.template.html` & `gramex-1.92.0/gramex/handlers/auth.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/authhandler.py` & `gramex-1.92.0/gramex/handlers/authhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         # If session_inactive: is specified, set expiry date on the session
         if self.session_inactive is not None:
             self.session['_i'] = self.session_inactive * 24 * 60 * 60
 
         # Apply rules to the user
         for _, rule in self.rules.iterrows():
-            if fnmatch(user.get(rule['selector'], ''), rule['pattern']):
+            if fnmatch(user.get(rule['selector'], '') or '', rule['pattern']):
                 user[rule['field']] = rule['value']
 
         # Run post-login events (e.g. ensure_single_session) specified in config
         for callback in self.actions:
             callback(self)
         self.log_user_event(event='login')
```

### Comparing `gramex-1.91.1/gramex/handlers/basehandler.py` & `gramex-1.92.0/gramex/handlers/basehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,15 +986,15 @@
         # Skip expired tokens
         if row['expire'] <= time.time():
             return None
         # Return the user column parsed as JSON.
         # Add custom keys from the table to the user object.
         row['user'] = json.loads(row['user'])
         custom_keys = [key for key in row if key not in {'user', 'token', 'expire'}]
-        if isinstance(row, dict):
+        if isinstance(row['user'], dict):
             row['user'].update({key: row[key] for key in custom_keys})
         else:
             app_log.warning('Cannot add custom keys to non-dict "user" in: %r', row)
         return row
 
     def revoke_otp(self, key: str) -> Union[str, dict, None]:
         '''Revoke an OTP. Returns the user object from [gramex.handlers.BaseMixin.get_otp][].'''
```

### Comparing `gramex-1.91.1/gramex/handlers/capturehandler.py` & `gramex-1.92.0/gramex/handlers/capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/chatgpthandler.py` & `gramex-1.92.0/gramex/handlers/chatgpthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/comichandler.py` & `gramex-1.92.0/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/drivehandler.py` & `gramex-1.92.0/gramex/handlers/drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/filehandler.py` & `gramex-1.92.0/gramex/handlers/filehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         - `root`: Root path for this handler. Aligns with the `path` argument
         - `path`; Absolute path requested by the user, without adding a default filename
         - `file`: Absolute path served to the user, after adding a default filename
         '''
         # Convert template: '*.html' into transform: {'*.html': {function: template}}
         # Convert sass: ['*.scss', '*.sass'] into transform: {'*.scss': {function: sass}}
         # Do this before BaseHandler setup so that it can invoke the transforms required
-        for key in ('template', 'sass', 'scss', 'ts', 'vue'):
+        for key in ('template', 'sass', 'scss', 'ts'):
             val = kwargs.pop(key, None)
             if val:
                 # template/sass/...: true is the same as template: '*'
                 val = '*' if val is True else val if isinstance(val, (list, tuple)) else [val]
                 kwargs.setdefault('transform', AttrDict()).update(
                     {v: AttrDict(function=key) for v in val}
                 )
```

### Comparing `gramex-1.91.1/gramex/handlers/filehandler.template.html` & `gramex-1.92.0/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/formhandler.py` & `gramex-1.92.0/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/functionhandler.py` & `gramex-1.92.0/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/jsonhandler.py` & `gramex-1.92.0/gramex/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/messagehandler.py` & `gramex-1.92.0/gramex/handlers/messagehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/mlhandler.py` & `gramex-1.92.0/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/modelhandler.py` & `gramex-1.92.0/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/openapiconfig.yaml` & `gramex-1.92.0/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/openapihandler.py` & `gramex-1.92.0/gramex/handlers/openapihandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from copy import deepcopy
 from typing import get_type_hints
 from textwrap import dedent
 from gramex.config import merge
 from gramex.transforms.transforms import typelist, Header
 from gramex.handlers import BaseHandler
 
-config = gramex.cache.open('openapiconfig.yaml', 'config', rel=True)
+config = gramex.cache.open('openapiconfig.yaml', rel=True)
 
 
 def url_name(pattern):
     # Spec name is the last URL path that has alphabets
     names = [part for part in pattern.split('/') if any(c.isalnum() for c in part)]
     # Capitalize. url-like_this becomes "Url Like This"
     names = [word.capitalize() for word in re.split(r'[\s\-_]', ' '.join(names))]
@@ -57,15 +57,15 @@
             # JSON Schema uses {type: array, items: {type: integer}} for array of ints.
             # But a simple int is {type: integer}
             if is_list:
                 conf['schema']['type'] = 'array'
                 conf['schema']['items'] = {'type': cls.types.get(typ, 'string')}
             else:
                 conf['schema']['type'] = cls.types.get(typ, 'string')
-        spec['responses'] = deepcopy(config.responses)
+        spec['responses'] = deepcopy(config['responses'])
         return spec
 
     def formhandler_spec(self, cls, summary):
         spec = {}
         datasets = getattr(cls, 'datasets', {})
         get_spec = spec['get'] = {
             'summary': summary,
@@ -90,30 +90,34 @@
             # For every column, add
             #   ?_c=<col>
             #   ?_sort=<col> and ?_sort=-<col>
             #   ?<col>=
             cols, sorts = [], []
             for col in dataset.get('columns', []):
                 if isinstance(col, dict):
-                    add(config.formhandler.col, name=col['name'], schema={'type': col['type']})
+                    add(
+                        config['formhandler']['col'],
+                        name=col['name'],
+                        schema={'type': col['type']},
+                    )
                     cols.append(col['name'])
                     sorts.append(col['name'])
                     sorts.append('-' + col['name'])
                 else:
-                    add(config.formhandler.col, name=col)
+                    add(config['formhandler']['col'], name=col)
                     cols.append(col)
                     sorts.append(col)
                     sorts.append('-' + col)
-            add(config.formhandler._sort, schema={'items': {'enum': sorts}})
-            add(config.formhandler._c, schema={'items': {'enum': cols}})
-            add(config.formhandler._offset)
-            add(config.formhandler._limit)
-            add(config.formhandler._meta)
+            add(config['formhandler']['_sort'], schema={'items': {'enum': sorts}})
+            add(config['formhandler']['_c'], schema={'items': {'enum': cols}})
+            add(config['formhandler']['_offset'])
+            add(config['formhandler']['_limit'])
+            add(config['formhandler']['_meta'])
         # TODO: If ID is present, allow GET, POST, DELETE. Else only GET
-        get_spec['responses'] = deepcopy(config.responses)
+        get_spec['responses'] = deepcopy(config['responses'])
         return spec
 
     def get(self):
         kwargs = self.conf.get('kwargs', {})
         # TODO: Set header only if not already set in the configuration.
         # This can be handled in gramex/gramex.yaml as a default configuration.
         # Switch to YAML if a YAML spec is requested
```

### Comparing `gramex-1.91.1/gramex/handlers/pptxhandler.py` & `gramex-1.92.0/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/processhandler.py` & `gramex-1.92.0/gramex/handlers/processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/proxyhandler.py` & `gramex-1.92.0/gramex/handlers/proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/queryhandler.template.html` & `gramex-1.92.0/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/socialhandler.py` & `gramex-1.92.0/gramex/handlers/socialhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/uploadhandler.py` & `gramex-1.92.0/gramex/handlers/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/handlers/websockethandler.py` & `gramex-1.92.0/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/http.py` & `gramex-1.92.0/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/install.py` & `gramex-1.92.0/gramex/install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/license.py` & `gramex-1.92.0/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/migrate.py` & `gramex-1.92.0/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/ml.py` & `gramex-1.92.0/gramex/ml.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/ml_api.py` & `gramex-1.92.0/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/__init__.py` & `gramex-1.92.0/gramex/pptgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/color.py` & `gramex-1.92.0/gramex/pptgen/color.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/colors.json` & `gramex-1.92.0/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/commands.py` & `gramex-1.92.0/gramex/pptgen/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/fonts.json` & `gramex-1.92.0/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/fontwidth.py` & `gramex-1.92.0/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen/utils.py` & `gramex-1.92.0/gramex/pptgen/utils.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen2/__init__.py` & `gramex-1.92.0/gramex/pptgen2/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen2/commands.py` & `gramex-1.92.0/gramex/pptgen2/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pptgen2/config.yaml` & `gramex-1.92.0/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/pynode.py` & `gramex-1.92.0/gramex/pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/scale.py` & `gramex-1.92.0/gramex/scale.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/secrets.py` & `gramex-1.92.0/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/servicenow.yaml` & `gramex-1.92.0/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/services/__init__.py` & `gramex-1.92.0/gramex/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,17 +396,23 @@
                 info.cache[name] = urlcache.RedisCache(path=path, maxsize=config['size'])
             except Exception:
                 app_log.exception(f'cache:{name} cannot connect to redis')
         # if default: true, make this the default cache for gramex.cache.{open,query}
         if config.get('default'):
             for key in ['_OPEN_CACHE', '_QUERY_CACHE']:
                 old_cache = getattr(gramex.cache, key, {})
-                info.cache[name].update(old_cache)
-                setattr(gramex.cache, key, info.cache[name])
+                # Migrate cache and clear it
+                for k in old_cache.keys():
+                    try:
+                        info.cache[name].set(k, old_cache.get(k, None))
+                    except Exception:
+                        # Don't f-string the `k` into the message. It might contain a %s
+                        app_log.exception(f"cache:{name} can't migrate %r", k)
                 old_cache.clear()
+                setattr(gramex.cache, key, info.cache[name])
 
 
 def eventlog(conf: dict) -> None:
     '''Set up the application event logger'''
     if not conf.path:
         return
```

### Comparing `gramex-1.91.1/gramex/services/emailer.py` & `gramex-1.92.0/gramex/services/emailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,21 @@
 
         - a string with comma-separated emails, e.g. `'a@x.com, b@x.com'`
         - a list of strings with emails, e.g. `['a@x.com', 'b@x.com']`
         - a list of strings with comma-separated emails, e.g. `['a@x.com', 'b@x.com, c@x.com']`
         '''
         sender = kwargs.get('sender', self.email)
         # SES allows restricting the From: address. https://amzn.to/2Kqwh2y
+        # SES uses an IAM ID for login (self.email), but restricts sender -- so from= is required
         # Mailgun suggests From: be the same as Sender: http://bit.ly/2tGS5wt
-        kwargs.setdefault('from', sender)
+        # If mail(from=) is specified, use that as the sender. Else use email: from the service
+        if kwargs.get('from', None):
+            sender = kwargs['from']
+        else:
+            kwargs['from'] = sender
         # Identify recipients from to/cc/bcc fields.
         # Note: We MUST explicitly add EVERY recipient (to/cc/bcc) in sendmail(recipients=)
         to = recipients(**kwargs)
         msg = message(**kwargs)
         tls = self.client.get('tls', True)
         # Test cases specify stub: true. This uses a stub that logs emails
         if self.stub:
```

### Comparing `gramex-1.91.1/gramex/services/rediscache.py` & `gramex-1.92.0/gramex/services/rediscache.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,7 +95,10 @@
 
     def keys(self):
         return self.store.keys()
 
     def flush(self):
         '''Delete all keys in the current database'''
         self.store.execute_command('FLUSHDB')
+
+    def clear(self):
+        self.flush()
```

### Comparing `gramex-1.91.1/gramex/services/scheduler.py` & `gramex-1.92.0/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/services/sms.py` & `gramex-1.92.0/gramex/services/sms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/services/ttlcache.py` & `gramex-1.92.0/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/services/urlcache.py` & `gramex-1.92.0/gramex/services/urlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/services/watcher.py` & `gramex-1.92.0/gramex/services/watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/sm_api.py` & `gramex-1.92.0/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/topcause.py` & `gramex-1.92.0/gramex/topcause.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/transformers.py` & `gramex-1.92.0/gramex/transformers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/transforms/__init__.py` & `gramex-1.92.0/gramex/transforms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Utility functions for actions or conversions'''
 
 from .auth import ensure_single_session
-from .template import template, sass, scss, ts, vue
+from .template import template, sass, scss, ts
 from .transforms import build_transform, build_pipeline, build_log_info, condition, flattener, once
 from .transforms import handler, handler_expr, time_key, Header
 
 # Import common libraries with their popular abbreviations.
 # This lets build_transform() to use, for e.g., `pd.concat()` instead of `pandas.concat()`.
 import pandas as pd
 import numpy as np
@@ -14,15 +14,14 @@
     'build_transform',
     'build_pipeline',
     'build_log_info',
     'template',
     'sass',
     'scss',
     'ts',
-    'vue',
     'ensure_single_session',
     'condition',
     'flattener',
     'once',
     'handler',
     'handler_expr',
     'time_key',
```

### Comparing `gramex-1.91.1/gramex/transforms/auth.py` & `gramex-1.92.0/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/transforms/template.py` & `gramex-1.92.0/gramex/transforms/template.py`

 * *Files 15% similar despite different names*

```diff
@@ -76,35 +76,14 @@
     from gramex.apps.ui import ts
 
     # Ignore the content provided. ts needs the file actually located at handler.path.
     result = yield ts(handler, handler.path)
     return result.decode('utf-8')
 
 
-@tornado.gen.coroutine
-def vue(content, handler):
-    '''Renders a Vue file as JS web component via @vue/cli in a FileHandler.
-
-    This can be used as a keyword argument to FileHandler:
-
-    ```yaml
-    pattern: /file.vue
-    handler: FileHandler
-    kwargs:
-        ...
-        template: '*.vue'
-    ```
-    '''
-    from gramex.apps.ui import vue
-
-    # Ignore the content provided. vue needs the file actually located at handler.path.
-    result = yield vue(handler, handler.path)
-    return result.decode('utf-8')
-
-
 class CacheLoader(tornado.template.Loader):
     # Like tornado.template.Loader, but caching only until underlying file is changed.
     # Used internally by BaseHandler to override the Tornado default template loader.
 
     def load(self, name, parent_path=None):
         # Always load the file. _create_template takes care of the caching
         name = self.resolve_path(name, parent_path=parent_path)
```

### Comparing `gramex-1.91.1/gramex/transforms/transforms.py` & `gramex-1.92.0/gramex/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/transforms/twitterstream.py` & `gramex-1.92.0/gramex/transforms/twitterstream.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex/winservice.py` & `gramex-1.92.0/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex.egg-info/PKG-INFO` & `gramex-1.92.0/gramex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.91.1
+Version: 1.92.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.91.1/gramex.egg-info/SOURCES.txt` & `gramex-1.92.0/gramex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/gramex.egg-info/requires.txt` & `gramex-1.92.0/gramex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/pyproject.toml` & `gramex-1.92.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.91.1"
+version = "1.92.0"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
```

### Comparing `gramex-1.91.1/tests/test_admin.py` & `gramex-1.92.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_alerts.py` & `gramex-1.92.0/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_args.py` & `gramex-1.92.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_auth.py` & `gramex-1.92.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_cache.py` & `gramex-1.92.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_capturehandler.py` & `gramex-1.92.0/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_comichandler.py` & `gramex-1.92.0/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_drivehandler.py` & `gramex-1.92.0/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_filehandler.py` & `gramex-1.92.0/tests/test_filehandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,26 +187,14 @@
                 ok_('--alpha: purple' in text, f'{dir}.{file}: import gramexui with vars')
                 self.check_sourcemap(url, text)
         self.check('/dir/transform-sass/a.scss?primary=blue', text='.ui-import-a{color:blue}')
         self.check('/dir/transform-sass/b.scss?primary=blue', text='.ui-import-b{color:blue}')
         # TODO: Invalid file should generate a compilation failure
         # TODO: Changing file should recompile
 
-    def test_vue(self):
-        for dir in ('/dir/transform-vue', '/dir/vue-file'):
-            for name in ('a', 'b'):
-                url = f'{dir}/comp-{name}.vue'
-                text = self.check(
-                    url, timeout=30, headers={'Content-Type': 'text/javascript'}
-                ).text
-                ok_(f'Component: {name}' in text, f'{url}: has component name')
-                self.check_sourcemap(url, text)
-        # TODO: Invalid file should generate a compilation failure
-        # TODO: Changing file should recompile
-
     def test_ts(self):
         for dir in ('/dir/transform-ts', '/dir/ts-file'):
             for name in ('a', 'b'):
                 url = f'{dir}/{name}.ts?minify=false&bundle=true'
                 text = self.check(
                     url, timeout=30, headers={'Content-Type': 'text/javascript'}
                 ).text
```

### Comparing `gramex-1.91.1/tests/test_filterhandler.py` & `gramex-1.92.0/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_formhandler.py` & `gramex-1.92.0/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_functionhandler.py` & `gramex-1.92.0/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_gramexlog.py` & `gramex-1.92.0/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_handlers.py` & `gramex-1.92.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_init.py` & `gramex-1.92.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_install.py` & `gramex-1.92.0/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_jsonhandler.py` & `gramex-1.92.0/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_ldapauth.py` & `gramex-1.92.0/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_logviewer.py` & `gramex-1.92.0/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_mlhandler.py` & `gramex-1.92.0/tests/test_mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_modelhandler.py` & `gramex-1.92.0/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_openapihandler.py` & `gramex-1.92.0/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_pptxhandler.py` & `gramex-1.92.0/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_processhandler.py` & `gramex-1.92.0/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_proxyhandler.py` & `gramex-1.92.0/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_pynode.py` & `gramex-1.92.0/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_schedule.py` & `gramex-1.92.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_secrets.py` & `gramex-1.92.0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_subprocess.py` & `gramex-1.92.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_translater.py` & `gramex-1.92.0/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_twitterresthandler.py` & `gramex-1.92.0/tests/test_twitterresthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_ui.py` & `gramex-1.92.0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_update.py` & `gramex-1.92.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_uploadhandler.py` & `gramex-1.92.0/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_watcher.py` & `gramex-1.92.0/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.91.1/tests/test_websockethandler.py` & `gramex-1.92.0/tests/test_websockethandler.py`

 * *Files identical despite different names*

