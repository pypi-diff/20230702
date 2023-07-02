# Comparing `tmp/not1mm-23.6.30.1.tar.gz` & `tmp/not1mm-23.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.6.30.1.tar", last modified: Sat Jul  1 04:43:38 2023, max compression
+gzip compressed data, was "not1mm-23.7.2.tar", last modified: Sun Jul  2 16:56:03 2023, max compression
```

## Comparing `not1mm-23.6.30.1.tar` & `not1mm-23.7.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.30.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23264 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22516 2023-07-01 04:16:01.000000 not1mm-23.6.30.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.747132 not1mm-23.6.30.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94445 2023-07-01 04:11:44.000000 not1mm-23.6.30.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26505 2023-06-28 22:11:02.000000 not1mm-23.6.30.1/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.781133 not1mm-23.6.30.1/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.30.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.6.30.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.30.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.30.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.30.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.30.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.30.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.30.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.6.30.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.30.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.6.30.1/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.30.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.30.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.30.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.30.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.30.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.6.30.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18069 2023-06-30 21:41:06.000000 not1mm-23.6.30.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.6.30.1/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.30.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.865134 not1mm-23.6.30.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.30.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.30.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.30.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.30.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.30.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.30.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.30.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.30.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.30.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.30.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.30.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.30.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.30.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.30.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.30.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.30.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.30.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.30.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.30.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.30.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.30.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.30.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.30.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.30.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.30.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.30.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.30.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.30.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.30.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.30.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.30.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.30.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.30.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.30.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.30.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.30.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.30.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.30.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.30.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.30.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.30.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.30.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.30.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.30.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.30.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.30.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.30.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.30.1/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.871134 not1mm-23.6.30.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.30.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.30.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.30.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.30.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35883 2023-06-28 19:43:33.000000 not1mm-23.6.30.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.30.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.30.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.30.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.30.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.30.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.30.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.30.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.30.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.30.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.30.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.30.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-07-01 04:42:28.000000 not1mm-23.6.30.1/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.30.1/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.30.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.878134 not1mm-23.6.30.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.30.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.30.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.30.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14705 2023-07-01 04:39:54.000000 not1mm-23.6.30.1/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.30.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.30.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.30.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.30.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.30.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.30.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.30.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.30.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.30.1/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.879134 not1mm-23.6.30.1/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.30.1/not1mm/testing/fakeflrig.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.30.1/not1mm/testing/flrigclient.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.6.30.1/not1mm/testing/multicast_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.6.30.1/not1mm/testing/n1mm_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.30.1/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.755133 not1mm-23.6.30.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23264 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3647 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-07-01 04:43:38.000000 not1mm-23.6.30.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1274 2023-07-01 04:42:11.000000 not1mm-23.6.30.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-07-01 04:43:38.881134 not1mm-23.6.30.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-01 04:43:38.880134 not1mm-23.6.30.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.6.30.1/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.134659 not1mm-23.7.2/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.7.2/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22723 2023-07-02 16:56:03.133659 not1mm-23.7.2/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21978 2023-07-02 16:54:30.000000 not1mm-23.7.2/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:02.909656 not1mm-23.7.2/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.7.2/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94308 2023-07-02 16:45:33.000000 not1mm-23.7.2/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26459 2023-07-02 16:26:27.000000 not1mm-23.7.2/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:02.984657 not1mm-23.7.2/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.7.2/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.7.2/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.7.2/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.7.2/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.7.2/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.7.2/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.7.2/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.7.2/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.7.2/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.7.2/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.7.2/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.7.2/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.7.2/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.7.2/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.7.2/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.7.2/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.7.2/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.7.2/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.7.2/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.7.2/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18069 2023-06-30 21:41:06.000000 not1mm-23.7.2/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.7.2/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.7.2/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.097659 not1mm-23.7.2/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.7.2/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.7.2/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.7.2/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.7.2/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.7.2/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.7.2/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.7.2/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.7.2/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.7.2/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.7.2/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.7.2/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.7.2/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.7.2/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.7.2/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.7.2/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.7.2/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.7.2/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.7.2/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.7.2/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.7.2/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.7.2/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.7.2/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.7.2/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.7.2/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.7.2/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.7.2/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.7.2/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.7.2/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.7.2/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.7.2/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.7.2/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.7.2/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.7.2/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.7.2/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.7.2/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.7.2/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.7.2/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.7.2/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.7.2/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.7.2/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.7.2/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.7.2/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.7.2/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.7.2/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.7.2/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.7.2/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.7.2/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.7.2/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.7.2/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.7.2/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.7.2/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.7.2/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.117659 not1mm-23.7.2/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.7.2/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.7.2/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.7.2/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.7.2/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35883 2023-06-28 19:43:33.000000 not1mm-23.7.2/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.7.2/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.7.2/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.7.2/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.7.2/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.7.2/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.7.2/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.7.2/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.7.2/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.7.2/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.7.2/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.7.2/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-07-02 16:46:47.000000 not1mm-23.7.2/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.7.2/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.7.2/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.131659 not1mm-23.7.2/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.7.2/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.7.2/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.7.2/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.7.2/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.7.2/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.7.2/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.7.2/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.7.2/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.7.2/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.7.2/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.7.2/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14705 2023-07-01 04:39:54.000000 not1mm-23.7.2/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.7.2/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.7.2/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.7.2/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.7.2/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.7.2/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.7.2/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.7.2/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.7.2/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.7.2/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.133659 not1mm-23.7.2/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.7.2/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.7.2/not1mm/testing/flrigclient.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.7.2/not1mm/testing/multicast_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.7.2/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.7.2/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:02.918657 not1mm-23.7.2/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22723 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3647 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-07-02 16:56:02.000000 not1mm-23.7.2/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-07-02 16:47:32.000000 not1mm-23.7.2/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-07-02 16:56:03.134659 not1mm-23.7.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-07-02 16:56:03.133659 not1mm-23.7.2/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.7.2/testing/test.py
```

### Comparing `not1mm-23.6.30.1/LICENSE` & `not1mm-23.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/PKG-INFO` & `not1mm-23.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.30.1
+Version: 23.7.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -74,15 +74,15 @@
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
-    - [Bandmap](#bandmap)
+  - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -132,24 +132,17 @@
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 - RAC Canada Day
 
 ## Recent Changes
 
-- [23-6-30] Added RAC Canada Day.
-- [23-6-28] bandmap now displays callsigns in red if they have been worked before.
-- [23-6-21] cty updater needs work changed to ondemand.
-- [23-6-18] Pinned lib notctyparser to >= 26.6.18. Fix bug allowing editing RST field.
-- [23-6-17] Trapped ValueError from notctyparser when environment variable `LC_TIME` set to `lt_LT.UTF-8`.
-- [23-6-16] Send F1-12 button text, not tooltip in RadioInfo packet. Add `File->Update MASTER.SCP`. Add `Help->Help`
-- [23-6-15] Add `Help->HotKeys`.
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
-- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+- [23-7-2] bandmap now requests worked list at startup.
+
+See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
 ### Python and pip
 
 This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
@@ -449,24 +442,30 @@
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
-### Bandmap
+## Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
+VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/VFO_and_bandwidth_markers.png)
+
+Clicked on spots now tune the radio and set the callsign field. Previously worked calls are displayed in red.
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.6.30.1/README.md` & `not1mm-23.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
-    - [Bandmap](#bandmap)
+  - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -113,24 +113,17 @@
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 - RAC Canada Day
 
 ## Recent Changes
 
-- [23-6-30] Added RAC Canada Day.
-- [23-6-28] bandmap now displays callsigns in red if they have been worked before.
-- [23-6-21] cty updater needs work changed to ondemand.
-- [23-6-18] Pinned lib notctyparser to >= 26.6.18. Fix bug allowing editing RST field.
-- [23-6-17] Trapped ValueError from notctyparser when environment variable `LC_TIME` set to `lt_LT.UTF-8`.
-- [23-6-16] Send F1-12 button text, not tooltip in RadioInfo packet. Add `File->Update MASTER.SCP`. Add `Help->Help`
-- [23-6-15] Add `Help->HotKeys`.
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
-- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+- [23-7-2] bandmap now requests worked list at startup.
+
+See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
 ### Python and pip
 
 This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
@@ -430,24 +423,30 @@
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
-### Bandmap
+## Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
+VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/VFO_and_bandwidth_markers.png)
+
+Clicked on spots now tune the radio and set the callsign field. Previously worked calls are displayed in red.
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.6.30.1/not1mm/__main__.py` & `not1mm-23.7.2/not1mm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4570,1334 +4570,1326 @@
 00011d90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
 00011da0: 662e 6361 6c6c 7369 676e 2e73 6574 466f  f.callsign.setFo
 00011db0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
 00011dc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
 00011dd0: 616c 6c73 6967 6e2e 6163 7469 7661 7465  allsign.activate
 00011de0: 5769 6e64 6f77 2829 0a20 2020 2020 2020  Window().       
 00011df0: 2020 2020 2020 2020 2020 2020 2077 696e               win
-00011e00: 646f 772e 7261 6973 655f 2829 0a20 2020  dow.raise_().   
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2023 2066 6720 3d20 7769 6e64 6f77 2e66   # fg = window.f
-00011e30: 7261 6d65 4765 6f6d 6574 7279 2829 2e74  rameGeometry().t
-00011e40: 6f70 4c65 6674 0a20 2020 2020 2020 2020  opLeft.         
-00011e50: 2020 2020 2020 2020 2020 2023 2023 205f             # # _
-00011e60: 7769 6474 6820 3d20 7365 6c66 2e73 697a  width = self.siz
-00011e70: 6528 292e 7769 6474 6828 290a 2020 2020  e().width().    
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2320 2320 5f68 6569 6768 7420 3d20 7365  # # _height = se
-00011ea0: 6c66 2e73 697a 6528 292e 6865 6967 6874  lf.size().height
-00011eb0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011ec0: 2020 2020 2020 2023 2023 205f 7820 3d20         # # _x = 
-00011ed0: 7365 6c66 2e70 6f73 2829 2e78 2829 0a20  self.pos().x(). 
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2020 2023 2023 205f 7920 3d20 7365 6c66     # # _y = self
-00011f00: 2e70 6f73 2829 2e79 2829 0a20 2020 2020  .pos().y().     
-00011f10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011f20: 2023 2070 7269 6e74 2866 222a 2a2a 2a2a   # print(f"*****
-00011f30: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00011f40: 2a2a 2a2a 2a2a 2a20 7820 7b5f 787d 2079  ******* x {_x} y
-00011f50: 207b 5f79 7d22 290a 2020 2020 2020 2020   {_y}").        
-00011f60: 2020 2020 2020 2020 2020 2020 2320 2320              # # 
-00011f70: 7769 6e64 6f77 2e68 6964 6528 290a 2020  window.hide().  
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2020 2320 2320 7769 6e64 6f77 2e73 686f    # # window.sho
-00011fa0: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-00011fb0: 2020 2020 2020 2020 2320 2320 7769 6e64          # # wind
-00011fc0: 6f77 2e73 6574 4765 6f6d 6574 7279 2830  ow.setGeometry(0
-00011fd0: 2c20 302c 205f 7769 6474 682c 205f 6865  , 0, _width, _he
-00011fe0: 6967 6874 290a 2020 2020 2020 2020 2020  ight).          
-00011ff0: 2020 2020 2020 2020 2020 2320 7769 6e64            # wind
-00012000: 6f77 2e73 686f 7728 290a 2020 2020 2020  ow.show().      
-00012010: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00012020: 7769 6e64 6f77 2e67 656f 6d65 7472 7928  window.geometry(
-00012030: 292e 7365 7458 2831 3030 290a 2020 2020  ).setX(100).    
-00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012050: 2320 7769 6e64 6f77 2e67 656f 6d65 7472  # window.geometr
-00012060: 7928 292e 7365 7459 2831 3030 290a 0a20  y().setY(100).. 
-00012070: 2020 2064 6566 2063 775f 6d61 6372 6f73     def cw_macros
-00012080: 5f73 7461 7465 5f63 6861 6e67 6564 2873  _state_changed(s
-00012090: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000120a0: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
-000120b0: 6f77 2f68 6964 6520 6d61 6372 6f20 6275  ow/hide macro bu
-000120c0: 7474 6f6e 7322 2222 0a20 2020 2020 2020  ttons""".       
-000120d0: 2073 656c 662e 7072 6566 5b22 6377 5f6d   self.pref["cw_m
-000120e0: 6163 726f 7322 5d20 3d20 7365 6c66 2e61  acros"] = self.a
-000120f0: 6374 696f 6e43 575f 4d61 6372 6f73 2e69  ctionCW_Macros.i
-00012100: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
-00012110: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-00012120: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-00012130: 2020 2073 656c 662e 7368 6f77 5f43 575f     self.show_CW_
-00012140: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
-00012150: 6620 7368 6f77 5f43 575f 6d61 6372 6f73  f show_CW_macros
-00012160: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00012170: 2222 226d 6163 726f 2062 7574 746f 6e20  """macro button 
-00012180: 7374 6174 6520 6368 616e 6765 2222 220a  state change""".
-00012190: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000121a0: 7072 6566 2e67 6574 2822 6377 5f6d 6163  pref.get("cw_mac
-000121b0: 726f 7322 293a 0a20 2020 2020 2020 2020  ros"):.         
-000121c0: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
-000121d0: 6f77 312e 7368 6f77 2829 0a20 2020 2020  ow1.show().     
-000121e0: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
-000121f0: 6f6e 5f52 6f77 322e 7368 6f77 2829 0a20  on_Row2.show(). 
-00012200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00012210: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
-00012220: 7474 6f6e 5f52 6f77 312e 6869 6465 2829  tton_Row1.hide()
-00012230: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012240: 662e 4275 7474 6f6e 5f52 6f77 322e 6869  f.Button_Row2.hi
-00012250: 6465 2829 0a0a 2020 2020 6465 6620 636f  de()..    def co
-00012260: 6d6d 616e 645f 6275 7474 6f6e 735f 7374  mmand_buttons_st
-00012270: 6174 655f 6368 616e 6765 2873 656c 6629  ate_change(self)
-00012280: 3a0a 2020 2020 2020 2020 2222 224d 656e  :.        """Men
-00012290: 7520 6974 656d 2074 6f20 7368 6f77 2f68  u item to show/h
-000122a0: 6964 6520 636f 6d6d 616e 6420 6275 7474  ide command butt
-000122b0: 6f6e 7322 2222 0a20 2020 2020 2020 2073  ons""".        s
-000122c0: 656c 662e 7072 6566 5b22 636f 6d6d 616e  elf.pref["comman
-000122d0: 645f 6275 7474 6f6e 7322 5d20 3d20 7365  d_buttons"] = se
-000122e0: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
-000122f0: 5f42 7574 746f 6e73 2e69 7343 6865 636b  _Buttons.isCheck
-00012300: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-00012310: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-00012320: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-00012330: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
-00012340: 7574 746f 6e73 2829 0a0a 2020 2020 6465  uttons()..    de
-00012350: 6620 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f show_command_b
-00012360: 7574 746f 6e73 2873 656c 6629 3a0a 2020  uttons(self):.  
-00012370: 2020 2020 2020 2222 2263 6f6d 6d61 6e64        """command
-00012380: 2062 7574 746f 6e20 7374 6174 6520 6368   button state ch
-00012390: 616e 6765 2222 220a 2020 2020 2020 2020  ange""".        
-000123a0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-000123b0: 2822 636f 6d6d 616e 645f 6275 7474 6f6e  ("command_button
-000123c0: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
-000123d0: 2073 656c 662e 436f 6d6d 616e 645f 4275   self.Command_Bu
-000123e0: 7474 6f6e 732e 7368 6f77 2829 0a20 2020  ttons.show().   
-000123f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012400: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
-00012410: 616e 645f 4275 7474 6f6e 732e 6869 6465  and_Buttons.hide
-00012420: 2829 0a0a 2020 2020 6465 6620 6973 5f66  ()..    def is_f
-00012430: 6c6f 6174 6162 6c65 2873 656c 662c 2069  loatable(self, i
-00012440: 7465 6d3a 2073 7472 2920 2d3e 2062 6f6f  tem: str) -> boo
-00012450: 6c3a 0a20 2020 2020 2020 2022 2222 6368  l:.        """ch
-00012460: 6563 6b20 746f 2073 6565 2069 6620 7374  eck to see if st
-00012470: 7269 6e67 2063 616e 2062 6520 6120 666c  ring can be a fl
-00012480: 6f61 7422 2222 0a20 2020 2020 2020 2069  oat""".        i
-00012490: 6620 6974 656d 2e69 736e 756d 6572 6963  f item.isnumeric
-000124a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000124b0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-000124c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000124d0: 2020 2020 205f 7465 7374 203d 2066 6c6f       _test = flo
-000124e0: 6174 2869 7465 6d29 0a20 2020 2020 2020  at(item).       
-000124f0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00012500: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00012510: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00012520: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00012530: 0a0a 2020 2020 6465 6620 6f74 6865 725f  ..    def other_
-00012540: 325f 6368 616e 6765 6428 7365 6c66 293a  2_changed(self):
-00012550: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
-00012560: 6564 2077 6865 6e20 7765 206e 6565 6420  ed when we need 
-00012570: 746f 2070 6172 7365 2053 5320 6578 6368  to parse SS exch
-00012580: 616e 6765 2e22 2222 0a20 2020 2020 2020  ange.""".       
-00012590: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-000125a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000125b0: 2022 4152 524c 2053 7765 6570 7374 616b   "ARRL Sweepstak
-000125c0: 6573 2220 696e 2073 656c 662e 636f 6e74  es" in self.cont
-000125d0: 6573 742e 6e61 6d65 3a0a 2020 2020 2020  est.name:.      
-000125e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000125f0: 6f6e 7465 7374 2e70 6172 7365 5f65 7863  ontest.parse_exc
-00012600: 6861 6e67 6528 7365 6c66 290a 0a20 2020  hange(self)..   
-00012610: 2064 6566 2063 616c 6c73 6967 6e5f 6368   def callsign_ch
-00012620: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
-00012630: 2020 2020 2022 2222 4361 6c6c 6564 2077       """Called w
-00012640: 6865 6e20 7465 7874 2069 6e20 7468 6520  hen text in the 
-00012650: 6361 6c6c 7369 676e 2066 6965 6c64 2068  callsign field h
-00012660: 6173 2063 6861 6e67 6564 2222 220a 2020  as changed""".  
-00012670: 2020 2020 2020 7465 7874 203d 2073 656c        text = sel
-00012680: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
-00012690: 290a 2020 2020 2020 2020 7465 7874 203d  ).        text =
-000126a0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
-000126b0: 2020 2020 2020 706f 7369 7469 6f6e 203d        position =
-000126c0: 2073 656c 662e 6361 6c6c 7369 676e 2e63   self.callsign.c
-000126d0: 7572 736f 7250 6f73 6974 696f 6e28 290a  ursorPosition().
-000126e0: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-000126f0: 5f74 6578 7420 3d20 7465 7874 2e73 7472  _text = text.str
-00012700: 6970 2829 2e72 6570 6c61 6365 2822 2022  ip().replace(" "
-00012710: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-00012720: 6c66 2e63 616c 6c73 6967 6e2e 7365 7454  lf.callsign.setT
-00012730: 6578 7428 7374 7269 7070 6564 5f74 6578  ext(stripped_tex
-00012740: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00012750: 6361 6c6c 7369 676e 2e73 6574 4375 7273  callsign.setCurs
-00012760: 6f72 506f 7369 7469 6f6e 2870 6f73 6974  orPosition(posit
-00012770: 696f 6e29 0a0a 2020 2020 2020 2020 6966  ion)..        if
-00012780: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
-00012790: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-000127a0: 6970 7065 645f 7465 7874 203d 3d20 2243  ipped_text == "C
-000127b0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
-000127c0: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
-000127d0: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
-000127e0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-000127f0: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
-00012800: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
-00012810: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00012820: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00012850: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012870: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-00012880: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2243  trol.set_mode("C
-00012890: 5722 290a 2020 2020 2020 2020 2020 2020  W").            
-000128a0: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
-000128b0: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
-000128c0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-000128d0: 6122 2c20 2230 2e30 2229 2929 0a20 2020  a", "0.0"))).   
-000128e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000128f0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
-00012900: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
-00012910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012920: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-00012930: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00012940: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
-00012950: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
-00012960: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
-00012970: 6377 5f6d 6163 726f 7328 290a 2020 2020  cw_macros().    
-00012980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012990: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
-000129a0: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
-000129b0: 3d3d 2022 5254 5459 223a 0a20 2020 2020  == "RTTY":.     
-000129c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000129d0: 7365 746d 6f64 6528 2252 5454 5922 290a  setmode("RTTY").
-000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129f0: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00012a00: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-00012a10: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00012a20: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
-00012a30: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
-00012a40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012a50: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
-00012a60: 745f 6d6f 6465 2822 5254 5459 2229 0a20  t_mode("RTTY"). 
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00012ab0: 655b 226d 6f64 6522 5d20 3d20 2252 5454  e["mode"] = "RTT
-00012ac0: 5922 0a20 2020 2020 2020 2020 2020 2020  Y".             
-00012ad0: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-00012ae0: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
-00012af0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-00012b00: 222c 2022 302e 3022 2929 290a 2020 2020  ", "0.0"))).    
-00012b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012b20: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-00012b30: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
+00011e00: 646f 772e 7261 6973 655f 2829 0a0a 2020  dow.raise_()..  
+00011e10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011e20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00011e30: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
+00011e40: 2e67 6574 2822 636d 6422 2c20 2222 2920  .get("cmd", "") 
+00011e50: 3d3d 2022 4745 5457 4f52 4b45 444c 4953  == "GETWORKEDLIS
+00011e60: 5422 0a20 2020 2020 2020 2020 2020 2020  T".             
+00011e70: 2020 2020 2020 2061 6e64 206a 736f 6e5f         and json_
+00011e80: 6461 7461 2e67 6574 2822 7374 6174 696f  data.get("statio
+00011e90: 6e22 2c20 2222 2920 3d3d 2070 6c61 7466  n", "") == platf
+00011ea0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00011eb0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00011ee0: 6461 7461 6261 7365 2e67 6574 5f63 616c  database.get_cal
+00011ef0: 6c73 5f61 6e64 5f62 616e 6473 2829 0a20  ls_and_bands(). 
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f30: 636d 645b 2263 6d64 225d 203d 2022 574f  cmd["cmd"] = "WO
+00011f40: 524b 4544 220a 2020 2020 2020 2020 2020  RKED".          
+00011f50: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00011f60: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00011f70: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011f90: 6d64 5b22 776f 726b 6564 225d 203d 2072  md["worked"] = r
+00011fa0: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
+00011fb0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00011fc0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+00011fd0: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+00011fe0: 636d 6429 0a0a 2020 2020 6465 6620 6377  cmd)..    def cw
+00011ff0: 5f6d 6163 726f 735f 7374 6174 655f 6368  _macros_state_ch
+00012000: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
+00012010: 2020 2020 2022 2222 4d65 6e75 2069 7465       """Menu ite
+00012020: 6d20 746f 2073 686f 772f 6869 6465 206d  m to show/hide m
+00012030: 6163 726f 2062 7574 746f 6e73 2222 220a  acro buttons""".
+00012040: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00012050: 665b 2263 775f 6d61 6372 6f73 225d 203d  f["cw_macros"] =
+00012060: 2073 656c 662e 6163 7469 6f6e 4357 5f4d   self.actionCW_M
+00012070: 6163 726f 732e 6973 4368 6563 6b65 6428  acros.isChecked(
+00012080: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
+00012090: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+000120a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000120b0: 686f 775f 4357 5f6d 6163 726f 7328 290a  how_CW_macros().
+000120c0: 0a20 2020 2064 6566 2073 686f 775f 4357  .    def show_CW
+000120d0: 5f6d 6163 726f 7328 7365 6c66 293a 0a20  _macros(self):. 
+000120e0: 2020 2020 2020 2022 2222 6d61 6372 6f20         """macro 
+000120f0: 6275 7474 6f6e 2073 7461 7465 2063 6861  button state cha
+00012100: 6e67 6522 2222 0a20 2020 2020 2020 2069  nge""".        i
+00012110: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00012120: 2263 775f 6d61 6372 6f73 2229 3a0a 2020  "cw_macros"):.  
+00012130: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
+00012140: 7574 746f 6e5f 526f 7731 2e73 686f 7728  utton_Row1.show(
+00012150: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00012160: 6c66 2e42 7574 746f 6e5f 526f 7732 2e73  lf.Button_Row2.s
+00012170: 686f 7728 290a 2020 2020 2020 2020 656c  how().        el
+00012180: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012190: 7365 6c66 2e42 7574 746f 6e5f 526f 7731  self.Button_Row1
+000121a0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+000121b0: 2020 2020 7365 6c66 2e42 7574 746f 6e5f      self.Button_
+000121c0: 526f 7732 2e68 6964 6528 290a 0a20 2020  Row2.hide()..   
+000121d0: 2064 6566 2063 6f6d 6d61 6e64 5f62 7574   def command_but
+000121e0: 746f 6e73 5f73 7461 7465 5f63 6861 6e67  tons_state_chang
+000121f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00012200: 2022 2222 4d65 6e75 2069 7465 6d20 746f   """Menu item to
+00012210: 2073 686f 772f 6869 6465 2063 6f6d 6d61   show/hide comma
+00012220: 6e64 2062 7574 746f 6e73 2222 220a 2020  nd buttons""".  
+00012230: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+00012240: 2263 6f6d 6d61 6e64 5f62 7574 746f 6e73  "command_buttons
+00012250: 225d 203d 2073 656c 662e 6163 7469 6f6e  "] = self.action
+00012260: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
+00012270: 6973 4368 6563 6b65 6428 290a 2020 2020  isChecked().    
+00012280: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
+00012290: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
+000122a0: 2020 2020 7365 6c66 2e73 686f 775f 636f      self.show_co
+000122b0: 6d6d 616e 645f 6275 7474 6f6e 7328 290a  mmand_buttons().
+000122c0: 0a20 2020 2064 6566 2073 686f 775f 636f  .    def show_co
+000122d0: 6d6d 616e 645f 6275 7474 6f6e 7328 7365  mmand_buttons(se
+000122e0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000122f0: 636f 6d6d 616e 6420 6275 7474 6f6e 2073  command button s
+00012300: 7461 7465 2063 6861 6e67 6522 2222 0a20  tate change""". 
+00012310: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00012320: 7265 662e 6765 7428 2263 6f6d 6d61 6e64  ref.get("command
+00012330: 5f62 7574 746f 6e73 2229 3a0a 2020 2020  _buttons"):.    
+00012340: 2020 2020 2020 2020 7365 6c66 2e43 6f6d          self.Com
+00012350: 6d61 6e64 5f42 7574 746f 6e73 2e73 686f  mand_Buttons.sho
+00012360: 7728 290a 2020 2020 2020 2020 656c 7365  w().        else
+00012370: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012380: 6c66 2e43 6f6d 6d61 6e64 5f42 7574 746f  lf.Command_Butto
+00012390: 6e73 2e68 6964 6528 290a 0a20 2020 2064  ns.hide()..    d
+000123a0: 6566 2069 735f 666c 6f61 7461 626c 6528  ef is_floatable(
+000123b0: 7365 6c66 2c20 6974 656d 3a20 7374 7229  self, item: str)
+000123c0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+000123d0: 2020 2222 2263 6865 636b 2074 6f20 7365    """check to se
+000123e0: 6520 6966 2073 7472 696e 6720 6361 6e20  e if string can 
+000123f0: 6265 2061 2066 6c6f 6174 2222 220a 2020  be a float""".  
+00012400: 2020 2020 2020 6966 2069 7465 6d2e 6973        if item.is
+00012410: 6e75 6d65 7269 6328 293a 0a20 2020 2020  numeric():.     
+00012420: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00012430: 7565 0a20 2020 2020 2020 2074 7279 3a0a  ue.        try:.
+00012440: 2020 2020 2020 2020 2020 2020 5f74 6573              _tes
+00012450: 7420 3d20 666c 6f61 7428 6974 656d 290a  t = float(item).
+00012460: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+00012470: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
+00012480: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00012490: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+000124a0: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+000124b0: 206f 7468 6572 5f32 5f63 6861 6e67 6564   other_2_changed
+000124c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000124d0: 2222 2243 616c 6c65 6420 7768 656e 2077  """Called when w
+000124e0: 6520 6e65 6564 2074 6f20 7061 7273 6520  e need to parse 
+000124f0: 5353 2065 7863 6861 6e67 652e 2222 220a  SS exchange.""".
+00012500: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012510: 636f 6e74 6573 743a 0a20 2020 2020 2020  contest:.       
+00012520: 2020 2020 2069 6620 2241 5252 4c20 5377       if "ARRL Sw
+00012530: 6565 7073 7461 6b65 7322 2069 6e20 7365  eepstakes" in se
+00012540: 6c66 2e63 6f6e 7465 7374 2e6e 616d 653a  lf.contest.name:
+00012550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012560: 2073 656c 662e 636f 6e74 6573 742e 7061   self.contest.pa
+00012570: 7273 655f 6578 6368 616e 6765 2873 656c  rse_exchange(sel
+00012580: 6629 0a0a 2020 2020 6465 6620 6361 6c6c  f)..    def call
+00012590: 7369 676e 5f63 6861 6e67 6564 2873 656c  sign_changed(sel
+000125a0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+000125b0: 616c 6c65 6420 7768 656e 2074 6578 7420  alled when text 
+000125c0: 696e 2074 6865 2063 616c 6c73 6967 6e20  in the callsign 
+000125d0: 6669 656c 6420 6861 7320 6368 616e 6765  field has change
+000125e0: 6422 2222 0a20 2020 2020 2020 2074 6578  d""".        tex
+000125f0: 7420 3d20 7365 6c66 2e63 616c 6c73 6967  t = self.callsig
+00012600: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
+00012610: 2074 6578 7420 3d20 7465 7874 2e75 7070   text = text.upp
+00012620: 6572 2829 0a20 2020 2020 2020 2070 6f73  er().        pos
+00012630: 6974 696f 6e20 3d20 7365 6c66 2e63 616c  ition = self.cal
+00012640: 6c73 6967 6e2e 6375 7273 6f72 506f 7369  lsign.cursorPosi
+00012650: 7469 6f6e 2829 0a20 2020 2020 2020 2073  tion().        s
+00012660: 7472 6970 7065 645f 7465 7874 203d 2074  tripped_text = t
+00012670: 6578 742e 7374 7269 7028 292e 7265 706c  ext.strip().repl
+00012680: 6163 6528 2220 222c 2022 2229 0a20 2020  ace(" ", "").   
+00012690: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+000126a0: 676e 2e73 6574 5465 7874 2873 7472 6970  gn.setText(strip
+000126b0: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
+000126c0: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
+000126d0: 7365 7443 7572 736f 7250 6f73 6974 696f  setCursorPositio
+000126e0: 6e28 706f 7369 7469 6f6e 290a 0a20 2020  n(position)..   
+000126f0: 2020 2020 2069 6620 2220 2220 696e 2074       if " " in t
+00012700: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+00012710: 2069 6620 7374 7269 7070 6564 5f74 6578   if stripped_tex
+00012720: 7420 3d3d 2022 4357 223a 0a20 2020 2020  t == "CW":.     
+00012730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012740: 7365 746d 6f64 6528 2243 5722 290a 2020  setmode("CW").  
+00012750: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012760: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00012770: 6d6f 6465 225d 203d 2022 4357 220a 2020  mode"] = "CW".  
+00012780: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012790: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+000127a0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+000127b0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000127c0: 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c 696e  ig_control.onlin
+000127d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000127e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000127f0: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
+00012800: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
+00012810: 2020 2020 2020 2020 2020 2062 616e 6420             band 
+00012820: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
+00012830: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00012840: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
+00012850: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00012860: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
+00012870: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
+00012880: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012890: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+000128a0: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+000128b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000128c0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+000128d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000128e0: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
+000128f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012900: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00012910: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
+00012920: 645f 7465 7874 203d 3d20 2252 5454 5922  d_text == "RTTY"
+00012930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012940: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
+00012950: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
+00012960: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00012970: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012990: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+000129a0: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
+000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129c0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+000129d0: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2252  trol.set_mode("R
+000129e0: 5454 5922 290a 2020 2020 2020 2020 2020  TTY").          
+000129f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a10: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00012a20: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
+00012a30: 203d 2022 5254 5459 220a 2020 2020 2020   = "RTTY".      
+00012a40: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
+00012a50: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
+00012a60: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00012a70: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
+00012a80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00012a90: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
+00012aa0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
+00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ac0: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
+00012ad0: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
+00012ae0: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00012af0: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
+00012b00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012b10: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00012b20: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
+00012b30: 3d3d 2022 5353 4222 3a0a 2020 2020 2020  == "SSB":.      
 00012b40: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00012b50: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00012b60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012b70: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00012b80: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00012b90: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00012ba0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-00012bb0: 7065 645f 7465 7874 203d 3d20 2253 5342  ped_text == "SSB
-00012bc0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00012bd0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
-00012be0: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
-00012bf0: 2020 2020 2020 2069 6620 696e 7428 7365         if int(se
-00012c00: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00012c10: 6574 2822 7666 6f61 222c 2030 2929 203e  et("vfoa", 0)) >
-00012c20: 2031 3030 3030 3030 303a 0a20 2020 2020   10000000:.     
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012c40: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00012c50: 226d 6f64 6522 5d20 3d20 2255 5342 220a  "mode"] = "USB".
-00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012c80: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00012c90: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00012ca0: 225d 203d 2022 4c53 4222 0a20 2020 2020  "] = "LSB".     
-00012cb0: 2020 2020 2020 2020 2020 2062 616e 6420             band 
-00012cc0: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
-00012cd0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00012ce0: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
-00012cf0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00012d00: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
-00012d10: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
-00012d20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012d30: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-00012d40: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-00012d50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00012d60: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-00012d90: 726f 6c2e 7365 745f 6d6f 6465 2873 656c  rol.set_mode(sel
-00012da0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00012db0: 7428 226d 6f64 6522 2929 0a20 2020 2020  t("mode")).     
-00012dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012dd0: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
-00012de0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012df0: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
-00012e00: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00012e10: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00012e20: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
-00012e30: 6564 5f74 6578 7420 3d3d 2022 4f50 4f4e  ed_text == "OPON
-00012e40: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00012e50: 2020 2073 656c 662e 6765 745f 6f70 6f6e     self.get_opon
-00012e60: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00012e70: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
-00012e80: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
-00012e90: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00012ea0: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
-00012eb0: 7070 6564 5f74 6578 7420 3d3d 2022 4845  pped_text == "HE
-00012ec0: 4c50 223a 0a20 2020 2020 2020 2020 2020  LP":.           
-00012ed0: 2020 2020 2073 656c 662e 7368 6f77 5f68       self.show_h
-00012ee0: 656c 705f 6469 616c 6f67 2829 0a20 2020  elp_dialog().   
-00012ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012f00: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00012f30: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
-00012f40: 6578 7420 3d3d 2022 5445 5354 223a 0a20  ext == "TEST":. 
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012f60: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
-00012f70: 6162 6173 652e 6765 745f 6361 6c6c 735f  abase.get_calls_
-00012f80: 616e 645f 6261 6e64 7328 290a 2020 2020  and_bands().    
-00012f90: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00012fa0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00012fb0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-00012fc0: 3d20 2257 4f52 4b45 4422 0a20 2020 2020  = "WORKED".     
-00012fd0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00012fe0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00012ff0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00013000: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00013010: 2277 6f72 6b65 6422 5d20 3d20 7265 7375  "worked"] = resu
-00013020: 6c74 0a20 2020 2020 2020 2020 2020 2020  lt.             
-00013030: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
-00013040: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
-00013050: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
-00013060: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013070: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
-00013080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013090: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000130a0: 2020 2020 6966 2073 656c 662e 6973 5f66      if self.is_f
-000130b0: 6c6f 6174 6162 6c65 2873 7472 6970 7065  loatable(strippe
-000130c0: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
-000130d0: 2020 2020 2020 2020 2076 666f 203d 2066           vfo = f
-000130e0: 6c6f 6174 2873 7472 6970 7065 645f 7465  loat(stripped_te
-000130f0: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
-00013100: 2020 2020 7666 6f20 3d20 696e 7428 7666      vfo = int(vf
-00013110: 6f20 2a20 3130 3030 290a 2020 2020 2020  o * 1000).      
-00013120: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-00013130: 2067 6574 6261 6e64 2873 7472 2876 666f   getband(str(vfo
-00013140: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00013150: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
-00013160: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
-00013170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013180: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-00013190: 2242 616e 6422 5d20 3d20 6765 745f 6c6f  "Band"] = get_lo
-000131a0: 6767 6564 5f62 616e 6428 7374 7228 7365  gged_band(str(se
-000131b0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-000131c0: 6574 2822 7666 6f61 222c 2030 2e30 2929  et("vfoa", 0.0))
-000131d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000131e0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
-000131f0: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
-00013200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013210: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00013220: 655b 2262 616e 6422 5d20 3d20 6261 6e64  e["band"] = band
-00013230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013240: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
-00013250: 616e 6422 5d20 3d20 6765 745f 6c6f 6767  and"] = get_logg
-00013260: 6564 5f62 616e 6428 7374 7228 7666 6f29  ed_band(str(vfo)
-00013270: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013280: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-00013290: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-000132a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000132b0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-000132c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000132d0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-000132e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000132f0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-00013300: 6f6e 7472 6f6c 2e73 6574 5f76 666f 2876  ontrol.set_vfo(v
-00013310: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
-00013320: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00013330: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013340: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00013350: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00013360: 225d 203d 2022 5241 4449 4f5f 5354 4154  "] = "RADIO_STAT
-00013370: 4522 0a20 2020 2020 2020 2020 2020 2020  E".             
-00013380: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-00013390: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-000133a0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-000133b0: 2020 2020 636d 645b 2262 616e 6422 5d20      cmd["band"] 
-000133c0: 3d20 6261 6e64 0a20 2020 2020 2020 2020  = band.         
-000133d0: 2020 2020 2020 2063 6d64 5b22 7666 6f61         cmd["vfoa
-000133e0: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
-000133f0: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-00013400: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00013410: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00013420: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-00013430: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-00013440: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-00013450: 636b 5f63 616c 6c73 6967 6e28 7374 7269  ck_callsign(stri
-00013460: 7070 6564 5f74 6578 7429 0a20 2020 2020  pped_text).     
-00013470: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00013480: 6865 636b 5f64 7570 6528 7374 7269 7070  heck_dupe(stripp
-00013490: 6564 5f74 6578 7429 3a0a 2020 2020 2020  ed_text):.      
-000134a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000134b0: 7570 655f 696e 6469 6361 746f 722e 7368  upe_indicator.sh
-000134c0: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
-000134d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000134e0: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
-000134f0: 5f69 6e64 6963 6174 6f72 2e68 6964 6528  _indicator.hide(
-00013500: 290a 2020 2020 2020 2020 2020 2020 5f74  ).            _t
-00013510: 6865 7468 7265 6164 203d 2074 6872 6561  hethread = threa
-00013520: 6469 6e67 2e54 6872 6561 6428 0a20 2020  ding.Thread(.   
-00013530: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00013540: 6765 743d 7365 6c66 2e63 6865 636b 5f63  get=self.check_c
-00013550: 616c 6c73 6967 6e32 2c0a 2020 2020 2020  allsign2,.      
-00013560: 2020 2020 2020 2020 2020 6172 6773 3d28            args=(
-00013570: 7465 7874 2c29 2c0a 2020 2020 2020 2020  text,),.        
-00013580: 2020 2020 2020 2020 6461 656d 6f6e 3d54          daemon=T
-00013590: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000135a0: 2029 0a20 2020 2020 2020 2020 2020 205f   ).            _
-000135b0: 7468 6574 6872 6561 642e 7374 6172 7428  thethread.start(
-000135c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000135d0: 6c66 2e6e 6578 745f 6669 656c 642e 7365  lf.next_field.se
-000135e0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-000135f0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00013600: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-00013610: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-00013620: 3d20 2243 414c 4c43 4841 4e47 4544 220a  = "CALLCHANGED".
-00013630: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-00013640: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-00013650: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-00013660: 2063 6d64 5b22 6361 6c6c 225d 203d 2073   cmd["call"] = s
-00013670: 7472 6970 7065 645f 7465 7874 0a20 2020  tripped_text.   
-00013680: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
-00013690: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
-000136a0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
-000136b0: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-000136c0: 636b 5f63 616c 6c73 6967 6e28 7374 7269  ck_callsign(stri
-000136d0: 7070 6564 5f74 6578 7429 0a0a 2020 2020  pped_text)..    
-000136e0: 6465 6620 6368 6563 6b5f 6361 6c6c 7369  def check_callsi
-000136f0: 676e 2873 656c 662c 2063 616c 6c73 6967  gn(self, callsig
-00013700: 6e29 3a0a 2020 2020 2020 2020 2222 2243  n):.        """C
-00013710: 6865 636b 2063 616c 6c20 6173 2065 6e74  heck call as ent
-00013720: 6572 6564 2222 220a 2020 2020 2020 2020  ered""".        
-00013730: 7265 7375 6c74 203d 2073 656c 662e 6374  result = self.ct
-00013740: 795f 6c6f 6f6b 7570 2863 616c 6c73 6967  y_lookup(callsig
-00013750: 6e29 0a20 2020 2020 2020 2064 6562 7567  n).        debug
-00013760: 5f72 6573 756c 7420 3d20 6622 7b72 6573  _result = f"{res
-00013770: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
-00013780: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00013790: 2064 6562 7567 5f72 6573 756c 7429 0a20   debug_result). 
-000137a0: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-000137b0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000137c0: 7220 6120 696e 2072 6573 756c 742e 6974  r a in result.it
-000137d0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-000137e0: 2020 2020 2020 2065 6e74 6974 7920 3d20         entity = 
-000137f0: 615b 315d 2e67 6574 2822 656e 7469 7479  a[1].get("entity
-00013800: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-00013810: 2020 2020 2020 2063 7120 3d20 615b 315d         cq = a[1]
-00013820: 2e67 6574 2822 6371 222c 2022 2229 0a20  .get("cq", ""). 
-00013830: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013840: 7475 203d 2061 5b31 5d2e 6765 7428 2269  tu = a[1].get("i
-00013850: 7475 222c 2022 2229 0a20 2020 2020 2020  tu", "").       
-00013860: 2020 2020 2020 2020 2063 6f6e 7469 6e65           contine
-00013870: 6e74 203d 2061 5b31 5d2e 6765 7428 2263  nt = a[1].get("c
-00013880: 6f6e 7469 6e65 6e74 2229 0a20 2020 2020  ontinent").     
-00013890: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
-000138a0: 2066 6c6f 6174 2861 5b31 5d2e 6765 7428   float(a[1].get(
-000138b0: 226c 6174 222c 2022 302e 3022 2929 0a20  "lat", "0.0")). 
-000138c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000138d0: 6f6e 203d 2066 6c6f 6174 2861 5b31 5d2e  on = float(a[1].
-000138e0: 6765 7428 226c 6f6e 6722 2c20 2230 2e30  get("long", "0.0
-000138f0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-00013900: 2020 2020 6c6f 6e20 3d20 6c6f 6e20 2a20      lon = lon * 
-00013910: 2d31 2020 2320 6374 792e 6461 7420 6669  -1  # cty.dat fi
-00013920: 6c65 2069 6e76 6572 7473 206c 6f6e 6769  le inverts longi
-00013930: 7475 6465 730a 2020 2020 2020 2020 2020  tudes.          
-00013940: 2020 2020 2020 7072 696d 6172 795f 7066        primary_pf
-00013950: 7820 3d20 615b 315d 2e67 6574 2822 7072  x = a[1].get("pr
-00013960: 696d 6172 795f 7066 7822 2c20 2222 290a  imary_pfx", "").
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
-00013990: 675f 7769 7468 5f6c 6174 6c6f 6e28 7365  g_with_latlon(se
-000139a0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-000139b0: 4772 6964 5371 7561 7265 2229 2c20 6c61  GridSquare"), la
-000139c0: 742c 206c 6f6e 290a 2020 2020 2020 2020  t, lon).        
-000139d0: 2020 2020 2020 2020 6b69 6c6f 6d65 7465          kilomete
-000139e0: 7273 203d 2064 6973 7461 6e63 655f 7769  rs = distance_wi
-000139f0: 7468 5f6c 6174 6c6f 6e28 0a20 2020 2020  th_latlon(.     
-00013a00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013a10: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00013a20: 2247 7269 6453 7175 6172 6522 292c 206c  "GridSquare"), l
-00013a30: 6174 2c20 6c6f 6e0a 2020 2020 2020 2020  at, lon.        
-00013a40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013a50: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00013a60: 6561 6469 6e67 5f64 6973 7461 6e63 652e  eading_distance.
-00013a70: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
-00013a80: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
-00013a90: 6567 696f 6e61 6c20 4864 6720 7b68 6561  egional Hdg {hea
-00013aa0: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
-00013ab0: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
-00013ac0: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
-00013ad0: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
-00013ae0: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
-00013af0: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
-00013b00: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
-00013b10: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
-00013b20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00013b30: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00013b40: 745b 2243 6f75 6e74 7279 5072 6566 6978  t["CountryPrefix
-00013b50: 225d 203d 2070 7269 6d61 7279 5f70 6678  "] = primary_pfx
-00013b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b70: 2073 656c 662e 636f 6e74 6163 745b 225a   self.contact["Z
-00013b80: 4e22 5d20 3d20 696e 7428 6371 290a 2020  N"] = int(cq).  
-00013b90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013ba0: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-00013bb0: 696e 656e 7422 5d20 3d20 636f 6e74 696e  inent"] = contin
-00013bc0: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-00013bd0: 2020 2020 7365 6c66 2e64 785f 656e 7469      self.dx_enti
-00013be0: 7479 2e73 6574 5465 7874 280a 2020 2020  ty.setText(.    
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 6622 7b70 7269 6d61 7279 5f70 6678 7d3a  f"{primary_pfx}:
-00013c10: 207b 636f 6e74 696e 656e 747d 2f7b 656e   {continent}/{en
-00013c20: 7469 7479 7d20 6371 3a7b 6371 7d20 6974  tity} cq:{cq} it
-00013c30: 753a 7b69 7475 7d22 0a20 2020 2020 2020  u:{itu}".       
-00013c40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00013c50: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00013c60: 6e28 6361 6c6c 7369 676e 2920 3e20 323a  n(callsign) > 2:
-00013c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c80: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00013c90: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013cb0: 6c66 2e63 6f6e 7465 7374 2e70 7265 6669  lf.contest.prefi
-00013cc0: 6c6c 2873 656c 6629 0a0a 2020 2020 6465  ll(self)..    de
-00013cd0: 6620 6368 6563 6b5f 6361 6c6c 7369 676e  f check_callsign
-00013ce0: 3228 7365 6c66 2c20 6361 6c6c 7369 676e  2(self, callsign
-00013cf0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-00013d00: 6563 6b20 6361 6c6c 206f 6e63 6520 656e  eck call once en
-00013d10: 7465 7265 6422 2222 0a20 2020 2020 2020  tered""".       
-00013d20: 2063 616c 6c73 6967 6e20 3d20 6361 6c6c   callsign = call
-00013d30: 7369 676e 2e73 7472 6970 2829 0a20 2020  sign.strip().   
-00013d40: 2020 2020 2064 6562 7567 5f6c 6f6f 6b75       debug_looku
-00013d50: 7020 3d20 6622 7b73 656c 662e 6c6f 6f6b  p = f"{self.look
-00013d60: 5f75 707d 220a 2020 2020 2020 2020 6c6f  _up}".        lo
-00013d70: 6767 6572 2e64 6562 7567 2822 2573 2c20  gger.debug("%s, 
-00013d80: 2573 222c 2063 616c 6c73 6967 6e2c 2064  %s", callsign, d
-00013d90: 6562 7567 5f6c 6f6f 6b75 7029 0a20 2020  ebug_lookup).   
-00013da0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00013db0: 7365 6c66 2e6c 6f6f 6b5f 7570 2c20 2273  self.look_up, "s
-00013dc0: 6573 7369 6f6e 2229 3a0a 2020 2020 2020  ession"):.      
-00013dd0: 2020 2020 2020 6966 2073 656c 662e 6c6f        if self.lo
-00013de0: 6f6b 5f75 702e 7365 7373 696f 6e3a 0a20  ok_up.session:. 
-00013df0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013e00: 6573 706f 6e73 6520 3d20 7365 6c66 2e6c  esponse = self.l
-00013e10: 6f6f 6b5f 7570 2e6c 6f6f 6b75 7028 6361  ook_up.lookup(ca
-00013e20: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
-00013e30: 2020 2020 2020 2020 6465 6275 675f 7265          debug_re
-00013e40: 7370 6f6e 7365 203d 2066 227b 7265 7370  sponse = f"{resp
-00013e50: 6f6e 7365 7d22 0a20 2020 2020 2020 2020  onse}".         
-00013e60: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00013e70: 6275 6728 2254 6865 2052 6573 706f 6e73  bug("The Respons
-00013e80: 653a 2025 735c 6e22 2c20 6465 6275 675f  e: %s\n", debug_
-00013e90: 7265 7370 6f6e 7365 290a 2020 2020 2020  response).      
-00013ea0: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00013eb0: 706f 6e73 653a 0a20 2020 2020 2020 2020  ponse:.         
-00013ec0: 2020 2020 2020 2020 2020 2074 6865 6972             their
-00013ed0: 6772 6964 203d 2072 6573 706f 6e73 652e  grid = response.
-00013ee0: 6765 7428 2267 7269 6422 290a 2020 2020  get("grid").    
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 7365 6c66 2e63 6f6e 7461 6374 5b22 4772  self.contact["Gr
-00013f10: 6964 5371 7561 7265 225d 203d 2074 6865  idSquare"] = the
-00013f20: 6972 6772 6964 0a20 2020 2020 2020 2020  irgrid.         
-00013f30: 2020 2020 2020 2020 2020 205f 7468 6569             _thei
-00013f40: 7263 6f75 6e74 7279 203d 2072 6573 706f  rcountry = respo
-00013f50: 6e73 652e 6765 7428 2263 6f75 6e74 7279  nse.get("country
-00013f60: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00013f70: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00013f80: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
-00013f90: 5371 7561 7265 222c 2022 2229 3a0a 2020  Square", ""):.  
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2020 2020 2020 6865 6164 696e 6720 3d20        heading = 
-00013fc0: 6265 6172 696e 6728 7365 6c66 2e73 7461  bearing(self.sta
-00013fd0: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
-00013fe0: 7561 7265 222c 2022 2229 2c20 7468 6569  uare", ""), thei
-00013ff0: 7267 7269 6429 0a20 2020 2020 2020 2020  rgrid).         
-00014000: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00014010: 696c 6f6d 6574 6572 7320 3d20 6469 7374  ilometers = dist
-00014020: 616e 6365 2873 656c 662e 7374 6174 696f  ance(self.statio
-00014030: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
-00014040: 6522 292c 2074 6865 6972 6772 6964 290a  e"), theirgrid).
-00014050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014060: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00014070: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-00014080: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
-00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2020 2066 227b 7468 6569 7267 7269 647d     f"{theirgrid}
-000140b0: 2048 6467 207b 6865 6164 696e 677d c2b0   Hdg {heading}..
-000140c0: 204c 5020 7b72 6563 6970 726f 636f 6c28   LP {reciprocol(
-000140d0: 6865 6164 696e 6729 7dc2 b020 2f20 220a  heading)}.. / ".
-000140e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140f0: 2020 2020 2020 2020 2020 2020 6622 6469              f"di
-00014100: 7374 616e 6365 207b 696e 7428 6b69 6c6f  stance {int(kilo
-00014110: 6d65 7465 7273 2a30 2e36 3231 3337 3129  meters*0.621371)
-00014120: 7d6d 6920 7b6b 696c 6f6d 6574 6572 737d  }mi {kilometers}
-00014130: 6b6d 220a 2020 2020 2020 2020 2020 2020  km".            
-00014140: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014160: 2020 2320 7365 6c66 2e64 785f 656e 7469    # self.dx_enti
-00014170: 7479 2e73 6574 5465 7874 2866 227b 7468  ty.setText(f"{th
-00014180: 6569 7263 6f75 6e74 7279 7d22 290a 2020  eircountry}").  
-00014190: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000141a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000141b0: 2020 2020 2020 2320 7365 6c66 2e68 6561        # self.hea
-000141c0: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-000141d0: 7454 6578 7428 224c 6f6f 6b75 7020 6661  tText("Lookup fa
-000141e0: 696c 6564 2e22 290a 0a20 2020 2064 6566  iled.")..    def
-000141f0: 2063 6865 636b 5f64 7570 6528 7365 6c66   check_dupe(self
-00014200: 2c20 6361 6c6c 3a20 7374 7229 202d 3e20  , call: str) -> 
-00014210: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00014220: 2243 6865 636b 7320 6966 2061 2063 616c  "Checks if a cal
-00014230: 6c73 6967 6e20 6973 2061 2064 7570 6520  lsign is a dupe 
-00014240: 6f6e 2063 7572 7265 6e74 2062 616e 642f  on current band/
-00014250: 6d6f 6465 2e22 2222 0a20 2020 2020 2020  mode.""".       
-00014260: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-00014270: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00014280: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-00014290: 6d65 7373 6167 655f 626f 7828 2259 6f75  message_box("You
-000142a0: 2068 6176 6520 6e6f 2063 6f6e 7465 7374   have no contest
-000142b0: 206c 6f61 6465 642e 2229 0a20 2020 2020   loaded.").     
-000142c0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000142d0: 6c73 650a 2020 2020 2020 2020 7365 6c66  lse.        self
-000142e0: 2e63 6f6e 7465 7374 2e70 7265 6475 7065  .contest.predupe
-000142f0: 2873 656c 6629 0a20 2020 2020 2020 2062  (self).        b
-00014300: 616e 6420 3d20 666c 6f61 7428 6765 745f  and = float(get_
-00014310: 6c6f 6767 6564 5f62 616e 6428 7374 7228  logged_band(str(
-00014320: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00014330: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
-00014340: 2929 2929 0a20 2020 2020 2020 206d 6f64  )))).        mod
-00014350: 6520 3d20 7365 6c66 2e72 6164 696f 5f73  e = self.radio_s
-00014360: 7461 7465 2e67 6574 2822 6d6f 6465 222c  tate.get("mode",
-00014370: 2022 2229 0a20 2020 2020 2020 2064 6562   "").        deb
-00014380: 7567 6c69 6e65 203d 2028 0a20 2020 2020  ugline = (.     
-00014390: 2020 2020 2020 2066 2243 616c 6c3a 207b         f"Call: {
-000143a0: 6361 6c6c 7d20 4261 6e64 3a20 7b62 616e  call} Band: {ban
-000143b0: 647d 204d 6f64 653a 207b 6d6f 6465 7d20  d} Mode: {mode} 
-000143c0: 4475 7065 7479 7065 3a20 7b73 656c 662e  Dupetype: {self.
-000143d0: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-000143e0: 657d 220a 2020 2020 2020 2020 290a 2020  e}".        ).  
-000143f0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00014400: 7567 2822 2573 222c 2064 6562 7567 6c69  ug("%s", debugli
-00014410: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-00014420: 656c 662e 636f 6e74 6573 742e 6475 7065  elf.contest.dupe
-00014430: 5f74 7970 6520 3d3d 2031 3a0a 2020 2020  _type == 1:.    
-00014440: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00014450: 2073 656c 662e 6461 7461 6261 7365 2e63   self.database.c
-00014460: 6865 636b 5f64 7570 6528 6361 6c6c 290a  heck_dupe(call).
-00014470: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014480: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-00014490: 6520 3d3d 2032 3a0a 2020 2020 2020 2020  e == 2:.        
-000144a0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-000144b0: 662e 6461 7461 6261 7365 2e63 6865 636b  f.database.check
-000144c0: 5f64 7570 655f 6f6e 5f62 616e 6428 6361  _dupe_on_band(ca
-000144d0: 6c6c 2c20 6261 6e64 290a 2020 2020 2020  ll, band).      
-000144e0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-000144f0: 742e 6475 7065 5f74 7970 6520 3d3d 2033  t.dupe_type == 3
-00014500: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00014510: 7375 6c74 203d 2073 656c 662e 6461 7461  sult = self.data
-00014520: 6261 7365 2e63 6865 636b 5f64 7570 655f  base.check_dupe_
-00014530: 6f6e 5f62 616e 645f 6d6f 6465 2863 616c  on_band_mode(cal
-00014540: 6c2c 2062 616e 642c 206d 6f64 6529 0a20  l, band, mode). 
-00014550: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00014560: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
-00014570: 203d 3d20 343a 0a20 2020 2020 2020 2020   == 4:.         
-00014580: 2020 2072 6573 756c 7420 3d20 7b22 6973     result = {"is
-00014590: 6475 7065 223a 2046 616c 7365 7d0a 2020  dupe": False}.  
-000145a0: 2020 2020 2020 6465 6275 676c 696e 6520        debugline 
-000145b0: 3d20 6622 7b72 6573 756c 747d 220a 2020  = f"{result}".  
-000145c0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000145d0: 7567 2822 2573 222c 2064 6562 7567 6c69  ug("%s", debugli
-000145e0: 6e65 290a 2020 2020 2020 2020 7265 7475  ne).        retu
-000145f0: 726e 2072 6573 756c 742e 6765 7428 2269  rn result.get("i
-00014600: 7364 7570 6522 2c20 4661 6c73 6529 0a0a  sdupe", False)..
-00014610: 2020 2020 6465 6620 7365 746d 6f64 6528      def setmode(
-00014620: 7365 6c66 2c20 6d6f 6465 3a20 7374 7229  self, mode: str)
-00014630: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00014640: 2020 2222 2273 7475 6220 666f 7220 7768    """stub for wh
-00014650: 656e 2074 6865 206d 6f64 6520 6368 616e  en the mode chan
-00014660: 6765 732e 2222 220a 2020 2020 2020 2020  ges.""".        
-00014670: 6966 206d 6f64 6520 3d3d 2022 4357 223a  if mode == "CW":
-00014680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014690: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
-000146a0: 6520 213d 2022 4357 223a 0a20 2020 2020  e != "CW":.     
-000146b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000146c0: 6375 7272 656e 745f 6d6f 6465 203d 2022  current_mode = "
-000146d0: 4357 220a 2020 2020 2020 2020 2020 2020  CW".            
-000146e0: 2020 2020 2320 7365 6c66 2e6d 6f64 652e      # self.mode.
-000146f0: 7365 7454 6578 7428 2243 5722 290a 2020  setText("CW").  
-00014700: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014710: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
-00014720: 2235 3939 2229 0a20 2020 2020 2020 2020  "599").         
-00014730: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
-00014740: 6976 652e 7365 7454 6578 7428 2235 3939  ive.setText("599
-00014750: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00014760: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
-00014770: 6d61 6372 6f73 2829 0a20 2020 2020 2020  macros().       
-00014780: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00014790: 2020 2020 6966 206d 6f64 6520 3d3d 2022      if mode == "
-000147a0: 5353 4222 3a0a 2020 2020 2020 2020 2020  SSB":.          
-000147b0: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
-000147c0: 745f 6d6f 6465 2021 3d20 2253 5342 223a  t_mode != "SSB":
-000147d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147e0: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
-000147f0: 6465 203d 2022 5353 4222 0a20 2020 2020  de = "SSB".     
-00014800: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00014810: 662e 6d6f 6465 2e73 6574 5465 7874 2822  f.mode.setText("
-00014820: 5353 4222 290a 2020 2020 2020 2020 2020  SSB").          
-00014830: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-00014840: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
-00014850: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014860: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
-00014870: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00014880: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00014890: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-000148a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000148b0: 6e0a 2020 2020 2020 2020 6966 206d 6f64  n.        if mod
-000148c0: 6520 3d3d 2022 5254 5459 223a 0a20 2020  e == "RTTY":.   
-000148d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000148e0: 2e63 7572 7265 6e74 5f6d 6f64 6520 213d  .current_mode !=
-000148f0: 2022 5254 5459 223a 0a20 2020 2020 2020   "RTTY":.       
-00014900: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00014910: 7272 656e 745f 6d6f 6465 203d 2022 5254  rrent_mode = "RT
-00014920: 5459 220a 2020 2020 2020 2020 2020 2020  TY".            
-00014930: 2020 2020 2320 7365 6c66 2e6d 6f64 652e      # self.mode.
-00014940: 7365 7454 6578 7428 2252 5454 5922 290a  setText("RTTY").
-00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014960: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
-00014970: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
-00014980: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00014990: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
-000149a0: 2229 0a0a 2020 2020 6465 6620 6765 745f  ")..    def get_
-000149b0: 6f70 6f6e 2873 656c 6629 3a0a 2020 2020  opon(self):.    
-000149c0: 2020 2020 2222 2243 7472 6c2b 4f20 6f72      """Ctrl+O or
-000149d0: 204f 504f 4e20 6469 616c 6f67 2222 220a   OPON dialog""".
-000149e0: 2020 2020 2020 2020 7365 6c66 2e6f 706f          self.opo
-000149f0: 6e5f 6469 616c 6f67 203d 204f 704f 6e28  n_dialog = OpOn(
-00014a00: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-00014a10: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
-00014a20: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-00014a30: 636f 6e6e 6563 7428 7365 6c66 2e6e 6577  connect(self.new
-00014a40: 5f6f 7029 0a20 2020 2020 2020 2073 656c  _op).        sel
-00014a50: 662e 6f70 6f6e 5f64 6961 6c6f 672e 6f70  f.opon_dialog.op
-00014a60: 656e 2829 0a0a 2020 2020 6465 6620 6e65  en()..    def ne
-00014a70: 775f 6f70 2873 656c 6629 3a0a 2020 2020  w_op(self):.    
-00014a80: 2020 2020 2222 2253 6176 6520 6e65 7720      """Save new 
-00014a90: 4f50 2222 220a 2020 2020 2020 2020 6966  OP""".        if
-00014aa0: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-00014ab0: 672e 4e65 774f 7065 7261 746f 722e 7465  g.NewOperator.te
-00014ac0: 7874 2829 3a0a 2020 2020 2020 2020 2020  xt():.          
-00014ad0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6f    self.current_o
-00014ae0: 7020 3d20 7365 6c66 2e6f 706f 6e5f 6469  p = self.opon_di
-00014af0: 616c 6f67 2e4e 6577 4f70 6572 6174 6f72  alog.NewOperator
-00014b00: 2e74 6578 7428 292e 7570 7065 7228 290a  .text().upper().
-00014b10: 2020 2020 2020 2020 7365 6c66 2e6f 706f          self.opo
-00014b20: 6e5f 6469 616c 6f67 2e63 6c6f 7365 2829  n_dialog.close()
-00014b30: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00014b40: 6465 6275 6728 224e 6577 204f 703a 2025  debug("New Op: %
-00014b50: 7322 2c20 7365 6c66 2e63 7572 7265 6e74  s", self.current
-00014b60: 5f6f 7029 0a20 2020 2020 2020 2073 656c  _op).        sel
-00014b70: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-00014b80: 0a20 2020 2064 6566 206d 616b 655f 6f70  .    def make_op
-00014b90: 5f64 6972 2873 656c 6629 3a0a 2020 2020  _dir(self):.    
-00014ba0: 2020 2020 2222 2243 7265 6174 6520 4f50      """Create OP
-00014bb0: 2064 6972 6563 746f 7279 2069 6620 6974   directory if it
-00014bc0: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-00014bd0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00014be0: 656c 662e 6375 7272 656e 745f 6f70 3a0a  elf.current_op:.
-00014bf0: 2020 2020 2020 2020 2020 2020 6f70 5f70              op_p
-00014c00: 6174 6820 3d20 5061 7468 2844 4154 415f  ath = Path(DATA_
-00014c10: 5041 5448 2920 2f20 7365 6c66 2e63 7572  PATH) / self.cur
-00014c20: 7265 6e74 5f6f 700a 2020 2020 2020 2020  rent_op.        
-00014c30: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00014c40: 2822 6f70 5f70 6174 683a 2025 7322 2c20  ("op_path: %s", 
-00014c50: 7374 7228 6f70 5f70 6174 6829 290a 2020  str(op_path)).  
-00014c60: 2020 2020 2020 2020 2020 6966 206f 705f            if op_
-00014c70: 7061 7468 2e69 735f 6469 7228 2920 6973  path.is_dir() is
-00014c80: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
-00014c90: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00014ca0: 6562 7567 2822 4372 6561 7469 6e67 204f  ebug("Creating O
-00014cb0: 7020 4469 7265 6374 6f72 793a 2025 7322  p Directory: %s"
-00014cc0: 2c20 7374 7228 6f70 5f70 6174 6829 290a  , str(op_path)).
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ce0: 6f73 2e6d 6b64 6972 2873 7472 286f 705f  os.mkdir(str(op_
-00014cf0: 7061 7468 2929 0a20 2020 2020 2020 2020  path)).         
-00014d00: 2020 2069 6620 6f70 5f70 6174 682e 6973     if op_path.is
-00014d10: 5f64 6972 2829 3a0a 2020 2020 2020 2020  _dir():.        
-00014d20: 2020 2020 2020 2020 736f 7572 6365 5f70          source_p
-00014d30: 6174 6820 3d20 5061 7468 2857 4f52 4b49  ath = Path(WORKI
-00014d40: 4e47 5f50 4154 4829 202f 2022 6461 7461  NG_PATH) / "data
-00014d50: 2220 2f20 2270 686f 6e65 7469 6373 220a  " / "phonetics".
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d70: 6c6f 6767 6572 2e64 6562 7567 2822 736f  logger.debug("so
-00014d80: 7572 6365 5f70 6174 683a 2025 7322 2c20  urce_path: %s", 
-00014d90: 7374 7228 736f 7572 6365 5f70 6174 6829  str(source_path)
-00014da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014db0: 2020 666f 7220 6368 696c 6420 696e 2073    for child in s
-00014dc0: 6f75 7263 655f 7061 7468 2e69 7465 7264  ource_path.iterd
-00014dd0: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
-00014de0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00014df0: 6174 696f 6e5f 6669 6c65 203d 206f 705f  ation_file = op_
-00014e00: 7061 7468 202f 2063 6869 6c64 2e6e 616d  path / child.nam
-00014e10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00014e20: 2020 2020 2020 6966 2064 6573 7469 6e61        if destina
-00014e30: 7469 6f6e 5f66 696c 652e 6973 5f66 696c  tion_file.is_fil
-00014e40: 6528 2920 6973 2046 616c 7365 3a0a 2020  e() is False:.  
-00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e60: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00014e70: 7567 2822 4465 7374 696e 6174 696f 6e3a  ug("Destination:
-00014e80: 2025 7322 2c20 7374 7228 6465 7374 696e   %s", str(destin
-00014e90: 6174 696f 6e5f 6669 6c65 2929 0a20 2020  ation_file)).   
-00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014eb0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00014ec0: 5f66 696c 652e 7772 6974 655f 6279 7465  _file.write_byte
-00014ed0: 7328 6368 696c 642e 7265 6164 5f62 7974  s(child.read_byt
-00014ee0: 6573 2829 290a 0a20 2020 2064 6566 2070  es())..    def p
-00014ef0: 6f6c 6c5f 7261 6469 6f28 7365 6c66 293a  oll_radio(self):
-00014f00: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-00014f10: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00014f20: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
-00014f30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014f40: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00014f50: 2e6f 6e6c 696e 6520 6973 2046 616c 7365  .online is False
-00014f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014f70: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-00014f80: 6f6c 2e72 6569 6e69 7428 290a 2020 2020  ol.reinit().    
-00014f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014fa0: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
-00014fb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00014fc0: 2020 2020 696e 666f 5f64 6972 7479 203d      info_dirty =
-00014fd0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00014fe0: 2020 2020 2020 2076 666f 203d 2073 656c         vfo = sel
-00014ff0: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
-00015000: 745f 7666 6f28 290a 2020 2020 2020 2020  t_vfo().        
-00015010: 2020 2020 2020 2020 6d6f 6465 203d 2073          mode = s
-00015020: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00015030: 6765 745f 6d6f 6465 2829 0a20 2020 2020  get_mode().     
-00015040: 2020 2020 2020 2020 2020 2062 7720 3d20             bw = 
-00015050: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00015060: 2e67 6574 5f62 7728 290a 2020 2020 2020  .get_bw().      
-00015070: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00015080: 2e72 6164 696f 5f73 7461 7465 5b22 7074  .radio_state["pt
-00015090: 7422 5d20 3d20 7365 6c66 2e72 6967 5f63  t"] = self.rig_c
-000150a0: 6f6e 7472 6f6c 2e67 6574 5f70 7474 2829  ontrol.get_ptt()
-000150b0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000150c0: 2020 6966 206d 6f64 6520 3d3d 2022 4357    if mode == "CW
-000150d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000150e0: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-000150f0: 6f64 6528 6d6f 6465 290a 2020 2020 2020  ode(mode).      
-00015100: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00015110: 6520 3d3d 2022 4c53 4222 206f 7220 6d6f  e == "LSB" or mo
-00015120: 6465 203d 3d20 2255 5342 223a 0a20 2020  de == "USB":.   
-00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015140: 2073 656c 662e 7365 746d 6f64 6528 2253   self.setmode("S
-00015150: 5342 2229 0a20 2020 2020 2020 2020 2020  SB").           
-00015160: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
-00015170: 2252 5454 5922 3a0a 2020 2020 2020 2020  "RTTY":.        
-00015180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015190: 2e73 6574 6d6f 6465 2822 5254 5459 2229  .setmode("RTTY")
-000151a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000151b0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
-000151c0: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-000151d0: 2920 213d 2076 666f 3a0a 2020 2020 2020  ) != vfo:.      
-000151e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000151f0: 666f 5f64 6972 7479 203d 2054 7275 650a  fo_dirty = True.
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-00015220: 7461 7465 5b22 7666 6f61 225d 203d 2076  tate["vfoa"] = v
-00015230: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
-00015240: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-00015250: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
-00015260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015270: 2e72 6164 696f 5f73 7461 7465 5b22 6261  .radio_state["ba
-00015280: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
-00015290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000152a0: 2e63 6f6e 7461 6374 5b22 4261 6e64 225d  .contact["Band"]
-000152b0: 203d 2067 6574 5f6c 6f67 6765 645f 6261   = get_logged_ba
-000152c0: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
-000152d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000152e0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
-000152f0: 6174 6f72 2862 616e 6429 0a0a 2020 2020  ator(band)..    
-00015300: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00015310: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00015320: 6765 7428 226d 6f64 6522 2920 213d 206d  get("mode") != m
-00015330: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
-00015340: 2020 2020 2020 2020 2069 6e66 6f5f 6469           info_di
-00015350: 7274 7920 3d20 5472 7565 0a20 2020 2020  rty = True.     
-00015360: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015370: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00015380: 226d 6f64 6522 5d20 3d20 6d6f 6465 0a0a  "mode"] = mode..
-00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153a0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-000153b0: 6174 652e 6765 7428 2262 7722 2920 213d  ate.get("bw") !=
-000153c0: 2062 773a 0a20 2020 2020 2020 2020 2020   bw:.           
-000153d0: 2020 2020 2020 2020 2069 6e66 6f5f 6469           info_di
-000153e0: 7274 7920 3d20 5472 7565 0a20 2020 2020  rty = True.     
-000153f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015400: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00015410: 2262 7722 5d20 3d20 6277 0a0a 2020 2020  "bw"] = bw..    
-00015420: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00015430: 6174 6574 696d 652e 6e6f 7728 2920 3e20  atetime.now() > 
-00015440: 676c 6f62 616c 7328 295b 2270 6f6c 6c5f  globals()["poll_
-00015450: 7469 6d65 225d 206f 7220 696e 666f 5f64  time"] or info_d
-00015460: 6972 7479 3a0a 2020 2020 2020 2020 2020  irty:.          
-00015470: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00015480: 2e64 6562 7567 2822 5646 4f3a 2025 7320  .debug("VFO: %s 
-00015490: 204d 4f44 453a 2025 7320 4257 3a20 2573   MODE: %s BW: %s
-000154a0: 222c 2076 666f 2c20 6d6f 6465 2c20 6277  ", vfo, mode, bw
-000154b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000154c0: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
-000154d0: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
-000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154f0: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-00015500: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015510: 6d64 5b22 636d 6422 5d20 3d20 2252 4144  md["cmd"] = "RAD
-00015520: 494f 5f53 5441 5445 220a 2020 2020 2020  IO_STATE".      
-00015530: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00015540: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-00015550: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2020 2063 6d64 5b22 6261 6e64 225d 203d     cmd["band"] =
-00015580: 2062 616e 640a 2020 2020 2020 2020 2020   band.          
-00015590: 2020 2020 2020 2020 2020 636d 645b 2276            cmd["v
-000155a0: 666f 6122 5d20 3d20 7666 6f0a 2020 2020  foa"] = vfo.    
+00012b50: 6574 6d6f 6465 2822 5353 4222 290a 2020  etmode("SSB").  
+00012b60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012b70: 2069 6e74 2873 656c 662e 7261 6469 6f5f   int(self.radio_
+00012b80: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+00012b90: 2c20 3029 2920 3e20 3130 3030 3030 3030  , 0)) > 10000000
+00012ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012bb0: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+00012bc0: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
+00012bd0: 2022 5553 4222 0a20 2020 2020 2020 2020   "USB".         
+00012be0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00012c10: 655b 226d 6f64 6522 5d20 3d20 224c 5342  e["mode"] = "LSB
+00012c20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012c30: 2020 6261 6e64 203d 2067 6574 6261 6e64    band = getband
+00012c40: 2873 7472 2873 656c 662e 7261 6469 6f5f  (str(self.radio_
+00012c50: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+00012c60: 2c20 2230 2e30 2229 2929 0a20 2020 2020  , "0.0"))).     
+00012c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012c80: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
+00012c90: 6f72 2862 616e 6429 0a20 2020 2020 2020  or(band).       
+00012ca0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00012cb0: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
+00012cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012cd0: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
+00012ce0: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
+00012cf0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00012d00: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
+00012d10: 6f64 6528 7365 6c66 2e72 6164 696f 5f73  ode(self.radio_s
+00012d20: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+00012d30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012d40: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+00012d50: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+00012d60: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
+00012d70: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
+00012d80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00012d90: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+00012da0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
+00012db0: 3d20 224f 504f 4e22 3a0a 2020 2020 2020  = "OPON":.      
+00012dc0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00012dd0: 6574 5f6f 706f 6e28 290a 2020 2020 2020  et_opon().      
+00012de0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00012df0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+00012e00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012e10: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00012e20: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
+00012e30: 203d 3d20 2248 454c 5022 3a0a 2020 2020   == "HELP":.    
+00012e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012e50: 2e73 686f 775f 6865 6c70 5f64 6961 6c6f  .show_help_dialo
+00012e60: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00012e70: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
+00012e80: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
+00012e90: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00012ea0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00012eb0: 6970 7065 645f 7465 7874 203d 3d20 2254  ipped_text == "T
+00012ec0: 4553 5422 3a0a 2020 2020 2020 2020 2020  EST":.          
+00012ed0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00012ee0: 656c 662e 6461 7461 6261 7365 2e67 6574  elf.database.get
+00012ef0: 5f63 616c 6c73 5f61 6e64 5f62 616e 6473  _calls_and_bands
+00012f00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012f10: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+00012f20: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00012f30: 2263 6d64 225d 203d 2022 574f 524b 4544  "cmd"] = "WORKED
+00012f40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012f50: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00012f60: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00012f70: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012f80: 2020 2063 6d64 5b22 776f 726b 6564 225d     cmd["worked"]
+00012f90: 203d 2072 6573 756c 740a 2020 2020 2020   = result.      
+00012fa0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00012fb0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+00012fc0: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+00012fd0: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
+00012fe0: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
+00012ff0: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
+00013000: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00013010: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00013020: 6c66 2e69 735f 666c 6f61 7461 626c 6528  lf.is_floatable(
+00013030: 7374 7269 7070 6564 5f74 6578 7429 3a0a  stripped_text):.
+00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013050: 7666 6f20 3d20 666c 6f61 7428 7374 7269  vfo = float(stri
+00013060: 7070 6564 5f74 6578 7429 0a20 2020 2020  pped_text).     
+00013070: 2020 2020 2020 2020 2020 2076 666f 203d             vfo =
+00013080: 2069 6e74 2876 666f 202a 2031 3030 3029   int(vfo * 1000)
+00013090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000130a0: 2062 616e 6420 3d20 6765 7462 616e 6428   band = getband(
+000130b0: 7374 7228 7666 6f29 290a 2020 2020 2020  str(vfo)).      
+000130c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000130d0: 6574 5f62 616e 645f 696e 6469 6361 746f  et_band_indicato
+000130e0: 7228 6261 6e64 290a 2020 2020 2020 2020  r(band).        
+000130f0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+00013100: 6f6e 7461 6374 5b22 4261 6e64 225d 203d  ontact["Band"] =
+00013110: 2067 6574 5f6c 6f67 6765 645f 6261 6e64   get_logged_band
+00013120: 2873 7472 2873 656c 662e 7261 6469 6f5f  (str(self.radio_
+00013130: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+00013140: 2c20 302e 3029 2929 0a20 2020 2020 2020  , 0.0))).       
+00013150: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00013160: 6469 6f5f 7374 6174 655b 2276 666f 6122  dio_state["vfoa"
+00013170: 5d20 3d20 7666 6f0a 2020 2020 2020 2020  ] = vfo.        
+00013180: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00013190: 696f 5f73 7461 7465 5b22 6261 6e64 225d  io_state["band"]
+000131a0: 203d 2062 616e 640a 2020 2020 2020 2020   = band.        
+000131b0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000131c0: 7461 6374 5b22 4261 6e64 225d 203d 2067  tact["Band"] = g
+000131d0: 6574 5f6c 6f67 6765 645f 6261 6e64 2873  et_logged_band(s
+000131e0: 7472 2876 666f 2929 0a20 2020 2020 2020  tr(vfo)).       
+000131f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00013200: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
+00013210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013220: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00013230: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00013240: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00013250: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+00013260: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013270: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
+00013280: 745f 7666 6f28 7666 6f29 0a20 2020 2020  t_vfo(vfo).     
+00013290: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000132a0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+000132b0: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000132d0: 6d64 5b22 636d 6422 5d20 3d20 2252 4144  md["cmd"] = "RAD
+000132e0: 494f 5f53 5441 5445 220a 2020 2020 2020  IO_STATE".      
+000132f0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00013300: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00013310: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00013320: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00013330: 6261 6e64 225d 203d 2062 616e 640a 2020  band"] = band.  
+00013340: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00013350: 645b 2276 666f 6122 5d20 3d20 7666 6f0a  d["vfoa"] = vfo.
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00013380: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00013390: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+000133a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000133b0: 6e0a 0a20 2020 2020 2020 2020 2020 2073  n..            s
+000133c0: 656c 662e 6368 6563 6b5f 6361 6c6c 7369  elf.check_callsi
+000133d0: 676e 2873 7472 6970 7065 645f 7465 7874  gn(stripped_text
+000133e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000133f0: 2073 656c 662e 6368 6563 6b5f 6475 7065   self.check_dupe
+00013400: 2873 7472 6970 7065 645f 7465 7874 293a  (stripped_text):
+00013410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013420: 2073 656c 662e 6475 7065 5f69 6e64 6963   self.dupe_indic
+00013430: 6174 6f72 2e73 686f 7728 290a 2020 2020  ator.show().    
+00013440: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00013450: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013460: 6c66 2e64 7570 655f 696e 6469 6361 746f  lf.dupe_indicato
+00013470: 722e 6869 6465 2829 0a20 2020 2020 2020  r.hide().       
+00013480: 2020 2020 205f 7468 6574 6872 6561 6420       _thethread 
+00013490: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
+000134a0: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
+000134b0: 2020 2020 7461 7267 6574 3d73 656c 662e      target=self.
+000134c0: 6368 6563 6b5f 6361 6c6c 7369 676e 322c  check_callsign2,
+000134d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000134e0: 2061 7267 733d 2874 6578 742c 292c 0a20   args=(text,),. 
+000134f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00013500: 6165 6d6f 6e3d 5472 7565 2c0a 2020 2020  aemon=True,.    
+00013510: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013520: 2020 2020 2020 5f74 6865 7468 7265 6164        _thethread
+00013530: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
+00013540: 2020 2020 2073 656c 662e 6e65 7874 5f66       self.next_f
+00013550: 6965 6c64 2e73 6574 466f 6375 7328 290a  ield.setFocus().
+00013560: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013570: 726e 0a20 2020 2020 2020 2063 6d64 203d  rn.        cmd =
+00013580: 207b 7d0a 2020 2020 2020 2020 636d 645b   {}.        cmd[
+00013590: 2263 6d64 225d 203d 2022 4341 4c4c 4348  "cmd"] = "CALLCH
+000135a0: 414e 4745 4422 0a20 2020 2020 2020 2063  ANGED".        c
+000135b0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+000135c0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+000135d0: 2020 2020 2020 2020 636d 645b 2263 616c          cmd["cal
+000135e0: 6c22 5d20 3d20 7374 7269 7070 6564 5f74  l"] = stripped_t
+000135f0: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
+00013600: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+00013610: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+00013620: 6e28 636d 6429 0a20 2020 2020 2020 2073  n(cmd).        s
+00013630: 656c 662e 6368 6563 6b5f 6361 6c6c 7369  elf.check_callsi
+00013640: 676e 2873 7472 6970 7065 645f 7465 7874  gn(stripped_text
+00013650: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
+00013660: 5f63 616c 6c73 6967 6e28 7365 6c66 2c20  _callsign(self, 
+00013670: 6361 6c6c 7369 676e 293a 0a20 2020 2020  callsign):.     
+00013680: 2020 2022 2222 4368 6563 6b20 6361 6c6c     """Check call
+00013690: 2061 7320 656e 7465 7265 6422 2222 0a20   as entered""". 
+000136a0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000136b0: 7365 6c66 2e63 7479 5f6c 6f6f 6b75 7028  self.cty_lookup(
+000136c0: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
+000136d0: 2020 6465 6275 675f 7265 7375 6c74 203d    debug_result =
+000136e0: 2066 227b 7265 7375 6c74 7d22 0a20 2020   f"{result}".   
+000136f0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00013700: 6728 2225 7322 2c20 6465 6275 675f 7265  g("%s", debug_re
+00013710: 7375 6c74 290a 2020 2020 2020 2020 6966  sult).        if
+00013720: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
+00013730: 2020 2020 2066 6f72 2061 2069 6e20 7265       for a in re
+00013740: 7375 6c74 2e69 7465 6d73 2829 3a0a 2020  sult.items():.  
+00013750: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00013760: 7469 7479 203d 2061 5b31 5d2e 6765 7428  tity = a[1].get(
+00013770: 2265 6e74 6974 7922 2c20 2222 290a 2020  "entity", "").  
+00013780: 2020 2020 2020 2020 2020 2020 2020 6371                cq
+00013790: 203d 2061 5b31 5d2e 6765 7428 2263 7122   = a[1].get("cq"
+000137a0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+000137b0: 2020 2020 2020 6974 7520 3d20 615b 315d        itu = a[1]
+000137c0: 2e67 6574 2822 6974 7522 2c20 2222 290a  .get("itu", "").
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137e0: 636f 6e74 696e 656e 7420 3d20 615b 315d  continent = a[1]
+000137f0: 2e67 6574 2822 636f 6e74 696e 656e 7422  .get("continent"
+00013800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013810: 2020 6c61 7420 3d20 666c 6f61 7428 615b    lat = float(a[
+00013820: 315d 2e67 6574 2822 6c61 7422 2c20 2230  1].get("lat", "0
+00013830: 2e30 2229 290a 2020 2020 2020 2020 2020  .0")).          
+00013840: 2020 2020 2020 6c6f 6e20 3d20 666c 6f61        lon = floa
+00013850: 7428 615b 315d 2e67 6574 2822 6c6f 6e67  t(a[1].get("long
+00013860: 222c 2022 302e 3022 2929 0a20 2020 2020  ", "0.0")).     
+00013870: 2020 2020 2020 2020 2020 206c 6f6e 203d             lon =
+00013880: 206c 6f6e 202a 202d 3120 2023 2063 7479   lon * -1  # cty
+00013890: 2e64 6174 2066 696c 6520 696e 7665 7274  .dat file invert
+000138a0: 7320 6c6f 6e67 6974 7564 6573 0a20 2020  s longitudes.   
+000138b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000138c0: 6d61 7279 5f70 6678 203d 2061 5b31 5d2e  mary_pfx = a[1].
+000138d0: 6765 7428 2270 7269 6d61 7279 5f70 6678  get("primary_pfx
+000138e0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
+000138f0: 2020 2020 2020 2068 6561 6469 6e67 203d         heading =
+00013900: 2062 6561 7269 6e67 5f77 6974 685f 6c61   bearing_with_la
+00013910: 746c 6f6e 2873 656c 662e 7374 6174 696f  tlon(self.statio
+00013920: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
+00013930: 6522 292c 206c 6174 2c20 6c6f 6e29 0a20  e"), lat, lon). 
+00013940: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00013950: 696c 6f6d 6574 6572 7320 3d20 6469 7374  ilometers = dist
+00013960: 616e 6365 5f77 6974 685f 6c61 746c 6f6e  ance_with_latlon
+00013970: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013980: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+00013990: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
+000139a0: 7265 2229 2c20 6c61 742c 206c 6f6e 0a20  re"), lat, lon. 
+000139b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000139c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000139d0: 2073 656c 662e 6865 6164 696e 675f 6469   self.heading_di
+000139e0: 7374 616e 6365 2e73 6574 5465 7874 280a  stance.setText(.
+000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a00: 2020 2020 6622 5265 6769 6f6e 616c 2048      f"Regional H
+00013a10: 6467 207b 6865 6164 696e 677d c2b0 204c  dg {heading}.. L
+00013a20: 5020 7b72 6563 6970 726f 636f 6c28 6865  P {reciprocol(he
+00013a30: 6164 696e 6729 7dc2 b020 2f20 220a 2020  ading)}.. / ".  
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 2020 6622 6469 7374 616e 6365 207b 696e    f"distance {in
+00013a60: 7428 6b69 6c6f 6d65 7465 7273 2a30 2e36  t(kilometers*0.6
+00013a70: 3231 3337 3129 7d6d 6920 7b6b 696c 6f6d  21371)}mi {kilom
+00013a80: 6574 6572 737d 6b6d 220a 2020 2020 2020  eters}km".      
+00013a90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013ab0: 2e63 6f6e 7461 6374 5b22 436f 756e 7472  .contact["Countr
+00013ac0: 7950 7265 6669 7822 5d20 3d20 7072 696d  yPrefix"] = prim
+00013ad0: 6172 795f 7066 780a 2020 2020 2020 2020  ary_pfx.        
+00013ae0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00013af0: 7461 6374 5b22 5a4e 225d 203d 2069 6e74  tact["ZN"] = int
+00013b00: 2863 7129 0a20 2020 2020 2020 2020 2020  (cq).           
+00013b10: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00013b20: 745b 2243 6f6e 7469 6e65 6e74 225d 203d  t["Continent"] =
+00013b30: 2063 6f6e 7469 6e65 6e74 0a20 2020 2020   continent.     
+00013b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013b50: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
+00013b60: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00013b70: 2020 2020 2020 2066 227b 7072 696d 6172         f"{primar
+00013b80: 795f 7066 787d 3a20 7b63 6f6e 7469 6e65  y_pfx}: {contine
+00013b90: 6e74 7d2f 7b65 6e74 6974 797d 2063 713a  nt}/{entity} cq:
+00013ba0: 7b63 717d 2069 7475 3a7b 6974 757d 220a  {cq} itu:{itu}".
+00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013bd0: 2020 6966 206c 656e 2863 616c 6c73 6967    if len(callsig
+00013be0: 6e29 203e 2032 3a0a 2020 2020 2020 2020  n) > 2:.        
+00013bf0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00013c00: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c20: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00013c30: 742e 7072 6566 696c 6c28 7365 6c66 290a  t.prefill(self).
+00013c40: 0a20 2020 2064 6566 2063 6865 636b 5f63  .    def check_c
+00013c50: 616c 6c73 6967 6e32 2873 656c 662c 2063  allsign2(self, c
+00013c60: 616c 6c73 6967 6e29 3a0a 2020 2020 2020  allsign):.      
+00013c70: 2020 2222 2243 6865 636b 2063 616c 6c20    """Check call 
+00013c80: 6f6e 6365 2065 6e74 6572 6564 2222 220a  once entered""".
+00013c90: 2020 2020 2020 2020 6361 6c6c 7369 676e          callsign
+00013ca0: 203d 2063 616c 6c73 6967 6e2e 7374 7269   = callsign.stri
+00013cb0: 7028 290a 2020 2020 2020 2020 6465 6275  p().        debu
+00013cc0: 675f 6c6f 6f6b 7570 203d 2066 227b 7365  g_lookup = f"{se
+00013cd0: 6c66 2e6c 6f6f 6b5f 7570 7d22 0a20 2020  lf.look_up}".   
+00013ce0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00013cf0: 6728 2225 732c 2025 7322 2c20 6361 6c6c  g("%s, %s", call
+00013d00: 7369 676e 2c20 6465 6275 675f 6c6f 6f6b  sign, debug_look
+00013d10: 7570 290a 2020 2020 2020 2020 6966 2068  up).        if h
+00013d20: 6173 6174 7472 2873 656c 662e 6c6f 6f6b  asattr(self.look
+00013d30: 5f75 702c 2022 7365 7373 696f 6e22 293a  _up, "session"):
+00013d40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013d50: 7365 6c66 2e6c 6f6f 6b5f 7570 2e73 6573  self.look_up.ses
+00013d60: 7369 6f6e 3a0a 2020 2020 2020 2020 2020  sion:.          
+00013d70: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00013d80: 2073 656c 662e 6c6f 6f6b 5f75 702e 6c6f   self.look_up.lo
+00013d90: 6f6b 7570 2863 616c 6c73 6967 6e29 0a20  okup(callsign). 
+00013da0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00013db0: 6562 7567 5f72 6573 706f 6e73 6520 3d20  ebug_response = 
+00013dc0: 6622 7b72 6573 706f 6e73 657d 220a 2020  f"{response}".  
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00013de0: 6767 6572 2e64 6562 7567 2822 5468 6520  gger.debug("The 
+00013df0: 5265 7370 6f6e 7365 3a20 2573 5c6e 222c  Response: %s\n",
+00013e00: 2064 6562 7567 5f72 6573 706f 6e73 6529   debug_response)
+00013e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e20: 2069 6620 7265 7370 6f6e 7365 3a0a 2020   if response:.  
+00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e40: 2020 7468 6569 7267 7269 6420 3d20 7265    theirgrid = re
+00013e50: 7370 6f6e 7365 2e67 6574 2822 6772 6964  sponse.get("grid
+00013e60: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00013e70: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00013e80: 6163 745b 2247 7269 6453 7175 6172 6522  act["GridSquare"
+00013e90: 5d20 3d20 7468 6569 7267 7269 640a 2020  ] = theirgrid.  
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 5f74 6865 6972 636f 756e 7472 7920    _theircountry 
+00013ec0: 3d20 7265 7370 6f6e 7365 2e67 6574 2822  = response.get("
+00013ed0: 636f 756e 7472 7922 290a 2020 2020 2020  country").      
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013ef0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+00013f00: 7428 2247 7269 6453 7175 6172 6522 2c20  t("GridSquare", 
+00013f10: 2222 293a 0a20 2020 2020 2020 2020 2020  ""):.           
+00013f20: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+00013f30: 6469 6e67 203d 2062 6561 7269 6e67 2873  ding = bearing(s
+00013f40: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00013f50: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
+00013f60: 292c 2074 6865 6972 6772 6964 290a 2020  ), theirgrid).  
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f80: 2020 2020 2020 6b69 6c6f 6d65 7465 7273        kilometers
+00013f90: 203d 2064 6973 7461 6e63 6528 7365 6c66   = distance(self
+00013fa0: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
+00013fb0: 6964 5371 7561 7265 2229 2c20 7468 6569  idSquare"), thei
+00013fc0: 7267 7269 6429 0a20 2020 2020 2020 2020  rgrid).         
+00013fd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013fe0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
+00013ff0: 616e 6365 2e73 6574 5465 7874 280a 2020  ance.setText(.  
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 2020 2020 2020 2020 2020 6622 7b74 6865            f"{the
+00014020: 6972 6772 6964 7d20 4864 6720 7b68 6561  irgrid} Hdg {hea
+00014030: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
+00014040: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
+00014050: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
+00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014070: 2020 2066 2264 6973 7461 6e63 6520 7b69     f"distance {i
+00014080: 6e74 286b 696c 6f6d 6574 6572 732a 302e  nt(kilometers*0.
+00014090: 3632 3133 3731 297d 6d69 207b 6b69 6c6f  621371)}mi {kilo
+000140a0: 6d65 7465 7273 7d6b 6d22 0a20 2020 2020  meters}km".     
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000140d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+000140e0: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
+000140f0: 7428 6622 7b74 6865 6972 636f 756e 7472  t(f"{theircountr
+00014100: 797d 2229 0a20 2020 2020 2020 2020 2020  y}").           
+00014110: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+00014120: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00014130: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
+00014140: 616e 6365 2e73 6574 5465 7874 2822 4c6f  ance.setText("Lo
+00014150: 6f6b 7570 2066 6169 6c65 642e 2229 0a0a  okup failed.")..
+00014160: 2020 2020 6465 6620 6368 6563 6b5f 6475      def check_du
+00014170: 7065 2873 656c 662c 2063 616c 6c3a 2073  pe(self, call: s
+00014180: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
+00014190: 2020 2020 2022 2222 4368 6563 6b73 2069       """Checks i
+000141a0: 6620 6120 6361 6c6c 7369 676e 2069 7320  f a callsign is 
+000141b0: 6120 6475 7065 206f 6e20 6375 7272 656e  a dupe on curren
+000141c0: 7420 6261 6e64 2f6d 6f64 652e 2222 220a  t band/mode.""".
+000141d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000141e0: 636f 6e74 6573 7420 6973 204e 6f6e 653a  contest is None:
+000141f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014200: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
+00014210: 6f78 2822 596f 7520 6861 7665 206e 6f20  ox("You have no 
+00014220: 636f 6e74 6573 7420 6c6f 6164 6564 2e22  contest loaded."
+00014230: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00014240: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00014250: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+00014260: 7072 6564 7570 6528 7365 6c66 290a 2020  predupe(self).  
+00014270: 2020 2020 2020 6261 6e64 203d 2066 6c6f        band = flo
+00014280: 6174 2867 6574 5f6c 6f67 6765 645f 6261  at(get_logged_ba
+00014290: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
+000142a0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+000142b0: 6122 2c20 302e 3029 2929 290a 2020 2020  a", 0.0)))).    
+000142c0: 2020 2020 6d6f 6465 203d 2073 656c 662e      mode = self.
+000142d0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+000142e0: 226d 6f64 6522 2c20 2222 290a 2020 2020  "mode", "").    
+000142f0: 2020 2020 6465 6275 676c 696e 6520 3d20      debugline = 
+00014300: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00014310: 4361 6c6c 3a20 7b63 616c 6c7d 2042 616e  Call: {call} Ban
+00014320: 643a 207b 6261 6e64 7d20 4d6f 6465 3a20  d: {band} Mode: 
+00014330: 7b6d 6f64 657d 2044 7570 6574 7970 653a  {mode} Dupetype:
+00014340: 207b 7365 6c66 2e63 6f6e 7465 7374 2e64   {self.contest.d
+00014350: 7570 655f 7479 7065 7d22 0a20 2020 2020  upe_type}".     
+00014360: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
+00014370: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+00014380: 6465 6275 676c 696e 6529 0a20 2020 2020  debugline).     
+00014390: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+000143a0: 7374 2e64 7570 655f 7479 7065 203d 3d20  st.dupe_type == 
+000143b0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000143c0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
+000143d0: 6162 6173 652e 6368 6563 6b5f 6475 7065  abase.check_dupe
+000143e0: 2863 616c 6c29 0a20 2020 2020 2020 2069  (call).        i
+000143f0: 6620 7365 6c66 2e63 6f6e 7465 7374 2e64  f self.contest.d
+00014400: 7570 655f 7479 7065 203d 3d20 323a 0a20  upe_type == 2:. 
+00014410: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00014420: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
+00014430: 652e 6368 6563 6b5f 6475 7065 5f6f 6e5f  e.check_dupe_on_
+00014440: 6261 6e64 2863 616c 6c2c 2062 616e 6429  band(call, band)
+00014450: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00014460: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+00014470: 7065 203d 3d20 333a 0a20 2020 2020 2020  pe == 3:.       
+00014480: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00014490: 6c66 2e64 6174 6162 6173 652e 6368 6563  lf.database.chec
+000144a0: 6b5f 6475 7065 5f6f 6e5f 6261 6e64 5f6d  k_dupe_on_band_m
+000144b0: 6f64 6528 6361 6c6c 2c20 6261 6e64 2c20  ode(call, band, 
+000144c0: 6d6f 6465 290a 2020 2020 2020 2020 6966  mode).        if
+000144d0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
+000144e0: 7065 5f74 7970 6520 3d3d 2034 3a0a 2020  pe_type == 4:.  
+000144f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00014500: 203d 207b 2269 7364 7570 6522 3a20 4661   = {"isdupe": Fa
+00014510: 6c73 657d 0a20 2020 2020 2020 2064 6562  lse}.        deb
+00014520: 7567 6c69 6e65 203d 2066 227b 7265 7375  ugline = f"{resu
+00014530: 6c74 7d22 0a20 2020 2020 2020 206c 6f67  lt}".        log
+00014540: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+00014550: 6465 6275 676c 696e 6529 0a20 2020 2020  debugline).     
+00014560: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00014570: 2e67 6574 2822 6973 6475 7065 222c 2046  .get("isdupe", F
+00014580: 616c 7365 290a 0a20 2020 2064 6566 2073  alse)..    def s
+00014590: 6574 6d6f 6465 2873 656c 662c 206d 6f64  etmode(self, mod
+000145a0: 653a 2073 7472 2920 2d3e 204e 6f6e 653a  e: str) -> None:
+000145b0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+000145c0: 2066 6f72 2077 6865 6e20 7468 6520 6d6f   for when the mo
+000145d0: 6465 2063 6861 6e67 6573 2e22 2222 0a20  de changes.""". 
+000145e0: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+000145f0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00014600: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
+00014610: 656e 745f 6d6f 6465 2021 3d20 2243 5722  ent_mode != "CW"
+00014620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014630: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
+00014640: 6f64 6520 3d20 2243 5722 0a20 2020 2020  ode = "CW".     
+00014650: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00014660: 662e 6d6f 6465 2e73 6574 5465 7874 2822  f.mode.setText("
+00014670: 4357 2229 0a20 2020 2020 2020 2020 2020  CW").           
+00014680: 2020 2020 2073 656c 662e 7365 6e74 2e73       self.sent.s
+00014690: 6574 5465 7874 2822 3539 3922 290a 2020  etText("599").  
+000146a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000146b0: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+000146c0: 7874 2822 3539 3922 290a 2020 2020 2020  xt("599").      
+000146d0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000146e0: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+000146f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014700: 726e 0a20 2020 2020 2020 2069 6620 6d6f  rn.        if mo
+00014710: 6465 203d 3d20 2253 5342 223a 0a20 2020  de == "SSB":.   
+00014720: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00014730: 2e63 7572 7265 6e74 5f6d 6f64 6520 213d  .current_mode !=
+00014740: 2022 5353 4222 3a0a 2020 2020 2020 2020   "SSB":.        
+00014750: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
+00014760: 7265 6e74 5f6d 6f64 6520 3d20 2253 5342  rent_mode = "SSB
+00014770: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00014780: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00014790: 7454 6578 7428 2253 5342 2229 0a20 2020  tText("SSB").   
+000147a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000147b0: 662e 7365 6e74 2e73 6574 5465 7874 2822  f.sent.setText("
+000147c0: 3539 2229 0a20 2020 2020 2020 2020 2020  59").           
+000147d0: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
+000147e0: 652e 7365 7454 6578 7428 2235 3922 290a  e.setText("59").
+000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014800: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
+00014810: 726f 7328 290a 2020 2020 2020 2020 2020  ros().          
+00014820: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00014830: 2069 6620 6d6f 6465 203d 3d20 2252 5454   if mode == "RTT
+00014840: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
+00014850: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
+00014860: 6d6f 6465 2021 3d20 2252 5454 5922 3a0a  mode != "RTTY":.
+00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014880: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
+00014890: 6520 3d20 2252 5454 5922 0a20 2020 2020  e = "RTTY".     
+000148a0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+000148b0: 662e 6d6f 6465 2e73 6574 5465 7874 2822  f.mode.setText("
+000148c0: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
+000148d0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+000148e0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+000148f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014900: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
+00014910: 6578 7428 2235 3922 290a 0a20 2020 2064  ext("59")..    d
+00014920: 6566 2067 6574 5f6f 706f 6e28 7365 6c66  ef get_opon(self
+00014930: 293a 0a20 2020 2020 2020 2022 2222 4374  ):.        """Ct
+00014940: 726c 2b4f 206f 7220 4f50 4f4e 2064 6961  rl+O or OPON dia
+00014950: 6c6f 6722 2222 0a20 2020 2020 2020 2073  log""".        s
+00014960: 656c 662e 6f70 6f6e 5f64 6961 6c6f 6720  elf.opon_dialog 
+00014970: 3d20 4f70 4f6e 2857 4f52 4b49 4e47 5f50  = OpOn(WORKING_P
+00014980: 4154 4829 0a20 2020 2020 2020 2073 656c  ATH).        sel
+00014990: 662e 6f70 6f6e 5f64 6961 6c6f 672e 6163  f.opon_dialog.ac
+000149a0: 6365 7074 6564 2e63 6f6e 6e65 6374 2873  cepted.connect(s
+000149b0: 656c 662e 6e65 775f 6f70 290a 2020 2020  elf.new_op).    
+000149c0: 2020 2020 7365 6c66 2e6f 706f 6e5f 6469      self.opon_di
+000149d0: 616c 6f67 2e6f 7065 6e28 290a 0a20 2020  alog.open()..   
+000149e0: 2064 6566 206e 6577 5f6f 7028 7365 6c66   def new_op(self
+000149f0: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
+00014a00: 7665 206e 6577 204f 5022 2222 0a20 2020  ve new OP""".   
+00014a10: 2020 2020 2069 6620 7365 6c66 2e6f 706f       if self.opo
+00014a20: 6e5f 6469 616c 6f67 2e4e 6577 4f70 6572  n_dialog.NewOper
+00014a30: 6174 6f72 2e74 6578 7428 293a 0a20 2020  ator.text():.   
+00014a40: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
+00014a50: 7272 656e 745f 6f70 203d 2073 656c 662e  rrent_op = self.
+00014a60: 6f70 6f6e 5f64 6961 6c6f 672e 4e65 774f  opon_dialog.NewO
+00014a70: 7065 7261 746f 722e 7465 7874 2829 2e75  perator.text().u
+00014a80: 7070 6572 2829 0a20 2020 2020 2020 2073  pper().        s
+00014a90: 656c 662e 6f70 6f6e 5f64 6961 6c6f 672e  elf.opon_dialog.
+00014aa0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+00014ab0: 6c6f 6767 6572 2e64 6562 7567 2822 4e65  logger.debug("Ne
+00014ac0: 7720 4f70 3a20 2573 222c 2073 656c 662e  w Op: %s", self.
+00014ad0: 6375 7272 656e 745f 6f70 290a 2020 2020  current_op).    
+00014ae0: 2020 2020 7365 6c66 2e6d 616b 655f 6f70      self.make_op
+00014af0: 5f64 6972 2829 0a0a 2020 2020 6465 6620  _dir()..    def 
+00014b00: 6d61 6b65 5f6f 705f 6469 7228 7365 6c66  make_op_dir(self
+00014b10: 293a 0a20 2020 2020 2020 2022 2222 4372  ):.        """Cr
+00014b20: 6561 7465 204f 5020 6469 7265 6374 6f72  eate OP director
+00014b30: 7920 6966 2069 7420 646f 6573 206e 6f74  y if it does not
+00014b40: 2065 7869 7374 2e22 2222 0a20 2020 2020   exist.""".     
+00014b50: 2020 2069 6620 7365 6c66 2e63 7572 7265     if self.curre
+00014b60: 6e74 5f6f 703a 0a20 2020 2020 2020 2020  nt_op:.         
+00014b70: 2020 206f 705f 7061 7468 203d 2050 6174     op_path = Pat
+00014b80: 6828 4441 5441 5f50 4154 4829 202f 2073  h(DATA_PATH) / s
+00014b90: 656c 662e 6375 7272 656e 745f 6f70 0a20  elf.current_op. 
+00014ba0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00014bb0: 722e 6465 6275 6728 226f 705f 7061 7468  r.debug("op_path
+00014bc0: 3a20 2573 222c 2073 7472 286f 705f 7061  : %s", str(op_pa
+00014bd0: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
+00014be0: 2069 6620 6f70 5f70 6174 682e 6973 5f64   if op_path.is_d
+00014bf0: 6972 2829 2069 7320 4661 6c73 653a 0a20  ir() is False:. 
+00014c00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00014c10: 6f67 6765 722e 6465 6275 6728 2243 7265  ogger.debug("Cre
+00014c20: 6174 696e 6720 4f70 2044 6972 6563 746f  ating Op Directo
+00014c30: 7279 3a20 2573 222c 2073 7472 286f 705f  ry: %s", str(op_
+00014c40: 7061 7468 2929 0a20 2020 2020 2020 2020  path)).         
+00014c50: 2020 2020 2020 206f 732e 6d6b 6469 7228         os.mkdir(
+00014c60: 7374 7228 6f70 5f70 6174 6829 290a 2020  str(op_path)).  
+00014c70: 2020 2020 2020 2020 2020 6966 206f 705f            if op_
+00014c80: 7061 7468 2e69 735f 6469 7228 293a 0a20  path.is_dir():. 
+00014c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014ca0: 6f75 7263 655f 7061 7468 203d 2050 6174  ource_path = Pat
+00014cb0: 6828 574f 524b 494e 475f 5041 5448 2920  h(WORKING_PATH) 
+00014cc0: 2f20 2264 6174 6122 202f 2022 7068 6f6e  / "data" / "phon
+00014cd0: 6574 6963 7322 0a20 2020 2020 2020 2020  etics".         
+00014ce0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00014cf0: 6275 6728 2273 6f75 7263 655f 7061 7468  bug("source_path
+00014d00: 3a20 2573 222c 2073 7472 2873 6f75 7263  : %s", str(sourc
+00014d10: 655f 7061 7468 2929 0a20 2020 2020 2020  e_path)).       
+00014d20: 2020 2020 2020 2020 2066 6f72 2063 6869           for chi
+00014d30: 6c64 2069 6e20 736f 7572 6365 5f70 6174  ld in source_pat
+00014d40: 682e 6974 6572 6469 7228 293a 0a20 2020  h.iterdir():.   
+00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d60: 2064 6573 7469 6e61 7469 6f6e 5f66 696c   destination_fil
+00014d70: 6520 3d20 6f70 5f70 6174 6820 2f20 6368  e = op_path / ch
+00014d80: 696c 642e 6e61 6d65 0a20 2020 2020 2020  ild.name.       
+00014d90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014da0: 6465 7374 696e 6174 696f 6e5f 6669 6c65  destination_file
+00014db0: 2e69 735f 6669 6c65 2829 2069 7320 4661  .is_file() is Fa
+00014dc0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014dd0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00014de0: 6765 722e 6465 6275 6728 2244 6573 7469  ger.debug("Desti
+00014df0: 6e61 7469 6f6e 3a20 2573 222c 2073 7472  nation: %s", str
+00014e00: 2864 6573 7469 6e61 7469 6f6e 5f66 696c  (destination_fil
+00014e10: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00014e20: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00014e30: 696e 6174 696f 6e5f 6669 6c65 2e77 7269  ination_file.wri
+00014e40: 7465 5f62 7974 6573 2863 6869 6c64 2e72  te_bytes(child.r
+00014e50: 6561 645f 6279 7465 7328 2929 0a0a 2020  ead_bytes())..  
+00014e60: 2020 6465 6620 706f 6c6c 5f72 6164 696f    def poll_radio
+00014e70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014e80: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+00014e90: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00014ea0: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
+00014eb0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00014ec0: 636f 6e74 726f 6c2e 6f6e 6c69 6e65 2069  control.online i
+00014ed0: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
+00014ee0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00014ef0: 675f 636f 6e74 726f 6c2e 7265 696e 6974  g_control.reinit
+00014f00: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00014f10: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+00014f20: 6f6c 2e6f 6e6c 696e 653a 0a20 2020 2020  ol.online:.     
+00014f30: 2020 2020 2020 2020 2020 2069 6e66 6f5f             info_
+00014f40: 6469 7274 7920 3d20 4661 6c73 650a 2020  dirty = False.  
+00014f50: 2020 2020 2020 2020 2020 2020 2020 7666                vf
+00014f60: 6f20 3d20 7365 6c66 2e72 6967 5f63 6f6e  o = self.rig_con
+00014f70: 7472 6f6c 2e67 6574 5f76 666f 2829 0a20  trol.get_vfo(). 
+00014f80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00014f90: 6f64 6520 3d20 7365 6c66 2e72 6967 5f63  ode = self.rig_c
+00014fa0: 6f6e 7472 6f6c 2e67 6574 5f6d 6f64 6528  ontrol.get_mode(
+00014fb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014fc0: 2020 6277 203d 2073 656c 662e 7269 675f    bw = self.rig_
+00014fd0: 636f 6e74 726f 6c2e 6765 745f 6277 2829  control.get_bw()
+00014fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ff0: 2023 2073 656c 662e 7261 6469 6f5f 7374   # self.radio_st
+00015000: 6174 655b 2270 7474 225d 203d 2073 656c  ate["ptt"] = sel
+00015010: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
+00015020: 745f 7074 7428 290a 0a20 2020 2020 2020  t_ptt()..       
+00015030: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
+00015040: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+00015050: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015060: 6c66 2e73 6574 6d6f 6465 286d 6f64 6529  lf.setmode(mode)
+00015070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015080: 2069 6620 6d6f 6465 203d 3d20 224c 5342   if mode == "LSB
+00015090: 2220 6f72 206d 6f64 6520 3d3d 2022 5553  " or mode == "US
+000150a0: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+000150b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000150c0: 6d6f 6465 2822 5353 4222 290a 2020 2020  mode("SSB").    
+000150d0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+000150e0: 6f64 6520 3d3d 2022 5254 5459 223a 0a20  ode == "RTTY":. 
+000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015100: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+00015110: 2252 5454 5922 290a 0a20 2020 2020 2020  "RTTY")..       
+00015120: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00015130: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00015140: 2822 7666 6f61 2229 2021 3d20 7666 6f3a  ("vfoa") != vfo:
+00015150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015160: 2020 2020 2069 6e66 6f5f 6469 7274 7920       info_dirty 
+00015170: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+00015180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015190: 7261 6469 6f5f 7374 6174 655b 2276 666f  radio_state["vfo
+000151a0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+000151b0: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
+000151c0: 2067 6574 6261 6e64 2873 7472 2876 666f   getband(str(vfo
+000151d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000151e0: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+000151f0: 6174 655b 2262 616e 6422 5d20 3d20 6261  ate["band"] = ba
+00015200: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00015210: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00015220: 2242 616e 6422 5d20 3d20 6765 745f 6c6f  "Band"] = get_lo
+00015230: 6767 6564 5f62 616e 6428 7374 7228 7666  gged_band(str(vf
+00015240: 6f29 290a 2020 2020 2020 2020 2020 2020  o)).            
+00015250: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
+00015260: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
+00015270: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015280: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+00015290: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+000152a0: 2229 2021 3d20 6d6f 6465 3a0a 2020 2020  ") != mode:.    
+000152b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152c0: 696e 666f 5f64 6972 7479 203d 2054 7275  info_dirty = Tru
+000152d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000152e0: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+000152f0: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
+00015300: 206d 6f64 650a 0a20 2020 2020 2020 2020   mode..         
+00015310: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00015320: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+00015330: 6277 2229 2021 3d20 6277 3a0a 2020 2020  bw") != bw:.    
+00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015350: 696e 666f 5f64 6972 7479 203d 2054 7275  info_dirty = Tru
+00015360: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015370: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+00015380: 5f73 7461 7465 5b22 6277 225d 203d 2062  _state["bw"] = b
+00015390: 770a 0a20 2020 2020 2020 2020 2020 2020  w..             
+000153a0: 2020 2069 6620 6461 7465 7469 6d65 2e6e     if datetime.n
+000153b0: 6f77 2829 203e 2067 6c6f 6261 6c73 2829  ow() > globals()
+000153c0: 5b22 706f 6c6c 5f74 696d 6522 5d20 6f72  ["poll_time"] or
+000153d0: 2069 6e66 6f5f 6469 7274 793a 0a20 2020   info_dirty:.   
+000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153f0: 206c 6f67 6765 722e 6465 6275 6728 2256   logger.debug("V
+00015400: 464f 3a20 2573 2020 4d4f 4445 3a20 2573  FO: %s  MODE: %s
+00015410: 2042 573a 2025 7322 2c20 7666 6f2c 206d   BW: %s", vfo, m
+00015420: 6f64 652c 2062 7729 0a20 2020 2020 2020  ode, bw).       
+00015430: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015440: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+00015450: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+00015460: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00015470: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00015480: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+00015490: 203d 2022 5241 4449 4f5f 5354 4154 4522   = "RADIO_STATE"
+000154a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000154b0: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+000154c0: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+000154d0: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+000154e0: 2020 2020 2020 2020 2020 636d 645b 2262            cmd["b
+000154f0: 616e 6422 5d20 3d20 6261 6e64 0a20 2020  and"] = band.   
+00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015510: 2063 6d64 5b22 7666 6f61 225d 203d 2076   cmd["vfoa"] = v
+00015520: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
+00015530: 2020 2020 2020 2063 6d64 5b22 6d6f 6465         cmd["mode
+00015540: 225d 203d 206d 6f64 650a 2020 2020 2020  "] = mode.      
+00015550: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00015560: 645b 2262 7722 5d20 3d20 6277 0a20 2020  d["bw"] = bw.   
+00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015580: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00015590: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+000155a0: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
 000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 636d 645b 226d 6f64 6522 5d20 3d20 6d6f  cmd["mode"] = mo
-000155d0: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
-000155e0: 2020 2020 2020 2063 6d64 5b22 6277 225d         cmd["bw"]
-000155f0: 203d 2062 770a 2020 2020 2020 2020 2020   = bw.          
-00015600: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015610: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00015620: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
-00015630: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
-00015640: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00015650: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
-00015660: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015670: 6620 7365 6c66 2e6e 316d 6d2e 7365 6e64  f self.n1mm.send
-00015680: 5f72 6164 696f 5f70 6163 6b65 7473 3a0a  _radio_packets:.
-00015690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000156b0: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
-000156c0: 5b22 4672 6571 225d 203d 2076 666f 5b3a  ["Freq"] = vfo[:
-000156d0: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
-000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156f0: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-00015700: 696e 666f 5b22 5458 4672 6571 225d 203d  info["TXFreq"] =
-00015710: 2076 666f 5b3a 2d31 5d0a 2020 2020 2020   vfo[:-1].      
+000155c0: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
+000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155e0: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
+000155f0: 6d6d 2e73 656e 645f 7261 6469 6f5f 7061  mm.send_radio_pa
+00015600: 636b 6574 733a 0a20 2020 2020 2020 2020  ckets:.         
+00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015620: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
+00015630: 696f 5f69 6e66 6f5b 2246 7265 7122 5d20  io_info["Freq"] 
+00015640: 3d20 7666 6f5b 3a2d 315d 0a20 2020 2020  = vfo[:-1].     
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00015670: 2e72 6164 696f 5f69 6e66 6f5b 2254 5846  .radio_info["TXF
+00015680: 7265 7122 5d20 3d20 7666 6f5b 3a2d 315d  req"] = vfo[:-1]
+00015690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000156a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000156b0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+000156c0: 6f5b 224d 6f64 6522 5d20 3d20 6d6f 6465  o["Mode"] = mode
+000156d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000156e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000156f0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+00015700: 6f5b 224f 7043 616c 6c22 5d20 3d20 7365  o["OpCall"] = se
+00015710: 6c66 2e63 7572 7265 6e74 5f6f 700a 2020  lf.current_op.  
 00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015730: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00015740: 7261 6469 6f5f 696e 666f 5b22 4d6f 6465  radio_info["Mode
-00015750: 225d 203d 206d 6f64 650a 2020 2020 2020  "] = mode.      
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00015780: 7261 6469 6f5f 696e 666f 5b22 4f70 4361  radio_info["OpCa
-00015790: 6c6c 225d 203d 2073 656c 662e 6375 7272  ll"] = self.curr
-000157a0: 656e 745f 6f70 0a20 2020 2020 2020 2020  ent_op.         
+00015730: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00015740: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+00015750: 4973 5275 6e6e 696e 6722 5d20 3d20 7374  IsRunning"] = st
+00015760: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015780: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+00015790: 2822 7275 6e5f 7374 6174 6522 2c20 4661  ("run_state", Fa
+000157a0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
 000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157c0: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
-000157d0: 696f 5f69 6e66 6f5b 2249 7352 756e 6e69  io_info["IsRunni
-000157e0: 6e67 225d 203d 2073 7472 280a 2020 2020  ng"] = str(.    
-000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015810: 2e70 7265 662e 6765 7428 2272 756e 5f73  .pref.get("run_s
-00015820: 7461 7465 222c 2046 616c 7365 290a 2020  tate", False).  
-00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015840: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015860: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00015870: 6d2e 7365 6e64 5f72 6164 696f 2829 0a20  m.send_radio(). 
-00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015890: 2020 2067 6c6f 6261 6c73 2829 5b22 706f     globals()["po
-000158a0: 6c6c 5f74 696d 6522 5d20 3d20 6461 7465  ll_time"] = date
-000158b0: 7469 6d65 2e6e 6f77 2829 202b 2064 742e  time.now() + dt.
-000158c0: 7469 6d65 6465 6c74 6128 7365 636f 6e64  timedelta(second
-000158d0: 733d 3130 290a 0a20 2020 2064 6566 2065  s=10)..    def e
-000158e0: 6469 745f 6377 5f6d 6163 726f 7328 7365  dit_cw_macros(se
-000158f0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00015900: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015910: 2043 616c 6c73 2074 6865 2064 6566 6175   Calls the defau
-00015920: 6c74 2074 6578 7420 6564 6974 6f72 2074  lt text editor t
-00015930: 6f20 6564 6974 2074 6865 2043 5720 6d61  o edit the CW ma
-00015940: 6372 6f20 6669 6c65 2e0a 2020 2020 2020  cro file..      
-00015950: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00015960: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00015970: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
-00015980: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-00015990: 2020 206d 6163 726f 5f66 696c 6520 3d20     macro_file = 
-000159a0: 222f 6377 6d61 6372 6f73 2e74 7874 220a  "/cwmacros.txt".
-000159b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000159c0: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
-000159d0: 6669 6c65 203d 2022 2f73 7362 6d61 6372  file = "/ssbmacr
-000159e0: 6f73 2e74 7874 220a 2020 2020 2020 2020  os.txt".        
-000159f0: 6966 206e 6f74 2050 6174 6828 4441 5441  if not Path(DATA
-00015a00: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
-00015a10: 6c65 292e 6578 6973 7473 2829 3a0a 2020  le).exists():.  
-00015a20: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00015a30: 2e64 6562 7567 2822 7265 6164 5f63 775f  .debug("read_cw_
-00015a40: 6d61 6372 6f73 3a20 636f 7079 696e 6720  macros: copying 
-00015a50: 6465 6661 756c 7420 6d61 6372 6f20 6669  default macro fi
-00015a60: 6c65 2e22 290a 2020 2020 2020 2020 2020  le.").          
-00015a70: 2020 636f 7079 6669 6c65 2857 4f52 4b49    copyfile(WORKI
-00015a80: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
-00015a90: 2220 2b20 6d61 6372 6f5f 6669 6c65 2c20  " + macro_file, 
-00015aa0: 4441 5441 5f50 4154 4820 2b20 6d61 6372  DATA_PATH + macr
-00015ab0: 6f5f 6669 6c65 290a 2020 2020 2020 2020  o_file).        
-00015ac0: 6f73 2e73 7973 7465 6d28 6622 7864 672d  os.system(f"xdg-
-00015ad0: 6f70 656e 207b 4441 5441 5f50 4154 487d  open {DATA_PATH}
-00015ae0: 7b6d 6163 726f 5f66 696c 657d 2229 0a0a  {macro_file}")..
-00015af0: 2020 2020 6465 6620 7265 6164 5f63 775f      def read_cw_
-00015b00: 6d61 6372 6f73 2873 656c 6629 202d 3e20  macros(self) -> 
-00015b10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00015b20: 220a 2020 2020 2020 2020 5265 6164 7320  ".        Reads 
-00015b30: 696e 2074 6865 2043 5720 6d61 6372 6f73  in the CW macros
-00015b40: 2c20 6669 7273 7473 2069 7420 6368 6563  , firsts it chec
-00015b50: 6b73 2074 6f20 7365 6520 6966 2074 6865  ks to see if the
-00015b60: 2066 696c 6520 6578 6973 7473 2e20 4966   file exists. If
-00015b70: 2069 7420 646f 6573 206e 6f74 2c0a 2020   it does not,.  
-00015b80: 2020 2020 2020 616e 6420 7468 6973 2068        and this h
-00015b90: 6173 2062 6565 6e20 7061 636b 6167 6564  as been packaged
-00015ba0: 2077 6974 6820 7079 696e 7374 616c 6c65   with pyinstalle
-00015bb0: 7220 6974 2077 696c 6c20 636f 7079 2074  r it will copy t
-00015bc0: 6865 2064 6566 6175 6c74 2066 696c 6520  he default file 
-00015bd0: 6672 6f6d 2074 6865 0a20 2020 2020 2020  from the.       
-00015be0: 2074 656d 7020 6469 7265 6374 6f72 7920   temp directory 
-00015bf0: 7468 6973 2069 7320 7275 6e6e 696e 6720  this is running 
-00015c00: 6672 6f6d 2e2e 2e20 496e 2074 6865 6f72  from... In theor
-00015c10: 792e 0a20 2020 2020 2020 2022 2222 0a0a  y..        """..
-00015c20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00015c30: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00015c40: 226d 6f64 6522 2920 3d3d 2022 4357 223a  "mode") == "CW":
-00015c50: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
-00015c60: 726f 5f66 696c 6520 3d20 222f 6377 6d61  ro_file = "/cwma
-00015c70: 6372 6f73 2e74 7874 220a 2020 2020 2020  cros.txt".      
-00015c80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00015c90: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
-00015ca0: 2022 2f73 7362 6d61 6372 6f73 2e74 7874   "/ssbmacros.txt
-00015cb0: 220a 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
-00015cc0: 7420 5061 7468 2844 4154 415f 5041 5448  t Path(DATA_PATH
-00015cd0: 202b 206d 6163 726f 5f66 696c 6529 2e65   + macro_file).e
-00015ce0: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
-00015cf0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00015d00: 6728 2272 6561 645f 6377 5f6d 6163 726f  g("read_cw_macro
-00015d10: 733a 2063 6f70 7969 6e67 2064 6566 6175  s: copying defau
-00015d20: 6c74 206d 6163 726f 2066 696c 652e 2229  lt macro file.")
-00015d30: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
-00015d40: 7966 696c 6528 574f 524b 494e 475f 5041  yfile(WORKING_PA
-00015d50: 5448 202b 2022 2f64 6174 6122 202b 206d  TH + "/data" + m
-00015d60: 6163 726f 5f66 696c 652c 2044 4154 415f  acro_file, DATA_
-00015d70: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
-00015d80: 6529 0a20 2020 2020 2020 2077 6974 6820  e).        with 
-00015d90: 6f70 656e 2844 4154 415f 5041 5448 202b  open(DATA_PATH +
-00015da0: 206d 6163 726f 5f66 696c 652c 2022 7222   macro_file, "r"
-00015db0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00015dc0: 3822 2920 6173 2066 696c 655f 6465 7363  8") as file_desc
-00015dd0: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
-00015de0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00015df0: 6669 6c65 5f64 6573 6372 6970 746f 723a  file_descriptor:
-00015e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00015e20: 2020 2020 2020 2020 2020 6d6f 6465 2c20            mode, 
-00015e30: 666b 6579 2c20 6275 7474 6f6e 6e61 6d65  fkey, buttonname
-00015e40: 2c20 6377 7465 7874 203d 206c 696e 652e  , cwtext = line.
-00015e50: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-00015e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015e70: 6620 6d6f 6465 2e73 7472 6970 2829 2e75  f mode.strip().u
-00015e80: 7070 6572 2829 203d 3d20 2252 2220 616e  pper() == "R" an
-00015e90: 6420 7365 6c66 2e70 7265 662e 6765 7428  d self.pref.get(
-00015ea0: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ec0: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
-00015ed0: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
-00015ee0: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
-00015ef0: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
-00015f00: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
-00015f10: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00015f20: 652e 7374 7269 7028 292e 7570 7065 7228  e.strip().upper(
-00015f30: 2920 213d 2022 5222 2061 6e64 206e 6f74  ) != "R" and not
-00015f40: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00015f50: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
-00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f70: 2020 2020 2073 656c 662e 666b 6579 735b       self.fkeys[
-00015f80: 666b 6579 2e73 7472 6970 2829 5d20 3d20  fkey.strip()] = 
-00015f90: 2862 7574 746f 6e6e 616d 652e 7374 7269  (buttonname.stri
-00015fa0: 7028 292c 2063 7774 6578 742e 7374 7269  p(), cwtext.stri
-00015fb0: 7028 2929 0a20 2020 2020 2020 2020 2020  p()).           
-00015fc0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-00015fd0: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
-00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-00016000: 7265 6164 5f63 775f 6d61 6372 6f73 3a20  read_cw_macros: 
-00016010: 2573 222c 2065 7272 290a 2020 2020 2020  %s", err).      
-00016020: 2020 6b65 7973 203d 2073 656c 662e 666b    keys = self.fk
-00016030: 6579 732e 6b65 7973 2829 0a20 2020 2020  eys.keys().     
-00016040: 2020 2069 6620 2246 3122 2069 6e20 6b65     if "F1" in ke
-00016050: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00016060: 7365 6c66 2e46 312e 7365 7454 6578 7428  self.F1.setText(
-00016070: 6622 4631 3a20 7b73 656c 662e 666b 6579  f"F1: {self.fkey
-00016080: 735b 2746 3127 5d5b 305d 7d22 290a 2020  s['F1'][0]}").  
-00016090: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000160a0: 312e 7365 7454 6f6f 6c54 6970 2873 656c  1.setToolTip(sel
-000160b0: 662e 666b 6579 735b 2246 3122 5d5b 315d  f.fkeys["F1"][1]
-000160c0: 290a 2020 2020 2020 2020 6966 2022 4632  ).        if "F2
-000160d0: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-000160e0: 2020 2020 2020 2073 656c 662e 4632 2e73         self.F2.s
-000160f0: 6574 5465 7874 2866 2246 323a 207b 7365  etText(f"F2: {se
-00016100: 6c66 2e66 6b65 7973 5b27 4632 275d 5b30  lf.fkeys['F2'][0
-00016110: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00016120: 2073 656c 662e 4632 2e73 6574 546f 6f6c   self.F2.setTool
-00016130: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-00016140: 4632 225d 5b31 5d29 0a20 2020 2020 2020  F2"][1]).       
-00016150: 2069 6620 2246 3322 2069 6e20 6b65 7973   if "F3" in keys
-00016160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00016170: 6c66 2e46 332e 7365 7454 6578 7428 6622  lf.F3.setText(f"
-00016180: 4633 3a20 7b73 656c 662e 666b 6579 735b  F3: {self.fkeys[
-00016190: 2746 3327 5d5b 305d 7d22 290a 2020 2020  'F3'][0]}").    
-000161a0: 2020 2020 2020 2020 7365 6c66 2e46 332e          self.F3.
-000161b0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-000161c0: 666b 6579 735b 2246 3322 5d5b 315d 290a  fkeys["F3"][1]).
-000161d0: 2020 2020 2020 2020 6966 2022 4634 2220          if "F4" 
-000161e0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-000161f0: 2020 2020 2073 656c 662e 4634 2e73 6574       self.F4.set
-00016200: 5465 7874 2866 2246 343a 207b 7365 6c66  Text(f"F4: {self
-00016210: 2e66 6b65 7973 5b27 4634 275d 5b30 5d7d  .fkeys['F4'][0]}
-00016220: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00016230: 656c 662e 4634 2e73 6574 546f 6f6c 5469  elf.F4.setToolTi
-00016240: 7028 7365 6c66 2e66 6b65 7973 5b22 4634  p(self.fkeys["F4
-00016250: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-00016260: 6620 2246 3522 2069 6e20 6b65 7973 3a0a  f "F5" in keys:.
-00016270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016280: 2e46 352e 7365 7454 6578 7428 6622 4635  .F5.setText(f"F5
-00016290: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-000162a0: 3527 5d5b 305d 7d22 290a 2020 2020 2020  5'][0]}").      
-000162b0: 2020 2020 2020 7365 6c66 2e46 352e 7365        self.F5.se
-000162c0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-000162d0: 6579 735b 2246 3522 5d5b 315d 290a 2020  eys["F5"][1]).  
-000162e0: 2020 2020 2020 6966 2022 4636 2220 696e        if "F6" in
-000162f0: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
-00016300: 2020 2073 656c 662e 4636 2e73 6574 5465     self.F6.setTe
-00016310: 7874 2866 2246 363a 207b 7365 6c66 2e66  xt(f"F6: {self.f
-00016320: 6b65 7973 5b27 4636 275d 5b30 5d7d 2229  keys['F6'][0]}")
-00016330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016340: 662e 4636 2e73 6574 546f 6f6c 5469 7028  f.F6.setToolTip(
-00016350: 7365 6c66 2e66 6b65 7973 5b22 4636 225d  self.fkeys["F6"]
-00016360: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-00016370: 2246 3722 2069 6e20 6b65 7973 3a0a 2020  "F7" in keys:.  
-00016380: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00016390: 372e 7365 7454 6578 7428 6622 4637 3a20  7.setText(f"F7: 
-000163a0: 7b73 656c 662e 666b 6579 735b 2746 3727  {self.fkeys['F7'
-000163b0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
-000163c0: 2020 2020 7365 6c66 2e46 372e 7365 7454      self.F7.setT
-000163d0: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
-000163e0: 735b 2246 3722 5d5b 315d 290a 2020 2020  s["F7"][1]).    
-000163f0: 2020 2020 6966 2022 4638 2220 696e 206b      if "F8" in k
-00016400: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00016410: 2073 656c 662e 4638 2e73 6574 5465 7874   self.F8.setText
-00016420: 2866 2246 383a 207b 7365 6c66 2e66 6b65  (f"F8: {self.fke
-00016430: 7973 5b27 4638 275d 5b30 5d7d 2229 0a20  ys['F8'][0]}"). 
-00016440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016450: 4638 2e73 6574 546f 6f6c 5469 7028 7365  F8.setToolTip(se
-00016460: 6c66 2e66 6b65 7973 5b22 4638 225d 5b31  lf.fkeys["F8"][1
-00016470: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-00016480: 3922 2069 6e20 6b65 7973 3a0a 2020 2020  9" in keys:.    
-00016490: 2020 2020 2020 2020 7365 6c66 2e46 392e          self.F9.
-000164a0: 7365 7454 6578 7428 6622 4639 3a20 7b73  setText(f"F9: {s
-000164b0: 656c 662e 666b 6579 735b 2746 3927 5d5b  elf.fkeys['F9'][
-000164c0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-000164d0: 2020 7365 6c66 2e46 392e 7365 7454 6f6f    self.F9.setToo
-000164e0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-000164f0: 2246 3922 5d5b 315d 290a 2020 2020 2020  "F9"][1]).      
-00016500: 2020 6966 2022 4631 3022 2069 6e20 6b65    if "F10" in ke
-00016510: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00016520: 7365 6c66 2e46 3130 2e73 6574 5465 7874  self.F10.setText
-00016530: 2866 2246 3130 3a20 7b73 656c 662e 666b  (f"F10: {self.fk
-00016540: 6579 735b 2746 3130 275d 5b30 5d7d 2229  eys['F10'][0]}")
-00016550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016560: 662e 4631 302e 7365 7454 6f6f 6c54 6970  f.F10.setToolTip
-00016570: 2873 656c 662e 666b 6579 735b 2246 3130  (self.fkeys["F10
-00016580: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-00016590: 6620 2246 3131 2220 696e 206b 6579 733a  f "F11" in keys:
-000165a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000165b0: 662e 4631 312e 7365 7454 6578 7428 6622  f.F11.setText(f"
-000165c0: 4631 313a 207b 7365 6c66 2e66 6b65 7973  F11: {self.fkeys
-000165d0: 5b27 4631 3127 5d5b 305d 7d22 290a 2020  ['F11'][0]}").  
-000165e0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000165f0: 3131 2e73 6574 546f 6f6c 5469 7028 7365  11.setToolTip(se
-00016600: 6c66 2e66 6b65 7973 5b22 4631 3122 5d5b  lf.fkeys["F11"][
-00016610: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00016620: 4631 3222 2069 6e20 6b65 7973 3a0a 2020  F12" in keys:.  
-00016630: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00016640: 3132 2e73 6574 5465 7874 2866 2246 3132  12.setText(f"F12
-00016650: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-00016660: 3132 275d 5b30 5d7d 2229 0a20 2020 2020  12'][0]}").     
-00016670: 2020 2020 2020 2073 656c 662e 4631 322e         self.F12.
-00016680: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-00016690: 666b 6579 735b 2246 3132 225d 5b31 5d29  fkeys["F12"][1])
-000166a0: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
-000166b0: 7465 5f61 6469 6628 7365 6c66 293a 0a20  te_adif(self):. 
-000166c0: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-000166d0: 7465 2041 4449 4622 2222 0a20 2020 2020  te ADIF""".     
-000166e0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-000166f0: 222a 2a2a 2a2a 2a41 4449 462a 2a2a 2a2a  "******ADIF*****
-00016700: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00016710: 636f 6e74 6573 742e 6164 6966 2873 656c  contest.adif(sel
-00016720: 6629 0a0a 2020 2020 6465 6620 6765 6e65  f)..    def gene
-00016730: 7261 7465 5f63 6162 7269 6c6c 6f28 7365  rate_cabrillo(se
-00016740: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00016750: 4765 6e65 7261 7465 7320 4361 6272 696c  Generates Cabril
-00016760: 6c6f 2066 696c 652e 204d 6179 6265 2e22  lo file. Maybe."
-00016770: 2222 0a20 2020 2020 2020 2023 2068 7474  "".        # htt
-00016780: 7073 3a2f 2f77 7777 2e63 7177 7078 2e63  ps://www.cqwpx.c
-00016790: 6f6d 2f63 6162 7269 6c6c 6f2e 6874 6d0a  om/cabrillo.htm.
-000167a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-000167b0: 6562 7567 2822 2a2a 2a2a 2a2a 4361 6272  ebug("******Cabr
-000167c0: 696c 6c6f 2a2a 2a2a 2a22 290a 2020 2020  illo*****").    
-000167d0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-000167e0: 2e63 6162 7269 6c6c 6f28 7365 6c66 290a  .cabrillo(self).
-000167f0: 0a0a 6465 6620 6c6f 6164 5f66 6f6e 7473  ..def load_fonts
-00016800: 5f66 726f 6d5f 6469 7228 6469 7265 6374  _from_dir(direct
-00016810: 6f72 793a 2073 7472 2920 2d3e 2073 6574  ory: str) -> set
-00016820: 3a0a 2020 2020 2222 220a 2020 2020 5765  :.    """.    We
-00016830: 6c6c 2069 7420 6c6f 6164 7320 666f 6e74  ll it loads font
-00016840: 7320 6672 6f6d 2061 2064 6972 6563 746f  s from a directo
-00016850: 7279 2e2e 2e0a 2020 2020 2222 220a 2020  ry....    """.  
-00016860: 2020 666f 6e74 5f66 616d 696c 6965 7320    font_families 
-00016870: 3d20 7365 7428 290a 2020 2020 666f 7220  = set().    for 
-00016880: 5f66 6920 696e 2051 4469 7228 6469 7265  _fi in QDir(dire
-00016890: 6374 6f72 7929 2e65 6e74 7279 496e 666f  ctory).entryInfo
-000168a0: 4c69 7374 285b 222a 2e74 7466 222c 2022  List(["*.ttf", "
-000168b0: 2a2e 776f 6666 222c 2022 2a2e 776f 6666  *.woff", "*.woff
-000168c0: 3222 5d29 3a0a 2020 2020 2020 2020 5f69  2"]):.        _i
-000168d0: 6420 3d20 5146 6f6e 7444 6174 6162 6173  d = QFontDatabas
-000168e0: 652e 6164 6441 7070 6c69 6361 7469 6f6e  e.addApplication
-000168f0: 466f 6e74 285f 6669 2e61 6273 6f6c 7574  Font(_fi.absolut
-00016900: 6546 696c 6550 6174 6828 2929 0a20 2020  eFilePath()).   
-00016910: 2020 2020 2066 6f6e 745f 6661 6d69 6c69       font_famili
-00016920: 6573 207c 3d20 7365 7428 5146 6f6e 7444  es |= set(QFontD
-00016930: 6174 6162 6173 652e 6170 706c 6963 6174  atabase.applicat
-00016940: 696f 6e46 6f6e 7446 616d 696c 6965 7328  ionFontFamilies(
-00016950: 5f69 6429 290a 2020 2020 7265 7475 726e  _id)).    return
-00016960: 2066 6f6e 745f 6661 6d69 6c69 6573 0a0a   font_families..
-00016970: 0a64 6566 2069 6e73 7461 6c6c 5f69 636f  .def install_ico
-00016980: 6e73 2829 3a0a 2020 2020 2222 2249 6e73  ns():.    """Ins
-00016990: 7461 6c6c 2069 636f 6e73 2222 220a 2020  tall icons""".  
-000169a0: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
-000169b0: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
-000169c0: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
-000169d0: 2d2d 7369 7a65 2033 3220 2d2d 636f 6e74  --size 32 --cont
-000169e0: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-000169f0: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-00016a00: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-00016a10: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-00016a20: 6d2d 3332 2e70 6e67 206b 3667 7465 2d6e  m-32.png k6gte-n
-00016a30: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-00016a40: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
-00016a50: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
-00016a60: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
-00016a70: 2d73 697a 6520 3634 202d 2d63 6f6e 7465  -size 64 --conte
-00016a80: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
-00016a90: 7365 7220 220a 2020 2020 2020 2020 6622  ser ".        f"
-00016aa0: 7b57 4f52 4b49 4e47 5f50 4154 487d 2f64  {WORKING_PATH}/d
-00016ab0: 6174 612f 6b36 6774 652e 6e6f 7431 6d6d  ata/k6gte.not1mm
-00016ac0: 2d36 342e 706e 6720 6b36 6774 652d 6e6f  -64.png k6gte-no
-00016ad0: 7431 6d6d 220a 2020 2020 290a 2020 2020  t1mm".    ).    
-00016ae0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
-00016af0: 2020 2022 7864 672d 6963 6f6e 2d72 6573     "xdg-icon-res
-00016b00: 6f75 7263 6520 696e 7374 616c 6c20 2d2d  ource install --
-00016b10: 7369 7a65 2031 3238 202d 2d63 6f6e 7465  size 128 --conte
-00016b20: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
-00016b30: 7365 7220 220a 2020 2020 2020 2020 6622  ser ".        f"
-00016b40: 7b57 4f52 4b49 4e47 5f50 4154 487d 2f64  {WORKING_PATH}/d
-00016b50: 6174 612f 6b36 6774 652e 6e6f 7431 6d6d  ata/k6gte.not1mm
-00016b60: 2d31 3238 2e70 6e67 206b 3667 7465 2d6e  -128.png k6gte-n
-00016b70: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-00016b80: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
-00016b90: 2d64 6573 6b74 6f70 2d6d 656e 7520 696e  -desktop-menu in
-00016ba0: 7374 616c 6c20 7b57 4f52 4b49 4e47 5f50  stall {WORKING_P
-00016bb0: 4154 487d 2f64 6174 612f 6b36 6774 652d  ATH}/data/k6gte-
-00016bc0: 6e6f 7431 6d6d 2e64 6573 6b74 6f70 2229  not1mm.desktop")
-00016bd0: 0a0a 0a64 6566 2064 6f69 6d70 286d 6f64  ...def doimp(mod
-00016be0: 6e61 6d65 293a 0a20 2020 2022 2222 7265  name):.    """re
-00016bf0: 7475 726e 206d 6f64 756c 6520 7061 7468  turn module path
-00016c00: 2222 220a 2020 2020 7265 7475 726e 2069  """.    return i
-00016c10: 6d70 6f72 746c 6962 2e69 6d70 6f72 745f  mportlib.import_
-00016c20: 6d6f 6475 6c65 2866 226e 6f74 316d 6d2e  module(f"not1mm.
-00016c30: 706c 7567 696e 732e 7b6d 6f64 6e61 6d65  plugins.{modname
-00016c40: 7d22 290a 0a0a 6465 6620 7275 6e28 293a  }")...def run():
-00016c50: 0a20 2020 2022 2222 0a20 2020 204d 6169  .    """.    Mai
-00016c60: 6e20 456e 7472 790a 2020 2020 2222 220a  n Entry.    """.
-00016c70: 2020 2020 696e 7374 616c 6c5f 6963 6f6e      install_icon
-00016c80: 7328 290a 2020 2020 7469 6d65 722e 7374  s().    timer.st
-00016c90: 6172 7428 3235 3029 0a20 2020 2073 7973  art(250).    sys
-00016ca0: 2e65 7869 7428 6170 702e 6578 6563 2829  .exit(app.exec()
-00016cb0: 290a 0a0a 6c6f 6767 6572 203d 206c 6f67  )...logger = log
-00016cc0: 6769 6e67 2e67 6574 4c6f 6767 6572 2822  ging.getLogger("
-00016cd0: 5f5f 6d61 696e 5f5f 2229 0a68 616e 646c  __main__").handl
-00016ce0: 6572 203d 206c 6f67 6769 6e67 2e53 7472  er = logging.Str
-00016cf0: 6561 6d48 616e 646c 6572 2829 0a66 6f72  eamHandler().for
-00016d00: 6d61 7474 6572 203d 206c 6f67 6769 6e67  matter = logging
-00016d10: 2e46 6f72 6d61 7474 6572 280a 2020 2020  .Formatter(.    
-00016d20: 6461 7465 666d 743d 2225 483a 254d 3a25  datefmt="%H:%M:%
-00016d30: 5322 2c0a 2020 2020 666d 743d 225b 2528  S",.    fmt="[%(
-00016d40: 6173 6374 696d 6529 735d 2025 286c 6576  asctime)s] %(lev
-00016d50: 656c 6e61 6d65 2973 2025 286d 6f64 756c  elname)s %(modul
-00016d60: 6529 7320 2d20 2528 6675 6e63 4e61 6d65  e)s - %(funcName
-00016d70: 2973 204c 696e 6520 2528 6c69 6e65 6e6f  )s Line %(lineno
-00016d80: 2964 3a20 2528 6d65 7373 6167 6529 7322  )d: %(message)s"
-00016d90: 2c0a 290a 6861 6e64 6c65 722e 7365 7446  ,.).handler.setF
-00016da0: 6f72 6d61 7474 6572 2866 6f72 6d61 7474  ormatter(formatt
-00016db0: 6572 290a 6c6f 6767 6572 2e61 6464 4861  er).logger.addHa
-00016dc0: 6e64 6c65 7228 6861 6e64 6c65 7229 0a0a  ndler(handler)..
-00016dd0: 4245 5441 5f54 4553 5420 3d20 4661 6c73  BETA_TEST = Fals
-00016de0: 650a 6966 2050 6174 6828 222e 2f62 6574  e.if Path("./bet
-00016df0: 6174 6573 7422 292e 6578 6973 7473 2829  atest").exists()
-00016e00: 3a0a 2020 2020 4245 5441 5f54 4553 5420  :.    BETA_TEST 
-00016e10: 3d20 5472 7565 0a0a 6966 2050 6174 6828  = True..if Path(
-00016e20: 222e 2f64 6562 7567 2229 2e65 7869 7374  "./debug").exist
-00016e30: 7328 293a 0a20 2020 206c 6f67 6765 722e  s():.    logger.
-00016e40: 7365 744c 6576 656c 286c 6f67 6769 6e67  setLevel(logging
-00016e50: 2e44 4542 5547 290a 2020 2020 6c6f 6767  .DEBUG).    logg
-00016e60: 6572 2e64 6562 7567 2822 6465 6275 6767  er.debug("debugg
-00016e70: 696e 6720 6f6e 2229 0a65 6c73 653a 0a20  ing on").else:. 
-00016e80: 2020 206c 6f67 6765 722e 7365 744c 6576     logger.setLev
-00016e90: 656c 286c 6f67 6769 6e67 2e57 4152 4e49  el(logging.WARNI
-00016ea0: 4e47 290a 2020 2020 6c6f 6767 6572 2e77  NG).    logger.w
-00016eb0: 6172 6e69 6e67 2822 6465 6275 6767 696e  arning("debuggin
-00016ec0: 6720 6f66 6622 290a 0a61 7070 203d 2051  g off")..app = Q
-00016ed0: 7457 6964 6765 7473 2e51 4170 706c 6963  tWidgets.QApplic
-00016ee0: 6174 696f 6e28 7379 732e 6172 6776 290a  ation(sys.argv).
-00016ef0: 6170 702e 7365 7453 7479 6c65 2822 4164  app.setStyle("Ad
-00016f00: 7761 6974 612d 4461 726b 2229 0a66 6f6e  waita-Dark").fon
-00016f10: 745f 7061 7468 203d 2057 4f52 4b49 4e47  t_path = WORKING
-00016f20: 5f50 4154 4820 2b20 222f 6461 7461 220a  _PATH + "/data".
-00016f30: 6661 6d69 6c69 6573 203d 206c 6f61 645f  families = load_
-00016f40: 666f 6e74 735f 6672 6f6d 5f64 6972 286f  fonts_from_dir(o
-00016f50: 732e 6673 7061 7468 2866 6f6e 745f 7061  s.fspath(font_pa
-00016f60: 7468 2929 0a6c 6f67 6765 722e 696e 666f  th)).logger.info
-00016f70: 2866 616d 696c 6965 7329 0a77 696e 646f  (families).windo
-00016f80: 7720 3d20 4d61 696e 5769 6e64 6f77 2829  w = MainWindow()
-00016f90: 0a68 6569 6768 7420 3d20 7769 6e64 6f77  .height = window
-00016fa0: 2e70 7265 662e 6765 7428 2277 696e 646f  .pref.get("windo
-00016fb0: 775f 6865 6967 6874 222c 2033 3030 290a  w_height", 300).
-00016fc0: 7769 6474 6820 3d20 7769 6e64 6f77 2e70  width = window.p
-00016fd0: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
-00016fe0: 7769 6474 6822 2c20 3730 3029 0a78 203d  width", 700).x =
-00016ff0: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
-00017000: 2822 7769 6e64 6f77 5f78 222c 202d 3129  ("window_x", -1)
-00017010: 0a79 203d 2077 696e 646f 772e 7072 6566  .y = window.pref
-00017020: 2e67 6574 2822 7769 6e64 6f77 5f79 222c  .get("window_y",
-00017030: 202d 3129 0a77 696e 646f 772e 7365 7447   -1).window.setG
-00017040: 656f 6d65 7472 7928 782c 2079 2c20 7769  eometry(x, y, wi
-00017050: 6474 682c 2068 6569 6768 7429 0a77 696e  dth, height).win
-00017060: 646f 772e 6361 6c6c 7369 676e 2e73 6574  dow.callsign.set
-00017070: 466f 6375 7328 290a 7769 6e64 6f77 2e73  Focus().window.s
-00017080: 686f 7728 290a 7469 6d65 7220 3d20 5174  how().timer = Qt
-00017090: 436f 7265 2e51 5469 6d65 7228 290a 7469  Core.QTimer().ti
-000170a0: 6d65 722e 7469 6d65 6f75 742e 636f 6e6e  mer.timeout.conn
-000170b0: 6563 7428 7769 6e64 6f77 2e70 6f6c 6c5f  ect(window.poll_
-000170c0: 7261 6469 6f29 0a0a 6966 205f 5f6e 616d  radio)..if __nam
-000170d0: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-000170e0: 223a 0a20 2020 2072 756e 2829 0a         ":.    run().
+000157c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000157d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000157e0: 656c 662e 6e31 6d6d 2e73 656e 645f 7261  elf.n1mm.send_ra
+000157f0: 6469 6f28 290a 2020 2020 2020 2020 2020  dio().          
+00015800: 2020 2020 2020 2020 2020 676c 6f62 616c            global
+00015810: 7328 295b 2270 6f6c 6c5f 7469 6d65 225d  s()["poll_time"]
+00015820: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
+00015830: 2920 2b20 6474 2e74 696d 6564 656c 7461  ) + dt.timedelta
+00015840: 2873 6563 6f6e 6473 3d31 3029 0a0a 2020  (seconds=10)..  
+00015850: 2020 6465 6620 6564 6974 5f63 775f 6d61    def edit_cw_ma
+00015860: 6372 6f73 2873 656c 6629 202d 3e20 4e6f  cros(self) -> No
+00015870: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00015880: 2020 2020 2020 2020 4361 6c6c 7320 7468          Calls th
+00015890: 6520 6465 6661 756c 7420 7465 7874 2065  e default text e
+000158a0: 6469 746f 7220 746f 2065 6469 7420 7468  ditor to edit th
+000158b0: 6520 4357 206d 6163 726f 2066 696c 652e  e CW macro file.
+000158c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000158d0: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
+000158e0: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+000158f0: 6465 2229 203d 3d20 2243 5722 3a0a 2020  de") == "CW":.  
+00015900: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
+00015910: 6669 6c65 203d 2022 2f63 776d 6163 726f  file = "/cwmacro
+00015920: 732e 7478 7422 0a20 2020 2020 2020 2065  s.txt".        e
+00015930: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00015940: 206d 6163 726f 5f66 696c 6520 3d20 222f   macro_file = "/
+00015950: 7373 626d 6163 726f 732e 7478 7422 0a20  ssbmacros.txt". 
+00015960: 2020 2020 2020 2069 6620 6e6f 7420 5061         if not Pa
+00015970: 7468 2844 4154 415f 5041 5448 202b 206d  th(DATA_PATH + m
+00015980: 6163 726f 5f66 696c 6529 2e65 7869 7374  acro_file).exist
+00015990: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+000159a0: 206c 6f67 6765 722e 6465 6275 6728 2272   logger.debug("r
+000159b0: 6561 645f 6377 5f6d 6163 726f 733a 2063  ead_cw_macros: c
+000159c0: 6f70 7969 6e67 2064 6566 6175 6c74 206d  opying default m
+000159d0: 6163 726f 2066 696c 652e 2229 0a20 2020  acro file.").   
+000159e0: 2020 2020 2020 2020 2063 6f70 7966 696c           copyfil
+000159f0: 6528 574f 524b 494e 475f 5041 5448 202b  e(WORKING_PATH +
+00015a00: 2022 2f64 6174 6122 202b 206d 6163 726f   "/data" + macro
+00015a10: 5f66 696c 652c 2044 4154 415f 5041 5448  _file, DATA_PATH
+00015a20: 202b 206d 6163 726f 5f66 696c 6529 0a20   + macro_file). 
+00015a30: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
+00015a40: 2866 2278 6467 2d6f 7065 6e20 7b44 4154  (f"xdg-open {DAT
+00015a50: 415f 5041 5448 7d7b 6d61 6372 6f5f 6669  A_PATH}{macro_fi
+00015a60: 6c65 7d22 290a 0a20 2020 2064 6566 2072  le}")..    def r
+00015a70: 6561 645f 6377 5f6d 6163 726f 7328 7365  ead_cw_macros(se
+00015a80: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00015a90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00015aa0: 2052 6561 6473 2069 6e20 7468 6520 4357   Reads in the CW
+00015ab0: 206d 6163 726f 732c 2066 6972 7374 7320   macros, firsts 
+00015ac0: 6974 2063 6865 636b 7320 746f 2073 6565  it checks to see
+00015ad0: 2069 6620 7468 6520 6669 6c65 2065 7869   if the file exi
+00015ae0: 7374 732e 2049 6620 6974 2064 6f65 7320  sts. If it does 
+00015af0: 6e6f 742c 0a20 2020 2020 2020 2061 6e64  not,.        and
+00015b00: 2074 6869 7320 6861 7320 6265 656e 2070   this has been p
+00015b10: 6163 6b61 6765 6420 7769 7468 2070 7969  ackaged with pyi
+00015b20: 6e73 7461 6c6c 6572 2069 7420 7769 6c6c  nstaller it will
+00015b30: 2063 6f70 7920 7468 6520 6465 6661 756c   copy the defaul
+00015b40: 7420 6669 6c65 2066 726f 6d20 7468 650a  t file from the.
+00015b50: 2020 2020 2020 2020 7465 6d70 2064 6972          temp dir
+00015b60: 6563 746f 7279 2074 6869 7320 6973 2072  ectory this is r
+00015b70: 756e 6e69 6e67 2066 726f 6d2e 2e2e 2049  unning from... I
+00015b80: 6e20 7468 656f 7279 2e0a 2020 2020 2020  n theory..      
+00015b90: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+00015ba0: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+00015bb0: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+00015bc0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00015bd0: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
+00015be0: 2022 2f63 776d 6163 726f 732e 7478 7422   "/cwmacros.txt"
+00015bf0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00015c00: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+00015c10: 5f66 696c 6520 3d20 222f 7373 626d 6163  _file = "/ssbmac
+00015c20: 726f 732e 7478 7422 0a0a 2020 2020 2020  ros.txt"..      
+00015c30: 2020 6966 206e 6f74 2050 6174 6828 4441    if not Path(DA
+00015c40: 5441 5f50 4154 4820 2b20 6d61 6372 6f5f  TA_PATH + macro_
+00015c50: 6669 6c65 292e 6578 6973 7473 2829 3a0a  file).exists():.
+00015c60: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00015c70: 6572 2e64 6562 7567 2822 7265 6164 5f63  er.debug("read_c
+00015c80: 775f 6d61 6372 6f73 3a20 636f 7079 696e  w_macros: copyin
+00015c90: 6720 6465 6661 756c 7420 6d61 6372 6f20  g default macro 
+00015ca0: 6669 6c65 2e22 290a 2020 2020 2020 2020  file.").        
+00015cb0: 2020 2020 636f 7079 6669 6c65 2857 4f52      copyfile(WOR
+00015cc0: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
+00015cd0: 7461 2220 2b20 6d61 6372 6f5f 6669 6c65  ta" + macro_file
+00015ce0: 2c20 4441 5441 5f50 4154 4820 2b20 6d61  , DATA_PATH + ma
+00015cf0: 6372 6f5f 6669 6c65 290a 2020 2020 2020  cro_file).      
+00015d00: 2020 7769 7468 206f 7065 6e28 4441 5441    with open(DATA
+00015d10: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
+00015d20: 6c65 2c20 2272 222c 2065 6e63 6f64 696e  le, "r", encodin
+00015d30: 673d 2275 7466 2d38 2229 2061 7320 6669  g="utf-8") as fi
+00015d40: 6c65 5f64 6573 6372 6970 746f 723a 0a20  le_descriptor:. 
+00015d50: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+00015d60: 696e 6520 696e 2066 696c 655f 6465 7363  ine in file_desc
+00015d70: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
+00015d80: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00015d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015da0: 206d 6f64 652c 2066 6b65 792c 2062 7574   mode, fkey, but
+00015db0: 746f 6e6e 616d 652c 2063 7774 6578 7420  tonname, cwtext 
+00015dc0: 3d20 6c69 6e65 2e73 706c 6974 2822 7c22  = line.split("|"
+00015dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015de0: 2020 2020 2020 6966 206d 6f64 652e 7374        if mode.st
+00015df0: 7269 7028 292e 7570 7065 7228 2920 3d3d  rip().upper() ==
+00015e00: 2022 5222 2061 6e64 2073 656c 662e 7072   "R" and self.pr
+00015e10: 6566 2e67 6574 2822 7275 6e5f 7374 6174  ef.get("run_stat
+00015e20: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+00015e30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015e40: 662e 666b 6579 735b 666b 6579 2e73 7472  f.fkeys[fkey.str
+00015e50: 6970 2829 5d20 3d20 2862 7574 746f 6e6e  ip()] = (buttonn
+00015e60: 616d 652e 7374 7269 7028 292c 2063 7774  ame.strip(), cwt
+00015e70: 6578 742e 7374 7269 7028 2929 0a20 2020  ext.strip()).   
+00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e90: 2069 6620 6d6f 6465 2e73 7472 6970 2829   if mode.strip()
+00015ea0: 2e75 7070 6572 2829 2021 3d20 2252 2220  .upper() != "R" 
+00015eb0: 616e 6420 6e6f 7420 7365 6c66 2e70 7265  and not self.pre
+00015ec0: 662e 6765 7428 2272 756e 5f73 7461 7465  f.get("run_state
+00015ed0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00015ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015ef0: 2e66 6b65 7973 5b66 6b65 792e 7374 7269  .fkeys[fkey.stri
+00015f00: 7028 295d 203d 2028 6275 7474 6f6e 6e61  p()] = (buttonna
+00015f10: 6d65 2e73 7472 6970 2829 2c20 6377 7465  me.strip(), cwte
+00015f20: 7874 2e73 7472 6970 2829 290a 2020 2020  xt.strip()).    
+00015f30: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00015f40: 7074 2056 616c 7565 4572 726f 7220 6173  pt ValueError as
+00015f50: 2065 7272 3a0a 2020 2020 2020 2020 2020   err:.          
+00015f60: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00015f70: 2e69 6e66 6f28 2272 6561 645f 6377 5f6d  .info("read_cw_m
+00015f80: 6163 726f 733a 2025 7322 2c20 6572 7229  acros: %s", err)
+00015f90: 0a20 2020 2020 2020 206b 6579 7320 3d20  .        keys = 
+00015fa0: 7365 6c66 2e66 6b65 7973 2e6b 6579 7328  self.fkeys.keys(
+00015fb0: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
+00015fc0: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+00015fd0: 2020 2020 2020 2073 656c 662e 4631 2e73         self.F1.s
+00015fe0: 6574 5465 7874 2866 2246 313a 207b 7365  etText(f"F1: {se
+00015ff0: 6c66 2e66 6b65 7973 5b27 4631 275d 5b30  lf.fkeys['F1'][0
+00016000: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00016010: 2073 656c 662e 4631 2e73 6574 546f 6f6c   self.F1.setTool
+00016020: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+00016030: 4631 225d 5b31 5d29 0a20 2020 2020 2020  F1"][1]).       
+00016040: 2069 6620 2246 3222 2069 6e20 6b65 7973   if "F2" in keys
+00016050: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016060: 6c66 2e46 322e 7365 7454 6578 7428 6622  lf.F2.setText(f"
+00016070: 4632 3a20 7b73 656c 662e 666b 6579 735b  F2: {self.fkeys[
+00016080: 2746 3227 5d5b 305d 7d22 290a 2020 2020  'F2'][0]}").    
+00016090: 2020 2020 2020 2020 7365 6c66 2e46 322e          self.F2.
+000160a0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+000160b0: 666b 6579 735b 2246 3222 5d5b 315d 290a  fkeys["F2"][1]).
+000160c0: 2020 2020 2020 2020 6966 2022 4633 2220          if "F3" 
+000160d0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
+000160e0: 2020 2020 2073 656c 662e 4633 2e73 6574       self.F3.set
+000160f0: 5465 7874 2866 2246 333a 207b 7365 6c66  Text(f"F3: {self
+00016100: 2e66 6b65 7973 5b27 4633 275d 5b30 5d7d  .fkeys['F3'][0]}
+00016110: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00016120: 656c 662e 4633 2e73 6574 546f 6f6c 5469  elf.F3.setToolTi
+00016130: 7028 7365 6c66 2e66 6b65 7973 5b22 4633  p(self.fkeys["F3
+00016140: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
+00016150: 6620 2246 3422 2069 6e20 6b65 7973 3a0a  f "F4" in keys:.
+00016160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016170: 2e46 342e 7365 7454 6578 7428 6622 4634  .F4.setText(f"F4
+00016180: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+00016190: 3427 5d5b 305d 7d22 290a 2020 2020 2020  4'][0]}").      
+000161a0: 2020 2020 2020 7365 6c66 2e46 342e 7365        self.F4.se
+000161b0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+000161c0: 6579 735b 2246 3422 5d5b 315d 290a 2020  eys["F4"][1]).  
+000161d0: 2020 2020 2020 6966 2022 4635 2220 696e        if "F5" in
+000161e0: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+000161f0: 2020 2073 656c 662e 4635 2e73 6574 5465     self.F5.setTe
+00016200: 7874 2866 2246 353a 207b 7365 6c66 2e66  xt(f"F5: {self.f
+00016210: 6b65 7973 5b27 4635 275d 5b30 5d7d 2229  keys['F5'][0]}")
+00016220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016230: 662e 4635 2e73 6574 546f 6f6c 5469 7028  f.F5.setToolTip(
+00016240: 7365 6c66 2e66 6b65 7973 5b22 4635 225d  self.fkeys["F5"]
+00016250: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+00016260: 2246 3622 2069 6e20 6b65 7973 3a0a 2020  "F6" in keys:.  
+00016270: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+00016280: 362e 7365 7454 6578 7428 6622 4636 3a20  6.setText(f"F6: 
+00016290: 7b73 656c 662e 666b 6579 735b 2746 3627  {self.fkeys['F6'
+000162a0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+000162b0: 2020 2020 7365 6c66 2e46 362e 7365 7454      self.F6.setT
+000162c0: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+000162d0: 735b 2246 3622 5d5b 315d 290a 2020 2020  s["F6"][1]).    
+000162e0: 2020 2020 6966 2022 4637 2220 696e 206b      if "F7" in k
+000162f0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+00016300: 2073 656c 662e 4637 2e73 6574 5465 7874   self.F7.setText
+00016310: 2866 2246 373a 207b 7365 6c66 2e66 6b65  (f"F7: {self.fke
+00016320: 7973 5b27 4637 275d 5b30 5d7d 2229 0a20  ys['F7'][0]}"). 
+00016330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016340: 4637 2e73 6574 546f 6f6c 5469 7028 7365  F7.setToolTip(se
+00016350: 6c66 2e66 6b65 7973 5b22 4637 225d 5b31  lf.fkeys["F7"][1
+00016360: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+00016370: 3822 2069 6e20 6b65 7973 3a0a 2020 2020  8" in keys:.    
+00016380: 2020 2020 2020 2020 7365 6c66 2e46 382e          self.F8.
+00016390: 7365 7454 6578 7428 6622 4638 3a20 7b73  setText(f"F8: {s
+000163a0: 656c 662e 666b 6579 735b 2746 3827 5d5b  elf.fkeys['F8'][
+000163b0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+000163c0: 2020 7365 6c66 2e46 382e 7365 7454 6f6f    self.F8.setToo
+000163d0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+000163e0: 2246 3822 5d5b 315d 290a 2020 2020 2020  "F8"][1]).      
+000163f0: 2020 6966 2022 4639 2220 696e 206b 6579    if "F9" in key
+00016400: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00016410: 656c 662e 4639 2e73 6574 5465 7874 2866  elf.F9.setText(f
+00016420: 2246 393a 207b 7365 6c66 2e66 6b65 7973  "F9: {self.fkeys
+00016430: 5b27 4639 275d 5b30 5d7d 2229 0a20 2020  ['F9'][0]}").   
+00016440: 2020 2020 2020 2020 2073 656c 662e 4639           self.F9
+00016450: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00016460: 2e66 6b65 7973 5b22 4639 225d 5b31 5d29  .fkeys["F9"][1])
+00016470: 0a20 2020 2020 2020 2069 6620 2246 3130  .        if "F10
+00016480: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+00016490: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
+000164a0: 7365 7454 6578 7428 6622 4631 303a 207b  setText(f"F10: {
+000164b0: 7365 6c66 2e66 6b65 7973 5b27 4631 3027  self.fkeys['F10'
+000164c0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+000164d0: 2020 2020 7365 6c66 2e46 3130 2e73 6574      self.F10.set
+000164e0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+000164f0: 7973 5b22 4631 3022 5d5b 315d 290a 2020  ys["F10"][1]).  
+00016500: 2020 2020 2020 6966 2022 4631 3122 2069        if "F11" i
+00016510: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00016520: 2020 2020 7365 6c66 2e46 3131 2e73 6574      self.F11.set
+00016530: 5465 7874 2866 2246 3131 3a20 7b73 656c  Text(f"F11: {sel
+00016540: 662e 666b 6579 735b 2746 3131 275d 5b30  f.fkeys['F11'][0
+00016550: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00016560: 2073 656c 662e 4631 312e 7365 7454 6f6f   self.F11.setToo
+00016570: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+00016580: 2246 3131 225d 5b31 5d29 0a20 2020 2020  "F11"][1]).     
+00016590: 2020 2069 6620 2246 3132 2220 696e 206b     if "F12" in k
+000165a0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+000165b0: 2073 656c 662e 4631 322e 7365 7454 6578   self.F12.setTex
+000165c0: 7428 6622 4631 323a 207b 7365 6c66 2e66  t(f"F12: {self.f
+000165d0: 6b65 7973 5b27 4631 3227 5d5b 305d 7d22  keys['F12'][0]}"
+000165e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000165f0: 6c66 2e46 3132 2e73 6574 546f 6f6c 5469  lf.F12.setToolTi
+00016600: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
+00016610: 3222 5d5b 315d 290a 0a20 2020 2064 6566  2"][1])..    def
+00016620: 2067 656e 6572 6174 655f 6164 6966 2873   generate_adif(s
+00016630: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00016640: 2247 656e 6572 6174 6520 4144 4946 2222  "Generate ADIF""
+00016650: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+00016660: 2e64 6562 7567 2822 2a2a 2a2a 2a2a 4144  .debug("******AD
+00016670: 4946 2a2a 2a2a 2a22 290a 2020 2020 2020  IF*****").      
+00016680: 2020 7365 6c66 2e63 6f6e 7465 7374 2e61    self.contest.a
+00016690: 6469 6628 7365 6c66 290a 0a20 2020 2064  dif(self)..    d
+000166a0: 6566 2067 656e 6572 6174 655f 6361 6272  ef generate_cabr
+000166b0: 696c 6c6f 2873 656c 6629 3a0a 2020 2020  illo(self):.    
+000166c0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
+000166d0: 2043 6162 7269 6c6c 6f20 6669 6c65 2e20   Cabrillo file. 
+000166e0: 4d61 7962 652e 2222 220a 2020 2020 2020  Maybe.""".      
+000166f0: 2020 2320 6874 7470 733a 2f2f 7777 772e    # https://www.
+00016700: 6371 7770 782e 636f 6d2f 6361 6272 696c  cqwpx.com/cabril
+00016710: 6c6f 2e68 746d 0a20 2020 2020 2020 206c  lo.htm.        l
+00016720: 6f67 6765 722e 6465 6275 6728 222a 2a2a  ogger.debug("***
+00016730: 2a2a 2a43 6162 7269 6c6c 6f2a 2a2a 2a2a  ***Cabrillo*****
+00016740: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00016750: 636f 6e74 6573 742e 6361 6272 696c 6c6f  contest.cabrillo
+00016760: 2873 656c 6629 0a0a 0a64 6566 206c 6f61  (self)...def loa
+00016770: 645f 666f 6e74 735f 6672 6f6d 5f64 6972  d_fonts_from_dir
+00016780: 2864 6972 6563 746f 7279 3a20 7374 7229  (directory: str)
+00016790: 202d 3e20 7365 743a 0a20 2020 2022 2222   -> set:.    """
+000167a0: 0a20 2020 2057 656c 6c20 6974 206c 6f61  .    Well it loa
+000167b0: 6473 2066 6f6e 7473 2066 726f 6d20 6120  ds fonts from a 
+000167c0: 6469 7265 6374 6f72 792e 2e2e 0a20 2020  directory....   
+000167d0: 2022 2222 0a20 2020 2066 6f6e 745f 6661   """.    font_fa
+000167e0: 6d69 6c69 6573 203d 2073 6574 2829 0a20  milies = set(). 
+000167f0: 2020 2066 6f72 205f 6669 2069 6e20 5144     for _fi in QD
+00016800: 6972 2864 6972 6563 746f 7279 292e 656e  ir(directory).en
+00016810: 7472 7949 6e66 6f4c 6973 7428 5b22 2a2e  tryInfoList(["*.
+00016820: 7474 6622 2c20 222a 2e77 6f66 6622 2c20  ttf", "*.woff", 
+00016830: 222a 2e77 6f66 6632 225d 293a 0a20 2020  "*.woff2"]):.   
+00016840: 2020 2020 205f 6964 203d 2051 466f 6e74       _id = QFont
+00016850: 4461 7461 6261 7365 2e61 6464 4170 706c  Database.addAppl
+00016860: 6963 6174 696f 6e46 6f6e 7428 5f66 692e  icationFont(_fi.
+00016870: 6162 736f 6c75 7465 4669 6c65 5061 7468  absoluteFilePath
+00016880: 2829 290a 2020 2020 2020 2020 666f 6e74  ()).        font
+00016890: 5f66 616d 696c 6965 7320 7c3d 2073 6574  _families |= set
+000168a0: 2851 466f 6e74 4461 7461 6261 7365 2e61  (QFontDatabase.a
+000168b0: 7070 6c69 6361 7469 6f6e 466f 6e74 4661  pplicationFontFa
+000168c0: 6d69 6c69 6573 285f 6964 2929 0a20 2020  milies(_id)).   
+000168d0: 2072 6574 7572 6e20 666f 6e74 5f66 616d   return font_fam
+000168e0: 696c 6965 730a 0a0a 6465 6620 696e 7374  ilies...def inst
+000168f0: 616c 6c5f 6963 6f6e 7328 293a 0a20 2020  all_icons():.   
+00016900: 2022 2222 496e 7374 616c 6c20 6963 6f6e   """Install icon
+00016910: 7322 2222 0a20 2020 206f 732e 7379 7374  s""".    os.syst
+00016920: 656d 280a 2020 2020 2020 2020 2278 6467  em(.        "xdg
+00016930: 2d69 636f 6e2d 7265 736f 7572 6365 2069  -icon-resource i
+00016940: 6e73 7461 6c6c 202d 2d73 697a 6520 3332  nstall --size 32
+00016950: 202d 2d63 6f6e 7465 7874 2061 7070 7320   --context apps 
+00016960: 2d2d 6d6f 6465 2075 7365 7220 220a 2020  --mode user ".  
+00016970: 2020 2020 2020 6622 7b57 4f52 4b49 4e47        f"{WORKING
+00016980: 5f50 4154 487d 2f64 6174 612f 6b36 6774  _PATH}/data/k6gt
+00016990: 652e 6e6f 7431 6d6d 2d33 322e 706e 6720  e.not1mm-32.png 
+000169a0: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
+000169b0: 2020 290a 2020 2020 6f73 2e73 7973 7465    ).    os.syste
+000169c0: 6d28 0a20 2020 2020 2020 2022 7864 672d  m(.        "xdg-
+000169d0: 6963 6f6e 2d72 6573 6f75 7263 6520 696e  icon-resource in
+000169e0: 7374 616c 6c20 2d2d 7369 7a65 2036 3420  stall --size 64 
+000169f0: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
+00016a00: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
+00016a10: 2020 2020 2066 227b 574f 524b 494e 475f       f"{WORKING_
+00016a20: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00016a30: 2e6e 6f74 316d 6d2d 3634 2e70 6e67 206b  .not1mm-64.png k
+00016a40: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+00016a50: 2029 0a20 2020 206f 732e 7379 7374 656d   ).    os.system
+00016a60: 280a 2020 2020 2020 2020 2278 6467 2d69  (.        "xdg-i
+00016a70: 636f 6e2d 7265 736f 7572 6365 2069 6e73  con-resource ins
+00016a80: 7461 6c6c 202d 2d73 697a 6520 3132 3820  tall --size 128 
+00016a90: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
+00016aa0: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
+00016ab0: 2020 2020 2066 227b 574f 524b 494e 475f       f"{WORKING_
+00016ac0: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00016ad0: 2e6e 6f74 316d 6d2d 3132 382e 706e 6720  .not1mm-128.png 
+00016ae0: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
+00016af0: 2020 290a 2020 2020 6f73 2e73 7973 7465    ).    os.syste
+00016b00: 6d28 6622 7864 672d 6465 736b 746f 702d  m(f"xdg-desktop-
+00016b10: 6d65 6e75 2069 6e73 7461 6c6c 207b 574f  menu install {WO
+00016b20: 524b 494e 475f 5041 5448 7d2f 6461 7461  RKING_PATH}/data
+00016b30: 2f6b 3667 7465 2d6e 6f74 316d 6d2e 6465  /k6gte-not1mm.de
+00016b40: 736b 746f 7022 290a 0a0a 6465 6620 646f  sktop")...def do
+00016b50: 696d 7028 6d6f 646e 616d 6529 3a0a 2020  imp(modname):.  
+00016b60: 2020 2222 2272 6574 7572 6e20 6d6f 6475    """return modu
+00016b70: 6c65 2070 6174 6822 2222 0a20 2020 2072  le path""".    r
+00016b80: 6574 7572 6e20 696d 706f 7274 6c69 622e  eturn importlib.
+00016b90: 696d 706f 7274 5f6d 6f64 756c 6528 6622  import_module(f"
+00016ba0: 6e6f 7431 6d6d 2e70 6c75 6769 6e73 2e7b  not1mm.plugins.{
+00016bb0: 6d6f 646e 616d 657d 2229 0a0a 0a64 6566  modname}")...def
+00016bc0: 2072 756e 2829 3a0a 2020 2020 2222 220a   run():.    """.
+00016bd0: 2020 2020 4d61 696e 2045 6e74 7279 0a20      Main Entry. 
+00016be0: 2020 2022 2222 0a20 2020 2069 6e73 7461     """.    insta
+00016bf0: 6c6c 5f69 636f 6e73 2829 0a20 2020 2074  ll_icons().    t
+00016c00: 696d 6572 2e73 7461 7274 2832 3530 290a  imer.start(250).
+00016c10: 2020 2020 7379 732e 6578 6974 2861 7070      sys.exit(app
+00016c20: 2e65 7865 6328 2929 0a0a 0a6c 6f67 6765  .exec())...logge
+00016c30: 7220 3d20 6c6f 6767 696e 672e 6765 744c  r = logging.getL
+00016c40: 6f67 6765 7228 225f 5f6d 6169 6e5f 5f22  ogger("__main__"
+00016c50: 290a 6861 6e64 6c65 7220 3d20 6c6f 6767  ).handler = logg
+00016c60: 696e 672e 5374 7265 616d 4861 6e64 6c65  ing.StreamHandle
+00016c70: 7228 290a 666f 726d 6174 7465 7220 3d20  r().formatter = 
+00016c80: 6c6f 6767 696e 672e 466f 726d 6174 7465  logging.Formatte
+00016c90: 7228 0a20 2020 2064 6174 6566 6d74 3d22  r(.    datefmt="
+00016ca0: 2548 3a25 4d3a 2553 222c 0a20 2020 2066  %H:%M:%S",.    f
+00016cb0: 6d74 3d22 5b25 2861 7363 7469 6d65 2973  mt="[%(asctime)s
+00016cc0: 5d20 2528 6c65 7665 6c6e 616d 6529 7320  ] %(levelname)s 
+00016cd0: 2528 6d6f 6475 6c65 2973 202d 2025 2866  %(module)s - %(f
+00016ce0: 756e 634e 616d 6529 7320 4c69 6e65 2025  uncName)s Line %
+00016cf0: 286c 696e 656e 6f29 643a 2025 286d 6573  (lineno)d: %(mes
+00016d00: 7361 6765 2973 222c 0a29 0a68 616e 646c  sage)s",.).handl
+00016d10: 6572 2e73 6574 466f 726d 6174 7465 7228  er.setFormatter(
+00016d20: 666f 726d 6174 7465 7229 0a6c 6f67 6765  formatter).logge
+00016d30: 722e 6164 6448 616e 646c 6572 2868 616e  r.addHandler(han
+00016d40: 646c 6572 290a 0a42 4554 415f 5445 5354  dler)..BETA_TEST
+00016d50: 203d 2046 616c 7365 0a69 6620 5061 7468   = False.if Path
+00016d60: 2822 2e2f 6265 7461 7465 7374 2229 2e65  ("./betatest").e
+00016d70: 7869 7374 7328 293a 0a20 2020 2042 4554  xists():.    BET
+00016d80: 415f 5445 5354 203d 2054 7275 650a 0a69  A_TEST = True..i
+00016d90: 6620 5061 7468 2822 2e2f 6465 6275 6722  f Path("./debug"
+00016da0: 292e 6578 6973 7473 2829 3a0a 2020 2020  ).exists():.    
+00016db0: 6c6f 6767 6572 2e73 6574 4c65 7665 6c28  logger.setLevel(
+00016dc0: 6c6f 6767 696e 672e 4445 4255 4729 0a20  logging.DEBUG). 
+00016dd0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00016de0: 2264 6562 7567 6769 6e67 206f 6e22 290a  "debugging on").
+00016df0: 656c 7365 3a0a 2020 2020 6c6f 6767 6572  else:.    logger
+00016e00: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
+00016e10: 672e 5741 524e 494e 4729 0a20 2020 206c  g.WARNING).    l
+00016e20: 6f67 6765 722e 7761 726e 696e 6728 2264  ogger.warning("d
+00016e30: 6562 7567 6769 6e67 206f 6666 2229 0a0a  ebugging off")..
+00016e40: 6170 7020 3d20 5174 5769 6467 6574 732e  app = QtWidgets.
+00016e50: 5141 7070 6c69 6361 7469 6f6e 2873 7973  QApplication(sys
+00016e60: 2e61 7267 7629 0a61 7070 2e73 6574 5374  .argv).app.setSt
+00016e70: 796c 6528 2241 6477 6169 7461 2d44 6172  yle("Adwaita-Dar
+00016e80: 6b22 290a 666f 6e74 5f70 6174 6820 3d20  k").font_path = 
+00016e90: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
+00016ea0: 2f64 6174 6122 0a66 616d 696c 6965 7320  /data".families 
+00016eb0: 3d20 6c6f 6164 5f66 6f6e 7473 5f66 726f  = load_fonts_fro
+00016ec0: 6d5f 6469 7228 6f73 2e66 7370 6174 6828  m_dir(os.fspath(
+00016ed0: 666f 6e74 5f70 6174 6829 290a 6c6f 6767  font_path)).logg
+00016ee0: 6572 2e69 6e66 6f28 6661 6d69 6c69 6573  er.info(families
+00016ef0: 290a 7769 6e64 6f77 203d 204d 6169 6e57  ).window = MainW
+00016f00: 696e 646f 7728 290a 6865 6967 6874 203d  indow().height =
+00016f10: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
+00016f20: 2822 7769 6e64 6f77 5f68 6569 6768 7422  ("window_height"
+00016f30: 2c20 3330 3029 0a77 6964 7468 203d 2077  , 300).width = w
+00016f40: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
+00016f50: 7769 6e64 6f77 5f77 6964 7468 222c 2037  window_width", 7
+00016f60: 3030 290a 7820 3d20 7769 6e64 6f77 2e70  00).x = window.p
+00016f70: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
+00016f80: 7822 2c20 2d31 290a 7920 3d20 7769 6e64  x", -1).y = wind
+00016f90: 6f77 2e70 7265 662e 6765 7428 2277 696e  ow.pref.get("win
+00016fa0: 646f 775f 7922 2c20 2d31 290a 7769 6e64  dow_y", -1).wind
+00016fb0: 6f77 2e73 6574 4765 6f6d 6574 7279 2878  ow.setGeometry(x
+00016fc0: 2c20 792c 2077 6964 7468 2c20 6865 6967  , y, width, heig
+00016fd0: 6874 290a 7769 6e64 6f77 2e63 616c 6c73  ht).window.calls
+00016fe0: 6967 6e2e 7365 7446 6f63 7573 2829 0a77  ign.setFocus().w
+00016ff0: 696e 646f 772e 7368 6f77 2829 0a74 696d  indow.show().tim
+00017000: 6572 203d 2051 7443 6f72 652e 5154 696d  er = QtCore.QTim
+00017010: 6572 2829 0a74 696d 6572 2e74 696d 656f  er().timer.timeo
+00017020: 7574 2e63 6f6e 6e65 6374 2877 696e 646f  ut.connect(windo
+00017030: 772e 706f 6c6c 5f72 6164 696f 290a 0a69  w.poll_radio)..i
+00017040: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+00017050: 5f6d 6169 6e5f 5f22 3a0a 2020 2020 7275  _main__":.    ru
+00017060: 6e28 290a                                n().
```

### Comparing `not1mm-23.6.30.1/not1mm/bandmap.py` & `not1mm-23.7.2/not1mm/bandmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,14 @@
         self.spots = Database()
         self.bandmap_scene = QtWidgets.QGraphicsScene()
         self.socket = QtNetwork.QTcpSocket()
         self.socket.readyRead.connect(self.receive)
         self.socket.connected.connect(self.maybeconnected)
         self.socket.disconnected.connect(self.disconnected)
         self.socket.errorOccurred.connect(self.socket_error)
-        # self.socket.connectToHost("hamqth.com", 7300)
         self.bandmap_scene.clear()
         self.bandmap_scene.setFocusOnTouch(False)
         self.bandmap_scene.selectionChanged.connect(self.spot_clicked)
         self.freq = 0.0
         self.keepRXCenter = False
         self.update_timer = QtCore.QTimer()
         self.update_timer.timeout.connect(self.update_station_timer)
@@ -254,14 +253,15 @@
         self.udpsocket.bind(
             QtNetwork.QHostAddress.AnyIPv4,
             MULTICAST_PORT,
             QtNetwork.QUdpSocket.ShareAddress,
         )
         self.udpsocket.joinMulticastGroup(QtNetwork.QHostAddress(MULTICAST_GROUP))
         self.udpsocket.readyRead.connect(self.watch_udp)
+        self.request_workedlist()
 
     def connect(self):
         """doc"""
         if self.connected is True:
             self.socket.close()
             self.connected = False
             self.connectButton.setStyleSheet("color: red;")
@@ -393,14 +393,24 @@
                 cmd["freq"] = items[0].property("freq")
                 cmd["spot"] = items[0].toPlainText().split()[0]
                 packet = bytes(dumps(cmd), encoding="ascii")
                 self.udpsocket.writeDatagram(
                     packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
                 )
 
+    def request_workedlist(self):
+        """Request worked call list from logger"""
+        cmd = {}
+        cmd["cmd"] = "GETWORKEDLIST"
+        cmd["station"] = platform.node()
+        packet = bytes(dumps(cmd), encoding="ascii")
+        self.udpsocket.writeDatagram(
+            packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
+        )
+
     def update_station_timer(self):
         """doc"""
         self.update_stations()
 
     def update(self):
         """doc"""
         self.update_timer.setInterval(UPDATE_INTERVAL)
@@ -553,23 +563,19 @@
         step, _digits = self.determine_step_digits()
 
         result = self.spots.getspotsinband(self.currentBand.start, self.currentBand.end)
         entity = ""
         if result:
             min_y = 0.0
             for items in result:
-                # lookup = cty_lookup(items.get("callsign"))
-                # if lookup:
-                #     for a in lookup.items():
-                #         entity = a[1].get("entity", "")
                 pen_color = QtGui.QColor(192, 192, 192)
                 if items.get("callsign") in self.worked_list:
                     call_bandlist = self.worked_list.get(items.get("callsign"))
                     if self.currentBand.altname in call_bandlist:
-                        pen_color = QtGui.QColor(192, 25, 25)
+                        pen_color = QtGui.QColor(255, 47, 47)
                 freq_y = (
                     (items.get("freq") - self.currentBand.start) / step
                 ) * PIXELSPERSTEP
                 text_y = max(min_y + 5, freq_y)
                 self.lineitemlist.append(
                     self.bandmap_scene.addLine(
                         22, freq_y, 55, text_y, QtGui.QPen(pen_color)
@@ -589,18 +595,14 @@
                     | QtWidgets.QGraphicsItem.ItemIsSelectable
                     | text.flags()
                 )
                 text.setProperty("freq", items.get("freq"))
                 text.setToolTip(items.get("comment"))
                 text.setDefaultTextColor(pen_color)
                 min_y = text_y + text.boundingRect().height() / 2
-
-                # textColor = Data::statusToColor(lower.value().status,
-                # qApp->palette().color(QPalette::Text));
-                # text->setDefaultTextColor(textColor);
                 self.textItemList.append(text)
 
     def determine_step_digits(self):
         """doc"""
         return_zoom = {
             1: (0.0001, 4),
             2: (0.00025, 4),
```

### Comparing `not1mm-23.6.30.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.7.2/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/MASTER.SCP` & `not1mm-23.7.2/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/about.ui` & `not1mm-23.7.2/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/bandmap.ui` & `not1mm-23.7.2/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/configuration.ui` & `not1mm-23.7.2/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/contests.sql` & `not1mm-23.7.2/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/cty.json` & `not1mm-23.7.2/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/editcontact.ui` & `not1mm-23.7.2/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/editmacro.ui` & `not1mm-23.7.2/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.7.2/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.7.2/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.7.2/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/logwindow.ui` & `not1mm-23.7.2/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/main.ui` & `not1mm-23.7.2/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/new_contest.ui` & `not1mm-23.7.2/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/not1mm.html` & `not1mm-23.7.2/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/opon.ui` & `not1mm-23.7.2/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/0.wav` & `not1mm-23.7.2/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/1.wav` & `not1mm-23.7.2/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/2.wav` & `not1mm-23.7.2/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/3.wav` & `not1mm-23.7.2/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/4.wav` & `not1mm-23.7.2/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/5.wav` & `not1mm-23.7.2/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/6.wav` & `not1mm-23.7.2/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/7.wav` & `not1mm-23.7.2/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/73.wav` & `not1mm-23.7.2/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/8.wav` & `not1mm-23.7.2/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/9.wav` & `not1mm-23.7.2/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/a.wav` & `not1mm-23.7.2/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/again.wav` & `not1mm-23.7.2/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/b.wav` & `not1mm-23.7.2/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/c.wav` & `not1mm-23.7.2/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/contest.wav` & `not1mm-23.7.2/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/cq.wav` & `not1mm-23.7.2/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/d.wav` & `not1mm-23.7.2/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/e.wav` & `not1mm-23.7.2/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/f.wav` & `not1mm-23.7.2/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/g.wav` & `not1mm-23.7.2/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/h.wav` & `not1mm-23.7.2/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/i.wav` & `not1mm-23.7.2/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/j.wav` & `not1mm-23.7.2/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/k.wav` & `not1mm-23.7.2/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.7.2/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/l.wav` & `not1mm-23.7.2/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/m.wav` & `not1mm-23.7.2/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.7.2/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/n.wav` & `not1mm-23.7.2/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/nil.wav` & `not1mm-23.7.2/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/o.wav` & `not1mm-23.7.2/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/p.wav` & `not1mm-23.7.2/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/q.wav` & `not1mm-23.7.2/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/r.wav` & `not1mm-23.7.2/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/roger.wav` & `not1mm-23.7.2/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/s.wav` & `not1mm-23.7.2/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/space.wav` & `not1mm-23.7.2/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/t.wav` & `not1mm-23.7.2/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.7.2/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.7.2/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/u.wav` & `not1mm-23.7.2/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/v.wav` & `not1mm-23.7.2/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/w.wav` & `not1mm-23.7.2/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/x.wav` & `not1mm-23.7.2/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/y.wav` & `not1mm-23.7.2/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.7.2/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/phonetics/z.wav` & `not1mm-23.7.2/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/pickcontest.ui` & `not1mm-23.7.2/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/reddot.png` & `not1mm-23.7.2/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/data/settings.ui` & `not1mm-23.7.2/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/cat_interface.py` & `not1mm-23.7.2/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/cwinterface.py` & `not1mm-23.7.2/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/database.py` & `not1mm-23.7.2/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/edit_macro.py` & `not1mm-23.7.2/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/edit_station.py` & `not1mm-23.7.2/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/ham_utility.py` & `not1mm-23.7.2/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/lookup.py` & `not1mm-23.7.2/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/multicast.py` & `not1mm-23.7.2/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/n1mm.py` & `not1mm-23.7.2/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/settings.py` & `not1mm-23.7.2/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/lib/versiontest.py` & `not1mm-23.7.2/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/logwindow.py` & `not1mm-23.7.2/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.7.2/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.7.2/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.7.2/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.7.2/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.7.2/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.7.2/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_field_day.py` & `not1mm-23.7.2/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.7.2/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.7.2/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.7.2/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/canada_day.py` & `not1mm-23.7.2/not1mm/plugins/canada_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.7.2/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.7.2/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.7.2/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.7.2/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/cwt.py` & `not1mm-23.7.2/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/general_logging.py` & `not1mm-23.7.2/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/jidx_cw.py` & `not1mm-23.7.2/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/jidx_ph.py` & `not1mm-23.7.2/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/plugins/winter_field_day.py` & `not1mm-23.7.2/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/testing/fakeflrig.py` & `not1mm-23.7.2/not1mm/testing/fakeflrig.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/testing/flrigclient.py` & `not1mm-23.7.2/not1mm/testing/flrigclient.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/testing/multicast_listener.py` & `not1mm-23.7.2/not1mm/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/testing/n1mm_listener.py` & `not1mm-23.7.2/not1mm/testing/n1mm_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm/testing/test.py` & `not1mm-23.7.2/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/not1mm.egg-info/PKG-INFO` & `not1mm-23.7.2/not1mm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.30.1
+Version: 23.7.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -74,15 +74,15 @@
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
-    - [Bandmap](#bandmap)
+  - [Bandmap](#bandmap)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -132,24 +132,17 @@
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 - RAC Canada Day
 
 ## Recent Changes
 
-- [23-6-30] Added RAC Canada Day.
-- [23-6-28] bandmap now displays callsigns in red if they have been worked before.
-- [23-6-21] cty updater needs work changed to ondemand.
-- [23-6-18] Pinned lib notctyparser to >= 26.6.18. Fix bug allowing editing RST field.
-- [23-6-17] Trapped ValueError from notctyparser when environment variable `LC_TIME` set to `lt_LT.UTF-8`.
-- [23-6-16] Send F1-12 button text, not tooltip in RadioInfo packet. Add `File->Update MASTER.SCP`. Add `Help->Help`
-- [23-6-15] Add `Help->HotKeys`.
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
-- [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
+- [23-7-2] bandmap now requests worked list at startup.
+
+See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
 ### Python and pip
 
 This software is a Python package hosted on PyPi, and installable with the pip or pipx command. If this is your first exposure to pip you can get all the details from [The PyPA](https://packaging.python.org/en/latest/tutorials/installing-packages/). In short, most linux distros come with Python pre installed. If pip is not installed by default, you can usually load it through your package manager. For example `sudo apt install python3-pip` or `sudo dnf install python3-pip`.
 
@@ -449,24 +442,30 @@
 
 You can not directly edit the multiplier status of a contact. Instead see the next section on recalculating mults. If you change the callsign make sure the `WPX` field is still valid.
 
 ## Recalulate Mults
 
 After editing a contact and before generating a Cabrillo file. There is a Misc menu option that will recalculate the multipliers incase an edit had caused a change.
 
-### Bandmap
+## Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
+VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth.
+
+![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/VFO_and_bandwidth_markers.png)
+
+Clicked on spots now tune the radio and set the callsign field. Previously worked calls are displayed in red.
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.6.30.1/not1mm.egg-info/SOURCES.txt` & `not1mm-23.7.2/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.30.1/pyproject.toml` & `not1mm-23.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.6.30.1"
+version = "23.7.2"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

