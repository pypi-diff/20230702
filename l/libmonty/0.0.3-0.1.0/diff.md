# Comparing `tmp/libmonty-0.0.3.tar.gz` & `tmp/libmonty-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmonty-0.0.3.tar", last modified: Tue Jun 13 11:03:18 2023, max compression
+gzip compressed data, was "libmonty-0.1.0.tar", last modified: Sun Jul  2 11:30:59 2023, max compression
```

## Comparing `libmonty-0.0.3.tar` & `libmonty-0.1.0.tar`

### file list

```diff
@@ -1,70 +1,56 @@
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.528770 libmonty-0.0.3/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2021-12-20 00:21:09.000000 libmonty-0.0.3/LICENSE
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        2 2023-06-12 05:01:39.000000 libmonty-0.0.3/MANIFEST.in
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1913 2023-06-13 11:03:18.528770 libmonty-0.0.3/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      954 2023-06-13 10:43:12.000000 libmonty-0.0.3/README.md
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2021-12-16 04:36:50.000000 libmonty-0.0.3/pyproject.toml
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       77 2023-06-12 04:35:21.000000 libmonty-0.0.3/requirements.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1570 2023-06-13 11:03:18.528770 libmonty-0.0.3/setup.cfg
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.504770 libmonty-0.0.3/src/
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:31:14.000000 libmonty-0.0.3/src/libmonty/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1241 2023-06-12 05:33:33.000000 libmonty-0.0.3/src/libmonty/__main__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/environment/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/environment/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      575 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/environment/terminal.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty/fileformats/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-25 12:40:19.000000 libmonty-0.0.3/src/libmonty/fileformats/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    10020 2022-09-25 13:21:40.000000 libmonty-0.0.3/src/libmonty/fileformats/oab_process.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/filesystem/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/filesystem/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1797 2022-01-24 20:01:35.000000 libmonty-0.0.3/src/libmonty/filesystem/copy_stubs.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3264 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/filesystem/directory.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3845 2022-09-23 23:06:46.000000 libmonty-0.0.3/src/libmonty/filesystem/tree_exec.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/formatting/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1390 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/char_str.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      754 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/formatting/debugging.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1338 2021-12-20 00:53:31.000000 libmonty-0.0.3/src/libmonty/formatting/json.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2147 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/formatting/number_str.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.512770 libmonty-0.0.3/src/libmonty/images/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/images/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4206 2021-12-20 04:06:39.000000 libmonty-0.0.3/src/libmonty/images/colors_named.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1068 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/images/convert_from_stream.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.516770 libmonty-0.0.3/src/libmonty/network/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/network/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    36448 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/network/responses.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.516770 libmonty-0.0.3/src/libmonty/outpututils/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 01:03:42.000000 libmonty-0.0.3/src/libmonty/outpututils/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4853 2021-12-20 04:06:40.000000 libmonty-0.0.3/src/libmonty/outpututils/asciistyling.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     5179 2021-12-20 06:35:07.000000 libmonty-0.0.3/src/libmonty/outpututils/decorators.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      580 2022-10-02 12:32:54.000000 libmonty-0.0.3/src/libmonty/outpututils/discord.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty/sound/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-23 22:47:02.000000 libmonty-0.0.3/src/libmonty/sound/__init__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty/sound/formats/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty/sound/formats/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    12704 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty/sound/formats/wave_pcm.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      318 2023-06-12 04:35:09.000000 libmonty-0.0.3/src/libmonty/version.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.508770 libmonty-0.0.3/src/libmonty.egg-info/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1913 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1845 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/SOURCES.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/dependency_links.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      222 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/entry_points.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       69 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/requires.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       47 2023-06-13 11:03:18.000000 libmonty-0.0.3/src/libmonty.egg-info/top_level.txt
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.520770 libmonty-0.0.3/src/libmonty_easypass/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-24 21:02:31.000000 libmonty-0.0.3/src/libmonty_easypass/__init__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.524770 libmonty-0.0.3/src/libmonty_easypass/data/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    87335 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/agr-wordlist-en-alt-edited-by-alan-beale.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    87393 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/agr-wordlist-en-original.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)   108800 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-large-wordlist.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    13660 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-short-wordlist-1.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    17258 2021-06-15 09:07:49.000000 libmonty-0.0.3/src/libmonty_easypass/data/eff-short-wordlist-2-0.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1737 2022-09-24 22:16:34.000000 libmonty-0.0.3/src/libmonty_easypass/dice_methods.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     5861 2022-09-25 01:05:57.000000 libmonty-0.0.3/src/libmonty_easypass/easypass.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:03:18.528770 libmonty-0.0.3/src/libmonty_soundboard/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2441 2023-06-12 05:34:18.000000 libmonty-0.0.3/src/libmonty_soundboard/__main__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1496 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/config.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1323 2022-09-14 19:12:57.000000 libmonty-0.0.3/src/libmonty_soundboard/sound.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      329 2023-06-12 04:43:03.000000 libmonty-0.0.3/src/libmonty_soundboard/version.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2023-07-02 09:06:06.000000 libmonty-0.1.0/LICENSE
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        2 2023-07-02 09:06:06.000000 libmonty-0.1.0/MANIFEST.in
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1840 2023-07-02 11:30:59.767376 libmonty-0.1.0/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      873 2023-07-02 11:08:36.000000 libmonty-0.1.0/README.md
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2023-07-02 09:06:06.000000 libmonty-0.1.0/pyproject.toml
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      105 2023-07-02 11:13:12.000000 libmonty-0.1.0/requirements.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1297 2023-07-02 11:30:59.767376 libmonty-0.1.0/setup.cfg
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.759376 libmonty-0.1.0/src/
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.763376 libmonty-0.1.0/src/libmonty/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1195 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/__main__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.763376 libmonty-0.1.0/src/libmonty/environment/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/environment/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      582 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/environment/arguments.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      553 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/environment/terminal.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/fileformats/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/fileformats/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    10742 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/fileformats/oab_process.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/filesystem/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/filesystem/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1921 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/filesystem/copy_stubs.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3895 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/filesystem/directory.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4325 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/filesystem/tree_exec.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/formatting/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/formatting/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1504 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/formatting/char_str.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      958 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/formatting/debugging.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1341 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/formatting/json.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2263 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/formatting/number_str.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/images/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/images/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4163 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/images/colors_named.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1079 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/images/convert_from_stream.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/network/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/network/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2270 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/network/email_check.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    36471 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/network/responses.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/outpututils/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/outpututils/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     4528 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/outpututils/asciistyling.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     6146 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/outpututils/decorators.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      759 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/outpututils/discord.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/sound/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/sound/__init__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.767376 libmonty-0.1.0/src/libmonty/sound/formats/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/sound/formats/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    14113 2023-07-02 09:06:06.000000 libmonty-0.1.0/src/libmonty/sound/formats/wave_pcm.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      361 2023-07-02 11:13:12.000000 libmonty-0.1.0/src/libmonty/version.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 11:30:59.763376 libmonty-0.1.0/src/libmonty.egg-info/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1840 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1355 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/SOURCES.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/dependency_links.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      166 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/entry_points.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       95 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/requires.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        9 2023-07-02 11:30:59.000000 libmonty-0.1.0/src/libmonty.egg-info/top_level.txt
```

### Comparing `libmonty-0.0.3/LICENSE` & `libmonty-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libmonty-0.0.3/PKG-INFO` & `libmonty-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: libmonty
-Version: 0.0.3
-Summary: libmonty - a collection of Python tools
-Home-page: https://github.com/sunarch/libmonty
+Version: 0.1.0
+Summary: libmonty - a collection of Python libraries
+Home-page: https://codeberg.org/sunarch/libmonty
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
-Project-URL: Bug Tracker, https://github.com/sunarch/libmonty/issues
+Project-URL: Bug Tracker, https://codeberg.org/sunarch/libmonty/issues
 Keywords: libmonty
 Platform: Any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,19 +24,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty - Python libraries
 
 Python libraries
 
-## parts
-
-- [libmonty-easypass](easypass.md)
-    - a passphrase generation tool
-
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
```

### Comparing `libmonty-0.0.3/README.md` & `libmonty-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 # libmonty - Python libraries
 
 Python libraries
 
-## parts
-
-- [libmonty-easypass](easypass.md)
-    - a passphrase generation tool
-
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
```

### Comparing `libmonty-0.0.3/setup.cfg` & `libmonty-0.1.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = libmonty
 version = attr: libmonty.version.__version__
-url = https://github.com/sunarch/libmonty
+url = https://codeberg.org/sunarch/libmonty
 project_urls = 
-	Bug Tracker = https://github.com/sunarch/libmonty/issues
+	Bug Tracker = https://codeberg.org/sunarch/libmonty/issues
 author = András Németh (sunarch)
 author_email = sunarch@protonmail.com
 maintainer = András Németh (sunarch)
 maintainer_email = sunarch@protonmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -15,15 +15,15 @@
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Topic :: Utilities
 	Topic :: Multimedia :: Sound/Audio :: Players
 	Typing :: Typed
 license = Mozilla Public License 2.0 (MPL 2.0)
-description = libmonty - a collection of Python tools
+description = libmonty - a collection of Python libraries
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = libmonty
 platforms = Any
 
 [options]
 install_requires = file: requirements.txt
@@ -33,24 +33,15 @@
 	= src
 
 [options.entry_points]
 console_scripts = 
 	libmonty = libmonty.__main__:main
 	libmonty-copy-stubs = libmonty.filesystem.copy_stubs:main
 	libmonty-tree-exec = libmonty.filesystem.tree_exec:main
-	libmonty-soundboard = libmonty_soundboard.__main__:main
 
 [options.packages.find]
 where = src
 
-[options.package_data]
-libmonty_easypass = 
-	data/agr-wordlist-en-original.txt
-	data/agr-wordlist-en-alt-edited-by-alan-beale.txt
-	data/eff-large-wordlist.txt
-	data/eff-short-wordlist-1.txt
-	data/eff-short-wordlist-2-0.txt
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `libmonty-0.0.3/src/libmonty/__main__.py` & `libmonty-0.1.0/src/libmonty/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Main
+"""
+
 # imports: library
 from argparse import ArgumentParser
 import sys
 
 # imports: dependencies
 from libmonty_logging.config.file_and_stream.v1 import config as logging_config
 import libmonty_logging.helper as logging_helper
 import libmonty_logging.message as logging_message
 
 # imports: project
 from libmonty import version
 
 
 def main() -> None:
+    """Main"""
 
     logging_helper.apply_config(version.PROGRAM_NAME,
                                 version.__version__,
                                 logging_config)
 
     logging_message.program_header(version.PROGRAM_NAME)
 
@@ -35,9 +39,7 @@
     if args.version:
         print(f'{version.PROGRAM_NAME} {version.__version__}')
         return
 
 
 if __name__ == '__main__':
     main()
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/filesystem/tree_exec.py` & `libmonty-0.1.0/src/libmonty/filesystem/tree_exec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,144 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Tree exec
+"""
+
+# imports: library
+import argparse
 import os.path
 import subprocess
-import argparse
 
-DEBUG_INDENT = True
-DEBUG_PARENT_LAST = True
+
+DEBUG_INDENT: bool = True
+DEBUG_PARENT_LAST: bool = True
 
 
 class IndentItem:
-    BeforeLast = '│   '
-    AfterLast = '    '
-    DirRoot = ''
-    DirMiddle = '├── '
-    DirLast = '└── '
+    """IdentItem"""
+
+    BeforeLast: str = '│   '
+    AfterLast: str = '    '
+    DirRoot: str = ''
+    DirMiddle: str = '├── '
+    DirLast: str = '└── '
 
 
-def quoted(content):
+def quoted(content) -> str:
+    """Quoted"""
+
     return f'"{content}"'
 
 
-def prefixed(content, indents=None, tree=None):
+def prefixed(content: str, indents: list[str] = None, tree: str = None) -> str:
+    """Prefixed"""
+
     if indents is None:
-        indents = []
+        indents: list = []
 
-    prefix_str = ''.join(indents[:-1])
+    prefix: str = ''.join(indents[:-1])
 
     if tree is None:
-        prefix_str += '-> '
+        prefix += '-> '
     else:
-        prefix_str += tree
+        prefix += tree
+
+    return prefix + content
 
-    return prefix_str + content
 
+def recursive_list(dir_name: str,
+                   command: str = None,
+                   indents: list[str] = None,
+                   tree: str = None
+                   ) -> None:
+    """Recursive list"""
 
-def recursive_list(dir_name, command=None, indents=None, tree=None):
     if indents is None:
-        indents = []
+        indents: list = []
 
     if tree == IndentItem.DirRoot:
-        display_name = dir_name
+        display_name: str = dir_name
     else:
-        display_name = os.path.basename(dir_name)
+        display_name: str = os.path.basename(dir_name)
 
     print(prefixed(display_name, indents=indents, tree=tree))
 
     if command is not None:
-        indents_comment = indents + [IndentItem.AfterLast]
-        indents_subcomment = indents_comment + [IndentItem.AfterLast]
+        indents_comment: list[str] = indents + [IndentItem.AfterLast]
+        indents_subcomment: list[str] = indents_comment + [IndentItem.AfterLast]
 
         try:
-            dir_space_escaped = dir_name.replace(' ', '\\' + ' ')
-            command_substituted = command.replace('$', dir_space_escaped)
+            dir_space_escaped: str = dir_name.replace(' ', '\\' + ' ')
+            command_substituted: str = command.replace('$', dir_space_escaped)
             print(prefixed('applying ', indents=indents_comment) + quoted(command_substituted))
             sub_output = subprocess.check_output(command_substituted, shell=True)
         except subprocess.CalledProcessError as err:
             print(prefixed('Error code: ', indents=indents_comment) + quoted(err.returncode))
             print(prefixed('Error message: ', indents=indents_comment) + quoted(err.output))
         else:
             print(prefixed('Return code: ', indents=indents_comment) + quoted('0'))
             print(prefixed('Output: ', indents=indents_comment))
-            output_items = sub_output.split(b'\n')
+            output_items: list = sub_output.split(b'\n')
             if output_items[-1] == '':
-                output_items = output_items[:-1]
+                output_items: list = output_items[:-1]
             for item in output_items:
                 item = str(item, encoding='UTF-8')
                 print(prefixed(quoted(item), indents=indents_subcomment))
 
     try:
-        dir_list = [os.path.join(dir_name, item)
-                    for item in os.listdir(dir_name)]
+        dir_list: list[str] = [
+            os.path.join(dir_name, item)
+            for item in os.listdir(dir_name)
+        ]
     except OSError:
         return
 
-    dir_list_filtered = [os.path.normpath(item)
-                         for item in dir_list
-                         if os.path.isdir(item)]
+    dir_list_filtered: list[str] = [
+        os.path.normpath(item)
+        for item in dir_list
+        if os.path.isdir(item)
+    ]
 
-    indents_before = indents + [IndentItem.BeforeLast]
+    indents_before: list[str] = indents + [IndentItem.BeforeLast]
     for item in dir_list_filtered[:-1]:
         recursive_list(item, command,
                        indents=indents_before, tree=IndentItem.DirMiddle)
 
     if len(dir_list_filtered) > 0:
-        indents_after = indents + [IndentItem.AfterLast]
+        indents_after: list[str] = indents + [IndentItem.AfterLast]
         recursive_list(dir_list_filtered[-1], command,
                        indents=indents_after, tree=IndentItem.DirLast)
 
 
-def arg_type_dir_path(path):
+def arg_type_dir_path(path: str) -> str:
+    """Arg type: dir path"""
+
     if not os.path.isdir(path):
         raise argparse.ArgumentTypeError(f'Given argument "{path}" is not a valid directory path')
 
     return path
 
 
-def main():
+def main() -> None:
+    """Main"""
+
     parser = argparse.ArgumentParser(description='Directory list with applied command.')
 
     parser.add_argument('--root', dest='root', default=os.getcwd(), type=arg_type_dir_path,
                         help='Root directory to recursively execute script from.')
 
     parser.add_argument('--command', dest='command', default=None,
                         help='Shell command to execute on every directory.')
 
     args = parser.parse_args()
-    root = os.path.abspath(str(args.root, encoding='UTF-8'))
+    root: str = os.path.abspath(str(args.root, encoding='UTF-8'))
 
     recursive_list(root, command=args.command, tree=IndentItem.DirRoot)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `libmonty-0.0.3/src/libmonty/formatting/char_str.py` & `libmonty-0.1.0/src/libmonty/formatting/char_str.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Char str
+"""
+
+# imports: library
 import string
 
 
 def pseudo(value: int = ord('.')) -> str:
+    """Pseudo"""
 
     return chr(value)
 
 
 def _byte_to_printable_non_ws_or_space(value: int,
                                        default: str = '.',
                                        space: str = ' ',
                                        ) -> str:
+    """Byte to printable non-WS or space"""
 
-    s_char = chr(value)
+    char: str = chr(value)
 
-    if s_char in ('\r', '\n'):
+    if char in ('\r', '\n'):
         return chr(0x21B5)  # ↵ Downwards Arrow with Corner Leftwards
 
-    if s_char == ' ':
+    if char == ' ':
         return space
 
-    if s_char in string.printable and s_char not in string.whitespace:
-        return s_char
+    if char in string.printable and char not in string.whitespace:
+        return char
 
     return default
 
 
 def byte_to_compact_printable_with_dots(value: int) -> str:
+    """Byte to compact printable with dots"""
 
-    s_default = '.'
-    s_space = chr(0x22C5)  # ⋅ Dot Operator
+    default: str = '.'
+    space: str = chr(0x22C5)  # ⋅ Dot Operator
 
-    return _byte_to_printable_non_ws_or_space(value, s_default, s_space)
+    return _byte_to_printable_non_ws_or_space(value, default, space)
 
 
 def byte_to_compact_printable_with_frames(value: int) -> str:
+    """Byte to compact printable with frames"""
 
-    s_default = chr(0x2395)  # ⎕ Apl Functional Symbol Quad
-    s_space = chr(0x02FD)  # ⋅˽ Modifier Letter Shelf
-
-    return _byte_to_printable_non_ws_or_space(value, s_default, s_space)
+    default: str = chr(0x2395)  # ⎕ Apl Functional Symbol Quad
+    space: str = chr(0x02FD)  # ⋅˽ Modifier Letter Shelf
 
-# -------------------------------------------------------------------- #
+    return _byte_to_printable_non_ws_or_space(value, default, space)
```

### Comparing `libmonty-0.0.3/src/libmonty/formatting/debugging.py` & `libmonty-0.1.0/src/libmonty/formatting/debugging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Debugging
+"""
+
+# imports: project
 from libmonty.outpututils.asciistyling import AsciiColor, AsciiStyle
 
 
-def display_error_message(error):
+def display_error_message(error: Exception) -> None:
+    """Display error message"""
+
     print(AsciiStyle.bold((AsciiColor.red('Error')) + ', ' + error.args[0]))
 
 
-def error_message(message):
+def error_message(message: str) -> None:
+    """Error message"""
+
     print(AsciiStyle.bold(AsciiColor.red('Error')) + ', ' + message)
 
 
-def warning_message(message):
+def warning_message(message: str) -> None:
+    """Warning message"""
+
     print(AsciiStyle.bold(AsciiColor.yellow('Warning')) + ', ' + message)
 
 
-def info_message(message):
+def info_message(message: str) -> None:
+    """Info message"""
+
     print(AsciiStyle.bold(AsciiColor.blue('Info')) + ', ' + message)
```

### Comparing `libmonty-0.0.3/src/libmonty/formatting/json.py` & `libmonty-0.1.0/src/libmonty/formatting/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""JSON
+"""
+
+# imports: library
 from typing import Any, Generator
 
 
-def indent(steps: int = 0, size: int = 2):
+def indent(steps: int = 0, size: int = 2) -> str:
+    """Indent"""
+
     return ' ' * size * steps
 
 
 def formatter(unit: Any, indent_steps: int = 0) -> Generator:
+    """Formatter"""
 
     if isinstance(unit, list):
         for index, item in enumerate(unit):
 
             if not isinstance(item, list) and not isinstance(item, dict):
                 yield f'{indent(indent_steps)}[{index}] \'{item}\''
             else:
@@ -33,9 +40,7 @@
             else:
                 yield start
                 for item in formatter(value, indent_steps + 1):
                     yield item
 
     else:
         yield str(unit)
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/formatting/number_str.py` & `libmonty-0.1.0/src/libmonty/formatting/number_str.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Number str
+"""
+
 
 def pseudo(value: int,
            pad_to: int = 0,
            prefix: str = '',
            ) -> str:
+    """Pseudo"""
 
     return prefix + str(value).zfill(pad_to)
 
 
 def _number_str(name: str,
                 base: str,
                 value: int,
                 pad_to: int = 0,
                 prefix: str = None,
                 ) -> str:
+    """Number str"""
 
     if value < -1:
         raise ValueError(f'Negative value in number formatting: {value}')
 
     if value == -1:
         return name
 
@@ -40,51 +45,55 @@
     return s_output
 
 
 def hexadecimal(value: int,
                 pad_to: int = 0,
                 prefix: str = None,
                 ) -> str:
+    """Hexadecimal"""
 
     return hexadecimal_lower(value, pad_to, prefix)
 
 
 def hexadecimal_lower(value: int,
                       pad_to: int = 0,
                       prefix: str = None,
                       ) -> str:
+    """Hexadecimal - lower"""
 
     return _number_str('h', 'x', value, pad_to, prefix)
 
 
 def hexadecimal_upper(value: int,
                       pad_to: int = 0,
                       prefix: str = None,
                       ) -> str:
+    """Hexadecimal - upper"""
 
     return _number_str('h', 'X', value, pad_to, prefix)
 
 
 def decimal(value: int,
             pad_to: int = 0,
             prefix: str = None
             ) -> str:
+    """Decimal"""
 
     return _number_str('d', 'd', value, pad_to, prefix)
 
 
 def octal(value: int,
           pad_to: int = 0,
           prefix: str = None
           ) -> str:
+    """Octal"""
 
     return _number_str('o', 'o', value, pad_to, prefix)
 
 
 def binary(value: int,
            pad_to: int = 0,
            prefix: str = None
            ) -> str:
+    """Binary"""
 
     return _number_str('b', 'b', value, pad_to, prefix)
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/images/colors_named.py` & `libmonty-0.1.0/src/libmonty/images/colors_named.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-COLORS = {
+"""Colors
+"""
+
+COLORS: dict[str, str] = {
     'F0F8FF': 'AliceBlue',
     'FAEBD7': 'AntiqueWhite',
     '00FFFF': 'Aqua / Cyan',
     '7FFFD4': 'Aquamarine',
     'F0FFFF': 'Azure',
     'F5F5DC': 'Beige',
     'FFE4C4': 'Bisque',
@@ -142,9 +145,7 @@
     'EE82EE': 'Violet',
     'F5DEB3': 'Wheat',
     'FFFFFF': 'White',
     'F5F5F5': 'WhiteSmoke',
     'FFFF00': 'Yellow',
     '9ACD32': 'YellowGreen'
 }
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/images/convert_from_stream.py` & `libmonty-0.1.0/src/libmonty/images/convert_from_stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Convert image from stream
+"""
+
+# imports: requirements
 import PIL.Image
 
 # modes: https://pillow.readthedocs.io/en/stable/handbook/concepts.html#concept-modes
 
 # MODE "RGB" : (3x8-bit pixels, true color)
 
-_DECODER_RAW = 'raw'
+_DECODER_RAW: str = 'raw'
 
 
 def rgb(folder: str,
         filename: str,
         data: bytes,
         size: tuple[int, int],
-        scale: int = None):
+        scale: int = None) -> None:
+    """RGB"""
 
     width, height = size
 
     img = PIL.Image.frombytes('RGB', size, data, decoder_name=_DECODER_RAW)
     img.save(f'{folder}/{filename}.png')
 
     if scale is not None:
 
         scaled_size = (width * 8, height * 8)
 
         img2 = PIL.Image.frombytes('RGB', size, data, decoder_name=_DECODER_RAW)
         img2 = img2.resize(scaled_size, resample=PIL.Image.NEAREST)
         img2.save(f'{folder}/{filename}-scale-{scale}.png')
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/network/responses.py` & `libmonty-0.1.0/src/libmonty/network/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""HTTP responses
+"""
+
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
 # https://en.wikipedia.org/wiki/List_of_HTTP_status_codes
 
+
 def get(code: int) -> dict:
+    """Get response code"""
 
     try:
-        d_details = _responses[code]
-    except KeyError:
-        raise ValueError(f'Response code not found: {code}')
+        details: dict = _responses[code]
+    except KeyError as exc:
+        raise ValueError(f'Response code not found: {code}') from exc
 
-    return d_details
+    return details
 
 
-_responses = {
+_responses: dict[int, dict[str, str]] = {
 
     # ---------------------------------------------------------------- #
     # Informational responses (100–199)
 
     100: {
         'title': 'Continue',
         'description': (
@@ -906,9 +911,7 @@
         'description': (
             'Used by some HTTP proxies to signal a network read timeout '
             'behind the proxy to a client in front of the proxy.'
         ),
         'link': 'https://en.wikipedia.org/wiki/List_of_HTTP_status_codes#598'
     }
 }
-
-# -------------------------------------------------------------------- #
```

### Comparing `libmonty-0.0.3/src/libmonty/sound/formats/wave_pcm.py` & `libmonty-0.1.0/src/libmonty/sound/formats/wave_pcm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Wave PCM audio
+"""
+
+# import: requirements
 from tqdm import tqdm
 
 
 class WavePCMAudio:
+    """Wave PCM audio"""
 
-    DEFAULT_NUM_CHANNELS = 1
-    DEFAULT_SAMPLE_RATE = 44100
-    DEFAULT_BITS_PER_SAMPLE = 16
+    DEFAULT_NUM_CHANNELS: int = 1
+    DEFAULT_SAMPLE_RATE: int = 44100
+    DEFAULT_BITS_PER_SAMPLE: int = 16
 
     # format source: http://soundfile.sapp.org/doc/WaveFormat/
     # The Canonical WAVE PCM Soundfile Format
 
     def __init__(self,
-                 num_channels=DEFAULT_NUM_CHANNELS,
-                 sample_rate=DEFAULT_SAMPLE_RATE,
-                 bits_per_sample=DEFAULT_BITS_PER_SAMPLE):
+                 num_channels: int = DEFAULT_NUM_CHANNELS,
+                 sample_rate: int = DEFAULT_SAMPLE_RATE,
+                 bits_per_sample: int = DEFAULT_BITS_PER_SAMPLE) -> None:
+        """Initialize"""
 
         print('Initializing WavePCMAudioClass object ...', end='')
 
         # init instance variables
         self._num_channels = self.DEFAULT_NUM_CHANNELS
         self._sample_rate = self.DEFAULT_SAMPLE_RATE
         self._bits_per_sample = self.DEFAULT_BITS_PER_SAMPLE
@@ -46,49 +52,61 @@
 
     # Offset: 0, Size: 4, Endian: big
     # Contains the letters 'RIFF' in ASCII form
     # (0x52494646 big-endian form)
 
     @property
     def chunk_id(self) -> str:
+        """Chunk ID"""
+
         return 'RIFF'
 
     @property
     def chunk_id_bytes(self) -> bytes:
+        """Chunk ID bytes"""
+
         return bytes(self.chunk_id, encoding='ASCII')
 
     # ChunkSize ################################################################
 
     # Offset: 4, Size: 4, Endian: little
     # 36 + SubChunk2Size, or more precisely:
     # 4 + (8 + SubChunk1Size) + (8 + SubChunk2Size)
     # This is the size of the rest of the chunk following this number.
     # This is the size of the entire file in bytes minus 8 bytes for the
     # two fields not included in this count: ChunkID and ChunkSize.
 
     @property
     def chunk_size(self) -> int:
+        """Chunk size"""
+
         return 36 + self.subchunk_2_size
 
     @property
     def chunk_size_bytes(self) -> bytes:
+        """Chunk size bytes"""
+
         return self.chunk_size.to_bytes(4, byteorder='little', signed=False)
 
     # Format ###################################################################
 
     # Offset: 8, Size: 4, Endian: big
     # Contains the letters 'WAVE'
     # (0x57415645 big-endian form)
 
     @property
     def format(self) -> str:
+        """Format"""
+
         return 'WAVE'
 
     @property
     def format_bytes(self) -> bytes:
+        """Format bytes"""
+
         return bytes(self.format, encoding='ASCII')
 
     ############################################################################
     # The 'WAVE' format consists of two subchunks: 'fmt ' and 'data': ##########
 
     ############################################################################
     # The 'fmt ' subchunk describes the sound data's format: ###################
@@ -97,173 +115,227 @@
 
     # Offset: 12, Size: 4, Endian: big
     # Contains the letters 'fmt '
     # (0x666d7420 big-endian form)
 
     @property
     def subchunk_1_id(self) -> str:
+        """Subchunk 1 ID"""
+
         return 'fmt '
 
     @property
     def subchunk_1_id_bytes(self) -> bytes:
+        """Subchunk 1 ID bytes"""
+
         return bytes(self.subchunk_1_id, encoding='ASCII')
 
     # Subchunk1Size ############################################################
 
     # Offset: 16, Size: 4, Endian: little
     # 16 for PCM.
     # This is the size of the rest of the Subchunk which follows this number.
 
     @property
     def subchunk_1_size(self) -> int:
+        """Subchunk 1 size"""
+
         return 16
 
     @property
     def subchunk_1_size_bytes(self) -> bytes:
+        """Subchunk 1 size bytes"""
+
         return self.subchunk_1_size.to_bytes(4, byteorder='little', signed=False)
 
     # AudioFormat ##############################################################
 
     # Offset: 20, Size: 2, Endian: little
     # PCM = 1 (i.e. Linear quantization)
     # Values other than 1 indicate some form of compression.
 
     @property
     def audio_format(self) -> int:
+        """Audio format"""
+
         return 1
 
     @property
     def audio_format_bytes(self) -> bytes:
+        """Audio format bytes"""
+
         return self.audio_format.to_bytes(2, byteorder='little', signed=False)
 
     # NumChannels ##############################################################
 
     # Offset: 22, Size: 2, Endian: little
     # Mono = 1, Stereo = 2, etc.
 
     @property
     def num_channels(self) -> int:
+        """Num channels"""
+
         return self._num_channels
 
     @num_channels.setter
     def num_channels(self, new_value: int) -> None:
+        """Set num channels"""
+
         if new_value < 1:
             raise ValueError('Channel count can\'t be lower than 1')
         if new_value > 8:
             raise ValueError('Channel count can\'t be higher than 8')
 
         self._num_channels = new_value
 
     @property
     def num_channels_bytes(self) -> bytes:
+        """Num channels - bytes"""
+
         return self.num_channels.to_bytes(2, byteorder='little', signed=False)
 
     # SampleRate ###############################################################
 
     # Offset: 24, Size: 4, Endian: little
     # 8000, 44100, etc.
 
     @property
     def sample_rate(self) -> int:
+        """Sample rate"""
+
         return self._sample_rate
 
     @sample_rate.setter
     def sample_rate(self, new_value: int) -> None:
+        """Set - sample rate"""
+
         if new_value < 8000:
             raise ValueError('Sample rate can\'t be lower than 8 KHz')
         if new_value > 96000:
             raise ValueError('Sample rate can\'t be higher than 96 KHz')
 
         self._sample_rate = new_value
 
     @property
     def sample_rate_bytes(self) -> bytes:
+        """Sample rate bytes"""
+
         return self.sample_rate.to_bytes(4, byteorder='little', signed=False)
 
     # ByteRate #################################################################
 
     # Offset: 28, Size: 4, Endian: little
     # == SampleRate * NumChannels * BitsPerSample/8
 
     @property
     def byte_rate(self) -> int:
+        """Byte rate"""
+
         return int(self.sample_rate * self.num_channels * self.bits_per_sample / 8)
 
     @property
     def byte_rate_bytes(self) -> bytes:
+        """Byte rate bytes"""
+
         return self.byte_rate.to_bytes(4, byteorder='little', signed=False)
 
     # BlockAlign ###############################################################
 
     # Offset: 32, Size: 2, Endian: little
     # == NumChannels * BitsPerSample/8
     # The number of bytes for one sample including all channels.
     # I wonder what happens when this number isn't an integer?
 
     @property
     def block_align(self) -> int:
+        """Block align"""
+
         return int(self.num_channels * self.bits_per_sample / 8)
 
     @property
     def block_align_bytes(self) -> bytes:
+        """Block align bytes"""
+
         return self.block_align.to_bytes(2, byteorder='little', signed=False)
 
     # BitsPerSample ############################################################
 
     # Offset: 34, Size: 2, Endian: little
     # 8 bits = 8, 16 bits = 16, etc.
 
     @property
     def bits_per_sample(self) -> int:
+        """Bits per sample"""
+
         return self._bits_per_sample
 
     @bits_per_sample.setter
     def bits_per_sample(self, new_value: int) -> None:
+        """Bits per sample"""
+
         if new_value in {8, 16, 24, 32}:
             self._bits_per_sample = new_value
         else:
             raise ValueError('Valid values for Bits per Sample: 8, 16, 24 or 32')
 
     @property
     def bits_per_sample_bytes(self) -> bytes:
+        """Bits per sample bytes"""
+
         return self.bits_per_sample.to_bytes(2, byteorder='little', signed=False)
 
     ######################################
 
     @property
     def is_sample_format_signed(self) -> bool:
+        """Is sample format signed?"""
+
         return False
 
     @property
     def sample_format_signed(self) -> str:
+        """Sample format signed"""
+
         return 'S' if self.is_sample_format_signed else 'U'
 
     @property
     def is_sample_format_big_endian(self) -> bool:
+        """Is sample format big endian"""
+
         return False
 
     @property
     def sample_format_endian(self) -> str:
+        """Sample format endian"""
+
         return 'BE' if self.is_sample_format_big_endian else 'LE'
 
     @property
     def sample_format(self) -> str:
-        sample_format = f'{self.sample_format_signed}{self.bits_per_sample}'
+        """Sample format"""
+
+        sample_format: str = f'{self.sample_format_signed}{self.bits_per_sample}'
+
         if self.bits_per_sample > 8:
             sample_format += f'_{self.sample_format_endian}'
+
         return sample_format
 
     ######################################
 
     @property
     def min_sample_value(self) -> int:
+        """Min sample value"""
+
         return 0
 
     @property
     def max_sample_value(self) -> int:
+        """Max sample value"""
+
         return pow(2, self.bits_per_sample) - 1
 
     ############################################################################
 
     # Offset: ---, Size: 2, Endian: little
     # if PCM, then doesn't exist
     # ExtraParamSize
@@ -279,46 +351,58 @@
 
     # Offset: 36, Size: 4, Endian: big
     # Contains the letters 'data'
     # (0x64617461 big-endian form)
 
     @property
     def subchunk_2_id(self) -> str:
+        """Subchunk 2 ID"""
+
         return 'data'
 
     @property
     def subchunk_2_id_bytes(self) -> bytes:
+        """Subchunk 2 ID bytes"""
+
         return bytes(self.subchunk_2_id, encoding='ASCII')
 
     # Subchunk2Size ############################################################
 
     # Offset: 40, Size: 4, Endian: little
     # == NumSamples * NumChannels * BitsPerSample/8
     # This is the number of bytes in the data.
     # You can also think of this as the size
     # of the read of the subchunk following this number.
 
     @property
     def subchunk_2_size(self) -> int:
+        """Subchunk 2 size"""
+
         return len(self.data)
 
     @property
     def subchunk_2_size_bytes(self) -> bytes:
+        """Subchunk 2 size bytes"""
+
         return self.subchunk_2_size.to_bytes(4, byteorder='little', signed=False)
 
     # Data #####################################################################
 
     # Offset: 44, Size: *, Endian: little
     # The actual sound data.
 
     @property
     def data(self) -> bytearray:
+        """Data"""
+
         return self._data
 
     def add_sample(self, channel_values: list[int], mono_to_all: bool = False) -> None:
+        """Add sample"""
+
         print('Adding sample ', str(channel_values))
 
         if len(channel_values) > self.num_channels:
             raise ValueError('More values in current sample than channels available')
 
         if len(channel_values) < self.num_channels:
             if len(channel_values) == 1 and mono_to_all:
@@ -332,26 +416,29 @@
 
             if item < self.min_sample_value:
                 raise ValueError('A value inside the sample is too low')
 
             if item > self.max_sample_value:
                 raise ValueError('A value inside the sample is too high')
 
-            sample_part_bytes = item.to_bytes(bytes_per_sample, byteorder='little', signed=False)
+            sample_part_bytes: bytes = item.to_bytes(bytes_per_sample, byteorder='little', signed=False)
             self._data.extend(bytearray(sample_part_bytes))
 
     # OTHER ####################################################################
 
     def print_format_info(self) -> None:
+        """Print format info"""
+
         print('Number of channels:  ', str(self.num_channels))
         print('Sample Rate:         ', str(self.sample_rate) + ' Hz')
         print('Bits per Sample:     ', str(self.bits_per_sample))
         print('Sample Format:       ', str(self.sample_format))
 
-    def write_to_file(self, arg_file_name='output.wav'):
+    def write_to_file(self, arg_file_name='output.wav') -> None:
+        """Write to file"""
 
         print('')
         print('WRITING AUDIO DATA TO FILE')
 
         self.print_format_info()
 
         print('File name:           ', arg_file_name)
```

### Comparing `libmonty-0.0.3/src/libmonty.egg-info/PKG-INFO` & `libmonty-0.1.0/src/libmonty.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: libmonty
-Version: 0.0.3
-Summary: libmonty - a collection of Python tools
-Home-page: https://github.com/sunarch/libmonty
+Version: 0.1.0
+Summary: libmonty - a collection of Python libraries
+Home-page: https://codeberg.org/sunarch/libmonty
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
-Project-URL: Bug Tracker, https://github.com/sunarch/libmonty/issues
+Project-URL: Bug Tracker, https://codeberg.org/sunarch/libmonty/issues
 Keywords: libmonty
 Platform: Any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,19 +24,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty - Python libraries
 
 Python libraries
 
-## parts
-
-- [libmonty-easypass](easypass.md)
-    - a passphrase generation tool
-
 ## Installation
 
 The package is on PyPI: [libmonty](https://pypi.org/project/libmonty/)
 
 ```
 pip install libmonty
 ```
```

### Comparing `libmonty-0.0.3/src/libmonty.egg-info/SOURCES.txt` & `libmonty-0.1.0/src/libmonty.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/libmonty.egg-info/PKG-INFO
 src/libmonty.egg-info/SOURCES.txt
 src/libmonty.egg-info/dependency_links.txt
 src/libmonty.egg-info/entry_points.txt
 src/libmonty.egg-info/requires.txt
 src/libmonty.egg-info/top_level.txt
 src/libmonty/environment/__init__.py
+src/libmonty/environment/arguments.py
 src/libmonty/environment/terminal.py
 src/libmonty/fileformats/__init__.py
 src/libmonty/fileformats/oab_process.py
 src/libmonty/filesystem/__init__.py
 src/libmonty/filesystem/copy_stubs.py
 src/libmonty/filesystem/directory.py
 src/libmonty/filesystem/tree_exec.py
@@ -26,28 +27,16 @@
 src/libmonty/formatting/debugging.py
 src/libmonty/formatting/json.py
 src/libmonty/formatting/number_str.py
 src/libmonty/images/__init__.py
 src/libmonty/images/colors_named.py
 src/libmonty/images/convert_from_stream.py
 src/libmonty/network/__init__.py
+src/libmonty/network/email_check.py
 src/libmonty/network/responses.py
 src/libmonty/outpututils/__init__.py
 src/libmonty/outpututils/asciistyling.py
 src/libmonty/outpututils/decorators.py
 src/libmonty/outpututils/discord.py
 src/libmonty/sound/__init__.py
 src/libmonty/sound/formats/__init__.py
-src/libmonty/sound/formats/wave_pcm.py
-src/libmonty_easypass/__init__.py
-src/libmonty_easypass/dice_methods.py
-src/libmonty_easypass/easypass.py
-src/libmonty_easypass/data/agr-wordlist-en-alt-edited-by-alan-beale.txt
-src/libmonty_easypass/data/agr-wordlist-en-original.txt
-src/libmonty_easypass/data/eff-large-wordlist.txt
-src/libmonty_easypass/data/eff-short-wordlist-1.txt
-src/libmonty_easypass/data/eff-short-wordlist-2-0.txt
-src/libmonty_soundboard/__init__.py
-src/libmonty_soundboard/__main__.py
-src/libmonty_soundboard/config.py
-src/libmonty_soundboard/sound.py
-src/libmonty_soundboard/version.py
+src/libmonty/sound/formats/wave_pcm.py
```

