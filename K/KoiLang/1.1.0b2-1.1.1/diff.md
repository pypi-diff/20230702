# Comparing `tmp/KoiLang-1.1.0b2.tar.gz` & `tmp/KoiLang-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KoiLang-1.1.0b2.tar", last modified: Wed Apr  5 12:08:00 2023, max compression
+gzip compressed data, was "KoiLang-1.1.1.tar", last modified: Sun Jul  2 17:29:31 2023, max compression
```

## Comparing `KoiLang-1.1.0b2.tar` & `KoiLang-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.652753 KoiLang-1.1.0b2/KoiLang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.660754 KoiLang-1.1.0b2/kola/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_cutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_cutil.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_yylex.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.660754 KoiLang-1.1.0b2/kola/klvm/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/commandset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/commandset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/koilang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)   676158 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.c
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/kola/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/kola/lib/debugger/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/command_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/default_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/fast_file.py
--rw-r--r--   0 runner    (1001) docker     (123)   577659 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/unicode_handler.c
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/version.py
--rw-r--r--   0 runner    (1001) docker     (123)  1137811 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.557168 KoiLang-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.479516 KoiLang-1.1.1/KoiLang.egg-info/
+-rw-rw-rw-   0        0        0    12456 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1463 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-08-17 13:41:36.000000 KoiLang-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    12456 2023-07-02 17:29:31.556178 KoiLang-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11401 2023-06-01 10:51:09.000000 KoiLang-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.511522 KoiLang-1.1.1/kola/
+-rw-rw-rw-   0        0        0     1067 2023-05-18 14:12:37.000000 KoiLang-1.1.1/kola/__init__.py
+-rw-rw-rw-   0        0        0     3172 2023-04-05 04:13:29.000000 KoiLang-1.1.1/kola/__main__.py
+-rw-rw-rw-   0        0        0     7002 2023-04-07 10:48:13.000000 KoiLang-1.1.1/kola/_cutil.h
+-rw-rw-rw-   0        0        0     3221 2023-04-06 11:35:14.000000 KoiLang-1.1.1/kola/_cutil.pxd
+-rw-rw-rw-   0        0        0     1559 2023-03-28 16:42:40.000000 KoiLang-1.1.1/kola/_yylex.pxd
+-rw-rw-rw-   0        0        0      375 2023-01-15 16:44:08.000000 KoiLang-1.1.1/kola/exception.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.528167 KoiLang-1.1.1/kola/klvm/
+-rw-rw-rw-   0        0        0      561 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/klvm/__init__.py
+-rw-rw-rw-   0        0        0     3057 2023-07-02 16:39:22.000000 KoiLang-1.1.1/kola/klvm/command.py
+-rw-rw-rw-   0        0        0     5124 2023-07-02 16:53:02.000000 KoiLang-1.1.1/kola/klvm/commandset.py
+-rw-rw-rw-   0        0        0     2419 2023-05-15 13:04:03.000000 KoiLang-1.1.1/kola/klvm/commandset.pyi
+-rw-rw-rw-   0        0        0     2305 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/klvm/decorator.py
+-rw-rw-rw-   0        0        0     2837 2023-04-20 10:43:55.000000 KoiLang-1.1.1/kola/klvm/decorator.pyi
+-rw-rw-rw-   0        0        0     8316 2023-07-02 15:45:52.000000 KoiLang-1.1.1/kola/klvm/environment.py
+-rw-rw-rw-   0        0        0     5894 2023-07-02 15:06:42.000000 KoiLang-1.1.1/kola/klvm/handler.py
+-rw-rw-rw-   0        0        0    11575 2023-05-16 10:25:45.000000 KoiLang-1.1.1/kola/klvm/koilang.py
+-rw-rw-rw-   0        0        0     2428 2023-07-02 14:57:58.000000 KoiLang-1.1.1/kola/klvm/mask.py
+-rw-rw-rw-   0        0        0     3337 2023-05-15 09:19:47.000000 KoiLang-1.1.1/kola/klvm/writer.py
+-rw-rw-rw-   0        0        0   680498 2023-04-06 12:20:02.000000 KoiLang-1.1.1/kola/lexer.c
+-rw-rw-rw-   0        0        0     1087 2023-04-06 11:32:42.000000 KoiLang-1.1.1/kola/lexer.pxd
+-rw-rw-rw-   0        0        0     3049 2023-04-06 12:02:51.000000 KoiLang-1.1.1/kola/lexer.pyi
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.534168 KoiLang-1.1.1/kola/lib/
+-rw-rw-rw-   0        0        0     3697 2023-04-21 10:29:04.000000 KoiLang-1.1.1/kola/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.540167 KoiLang-1.1.1/kola/lib/debugger/
+-rw-rw-rw-   0        0        0      327 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/lib/debugger/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-05-16 11:17:29.000000 KoiLang-1.1.1/kola/lib/debugger/base.py
+-rw-rw-rw-   0        0        0      465 2023-04-13 10:44:00.000000 KoiLang-1.1.1/kola/lib/debugger/command_debugger.py
+-rw-rw-rw-   0        0        0     6372 2023-05-16 11:39:57.000000 KoiLang-1.1.1/kola/lib/debugger/default_runner.py
+-rw-rw-rw-   0        0        0    11900 2023-04-23 08:21:48.000000 KoiLang-1.1.1/kola/lib/disabled.jklvm.py
+-rw-rw-rw-   0        0        0     3349 2023-07-02 16:37:30.000000 KoiLang-1.1.1/kola/lib/fastfiles.py
+-rw-rw-rw-   0        0        0     1253 2023-05-05 14:41:55.000000 KoiLang-1.1.1/kola/lib/recorder.py
+-rw-rw-rw-   0        0        0   577664 2023-04-06 11:40:03.000000 KoiLang-1.1.1/kola/parser.c
+-rw-rw-rw-   0        0        0      586 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/parser.pxd
+-rw-rw-rw-   0        0        0      845 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/parser.pyi
+-rw-rw-rw-   0        0        0     3769 2023-03-28 17:09:26.000000 KoiLang-1.1.1/kola/unicode_handler.c
+-rw-rw-rw-   0        0        0       46 2023-07-02 17:29:16.000000 KoiLang-1.1.1/kola/version.py
+-rw-rw-rw-   0        0        0  1137811 2023-04-06 11:40:04.000000 KoiLang-1.1.1/kola/writer.c
+-rw-rw-rw-   0        0        0     2374 2023-02-24 14:55:22.000000 KoiLang-1.1.1/kola/writer.pxd
+-rw-rw-rw-   0        0        0     2185 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/writer.pyi
+-rw-rw-rw-   0        0        0       42 2023-07-02 17:29:31.557168 KoiLang-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3131 2023-07-02 14:56:00.000000 KoiLang-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.554169 KoiLang-1.1.1/tests/
+-rw-rw-rw-   0        0        0     5834 2023-05-15 17:49:36.000000 KoiLang-1.1.1/tests/test_kola.py
+-rw-rw-rw-   0        0        0     3685 2023-04-12 07:40:39.000000 KoiLang-1.1.1/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     2709 2023-04-20 12:41:53.000000 KoiLang-1.1.1/tests/test_parser.py
+-rw-rw-rw-   0        0        0     3668 2023-04-20 09:10:18.000000 KoiLang-1.1.1/tests/test_writer.py
```

### Comparing `KoiLang-1.1.0b2/KoiLang.egg-info/PKG-INFO` & `KoiLang-1.1.1/KoiLang.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,340 +1,342 @@
-Metadata-Version: 2.1
-Name: KoiLang
-Version: 1.1.0b2
-Summary: simple python module for KoiLang parsing
-Home-page: https://github.com/Ovizro/Kola
-Author: Ovizro
-Author-email: Ovizro@hypercol.com
-Maintainer: Ovizro
-Maintainer-email: Ovizro@hypercol.com
-License: Apache 2.0
-Description: # Kola
-        Simple python module for KoiLang parsing.
-        
-        [![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-        [![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-        ![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-        
-        ## Installation
-        From pip:
-        
-            pip install KoiLang
-        
-        From source code:
-            
-            python setup.py build_ext --inplace
-            python setup.py install
-        
-        ## What is KoiLang
-        
-        KoiLang is a markup language while is easy to read for people.
-        There is an simple example.
-        ```
-        #background Street
-            #camera on(Orga)
-            #character Orga
-                Huh... I'm a pretty good shot, huh?
-            #camera on(Ride, Ched)
-            #character Ride
-                B- boss...
-            #character Orga
-                #action bleed
-            #camera on(object: blood, source: Orga)
-        
-            #camera on(Ched, Orga, Ride)
-            #character Orga
-                How come you're stammering like that... Ride!
-        
-            #playsound freesia
-        
-            #character Orga
-                #action stand_up speed(slowly)
-        
-            #character Ride
-                But... but!
-            #character Orga
-                I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-            #character Ride
-                #action shed_tear
-                No... not for me...
-        
-            #camera on(Orga)
-            #character Orga
-                Protecting my members is my job!
-            #character Ched
-                #action shed_tear
-        
-            #character Ride
-                But...!
-            #character Orga
-                Shut up and let's go!
-        
-                #camera on(Orga)
-                #action walk direction(front) speed(slowly)
-                Everyone's waiting, besides...
-        
-                I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-                As long as we don't stop, the road will continue!
-        ```
-        
-        ### Grammar
-        
-        In KoiLang, the code contains 'command' section and 'text' section.
-        The format of the command section is similar to a C prepared statement,
-        using '#' as the prefix. And other lines that do not start with '#' are the text section.
-        
-            #command "This is a command"
-            This is the text.
-        
-        The format of a single command like:
-        
-            #command_name [param 1] [param 2] ...
-        
-        There are several parameters behind the command whose name should be a valid variable name.
-        
-        > An unsigned decimal integer like is also a legal command name, like `#114`.
-        
-        Each command can have several parameters behind the command name.
-        Valid argument type include integer, float, literal and string.
-            
-            #arg_int    1 0b101 0x6CF
-            #arg_float  1. 2e-2 .114514
-            #arg_literal string __name__
-            #arg_string "A string"
-        
-        > Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
-         
-        The above parameter types are often referred to base parameters.
-        Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-        The format is as follows:
-        
-            #kwargs key(value)
-            
-            And another format:
-            #keyargs_list key(item0, item1)
-            
-            And the third:
-            #kwargs_dict key(x: 11, y: 45, z: 14)
-        
-        All the parameters above can be put together:
-            
-            #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-                thickness(2) color(255, 255, 255)
-        
-        ## What can Kola module do
-        
-        Kola module provides a fast way to translate KoiLang command into a python function call.
-        
-        Above command `#draw` will convert to function call below:
-        
-        ```py
-        draw(
-            "Line", 2,
-            pos0={"x": 0, "y": 0},
-            pos1={"x": 16, "y": 16},
-            thickness=2,
-            color=[255, 255, 255]
-        )
-        ```
-        
-        Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-        
-        ### Example
-        
-        Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-        
-        Let us start with a kola file:
-        
-        ```
-        ## This is the file `makefiles.kola`
-        
-        #file "hello.txt" encoding("utf-8")
-        Hello world!
-        And there are all my friends.
-        
-        #space hello
-        
-            #file "Bob.txt"
-            Hello Bob.
-        
-            #file "Alice.txt"
-            Hello Alice.
-        
-        #endspace
-        ```
-        
-        Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-        
-        ```py
-        import os
-        from kola import KoiLang, kola_command, kola_text
-        
-        
-        class FastFile(KoiLang):
-            @kola_command
-            def file(self, path: str, encoding: str = "utf-8") -> None:
-                if self._file:
-                    self._file.close()
-                path_dir = os.path.dirname(path)
-                if path_dir:
-                    os.makedirs(path_dir, exist_ok=True)
-                self._file = open(path, "w", encoding=encoding)
-            
-            @kola_command
-            def space(self, name: str) -> None:
-                path = name.replace('.', '/')
-                if not os.path.isdir(path):
-                    os.makedirs(path)
-                os.chdir(path)
-            
-            @kola_command
-            def endspace(self) -> None:
-                os.chdir("..")
-                self.end()
-        
-            @kola_command
-            def end(self) -> None:
-                if self._file:
-                    self._file.close()
-                    self._file = None
-            
-            @kola_text
-            def text(self, text: str) -> None:
-                if not self._file:
-                    raise OSError("write texts before the file open")
-                self._file.write(text)
-            
-            def at_start(self) -> None:
-                self._file = None
-            
-            def at_end(self) -> None:
-                self.end()
-        ```
-        
-        You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-        
-        ```sh
-        python -m kola makefiles.kola -s script.py
-        ```
-        
-        Or add these directly at the end of the script:
-        ```py
-        if __name__ = "__main__":
-            FastFile().parse_file("makefiles.kola")
-        ```
-        
-        You will see new files in your work dir.
-        
-            <workdir>
-            │      
-            │  hello.txt
-            │      
-            └─hello
-                Alice.txt
-                Bob.txt
-        
-        ### What happened
-        
-        It seems amusing? Well, if you make a python script as this:
-        
-        ```py
-        vmobj = FastFile()
-        
-        with vmobj.exec_block():
-            vmobj.file("hello.txt", encoding="utf-8")
-            vmobj.text("Hello world!")
-            vmobj.text("And there are all my friends.")
-        
-            vmobj.space("hello")
-        
-            vmobj.file("Bob.txt")
-            vmobj.text("Hello Bob.")
-        
-            vmobj.file("Alice.txt")
-            vmobj.text("Hello Alice.")
-        
-            vmobj.endspace()
-        ```
-        the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-        
-        So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-        ```py
-        class FastFile(KoiLang):
-            ...
-        ```
-        The next step is making the kola command we need. So a function is defined here:
-        ```py
-        def file(self, path: str, encoding: str = "utf-8") -> None:
-            if self._file:
-                self._file.close()
-            path_dir = os.path.dirname(path)
-            if path_dir:
-                os.makedirs(path_dir, exist_ok=True)
-            self._file = open(path, "w", encoding=encoding)
-        ```
-        But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-        ```py
-        @kola_command("open")
-        def file(self, path: str, encoding: str = "utf-8") -> None:
-            if self._file:
-                self._file.close()
-            path_dir = os.path.dirname(path)
-            if path_dir:
-                os.makedirs(path_dir, exist_ok=True)
-            self._file = open(path, "w", encoding=encoding)
-        ```
-        Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-        
-        You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-        
-        ### File parse
-        `KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-        
-        ### Advanced techniques
-        In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-        
-        ```py
-        class FastFile(KoiLang):
-            ...
-        
-            class space(Environment):
-                @kola_env_enter("space")
-                def enter(self, name: str) -> None:
-                    self.pwd = os.getcwd()
-                    path = name.replace('.', '/')
-                    if not os.path.isdir(path):
-                        os.makedirs(path)
-                    os.chdir(path)
-                
-                @kola_env_exit("endspace")
-                def exit(self) -> None:
-                    os.chdir(self.pwd)
-        ```
-        
-        > There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-        
-        ## What is more
-        
-        The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-        
-        On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-        
-        ## Bugs/Requests
-        
-        Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: KoiLang
+Version: 1.1.1
+Summary: simple python module for KoiLang parsing
+Home-page: https://github.com/Ovizro/Kola
+Author: Visecy
+Author-email: Visecy@visecy.top
+Maintainer: Ovizro
+Maintainer-email: Ovizro@visecy.top
+License: Apache 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Kola
+Simple python module for KoiLang parsing.
+
+[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+
+## Installation
+From pip:
+
+    pip install KoiLang
+
+From source code:
+    
+    python setup.py build_ext --inplace
+    python setup.py install
+
+## What is KoiLang
+
+KoiLang is a markup language while is easy to read for people.
+There is an simple example.
+```
+#background Street
+    #camera on(Orga)
+    #character Orga
+        Huh... I'm a pretty good shot, huh?
+    #camera on(Ride, Ched)
+    #character Ride
+        B- boss...
+    #character Orga
+        #action bleed
+    #camera on(object: blood, source: Orga)
+
+    #camera on(Ched, Orga, Ride)
+    #character Orga
+        How come you're stammering like that... Ride!
+
+    #playsound freesia
+
+    #character Orga
+        #action stand_up speed(slowly)
+
+    #character Ride
+        But... but!
+    #character Orga
+        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+    #character Ride
+        #action shed_tear
+        No... not for me...
+
+    #camera on(Orga)
+    #character Orga
+        Protecting my members is my job!
+    #character Ched
+        #action shed_tear
+
+    #character Ride
+        But...!
+    #character Orga
+        Shut up and let's go!
+
+        #camera on(Orga)
+        #action walk direction(front) speed(slowly)
+        Everyone's waiting, besides...
+
+        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+        As long as we don't stop, the road will continue!
+```
+
+### Grammar
+
+In KoiLang, the code contains 'command' section and 'text' section.
+The format of the command section is similar to a C prepared statement,
+using '#' as the prefix. And other lines that do not start with '#' are the text section.
+
+    #command "This is a command"
+    This is the text.
+
+The format of a single command like:
+
+    #command_name [param 1] [param 2] ...
+
+There are several parameters behind the command whose name should be a valid variable name.
+
+> An unsigned decimal integer like is also a legal command name, like `#114`.
+
+Each command can have several parameters behind the command name.
+Valid argument type include integer, float, literal and string.
+    
+    #arg_int    1 0b101 0x6CF
+    #arg_float  1. 2e-2 .114514
+    #arg_literal string __name__
+    #arg_string "A string"
+
+> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+ 
+The above parameter types are often referred to base parameters.
+Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+The format is as follows:
+
+    #kwargs key(value)
+    
+    And another format:
+    #keyargs_list key(item0, item1)
+    
+    And the third:
+    #kwargs_dict key(x: 11, y: 45, z: 14)
+
+All the parameters above can be put together:
+    
+    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+        thickness(2) color(255, 255, 255)
+
+## What can Kola module do
+
+Kola module provides a fast way to translate KoiLang command into a python function call.
+
+Above command `#draw` will convert to function call below:
+
+```py
+draw(
+    "Line", 2,
+    pos0={"x": 0, "y": 0},
+    pos1={"x": 16, "y": 16},
+    thickness=2,
+    color=[255, 255, 255]
+)
+```
+
+Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+
+### Example
+
+Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+
+Let us start with a kola file:
+
+```
+## This is the file `makefiles.kola`
+
+#file "hello.txt" encoding("utf-8")
+Hello world!
+And there are all my friends.
+
+#space hello
+
+    #file "Bob.txt"
+    Hello Bob.
+
+    #file "Alice.txt"
+    Hello Alice.
+
+#endspace
+```
+
+Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+
+```py
+import os
+from kola import KoiLang, kola_command, kola_text
+
+
+class FastFile(KoiLang):
+    @kola_command
+    def file(self, path: str, encoding: str = "utf-8") -> None:
+        if self._file:
+            self._file.close()
+        path_dir = os.path.dirname(path)
+        if path_dir:
+            os.makedirs(path_dir, exist_ok=True)
+        self._file = open(path, "w", encoding=encoding)
+    
+    @kola_command
+    def space(self, name: str) -> None:
+        path = name.replace('.', '/')
+        if not os.path.isdir(path):
+            os.makedirs(path)
+        os.chdir(path)
+    
+    @kola_command
+    def endspace(self) -> None:
+        os.chdir("..")
+        self.end()
+
+    @kola_command
+    def end(self) -> None:
+        if self._file:
+            self._file.close()
+            self._file = None
+    
+    @kola_text
+    def text(self, text: str) -> None:
+        if not self._file:
+            raise OSError("write texts before the file open")
+        self._file.write(text)
+    
+    def at_start(self) -> None:
+        self._file = None
+    
+    def at_end(self) -> None:
+        self.end()
+```
+
+You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+
+```sh
+python -m kola makefiles.kola -s script.py
+```
+
+Or add these directly at the end of the script:
+```py
+if __name__ = "__main__":
+    FastFile().parse_file("makefiles.kola")
+```
+
+You will see new files in your work dir.
+
+    <workdir>
+    │      
+    │  hello.txt
+    │      
+    └─hello
+        Alice.txt
+        Bob.txt
+
+### What happened
+
+It seems amusing? Well, if you make a python script as this:
+
+```py
+vmobj = FastFile()
+
+with vmobj.exec_block():
+    vmobj.file("hello.txt", encoding="utf-8")
+    vmobj.text("Hello world!")
+    vmobj.text("And there are all my friends.")
+
+    vmobj.space("hello")
+
+    vmobj.file("Bob.txt")
+    vmobj.text("Hello Bob.")
+
+    vmobj.file("Alice.txt")
+    vmobj.text("Hello Alice.")
+
+    vmobj.endspace()
+```
+the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+
+So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+```py
+class FastFile(KoiLang):
+    ...
+```
+The next step is making the kola command we need. So a function is defined here:
+```py
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+```py
+@kola_command("open")
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+
+You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+
+### File parse
+`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+
+### Advanced techniques
+In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+
+```py
+class FastFile(KoiLang):
+    ...
+
+    class space(Environment):
+        @kola_env_enter("space")
+        def enter(self, name: str) -> None:
+            self.pwd = os.getcwd()
+            path = name.replace('.', '/')
+            if not os.path.isdir(path):
+                os.makedirs(path)
+            os.chdir(path)
+        
+        @kola_env_exit("endspace")
+        def exit(self) -> None:
+            os.chdir(self.pwd)
+```
+
+> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+
+## What is more
+
+The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+
+On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+
+## Bugs/Requests
+
+Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
```

### Comparing `KoiLang-1.1.0b2/KoiLang.egg-info/SOURCES.txt` & `KoiLang-1.1.1/KoiLang.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -26,15 +26,42 @@
 kola/klvm/__init__.py
 kola/klvm/command.py
 kola/klvm/commandset.py
 kola/klvm/commandset.pyi
 kola/klvm/decorator.py
 kola/klvm/decorator.pyi
 kola/klvm/environment.py
+kola/klvm/handler.py
 kola/klvm/koilang.py
+kola/klvm/mask.py
 kola/klvm/writer.py
 kola/lib/__init__.py
-kola/lib/fast_file.py
+kola/lib/disabled.jklvm.py
+kola/lib/fastfiles.py
+kola/lib/recorder.py
 kola/lib/debugger/__init__.py
 kola/lib/debugger/base.py
 kola/lib/debugger/command_debugger.py
-kola/lib/debugger/default_runner.py
+kola/lib/debugger/default_runner.py
+kola/klvm/__init__.py
+kola/klvm/command.py
+kola/klvm/commandset.py
+kola/klvm/commandset.pyi
+kola/klvm/decorator.py
+kola/klvm/decorator.pyi
+kola/klvm/environment.py
+kola/klvm/handler.py
+kola/klvm/koilang.py
+kola/klvm/mask.py
+kola/klvm/writer.py
+kola/lib/__init__.py
+kola/lib/disabled.jklvm.py
+kola/lib/fastfiles.py
+kola/lib/recorder.py
+kola/lib/debugger/__init__.py
+kola/lib/debugger/base.py
+kola/lib/debugger/command_debugger.py
+kola/lib/debugger/default_runner.py
+tests/test_kola.py
+tests/test_lexer.py
+tests/test_parser.py
+tests/test_writer.py
```

### Comparing `KoiLang-1.1.0b2/LICENSE` & `KoiLang-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `KoiLang-1.1.0b2/PKG-INFO` & `KoiLang-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,340 +1,342 @@
-Metadata-Version: 2.1
-Name: KoiLang
-Version: 1.1.0b2
-Summary: simple python module for KoiLang parsing
-Home-page: https://github.com/Ovizro/Kola
-Author: Ovizro
-Author-email: Ovizro@hypercol.com
-Maintainer: Ovizro
-Maintainer-email: Ovizro@hypercol.com
-License: Apache 2.0
-Description: # Kola
-        Simple python module for KoiLang parsing.
-        
-        [![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-        [![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-        ![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-        
-        ## Installation
-        From pip:
-        
-            pip install KoiLang
-        
-        From source code:
-            
-            python setup.py build_ext --inplace
-            python setup.py install
-        
-        ## What is KoiLang
-        
-        KoiLang is a markup language while is easy to read for people.
-        There is an simple example.
-        ```
-        #background Street
-            #camera on(Orga)
-            #character Orga
-                Huh... I'm a pretty good shot, huh?
-            #camera on(Ride, Ched)
-            #character Ride
-                B- boss...
-            #character Orga
-                #action bleed
-            #camera on(object: blood, source: Orga)
-        
-            #camera on(Ched, Orga, Ride)
-            #character Orga
-                How come you're stammering like that... Ride!
-        
-            #playsound freesia
-        
-            #character Orga
-                #action stand_up speed(slowly)
-        
-            #character Ride
-                But... but!
-            #character Orga
-                I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-            #character Ride
-                #action shed_tear
-                No... not for me...
-        
-            #camera on(Orga)
-            #character Orga
-                Protecting my members is my job!
-            #character Ched
-                #action shed_tear
-        
-            #character Ride
-                But...!
-            #character Orga
-                Shut up and let's go!
-        
-                #camera on(Orga)
-                #action walk direction(front) speed(slowly)
-                Everyone's waiting, besides...
-        
-                I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-                As long as we don't stop, the road will continue!
-        ```
-        
-        ### Grammar
-        
-        In KoiLang, the code contains 'command' section and 'text' section.
-        The format of the command section is similar to a C prepared statement,
-        using '#' as the prefix. And other lines that do not start with '#' are the text section.
-        
-            #command "This is a command"
-            This is the text.
-        
-        The format of a single command like:
-        
-            #command_name [param 1] [param 2] ...
-        
-        There are several parameters behind the command whose name should be a valid variable name.
-        
-        > An unsigned decimal integer like is also a legal command name, like `#114`.
-        
-        Each command can have several parameters behind the command name.
-        Valid argument type include integer, float, literal and string.
-            
-            #arg_int    1 0b101 0x6CF
-            #arg_float  1. 2e-2 .114514
-            #arg_literal string __name__
-            #arg_string "A string"
-        
-        > Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
-         
-        The above parameter types are often referred to base parameters.
-        Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-        The format is as follows:
-        
-            #kwargs key(value)
-            
-            And another format:
-            #keyargs_list key(item0, item1)
-            
-            And the third:
-            #kwargs_dict key(x: 11, y: 45, z: 14)
-        
-        All the parameters above can be put together:
-            
-            #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-                thickness(2) color(255, 255, 255)
-        
-        ## What can Kola module do
-        
-        Kola module provides a fast way to translate KoiLang command into a python function call.
-        
-        Above command `#draw` will convert to function call below:
-        
-        ```py
-        draw(
-            "Line", 2,
-            pos0={"x": 0, "y": 0},
-            pos1={"x": 16, "y": 16},
-            thickness=2,
-            color=[255, 255, 255]
-        )
-        ```
-        
-        Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-        
-        ### Example
-        
-        Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-        
-        Let us start with a kola file:
-        
-        ```
-        ## This is the file `makefiles.kola`
-        
-        #file "hello.txt" encoding("utf-8")
-        Hello world!
-        And there are all my friends.
-        
-        #space hello
-        
-            #file "Bob.txt"
-            Hello Bob.
-        
-            #file "Alice.txt"
-            Hello Alice.
-        
-        #endspace
-        ```
-        
-        Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-        
-        ```py
-        import os
-        from kola import KoiLang, kola_command, kola_text
-        
-        
-        class FastFile(KoiLang):
-            @kola_command
-            def file(self, path: str, encoding: str = "utf-8") -> None:
-                if self._file:
-                    self._file.close()
-                path_dir = os.path.dirname(path)
-                if path_dir:
-                    os.makedirs(path_dir, exist_ok=True)
-                self._file = open(path, "w", encoding=encoding)
-            
-            @kola_command
-            def space(self, name: str) -> None:
-                path = name.replace('.', '/')
-                if not os.path.isdir(path):
-                    os.makedirs(path)
-                os.chdir(path)
-            
-            @kola_command
-            def endspace(self) -> None:
-                os.chdir("..")
-                self.end()
-        
-            @kola_command
-            def end(self) -> None:
-                if self._file:
-                    self._file.close()
-                    self._file = None
-            
-            @kola_text
-            def text(self, text: str) -> None:
-                if not self._file:
-                    raise OSError("write texts before the file open")
-                self._file.write(text)
-            
-            def at_start(self) -> None:
-                self._file = None
-            
-            def at_end(self) -> None:
-                self.end()
-        ```
-        
-        You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-        
-        ```sh
-        python -m kola makefiles.kola -s script.py
-        ```
-        
-        Or add these directly at the end of the script:
-        ```py
-        if __name__ = "__main__":
-            FastFile().parse_file("makefiles.kola")
-        ```
-        
-        You will see new files in your work dir.
-        
-            <workdir>
-            │      
-            │  hello.txt
-            │      
-            └─hello
-                Alice.txt
-                Bob.txt
-        
-        ### What happened
-        
-        It seems amusing? Well, if you make a python script as this:
-        
-        ```py
-        vmobj = FastFile()
-        
-        with vmobj.exec_block():
-            vmobj.file("hello.txt", encoding="utf-8")
-            vmobj.text("Hello world!")
-            vmobj.text("And there are all my friends.")
-        
-            vmobj.space("hello")
-        
-            vmobj.file("Bob.txt")
-            vmobj.text("Hello Bob.")
-        
-            vmobj.file("Alice.txt")
-            vmobj.text("Hello Alice.")
-        
-            vmobj.endspace()
-        ```
-        the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-        
-        So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-        ```py
-        class FastFile(KoiLang):
-            ...
-        ```
-        The next step is making the kola command we need. So a function is defined here:
-        ```py
-        def file(self, path: str, encoding: str = "utf-8") -> None:
-            if self._file:
-                self._file.close()
-            path_dir = os.path.dirname(path)
-            if path_dir:
-                os.makedirs(path_dir, exist_ok=True)
-            self._file = open(path, "w", encoding=encoding)
-        ```
-        But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-        ```py
-        @kola_command("open")
-        def file(self, path: str, encoding: str = "utf-8") -> None:
-            if self._file:
-                self._file.close()
-            path_dir = os.path.dirname(path)
-            if path_dir:
-                os.makedirs(path_dir, exist_ok=True)
-            self._file = open(path, "w", encoding=encoding)
-        ```
-        Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-        
-        You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-        
-        ### File parse
-        `KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-        
-        ### Advanced techniques
-        In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-        
-        ```py
-        class FastFile(KoiLang):
-            ...
-        
-            class space(Environment):
-                @kola_env_enter("space")
-                def enter(self, name: str) -> None:
-                    self.pwd = os.getcwd()
-                    path = name.replace('.', '/')
-                    if not os.path.isdir(path):
-                        os.makedirs(path)
-                    os.chdir(path)
-                
-                @kola_env_exit("endspace")
-                def exit(self) -> None:
-                    os.chdir(self.pwd)
-        ```
-        
-        > There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-        
-        ## What is more
-        
-        The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-        
-        On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-        
-        ## Bugs/Requests
-        
-        Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: KoiLang
+Version: 1.1.1
+Summary: simple python module for KoiLang parsing
+Home-page: https://github.com/Ovizro/Kola
+Author: Visecy
+Author-email: Visecy@visecy.top
+Maintainer: Ovizro
+Maintainer-email: Ovizro@visecy.top
+License: Apache 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Kola
+Simple python module for KoiLang parsing.
+
+[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+
+## Installation
+From pip:
+
+    pip install KoiLang
+
+From source code:
+    
+    python setup.py build_ext --inplace
+    python setup.py install
+
+## What is KoiLang
+
+KoiLang is a markup language while is easy to read for people.
+There is an simple example.
+```
+#background Street
+    #camera on(Orga)
+    #character Orga
+        Huh... I'm a pretty good shot, huh?
+    #camera on(Ride, Ched)
+    #character Ride
+        B- boss...
+    #character Orga
+        #action bleed
+    #camera on(object: blood, source: Orga)
+
+    #camera on(Ched, Orga, Ride)
+    #character Orga
+        How come you're stammering like that... Ride!
+
+    #playsound freesia
+
+    #character Orga
+        #action stand_up speed(slowly)
+
+    #character Ride
+        But... but!
+    #character Orga
+        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+    #character Ride
+        #action shed_tear
+        No... not for me...
+
+    #camera on(Orga)
+    #character Orga
+        Protecting my members is my job!
+    #character Ched
+        #action shed_tear
+
+    #character Ride
+        But...!
+    #character Orga
+        Shut up and let's go!
+
+        #camera on(Orga)
+        #action walk direction(front) speed(slowly)
+        Everyone's waiting, besides...
+
+        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+        As long as we don't stop, the road will continue!
+```
+
+### Grammar
+
+In KoiLang, the code contains 'command' section and 'text' section.
+The format of the command section is similar to a C prepared statement,
+using '#' as the prefix. And other lines that do not start with '#' are the text section.
+
+    #command "This is a command"
+    This is the text.
+
+The format of a single command like:
+
+    #command_name [param 1] [param 2] ...
+
+There are several parameters behind the command whose name should be a valid variable name.
+
+> An unsigned decimal integer like is also a legal command name, like `#114`.
+
+Each command can have several parameters behind the command name.
+Valid argument type include integer, float, literal and string.
+    
+    #arg_int    1 0b101 0x6CF
+    #arg_float  1. 2e-2 .114514
+    #arg_literal string __name__
+    #arg_string "A string"
+
+> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+ 
+The above parameter types are often referred to base parameters.
+Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+The format is as follows:
+
+    #kwargs key(value)
+    
+    And another format:
+    #keyargs_list key(item0, item1)
+    
+    And the third:
+    #kwargs_dict key(x: 11, y: 45, z: 14)
+
+All the parameters above can be put together:
+    
+    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+        thickness(2) color(255, 255, 255)
+
+## What can Kola module do
+
+Kola module provides a fast way to translate KoiLang command into a python function call.
+
+Above command `#draw` will convert to function call below:
+
+```py
+draw(
+    "Line", 2,
+    pos0={"x": 0, "y": 0},
+    pos1={"x": 16, "y": 16},
+    thickness=2,
+    color=[255, 255, 255]
+)
+```
+
+Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+
+### Example
+
+Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+
+Let us start with a kola file:
+
+```
+## This is the file `makefiles.kola`
+
+#file "hello.txt" encoding("utf-8")
+Hello world!
+And there are all my friends.
+
+#space hello
+
+    #file "Bob.txt"
+    Hello Bob.
+
+    #file "Alice.txt"
+    Hello Alice.
+
+#endspace
+```
+
+Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+
+```py
+import os
+from kola import KoiLang, kola_command, kola_text
+
+
+class FastFile(KoiLang):
+    @kola_command
+    def file(self, path: str, encoding: str = "utf-8") -> None:
+        if self._file:
+            self._file.close()
+        path_dir = os.path.dirname(path)
+        if path_dir:
+            os.makedirs(path_dir, exist_ok=True)
+        self._file = open(path, "w", encoding=encoding)
+    
+    @kola_command
+    def space(self, name: str) -> None:
+        path = name.replace('.', '/')
+        if not os.path.isdir(path):
+            os.makedirs(path)
+        os.chdir(path)
+    
+    @kola_command
+    def endspace(self) -> None:
+        os.chdir("..")
+        self.end()
+
+    @kola_command
+    def end(self) -> None:
+        if self._file:
+            self._file.close()
+            self._file = None
+    
+    @kola_text
+    def text(self, text: str) -> None:
+        if not self._file:
+            raise OSError("write texts before the file open")
+        self._file.write(text)
+    
+    def at_start(self) -> None:
+        self._file = None
+    
+    def at_end(self) -> None:
+        self.end()
+```
+
+You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+
+```sh
+python -m kola makefiles.kola -s script.py
+```
+
+Or add these directly at the end of the script:
+```py
+if __name__ = "__main__":
+    FastFile().parse_file("makefiles.kola")
+```
+
+You will see new files in your work dir.
+
+    <workdir>
+    │      
+    │  hello.txt
+    │      
+    └─hello
+        Alice.txt
+        Bob.txt
+
+### What happened
+
+It seems amusing? Well, if you make a python script as this:
+
+```py
+vmobj = FastFile()
+
+with vmobj.exec_block():
+    vmobj.file("hello.txt", encoding="utf-8")
+    vmobj.text("Hello world!")
+    vmobj.text("And there are all my friends.")
+
+    vmobj.space("hello")
+
+    vmobj.file("Bob.txt")
+    vmobj.text("Hello Bob.")
+
+    vmobj.file("Alice.txt")
+    vmobj.text("Hello Alice.")
+
+    vmobj.endspace()
+```
+the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+
+So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+```py
+class FastFile(KoiLang):
+    ...
+```
+The next step is making the kola command we need. So a function is defined here:
+```py
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+```py
+@kola_command("open")
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+
+You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+
+### File parse
+`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+
+### Advanced techniques
+In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+
+```py
+class FastFile(KoiLang):
+    ...
+
+    class space(Environment):
+        @kola_env_enter("space")
+        def enter(self, name: str) -> None:
+            self.pwd = os.getcwd()
+            path = name.replace('.', '/')
+            if not os.path.isdir(path):
+                os.makedirs(path)
+            os.chdir(path)
+        
+        @kola_env_exit("endspace")
+        def exit(self) -> None:
+            os.chdir(self.pwd)
+```
+
+> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+
+## What is more
+
+The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+
+On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+
+## Bugs/Requests
+
+Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
```

### Comparing `KoiLang-1.1.0b2/README.md` & `KoiLang-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,314 +1,315 @@
-# Kola
-Simple python module for KoiLang parsing.
-
-[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-
-## Installation
-From pip:
-
-    pip install KoiLang
-
-From source code:
-    
-    python setup.py build_ext --inplace
-    python setup.py install
-
-## What is KoiLang
-
-KoiLang is a markup language while is easy to read for people.
-There is an simple example.
-```
-#background Street
-    #camera on(Orga)
-    #character Orga
-        Huh... I'm a pretty good shot, huh?
-    #camera on(Ride, Ched)
-    #character Ride
-        B- boss...
-    #character Orga
-        #action bleed
-    #camera on(object: blood, source: Orga)
-
-    #camera on(Ched, Orga, Ride)
-    #character Orga
-        How come you're stammering like that... Ride!
-
-    #playsound freesia
-
-    #character Orga
-        #action stand_up speed(slowly)
-
-    #character Ride
-        But... but!
-    #character Orga
-        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-    #character Ride
-        #action shed_tear
-        No... not for me...
-
-    #camera on(Orga)
-    #character Orga
-        Protecting my members is my job!
-    #character Ched
-        #action shed_tear
-
-    #character Ride
-        But...!
-    #character Orga
-        Shut up and let's go!
-
-        #camera on(Orga)
-        #action walk direction(front) speed(slowly)
-        Everyone's waiting, besides...
-
-        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-        As long as we don't stop, the road will continue!
-```
-
-### Grammar
-
-In KoiLang, the code contains 'command' section and 'text' section.
-The format of the command section is similar to a C prepared statement,
-using '#' as the prefix. And other lines that do not start with '#' are the text section.
-
-    #command "This is a command"
-    This is the text.
-
-The format of a single command like:
-
-    #command_name [param 1] [param 2] ...
-
-There are several parameters behind the command whose name should be a valid variable name.
-
-> An unsigned decimal integer like is also a legal command name, like `#114`.
-
-Each command can have several parameters behind the command name.
-Valid argument type include integer, float, literal and string.
-    
-    #arg_int    1 0b101 0x6CF
-    #arg_float  1. 2e-2 .114514
-    #arg_literal string __name__
-    #arg_string "A string"
-
-> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
- 
-The above parameter types are often referred to base parameters.
-Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-The format is as follows:
-
-    #kwargs key(value)
-    
-    And another format:
-    #keyargs_list key(item0, item1)
-    
-    And the third:
-    #kwargs_dict key(x: 11, y: 45, z: 14)
-
-All the parameters above can be put together:
-    
-    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-        thickness(2) color(255, 255, 255)
-
-## What can Kola module do
-
-Kola module provides a fast way to translate KoiLang command into a python function call.
-
-Above command `#draw` will convert to function call below:
-
-```py
-draw(
-    "Line", 2,
-    pos0={"x": 0, "y": 0},
-    pos1={"x": 16, "y": 16},
-    thickness=2,
-    color=[255, 255, 255]
-)
-```
-
-Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-
-### Example
-
-Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-
-Let us start with a kola file:
-
-```
-## This is the file `makefiles.kola`
-
-#file "hello.txt" encoding("utf-8")
-Hello world!
-And there are all my friends.
-
-#space hello
-
-    #file "Bob.txt"
-    Hello Bob.
-
-    #file "Alice.txt"
-    Hello Alice.
-
-#endspace
-```
-
-Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-
-```py
-import os
-from kola import KoiLang, kola_command, kola_text
-
-
-class FastFile(KoiLang):
-    @kola_command
-    def file(self, path: str, encoding: str = "utf-8") -> None:
-        if self._file:
-            self._file.close()
-        path_dir = os.path.dirname(path)
-        if path_dir:
-            os.makedirs(path_dir, exist_ok=True)
-        self._file = open(path, "w", encoding=encoding)
-    
-    @kola_command
-    def space(self, name: str) -> None:
-        path = name.replace('.', '/')
-        if not os.path.isdir(path):
-            os.makedirs(path)
-        os.chdir(path)
-    
-    @kola_command
-    def endspace(self) -> None:
-        os.chdir("..")
-        self.end()
-
-    @kola_command
-    def end(self) -> None:
-        if self._file:
-            self._file.close()
-            self._file = None
-    
-    @kola_text
-    def text(self, text: str) -> None:
-        if not self._file:
-            raise OSError("write texts before the file open")
-        self._file.write(text)
-    
-    def at_start(self) -> None:
-        self._file = None
-    
-    def at_end(self) -> None:
-        self.end()
-```
-
-You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-
-```sh
-python -m kola makefiles.kola -s script.py
-```
-
-Or add these directly at the end of the script:
-```py
-if __name__ = "__main__":
-    FastFile().parse_file("makefiles.kola")
-```
-
-You will see new files in your work dir.
-
-    <workdir>
-    │      
-    │  hello.txt
-    │      
-    └─hello
-        Alice.txt
-        Bob.txt
-
-### What happened
-
-It seems amusing? Well, if you make a python script as this:
-
-```py
-vmobj = FastFile()
-
-with vmobj.exec_block():
-    vmobj.file("hello.txt", encoding="utf-8")
-    vmobj.text("Hello world!")
-    vmobj.text("And there are all my friends.")
-
-    vmobj.space("hello")
-
-    vmobj.file("Bob.txt")
-    vmobj.text("Hello Bob.")
-
-    vmobj.file("Alice.txt")
-    vmobj.text("Hello Alice.")
-
-    vmobj.endspace()
-```
-the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-
-So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-```py
-class FastFile(KoiLang):
-    ...
-```
-The next step is making the kola command we need. So a function is defined here:
-```py
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-```py
-@kola_command("open")
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-
-You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-
-### File parse
-`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-
-### Advanced techniques
-In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-
-```py
-class FastFile(KoiLang):
-    ...
-
-    class space(Environment):
-        @kola_env_enter("space")
-        def enter(self, name: str) -> None:
-            self.pwd = os.getcwd()
-            path = name.replace('.', '/')
-            if not os.path.isdir(path):
-                os.makedirs(path)
-            os.chdir(path)
-        
-        @kola_env_exit("endspace")
-        def exit(self) -> None:
-            os.chdir(self.pwd)
-```
-
-> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-
-## What is more
-
-The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-
-On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-
-## Bugs/Requests
-
+# Kola
+Simple python module for KoiLang parsing.
+
+[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+
+## Installation
+From pip:
+
+    pip install KoiLang
+
+From source code:
+    
+    python setup.py build_ext --inplace
+    python setup.py install
+
+## What is KoiLang
+
+KoiLang is a markup language while is easy to read for people.
+There is an simple example.
+```
+#background Street
+    #camera on(Orga)
+    #character Orga
+        Huh... I'm a pretty good shot, huh?
+    #camera on(Ride, Ched)
+    #character Ride
+        B- boss...
+    #character Orga
+        #action bleed
+    #camera on(object: blood, source: Orga)
+
+    #camera on(Ched, Orga, Ride)
+    #character Orga
+        How come you're stammering like that... Ride!
+
+    #playsound freesia
+
+    #character Orga
+        #action stand_up speed(slowly)
+
+    #character Ride
+        But... but!
+    #character Orga
+        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+    #character Ride
+        #action shed_tear
+        No... not for me...
+
+    #camera on(Orga)
+    #character Orga
+        Protecting my members is my job!
+    #character Ched
+        #action shed_tear
+
+    #character Ride
+        But...!
+    #character Orga
+        Shut up and let's go!
+
+        #camera on(Orga)
+        #action walk direction(front) speed(slowly)
+        Everyone's waiting, besides...
+
+        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+        As long as we don't stop, the road will continue!
+```
+
+### Grammar
+
+In KoiLang, the code contains 'command' section and 'text' section.
+The format of the command section is similar to a C prepared statement,
+using '#' as the prefix. And other lines that do not start with '#' are the text section.
+
+    #command "This is a command"
+    This is the text.
+
+The format of a single command like:
+
+    #command_name [param 1] [param 2] ...
+
+There are several parameters behind the command whose name should be a valid variable name.
+
+> An unsigned decimal integer like is also a legal command name, like `#114`.
+
+Each command can have several parameters behind the command name.
+Valid argument type include integer, float, literal and string.
+    
+    #arg_int    1 0b101 0x6CF
+    #arg_float  1. 2e-2 .114514
+    #arg_literal string __name__
+    #arg_string "A string"
+
+> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+ 
+The above parameter types are often referred to base parameters.
+Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+The format is as follows:
+
+    #kwargs key(value)
+    
+    And another format:
+    #keyargs_list key(item0, item1)
+    
+    And the third:
+    #kwargs_dict key(x: 11, y: 45, z: 14)
+
+All the parameters above can be put together:
+    
+    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+        thickness(2) color(255, 255, 255)
+
+## What can Kola module do
+
+Kola module provides a fast way to translate KoiLang command into a python function call.
+
+Above command `#draw` will convert to function call below:
+
+```py
+draw(
+    "Line", 2,
+    pos0={"x": 0, "y": 0},
+    pos1={"x": 16, "y": 16},
+    thickness=2,
+    color=[255, 255, 255]
+)
+```
+
+Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+
+### Example
+
+Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+
+Let us start with a kola file:
+
+```
+## This is the file `makefiles.kola`
+
+#file "hello.txt" encoding("utf-8")
+Hello world!
+And there are all my friends.
+
+#space hello
+
+    #file "Bob.txt"
+    Hello Bob.
+
+    #file "Alice.txt"
+    Hello Alice.
+
+#endspace
+```
+
+Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+
+```py
+import os
+from kola import KoiLang, kola_command, kola_text
+
+
+class FastFile(KoiLang):
+    @kola_command
+    def file(self, path: str, encoding: str = "utf-8") -> None:
+        if self._file:
+            self._file.close()
+        path_dir = os.path.dirname(path)
+        if path_dir:
+            os.makedirs(path_dir, exist_ok=True)
+        self._file = open(path, "w", encoding=encoding)
+    
+    @kola_command
+    def space(self, name: str) -> None:
+        path = name.replace('.', '/')
+        if not os.path.isdir(path):
+            os.makedirs(path)
+        os.chdir(path)
+    
+    @kola_command
+    def endspace(self) -> None:
+        os.chdir("..")
+        self.end()
+
+    @kola_command
+    def end(self) -> None:
+        if self._file:
+            self._file.close()
+            self._file = None
+    
+    @kola_text
+    def text(self, text: str) -> None:
+        if not self._file:
+            raise OSError("write texts before the file open")
+        self._file.write(text)
+    
+    def at_start(self) -> None:
+        self._file = None
+    
+    def at_end(self) -> None:
+        self.end()
+```
+
+You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+
+```sh
+python -m kola makefiles.kola -s script.py
+```
+
+Or add these directly at the end of the script:
+```py
+if __name__ = "__main__":
+    FastFile().parse_file("makefiles.kola")
+```
+
+You will see new files in your work dir.
+
+    <workdir>
+    │      
+    │  hello.txt
+    │      
+    └─hello
+        Alice.txt
+        Bob.txt
+
+### What happened
+
+It seems amusing? Well, if you make a python script as this:
+
+```py
+vmobj = FastFile()
+
+with vmobj.exec_block():
+    vmobj.file("hello.txt", encoding="utf-8")
+    vmobj.text("Hello world!")
+    vmobj.text("And there are all my friends.")
+
+    vmobj.space("hello")
+
+    vmobj.file("Bob.txt")
+    vmobj.text("Hello Bob.")
+
+    vmobj.file("Alice.txt")
+    vmobj.text("Hello Alice.")
+
+    vmobj.endspace()
+```
+the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+
+So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+```py
+class FastFile(KoiLang):
+    ...
+```
+The next step is making the kola command we need. So a function is defined here:
+```py
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+```py
+@kola_command("open")
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+
+You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+
+### File parse
+`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+
+### Advanced techniques
+In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+
+```py
+class FastFile(KoiLang):
+    ...
+
+    class space(Environment):
+        @kola_env_enter("space")
+        def enter(self, name: str) -> None:
+            self.pwd = os.getcwd()
+            path = name.replace('.', '/')
+            if not os.path.isdir(path):
+                os.makedirs(path)
+            os.chdir(path)
+        
+        @kola_env_exit("endspace")
+        def exit(self) -> None:
+            os.chdir(self.pwd)
+```
+
+> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+
+## What is more
+
+The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+
+On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+
+## Bugs/Requests
+
 Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
```

### Comparing `KoiLang-1.1.0b2/kola/__init__.py` & `KoiLang-1.1.1/kola/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-from .lexer import BaseLexer, FileLexer, StringLexer
-from .parser import Parser
-from .writer import BaseWriter, FileWriter, StringWriter, BaseWriterItem, FormatItem, ComplexArg, WriterItemLike
-from .klvm import KoiLang, Environment, kola_command, kola_text, kola_number, kola_annotation, kola_env_enter, kola_env_exit, kola_env_class
-from .version import __version__, version_info
-from .exception import KoiLangError, KoiLangSyntaxError, KoiLangCommandError
-
-
-__author__ = "Ovizro"
-__author_email__ = "Ovizro@hypercol.com"
-
-__all__ = [
-    "KoiLang",
-    "Environment",
-    "kola_command",
-    "kola_text",
-    "kola_number",
-    "kola_annotation",
-    "kola_env_enter",
-    "kola_env_exit",
-    
-    "BaseLexer",
-    "FileLexer",
-    "StringLexer",
-    "Parser",
-    "BaseWriter",
-    "FileWriter",
-    "StringWriter",
-    "BaseWriterItem",
-    "FormatItem",
-    "ComplexArg",
-    "WriterItemLike",
-
-    "KoiLangError",
-    "KoiLangSyntaxError",
-    "KoiLangCommandError"
-]
+"""
+simple python module for KoiLang parsing
+"""
+
+from .lexer import BaseLexer, FileLexer, StringLexer
+from .parser import Parser
+from .writer import BaseWriter, FileWriter, StringWriter, BaseWriterItem, FormatItem, ComplexArg, WriterItemLike
+from .klvm import KoiLang, Environment, kola_command, kola_text, kola_number, kola_annotation, kola_env_enter, kola_env_exit, kola_env_class
+from .version import __version__, __version_num__
+from .exception import KoiLangError, KoiLangSyntaxError, KoiLangCommandError
+
+
+__author__ = "Ovizro"
+__author_email__ = "Ovizro@visecy.top"
+
+__all__ = [
+    "KoiLang",
+    "Environment",
+    "kola_command",
+    "kola_text",
+    "kola_number",
+    "kola_annotation",
+    "kola_env_enter",
+    "kola_env_exit",
+    
+    "BaseLexer",
+    "FileLexer",
+    "StringLexer",
+    "Parser",
+    "BaseWriter",
+    "FileWriter",
+    "StringWriter",
+    "BaseWriterItem",
+    "FormatItem",
+    "ComplexArg",
+    "WriterItemLike",
+
+    "KoiLangError",
+    "KoiLangSyntaxError",
+    "KoiLangCommandError"
+]
```

### Comparing `KoiLang-1.1.0b2/kola/_cutil.h` & `KoiLang-1.1.1/kola/_cutil.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,252 +1,255 @@
-#ifndef _INCLUDE_HELPER_
-#define _INCLUDE_HELPER_ 
-
-#include <stdint.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <Python.h>
-
-#ifdef MS_WINDOWS
-#include <Windows.h>
-#endif
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/* An opaque pointer. */
-#ifndef YY_TYPEDEF_YY_SCANNER_T
-#define YY_TYPEDEF_YY_SCANNER_T
-typedef void* yyscan_t;
-#endif
-
-#define LFLAG_DISABLED      (1 << 0)
-#define LFLAG_ISANNOTATION  (1 << 1)
-#define LFLAG_NOLSTRIP        (1 << 2)
-
-typedef struct lexer_extra {
-    const char* filename;
-    uint8_t command_threshold;
-    uint8_t flag;
-} LexerData;
-
-#define YY_EXTRA_TYPE LexerData*
-
-enum TokenSyn {
-    CMD=1, CMD_N, TEXT, LITERAL, STRING, NUM, NUM_H,
-    NUM_B, NUM_F, CLN, CMA, SLP, SRP, ANNOTATION
-};
-
-static const uint8_t yy_goto[7][8] = {
-    {15,    63,     0,      0,      0,      0,      0,  0},     // CMD | CMD_N | TEXT
-    {34,    162,    35,     117,    0,      151,    0,  40},    // LITERAL   
-    {17,    49,     35,     117,    0,      151,    0,  40},    // NUM | STRING
-    {0,     0,      134,    0,      0,      0,      0,  6},     // CLN
-    {0,     0,      100,    0,      4,      0,      8,  0},     // CMA
-    {0,     3,      0,      0,      0,      0,      0,  0},     // SLP
-    {0,     0,      65,     0,      81,     0,      81, 0}     // SRP
-};
-
-#ifdef Py_PYTHON_H
-
-#define get_type_qualname(obj) (Py_TYPE(obj)->tp_name)
-
-static __inline const char* get_type_name(PyObject* obj) {
-    const char* qualname = get_type_qualname(obj);
-    const char* name = strrchr(qualname, '.');
-    if (name == NULL) {
-        name = qualname;
-    } else {
-        name += 1;
-    }
-    return name;
-}
-
-#define ERR_CASE(syn, act) case (act << 4) + syn
-#define ERR_MSG(msg) return "[%d] " # msg
-
-static const char* get_format(int code) {
-    switch (code)
-    {
-    case 1:
-        ERR_MSG(unknown symbol '%s');
-    case 2:
-        ERR_MSG(command '%s' not found);
-    case 3:
-        ERR_MSG(an error occured during handling command '%s');
-    case 4:
-        ERR_MSG(an error occured during handling text '%s');
-    case 5:
-        ERR_MSG(cannot decode string '%s');
-    case 10:
-        ERR_MSG(end of line in incurrect place);
-    case 16:
-        ERR_MSG(unclosed parentheses);
-    case 28:
-        ERR_MSG(keyword must be a literal);
-    case 201:
-    case 202:
-    case 210:
-        ERR_MSG(bad argument count);
-    }
-    
-    switch (code & 0x0F)
-    {
-    case CMD:
-    case CMD_N:
-    case TEXT:
-    case ANNOTATION:
-        ERR_MSG(end of line in incurrect place);
-    }
-    ERR_MSG(unknown syntax);
-}
-
-#include "frameobject.h"
-// For Cython limiting, error setting function has to define here 
-static void __inline kola_set_error(PyObject* exc_type, int errorno,
-                            const char* filename, int lineno, const char* text) 
-{
-    PyErr_Format(exc_type, get_format(errorno), errorno, text);
-
-    // add traceback in .kola file
-    #if PY_VERSION_HEX >= 0x03080000
-        _PyTraceback_Add("<kola>", filename, lineno);
-    #else
-        PyCodeObject* code = NULL;
-        PyFrameObject* frame = NULL;
-        PyObject* globals = NULL;
-        PyObject *exc, *val, *tb;
-
-        PyErr_Fetch(&exc, &val, &tb);
-
-        globals = PyDict_New();
-        if (!globals) goto end;
-        code = PyCode_NewEmpty(filename, "<kola>", lineno);
-        if (!code) goto end;
-        frame = PyFrame_New(
-            PyThreadState_Get(),
-            code,
-            globals,
-            NULL
-        );
-        if (!frame) goto end;
-
-        frame->f_lineno = lineno;
-        PyErr_Restore(exc, val, tb);
-        PyTraceBack_Here(frame);
-
-    end:
-        Py_XDECREF(code);
-        Py_XDECREF(frame);
-        Py_XDECREF(globals);
-    #endif
-}
-
-static void __inline kola_set_errcause(PyObject* exc_type, int errorno,
-                            const char* filename, int lineno, const char* text, PyObject* cause) 
-{
-    PyErr_Format(exc_type, get_format(errorno), errorno, text);
-    
-    PyObject *exc, *val, *tb;
-    PyErr_Fetch(&exc, &val, &tb);
-    if (cause == Py_None) {
-        PyException_SetContext(val, NULL);
-    } else {
-        Py_INCREF(cause);
-        PyException_SetCause(val, cause);
-    }
-    #if PY_VERSION_HEX >= 0x03080000
-        PyErr_Restore(exc, val, tb);
-        _PyTraceback_Add("<kola>", filename, lineno);
-    #else
-        PyCodeObject* code = NULL;
-        PyFrameObject* frame = NULL;
-        PyObject* globals = NULL;
-        globals = PyDict_New();
-        if (!globals) goto end;
-        code = PyCode_NewEmpty(filename, "<kola>", lineno);
-        if (!code) goto end;
-        frame = PyFrame_New(
-            PyThreadState_Get(),
-            code,
-            globals,
-            NULL
-        );
-        if (!frame) goto end;
-
-        frame->f_lineno = lineno;
-        PyErr_Restore(exc, val, tb);
-        PyTraceBack_Here(frame);
-
-    end:
-        Py_XDECREF(code);
-        Py_XDECREF(frame);
-        Py_XDECREF(globals);
-    #endif
-}
-
-static __inline FILE* kola_open(PyObject* raw_path, PyObject** out, const char* mode) {
-    PyObject* stringobj = NULL;
-    FILE* fp;
-#ifdef MS_WINDOWS
-    wchar_t wmode[5];
-    DWORD dwNum = MultiByteToWideChar(CP_ACP, 0, mode, -1, NULL, 0); 
-    if (dwNum > 4) {
-        PyErr_Format(PyExc_ValueError, "invalid mode: %.200s", mode);
-        return NULL;
-    }
-    MultiByteToWideChar(CP_ACP, 0, mode, -1, wmode, dwNum);
-    Py_UNICODE *widename = NULL;
-    if (!PyUnicode_FSDecoder(raw_path, &stringobj)) {
-        return NULL;
-    }
-    widename = PyUnicode_AsWideCharString(stringobj, NULL);
-    if (widename == NULL) {
-        return NULL;
-    }
-
-    Py_BEGIN_ALLOW_THREADS
-    fp = _wfopen(widename, wmode);
-    Py_END_ALLOW_THREADS
-#else
-    const char *name = NULL;
-    if (!PyUnicode_FSConverter(raw_path, &stringobj)) {
-        return NULL;
-    }
-    name = PyBytes_AS_STRING(stringobj);
-
-    Py_BEGIN_ALLOW_THREADS
-    fp = fopen(name, mode);
-    Py_END_ALLOW_THREADS
-#endif
-    if (fp == NULL) {
-        PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
-    }
-    if (out)
-        *out = stringobj;
-    return fp;
-}
-
-static __inline const char* unicode2string(PyObject* __s, Py_ssize_t* s_len) {
-    Py_ssize_t _s_len;
-    const char* s = PyUnicode_AsUTF8AndSize(__s, &_s_len);
-    if (s == NULL)
-        return NULL;
-    else if (strlen(s) != (size_t)_s_len) {
-        PyErr_SetString(PyExc_ValueError, "embedded null character");
-        return NULL;
-    }
-    if (s_len)
-        *s_len = _s_len;
-    return s;
-}
-
-// from cpython:string_parser.decode_unicode_with_escapes
-PyObject* decode_escapes(const char* s, Py_ssize_t len);
-PyObject* filter_text(PyObject* string);
-#endif
-
-#ifdef __cplusplus
-}
-#endif
+#ifndef _INCLUDE_HELPER_
+#define _INCLUDE_HELPER_ 
+
+#include <stdint.h>
+#include <stdio.h>
+#include <stdlib.h>
+#include <Python.h>
+
+#ifdef MS_WINDOWS
+#include <Windows.h>
+#endif
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/* An opaque pointer. */
+#ifndef YY_TYPEDEF_YY_SCANNER_T
+#define YY_TYPEDEF_YY_SCANNER_T
+typedef void* yyscan_t;
+#endif
+
+#define LFLAG_DISABLED      (1 << 0)
+#define LFLAG_ISANNOTATION  (1 << 1)
+#define LFLAG_NOLSTRIP        (1 << 2)
+
+typedef struct lexer_extra {
+    const char* filename;
+    uint8_t command_threshold;
+    uint8_t flag;
+} LexerData;
+
+#define YY_EXTRA_TYPE LexerData*
+
+enum TokenSyn {
+    CMD=1, CMD_N, TEXT, LITERAL, STRING, NUM, NUM_H,
+    NUM_B, NUM_F, CLN, CMA, SLP, SRP, ANNOTATION
+};
+
+static const uint8_t yy_goto[7][8] = {
+    {15,    63,     0,      0,      0,      0,      0,  0},     // CMD | CMD_N | TEXT
+    {34,    162,    35,     117,    0,      151,    0,  40},    // LITERAL   
+    {17,    49,     35,     117,    0,      151,    0,  40},    // NUM | STRING
+    {0,     0,      134,    0,      0,      0,      0,  6},     // CLN
+    {0,     0,      100,    0,      4,      0,      8,  0},     // CMA
+    {0,     3,      0,      0,      0,      0,      0,  0},     // SLP
+    {0,     0,      65,     0,      81,     0,      81, 0}     // SRP
+};
+
+#ifdef Py_PYTHON_H
+
+#define get_type_qualname(obj) (Py_TYPE(obj)->tp_name)
+
+static __inline const char* get_type_name(PyObject* obj) {
+    const char* qualname = get_type_qualname(obj);
+    const char* name = strrchr(qualname, '.');
+    if (name == NULL) {
+        name = qualname;
+    } else {
+        name += 1;
+    }
+    return name;
+}
+
+#define ERR_CASE(syn, act) case (act << 4) + syn
+#define ERR_MSG(msg) return "[%d] " # msg
+
+static const char* get_format(int code) {
+    switch (code)
+    {
+    case 1:
+        ERR_MSG(unknown symbol '%s');
+    case 2:
+        ERR_MSG(command '%s' not found);
+    case 3:
+        ERR_MSG(an error occured during handling command '%s');
+    case 4:
+        ERR_MSG(an error occured during handling text '%s');
+    case 5:
+        ERR_MSG(cannot decode string '%s');
+    case 10:
+        ERR_MSG(end of line in incurrect place);
+    case 16:
+        ERR_MSG(unclosed parentheses);
+    case 28:
+        ERR_MSG(keyword must be a literal);
+    case 201:
+    case 202:
+    case 210:
+        ERR_MSG(bad argument count);
+    }
+    
+    switch (code & 0x0F)
+    {
+    case CMD:
+    case CMD_N:
+    case TEXT:
+    case ANNOTATION:
+        ERR_MSG(end of line in incurrect place);
+    }
+    ERR_MSG(unknown syntax);
+}
+
+#include "frameobject.h"
+// For Cython limiting, error setting function has to define here 
+static void __inline kola_set_error(PyObject* exc_type, int errorno,
+                            const char* filename, int lineno, const char* text) 
+{
+    PyErr_Format(exc_type, get_format(errorno), errorno, text);
+
+    // add traceback in .kola file
+    #if PY_VERSION_HEX >= 0x03080000
+        _PyTraceback_Add("<kola>", filename, lineno);
+    #else
+        PyCodeObject* code = NULL;
+        PyFrameObject* frame = NULL;
+        PyObject* globals = NULL;
+        PyObject *exc, *val, *tb;
+
+        PyErr_Fetch(&exc, &val, &tb);
+
+        globals = PyDict_New();
+        if (!globals) goto end;
+        code = PyCode_NewEmpty(filename, "<kola>", lineno);
+        if (!code) goto end;
+        frame = PyFrame_New(
+            PyThreadState_Get(),
+            code,
+            globals,
+            NULL
+        );
+        if (!frame) goto end;
+
+        frame->f_lineno = lineno;
+        PyErr_Restore(exc, val, tb);
+        PyTraceBack_Here(frame);
+
+    end:
+        Py_XDECREF(code);
+        Py_XDECREF(frame);
+        Py_XDECREF(globals);
+    #endif
+}
+
+static void __inline kola_set_errcause(PyObject* exc_type, int errorno,
+                            const char* filename, int lineno, const char* text, PyObject* cause) 
+{
+    PyErr_Format(exc_type, get_format(errorno), errorno, text);
+    
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    if (cause == Py_None) {
+        PyException_SetContext(val, NULL);
+    } else {
+        Py_INCREF(cause);
+        PyException_SetCause(val, cause);
+    }
+    #if PY_VERSION_HEX >= 0x03080000
+        PyErr_Restore(exc, val, tb);
+        _PyTraceback_Add("<kola>", filename, lineno);
+    #else
+        PyCodeObject* code = NULL;
+        PyFrameObject* frame = NULL;
+        PyObject* globals = NULL;
+        globals = PyDict_New();
+        if (!globals) goto end;
+        code = PyCode_NewEmpty(filename, "<kola>", lineno);
+        if (!code) goto end;
+        frame = PyFrame_New(
+            PyThreadState_Get(),
+            code,
+            globals,
+            NULL
+        );
+        if (!frame) goto end;
+
+        frame->f_lineno = lineno;
+        PyErr_Restore(exc, val, tb);
+        PyTraceBack_Here(frame);
+
+    end:
+        Py_XDECREF(code);
+        Py_XDECREF(frame);
+        Py_XDECREF(globals);
+    #endif
+}
+
+static __inline FILE* kola_open(PyObject* raw_path, PyObject** out, const char* mode) {
+    PyObject* stringobj = NULL;
+    FILE* fp;
+#ifdef MS_WINDOWS
+    wchar_t wmode[5];
+    DWORD dwNum = MultiByteToWideChar(CP_ACP, 0, mode, -1, NULL, 0); 
+    if (dwNum > 4) {
+        PyErr_Format(PyExc_ValueError, "invalid mode: %.200s", mode);
+        return NULL;
+    }
+    MultiByteToWideChar(CP_ACP, 0, mode, -1, wmode, dwNum);
+    Py_UNICODE *widename = NULL;
+    if (!PyUnicode_FSDecoder(raw_path, &stringobj)) {
+        return NULL;
+    }
+    widename = PyUnicode_AsWideCharString(stringobj, NULL);
+    if (widename == NULL) {
+        return NULL;
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    fp = _wfopen(widename, wmode);
+    Py_END_ALLOW_THREADS
+#else
+    const char *name = NULL;
+    if (!PyUnicode_FSConverter(raw_path, &stringobj)) {
+        return NULL;
+    }
+    name = PyBytes_AS_STRING(stringobj);
+
+    Py_BEGIN_ALLOW_THREADS
+    fp = fopen(name, mode);
+    Py_END_ALLOW_THREADS
+#endif
+    if (fp == NULL) {
+        PyErr_SetFromErrno(PyExc_OSError);
+        // PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
+    }
+    if (out)
+        *out = stringobj;
+    else
+        Py_DECREF(stringobj);
+    return fp;
+}
+
+static __inline const char* unicode2string(PyObject* __s, Py_ssize_t* s_len) {
+    Py_ssize_t _s_len;
+    const char* s = PyUnicode_AsUTF8AndSize(__s, &_s_len);
+    if (s == NULL)
+        return NULL;
+    else if (strlen(s) != (size_t)_s_len) {
+        PyErr_SetString(PyExc_ValueError, "embedded null character");
+        return NULL;
+    }
+    if (s_len)
+        *s_len = _s_len;
+    return s;
+}
+
+// from cpython:string_parser.decode_unicode_with_escapes
+PyObject* decode_escapes(const char* s, Py_ssize_t len);
+PyObject* filter_text(PyObject* string);
+#endif
+
+#ifdef __cplusplus
+}
+#endif
 #endif
```

### Comparing `KoiLang-1.1.0b2/kola/_cutil.pxd` & `KoiLang-1.1.1/kola/_cutil.pxd`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from libc.stdio cimport FILE
-from libc.stdint cimport uint8_t, uint64_t
-from cpython cimport PyObject
-
-
-cdef extern from "<stdarg.h>":
-    ctypedef struct va_list
-    void va_start(va_list ap, const char* last_arg) nogil
-    void va_end(va_list ap) nogil
-
-cdef extern from "Python.h":
-    PyObject* _PyType_Lookup(type t, str name)
-    
-    ctypedef uint64_t Py_UCS4
-    
-    str PyUnicode_FromFormat(const char* format, ...)
-    Py_UCS4 PyUnicode_READ_CHAR(str unicode, Py_ssize_t index)
-    int PyUnicode_WriteChar(
-        str unicode, Py_ssize_t index, Py_UCS4 character) except -1
-
-    enum PyUnicode_Kind:
-        PyUnicode_WCHAR_KIND = 0
-        PyUnicode_1BYTE_KIND = 1
-        PyUnicode_2BYTE_KIND = 2
-        PyUnicode_4BYTE_KIND = 4
-
-    ctypedef struct _PyUnicodeWriter:
-        PyObject* buffer
-        void* data
-        PyUnicode_Kind kind
-        Py_UCS4 maxchar
-        Py_ssize_t size
-        Py_ssize_t pos
-
-        # minimum number of allocated characters (default: 0)
-        Py_ssize_t min_length
-
-        # minimum character (default: 127, ASCII)
-        Py_UCS4 min_char
-
-        # If non-zero, overallocate the buffer (default: 0).
-        unsigned char overallocate
-
-        # If readonly is 1, buffer is a shared string (cannot be modified)
-        # and size is set to 0.
-        unsigned char readonly_ "readonly"
-    
-    void _PyUnicodeWriter_Init(_PyUnicodeWriter *writer)
-    int _PyUnicodeWriter_Prepare(_PyUnicodeWriter *writer, Py_ssize_t length, Py_UCS4 maxchar) except -1
-    int _PyUnicodeWriter_PrepareKind(_PyUnicodeWriter *writer, PyUnicode_Kind kind) except -1
-    int _PyUnicodeWriter_WriteChar(_PyUnicodeWriter *writer, Py_UCS4 ch) except -1
-    int _PyUnicodeWriter_WriteStr(_PyUnicodeWriter *writer, str string) except -1
-    int _PyUnicodeWriter_WriteASCIIString(_PyUnicodeWriter *writer, const char* string, Py_ssize_t len) except -1
-    str _PyUnicodeWriter_Finish(_PyUnicodeWriter *writer)
-    void _PyUnicodeWriter_Dealloc(_PyUnicodeWriter *writer)
-
-
-cdef extern from "_cutil.h":
-    enum TokenSyn:
-        CMD
-        CMD_N
-        TEXT
-        LITERAL
-        STRING
-        NUM
-        NUM_H
-        NUM_B
-        NUM_F
-        CLN
-        CMA
-        SLP
-        SRP
-        ANNOTATION
-    const uint8_t yy_goto[7][8]
-
-    const int LFLAG_DISABLED
-    const int LFLAG_ISANNOTATION
-    const int LFLAG_NOLSTRIP
-    
-    ctypedef struct LexerData:
-        const char* filename
-        uint8_t command_threshold
-        uint8_t flag
-    ctypedef void* yyscan_t
-
-    void kola_set_error(object exc_type, int errorno, const char* filename, int lineno, const char* text) except *
-    void kola_set_errcause(object exc_type, int errorno, const char* filename, int lineno, const char* text, object cause) except *
-
-    FILE* kola_open(object raw_path, PyObject** out, const char* mod) except NULL
-
-    const char* get_type_name(object obj) nogil
-    const char* get_type_qualname(object obj) nogil
-    const char* unicode2string(str __s, Py_ssize_t* s_len) except NULL
-    str decode_escapes(const char* string, Py_ssize_t len)
-    PyObject* filter_text(str string) except NULL
+from libc.stdio cimport FILE
+from libc.stdint cimport uint8_t, uint64_t
+from cpython cimport PyObject
+
+
+cdef extern from "<stdarg.h>":
+    ctypedef struct va_list
+    void va_start(va_list ap, const char* last_arg) nogil
+    void va_end(va_list ap) nogil
+
+cdef extern from "Python.h":
+    PyObject* _PyType_Lookup(type t, str name)
+    
+    ctypedef uint64_t Py_UCS4
+    
+    str PyUnicode_FromFormat(const char* format, ...)
+    Py_UCS4 PyUnicode_READ_CHAR(str unicode, Py_ssize_t index)
+    int PyUnicode_WriteChar(
+        str unicode, Py_ssize_t index, Py_UCS4 character) except -1
+
+    enum PyUnicode_Kind:
+        PyUnicode_WCHAR_KIND = 0
+        PyUnicode_1BYTE_KIND = 1
+        PyUnicode_2BYTE_KIND = 2
+        PyUnicode_4BYTE_KIND = 4
+
+    ctypedef struct _PyUnicodeWriter:
+        PyObject* buffer
+        void* data
+        PyUnicode_Kind kind
+        Py_UCS4 maxchar
+        Py_ssize_t size
+        Py_ssize_t pos
+
+        # minimum number of allocated characters (default: 0)
+        Py_ssize_t min_length
+
+        # minimum character (default: 127, ASCII)
+        Py_UCS4 min_char
+
+        # If non-zero, overallocate the buffer (default: 0).
+        unsigned char overallocate
+
+        # If readonly is 1, buffer is a shared string (cannot be modified)
+        # and size is set to 0.
+        unsigned char readonly_ "readonly"
+    
+    void _PyUnicodeWriter_Init(_PyUnicodeWriter *writer)
+    int _PyUnicodeWriter_Prepare(_PyUnicodeWriter *writer, Py_ssize_t length, Py_UCS4 maxchar) except -1
+    int _PyUnicodeWriter_PrepareKind(_PyUnicodeWriter *writer, PyUnicode_Kind kind) except -1
+    int _PyUnicodeWriter_WriteChar(_PyUnicodeWriter *writer, Py_UCS4 ch) except -1
+    int _PyUnicodeWriter_WriteStr(_PyUnicodeWriter *writer, str string) except -1
+    int _PyUnicodeWriter_WriteASCIIString(_PyUnicodeWriter *writer, const char* string, Py_ssize_t len) except -1
+    str _PyUnicodeWriter_Finish(_PyUnicodeWriter *writer)
+    void _PyUnicodeWriter_Dealloc(_PyUnicodeWriter *writer)
+
+
+cdef extern from "_cutil.h":
+    enum TokenSyn:
+        CMD
+        CMD_N
+        TEXT
+        LITERAL
+        STRING
+        NUM
+        NUM_H
+        NUM_B
+        NUM_F
+        CLN
+        CMA
+        SLP
+        SRP
+        ANNOTATION
+    const uint8_t yy_goto[7][8]
+
+    const int LFLAG_DISABLED
+    const int LFLAG_ISANNOTATION
+    const int LFLAG_NOLSTRIP
+    
+    ctypedef struct LexerData:
+        const char* filename
+        uint8_t command_threshold
+        uint8_t flag
+    ctypedef void* yyscan_t
+
+    void kola_set_error(object exc_type, int errorno, const char* filename, int lineno, const char* text) except *
+    void kola_set_errcause(object exc_type, int errorno, const char* filename, int lineno, const char* text, object cause) except *
+
+    FILE* kola_open(object raw_path, PyObject** out, const char* mod) except NULL
+
+    const char* get_type_name(object obj) nogil
+    const char* get_type_qualname(object obj) nogil
+    const char* unicode2string(str __s, Py_ssize_t* s_len) except NULL
+    str decode_escapes(const char* string, Py_ssize_t len)
+    PyObject* filter_text(str string) except NULL
```

### Comparing `KoiLang-1.1.0b2/kola/_yylex.pxd` & `KoiLang-1.1.1/kola/_yylex.pxd`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from libc.stdio cimport FILE
-from ._cutil cimport yyscan_t, LexerData
-
-cdef extern from "lex.yy.c":
-    ctypedef LexerData* YY_EXTRA_TYPE
-    ctypedef void* YY_BUFFER_STATE
-
-    # main parser
-    int yylex(yyscan_t yyscanner) nogil
-    
-    int yylex_init(yyscan_t* ptr_yy_globals) nogil
-    int yylex_init_extra(YY_EXTRA_TYPE yy_user_defined, yyscan_t* ptr_yy_globals) nogil
-    int yylex_destroy(yyscan_t yyscanner) nogil
-    void yyrestart(FILE* input_file, yyscan_t yyscanner) nogil
-    bint yylex_check(yyscan_t yyscanner) nogil
-
-    # Accessor  methods (get/set functions) to struct members.
-    int yyget_lineno(yyscan_t yyscanner) nogil
-    int yyget_column(yyscan_t yyscanner) nogil
-    FILE *yyget_in(yyscan_t yyscanner) nogil
-    FILE *yyget_out(yyscan_t yyscanner) nogil
-    int yyget_leng(yyscan_t yyscanner) nogil
-    char* yyget_text(yyscan_t yyscanner) nogil
-    void yyset_lineno(int _line_number, yyscan_t yyscanner) nogil
-    void yyset_column(int _column_no , yyscan_t yyscanner) nogil
-    void yyset_in(FILE* _in_str , yyscan_t yyscanner) nogil
-    void yyset_out(FILE* _out_str , yyscan_t yyscanner) nogil
-
-    void yypush_buffer_state(YY_BUFFER_STATE new_buffer, yyscan_t yyscanner) nogil
-    void yypop_buffer_state(yyscan_t yyscanner) nogil
-    YY_BUFFER_STATE yy_create_buffer(FILE* file, int size, yyscan_t yyscanner) nogil
-    YY_BUFFER_STATE yy_scan_buffer(char* base, Py_ssize_t size, yyscan_t yyscanner) nogil
+from libc.stdio cimport FILE
+from ._cutil cimport yyscan_t, LexerData
+
+cdef extern from "lex.yy.c":
+    ctypedef LexerData* YY_EXTRA_TYPE
+    ctypedef void* YY_BUFFER_STATE
+
+    # main parser
+    int yylex(yyscan_t yyscanner) nogil
+    
+    int yylex_init(yyscan_t* ptr_yy_globals) nogil
+    int yylex_init_extra(YY_EXTRA_TYPE yy_user_defined, yyscan_t* ptr_yy_globals) nogil
+    int yylex_destroy(yyscan_t yyscanner) nogil
+    void yyrestart(FILE* input_file, yyscan_t yyscanner) nogil
+    bint yylex_check(yyscan_t yyscanner) nogil
+
+    # Accessor  methods (get/set functions) to struct members.
+    int yyget_lineno(yyscan_t yyscanner) nogil
+    int yyget_column(yyscan_t yyscanner) nogil
+    FILE *yyget_in(yyscan_t yyscanner) nogil
+    FILE *yyget_out(yyscan_t yyscanner) nogil
+    int yyget_leng(yyscan_t yyscanner) nogil
+    char* yyget_text(yyscan_t yyscanner) nogil
+    void yyset_lineno(int _line_number, yyscan_t yyscanner) nogil
+    void yyset_column(int _column_no , yyscan_t yyscanner) nogil
+    void yyset_in(FILE* _in_str , yyscan_t yyscanner) nogil
+    void yyset_out(FILE* _out_str , yyscan_t yyscanner) nogil
+
+    void yypush_buffer_state(YY_BUFFER_STATE new_buffer, yyscan_t yyscanner) nogil
+    void yypop_buffer_state(yyscan_t yyscanner) nogil
+    YY_BUFFER_STATE yy_create_buffer(FILE* file, int size, yyscan_t yyscanner) nogil
+    YY_BUFFER_STATE yy_scan_buffer(char* base, Py_ssize_t size, yyscan_t yyscanner) nogil
     YY_BUFFER_STATE yy_scan_bytes(const char* text, int len, yyscan_t yyscanner) nogil
```

### Comparing `KoiLang-1.1.0b2/kola/klvm/command.py` & `KoiLang-1.1.1/kola/klvm/command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,89 @@
-from types import MethodType
-from typing import Any, Callable, Dict, Generator, Iterable, Tuple, Union, overload
-from typing_extensions import Self, Protocol, runtime_checkable
-
-
-class CommandCaller(Protocol):
-    def __call__(self, __command: Any, __args: tuple, __kwargs: Dict[str, Any], **kwds: Any) -> Any: ...
-
-
-@runtime_checkable
-class CommandLike(Protocol):
-    def __kola_command__(self) -> Generator[Tuple[str, Callable], None, None]: ...
-
-
-class Command(object):
-    __slots__ = ["__name__", "__func__", "suppression", "alias", "extra_data"]
-
-    def __init__(
-        self,
-        __name: str,
-        func: Callable,
-        *,
-        alias: Union[Iterable[str], str] = tuple(),
-        suppression: bool = False,
-        **kwds: Any
-    ) -> None:
-        self.__name__ = __name
-        self.__func__ = func
-        self.alias = (alias,) if isinstance(alias, str) else tuple(alias)
-        self.suppression = suppression
-        self.extra_data = kwds
-    
-    @overload
-    def set_data(self, __name: str, value: Any) -> Self: ...
-    @overload
-    def set_data(self, __name: str) -> Callable[[Any], Self]: ...
-
-    def set_data(self, __name: str, value: Any = None) -> Union[Self, Callable[[Any], Self]]:
-        if value is not None:
-            self.extra_data[__name] = value
-            return self
-        
-        def wrapper(val: Any) -> Self:
-            self.extra_data[__name] = val
-            return self
-        return wrapper
-
-    def writer(self, func: Callable) -> Self:
-        self.extra_data["writer_func"] = func
-        return self
-    
-    @classmethod
-    def from_command(cls, command: "Command", **kwds: Any) -> Self:
-        data = command.extra_data.copy()
-        data.update(kwds)
-        return cls(
-            command.__name__,
-            command.__func__,
-            alias=command.alias,
-            **data
-        )
-    
-    @property
-    def __wrapped__(self) -> Callable:
-        return self.__func__
-    
-    def __kola_command__(self, force: bool = False) -> Generator[Tuple[str, Self], None, None]:
-        if not self.suppression or force:
-            bound_func = self
-            yield self.__name__, bound_func
-            for i in self.alias:
-                yield i, bound_func
-
-    def __get__(self, ins: Any, owner: type) -> Any:
-        if ins is None:
-            return self
-        return MethodType(self, ins)
-
-    def __call__(self, vmobj: Any, *args: Any, **kwds: Any) -> Any:
-        caller = getattr(vmobj, "__kola_caller__", None)
-        if caller is None:
-            return self.__func__(vmobj, *args, **kwds)
-        return caller(self, args, kwds, **self.extra_data)
-
-    def __repr__(self) -> str:
-        return f"<kola command {self.__name__} with {self.__func__}>"
+from functools import partialmethod
+from types import MethodType
+from typing import Any, Callable, Dict, Generator, Iterable, Tuple, Union, overload
+from typing_extensions import Self, Protocol, runtime_checkable
+
+
+class CommandCaller(Protocol):
+    def __call__(self, __command: Any, __args: tuple, __kwargs: Dict[str, Any], **kwds: Any) -> Any: ...
+
+
+@runtime_checkable
+class CommandLike(Protocol):
+    def __kola_command__(self) -> Generator[Tuple[str, Callable], None, None]: ...
+
+
+class Command(object):
+    __slots__ = ["__name__", "__func__", "suppression", "virtual", "alias", "extra_data"]
+
+    def __init__(
+        self,
+        __name: str,
+        func: Callable,
+        *,
+        alias: Union[Iterable[str], str] = (),
+        suppression: bool = False,
+        virtual: bool = False,
+        **kwds: Any
+    ) -> None:
+        self.__name__ = __name
+        self.__func__ = func
+        self.alias = (alias,) if isinstance(alias, str) else tuple(alias)
+        self.suppression = suppression
+        self.virtual = virtual
+        self.extra_data = kwds
+    
+    @overload
+    def set_data(self, __name: str, value: Any) -> Self: ...
+    @overload
+    def set_data(self, __name: str) -> Callable[[Any], Self]: ...
+
+    def set_data(self, __name: str, value: Any = None) -> Union[Self, Callable[[Any], Self]]:
+        if value is not None:
+            self.extra_data[__name] = value
+            return self
+        
+        def wrapper(val: Any) -> Self:
+            self.extra_data[__name] = val
+            return self
+        return wrapper
+
+    writer = partialmethod(set_data, "writer_func")
+    
+    @classmethod
+    def from_command(cls, command: "Command", **kwds: Any) -> Self:
+        data = command.extra_data.copy()
+        data.update(kwds)
+        return cls(
+            command.__name__,
+            command.__func__,
+            alias=command.alias,
+            **data
+        )
+    
+    @property
+    def __wrapped__(self) -> Callable:  # pragma: no cover
+        return self.__func__
+    
+    def __kola_command__(self, force: bool = False) -> Generator[Tuple[str, Self], None, None]:
+        if not self.suppression or force:
+            bound_func = self
+            yield self.__name__, bound_func
+            for i in self.alias:
+                yield i, bound_func
+
+    def __get__(self, ins: Any, owner: type) -> Any:
+        if ins is None:
+            return self
+        elif self.virtual and (not hasattr(owner, "check_virtual") or ins.check_virtual(self)):
+            return ins[self.__name__]
+        return MethodType(self, ins)
+
+    def __call__(self, vmobj: Any, *args: Any, **kwds: Any) -> Any:
+        caller = getattr(vmobj, "__kola_caller__", None)
+        if caller is None:  # pragma: no cover
+            return self.__func__(vmobj, *args, **kwds)
+        return caller(self, args, kwds, **self.extra_data)
+
+    def __repr__(self) -> str:
+        return f"<kola command {self.__name__} with {self.__func__}>"
```

### Comparing `KoiLang-1.1.0b2/kola/klvm/commandset.pyi` & `KoiLang-1.1.1/kola/klvm/commandset.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-from abc import ABCMeta
-from typing import (Any, Callable, Dict, Iterable, Optional, Set, Tuple, Union,
-                    overload)
-
-from typing_extensions import Self
-
-from .command import Command, CommandLike
-
-
-class CommandSetMeta(ABCMeta):
-    __command_field__: Set[CommandLike]
-
-    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self: ...
-    def generate_raw_commands(self) -> Dict[str, Any]: ...
-    @overload
-    def register_command(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_command(
-        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_text(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_text(
-        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_number(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_number(
-        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_annotation(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_annotation(
-        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    
-
-class CommandSet(metaclass=CommandSetMeta):
-    raw_command_set: Dict[str, Callable]
-    _bound_command_set: Dict[str, Callable]
-
-    def __init__(self) -> None: ...
-    def get(self, __key: str, default: Optional[Callable] = ...) -> Optional[Callable]: ...
-    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds) -> Any: ...
-    def __getitem__(self, __key: str) -> Callable: ...
-
+from abc import ABCMeta
+from typing import (Any, Callable, Dict, Iterable, Optional, Set, Tuple, Union,
+                    overload)
+
+from typing_extensions import Self
+
+from .command import Command, CommandLike
+from .mask import Mask, ClassTypeMask
+
+
+class CommandSetMeta(ABCMeta):
+    __command_field__: Set[CommandLike]
+    __virtual_table__: Dict[str, str]
+
+    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self: ...
+    def generate_raw_commands(self) -> Dict[str, Any]: ...
+    @overload
+    def register_command(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_command(
+        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_text(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_text(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_number(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_number(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_annotation(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_annotation(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    
+
+class CommandSet(metaclass=CommandSetMeta):
+    __slots__ = ["raw_command_set", "_bound_command_cache"]
+
+    raw_command_set: Dict[str, Callable]
+    _bound_command_set: Dict[str, Callable]
+
+    def __init__(self) -> None: ...
+    def check_virtual(self, command: Command) -> bool: ...
+    def get(self, __key: str, default: Optional[Callable] = ...) -> Optional[Callable]: ...
+    @classmethod
+    def mask(cls, type: Union["Mask.MType", str] = "") -> ClassTypeMask: ...
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds) -> Any: ...
+    def __getitem__(self, __key: str) -> Callable: ...
```

### Comparing `KoiLang-1.1.0b2/kola/klvm/decorator.py` & `KoiLang-1.1.1/kola/klvm/decorator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from types import new_class
-from typing import Any, Callable, Optional, Type, Union
-
-from .command import Command
-from .commandset import CommandSet
-from .environment import Environment, EnvironmentEntry, EnvironmentExit
-from .koilang import KoiLang
-
-
-def _kola_decorator_factory(cmd_name: Optional[str] = None, cmd_type: Type[Command] = Command):
-    def kola_decorator(
-        func: Union[Callable[..., Any], str, None] = None,
-        **kwds
-    ) -> Union[Command, Callable[[Callable], Command]]:
-        def wrapper(wrapped_func: Callable[..., Any]) -> Command:
-            nonlocal cmd_type
-            if cmd_name is not None:
-                assert not isinstance(func, str)
-                name = cmd_name
-            elif isinstance(func, str):
-                name = func
-            else:
-                name = wrapped_func.__name__
-            return cmd_type(name, wrapped_func, **kwds)
-        if callable(func):
-            return wrapper(func)
-        else:
-            return wrapper
-    return kola_decorator
-
-
-kola_command = _kola_decorator_factory()
-kola_text = _kola_decorator_factory("@text")
-kola_number = _kola_decorator_factory("@number")
-kola_annotation = _kola_decorator_factory("@annotation")
-kola_env_enter = _kola_decorator_factory(cmd_type=EnvironmentEntry)
-kola_env_exit = _kola_decorator_factory(cmd_type=EnvironmentExit)
-
-
-def _kola_class_decorator_factory(base: Type[CommandSet] = CommandSet):
-    def kola_class_decoractor(kola_cls: Union[Type[KoiLang], str, None] = None, **kwds):
-        def wrapper(wrapped_class: Type) -> Type[CommandSet]:
-            if isinstance(kola_cls, str):
-                env_name = kola_cls
-            else:
-                env_name = wrapped_class.__name__
-            
-            return new_class(
-                env_name,
-                (base,),
-                kwds,
-                lambda attrs: attrs.update(wrapped_class.__dict__)
-            )
-        if isinstance(kola_cls, type):
-            return wrapper(kola_cls)
-        else:
-            return wrapper
-    return kola_class_decoractor
-
-
-kola_command_set = _kola_class_decorator_factory()
-kola_environment = _kola_class_decorator_factory(Environment)
-kola_main = _kola_class_decorator_factory(KoiLang)
+from types import new_class
+from typing import Any, Callable, Optional, Type, Union
+
+from .command import Command
+from .commandset import CommandSet
+from .environment import Environment, EnvironmentEntry, EnvironmentExit
+from .koilang import KoiLang
+
+
+def _kola_decorator_factory(cmd_name: Optional[str] = None, cmd_type: Type[Command] = Command):
+    def kola_decorator(
+        func: Union[Callable[..., Any], str, None] = None,
+        **kwds
+    ) -> Union[Command, Callable[[Callable], Command]]:
+        def wrapper(wrapped_func: Callable[..., Any]) -> Command:
+            nonlocal cmd_type
+            if cmd_name is not None:
+                assert not isinstance(func, str)
+                name = cmd_name
+            elif isinstance(func, str):
+                name = func
+            else:
+                name = wrapped_func.__name__
+            return cmd_type(name, wrapped_func, **kwds)
+        if callable(func):
+            return wrapper(func)
+        else:
+            return wrapper
+    return kola_decorator
+
+
+kola_command = _kola_decorator_factory()
+kola_text = _kola_decorator_factory("@text")
+kola_number = _kola_decorator_factory("@number")
+kola_annotation = _kola_decorator_factory("@annotation")
+kola_env_enter = _kola_decorator_factory(cmd_type=EnvironmentEntry)
+kola_env_exit = _kola_decorator_factory(cmd_type=EnvironmentExit)
+
+
+def _kola_class_decorator_factory(base: Type[CommandSet] = CommandSet):
+    def kola_class_decoractor(kola_cls: Union[Type[KoiLang], str, None] = None, **kwds):
+        def wrapper(wrapped_class: Type) -> Type[CommandSet]:
+            if isinstance(kola_cls, str):
+                env_name = kola_cls
+            else:
+                env_name = wrapped_class.__name__
+            
+            return new_class(
+                env_name,
+                (base,),
+                kwds,
+                lambda attrs: attrs.update(wrapped_class.__dict__)
+            )
+        if isinstance(kola_cls, type):
+            return wrapper(kola_cls)
+        else:
+            return wrapper
+    return kola_class_decoractor
+
+
+kola_command_set = _kola_class_decorator_factory()
+kola_environment = _kola_class_decorator_factory(Environment)
+kola_main = _kola_class_decorator_factory(KoiLang)
```

### Comparing `KoiLang-1.1.0b2/kola/klvm/koilang.py` & `KoiLang-1.1.1/kola/lib/disabled.jklvm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,343 +1,327 @@
-from contextlib import contextmanager
-import os
-import sys
-from threading import Lock
-from types import TracebackType, new_class
-from typing import Any, Callable, ClassVar, Dict, Generator, Optional, Tuple, Type, TypeVar, Union, overload
-from typing_extensions import Literal, Self
-
-from ..lexer import BaseLexer, FileLexer, StringLexer
-from ..parser import Parser
-from ..exception import KoiLangError
-from .command import Command
-from .commandset import CommandSetMeta, CommandSet
-from .environment import Environment
-
-
-_T_EnvCls = TypeVar("_T_EnvCls", bound=Type[Environment])
-
-
-class KoiLangMeta(CommandSetMeta):
-    """
-    metaclass for KoiLang class
-
-    Provide encoding and command threshold support.
-    """
-    __text_encoding__: str
-    __command_threshold__: int
-
-    builtin_mapping: ClassVar[Dict[str, str]] = {
-        "at_start": "@start", "at_end": "@end", "on_exception": "@exception"
-    }
-
-    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any],
-                command_threshold: int = 0, encoding: Optional[str] = None, **kwds: Any):
-        """
-        create a top-level language class
-
-        :param name: class name
-        :type name: str
-        :param bases: class bases
-        :type bases: Tuple[type, ...]
-        :param attr: class namespace
-        :type attr: Dict[str, Any]
-        :param command_threshold: the `#` prefix length of commands, defaults to 0
-        :type command_threshold: int, optional
-        :param encoding: encoding for file parsing, defaults to None
-        :type encoding: Optional[str], optional
-        :return: new class
-        :rtype: KoiLangMeta
-        """
-        has_base = any(isinstance(i, cls) for i in bases)
-        if command_threshold or not has_base:
-            assert command_threshold >= 0
-            attr["__command_threshold__"] = command_threshold or 1
-        if encoding or not has_base:
-            attr["__text_encoding__"] = encoding or "utf-8"
-        for k, n in cls.builtin_mapping.items():
-            if k not in attr:
-                continue
-            cmd = attr[k]
-            if not isinstance(cmd, Command):
-                attr[k] = Command(n, cmd)
-        return super().__new__(cls, name, bases, attr, **kwds)
-
-    def register_environment(self, env_class: _T_EnvCls) -> _T_EnvCls:
-        self.__command_field__.add(env_class)
-        return env_class
-    
-    @property
-    def writer(self) -> Type:
-        cache = getattr(self, "__writer_class__", None)
-        if cache is not None:
-            return cache
-        cache = new_class(f"{self.__qualname__}.writer", (KoiLangWriter, self))
-        self.__writer_class__ = cache
-        return cache
-
-
-class KoiLang(CommandSet, metaclass=KoiLangMeta):
-    """
-    main class for KoiLang virtual machine
-
-    `KoiLang` class is the top-level interface of 'kola' package.
-    Just create a subclass to define your own markup language based on KoiLang.
-    """
-    __slots__ = ["_lock", "__top", "__exec_level"]
-
-    def __init__(self) -> None:
-        super().__init__()
-        self._lock = Lock()
-        self.__top = self
-        self.__exec_level = 0
-    
-    def push_start(self, __env_type: Type[Environment]) -> Environment:
-        env = __env_type(self.__top)
-        env.at_initialize(self.__top)
-        return env
-
-    def push_end(self, __env_cache: Environment) -> None:
-        assert __env_cache.back is self.__top
-        with self._lock:
-            self.__top = __env_cache
-    
-    def pop_start(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
-        top = self.__top
-        if top is self:
-            raise ValueError('cannot pop the inital environment')
-        if __env_type is None:
-            assert isinstance(top, Environment)
-        else:
-            while isinstance(top, Environment) and top.__class__.__env_autopop__:
-                if isinstance(top, __env_type):
-                    break
-                top = top.back
-            else:
-                if not isinstance(top, __env_type):
-                    raise ValueError("unmatched environment")
-        return top
-
-    def pop_end(self, __env_cache: Environment) -> None:
-        with self._lock:
-            top = self.__top
-            self.__top = __env_cache.back
-        while isinstance(top, Environment):
-            top.at_finalize(self.__top)
-            if top is __env_cache:
-                break
-            top = top.back
-        else:
-            raise ValueError('cannot pop the inital environment')
-    
-    def ensure_env(self, names: Tuple[str, ...]) -> None:
-        if isinstance(names, str):
-            names = (names,)
-
-        ng, pt = [], []
-        for i in names:
-            if i.startswith('!'):
-                ng.append(i[1:])
-            else:
-                pt.append(i)
-
-        reachable = []
-        top = self.top
-        while isinstance(top, Environment):
-            reachable.append(top.__class__.__name__)
-            if not top.__class__.__env_autopop__:
-                break
-            top = top.back
-        else:
-            # the base KoiLang object name is '__init__'
-            reachable.append("__init__")
-
-        if ((not ng or all(not self._ensure_env(reachable, i) for i in ng)) and
-                (not pt or any(self._ensure_env(reachable, i) for i in pt))):
-            return
-        raise ValueError(f"unmatched environment name {reachable[0]}")
-    
-    @staticmethod
-    def _ensure_env(reachable: list, name: str) -> bool:
-        if name.startswith('+'):
-            strict = True
-            name = name[1:]
-        else:
-            strict = False
-        if name.startswith('!'):
-            inverse = True
-            name = name[1:]
-        else:
-            inverse = False
-
-        if strict:
-            is_in = reachable[0] == name
-        else:
-            is_in = name in reachable
-        return not is_in if inverse else is_in
-
-        # for n in names:
-        #     if n.startswith('+!'):
-        #         while n[2:] in reachable:
-        #             if len(reachable) < 2:
-        #                 break
-        #             cache = self.pop_start()
-        #             self.pop_end(cache)
-        #             reachable.popleft()
-        #         else:
-        #             continue
-        #     elif n.startswith('!'):
-        #         if any(i != n[1:] for i in reachable):
-        #             continue
-        #     elif n.startswith('+'):
-        #         while reachable[0] != n[1:]:
-        #             if len(reachable) < 2:
-        #                 break
-        #             cache = self.pop_start()
-        #             self.pop_end(cache)
-        #             reachable.popleft()
-        #         else:
-        #             continue
-        #     elif n in reachable:
-        #         continue
-        #     raise ValueError(f"unmatched environment name {n}")
-    
-    def __parse(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> None:
-        parser = Parser(__lexer, self)
-        try:
-            with self.exec_block():
-                while True:
-                    try:
-                        # Parser.exec() is a fast C level loop
-                        parser.exec()
-                    except KoiLangError:
-                        if not self["@exception"](*sys.exc_info()):
-                            raise
-                    else:
-                        break
-        finally:
-            if close_lexer:
-                __lexer.close()
-    
-    def __parse_and_ret(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> Generator[Any, None, None]:
-        parser = Parser(__lexer, self)
-        try:
-            with self.exec_block():
-                while True:
-                    try:
-                        yield from parser
-                    except KoiLangError:
-                        if not self["@exception"](*sys.exc_info()):
-
-                            raise
-                    else:
-                        break
-        finally:
-            if close_lexer:
-                __lexer.close()
-
-    @overload
-    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: Literal[False] = False, close_lexer: bool = True) -> None: ...
-    @overload  # noqa: E301
-    def parse(
-        self,
-        lexer: Union[BaseLexer, str],
-        *,
-        with_ret: Literal[True],
-        close_lexer: bool = True
-    ) -> Generator[Any, None, None]: ...
-    
-    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: bool = False, close_lexer: bool = True) -> Any:
-        """
-        Parse kola text or lexer from other method.
-        """
-        if isinstance(lexer, str):
-            if not close_lexer:
-                raise ValueError("inner string lexer must be closed at the end of parsing")
-            lexer = StringLexer(
-                lexer,
-                encoding=self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__
-            )
-        if with_ret:
-            return self.__parse_and_ret(lexer, close_lexer=close_lexer)
-        else:
-            self.__parse(lexer, close_lexer=close_lexer)
-        
-    def parse_file(self, path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> Any:
-        """
-        Parse a kola file.
-        """
-        return self.parse(
-            FileLexer(
-                path, encoding=encoding or self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__
-            ), **kwds
-        )
-    
-    @contextmanager
-    def exec_block(self) -> Generator[Self, None, None]:
-        if not self.__exec_level:
-            self["@start"]()
-        self.__exec_level += 1
-        try:
-            yield self
-        finally:
-            self.__exec_level -= 1
-            if not self.__exec_level:
-                self["@end"]()
-
-    def __getitem__(self, __key: str) -> Callable:
-        if self.__top is self:
-            return super().__getitem__(__key)
-        return self.__top[__key]
-
-    def __kola_caller__(
-        self,
-        command: Command,
-        args: tuple,
-        kwargs: Dict[str, Any],
-        *,
-        bound_instance: Optional[CommandSet] = None,
-        envs: Tuple[str, ...] = (),
-        **kwds: Any
-    ) -> Any:
-        if envs:
-            self.ensure_env(envs)
-        return command.__func__(bound_instance or self, *args, **kwargs)
-
-    @property
-    def top(self) -> CommandSet:
-        return self.__top
-    
-    @property
-    def home(self) -> Self:
-        return self
-
-    def at_start(self) -> None:
-        """
-        parser initalize command
-        
-        It is called before parsing start.
-        """
-
-    def at_end(self) -> None:
-        """
-        parser finalize command
-        
-        It is called after parsing end. And the return value
-        will be that of 'parse' method.
-        """
-        while isinstance(self.__top, Environment) and self.__top.__class__.__env_autopop__:
-            cache = self.pop_start()
-            self.pop_end(cache)
-    
-    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> None:
-        """
-        exception handling command
-
-        It is called when a KoiLang error occurs.
-        If the command wishes to suppress the exception, it should a true value.
-        """
-
-
-from .writer import KoiLangWriter
+import sys
+from operator import index
+from types import TracebackType
+from typing import (Any, Dict, Generator, Iterator, List, MutableSequence, NoReturn, Optional, SupportsIndex, Type,
+                    Union, overload)
+from typing_extensions import Literal
+
+from kola.exception import KoiLangError
+from kola.lexer import BaseLexer, StringLexer
+from kola.parser import Parser
+from kola.klvm import Command, CommandSet, Environment, KoiLang, kola_command
+from kola.lib.recorder import Instruction, recorder
+
+
+class CodeSection:
+    __slots__ = ["_codes", "base", "_length"]
+
+    def __init__(self, __base_codes: Union[List[Instruction], "CodeSection", None] = None, base: int = 0) -> None:
+        self._length = -1
+        self.base = 0
+        if __base_codes is None:
+            # run in real address mode
+            assert base == 0
+            self._codes = []
+        elif isinstance(__base_codes, list):
+            assert base == 0
+            self._codes = __base_codes
+            self._length = len(__base_codes)
+        else:
+            self._codes = __base_codes._codes
+            self.base = base + __base_codes.base
+    
+    def __getitem__(self, __index: SupportsIndex) -> Instruction:
+        __index = index(__index)
+        if __index < 0 or (self._length >= 0 and __index >= self._length):  # pragma: no cover
+            raise JKlvmAddressError("instruction access out of bounds", address=__index)
+        __index += self.base
+        return self._codes[__index]
+    
+    def append(self, instruction: Instruction) -> None:
+        if self._length != -1:
+            raise RuntimeError("modify a frozen section")
+        self._codes.append(instruction)
+    
+    def freeze(self, end: int = 0) -> None:
+        if self._length <= 0:
+            self._length = end or len(self._codes)
+    
+    def __iter__(self) -> Iterator[Instruction]:
+        return iter(self._codes[self.base:self.base + len(self)])
+    
+    def __bool__(self) -> bool:
+        return self._length > 0 or bool(self._codes)
+    
+    def __len__(self) -> int:
+        if self._length >= 0:
+            return self._length
+        raise RuntimeError("The effective length of this environment section is not set")  # pragma: no cover
+
+
+class JCommandSet(CommandSet):
+    """
+    base class for JKLvm classes
+    """
+    codes: CodeSection
+    labels: Dict[str, int]
+    exit_points: Dict[int, int]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.__ip = 0
+        self.labels = {}
+        
+    def step(self) -> Any:
+        name, args, kwargs = self.codes[self.ip]
+        self.__ip += 1
+        try:
+            return self[name](*args, **kwargs)
+        except KoiLangError:
+            if not self.on_exception(*sys.exc_info()):
+                raise
+    
+    def add_label(self, name: str, address: int) -> None:
+        self.labels[name] = address
+    
+    def goto(self, __address: Union[int, str]) -> NoReturn:
+        if isinstance(__address, str):
+            __address = self.labels[__address]
+        raise JKLvmJump(__address, base=self.codes.base)
+    
+    def exit(self) -> NoReturn:
+        raise JKLvmExit(0)
+    
+    @property
+    def ip(self) -> int:
+        return self.__ip
+    
+    @ip.setter
+    def ip(self, __address: int) -> None:
+        if __address < 0 or __address >= len(self.codes):  # pragma: no cover
+            raise JKlvmAddressError("instruction access out of bounds", address=__address)
+        self.__ip = __address
+    
+    @kola_command("@exception", virtual=True)
+    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> Any:
+        if issubclass(exc_type, JKLvmExit):
+            # set the value of the ip register to the length of
+            # the code cache to make JKlvm exit the loop.
+            self.__ip = len(self.codes)
+            return True
+        elif issubclass(exc_type, JKLvmJump):
+            assert isinstance(exc_ins, JKLvmJump)
+            self.ip = exc_ins.address + exc_ins.base
+            return True
+        return False
+
+
+class JEnvironment(JCommandSet, Environment):
+    """
+    an environemnt implementation that can use jump instructions in the environment
+    """
+    __slots__ = ["codes", "state", "labels"]
+
+    # state flag
+    STATE_RECORD = -1
+    STATE_READ_AHEAD = 0
+    STATE_EXECUTE = 1
+    STATE_INHERIT = 2
+
+    def __read_ahead(self, base: "JKoiLang") -> None:
+        if not hasattr(base, "exit_points"):
+            base.exit_points = {}
+        
+    def __execute(self) -> None:
+        self.ip = 0
+        length = len(self.codes)
+        while self.ip != length:
+            self.step()
+    
+    @property
+    def ip(self) -> int:
+        if self.state <= JEnvironment.STATE_READ_AHEAD:  # pragma: no cover
+            raise RuntimeError("cannot use reg ip in redaing mode")
+        elif self.state == JEnvironment.STATE_INHERIT:
+            home = self.jhome
+            return home.ip - self.codes.base
+        return super().ip
+    
+    @ip.setter
+    def ip(self, __address: int) -> None:
+        if self.state <= JEnvironment.STATE_READ_AHEAD:  # pragma: no cover
+            raise RuntimeError("cannot use reg ip in redaing mode")
+        elif self.state == JEnvironment.STATE_INHERIT:
+            home = self.jhome
+            home.ip = __address + self.codes.base
+        else:
+            super().ip = __address
+    
+    @property
+    def jhome(self) -> JCommandSet:
+        cur = self
+        while isinstance(cur, Environment):
+            if isinstance(cur, JEnvironment) and cur.state in [
+                JEnvironment.STATE_EXECUTE, JEnvironment.STATE_READ_AHEAD,
+            ]:
+                return cur
+            cur = cur.back
+        else:
+            if not isinstance(cur, JKoiLang):  # pragma: no cover
+                raise TypeError("no running JKLvm found")
+            return cur
+
+    def set_up(self, cur_top: CommandSet) -> None:
+        super().set_up(cur_top)
+
+        self.labels = {}
+        while isinstance(cur_top, Environment):
+            if isinstance(cur_top, JEnvironment):
+                if cur_top.state <= JEnvironment.STATE_READ_AHEAD:
+                    self.state = JEnvironment.STATE_RECORD
+                else:
+                    self.state = JEnvironment.STATE_INHERIT
+                break
+            cur_top = cur_top.back
+        else:
+            if isinstance(cur_top, JKoiLang):
+                self.state = JEnvironment.STATE_INHERIT
+                if not hasattr(cur_top, "exit_points"):
+                    cur_top.exit_points = {}
+            else:
+                self.state = JEnvironment.STATE_READ_AHEAD
+                self.codes = CodeSection()
+                self.exit_points = {}
+                return
+        self.codes = CodeSection(cur_top.codes, cur_top.ip - 1)
+        if self.state == JEnvironment.STATE_INHERIT:
+            try:
+                m_ep = self.jhome.exit_points
+                length = m_ep[self.codes.base]
+            except Exception as e:
+                raise JKlvmAddressError("fail to fetch infomation of the exit point", address=self.ip) from e
+            self.codes.freeze(length)
+    
+    def tear_down(self, cur_top: CommandSet) -> None:
+        if self.state == JEnvironment.STATE_RECORD:
+            jhome = self.jhome
+            assert isinstance(jhome, JEnvironment)
+            jhome.exit_points[self.codes.base] = self.ip
+        elif self.state == JEnvironment.STATE_READ_AHEAD:
+            self.state = JEnvironment.STATE_EXECUTE
+            self.__execute()
+        super().tear_down(cur_top)
+    
+    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> bool:
+        if issubclass(exc_type, JKLvmExit):
+            assert isinstance(exc_ins, exc_type)
+            if exc_ins.target is self:
+                try:
+                    m_ep: Any = self.jhome.exit_points  # type: ignore
+                    self.ip = m_ep[self.codes.base]
+                except Exception as e:
+                    raise JKlvmAddressError("fail to fetch infomation of the exit point", address=self.ip) from e
+                self.on_autopop()
+                return True
+        return self.back["@exception"](exc_type, exc_ins, traceback)
+
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
+        if self.state > JEnvironment.STATE_READ_AHEAD:
+            return super().__kola_caller__(command, args, kwargs, **kwds)
+        # preread mode, just record to cache
+        assert isinstance(self.codes, MutableSequence)
+        self.codes.append(Instruction(command.__name__, args, kwargs))
+
+
+class JKoiLang(JCommandSet, KoiLang):
+    """
+    a KoiLang implementation that can use global jump instructions
+    """
+    __slots__ = ["codes", "labels"]
+
+    def __execute(self) -> Generator[Any, None, None]:
+        self.codes.freeze()
+        with self.exec_block():
+            while self.ip != len(self.codes):
+                yield self.step()
+
+    @overload
+    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: Literal[False] = False, close_lexer: bool = True) -> None: ...
+    @overload  # noqa: E301
+    def parse(
+        self,
+        lexer: Union[BaseLexer, str],
+        *,
+        with_ret: Literal[True],
+        close_lexer: bool = True
+    ) -> Generator[Any, None, None]: ...
+    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: bool = False, close_lexer: bool = True) -> Any:  # noqa: E301
+        if isinstance(lexer, str):
+            if not close_lexer:
+                raise ValueError("inner string lexer must be closed at the end of parsing")
+            lexer = StringLexer(
+                lexer,
+                encoding=self.__class__.__text_encoding__,
+                command_threshold=self.__class__.__command_threshold__,
+                no_lstrip=not self.__class__.__text_lstrip__
+            )
+        
+        # read all command info
+        codes = []
+        while True:
+            try:
+                codes.extend(Parser(lexer, recorder))
+            except KoiLangError:
+                if not self.on_exception(*sys.exc_info()):
+                    if close_lexer:
+                        lexer.close()
+                    raise
+            else:
+                break
+        if close_lexer:
+            lexer.close()
+        
+        # start execution
+        self.codes = CodeSection(codes)
+        gen = self.__execute()
+        if with_ret:
+            return gen
+        for _ in gen:
+            pass
+    
+    def at_start(self) -> None:
+        super().at_start()
+        self.ip: int = 0
+        self.labels: Dict[str, int] = {}
+
+
+class JKLvmException(KoiLangError):
+    """the base exception used in JKLvm"""
+    __slots__ = []
+
+
+class JKlvmAddressError(JKLvmException):
+    """incurrect instruction address"""
+    __slots__ = ["address"]
+
+    def __init__(self, *args: object, address: Optional[int] = None) -> None:
+        super().__init__(*args)
+        self.address = address
+
+
+class JKLvmExit(JKLvmException):
+    """exit from an environemnt"""
+    __slots__ = ["target"]
+    
+    def __init__(self, *args: object, target: Optional[JCommandSet] = None) -> None:
+        super().__init__(*args)
+        self.target = target
+
+
+class JKLvmJump(JKLvmException):
+    """jump to a new address"""
+    __slots__ = ["address", "base"]
+    
+    def __init__(self, address: int, *, base: int = 0) -> None:
+        super().__init__(f"{address:08X}+{base:08X}")
+        self.address = address
+        self.base = base
```

### Comparing `KoiLang-1.1.0b2/kola/lexer.c` & `KoiLang-1.1.1/kola/lexer.c`

 * *Files 2% similar despite different names*

```diff
@@ -1255,28 +1255,28 @@
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 typedef struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 
-/* "kola/lexer.pxd":35
+/* "kola/lexer.pxd":39
  *     cpdef void close(self)
  *     cdef void set_error(self, const char* text) except *
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil             # <<<<<<<<<<<<<<
  *     cdef Token next_token(self)
  * 
  */
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t {
   int f0;
   char const *f1;
   Py_ssize_t f2;
 };
 
-/* "kola/lexer.pxd":8
+/* "kola/lexer.pxd":12
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 struct __pyx_obj_4kola_5lexer_Token {
@@ -1286,29 +1286,29 @@
   enum TokenSyn syn;
   PyObject *val;
   PyObject *raw_val;
   int lineno;
 };
 
 
-/* "kola/lexer.pxd":20
+/* "kola/lexer.pxd":24
  * 
  * 
  * cdef class LexerConfig:             # <<<<<<<<<<<<<<
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer
  */
 struct __pyx_obj_4kola_5lexer_LexerConfig {
   PyObject_HEAD
   LexerData *lexer_data;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
 };
 
 
-/* "kola/lexer.pxd":26
+/* "kola/lexer.pxd":30
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 struct __pyx_obj_4kola_5lexer_BaseLexer {
@@ -1316,58 +1316,58 @@
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtab;
   yyscan_t scanner;
   LexerData lexer_data;
   PyObject *encoding;
 };
 
 
-/* "kola/lexer.pxd":39
+/* "kola/lexer.pxd":43
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 struct __pyx_obj_4kola_5lexer_FileLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *_filenameo;
   PyObject *_filenameb;
   FILE *fp;
 };
 
 
-/* "kola/lexer.pxd":49
+/* "kola/lexer.pxd":53
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 struct __pyx_obj_4kola_5lexer_StringLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *content;
 };
 
 
 
-/* "kola/lexer.pyx":34
+/* "kola/lexer.pyx":37
  * 
  * @cython.final
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     """
  *     Token used in lexer
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_Token {
   int (*get_flag)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_Token *__pyx_vtabptr_4kola_5lexer_Token;
 static int __pyx_f_4kola_5lexer_5Token_get_flag(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 
 
-/* "kola/lexer.pyx":148
+/* "kola/lexer.pyx":161
  * 
  * 
  * cdef class BaseLexer(object):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from stdin
  */
 
@@ -1376,29 +1376,29 @@
   void (*set_error)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *);
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*next_syn)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
   struct __pyx_obj_4kola_5lexer_Token *(*next_token)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtabptr_4kola_5lexer_BaseLexer;
 
 
-/* "kola/lexer.pyx":280
+/* "kola/lexer.pyx":296
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from file
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_FileLexer {
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer __pyx_base;
 };
 static struct __pyx_vtabstruct_4kola_5lexer_FileLexer *__pyx_vtabptr_4kola_5lexer_FileLexer;
 
 
-/* "kola/lexer.pyx":311
+/* "kola/lexer.pyx":327
  * 
  * 
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from string provided
  */
 
@@ -1645,61 +1645,28 @@
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
-
-/* decode_c_string_utf16.proto */
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 0;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = -1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16BE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-
-/* decode_c_bytes.proto */
-static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
-         const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
-         const char* encoding, const char* errors,
-         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
-
-/* decode_bytes.proto */
-static CYTHON_INLINE PyObject* __Pyx_decode_bytes(
-         PyObject* string, Py_ssize_t start, Py_ssize_t stop,
-         const char* encoding, const char* errors,
-         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
-    return __Pyx_decode_c_bytes(
-        PyBytes_AS_STRING(string), PyBytes_GET_SIZE(string),
-        start, stop, encoding, errors, decode_func);
-}
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
+/* set_iter.proto */
+static CYTHON_INLINE PyObject* __Pyx_set_iterator(PyObject* iterable, int is_set,
+                                                  Py_ssize_t* p_orig_length, int* p_source_is_set);
+static CYTHON_INLINE int __Pyx_set_iter_next(
+        PyObject* iter_obj, Py_ssize_t orig_length,
+        Py_ssize_t* ppos, PyObject **value,
+        int source_is_set);
+
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+
 /* PyObjectCallNoArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
@@ -1734,14 +1701,34 @@
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
+/* pyfrozenset_new.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it);
+
+/* PySetContains.proto */
+static CYTHON_INLINE int __Pyx_PySet_ContainsTF(PyObject* key, PyObject* set, int eq);
+
+/* decode_c_string_utf16.proto */
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = 0;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = -1;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16BE(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = 1;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
+
 /* decode_c_string.proto */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* PyDictVersioning.proto */
@@ -1792,14 +1779,17 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -2011,14 +2001,18 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
+/* unicode_tailmatch.proto */
+static int __Pyx_PyUnicode_Tailmatch(
+    PyObject* s, PyObject* substr, Py_ssize_t start, Py_ssize_t end, int direction);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2044,15 +2038,14 @@
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
-static PyObject* __pyx_convert__to_py_LexerData(LexerData s);
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__TokenSyn(enum TokenSyn value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
@@ -2314,43 +2307,45 @@
 #if !CYTHON_USE_MODULE_STATE
 static PyTypeObject *__pyx_ptype_4kola_5lexer_Token = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_LexerConfig = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_BaseLexer = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_FileLexer = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_StringLexer = 0;
 #endif
+static PyObject *__pyx_v_4kola_5lexer__lexer_data_names = 0;
+static PyObject *__pyx_7genexpr__pyx_v_4kola_5lexer_i;
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "kola.lexer"
 extern int __pyx_module_is_main_kola__lexer;
 int __pyx_module_is_main_kola__lexer = 0;
 
 /* Implementation of "kola.lexer" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_AttributeError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_OSError;
 static PyObject *__pyx_builtin_StopIteration;
 /* #### Code section: string_decls ### */
-static const char __pyx_k_[] = "__";
+static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_v[] = "v";
-static const char __pyx_k__3[] = ".";
+static const char __pyx_k__2[] = ".";
 static const char __pyx_k_gc[] = "gc";
+static const char __pyx_k__14[] = "__";
 static const char __pyx_k__26[] = "?";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_syn[] = "syn";
 static const char __pyx_k_val[] = "val";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "dict";
 static const char __pyx_k_exit[] = "__exit__";
-static const char __pyx_k_flag[] = "flag";
 static const char __pyx_k_kwds[] = "kwds";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_S_CLN[] = "S_CLN";
 static const char __pyx_k_S_CMA[] = "S_CMA";
@@ -2375,32 +2370,29 @@
 static const char __pyx_k_S_NUM_B[] = "S_NUM_B";
 static const char __pyx_k_S_NUM_F[] = "S_NUM_F";
 static const char __pyx_k_S_NUM_H[] = "S_NUM_H";
 static const char __pyx_k_content[] = "content";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_raw_val[] = "raw_val";
 static const char __pyx_k_S_STRING[] = "S_STRING";
-static const char __pyx_k_encoding[] = "encoding";
-static const char __pyx_k_endswith[] = "endswith";
-static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_get_flag[] = "get_flag";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_BaseLexer[] = "BaseLexer";
 static const char __pyx_k_FileLexer[] = "FileLexer";
 static const char __pyx_k_S_LITERAL[] = "S_LITERAL";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_exception[] = "exception";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_F_DISABLED[] = "F_DISABLED";
+static const char __pyx_k_data_names[] = "data_names";
 static const char __pyx_k_kola_lexer[] = "kola.lexer";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
-static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_LexerConfig[] = "LexerConfig";
 static const char __pyx_k_StringLexer[] = "StringLexer";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_S_ANNOTATION[] = "S_ANNOTATION";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_F_LSTRIP_TEXT[] = "F_LSTRIP_TEXT";
@@ -2413,15 +2405,14 @@
 static const char __pyx_k_FileLexer__path[] = "_FileLexer__path";
 static const char __pyx_k_FileLexer_close[] = "FileLexer.close";
 static const char __pyx_k_LexerConfig_set[] = "LexerConfig.set";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_BaseLexer___exit[] = "BaseLexer.__exit__";
 static const char __pyx_k_LexerConfig_dict[] = "LexerConfig.dict";
 static const char __pyx_k_BaseLexer___enter[] = "BaseLexer.__enter__";
-static const char __pyx_k_command_threshold[] = "command_threshold";
 static const char __pyx_k_KoiLangSyntaxError[] = "KoiLangSyntaxError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Token___reduce_cython[] = "Token.__reduce_cython__";
 static const char __pyx_k_Token___setstate_cython[] = "Token.__setstate_cython__";
 static const char __pyx_k_BaseLexer___reduce_cython[] = "BaseLexer.__reduce_cython__";
 static const char __pyx_k_FileLexer___reduce_cython[] = "FileLexer.__reduce_cython__";
@@ -2431,15 +2422,14 @@
 static const char __pyx_k_LexerConfig___reduce_cython[] = "LexerConfig.__reduce_cython__";
 static const char __pyx_k_StringLexer___reduce_cython[] = "StringLexer.__reduce_cython__";
 static const char __pyx_k_LexerConfig___setstate_cython[] = "LexerConfig.__setstate_cython__";
 static const char __pyx_k_StringLexer___setstate_cython[] = "StringLexer.__setstate_cython__";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_self_lexer_data_cannot_be_conver[] = "self.lexer_data cannot be converted to a Python object for pickling";
 #if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_n_u_;
 static PyObject *__pyx_n_s_AttributeError;
 static PyObject *__pyx_n_s_BaseLexer;
 static PyObject *__pyx_n_s_BaseLexer___enter;
 static PyObject *__pyx_n_s_BaseLexer___exit;
 static PyObject *__pyx_n_s_BaseLexer___reduce_cython;
 static PyObject *__pyx_n_s_BaseLexer___setstate_cython;
 static PyObject *__pyx_n_s_BaseLexer_close;
@@ -2478,37 +2468,34 @@
 static PyObject *__pyx_n_s_StringLexer___reduce_cython;
 static PyObject *__pyx_n_s_StringLexer___setstate_cython;
 static PyObject *__pyx_n_s_Token;
 static PyObject *__pyx_n_s_Token___reduce_cython;
 static PyObject *__pyx_n_s_Token___setstate_cython;
 static PyObject *__pyx_n_s_Token_get_flag;
 static PyObject *__pyx_n_s_TypeError;
+static PyObject *__pyx_n_u__14;
+static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s__26;
-static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_asyncio_coroutines;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
-static PyObject *__pyx_n_s_command_threshold;
 static PyObject *__pyx_n_s_content;
 static PyObject *__pyx_n_s_data;
+static PyObject *__pyx_n_u_data_names;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_kp_u_disable;
 static PyObject *__pyx_kp_u_enable;
-static PyObject *__pyx_n_u_encoding;
-static PyObject *__pyx_n_s_endswith;
 static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_exit;
-static PyObject *__pyx_n_s_filename;
-static PyObject *__pyx_n_u_filename;
-static PyObject *__pyx_n_s_flag;
 static PyObject *__pyx_kp_u_gc;
 static PyObject *__pyx_n_s_get_flag;
 static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_is_coroutine;
 static PyObject *__pyx_kp_u_isenabled;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_kola_lexer;
 static PyObject *__pyx_kp_s_kola_lexer_pyx;
@@ -2527,15 +2514,14 @@
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_kp_s_self_lexer_data_cannot_be_conver;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_startswith;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_syn;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_val;
 #endif
@@ -2597,27 +2583,27 @@
 static PyObject *__pyx_tp_new_4kola_5lexer_LexerConfig(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_BaseLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_FileLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_StringLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 #if !CYTHON_USE_MODULE_STATE
 #endif
 #if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__14;
 static PyObject *__pyx_codeobj__15;
 static PyObject *__pyx_codeobj__16;
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__19;
 static PyObject *__pyx_codeobj__20;
 static PyObject *__pyx_codeobj__21;
 static PyObject *__pyx_codeobj__22;
@@ -2650,15 +2636,14 @@
   PyObject *__pyx_type_4kola_5lexer_LexerConfig;
   PyTypeObject *__pyx_ptype_4kola_5lexer_BaseLexer;
   PyObject *__pyx_type_4kola_5lexer_BaseLexer;
   PyTypeObject *__pyx_ptype_4kola_5lexer_FileLexer;
   PyObject *__pyx_type_4kola_5lexer_FileLexer;
   PyTypeObject *__pyx_ptype_4kola_5lexer_StringLexer;
   PyObject *__pyx_type_4kola_5lexer_StringLexer;
-  PyObject *__pyx_n_u_;
   PyObject *__pyx_n_s_AttributeError;
   PyObject *__pyx_n_s_BaseLexer;
   PyObject *__pyx_n_s_BaseLexer___enter;
   PyObject *__pyx_n_s_BaseLexer___exit;
   PyObject *__pyx_n_s_BaseLexer___reduce_cython;
   PyObject *__pyx_n_s_BaseLexer___setstate_cython;
   PyObject *__pyx_n_s_BaseLexer_close;
@@ -2697,37 +2682,34 @@
   PyObject *__pyx_n_s_StringLexer___reduce_cython;
   PyObject *__pyx_n_s_StringLexer___setstate_cython;
   PyObject *__pyx_n_s_Token;
   PyObject *__pyx_n_s_Token___reduce_cython;
   PyObject *__pyx_n_s_Token___setstate_cython;
   PyObject *__pyx_n_s_Token_get_flag;
   PyObject *__pyx_n_s_TypeError;
+  PyObject *__pyx_n_u__14;
+  PyObject *__pyx_kp_u__2;
   PyObject *__pyx_n_s__26;
-  PyObject *__pyx_kp_u__3;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_close;
-  PyObject *__pyx_n_s_command_threshold;
   PyObject *__pyx_n_s_content;
   PyObject *__pyx_n_s_data;
+  PyObject *__pyx_n_u_data_names;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_kp_u_enable;
-  PyObject *__pyx_n_u_encoding;
-  PyObject *__pyx_n_s_endswith;
   PyObject *__pyx_n_s_enter;
   PyObject *__pyx_n_s_exception;
   PyObject *__pyx_n_s_exit;
-  PyObject *__pyx_n_s_filename;
-  PyObject *__pyx_n_u_filename;
-  PyObject *__pyx_n_s_flag;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get_flag;
   PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_items;
   PyObject *__pyx_n_s_k;
   PyObject *__pyx_n_s_kola_lexer;
   PyObject *__pyx_kp_s_kola_lexer_pyx;
@@ -2746,34 +2728,33 @@
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_s_self_lexer_data_cannot_be_conver;
   PyObject *__pyx_n_s_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
-  PyObject *__pyx_n_s_startswith;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_syn;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_v;
   PyObject *__pyx_n_s_val;
-  PyObject *__pyx_tuple__2;
-  PyObject *__pyx_tuple__4;
-  PyObject *__pyx_tuple__7;
-  PyObject *__pyx_tuple__9;
-  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__17;
+  PyObject *__pyx_codeobj__4;
   PyObject *__pyx_codeobj__5;
-  PyObject *__pyx_codeobj__6;
-  PyObject *__pyx_codeobj__8;
-  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__15;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__18;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__20;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__22;
@@ -2822,15 +2803,14 @@
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_LexerConfig);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_FileLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_FileLexer);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_StringLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_StringLexer);
-  Py_CLEAR(clear_module_state->__pyx_n_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AttributeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___enter);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___exit);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer_close);
@@ -2869,37 +2849,34 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_StringLexer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_StringLexer___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token_get_flag);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
+  Py_CLEAR(clear_module_state->__pyx_n_u__14);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_n_s__26);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_close);
-  Py_CLEAR(clear_module_state->__pyx_n_s_command_threshold);
   Py_CLEAR(clear_module_state->__pyx_n_s_content);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
+  Py_CLEAR(clear_module_state->__pyx_n_u_data_names);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
-  Py_CLEAR(clear_module_state->__pyx_n_u_encoding);
-  Py_CLEAR(clear_module_state->__pyx_n_s_endswith);
   Py_CLEAR(clear_module_state->__pyx_n_s_enter);
   Py_CLEAR(clear_module_state->__pyx_n_s_exception);
   Py_CLEAR(clear_module_state->__pyx_n_s_exit);
-  Py_CLEAR(clear_module_state->__pyx_n_s_filename);
-  Py_CLEAR(clear_module_state->__pyx_n_u_filename);
-  Py_CLEAR(clear_module_state->__pyx_n_s_flag);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_flag);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_items);
   Py_CLEAR(clear_module_state->__pyx_n_s_k);
   Py_CLEAR(clear_module_state->__pyx_n_s_kola_lexer);
   Py_CLEAR(clear_module_state->__pyx_kp_s_kola_lexer_pyx);
@@ -2918,34 +2895,33 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_s_self_lexer_data_cannot_be_conver);
   Py_CLEAR(clear_module_state->__pyx_n_s_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_startswith);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_syn);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_v);
   Py_CLEAR(clear_module_state->__pyx_n_s_val);
-  Py_CLEAR(clear_module_state->__pyx_tuple__2);
-  Py_CLEAR(clear_module_state->__pyx_tuple__4);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
-  Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
@@ -2981,15 +2957,14 @@
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_LexerConfig);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_FileLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_FileLexer);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_StringLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_StringLexer);
-  Py_VISIT(traverse_module_state->__pyx_n_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AttributeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___enter);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___exit);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer_close);
@@ -3028,37 +3003,34 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_StringLexer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_StringLexer___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token_get_flag);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
+  Py_VISIT(traverse_module_state->__pyx_n_u__14);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_n_s__26);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_close);
-  Py_VISIT(traverse_module_state->__pyx_n_s_command_threshold);
   Py_VISIT(traverse_module_state->__pyx_n_s_content);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
+  Py_VISIT(traverse_module_state->__pyx_n_u_data_names);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
-  Py_VISIT(traverse_module_state->__pyx_n_u_encoding);
-  Py_VISIT(traverse_module_state->__pyx_n_s_endswith);
   Py_VISIT(traverse_module_state->__pyx_n_s_enter);
   Py_VISIT(traverse_module_state->__pyx_n_s_exception);
   Py_VISIT(traverse_module_state->__pyx_n_s_exit);
-  Py_VISIT(traverse_module_state->__pyx_n_s_filename);
-  Py_VISIT(traverse_module_state->__pyx_n_u_filename);
-  Py_VISIT(traverse_module_state->__pyx_n_s_flag);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_flag);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_items);
   Py_VISIT(traverse_module_state->__pyx_n_s_k);
   Py_VISIT(traverse_module_state->__pyx_n_s_kola_lexer);
   Py_VISIT(traverse_module_state->__pyx_kp_s_kola_lexer_pyx);
@@ -3077,34 +3049,33 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_s_self_lexer_data_cannot_be_conver);
   Py_VISIT(traverse_module_state->__pyx_n_s_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_startswith);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_syn);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_v);
   Py_VISIT(traverse_module_state->__pyx_n_s_val);
-  Py_VISIT(traverse_module_state->__pyx_tuple__2);
-  Py_VISIT(traverse_module_state->__pyx_tuple__4);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
-  Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
@@ -3137,15 +3108,14 @@
 #define __pyx_type_4kola_5lexer_LexerConfig __pyx_mstate_global->__pyx_type_4kola_5lexer_LexerConfig
 #define __pyx_ptype_4kola_5lexer_BaseLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_BaseLexer
 #define __pyx_type_4kola_5lexer_BaseLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_BaseLexer
 #define __pyx_ptype_4kola_5lexer_FileLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_FileLexer
 #define __pyx_type_4kola_5lexer_FileLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_FileLexer
 #define __pyx_ptype_4kola_5lexer_StringLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_StringLexer
 #define __pyx_type_4kola_5lexer_StringLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_StringLexer
-#define __pyx_n_u_ __pyx_mstate_global->__pyx_n_u_
 #define __pyx_n_s_AttributeError __pyx_mstate_global->__pyx_n_s_AttributeError
 #define __pyx_n_s_BaseLexer __pyx_mstate_global->__pyx_n_s_BaseLexer
 #define __pyx_n_s_BaseLexer___enter __pyx_mstate_global->__pyx_n_s_BaseLexer___enter
 #define __pyx_n_s_BaseLexer___exit __pyx_mstate_global->__pyx_n_s_BaseLexer___exit
 #define __pyx_n_s_BaseLexer___reduce_cython __pyx_mstate_global->__pyx_n_s_BaseLexer___reduce_cython
 #define __pyx_n_s_BaseLexer___setstate_cython __pyx_mstate_global->__pyx_n_s_BaseLexer___setstate_cython
 #define __pyx_n_s_BaseLexer_close __pyx_mstate_global->__pyx_n_s_BaseLexer_close
@@ -3184,37 +3154,34 @@
 #define __pyx_n_s_StringLexer___reduce_cython __pyx_mstate_global->__pyx_n_s_StringLexer___reduce_cython
 #define __pyx_n_s_StringLexer___setstate_cython __pyx_mstate_global->__pyx_n_s_StringLexer___setstate_cython
 #define __pyx_n_s_Token __pyx_mstate_global->__pyx_n_s_Token
 #define __pyx_n_s_Token___reduce_cython __pyx_mstate_global->__pyx_n_s_Token___reduce_cython
 #define __pyx_n_s_Token___setstate_cython __pyx_mstate_global->__pyx_n_s_Token___setstate_cython
 #define __pyx_n_s_Token_get_flag __pyx_mstate_global->__pyx_n_s_Token_get_flag
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
+#define __pyx_n_u__14 __pyx_mstate_global->__pyx_n_u__14
+#define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_n_s__26 __pyx_mstate_global->__pyx_n_s__26
-#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
-#define __pyx_n_s_command_threshold __pyx_mstate_global->__pyx_n_s_command_threshold
 #define __pyx_n_s_content __pyx_mstate_global->__pyx_n_s_content
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
+#define __pyx_n_u_data_names __pyx_mstate_global->__pyx_n_u_data_names
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
-#define __pyx_n_u_encoding __pyx_mstate_global->__pyx_n_u_encoding
-#define __pyx_n_s_endswith __pyx_mstate_global->__pyx_n_s_endswith
 #define __pyx_n_s_enter __pyx_mstate_global->__pyx_n_s_enter
 #define __pyx_n_s_exception __pyx_mstate_global->__pyx_n_s_exception
 #define __pyx_n_s_exit __pyx_mstate_global->__pyx_n_s_exit
-#define __pyx_n_s_filename __pyx_mstate_global->__pyx_n_s_filename
-#define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
-#define __pyx_n_s_flag __pyx_mstate_global->__pyx_n_s_flag
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get_flag __pyx_mstate_global->__pyx_n_s_get_flag
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
 #define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
 #define __pyx_n_s_kola_lexer __pyx_mstate_global->__pyx_n_s_kola_lexer
 #define __pyx_kp_s_kola_lexer_pyx __pyx_mstate_global->__pyx_kp_s_kola_lexer_pyx
@@ -3233,48 +3200,47 @@
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_s_self_lexer_data_cannot_be_conver __pyx_mstate_global->__pyx_kp_s_self_lexer_data_cannot_be_conver
 #define __pyx_n_s_set __pyx_mstate_global->__pyx_n_s_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
-#define __pyx_n_s_startswith __pyx_mstate_global->__pyx_n_s_startswith
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_syn __pyx_mstate_global->__pyx_n_s_syn
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
 #define __pyx_n_s_val __pyx_mstate_global->__pyx_n_s_val
-#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
-#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
-#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
-#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
-#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #endif
 /* #### Code section: module_code ### */
 
-/* "kola/lexer.pyx":42
+/* "kola/lexer.pyx":45
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3297,24 +3263,24 @@
     #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_syn,&__pyx_n_s_val,&__pyx_n_s_lineno,&__pyx_n_s_raw_val,0};
     #else
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_syn,&__pyx_n_s_val,&__pyx_n_s_lineno,&__pyx_n_s_raw_val,0};
     #endif
     PyObject* values[4] = {0,0,0,0};
 
-    /* "kola/lexer.pyx":45
+    /* "kola/lexer.pyx":48
  *         self,
  *         TokenSyn syn,
  *         val = None,             # <<<<<<<<<<<<<<
  *         *,
  *         int lineno = 0,
  */
     values[1] = ((PyObject *)Py_None);
 
-    /* "kola/lexer.pyx":48
+    /* "kola/lexer.pyx":51
  *         *,
  *         int lineno = 0,
  *         bytes raw_val = None             # <<<<<<<<<<<<<<
  *     ):
  *         self.syn = syn
  */
     values[3] = ((PyObject*)Py_None);
@@ -3328,66 +3294,66 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_syn)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_val);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 2)) {
         Py_ssize_t index;
         for (index = 2; index < 4 && kw_args > 0; index++) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 42, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 45, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_syn = ((enum TokenSyn)__Pyx_PyInt_As_enum__TokenSyn(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 44, __pyx_L3_error)
+    __pyx_v_syn = ((enum TokenSyn)__Pyx_PyInt_As_enum__TokenSyn(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 47, __pyx_L3_error)
     __pyx_v_val = values[1];
     if (values[2]) {
-      __pyx_v_lineno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 47, __pyx_L3_error)
+      __pyx_v_lineno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 50, __pyx_L3_error)
     } else {
       __pyx_v_lineno = ((int)0);
     }
     __pyx_v_raw_val = ((PyObject*)values[3]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 42, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 45, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.Token.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_val), (&PyBytes_Type), 1, "raw_val", 1))) __PYX_ERR(1, 48, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_val), (&PyBytes_Type), 1, "raw_val", 1))) __PYX_ERR(1, 51, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_5Token___cinit__(((struct __pyx_obj_4kola_5lexer_Token *)__pyx_v_self), __pyx_v_syn, __pyx_v_val, __pyx_v_lineno, __pyx_v_raw_val);
 
-  /* "kola/lexer.pyx":42
+  /* "kola/lexer.pyx":45
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3407,69 +3373,69 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "kola/lexer.pyx":50
+  /* "kola/lexer.pyx":53
  *         bytes raw_val = None
  *     ):
  *         self.syn = syn             # <<<<<<<<<<<<<<
  *         self.val = val
  * 
  */
   __pyx_v_self->syn = __pyx_v_syn;
 
-  /* "kola/lexer.pyx":51
+  /* "kola/lexer.pyx":54
  *     ):
  *         self.syn = syn
  *         self.val = val             # <<<<<<<<<<<<<<
  * 
  *         self.lineno = lineno
  */
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   __Pyx_GOTREF(__pyx_v_self->val);
   __Pyx_DECREF(__pyx_v_self->val);
   __pyx_v_self->val = __pyx_v_val;
 
-  /* "kola/lexer.pyx":53
+  /* "kola/lexer.pyx":56
  *         self.val = val
  * 
  *         self.lineno = lineno             # <<<<<<<<<<<<<<
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  */
   __pyx_v_self->lineno = __pyx_v_lineno;
 
-  /* "kola/lexer.pyx":54
+  /* "kola/lexer.pyx":57
  * 
  *         self.lineno = lineno
  *         self.raw_val = bytes(val) if raw_val is None else raw_val             # <<<<<<<<<<<<<<
  * 
  *     def __eq__(self, other) -> bool:
  */
   __pyx_t_2 = (__pyx_v_raw_val == ((PyObject*)Py_None));
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 54, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_raw_val);
     __pyx_t_1 = __pyx_v_raw_val;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->raw_val);
   __Pyx_DECREF(__pyx_v_self->raw_val);
   __pyx_v_self->raw_val = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":42
+  /* "kola/lexer.pyx":45
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3482,15 +3448,15 @@
   __Pyx_AddTraceback("kola.lexer.Token.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":56
+/* "kola/lexer.pyx":59
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  *     def __eq__(self, other) -> bool:             # <<<<<<<<<<<<<<
  *         return self is other or self.syn == other
  * 
  */
 
@@ -3516,44 +3482,44 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
 
-  /* "kola/lexer.pyx":57
+  /* "kola/lexer.pyx":60
  * 
  *     def __eq__(self, other) -> bool:
  *         return self is other or self.syn == other             # <<<<<<<<<<<<<<
  * 
  *     cpdef int get_flag(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = (((PyObject *)__pyx_v_self) == __pyx_v_other);
   if (!__pyx_t_2) {
   } else {
-    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 57, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_1 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":56
+  /* "kola/lexer.pyx":59
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  *     def __eq__(self, other) -> bool:             # <<<<<<<<<<<<<<
  *         return self is other or self.syn == other
  * 
  */
 
@@ -3566,15 +3532,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":59
+/* "kola/lexer.pyx":62
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
 
@@ -3588,15 +3554,15 @@
 static int __pyx_f_4kola_5lexer_5Token_get_flag(struct __pyx_obj_4kola_5lexer_Token *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("get_flag", 0);
 
-  /* "kola/lexer.pyx":60
+  /* "kola/lexer.pyx":63
  * 
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             return 0
  *         elif self.syn == LITERAL:
  */
   __pyx_t_2 = ((__pyx_v_self->syn <= TEXT) != 0);
@@ -3606,104 +3572,104 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_self->syn == ANNOTATION) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":61
+    /* "kola/lexer.pyx":64
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0             # <<<<<<<<<<<<<<
  *         elif self.syn == LITERAL:
  *             return 1
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":60
+    /* "kola/lexer.pyx":63
  * 
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             return 0
  *         elif self.syn == LITERAL:
  */
   }
 
-  /* "kola/lexer.pyx":62
+  /* "kola/lexer.pyx":65
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  *         elif self.syn == LITERAL:             # <<<<<<<<<<<<<<
  *             return 1
  *         elif self.syn <= NUM_F:
  */
   __pyx_t_1 = ((__pyx_v_self->syn == LITERAL) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":63
+    /* "kola/lexer.pyx":66
  *             return 0
  *         elif self.syn == LITERAL:
  *             return 1             # <<<<<<<<<<<<<<
  *         elif self.syn <= NUM_F:
  *             return 2
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":62
+    /* "kola/lexer.pyx":65
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  *         elif self.syn == LITERAL:             # <<<<<<<<<<<<<<
  *             return 1
  *         elif self.syn <= NUM_F:
  */
   }
 
-  /* "kola/lexer.pyx":64
+  /* "kola/lexer.pyx":67
  *         elif self.syn == LITERAL:
  *             return 1
  *         elif self.syn <= NUM_F:             # <<<<<<<<<<<<<<
  *             return 2
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->syn <= NUM_F) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":65
+    /* "kola/lexer.pyx":68
  *             return 1
  *         elif self.syn <= NUM_F:
  *             return 2             # <<<<<<<<<<<<<<
  *         else:
  *             return self.syn - CLN + 3
  */
     __pyx_r = 2;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":64
+    /* "kola/lexer.pyx":67
  *         elif self.syn == LITERAL:
  *             return 1
  *         elif self.syn <= NUM_F:             # <<<<<<<<<<<<<<
  *             return 2
  *         else:
  */
   }
 
-  /* "kola/lexer.pyx":67
+  /* "kola/lexer.pyx":70
  *             return 2
  *         else:
  *             return self.syn - CLN + 3             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   /*else*/ {
     __pyx_r = ((__pyx_v_self->syn - CLN) + 3);
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":59
+  /* "kola/lexer.pyx":62
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
 
@@ -3751,15 +3717,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_flag", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4kola_5lexer_5Token_get_flag(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4kola_5lexer_5Token_get_flag(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3768,15 +3734,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":69
+/* "kola/lexer.pyx":72
  *             return self.syn - CLN + 3
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  */
 
@@ -3801,65 +3767,65 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "kola/lexer.pyx":70
+  /* "kola/lexer.pyx":73
  * 
  *     def __repr__(self):
  *         if self.val is None:             # <<<<<<<<<<<<<<
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->val == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "kola/lexer.pyx":71
+    /* "kola/lexer.pyx":74
  *     def __repr__(self):
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)             # <<<<<<<<<<<<<<
  *         else:
  *             return PyUnicode_FromFormat("<token %d: %R>", self.syn, <void*>self.val)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d>"), __pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 71, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d>"), __pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":70
+    /* "kola/lexer.pyx":73
  * 
  *     def __repr__(self):
  *         if self.val is None:             # <<<<<<<<<<<<<<
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  */
   }
 
-  /* "kola/lexer.pyx":73
+  /* "kola/lexer.pyx":76
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  *             return PyUnicode_FromFormat("<token %d: %R>", self.syn, <void*>self.val)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d: %R>"), __pyx_v_self->syn, ((void *)__pyx_v_self->val)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 73, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d: %R>"), __pyx_v_self->syn, ((void *)__pyx_v_self->val)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":69
+  /* "kola/lexer.pyx":72
  *             return self.syn - CLN + 3
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  */
 
@@ -3870,15 +3836,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":12
+/* "kola/lexer.pxd":16
  *         Token next     # used in grammar parser
  *     cdef readonly:
  *         TokenSyn syn             # <<<<<<<<<<<<<<
  *         object val
  *         bytes raw_val
  */
 
@@ -3901,15 +3867,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3918,15 +3884,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":13
+/* "kola/lexer.pxd":17
  *     cdef readonly:
  *         TokenSyn syn
  *         object val             # <<<<<<<<<<<<<<
  *         bytes raw_val
  *         int lineno
  */
 
@@ -3956,15 +3922,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":14
+/* "kola/lexer.pxd":18
  *         TokenSyn syn
  *         object val
  *         bytes raw_val             # <<<<<<<<<<<<<<
  *         int lineno
  * 
  */
 
@@ -3994,15 +3960,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":15
+/* "kola/lexer.pxd":19
  *         object val
  *         bytes raw_val
  *         int lineno             # <<<<<<<<<<<<<<
  * 
  *     cpdef int get_flag(self)
  */
 
@@ -4025,15 +3991,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4227,15 +4193,15 @@
   __Pyx_AddTraceback("kola.lexer.Token.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":81
+/* "kola/lexer.pyx":84
  *     """
  * 
  *     def __init__(self, BaseLexer lexer not None):             # <<<<<<<<<<<<<<
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data
  */
 
@@ -4266,37 +4232,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_lexer)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 81, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 84, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 81, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 84, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_lexer = ((struct __pyx_obj_4kola_5lexer_BaseLexer *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 81, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 84, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lexer), __pyx_ptype_4kola_5lexer_BaseLexer, 0, "lexer", 0))) __PYX_ERR(1, 81, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lexer), __pyx_ptype_4kola_5lexer_BaseLexer, 0, "lexer", 0))) __PYX_ERR(1, 84, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_11LexerConfig___init__(((struct __pyx_obj_4kola_5lexer_LexerConfig *)__pyx_v_self), __pyx_v_lexer);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -4305,56 +4271,56 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig___init__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_lexer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":82
+  /* "kola/lexer.pyx":85
  * 
  *     def __init__(self, BaseLexer lexer not None):
  *         self.lexer = lexer             # <<<<<<<<<<<<<<
  *         self.lexer_data = &lexer.lexer_data
  * 
  */
   __Pyx_INCREF((PyObject *)__pyx_v_lexer);
   __Pyx_GIVEREF((PyObject *)__pyx_v_lexer);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->lexer);
   __Pyx_DECREF((PyObject *)__pyx_v_self->lexer);
   __pyx_v_self->lexer = __pyx_v_lexer;
 
-  /* "kola/lexer.pyx":83
+  /* "kola/lexer.pyx":86
  *     def __init__(self, BaseLexer lexer not None):
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data             # <<<<<<<<<<<<<<
  * 
  *     def dict(self) -> dict:
  */
   __pyx_v_self->lexer_data = (&__pyx_v_lexer->lexer_data);
 
-  /* "kola/lexer.pyx":81
+  /* "kola/lexer.pyx":84
  *     """
  * 
  *     def __init__(self, BaseLexer lexer not None):             # <<<<<<<<<<<<<<
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":85
+/* "kola/lexer.pyx":88
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11LexerConfig_3dict(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4384,121 +4350,115 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_2dict(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_v_data = 0;
+  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dict", 0);
 
-  /* "kola/lexer.pyx":86
+  /* "kola/lexer.pyx":89
  * 
  *     def dict(self) -> dict:
- *         cdef dict data = <dict>self.lexer_data[0]             # <<<<<<<<<<<<<<
- *         data["filename"] = (<bytes>data["filename"]).decode()
- *         data["encoding"] = self.lexer.encoding
+ *         cdef dict data = {}             # <<<<<<<<<<<<<<
+ *         for i in _lexer_data_names:
+ *             data[i] = getattr(self, <str>i)
  */
-  __pyx_t_1 = __pyx_convert__to_py_LexerData((__pyx_v_self->lexer_data[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyDict_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_1))) __PYX_ERR(1, 86, __pyx_L1_error)
-  __pyx_t_2 = __pyx_t_1;
-  __Pyx_INCREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_data = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_v_data = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":87
+  /* "kola/lexer.pyx":90
  *     def dict(self) -> dict:
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()             # <<<<<<<<<<<<<<
- *         data["encoding"] = self.lexer.encoding
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:             # <<<<<<<<<<<<<<
+ *             data[i] = getattr(self, <str>i)
  *         return data
  */
-  if (unlikely(__pyx_v_data == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 87, __pyx_L1_error)
-  }
-  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_data, __pyx_n_u_filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(__pyx_t_2 == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-    __PYX_ERR(1, 87, __pyx_L1_error)
-  }
-  __pyx_t_1 = __Pyx_decode_bytes(((PyObject*)__pyx_t_2), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(__pyx_v_data == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 87, __pyx_L1_error)
-  }
-  if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_n_u_filename, __pyx_t_1) < 0))) __PYX_ERR(1, 87, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_5 = __Pyx_set_iterator(__pyx_v_4kola_5lexer__lexer_data_names, 1, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_1);
+  __pyx_t_1 = __pyx_t_5;
+  __pyx_t_5 = 0;
+  while (1) {
+    __pyx_t_6 = __Pyx_set_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, __pyx_t_4);
+    if (unlikely(__pyx_t_6 == 0)) break;
+    if (unlikely(__pyx_t_6 == -1)) __PYX_ERR(1, 90, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
+    __pyx_t_5 = 0;
 
-  /* "kola/lexer.pyx":88
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()
- *         data["encoding"] = self.lexer.encoding             # <<<<<<<<<<<<<<
+    /* "kola/lexer.pyx":91
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:
+ *             data[i] = getattr(self, <str>i)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __pyx_t_1 = __pyx_v_self->lexer->encoding;
-  __Pyx_INCREF(__pyx_t_1);
-  if (unlikely(__pyx_v_data == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 88, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetAttr(((PyObject *)__pyx_v_self), __pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 91, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_v_i, __pyx_t_5) < 0))) __PYX_ERR(1, 91, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_n_u_encoding, __pyx_t_1) < 0))) __PYX_ERR(1, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":89
- *         data["filename"] = (<bytes>data["filename"]).decode()
- *         data["encoding"] = self.lexer.encoding
+  /* "kola/lexer.pyx":92
+ *         for i in _lexer_data_names:
+ *             data[i] = getattr(self, <str>i)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def set(self, **kwds) -> None:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":85
+  /* "kola/lexer.pyx":88
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("kola.lexer.LexerConfig.dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
+  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":91
+/* "kola/lexer.pyx":94
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11LexerConfig_5set(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4550,167 +4510,116 @@
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
-  PyObject *__pyx_t_11;
-  int __pyx_t_12;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10;
+  int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
 
-  /* "kola/lexer.pyx":92
+  /* "kola/lexer.pyx":95
  * 
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():             # <<<<<<<<<<<<<<
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  */
   __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_kwds, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 92, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_kwds, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_7 == 0)) break;
-    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(1, 92, __pyx_L1_error)
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(1, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "kola/lexer.pyx":93
+    /* "kola/lexer.pyx":96
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):             # <<<<<<<<<<<<<<
+ *             if not k in _lexer_data_names:             # <<<<<<<<<<<<<<
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_startswith); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = NULL;
-    __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_9);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_7 = 1;
-      }
-    }
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_n_u_};
-      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 93, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    }
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 93, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (__pyx_t_10) {
-    } else {
-      __pyx_t_8 = __pyx_t_10;
-      goto __pyx_L6_bool_binop_done;
-    }
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_endswith); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = NULL;
-    __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_9);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_7 = 1;
-      }
-    }
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_n_u_};
-      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 93, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    }
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 93, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_8 = __pyx_t_10;
-    __pyx_L6_bool_binop_done:;
-    if (__pyx_t_8) {
+    if (unlikely(__pyx_v_4kola_5lexer__lexer_data_names == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+      __PYX_ERR(1, 96, __pyx_L1_error)
+    }
+    __pyx_t_8 = (__Pyx_PySet_ContainsTF(__pyx_v_k, __pyx_v_4kola_5lexer__lexer_data_names, Py_NE)); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(1, 96, __pyx_L1_error)
+    __pyx_t_9 = (__pyx_t_8 != 0);
+    if (__pyx_t_9) {
 
-      /* "kola/lexer.pyx":94
+      /* "kola/lexer.pyx":97
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)             # <<<<<<<<<<<<<<
  *             setattr(self, k, v)
  * 
  */
-      __pyx_t_11 = PyErr_Format(__pyx_builtin_AttributeError, ((char *)"invalid config item '%U'"), ((void *)__pyx_v_k)); if (unlikely(__pyx_t_11 == ((PyObject *)NULL))) __PYX_ERR(1, 94, __pyx_L1_error)
+      __pyx_t_10 = PyErr_Format(__pyx_builtin_AttributeError, ((char *)"invalid config item '%U'"), ((void *)__pyx_v_k)); if (unlikely(__pyx_t_10 == ((PyObject *)NULL))) __PYX_ERR(1, 97, __pyx_L1_error)
 
-      /* "kola/lexer.pyx":93
+      /* "kola/lexer.pyx":96
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):             # <<<<<<<<<<<<<<
+ *             if not k in _lexer_data_names:             # <<<<<<<<<<<<<<
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)
  */
     }
 
-    /* "kola/lexer.pyx":95
- *             if k.startswith('__') and k.endswith('__'):
+    /* "kola/lexer.pyx":98
+ *             if not k in _lexer_data_names:
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-    __pyx_t_12 = PyObject_SetAttr(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(1, 95, __pyx_L1_error)
+    __pyx_t_11 = PyObject_SetAttr(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 98, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":91
+  /* "kola/lexer.pyx":94
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("kola.lexer.LexerConfig.set", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":97
+/* "kola/lexer.pyx":100
  *             setattr(self, k, v)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()
  */
 
@@ -4734,31 +4643,31 @@
   char const *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":99
+  /* "kola/lexer.pyx":102
  *     @property
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->lexer_data->filename;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 99, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":97
+  /* "kola/lexer.pyx":100
  *             setattr(self, k, v)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()
  */
 
@@ -4769,15 +4678,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":101
+/* "kola/lexer.pyx":104
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def encoding(self) -> str:
  *         return self.lexer.encoding
  */
 
@@ -4796,42 +4705,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_8encoding___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":103
+  /* "kola/lexer.pyx":106
  *     @property
  *     def encoding(self) -> str:
  *         return self.lexer.encoding             # <<<<<<<<<<<<<<
  * 
  *     @encoding.setter
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->lexer->encoding);
   __pyx_r = __pyx_v_self->lexer->encoding;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":101
+  /* "kola/lexer.pyx":104
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def encoding(self) -> str:
  *         return self.lexer.encoding
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":105
+/* "kola/lexer.pyx":108
  *         return self.lexer.encoding
  * 
  *     @encoding.setter             # <<<<<<<<<<<<<<
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val
  */
 
@@ -4841,15 +4750,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val), (&PyUnicode_Type), 1, "val", 1))) __PYX_ERR(1, 106, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val), (&PyUnicode_Type), 1, "val", 1))) __PYX_ERR(1, 109, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_11LexerConfig_8encoding_2__set__(((struct __pyx_obj_4kola_5lexer_LexerConfig *)__pyx_v_self), ((PyObject*)__pyx_v_val));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -4858,42 +4767,42 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_8encoding_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, PyObject *__pyx_v_val) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":107
+  /* "kola/lexer.pyx":110
  *     @encoding.setter
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   __Pyx_GOTREF(__pyx_v_self->lexer->encoding);
   __Pyx_DECREF(__pyx_v_self->lexer->encoding);
   __pyx_v_self->lexer->encoding = __pyx_v_val;
 
-  /* "kola/lexer.pyx":105
+  /* "kola/lexer.pyx":108
  *         return self.lexer.encoding
  * 
  *     @encoding.setter             # <<<<<<<<<<<<<<
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":109
+/* "kola/lexer.pyx":112
  *         self.lexer.encoding = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold
  */
 
@@ -4916,29 +4825,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":111
+  /* "kola/lexer.pyx":114
  *     @property
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold             # <<<<<<<<<<<<<<
  * 
  *     @command_threshold.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->command_threshold); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 111, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->command_threshold); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":109
+  /* "kola/lexer.pyx":112
  *         self.lexer.encoding = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold
  */
 
@@ -4949,15 +4858,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":113
+/* "kola/lexer.pyx":116
  *         return self.lexer_data.command_threshold
  * 
  *     @command_threshold.setter             # <<<<<<<<<<<<<<
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold
  */
 
@@ -4969,15 +4878,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_cmd_threshold); {
-    __pyx_v_cmd_threshold = __Pyx_PyInt_As_uint8_t(__pyx_arg_cmd_threshold); if (unlikely((__pyx_v_cmd_threshold == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 114, __pyx_L3_error)
+    __pyx_v_cmd_threshold = __Pyx_PyInt_As_uint8_t(__pyx_arg_cmd_threshold); if (unlikely((__pyx_v_cmd_threshold == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 117, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.command_threshold.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -4989,38 +4898,38 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_17command_threshold_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, uint8_t __pyx_v_cmd_threshold) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":115
+  /* "kola/lexer.pyx":118
  *     @command_threshold.setter
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->lexer_data->command_threshold = __pyx_v_cmd_threshold;
 
-  /* "kola/lexer.pyx":113
+  /* "kola/lexer.pyx":116
  *         return self.lexer_data.command_threshold
  * 
  *     @command_threshold.setter             # <<<<<<<<<<<<<<
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":117
+/* "kola/lexer.pyx":120
  *         self.lexer_data.command_threshold = cmd_threshold
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flag(self) -> int:
  *         return self.lexer_data.flag
  */
 
@@ -5043,29 +4952,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":119
+  /* "kola/lexer.pyx":122
  *     @property
  *     def flag(self) -> int:
  *         return self.lexer_data.flag             # <<<<<<<<<<<<<<
  * 
  *     @flag.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 119, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":117
+  /* "kola/lexer.pyx":120
  *         self.lexer_data.command_threshold = cmd_threshold
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flag(self) -> int:
  *         return self.lexer_data.flag
  */
 
@@ -5076,15 +4985,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":121
+/* "kola/lexer.pyx":124
  *         return self.lexer_data.flag
  * 
  *     @flag.setter             # <<<<<<<<<<<<<<
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val
  */
 
@@ -5096,15 +5005,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_val); {
-    __pyx_v_val = __Pyx_PyInt_As_uint8_t(__pyx_arg_val); if (unlikely((__pyx_v_val == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 122, __pyx_L3_error)
+    __pyx_v_val = __Pyx_PyInt_As_uint8_t(__pyx_arg_val); if (unlikely((__pyx_v_val == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 125, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.flag.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -5116,38 +5025,38 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_4flag_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, uint8_t __pyx_v_val) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":123
+  /* "kola/lexer.pyx":126
  *     @flag.setter
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->lexer_data->flag = __pyx_v_val;
 
-  /* "kola/lexer.pyx":121
+  /* "kola/lexer.pyx":124
  *         return self.lexer_data.flag
  * 
  *     @flag.setter             # <<<<<<<<<<<<<<
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":125
+/* "kola/lexer.pyx":128
  *         self.lexer_data.flag = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  */
 
@@ -5167,15 +5076,15 @@
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_8disabled___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":127
+  /* "kola/lexer.pyx":130
  *     @property
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False             # <<<<<<<<<<<<<<
  * 
  *     @disabled.setter
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5186,30 +5095,30 @@
     __Pyx_INCREF(Py_False);
     __pyx_t_1 = Py_False;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":125
+  /* "kola/lexer.pyx":128
  *         self.lexer_data.flag = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":129
+/* "kola/lexer.pyx":132
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  * 
  *     @disabled.setter             # <<<<<<<<<<<<<<
  *     def disabled(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5232,56 +5141,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":131
+  /* "kola/lexer.pyx":134
  *     @disabled.setter
  *     def disabled(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 131, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 134, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":132
+    /* "kola/lexer.pyx":135
  *     def disabled(self, val: bool) -> None:
  *         if val:
  *             self.lexer_data.flag |= LFLAG_DISABLED             # <<<<<<<<<<<<<<
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  */
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag | LFLAG_DISABLED);
 
-    /* "kola/lexer.pyx":131
+    /* "kola/lexer.pyx":134
  *     @disabled.setter
  *     def disabled(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kola/lexer.pyx":134
+  /* "kola/lexer.pyx":137
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_DISABLED             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag & (~LFLAG_DISABLED));
   }
   __pyx_L3:;
 
-  /* "kola/lexer.pyx":129
+  /* "kola/lexer.pyx":132
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  * 
  *     @disabled.setter             # <<<<<<<<<<<<<<
  *     def disabled(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5292,15 +5201,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.disabled.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":136
+/* "kola/lexer.pyx":139
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  */
 
@@ -5320,15 +5229,15 @@
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_9no_lstrip___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":138
+  /* "kola/lexer.pyx":141
  *     @property
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False             # <<<<<<<<<<<<<<
  * 
  *     @no_lstrip.setter
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5339,30 +5248,30 @@
     __Pyx_INCREF(Py_False);
     __pyx_t_1 = Py_False;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":136
+  /* "kola/lexer.pyx":139
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":140
+/* "kola/lexer.pyx":143
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  * 
  *     @no_lstrip.setter             # <<<<<<<<<<<<<<
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5385,56 +5294,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":142
+  /* "kola/lexer.pyx":145
  *     @no_lstrip.setter
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 142, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 145, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":143
+    /* "kola/lexer.pyx":146
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_NOLSTRIP
  */
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag | LFLAG_NOLSTRIP);
 
-    /* "kola/lexer.pyx":142
+    /* "kola/lexer.pyx":145
  *     @no_lstrip.setter
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kola/lexer.pyx":145
+  /* "kola/lexer.pyx":148
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag & (~LFLAG_NOLSTRIP));
   }
   __pyx_L3:;
 
-  /* "kola/lexer.pyx":140
+  /* "kola/lexer.pyx":143
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  * 
  *     @no_lstrip.setter             # <<<<<<<<<<<<<<
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5445,15 +5354,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.no_lstrip.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":22
+/* "kola/lexer.pxd":26
  * cdef class LexerConfig:
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -5668,15 +5577,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":153
+/* "kola/lexer.pyx":166
  *     """
  * 
  *     def __cinit__(self, *args, **kwds):             # <<<<<<<<<<<<<<
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  */
 
@@ -5708,74 +5617,74 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "kola/lexer.pyx":154
+  /* "kola/lexer.pyx":167
  * 
  *     def __cinit__(self, *args, **kwds):
  *         self.encoding = "utf-8"             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  */
   __Pyx_INCREF(__pyx_kp_u_utf_8);
   __Pyx_GIVEREF(__pyx_kp_u_utf_8);
   __Pyx_GOTREF(__pyx_v_self->encoding);
   __Pyx_DECREF(__pyx_v_self->encoding);
   __pyx_v_self->encoding = __pyx_kp_u_utf_8;
 
-  /* "kola/lexer.pyx":155
+  /* "kola/lexer.pyx":168
  *     def __cinit__(self, *args, **kwds):
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"             # <<<<<<<<<<<<<<
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  */
   __pyx_v_self->lexer_data.filename = ((char const *)"<unknown>");
 
-  /* "kola/lexer.pyx":156
+  /* "kola/lexer.pyx":169
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1             # <<<<<<<<<<<<<<
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  *             PyErr_SetFromErrno(RuntimeError)
  */
   __pyx_v_self->lexer_data.command_threshold = 1;
 
-  /* "kola/lexer.pyx":157
+  /* "kola/lexer.pyx":170
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):             # <<<<<<<<<<<<<<
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  */
   __pyx_t_1 = (yylex_init_extra((&__pyx_v_self->lexer_data), (&__pyx_v_self->scanner)) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":158
+    /* "kola/lexer.pyx":171
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  *             PyErr_SetFromErrno(RuntimeError)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, **kwds):
  */
-    __pyx_t_2 = PyErr_SetFromErrno(__pyx_builtin_RuntimeError); if (unlikely(__pyx_t_2 == ((PyObject *)NULL))) __PYX_ERR(1, 158, __pyx_L1_error)
+    __pyx_t_2 = PyErr_SetFromErrno(__pyx_builtin_RuntimeError); if (unlikely(__pyx_t_2 == ((PyObject *)NULL))) __PYX_ERR(1, 171, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":157
+    /* "kola/lexer.pyx":170
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):             # <<<<<<<<<<<<<<
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":153
+  /* "kola/lexer.pyx":166
  *     """
  * 
  *     def __cinit__(self, *args, **kwds):             # <<<<<<<<<<<<<<
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  */
 
@@ -5786,15 +5695,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":160
+/* "kola/lexer.pyx":173
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  *     def __init__(self, **kwds):             # <<<<<<<<<<<<<<
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  */
 
@@ -5834,53 +5743,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":161
+  /* "kola/lexer.pyx":174
  * 
  *     def __init__(self, **kwds):
  *         yyrestart(stdin, self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<stdin>"
  *         LexerConfig(self).set(**kwds)
  */
   yyrestart(stdin, __pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":162
+  /* "kola/lexer.pyx":175
  *     def __init__(self, **kwds):
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  * 
  */
   __pyx_v_self->lexer_data.filename = ((char const *)"<stdin>");
 
-  /* "kola/lexer.pyx":163
+  /* "kola/lexer.pyx":176
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_1 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":160
+  /* "kola/lexer.pyx":173
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  *     def __init__(self, **kwds):             # <<<<<<<<<<<<<<
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  */
 
@@ -5894,15 +5803,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":165
+/* "kola/lexer.pyx":178
  *         LexerConfig(self).set(**kwds)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.close()
  *         if self.scanner:
  */
 
@@ -5919,64 +5828,64 @@
 }
 
 static void __pyx_pf_4kola_5lexer_9BaseLexer_4__dealloc__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "kola/lexer.pyx":166
+  /* "kola/lexer.pyx":179
  * 
  *     def __dealloc__(self):
  *         self.close()             # <<<<<<<<<<<<<<
  *         if self.scanner:
  *             yylex_destroy(self.scanner)
  */
   ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0);
 
-  /* "kola/lexer.pyx":167
+  /* "kola/lexer.pyx":180
  *     def __dealloc__(self):
  *         self.close()
  *         if self.scanner:             # <<<<<<<<<<<<<<
  *             yylex_destroy(self.scanner)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->scanner != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":168
+    /* "kola/lexer.pyx":181
  *         self.close()
  *         if self.scanner:
  *             yylex_destroy(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self):
  */
     (void)(yylex_destroy(__pyx_v_self->scanner));
 
-    /* "kola/lexer.pyx":167
+    /* "kola/lexer.pyx":180
  *     def __dealloc__(self):
  *         self.close()
  *         if self.scanner:             # <<<<<<<<<<<<<<
  *             yylex_destroy(self.scanner)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":165
+  /* "kola/lexer.pyx":178
  *         LexerConfig(self).set(**kwds)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.close()
  *         if self.scanner:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "kola/lexer.pyx":170
+/* "kola/lexer.pyx":183
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
 
@@ -6003,15 +5912,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4kola_5lexer_9BaseLexer_7close)) {
@@ -6028,15 +5937,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 183, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6049,24 +5958,24 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "kola/lexer.pyx":171
+  /* "kola/lexer.pyx":184
  * 
  *     cpdef void close(self):
  *         yypop_buffer_state(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cdef void set_error(self, const char* text) except *:
  */
   yypop_buffer_state(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":170
+  /* "kola/lexer.pyx":183
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
 
@@ -6120,15 +6029,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9BaseLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9BaseLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6137,15 +6046,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":173
+/* "kola/lexer.pyx":186
  *         yypop_buffer_state(self.scanner)
  * 
  *     cdef void set_error(self, const char* text) except *:             # <<<<<<<<<<<<<<
  *         cdef int errno = 1
  * 
  */
 
@@ -6158,42 +6067,42 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_error", 0);
 
-  /* "kola/lexer.pyx":174
+  /* "kola/lexer.pyx":187
  * 
  *     cdef void set_error(self, const char* text) except *:
  *         cdef int errno = 1             # <<<<<<<<<<<<<<
  * 
  *         # correct lineno and set error
  */
   __pyx_v_errno = 1;
 
-  /* "kola/lexer.pyx":177
+  /* "kola/lexer.pyx":190
  * 
  *         # correct lineno and set error
  *         cdef bint c = strchr(text, ord('\n')) != NULL             # <<<<<<<<<<<<<<
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:
  */
   __pyx_v_c = (strchr(__pyx_v_text, 10) != NULL);
 
-  /* "kola/lexer.pyx":178
+  /* "kola/lexer.pyx":191
  *         # correct lineno and set error
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  *         if c or text[0] == 0:
  *             lineno -= c
  */
   __pyx_v_lineno = yyget_lineno(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":179
+  /* "kola/lexer.pyx":192
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:             # <<<<<<<<<<<<<<
  *             lineno -= c
  *             errno = 10
  */
   __pyx_t_2 = (__pyx_v_c != 0);
@@ -6203,54 +6112,54 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (((__pyx_v_text[0]) == 0) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":180
+    /* "kola/lexer.pyx":193
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:
  *             lineno -= c             # <<<<<<<<<<<<<<
  *             errno = 10
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  */
     __pyx_v_lineno = (__pyx_v_lineno - __pyx_v_c);
 
-    /* "kola/lexer.pyx":181
+    /* "kola/lexer.pyx":194
  *         if c or text[0] == 0:
  *             lineno -= c
  *             errno = 10             # <<<<<<<<<<<<<<
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  */
     __pyx_v_errno = 10;
 
-    /* "kola/lexer.pyx":179
+    /* "kola/lexer.pyx":192
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:             # <<<<<<<<<<<<<<
  *             lineno -= c
  *             errno = 10
  */
   }
 
-  /* "kola/lexer.pyx":182
+  /* "kola/lexer.pyx":195
  *             lineno -= c
  *             errno = 10
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)             # <<<<<<<<<<<<<<
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 182, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  kola_set_error(__pyx_t_3, __pyx_v_errno, __pyx_v_self->lexer_data.filename, __pyx_v_lineno, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 182, __pyx_L1_error)
+  kola_set_error(__pyx_t_3, __pyx_v_errno, __pyx_v_self->lexer_data.filename, __pyx_v_lineno, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 195, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":173
+  /* "kola/lexer.pyx":186
  *         yypop_buffer_state(self.scanner)
  * 
  *     cdef void set_error(self, const char* text) except *:             # <<<<<<<<<<<<<<
  *         cdef int errno = 1
  * 
  */
 
@@ -6259,63 +6168,63 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("kola.lexer.BaseLexer.set_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "kola/lexer.pyx":184
+/* "kola/lexer.pyx":197
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:             # <<<<<<<<<<<<<<
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  */
 
 static __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_f_4kola_5lexer_9BaseLexer_next_syn(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   int __pyx_v_syn;
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_r;
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_t_1;
 
-  /* "kola/lexer.pyx":185
+  /* "kola/lexer.pyx":198
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  *         cdef int syn = yylex(self.scanner)             # <<<<<<<<<<<<<<
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  */
   __pyx_v_syn = yylex(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":186
+  /* "kola/lexer.pyx":199
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cdef Token next_token(self):
  */
   __pyx_t_1.f0 = __pyx_v_syn;
   __pyx_t_1.f1 = yyget_text(__pyx_v_self->scanner);
   __pyx_t_1.f2 = yyget_leng(__pyx_v_self->scanner);
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":184
+  /* "kola/lexer.pyx":197
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:             # <<<<<<<<<<<<<<
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":188
+/* "kola/lexer.pyx":201
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  *     cdef Token next_token(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")
  */
 
@@ -6352,47 +6261,47 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_token", 0);
 
-  /* "kola/lexer.pyx":189
+  /* "kola/lexer.pyx":202
  * 
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
  *             raise OSError("operation on closed lexer")
  * 
  */
   __pyx_t_1 = ((!(yylex_check(__pyx_v_self->scanner) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "kola/lexer.pyx":190
+    /* "kola/lexer.pyx":203
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")             # <<<<<<<<<<<<<<
  * 
  *         cdef:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 190, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 203, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 190, __pyx_L1_error)
+    __PYX_ERR(1, 203, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":189
+    /* "kola/lexer.pyx":202
  * 
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
  *             raise OSError("operation on closed lexer")
  * 
  */
   }
 
-  /* "kola/lexer.pyx":197
+  /* "kola/lexer.pyx":210
  *             Py_ssize_t text_len
  *             const char* encoding
  *         with nogil:             # <<<<<<<<<<<<<<
  *             syn, text, text_len = self.next_syn()
  * 
  */
   {
@@ -6400,15 +6309,15 @@
       PyThreadState *_save;
       _save = NULL;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "kola/lexer.pyx":198
+        /* "kola/lexer.pyx":211
  *             const char* encoding
  *         with nogil:
  *             syn, text, text_len = self.next_syn()             # <<<<<<<<<<<<<<
  * 
  *         val = None
  */
         __pyx_t_3 = ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_syn(__pyx_v_self);
@@ -6416,15 +6325,15 @@
         __pyx_t_5 = __pyx_t_3.f1;
         __pyx_t_6 = __pyx_t_3.f2;
         __pyx_v_syn = __pyx_t_4;
         __pyx_v_text = __pyx_t_5;
         __pyx_v_text_len = __pyx_t_6;
       }
 
-      /* "kola/lexer.pyx":197
+      /* "kola/lexer.pyx":210
  *             Py_ssize_t text_len
  *             const char* encoding
  *         with nogil:             # <<<<<<<<<<<<<<
  *             syn, text, text_len = self.next_syn()
  * 
  */
       /*finally:*/ {
@@ -6435,271 +6344,271 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "kola/lexer.pyx":200
+  /* "kola/lexer.pyx":213
  *             syn, text, text_len = self.next_syn()
  * 
  *         val = None             # <<<<<<<<<<<<<<
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_val = Py_None;
 
-  /* "kola/lexer.pyx":201
+  /* "kola/lexer.pyx":214
  * 
  *         val = None
  *         if syn == NUM or syn == CMD_N:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  */
   switch (__pyx_v_syn) {
     case NUM:
     case CMD_N:
 
-    /* "kola/lexer.pyx":202
+    /* "kola/lexer.pyx":215
  *         val = None
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 10); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 202, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 10); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":201
+    /* "kola/lexer.pyx":214
  * 
  *         val = None
  *         if syn == NUM or syn == CMD_N:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  */
     break;
     case NUM_H:
 
-    /* "kola/lexer.pyx":204
+    /* "kola/lexer.pyx":217
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":203
+    /* "kola/lexer.pyx":216
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:
  */
     break;
     case NUM_B:
 
-    /* "kola/lexer.pyx":206
+    /* "kola/lexer.pyx":219
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 206, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":205
+    /* "kola/lexer.pyx":218
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:
  */
     break;
     case NUM_F:
 
-    /* "kola/lexer.pyx":208
+    /* "kola/lexer.pyx":221
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)             # <<<<<<<<<<<<<<
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 208, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyFloat_FromString(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 208, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFloat_FromString(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":207
+    /* "kola/lexer.pyx":220
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:             # <<<<<<<<<<<<<<
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:
  */
     break;
     case CMD:
 
-    /* "kola/lexer.pyx":209
+    /* "kola/lexer.pyx":222
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:             # <<<<<<<<<<<<<<
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  */
     case LITERAL:
 
-    /* "kola/lexer.pyx":210
+    /* "kola/lexer.pyx":223
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)             # <<<<<<<<<<<<<<
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)
  */
-    __pyx_t_7 = PyUnicode_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 210, __pyx_L1_error)
+    __pyx_t_7 = PyUnicode_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":209
+    /* "kola/lexer.pyx":222
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:             # <<<<<<<<<<<<<<
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  */
     break;
     case TEXT:
 
-    /* "kola/lexer.pyx":211
+    /* "kola/lexer.pyx":224
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     case ANNOTATION:
 
-    /* "kola/lexer.pyx":212
+    /* "kola/lexer.pyx":225
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)             # <<<<<<<<<<<<<<
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)
  */
     __pyx_t_7 = __pyx_v_self->encoding;
     __Pyx_INCREF(__pyx_t_7);
-    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 212, __pyx_L1_error)
+    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 225, __pyx_L1_error)
     __pyx_v_encoding = __pyx_t_8;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":213
+    /* "kola/lexer.pyx":226
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)             # <<<<<<<<<<<<<<
  *             val = <str>filter_text(s)
  *         elif syn == STRING:
  */
-    __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 213, __pyx_L1_error)
+    __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_v_s = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":214
+    /* "kola/lexer.pyx":227
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)             # <<<<<<<<<<<<<<
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 214, __pyx_L1_error)
-    __pyx_t_9 = filter_text(((PyObject*)__pyx_v_s)); if (unlikely(__pyx_t_9 == ((PyObject *)NULL))) __PYX_ERR(1, 214, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 227, __pyx_L1_error)
+    __pyx_t_9 = filter_text(((PyObject*)__pyx_v_s)); if (unlikely(__pyx_t_9 == ((PyObject *)NULL))) __PYX_ERR(1, 227, __pyx_L1_error)
     __pyx_t_7 = ((PyObject *)__pyx_t_9);
     __Pyx_INCREF(__pyx_t_7);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":211
+    /* "kola/lexer.pyx":224
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     break;
     case STRING:
 
-    /* "kola/lexer.pyx":216
+    /* "kola/lexer.pyx":229
  *             val = <str>filter_text(s)
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)             # <<<<<<<<<<<<<<
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     __pyx_t_7 = __pyx_v_self->encoding;
     __Pyx_INCREF(__pyx_t_7);
-    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 216, __pyx_L1_error)
+    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 229, __pyx_L1_error)
     __pyx_v_encoding = __pyx_t_8;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":217
+    /* "kola/lexer.pyx":230
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:             # <<<<<<<<<<<<<<
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  */
     __pyx_t_1 = ((strcmp(__pyx_v_encoding, ((char const *)"utf-8")) != 0) != 0);
     if (__pyx_t_1) {
 
-      /* "kola/lexer.pyx":218
+      /* "kola/lexer.pyx":231
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)             # <<<<<<<<<<<<<<
  *                 text = unicode2string(s, &text_len)
  *             try:
  */
-      __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 218, __pyx_L1_error)
+      __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 231, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_v_s = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "kola/lexer.pyx":219
+      /* "kola/lexer.pyx":232
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)             # <<<<<<<<<<<<<<
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  */
-      if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 219, __pyx_L1_error)
-      __pyx_t_8 = unicode2string(((PyObject*)__pyx_v_s), (&__pyx_v_text_len)); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 219, __pyx_L1_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 232, __pyx_L1_error)
+      __pyx_t_8 = unicode2string(((PyObject*)__pyx_v_s), (&__pyx_v_text_len)); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 232, __pyx_L1_error)
       __pyx_v_text = __pyx_t_8;
 
-      /* "kola/lexer.pyx":217
+      /* "kola/lexer.pyx":230
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:             # <<<<<<<<<<<<<<
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  */
     }
 
-    /* "kola/lexer.pyx":220
+    /* "kola/lexer.pyx":233
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
     {
@@ -6707,27 +6616,27 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       /*try:*/ {
 
-        /* "kola/lexer.pyx":221
+        /* "kola/lexer.pyx":234
  *                 text = unicode2string(s, &text_len)
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)             # <<<<<<<<<<<<<<
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  */
-        __pyx_t_7 = decode_escapes((__pyx_v_text + 1), (__pyx_v_text_len - 2)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 221, __pyx_L8_error)
+        __pyx_t_7 = decode_escapes((__pyx_v_text + 1), (__pyx_v_text_len - 2)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 234, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "kola/lexer.pyx":220
+        /* "kola/lexer.pyx":233
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
       }
@@ -6735,46 +6644,46 @@
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       goto __pyx_L13_try_end;
       __pyx_L8_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "kola/lexer.pyx":222
+      /* "kola/lexer.pyx":235
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  */
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("kola.lexer.BaseLexer.next_token", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_2, &__pyx_t_13) < 0) __PYX_ERR(1, 222, __pyx_L10_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_2, &__pyx_t_13) < 0) __PYX_ERR(1, 235, __pyx_L10_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_2);
         __pyx_v_e = __pyx_t_2;
         /*try:*/ {
 
-          /* "kola/lexer.pyx":223
+          /* "kola/lexer.pyx":236
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)             # <<<<<<<<<<<<<<
  *         elif syn == 0:
  *             self.set_error(text)
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 223, __pyx_L19_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 236, __pyx_L19_error)
           __Pyx_GOTREF(__pyx_t_14);
-          kola_set_errcause(__pyx_t_14, 5, __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner), __pyx_v_text, __pyx_v_e); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 223, __pyx_L19_error)
+          kola_set_errcause(__pyx_t_14, 5, __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner), __pyx_v_text, __pyx_v_e); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 236, __pyx_L19_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         }
 
-        /* "kola/lexer.pyx":222
+        /* "kola/lexer.pyx":235
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  */
         /*finally:*/ {
@@ -6820,15 +6729,15 @@
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         goto __pyx_L9_exception_handled;
       }
       goto __pyx_L10_except_error;
       __pyx_L10_except_error:;
 
-      /* "kola/lexer.pyx":220
+      /* "kola/lexer.pyx":233
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
       __Pyx_XGIVEREF(__pyx_t_10);
@@ -6840,142 +6749,142 @@
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       __pyx_L13_try_end:;
     }
 
-    /* "kola/lexer.pyx":215
+    /* "kola/lexer.pyx":228
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)
  *         elif syn == STRING:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:
  */
     break;
     case 0:
 
-    /* "kola/lexer.pyx":225
+    /* "kola/lexer.pyx":238
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  *             self.set_error(text)             # <<<<<<<<<<<<<<
  *         elif syn == EOF:
  *             return None
  */
-    ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->set_error(__pyx_v_self, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->set_error(__pyx_v_self, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":224
+    /* "kola/lexer.pyx":237
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:             # <<<<<<<<<<<<<<
  *             self.set_error(text)
  *         elif syn == EOF:
  */
     break;
     case EOF:
 
-    /* "kola/lexer.pyx":227
+    /* "kola/lexer.pyx":240
  *             self.set_error(text)
  *         elif syn == EOF:
  *             return None             # <<<<<<<<<<<<<<
  *         return Token(
  *             syn, val,
  */
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __pyx_r = ((struct __pyx_obj_4kola_5lexer_Token *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":226
+    /* "kola/lexer.pyx":239
  *         elif syn == 0:
  *             self.set_error(text)
  *         elif syn == EOF:             # <<<<<<<<<<<<<<
  *             return None
  *         return Token(
  */
     break;
     default: break;
   }
 
-  /* "kola/lexer.pyx":228
+  /* "kola/lexer.pyx":241
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
 
-  /* "kola/lexer.pyx":229
+  /* "kola/lexer.pyx":242
  *             return None
  *         return Token(
  *             syn, val,             # <<<<<<<<<<<<<<
  *             lineno=yyget_lineno(self.scanner),
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)
  */
-  __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_syn); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_syn); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
 
-  /* "kola/lexer.pyx":228
+  /* "kola/lexer.pyx":241
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_13);
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_val);
   __pyx_t_13 = 0;
 
-  /* "kola/lexer.pyx":230
+  /* "kola/lexer.pyx":243
  *         return Token(
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),             # <<<<<<<<<<<<<<
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)
  *         )
  */
-  __pyx_t_13 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 230, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_7 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 230, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_lineno, __pyx_t_7) < 0) __PYX_ERR(1, 230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_lineno, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":231
+  /* "kola/lexer.pyx":244
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = PyBytes_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 231, __pyx_L1_error)
+  __pyx_t_7 = PyBytes_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_raw_val, __pyx_t_7) < 0) __PYX_ERR(1, 230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_raw_val, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":228
+  /* "kola/lexer.pyx":241
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
-  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_4kola_5lexer_Token), __pyx_t_2, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_4kola_5lexer_Token), __pyx_t_2, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __pyx_r = ((struct __pyx_obj_4kola_5lexer_Token *)__pyx_t_7);
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":188
+  /* "kola/lexer.pyx":201
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  *     cdef Token next_token(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")
  */
 
@@ -6992,15 +6901,15 @@
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":234
+/* "kola/lexer.pyx":247
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self.lexer_data.filename.decode()
  */
 
@@ -7024,31 +6933,31 @@
   char const *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":236
+  /* "kola/lexer.pyx":249
  *     @property
  *     def filename(self):
  *         return self.lexer_data.filename.decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->lexer_data.filename;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 236, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":234
+  /* "kola/lexer.pyx":247
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self.lexer_data.filename.decode()
  */
 
@@ -7059,15 +6968,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":238
+/* "kola/lexer.pyx":251
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)
  */
 
@@ -7090,29 +6999,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":240
+  /* "kola/lexer.pyx":253
  *     @property
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":238
+  /* "kola/lexer.pyx":251
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)
  */
 
@@ -7123,15 +7032,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":242
+/* "kola/lexer.pyx":255
  *         return yyget_lineno(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def column(self):
  *         return yyget_column(self.scanner)
  */
 
@@ -7154,29 +7063,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":244
+  /* "kola/lexer.pyx":257
  *     @property
  *     def column(self):
  *         return yyget_column(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_column(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_column(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":242
+  /* "kola/lexer.pyx":255
  *         return yyget_lineno(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def column(self):
  *         return yyget_column(self.scanner)
  */
 
@@ -7187,15 +7096,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":246
+/* "kola/lexer.pyx":259
  *         return yyget_column(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)
  */
 
@@ -7218,29 +7127,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":248
+  /* "kola/lexer.pyx":261
  *     @property
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":246
+  /* "kola/lexer.pyx":259
  *         return yyget_column(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)
  */
 
@@ -7251,15 +7160,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":250
+/* "kola/lexer.pyx":263
  *         return LexerConfig(self)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)
  */
 
@@ -7282,29 +7191,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":252
+  /* "kola/lexer.pyx":265
  *     @property
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(yylex_check(__pyx_v_self->scanner) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(yylex_check(__pyx_v_self->scanner) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":250
+  /* "kola/lexer.pyx":263
  *         return LexerConfig(self)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)
  */
 
@@ -7315,15 +7224,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":254
+/* "kola/lexer.pyx":267
  *         return not yylex_check(self.scanner)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -7342,42 +7251,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_8__iter__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "kola/lexer.pyx":255
+  /* "kola/lexer.pyx":268
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":254
+  /* "kola/lexer.pyx":267
  *         return not yylex_check(self.scanner)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":257
+/* "kola/lexer.pyx":270
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         token = self.next_token()
  *         if token is None:
  */
 
@@ -7403,69 +7312,69 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "kola/lexer.pyx":258
+  /* "kola/lexer.pyx":271
  * 
  *     def __next__(self):
  *         token = self.next_token()             # <<<<<<<<<<<<<<
  *         if token is None:
  *             raise StopIteration
  */
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_token(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 258, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_token(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_token = ((struct __pyx_obj_4kola_5lexer_Token *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":259
+  /* "kola/lexer.pyx":272
  *     def __next__(self):
  *         token = self.next_token()
  *         if token is None:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  *         return token
  */
   __pyx_t_2 = (((PyObject *)__pyx_v_token) == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "kola/lexer.pyx":260
+    /* "kola/lexer.pyx":273
  *         token = self.next_token()
  *         if token is None:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  *         return token
  * 
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(1, 260, __pyx_L1_error)
+    __PYX_ERR(1, 273, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":259
+    /* "kola/lexer.pyx":272
  *     def __next__(self):
  *         token = self.next_token()
  *         if token is None:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  *         return token
  */
   }
 
-  /* "kola/lexer.pyx":261
+  /* "kola/lexer.pyx":274
  *         if token is None:
  *             raise StopIteration
  *         return token             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_token);
   __pyx_r = ((PyObject *)__pyx_v_token);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":257
+  /* "kola/lexer.pyx":270
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         token = self.next_token()
  *         if token is None:
  */
 
@@ -7477,15 +7386,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_token);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":263
+/* "kola/lexer.pyx":276
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -7523,42 +7432,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_12__enter__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "kola/lexer.pyx":264
+  /* "kola/lexer.pyx":277
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, *args):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":263
+  /* "kola/lexer.pyx":276
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":266
+/* "kola/lexer.pyx":279
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -7584,44 +7493,44 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_14__exit__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "kola/lexer.pyx":267
+  /* "kola/lexer.pyx":280
  * 
  *     def __exit__(self, *args):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0);
 
-  /* "kola/lexer.pyx":266
+  /* "kola/lexer.pyx":279
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":269
+/* "kola/lexer.pyx":282
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
+ *             return PyUnicode_FromFormat(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_9BaseLexer_17__repr__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4kola_5lexer_9BaseLexer_17__repr__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
@@ -7640,91 +7549,99 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "kola/lexer.pyx":270
+  /* "kola/lexer.pyx":283
  * 
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
- *         else:
+ *             return PyUnicode_FromFormat(
+ *                 "<kola lexer in file \"%s\" closed>",
  */
   __pyx_t_1 = ((!(yylex_check(__pyx_v_self->scanner) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":271
+    /* "kola/lexer.pyx":284
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")             # <<<<<<<<<<<<<<
- *         else:
- *             return PyUnicode_FromFormat(
+ *             return PyUnicode_FromFormat(             # <<<<<<<<<<<<<<
+ *                 "<kola lexer in file \"%s\" closed>",
+ *                 self.lexer_data.filename
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" closed>")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 271, __pyx_L1_error)
+
+    /* "kola/lexer.pyx":286
+ *             return PyUnicode_FromFormat(
+ *                 "<kola lexer in file \"%s\" closed>",
+ *                 self.lexer_data.filename             # <<<<<<<<<<<<<<
+ *             )
+ *         else:
+ */
+    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" closed>"), __pyx_v_self->lexer_data.filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":270
+    /* "kola/lexer.pyx":283
  * 
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
- *         else:
+ *             return PyUnicode_FromFormat(
+ *                 "<kola lexer in file \"%s\" closed>",
  */
   }
 
-  /* "kola/lexer.pyx":273
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
+  /* "kola/lexer.pyx":289
+ *             )
  *         else:
  *             return PyUnicode_FromFormat(             # <<<<<<<<<<<<<<
  *                 "<kola lexer in file \"%s\" line %d>",
  *                 self.lexer_data.filename,
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
 
-    /* "kola/lexer.pyx":276
+    /* "kola/lexer.pyx":292
  *                 "<kola lexer in file \"%s\" line %d>",
  *                 self.lexer_data.filename,
  *                 yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" line %d>"), __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 273, __pyx_L1_error)
+    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" line %d>"), __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":269
+  /* "kola/lexer.pyx":282
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
+ *             return PyUnicode_FromFormat(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":31
+/* "kola/lexer.pxd":35
  *         LexerData lexer_data
  *     cdef readonly:
  *         str encoding             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self)
  */
 
@@ -7939,15 +7856,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":285
+/* "kola/lexer.pyx":301
  *     """
  * 
  *     def __init__(self, __path not None, **kwds):             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
 
@@ -7981,39 +7898,39 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_FileLexer__path)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 285, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 285, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 301, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v__FileLexer__path = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 285, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 301, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwds); __pyx_v_kwds = 0;
   __Pyx_AddTraceback("kola.lexer.FileLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v__FileLexer__path) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "__path"); __PYX_ERR(1, 285, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "__path"); __PYX_ERR(1, 301, __pyx_L1_error)
   }
   __pyx_r = __pyx_pf_4kola_5lexer_9FileLexer___init__(((struct __pyx_obj_4kola_5lexer_FileLexer *)__pyx_v_self), __pyx_v__FileLexer__path, __pyx_v_kwds);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
@@ -8035,157 +7952,157 @@
   char const *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":286
+  /* "kola/lexer.pyx":302
  * 
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->fp != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":287
+    /* "kola/lexer.pyx":303
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:
  *             fclose(self.fp)             # <<<<<<<<<<<<<<
  * 
  *         self._filenameo = __path
  */
     (void)(fclose(__pyx_v_self->fp));
 
-    /* "kola/lexer.pyx":286
+    /* "kola/lexer.pyx":302
  * 
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":289
+  /* "kola/lexer.pyx":305
  *             fclose(self.fp)
  * 
  *         self._filenameo = __path             # <<<<<<<<<<<<<<
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')
  */
   __Pyx_INCREF(__pyx_v__FileLexer__path);
   __Pyx_GIVEREF(__pyx_v__FileLexer__path);
   __Pyx_GOTREF(__pyx_v_self->_filenameo);
   __Pyx_DECREF(__pyx_v_self->_filenameo);
   __pyx_v_self->_filenameo = __pyx_v__FileLexer__path;
 
-  /* "kola/lexer.pyx":291
+  /* "kola/lexer.pyx":307
  *         self._filenameo = __path
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')             # <<<<<<<<<<<<<<
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  */
-  __pyx_t_2 = kola_open(__pyx_v__FileLexer__path, (&__pyx_v_p_addr), ((char const *)"r")); if (unlikely(__pyx_t_2 == ((FILE *)NULL))) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_2 = kola_open(__pyx_v__FileLexer__path, (&__pyx_v_p_addr), ((char const *)"r")); if (unlikely(__pyx_t_2 == ((FILE *)NULL))) __PYX_ERR(1, 307, __pyx_L1_error)
   __pyx_v_self->fp = __pyx_t_2;
 
-  /* "kola/lexer.pyx":292
+  /* "kola/lexer.pyx":308
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')
  *         p = <object>p_addr             # <<<<<<<<<<<<<<
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  *         Py_DECREF(p)
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_p_addr);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_p = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":293
+  /* "kola/lexer.pyx":309
  *         self.fp = kola_open(__path, &p_addr, 'r')
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()             # <<<<<<<<<<<<<<
  *         Py_DECREF(p)
  * 
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_p); 
   if ((__pyx_t_1 != 0)) {
     __Pyx_INCREF(((PyObject*)__pyx_v_p));
     __pyx_t_3 = __pyx_v_p;
   } else {
     if (unlikely(__pyx_v_p == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-      __PYX_ERR(1, 293, __pyx_L1_error)
+      __PYX_ERR(1, 309, __pyx_L1_error)
     }
-    __pyx_t_4 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_p), NULL, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_p), NULL, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 309, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_filenameb);
   __Pyx_DECREF(__pyx_v_self->_filenameb);
   __pyx_v_self->_filenameb = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":294
+  /* "kola/lexer.pyx":310
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  *         Py_DECREF(p)             # <<<<<<<<<<<<<<
  * 
  *         yyrestart(self.fp, self.scanner)
  */
   Py_DECREF(__pyx_v_p);
 
-  /* "kola/lexer.pyx":296
+  /* "kola/lexer.pyx":312
  *         Py_DECREF(p)
  * 
  *         yyrestart(self.fp, self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = self._filenameb
  *         LexerConfig(self).set(**kwds)
  */
   yyrestart(__pyx_v_self->fp, __pyx_v_self->__pyx_base.scanner);
 
-  /* "kola/lexer.pyx":297
+  /* "kola/lexer.pyx":313
  * 
  *         yyrestart(self.fp, self.scanner)
  *         self.lexer_data.filename = self._filenameb             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  * 
  */
   if (unlikely(__pyx_v_self->_filenameb == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 297, __pyx_L1_error)
+    __PYX_ERR(1, 313, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_v_self->_filenameb); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(1, 297, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_v_self->_filenameb); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(1, 313, __pyx_L1_error)
   __pyx_v_self->__pyx_base.lexer_data.filename = __pyx_t_5;
 
-  /* "kola/lexer.pyx":298
+  /* "kola/lexer.pyx":314
  *         yyrestart(self.fp, self.scanner)
  *         self.lexer_data.filename = self._filenameb
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self):
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "kola/lexer.pyx":285
+  /* "kola/lexer.pyx":301
  *     """
  * 
  *     def __init__(self, __path not None, **kwds):             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
 
@@ -8200,15 +8117,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":300
+/* "kola/lexer.pyx":316
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
 
@@ -8236,15 +8153,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 316, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4kola_5lexer_9FileLexer_3close)) {
@@ -8261,15 +8178,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 300, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 316, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -8282,61 +8199,61 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "kola/lexer.pyx":301
+  /* "kola/lexer.pyx":317
  * 
  *     cpdef void close(self):
  *         BaseLexer.close(self)             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
   __pyx_f_4kola_5lexer_9BaseLexer_close(((struct __pyx_obj_4kola_5lexer_BaseLexer *)__pyx_v_self), 1);
 
-  /* "kola/lexer.pyx":302
+  /* "kola/lexer.pyx":318
  *     cpdef void close(self):
  *         BaseLexer.close(self)
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  *             self.fp = NULL
  */
   __pyx_t_6 = (__pyx_v_self->fp != 0);
   if (__pyx_t_6) {
 
-    /* "kola/lexer.pyx":303
+    /* "kola/lexer.pyx":319
  *         BaseLexer.close(self)
  *         if self.fp:
  *             fclose(self.fp)             # <<<<<<<<<<<<<<
  *             self.fp = NULL
  * 
  */
     (void)(fclose(__pyx_v_self->fp));
 
-    /* "kola/lexer.pyx":304
+    /* "kola/lexer.pyx":320
  *         if self.fp:
  *             fclose(self.fp)
  *             self.fp = NULL             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __pyx_v_self->fp = NULL;
 
-    /* "kola/lexer.pyx":302
+    /* "kola/lexer.pyx":318
  *     cpdef void close(self):
  *         BaseLexer.close(self)
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  *             self.fp = NULL
  */
   }
 
-  /* "kola/lexer.pyx":300
+  /* "kola/lexer.pyx":316
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
 
@@ -8390,15 +8307,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9FileLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9FileLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8407,15 +8324,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":306
+/* "kola/lexer.pyx":322
  *             self.fp = NULL
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self._filenameo
  */
 
@@ -8434,27 +8351,27 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9FileLexer_8filename___get__(struct __pyx_obj_4kola_5lexer_FileLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":308
+  /* "kola/lexer.pyx":324
  *     @property
  *     def filename(self):
  *         return self._filenameo             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_filenameo);
   __pyx_r = __pyx_v_self->_filenameo;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":306
+  /* "kola/lexer.pyx":322
  *             self.fp = NULL
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self._filenameo
  */
 
@@ -8646,15 +8563,15 @@
   __Pyx_AddTraceback("kola.lexer.FileLexer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":316
+/* "kola/lexer.pyx":332
  *     """
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):             # <<<<<<<<<<<<<<
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)
  */
 
@@ -8688,31 +8605,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_content)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 316, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 332, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 316, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 332, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_content = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 316, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 332, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwds); __pyx_v_kwds = 0;
   __Pyx_AddTraceback("kola.lexer.StringLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4kola_5lexer_11StringLexer___init__(((struct __pyx_obj_4kola_5lexer_StringLexer *)__pyx_v_self), __pyx_v_content, __pyx_v_kwds);
@@ -8734,151 +8651,151 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":317
+  /* "kola/lexer.pyx":333
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:             # <<<<<<<<<<<<<<
  *             yypop_buffer_state(self.scanner)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->content != ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "kola/lexer.pyx":318
+    /* "kola/lexer.pyx":334
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(content, str):
  */
     yypop_buffer_state(__pyx_v_self->__pyx_base.scanner);
 
-    /* "kola/lexer.pyx":317
+    /* "kola/lexer.pyx":333
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:             # <<<<<<<<<<<<<<
  *             yypop_buffer_state(self.scanner)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":320
+  /* "kola/lexer.pyx":336
  *             yypop_buffer_state(self.scanner)
  * 
  *         if isinstance(content, str):             # <<<<<<<<<<<<<<
  *             self.content = (<str>content).encode()
  *         else:
  */
   __pyx_t_2 = PyUnicode_Check(__pyx_v_content); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":321
+    /* "kola/lexer.pyx":337
  * 
  *         if isinstance(content, str):
  *             self.content = (<str>content).encode()             # <<<<<<<<<<<<<<
  *         else:
  *             self.content = content
  */
     if (unlikely(__pyx_v_content == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-      __PYX_ERR(1, 321, __pyx_L1_error)
+      __PYX_ERR(1, 337, __pyx_L1_error)
     }
-    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_content), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 321, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_content), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->content);
     __Pyx_DECREF(__pyx_v_self->content);
     __pyx_v_self->content = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "kola/lexer.pyx":320
+    /* "kola/lexer.pyx":336
  *             yypop_buffer_state(self.scanner)
  * 
  *         if isinstance(content, str):             # <<<<<<<<<<<<<<
  *             self.content = (<str>content).encode()
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "kola/lexer.pyx":323
+  /* "kola/lexer.pyx":339
  *             self.content = (<str>content).encode()
  *         else:
  *             self.content = content             # <<<<<<<<<<<<<<
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  */
   /*else*/ {
-    if (!(likely(PyBytes_CheckExact(__pyx_v_content))||((__pyx_v_content) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_content))) __PYX_ERR(1, 323, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_v_content))||((__pyx_v_content) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_content))) __PYX_ERR(1, 339, __pyx_L1_error)
     __pyx_t_3 = __pyx_v_content;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->content);
     __Pyx_DECREF(__pyx_v_self->content);
     __pyx_v_self->content = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
   }
   __pyx_L4:;
 
-  /* "kola/lexer.pyx":325
+  /* "kola/lexer.pyx":341
  *             self.content = content
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<string>"
  *         LexerConfig(self).set(**kwds)
  */
   if (unlikely(__pyx_v_self->content == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 325, __pyx_L1_error)
+    __PYX_ERR(1, 341, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_self->content); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 325, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_self->content); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 341, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_self->content;
   __Pyx_INCREF(__pyx_t_3);
   if (unlikely(__pyx_t_3 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(1, 325, __pyx_L1_error)
+    __PYX_ERR(1, 341, __pyx_L1_error)
   }
-  __pyx_t_5 = PyBytes_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 325, __pyx_L1_error)
+  __pyx_t_5 = PyBytes_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   (void)(yy_scan_bytes(__pyx_t_4, __pyx_t_5, __pyx_v_self->__pyx_base.scanner));
 
-  /* "kola/lexer.pyx":326
+  /* "kola/lexer.pyx":342
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  *         self.lexer_data.filename = "<string>"             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  */
   __pyx_v_self->__pyx_base.lexer_data.filename = ((char const *)"<string>");
 
-  /* "kola/lexer.pyx":327
+  /* "kola/lexer.pyx":343
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  *         self.lexer_data.filename = "<string>"
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 327, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 327, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":316
+  /* "kola/lexer.pyx":332
  *     """
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):             # <<<<<<<<<<<<<<
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)
  */
 
@@ -8892,15 +8809,15 @@
   __Pyx_AddTraceback("kola.lexer.StringLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":50
+/* "kola/lexer.pxd":54
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):
  *     cdef readonly bytes content             # <<<<<<<<<<<<<<
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11StringLexer_7content_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -10400,15 +10317,14 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   #if CYTHON_USE_MODULE_STATE
-  {0, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {0, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer, sizeof(__pyx_k_BaseLexer), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___enter, sizeof(__pyx_k_BaseLexer___enter), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___exit, sizeof(__pyx_k_BaseLexer___exit), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___reduce_cython, sizeof(__pyx_k_BaseLexer___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___setstate_cython, sizeof(__pyx_k_BaseLexer___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer_close, sizeof(__pyx_k_BaseLexer_close), 0, 0, 1, 1},
@@ -10447,37 +10363,34 @@
   {0, __pyx_k_StringLexer___reduce_cython, sizeof(__pyx_k_StringLexer___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_StringLexer___setstate_cython, sizeof(__pyx_k_StringLexer___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token, sizeof(__pyx_k_Token), 0, 0, 1, 1},
   {0, __pyx_k_Token___reduce_cython, sizeof(__pyx_k_Token___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token___setstate_cython, sizeof(__pyx_k_Token___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token_get_flag, sizeof(__pyx_k_Token_get_flag), 0, 0, 1, 1},
   {0, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
+  {0, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 1},
+  {0, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {0, __pyx_k__26, sizeof(__pyx_k__26), 0, 0, 1, 1},
-  {0, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {0, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {0, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {0, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {0, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
-  {0, __pyx_k_command_threshold, sizeof(__pyx_k_command_threshold), 0, 0, 1, 1},
   {0, __pyx_k_content, sizeof(__pyx_k_content), 0, 0, 1, 1},
   {0, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+  {0, __pyx_k_data_names, sizeof(__pyx_k_data_names), 0, 1, 0, 1},
   {0, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {0, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {0, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
-  {0, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 1, 0, 1},
-  {0, __pyx_k_endswith, sizeof(__pyx_k_endswith), 0, 0, 1, 1},
   {0, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {0, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {0, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {0, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
-  {0, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
-  {0, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
   {0, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
   {0, __pyx_k_get_flag, sizeof(__pyx_k_get_flag), 0, 0, 1, 1},
   {0, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {0, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {0, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {0, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
   {0, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
   {0, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {0, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {0, __pyx_k_kola_lexer, sizeof(__pyx_k_kola_lexer), 0, 0, 1, 1},
   {0, __pyx_k_kola_lexer_pyx, sizeof(__pyx_k_kola_lexer_pyx), 0, 0, 1, 0},
@@ -10496,23 +10409,21 @@
   {0, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {0, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {0, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {0, __pyx_k_self_lexer_data_cannot_be_conver, sizeof(__pyx_k_self_lexer_data_cannot_be_conver), 0, 0, 1, 0},
   {0, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {0, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {0, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {0, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {0, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {0, __pyx_k_syn, sizeof(__pyx_k_syn), 0, 0, 1, 1},
   {0, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {0, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {0, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   #else
-  {&__pyx_n_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {&__pyx_n_s_AttributeError, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer, __pyx_k_BaseLexer, sizeof(__pyx_k_BaseLexer), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___enter, __pyx_k_BaseLexer___enter, sizeof(__pyx_k_BaseLexer___enter), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___exit, __pyx_k_BaseLexer___exit, sizeof(__pyx_k_BaseLexer___exit), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___reduce_cython, __pyx_k_BaseLexer___reduce_cython, sizeof(__pyx_k_BaseLexer___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___setstate_cython, __pyx_k_BaseLexer___setstate_cython, sizeof(__pyx_k_BaseLexer___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer_close, __pyx_k_BaseLexer_close, sizeof(__pyx_k_BaseLexer_close), 0, 0, 1, 1},
@@ -10551,37 +10462,34 @@
   {&__pyx_n_s_StringLexer___reduce_cython, __pyx_k_StringLexer___reduce_cython, sizeof(__pyx_k_StringLexer___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_StringLexer___setstate_cython, __pyx_k_StringLexer___setstate_cython, sizeof(__pyx_k_StringLexer___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token, __pyx_k_Token, sizeof(__pyx_k_Token), 0, 0, 1, 1},
   {&__pyx_n_s_Token___reduce_cython, __pyx_k_Token___reduce_cython, sizeof(__pyx_k_Token___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token___setstate_cython, __pyx_k_Token___setstate_cython, sizeof(__pyx_k_Token___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token_get_flag, __pyx_k_Token_get_flag, sizeof(__pyx_k_Token_get_flag), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
+  {&__pyx_n_u__14, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 1},
+  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s__26, __pyx_k__26, sizeof(__pyx_k__26), 0, 0, 1, 1},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
-  {&__pyx_n_s_command_threshold, __pyx_k_command_threshold, sizeof(__pyx_k_command_threshold), 0, 0, 1, 1},
   {&__pyx_n_s_content, __pyx_k_content, sizeof(__pyx_k_content), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+  {&__pyx_n_u_data_names, __pyx_k_data_names, sizeof(__pyx_k_data_names), 0, 1, 0, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
-  {&__pyx_n_u_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 1, 0, 1},
-  {&__pyx_n_s_endswith, __pyx_k_endswith, sizeof(__pyx_k_endswith), 0, 0, 1, 1},
   {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
-  {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
-  {&__pyx_n_s_flag, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
   {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
   {&__pyx_n_s_get_flag, __pyx_k_get_flag, sizeof(__pyx_k_get_flag), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
   {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_kola_lexer, __pyx_k_kola_lexer, sizeof(__pyx_k_kola_lexer), 0, 0, 1, 1},
   {&__pyx_kp_s_kola_lexer_pyx, __pyx_k_kola_lexer_pyx, sizeof(__pyx_k_kola_lexer_pyx), 0, 0, 1, 0},
@@ -10600,317 +10508,311 @@
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_kp_s_self_lexer_data_cannot_be_conver, __pyx_k_self_lexer_data_cannot_be_conver, sizeof(__pyx_k_self_lexer_data_cannot_be_conver), 0, 0, 1, 0},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_syn, __pyx_k_syn, sizeof(__pyx_k_syn), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   #endif
   {0, 0, 0, 0, 0, 0, 0}
 };
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(1, 94, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 158, __pyx_L1_error)
-  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(1, 190, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(1, 260, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(1, 97, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(1, 203, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(1, 273, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "kola/lexer.pyx":190
+  /* "kola/lexer.pyx":203
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")             # <<<<<<<<<<<<<<
  * 
  *         cdef:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_operation_on_closed_lexer); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 190, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_operation_on_closed_lexer); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "kola/lexer.pyx":59
+  /* "kola/lexer.pyx":62
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_get_flag, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_get_flag, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 62, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":85
+  /* "kola/lexer.pyx":88
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_dict, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_i); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_dict, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 88, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":91
+  /* "kola/lexer.pyx":94
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  */
-  __pyx_tuple__11 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwds, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_set, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 91, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwds, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_set, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 94, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  */
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":170
+  /* "kola/lexer.pyx":183
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 183, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":263
+  /* "kola/lexer.pyx":276
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_enter, 263, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 263, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_enter, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 276, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":266
+  /* "kola/lexer.pyx":279
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_args); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 266, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_args); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_exit, 266, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 266, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_exit, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 279, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":300
+  /* "kola/lexer.pyx":316
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 300, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 300, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 316, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 316, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   #if CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_u_) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_n_s_AttributeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_BaseLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_BaseLexer___enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_BaseLexer___exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_BaseLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_BaseLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s_BaseLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s_F_DISABLED) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_F_LSTRIP_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_FileLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_FileLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_FileLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_FileLexer__path) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_FileLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_KoiLangSyntaxError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_LexerConfig) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_LexerConfig___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_LexerConfig___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s_LexerConfig_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_n_s_LexerConfig_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s_None) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_OSError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_RuntimeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_S_ANNOTATION) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_S_CLN) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_S_CMA) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_S_CMD) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_S_CMD_N) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_S_LITERAL) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_S_NUM) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_S_NUM_B) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_S_NUM_F) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_S_NUM_H) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_n_s_S_SLP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_n_s_S_SRP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_S_STRING) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_S_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_n_s_StopIteration) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_StringLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_StringLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_StringLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_Token) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_Token___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_n_s_Token___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_Token_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_s_TypeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_n_s__26) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_kp_u__3) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_s_AttributeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_n_s_BaseLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_BaseLexer___enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_BaseLexer___exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_BaseLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_BaseLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_BaseLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s_F_DISABLED) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s_F_LSTRIP_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_FileLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_FileLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_FileLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_FileLexer__path) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_FileLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_KoiLangSyntaxError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_LexerConfig) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_LexerConfig___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_LexerConfig___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_LexerConfig_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s_LexerConfig_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_n_s_None) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s_OSError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_RuntimeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_S_ANNOTATION) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_S_CLN) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_S_CMA) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_S_CMD) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_S_CMD_N) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_S_LITERAL) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_S_NUM) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_S_NUM_B) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_S_NUM_F) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_S_NUM_H) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_S_SLP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_n_s_S_SRP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_n_s_S_STRING) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_S_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_StopIteration) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_n_s_StringLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_StringLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_StringLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_Token) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_Token___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_Token___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_n_s_Token_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_TypeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_u__14) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_kp_u__2) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_n_s__26) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[49], &__pyx_n_s_args) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[50], &__pyx_n_s_asyncio_coroutines) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[51], &__pyx_n_s_cline_in_traceback) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[52], &__pyx_n_s_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[53], &__pyx_n_s_command_threshold) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[54], &__pyx_n_s_content) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[55], &__pyx_n_s_data) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[53], &__pyx_n_s_content) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[54], &__pyx_n_s_data) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[55], &__pyx_n_u_data_names) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[56], &__pyx_n_s_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[57], &__pyx_kp_u_disable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[58], &__pyx_kp_u_enable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[59], &__pyx_n_u_encoding) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[60], &__pyx_n_s_endswith) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[61], &__pyx_n_s_enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[62], &__pyx_n_s_exception) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[63], &__pyx_n_s_exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[64], &__pyx_n_s_filename) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[65], &__pyx_n_u_filename) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[66], &__pyx_n_s_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[67], &__pyx_kp_u_gc) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[68], &__pyx_n_s_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[69], &__pyx_n_s_getstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[70], &__pyx_n_s_import) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[71], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[72], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[73], &__pyx_n_s_items) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[74], &__pyx_n_s_k) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[75], &__pyx_n_s_kola_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[76], &__pyx_kp_s_kola_lexer_pyx) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[77], &__pyx_n_s_kwds) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[78], &__pyx_n_s_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[79], &__pyx_n_s_lineno) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[80], &__pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[81], &__pyx_n_s_name) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[82], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[83], &__pyx_kp_u_operation_on_closed_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[84], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[85], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[86], &__pyx_n_s_raw_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[87], &__pyx_n_s_reduce) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[88], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[89], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[90], &__pyx_n_s_return) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[91], &__pyx_n_s_self) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[92], &__pyx_kp_s_self_lexer_data_cannot_be_conver) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[93], &__pyx_n_s_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[94], &__pyx_n_s_setstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[95], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[96], &__pyx_n_s_startswith) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[97], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[98], &__pyx_n_s_syn) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[99], &__pyx_n_s_test) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[100], &__pyx_kp_u_utf_8) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[101], &__pyx_n_s_v) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[102], &__pyx_n_s_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[59], &__pyx_n_s_enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[60], &__pyx_n_s_exception) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[61], &__pyx_n_s_exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[62], &__pyx_kp_u_gc) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[63], &__pyx_n_s_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[64], &__pyx_n_s_getstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[65], &__pyx_n_s_i) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[66], &__pyx_n_s_import) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[67], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[68], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[69], &__pyx_n_s_items) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[70], &__pyx_n_s_k) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[71], &__pyx_n_s_kola_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[72], &__pyx_kp_s_kola_lexer_pyx) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[73], &__pyx_n_s_kwds) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[74], &__pyx_n_s_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[75], &__pyx_n_s_lineno) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[76], &__pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[77], &__pyx_n_s_name) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[78], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[79], &__pyx_kp_u_operation_on_closed_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[80], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[81], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[82], &__pyx_n_s_raw_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[83], &__pyx_n_s_reduce) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[84], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[85], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[86], &__pyx_n_s_return) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[87], &__pyx_n_s_self) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[88], &__pyx_kp_s_self_lexer_data_cannot_be_conver) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[89], &__pyx_n_s_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[90], &__pyx_n_s_setstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[91], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[92], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[93], &__pyx_n_s_syn) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[94], &__pyx_n_s_test) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[95], &__pyx_kp_u_utf_8) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[96], &__pyx_n_s_v) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[97], &__pyx_n_s_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   #endif
   #if !CYTHON_USE_MODULE_STATE
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   #endif
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -10930,14 +10832,16 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
+  __pyx_v_4kola_5lexer__lexer_data_names = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  __pyx_7genexpr__pyx_v_4kola_5lexer_i = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -10961,163 +10865,163 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_4kola_5lexer_Token = &__pyx_vtable_4kola_5lexer_Token;
   __pyx_vtable_4kola_5lexer_Token.get_flag = (int (*)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_5Token_get_flag;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_Token = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_Token_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_Token)) __PYX_ERR(1, 34, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_Token_spec, __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_Token = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_Token_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_Token)) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_Token_spec, __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_Token = &__pyx_type_4kola_5lexer_Token;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_Token->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_Token->tp_dictoffset && __pyx_ptype_4kola_5lexer_Token->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_Token->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_Token, __pyx_vtabptr_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_Token, __pyx_vtabptr_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Token, (PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Token, (PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_LexerConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_LexerConfig_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_LexerConfig)) __PYX_ERR(1, 76, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_LexerConfig_spec, __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_LexerConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_LexerConfig_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_LexerConfig)) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_LexerConfig_spec, __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_LexerConfig = &__pyx_type_4kola_5lexer_LexerConfig;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_LexerConfig->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_LexerConfig->tp_dictoffset && __pyx_ptype_4kola_5lexer_LexerConfig->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_LexerConfig->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LexerConfig, (PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LexerConfig, (PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_BaseLexer = &__pyx_vtable_4kola_5lexer_BaseLexer;
   __pyx_vtable_4kola_5lexer_BaseLexer.close = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_9BaseLexer_close;
   __pyx_vtable_4kola_5lexer_BaseLexer.set_error = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *))__pyx_f_4kola_5lexer_9BaseLexer_set_error;
   __pyx_vtable_4kola_5lexer_BaseLexer.next_syn = (__pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *))__pyx_f_4kola_5lexer_9BaseLexer_next_syn;
   __pyx_vtable_4kola_5lexer_BaseLexer.next_token = (struct __pyx_obj_4kola_5lexer_Token *(*)(struct __pyx_obj_4kola_5lexer_BaseLexer *))__pyx_f_4kola_5lexer_9BaseLexer_next_token;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_BaseLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_BaseLexer_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_BaseLexer)) __PYX_ERR(1, 148, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_BaseLexer_spec, __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_BaseLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_BaseLexer_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_BaseLexer)) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_BaseLexer_spec, __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_BaseLexer = &__pyx_type_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_BaseLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_BaseLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_BaseLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_BaseLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_BaseLexer, __pyx_vtabptr_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_BaseLexer, __pyx_vtabptr_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseLexer, (PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseLexer, (PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_FileLexer = &__pyx_vtable_4kola_5lexer_FileLexer;
   __pyx_vtable_4kola_5lexer_FileLexer.__pyx_base = *__pyx_vtabptr_4kola_5lexer_BaseLexer;
   __pyx_vtable_4kola_5lexer_FileLexer.__pyx_base.close = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_9FileLexer_close;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 280, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_FileLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_4kola_5lexer_FileLexer)) __PYX_ERR(1, 280, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_4kola_5lexer_FileLexer)) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_FileLexer = &__pyx_type_4kola_5lexer_FileLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_4kola_5lexer_FileLexer->tp_base = __pyx_ptype_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_FileLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_FileLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_FileLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_FileLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_FileLexer, __pyx_vtabptr_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_FileLexer, __pyx_vtabptr_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FileLexer, (PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FileLexer, (PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_StringLexer = &__pyx_vtable_4kola_5lexer_StringLexer;
   __pyx_vtable_4kola_5lexer_StringLexer.__pyx_base = *__pyx_vtabptr_4kola_5lexer_BaseLexer;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 311, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_StringLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_4kola_5lexer_StringLexer)) __PYX_ERR(1, 311, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_4kola_5lexer_StringLexer)) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_StringLexer = &__pyx_type_4kola_5lexer_StringLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_4kola_5lexer_StringLexer->tp_base = __pyx_ptype_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_StringLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_StringLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_StringLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_StringLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_StringLexer, __pyx_vtabptr_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_StringLexer, __pyx_vtabptr_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringLexer, (PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringLexer, (PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11335,14 +11239,21 @@
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  int __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -11451,354 +11362,525 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
-  /* "kola/lexer.pyx":9
+  /* "kola/lexer.pyx":12
  * from ._yylex cimport *
  * 
  * from .exception import KoiLangSyntaxError             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 9, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_KoiLangSyntaxError);
   __Pyx_GIVEREF(__pyx_n_s_KoiLangSyntaxError);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_KoiLangSyntaxError);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KoiLangSyntaxError, __pyx_t_2) < 0) __PYX_ERR(1, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KoiLangSyntaxError, __pyx_t_2) < 0) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":15
+  /* "kola/lexer.pyx":18
  * 
  * # token syn
  * S_CMD = CMD             # <<<<<<<<<<<<<<
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD, __pyx_t_3) < 0) __PYX_ERR(1, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD, __pyx_t_3) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":16
+  /* "kola/lexer.pyx":19
  * # token syn
  * S_CMD = CMD
  * S_CMD_N = CMD_N             # <<<<<<<<<<<<<<
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD_N); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD_N); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD_N, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD_N, __pyx_t_3) < 0) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":17
+  /* "kola/lexer.pyx":20
  * S_CMD = CMD
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT             # <<<<<<<<<<<<<<
  * S_LITERAL = LITERAL
  * S_STRING = STRING
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":18
+  /* "kola/lexer.pyx":21
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL             # <<<<<<<<<<<<<<
  * S_STRING = STRING
  * S_NUM = NUM
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(LITERAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 18, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(LITERAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_LITERAL, __pyx_t_3) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_LITERAL, __pyx_t_3) < 0) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":19
+  /* "kola/lexer.pyx":22
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL
  * S_STRING = STRING             # <<<<<<<<<<<<<<
  * S_NUM = NUM
  * S_NUM_H = NUM_H
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 19, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_STRING, __pyx_t_3) < 0) __PYX_ERR(1, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_STRING, __pyx_t_3) < 0) __PYX_ERR(1, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":20
+  /* "kola/lexer.pyx":23
  * S_LITERAL = LITERAL
  * S_STRING = STRING
  * S_NUM = NUM             # <<<<<<<<<<<<<<
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM, __pyx_t_3) < 0) __PYX_ERR(1, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM, __pyx_t_3) < 0) __PYX_ERR(1, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":21
+  /* "kola/lexer.pyx":24
  * S_STRING = STRING
  * S_NUM = NUM
  * S_NUM_H = NUM_H             # <<<<<<<<<<<<<<
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_H); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_H); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_H, __pyx_t_3) < 0) __PYX_ERR(1, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_H, __pyx_t_3) < 0) __PYX_ERR(1, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":22
+  /* "kola/lexer.pyx":25
  * S_NUM = NUM
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B             # <<<<<<<<<<<<<<
  * S_NUM_F = NUM_F
  * S_CLN = CLN
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_B); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_B); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_B, __pyx_t_3) < 0) __PYX_ERR(1, 22, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_B, __pyx_t_3) < 0) __PYX_ERR(1, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":23
+  /* "kola/lexer.pyx":26
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F             # <<<<<<<<<<<<<<
  * S_CLN = CLN
  * S_CMA = CMA
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_F); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_F); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_F, __pyx_t_3) < 0) __PYX_ERR(1, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_F, __pyx_t_3) < 0) __PYX_ERR(1, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":24
+  /* "kola/lexer.pyx":27
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F
  * S_CLN = CLN             # <<<<<<<<<<<<<<
  * S_CMA = CMA
  * S_SLP = SLP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CLN); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CLN); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CLN, __pyx_t_3) < 0) __PYX_ERR(1, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CLN, __pyx_t_3) < 0) __PYX_ERR(1, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":25
+  /* "kola/lexer.pyx":28
  * S_NUM_F = NUM_F
  * S_CLN = CLN
  * S_CMA = CMA             # <<<<<<<<<<<<<<
  * S_SLP = SLP
  * S_SRP = SRP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMA); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 25, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMA); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMA, __pyx_t_3) < 0) __PYX_ERR(1, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMA, __pyx_t_3) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":26
+  /* "kola/lexer.pyx":29
  * S_CLN = CLN
  * S_CMA = CMA
  * S_SLP = SLP             # <<<<<<<<<<<<<<
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SLP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SLP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SLP, __pyx_t_3) < 0) __PYX_ERR(1, 26, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SLP, __pyx_t_3) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":27
+  /* "kola/lexer.pyx":30
  * S_CMA = CMA
  * S_SLP = SLP
  * S_SRP = SRP             # <<<<<<<<<<<<<<
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SRP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 27, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SRP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SRP, __pyx_t_3) < 0) __PYX_ERR(1, 27, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SRP, __pyx_t_3) < 0) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":28
+  /* "kola/lexer.pyx":31
  * S_SLP = SLP
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION             # <<<<<<<<<<<<<<
  * F_DISABLED = LFLAG_DISABLED
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(ANNOTATION); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(ANNOTATION); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_ANNOTATION, __pyx_t_3) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_ANNOTATION, __pyx_t_3) < 0) __PYX_ERR(1, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":29
+  /* "kola/lexer.pyx":32
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED             # <<<<<<<<<<<<<<
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_DISABLED); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 29, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_DISABLED); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_DISABLED, __pyx_t_3) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_DISABLED, __pyx_t_3) < 0) __PYX_ERR(1, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":30
+  /* "kola/lexer.pyx":33
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_NOLSTRIP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_NOLSTRIP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_LSTRIP_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_LSTRIP_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":59
+  /* "kola/lexer.pyx":62
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_5get_flag, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token_get_flag, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_5get_flag, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token_get_flag, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_Token->tp_dict, __pyx_n_s_get_flag, __pyx_t_3) < 0) __PYX_ERR(1, 59, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_Token->tp_dict, __pyx_n_s_get_flag, __pyx_t_3) < 0) __PYX_ERR(1, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_Token);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":85
+  /* "kola/lexer.pyx":88
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = <dict>self.lexer_data[0]
- *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         cdef dict data = {}
+ *         for i in _lexer_data_names:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_dict) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_3dict, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_dict, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_dict) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_3dict, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_dict, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_dict, __pyx_t_2) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_dict, __pyx_t_2) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_LexerConfig);
 
-  /* "kola/lexer.pyx":91
+  /* "kola/lexer.pyx":94
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if k.startswith('__') and k.endswith('__'):
+ *             if not k in _lexer_data_names:
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 91, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 91, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_5set, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_set, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 91, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 94, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_5set, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_set, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_set, __pyx_t_3) < 0) __PYX_ERR(1, 91, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_set, __pyx_t_3) < 0) __PYX_ERR(1, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_LexerConfig);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":170
+  /* "kola/lexer.pyx":151
+ * 
+ * 
+ * cdef set _lexer_data_names = {             # <<<<<<<<<<<<<<
+ *     i for i in dir(LexerConfig)
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
+ */
+  { /* enter inner scope */
+    __pyx_t_3 = PySet_New(NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L4_error)
+    __Pyx_GOTREF(__pyx_t_3);
+
+    /* "kola/lexer.pyx":152
+ * 
+ * cdef set _lexer_data_names = {
+ *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
+ * }
+ */
+    __pyx_t_2 = PyObject_Dir(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
+      __pyx_t_4 = __pyx_t_2; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+      __pyx_t_6 = NULL;
+    } else {
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 152, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 152, __pyx_L4_error)
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_6)) {
+        if (likely(PyList_CheckExact(__pyx_t_4))) {
+          if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(1, 152, __pyx_L4_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(1, 152, __pyx_L4_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_6(__pyx_t_4);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(1, 152, __pyx_L4_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XGOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
+      __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, __pyx_t_2);
+      __Pyx_GIVEREF(__pyx_t_2);
+      __pyx_t_2 = 0;
+
+      /* "kola/lexer.pyx":153
+ * cdef set _lexer_data_names = {
+ *     i for i in dir(LexerConfig)
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))             # <<<<<<<<<<<<<<
+ * }
+ * 
+ */
+      if (unlikely(__pyx_7genexpr__pyx_v_4kola_5lexer_i == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
+        __PYX_ERR(1, 153, __pyx_L4_error)
+      }
+      __pyx_t_8 = __Pyx_PyUnicode_Tailmatch(((PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i), __pyx_n_u__14, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 153, __pyx_L4_error)
+      __pyx_t_9 = ((!(__pyx_t_8 != 0)) != 0);
+      if (__pyx_t_9) {
+      } else {
+        __pyx_t_7 = __pyx_t_9;
+        goto __pyx_L8_bool_binop_done;
+      }
+      if (unlikely(__pyx_7genexpr__pyx_v_4kola_5lexer_i == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "endswith");
+        __PYX_ERR(1, 153, __pyx_L4_error)
+      }
+      __pyx_t_9 = __Pyx_PyUnicode_Tailmatch(((PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i), __pyx_n_u__14, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 153, __pyx_L4_error)
+      __pyx_t_8 = ((!(__pyx_t_9 != 0)) != 0);
+      if (__pyx_t_8) {
+      } else {
+        __pyx_t_7 = __pyx_t_8;
+        goto __pyx_L8_bool_binop_done;
+      }
+      __pyx_t_2 = __pyx_7genexpr__pyx_v_4kola_5lexer_i;
+      __Pyx_INCREF(__pyx_t_2);
+      __pyx_t_10 = __Pyx_GetAttr(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 153, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_8 = (PyDescr_IsData(__pyx_t_10) != 0);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_7 = __pyx_t_8;
+      __pyx_L8_bool_binop_done:;
+      if (__pyx_t_7) {
+
+        /* "kola/lexer.pyx":152
+ * 
+ * cdef set _lexer_data_names = {
+ *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
+ * }
+ */
+        if (unlikely(PySet_Add(__pyx_t_3, (PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i))) __PYX_ERR(1, 152, __pyx_L4_error)
+
+        /* "kola/lexer.pyx":153
+ * cdef set _lexer_data_names = {
+ *     i for i in dir(LexerConfig)
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))             # <<<<<<<<<<<<<<
+ * }
+ * 
+ */
+      }
+
+      /* "kola/lexer.pyx":152
+ * 
+ * cdef set _lexer_data_names = {
+ *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
+ *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
+ * }
+ */
+    }
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, Py_None);
+    goto __pyx_L11_exit_scope;
+    __pyx_L4_error:;
+    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
+    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, Py_None);
+    goto __pyx_L1_error;
+    __pyx_L11_exit_scope:;
+  } /* exit inner scope */
+  __Pyx_XGOTREF(__pyx_v_4kola_5lexer__lexer_data_names);
+  __Pyx_DECREF_SET(__pyx_v_4kola_5lexer__lexer_data_names, ((PyObject*)__pyx_t_3));
+  __Pyx_GIVEREF(__pyx_t_3);
+  __pyx_t_3 = 0;
+
+  /* "kola/lexer.pyx":157
+ * 
+ * # update LexerConfig.attr_names
+ * (<dict>(<PyTypeObject*>LexerConfig).tp_dict)["data_names"] = frozenset(_lexer_data_names)             # <<<<<<<<<<<<<<
+ * PyType_Modified(LexerConfig)
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyFrozenSet_New(__pyx_v_4kola_5lexer__lexer_data_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (unlikely(((PyObject *)((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig)->tp_dict) == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 157, __pyx_L1_error)
+  }
+  if (unlikely((PyDict_SetItem(((PyObject*)((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig)->tp_dict), __pyx_n_u_data_names, __pyx_t_3) < 0))) __PYX_ERR(1, 157, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "kola/lexer.pyx":158
+ * # update LexerConfig.attr_names
+ * (<dict>(<PyTypeObject*>LexerConfig).tp_dict)["data_names"] = frozenset(_lexer_data_names)
+ * PyType_Modified(LexerConfig)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  PyType_Modified(((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig));
+
+  /* "kola/lexer.pyx":183
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_7close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_7close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 170, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
-  /* "kola/lexer.pyx":263
+  /* "kola/lexer.pyx":276
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_13__enter__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___enter, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 263, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_13__enter__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___enter, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_enter, __pyx_t_3) < 0) __PYX_ERR(1, 263, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_enter, __pyx_t_3) < 0) __PYX_ERR(1, 276, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
-  /* "kola/lexer.pyx":266
+  /* "kola/lexer.pyx":279
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_15__exit__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___exit, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 266, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_15__exit__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___exit, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_exit, __pyx_t_3) < 0) __PYX_ERR(1, 266, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_exit, __pyx_t_3) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11815,24 +11897,24 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_21__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":300
+  /* "kola/lexer.pyx":316
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9FileLexer_3close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FileLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 300, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9FileLexer_3close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FileLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_FileLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 300, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_FileLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 316, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_FileLexer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11894,14 +11976,16 @@
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_10);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init kola.lexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #endif
@@ -12894,76 +12978,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* RaiseUnexpectedTypeError */
-static int
-__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
-{
-    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
-                 expected, obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
-/* decode_c_bytes */
-static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
-         const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
-         const char* encoding, const char* errors,
-         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
-    if (unlikely((start < 0) | (stop < 0))) {
-        if (start < 0) {
-            start += length;
-            if (start < 0)
-                start = 0;
-        }
-        if (stop < 0)
-            stop += length;
-    }
-    if (stop > length)
-        stop = length;
-    if (unlikely(stop <= start))
-        return __Pyx_NewRef(__pyx_empty_unicode);
-    length = stop - start;
-    cstring += start;
-    if (decode_func) {
-        return decode_func(cstring, length, errors);
-    } else {
-        return PyUnicode_Decode(cstring, length, encoding, errors);
-    }
-}
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
         if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
@@ -12991,14 +13013,78 @@
             return -1;
         }
     }
     return 0;
 #endif
 }
 
+/* set_iter */
+static CYTHON_INLINE PyObject* __Pyx_set_iterator(PyObject* iterable, int is_set,
+                                                  Py_ssize_t* p_orig_length, int* p_source_is_set) {
+#if CYTHON_COMPILING_IN_CPYTHON
+    is_set = is_set || likely(PySet_CheckExact(iterable) || PyFrozenSet_CheckExact(iterable));
+    *p_source_is_set = is_set;
+    if (likely(is_set)) {
+        *p_orig_length = PySet_Size(iterable);
+        Py_INCREF(iterable);
+        return iterable;
+    }
+#else
+    (void)is_set;
+    *p_source_is_set = 0;
+#endif
+    *p_orig_length = 0;
+    return PyObject_GetIter(iterable);
+}
+static CYTHON_INLINE int __Pyx_set_iter_next(
+        PyObject* iter_obj, Py_ssize_t orig_length,
+        Py_ssize_t* ppos, PyObject **value,
+        int source_is_set) {
+    if (!CYTHON_COMPILING_IN_CPYTHON || unlikely(!source_is_set)) {
+        *value = PyIter_Next(iter_obj);
+        if (unlikely(!*value)) {
+            return __Pyx_IterFinish();
+        }
+        (void)orig_length;
+        (void)ppos;
+        return 1;
+    }
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (unlikely(PySet_GET_SIZE(iter_obj) != orig_length)) {
+        PyErr_SetString(
+            PyExc_RuntimeError,
+            "set changed size during iteration");
+        return -1;
+    }
+    {
+        Py_hash_t hash;
+        int ret = _PySet_NextEntry(iter_obj, ppos, value, &hash);
+        assert (ret != -1);
+        if (likely(ret)) {
+            Py_INCREF(*value);
+            return 1;
+        }
+    }
+#endif
+    return 0;
+}
+
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
     PyObject *arg = NULL;
     return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
@@ -13318,14 +13404,68 @@
         *pkey = next_item;
     } else {
         *pvalue = next_item;
     }
     return 1;
 }
 
+/* pyfrozenset_new */
+static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it) {
+    if (it) {
+        PyObject* result;
+#if CYTHON_COMPILING_IN_PYPY
+        PyObject* args;
+        args = PyTuple_Pack(1, it);
+        if (unlikely(!args))
+            return NULL;
+        result = PyObject_Call((PyObject*)&PyFrozenSet_Type, args, NULL);
+        Py_DECREF(args);
+        return result;
+#else
+        if (PyFrozenSet_CheckExact(it)) {
+            Py_INCREF(it);
+            return it;
+        }
+        result = PyFrozenSet_New(it);
+        if (unlikely(!result))
+            return NULL;
+        if ((PY_VERSION_HEX >= 0x031000A1) || likely(PySet_GET_SIZE(result)))
+            return result;
+        Py_DECREF(result);
+#endif
+    }
+#if CYTHON_USE_TYPE_SLOTS
+    return PyFrozenSet_Type.tp_new(&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
+#else
+    return PyObject_Call((PyObject*)&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
+#endif
+}
+
+/* PySetContains */
+static int __Pyx_PySet_ContainsUnhashable(PyObject *set, PyObject *key) {
+    int result = -1;
+    if (PySet_Check(key) && PyErr_ExceptionMatches(PyExc_TypeError)) {
+        PyObject *tmpkey;
+        PyErr_Clear();
+        tmpkey = __Pyx_PyFrozenSet_New(key);
+        if (tmpkey != NULL) {
+            result = PySet_Contains(set, tmpkey);
+            Py_DECREF(tmpkey);
+        }
+    }
+    return result;
+}
+static CYTHON_INLINE int __Pyx_PySet_ContainsTF(PyObject* key, PyObject* set, int eq) {
+    int result = PySet_Contains(set, key);
+    if (unlikely(result < 0)) {
+        result = __Pyx_PySet_ContainsUnhashable(set, key);
+    }
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
@@ -13466,14 +13606,25 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -14226,15 +14377,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__3);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__2);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -15292,14 +15443,43 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
+/* unicode_tailmatch */
+static int __Pyx_PyUnicode_TailmatchTuple(PyObject* s, PyObject* substrings,
+                                          Py_ssize_t start, Py_ssize_t end, int direction) {
+    Py_ssize_t i, count = PyTuple_GET_SIZE(substrings);
+    for (i = 0; i < count; i++) {
+        Py_ssize_t result;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        result = PyUnicode_Tailmatch(s, PyTuple_GET_ITEM(substrings, i),
+                                     start, end, direction);
+#else
+        PyObject* sub = PySequence_ITEM(substrings, i);
+        if (unlikely(!sub)) return -1;
+        result = PyUnicode_Tailmatch(s, sub, start, end, direction);
+        Py_DECREF(sub);
+#endif
+        if (result) {
+            return (int) result;
+        }
+    }
+    return 0;
+}
+static int __Pyx_PyUnicode_Tailmatch(PyObject* s, PyObject* substr,
+                                     Py_ssize_t start, Py_ssize_t end, int direction) {
+    if (unlikely(PyTuple_Check(substr))) {
+        return __Pyx_PyUnicode_TailmatchTuple(s, substr, start, end, direction);
+    }
+    return (int) PyUnicode_Tailmatch(s, substr, start, end, direction);
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -15541,33 +15721,14 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-static PyObject* __pyx_convert__to_py_LexerData(LexerData s) {
-  PyObject* res;
-  PyObject* member;
-  res = __Pyx_PyDict_NewPresized(3); if (unlikely(!res)) return NULL;
-  member = __Pyx_PyObject_FromString(s.filename); if (unlikely(!member)) goto bad;
-  if (unlikely(PyDict_SetItem(res, __pyx_n_s_filename, member) < 0)) goto bad;
-  Py_DECREF(member);
-  member = __Pyx_PyInt_From_uint8_t(s.command_threshold); if (unlikely(!member)) goto bad;
-  if (unlikely(PyDict_SetItem(res, __pyx_n_s_command_threshold, member) < 0)) goto bad;
-  Py_DECREF(member);
-  member = __Pyx_PyInt_From_uint8_t(s.flag); if (unlikely(!member)) goto bad;
-  if (unlikely(PyDict_SetItem(res, __pyx_n_s_flag, member) < 0)) goto bad;
-  Py_DECREF(member);
-  return res;
-  bad:
-  Py_XDECREF(member);
-  Py_DECREF(res);
-  return NULL;
-}
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__TokenSyn(enum TokenSyn value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum TokenSyn neg_one = (enum TokenSyn) -1, const_zero = (enum TokenSyn) 0;
```

### Comparing `KoiLang-1.1.0b2/kola/lexer.pxd` & `KoiLang-1.1.1/kola/lexer.pxd`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-cimport cython
-from libc.stdio cimport stdin, FILE, fopen, fclose, EOF
-from cpython cimport PyObject
-
-from ._cutil cimport *
-
-
-cdef class Token:
-    cdef:
-        Token next     # used in grammar parser
-    cdef readonly:
-        TokenSyn syn
-        object val
-        bytes raw_val
-        int lineno
-    
-    cpdef int get_flag(self)
-
-
-cdef class LexerConfig:
-    cdef LexerData* lexer_data
-    cdef readonly BaseLexer lexer
-
-
-@cython.no_gc
-cdef class BaseLexer:
-    cdef:
-        yyscan_t scanner
-        LexerData lexer_data
-    cdef readonly:
-        str encoding
-
-    cpdef void close(self)
-    cdef void set_error(self, const char* text) except *
-    cdef (int, const char*, Py_ssize_t) next_syn(self) nogil
-    cdef Token next_token(self)
-
-
-cdef class FileLexer(BaseLexer):
-    cdef:
-        object _filenameo
-        bytes _filenameb
-        FILE* fp
-    
-    cpdef void close(self)
-
-
-@cython.no_gc
-cdef class StringLexer(BaseLexer):
+cimport cython
+from libc.stdio cimport stdin, FILE, fopen, fclose, EOF
+from cpython cimport PyObject
+
+from ._cutil cimport *
+
+
+cdef extern from *:
+    bint PyDescr_IsData(object desc)
+
+
+cdef class Token:
+    cdef:
+        Token next     # used in grammar parser
+    cdef readonly:
+        TokenSyn syn
+        object val
+        bytes raw_val
+        int lineno
+    
+    cpdef int get_flag(self)
+
+
+cdef class LexerConfig:
+    cdef LexerData* lexer_data
+    cdef readonly BaseLexer lexer
+
+
+@cython.no_gc
+cdef class BaseLexer:
+    cdef:
+        yyscan_t scanner
+        LexerData lexer_data
+    cdef readonly:
+        str encoding
+
+    cpdef void close(self)
+    cdef void set_error(self, const char* text) except *
+    cdef (int, const char*, Py_ssize_t) next_syn(self) nogil
+    cdef Token next_token(self)
+
+
+cdef class FileLexer(BaseLexer):
+    cdef:
+        object _filenameo
+        bytes _filenameb
+        FILE* fp
+    
+    cpdef void close(self)
+
+
+@cython.no_gc
+cdef class StringLexer(BaseLexer):
     cdef readonly bytes content
```

### Comparing `KoiLang-1.1.0b2/kola/lexer.pyi` & `KoiLang-1.1.1/kola/writer.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,71 @@
-import os
-from typing import Any, Final, Union, final, TypedDict
-from typing_extensions import Self
-
-
-S_CMD: int
-S_CMD_N: int
-S_TEXT: int
-S_LITERAL: int
-S_STRING: int
-S_NUM: int
-S_NUM_H: int
-S_NUM_B: int
-S_NUM_F: int
-S_CLN: int
-S_CMA: int
-S_SLP: int
-S_SRP: int
-S_ANNOTATION: int
-F_DISABLED: int
-F_LSTRIP_TEXT: int
-
-
-class _LexerData(TypedDict):
-    filename: str
-    encoding: str
-    command_threshold: int
-    flag: int
-
-
-@final
-class Token:
-    """
-    Token used in lexer
-
-    Don't instantiate this class directly unless you make
-    sure enough arguments provided.
-    """
-
-    syn: Final[int]
-    val: Final[Any]
-
-    def __new__(cls, syn: int, val: Any = ..., *, lineno: int = ..., raw_val: bytes = ...) -> Self: ...
-    def get_flag(self) -> int: ...
-
-
-class LexerConfig:
-    """
-    Python-level interface to access extra lexer data
-    """
-    def __init__(self, lexer: BaseLexer) -> None: ...
-    def dict(self) -> _LexerData: ...
-    def set(
-        self,
-        *,
-        encoding: str = ...,
-        command_threshold: int = ...,
-        flag: int = ...,
-        disabled: bool = ...,
-        no_lstrip: bool = ...
-    ) -> None: ...
-    @property
-    def filename(self) -> str: ...
-    @property
-    def encoding(self) -> str: ...
-    @encoding.setter
-    def encoding(self, val: str) -> None: ...
-    @property
-    def command_threshold(self) -> int: ...
-    @command_threshold.setter
-    def command_threshold(self, cmd_threshold: int) -> None: ...    
-    @property
-    def flag(self) -> int: ...
-    @flag.setter
-    def flag(self, val: int) -> None: ...
-    @property
-    def disabled(self) -> bool: ...
-    @disabled.setter
-    def disabled(self, val: bool) -> None: ...
-    @property
-    def no_lstrip(self) -> bool: ...
-    @no_lstrip.setter
-    def no_lstrip(self, val: bool) -> None: ...
-
-
-class BaseLexer:
-    def __init__(self, *, encoding: str = ..., command_threshold: int = 1, no_lstrip: bool = ...) -> None: ...
-    def close(self) -> None: ...
-    @property
-    def filename(self) -> str: ...
-    @property
-    def lineno(self) -> int: ...
-    @property
-    def column(self) -> int: ...
-    @property
-    def config(self) -> LexerConfig: ...
-    @property
-    def closed(self) -> bool: ...
-    def __iter__(self) -> Self: ...
-    def __next__(self) -> Token: ...
-    def __enter__(self) -> Self: ...
-    def __exit__(self, *args) -> None: ...
-
-
-class FileLexer(BaseLexer):
-    def __init__(self, __path: Union[str, bytes, os.PathLike], *, encoding: str = ...,
-                 command_threshold: int = 1, no_lstrip: bool = ...) -> None: ...
-    @property
-    def filename(self) -> Union[str, bytes, os.PathLike]: ...
-
-
-class StringLexer(BaseLexer):
-    content: Final[bytes]
-
-    def __init__(self, content: Union[str, bytes], *, encoding: str = ...,
-                 command_threshold: int = 1, no_lstrip: bool = ...) -> None: ...
+import os
+from types import TracebackType
+from typing import Any, Dict, Final, List, Type, Union
+from typing_extensions import Protocol, runtime_checkable, Self
+
+
+WF_BASE_ITEM: int
+WF_COMPLEX_ITEM: int
+WF_ARG_ITEM: int
+WF_FULL_CMD: int
+
+
+@runtime_checkable
+class WriterItemLike(Protocol):
+    def __kola_write__(self, __writer: BaseWriter, __level: int) -> None: ...
+
+
+class BaseWriterItem(object):
+    def __kola_write__(self, writer: BaseWriter, level: int) -> None: ...
+
+
+class FormatItem(BaseWriterItem):
+    value: Final[Any]
+    spec: Final[str]
+
+    def __init__(self, value: Any, spec: str) -> None: ...
+
+
+class ComplexArg(BaseWriterItem):
+    name: Final[str]
+    value: Final[Any]
+
+    def __init__(self, name: str, value: Any, *, split_line: bool = ...) -> None: ...
+
+
+WI_NEWLINE: BaseWriterItem
+
+
+_BaseItem = Union[str, bytes, int, float, WriterItemLike]
+_ComplexItem = Union[_BaseItem, List[_BaseItem], Dict[str, _BaseItem]]
+
+
+class BaseWriter(object):
+    indent: Final[int]
+
+    def __init__(self, indent: int = 4, command_threshold: int = 1) -> None: ...
+    def raw_write(self, text: str) -> None: ...
+    def close(self) -> None: ...
+    def inc_indent(self) -> None: ...
+    def dec_indent(self) -> None: ...
+    def newline(self, concat_prev: bool = ...) -> None: ...
+    def write_text(self, text: str) -> None: ...
+    def write_annotation(self, annotation: str) -> None: ...
+    def write_command(self, __name: Union[str, int], *args: _BaseItem, **kwds: _ComplexItem) -> None: ...
+    def write(self, command: Union[str, WriterItemLike]) -> None: ...
+    @property
+    def closed(self) -> bool: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, exc_type: Type[BaseException], exc_ins: Exception, traceback: TracebackType) -> None: ...
+
+
+class FileWriter(BaseWriter):
+    path: Final[Union[str, bytes, os.PathLike]]
+    encoding: Final[str]
+
+    def __init__(self, __path: Union[str, bytes, os.PathLike], encoding: str = "utf-8",
+                 indent: int = ..., command_threshold: int = ...) -> None: ...
+
+
+class StringWriter(BaseWriter):
+    def getvalue(self) -> str: ...
```

### Comparing `KoiLang-1.1.0b2/kola/lib/__init__.py` & `KoiLang-1.1.1/kola/lib/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,117 @@
-import inspect
-import os
-import re
-import sys
-from glob import glob
-from importlib.util import spec_from_file_location
-from importlib._bootstrap import _load
-from types import ModuleType
-from typing import List, NamedTuple, Optional, Type
-
-from ..klvm import CommandSetMeta, KoiLang
-
-
-if "KOLA_LIB_PATH" in os.environ:
-    KOLA_LIB_PATH = os.environ["KOLA_LIB_PATH"].split(os.pathsep)
-else:
-    KOLA_LIB_PATH = ['.', './kola_lib', os.path.dirname(__file__)]
-
-
-_module_pattern = re.compile(r"^[A-Za-z_]\w*(?:\.[A-Za-z_]\w*)*$", re.A)
-
-
-class KolaSpec(NamedTuple):
-    name: str
-    command_set_classes: List[CommandSetMeta]
-    
-    doc: Optional[str] = None
-    main_class: Optional[Type[KoiLang]] = None
-
-
-def collect_all() -> List[CommandSetMeta]:
-    frame = inspect.currentframe()
-    assert frame and frame.f_back
-    return [
-        i for i in frame.f_back.f_locals.values()
-        if isinstance(i, CommandSetMeta)
-    ]
-
-
-def load_library(name: str, bases: List[str] = KOLA_LIB_PATH) -> ModuleType:
-    if not _module_pattern.match(name):
-        raise ValueError(f"illegal module name '{name}'")
-    module_name = "kola.lib." + name
-    if module_name in sys.modules:
-        return sys.modules[module_name]
-
-    for b in bases:
-        spec = None
-        b = os.path.abspath(b)
-        full_path = os.path.join(b, name)
-        if os.path.isfile(full_path):
-            spec = spec_from_file_location(module_name, full_path)
-        elif os.path.isdir(full_path):
-            spec = spec_from_file_location(
-                module_name, os.path.join(full_path, "__init__.py"),
-                submodule_search_locations=[full_path]
-            )
-        else:
-            for i in glob(full_path + '.*'):
-                spec = spec_from_file_location(module_name, i)
-                if spec:
-                    full_path = i
-                    break
-        if spec:
-            spec.name = module_name
-            return _load(spec)
-    raise ImportError(f"cannot load script {name}", name=name)
-
-
-def main_class_from_module(module: ModuleType) -> Type[KoiLang]:
-    spec = getattr(module, "__kola_spec__", None)
-    if spec:
-        if not isinstance(spec, KolaSpec):
-            spec = KolaSpec(*spec)
-        if spec.main_class:
-            return spec.main_class
-        for i in spec.command_set_classes:
-            if issubclass(i, KoiLang):
-                return i
-    else:
-        for i in module.__dict__.values():
-            if isinstance(i, type) and issubclass(i, KoiLang) and i is not KoiLang:
-                return i
-    raise ValueError(
-        f"no available main class for kola module '{spec.name if spec else module.__name__}'"
-    )
+"""
+Kola sub libraries support modules
+
+Include some useful builtin kola sub module.
+And modules imported from `load_library()` will be mounted as a sub module.
+"""
+
+import inspect
+import os
+import re
+import sys
+from glob import glob
+from importlib.util import spec_from_file_location
+from importlib._bootstrap import _load
+from types import ModuleType
+from typing import List, NamedTuple, Optional, Type
+
+from ..klvm import CommandSetMeta, KoiLang
+
+
+if "KOLA_LIB_PATH" in os.environ:  # pragma: no cover
+    KOLA_LIB_PATH = os.environ["KOLA_LIB_PATH"].split(os.pathsep)
+else:
+    KOLA_LIB_PATH = ['.', './kola_lib', os.path.dirname(__file__)]
+
+
+_module_pattern = re.compile(r"^[A-Za-z_]\w*(?:\.[A-Za-z_]\w*)*$", re.A)
+
+
+class KolaSpec(NamedTuple):
+    """
+    Kola module spec
+    
+    Usage:
+        __kola_spec__ = KolaSpec(
+            __name__,
+            collect_all()
+        )
+    """
+    name: str
+    command_set_classes: List[CommandSetMeta]
+    
+    doc: Optional[str] = None
+    main_class: Optional[Type[KoiLang]] = None
+
+
+def collect_all() -> List[CommandSetMeta]:
+    """get all CommandSet class defined in the module
+
+    :return: a list of CommandSet class found
+    :rtype: List[CommandSetMeta]
+    """
+    frame = inspect.currentframe()
+    if not frame or not frame.f_back:  # pragma: no cover
+        raise ValueError("cannot read variables from the frame")
+    return [
+        i for i in frame.f_back.f_locals.values()
+        if isinstance(i, CommandSetMeta)
+    ]
+
+
+def load_library(name: str, paths: List[str] = KOLA_LIB_PATH) -> ModuleType:
+    """load a Phython script or package as a Kola module
+
+    :param name: module name like 'mymodule.sub'
+    :type name: str
+    :param paths: base path to load the module, defaults to KOLA_LIB_PATH
+    :type paths: List[str], optional
+    :raises ValueError: illegal module name
+    :raises ImportError: fail to load the module
+    :return: the Kola module
+    :rtype: ModuleType
+    """
+    if not _module_pattern.match(name):  # pragma: no cover
+        raise ValueError(f"illegal module name '{name}'")
+    module_name = "kola.lib." + name
+    if module_name in sys.modules:
+        return sys.modules[module_name]
+
+    for b in paths:
+        spec = None
+        b = os.path.abspath(b)
+        full_path = os.path.join(b, name)
+        if os.path.isdir(full_path):
+            spec = spec_from_file_location(
+                module_name, os.path.join(full_path, "__init__.py"),
+                submodule_search_locations=[full_path]
+            )
+        else:
+            for i in glob(full_path + '.*'):
+                spec = spec_from_file_location(module_name, i)
+                if spec:
+                    full_path = i
+                    break
+        if spec:
+            spec.name = module_name
+            return _load(spec)
+    raise ImportError(f"cannot load script {name}", name=name)  # pragma: no cover
+
+
+def main_class_from_module(module: ModuleType) -> Type[KoiLang]:
+    spec = getattr(module, "__kola_spec__", None)
+    if spec:
+        if not isinstance(spec, KolaSpec):
+            spec = KolaSpec(*spec)
+        if spec.main_class:
+            return spec.main_class
+        for i in spec.command_set_classes:
+            if issubclass(i, KoiLang):
+                return i
+    else:
+        for i in module.__dict__.values():
+            if isinstance(i, type) and issubclass(i, KoiLang) and i is not KoiLang:
+                return i
+    raise ValueError(  # pragma: no cover
+        f"no available main class for kola module '{spec.name if spec else module.__name__}'"
+    )
```

### Comparing `KoiLang-1.1.0b2/kola/lib/debugger/base.py` & `KoiLang-1.1.1/kola/lib/debugger/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import sys
-from types import TracebackType
-from typing import Optional, Type
-from traceback import print_exception
-
-from kola import __version__
-from kola.klvm import KoiLang, kola_command
-
-
-class BaseDebugger(KoiLang):
-    """
-    provide unified version checking and error suppression functions
-    """
-    __slots__ = []
-
-    @kola_command
-    def version(self, __chk_ver: Optional[int] = None) -> None:
-        if __chk_ver is None:
-            print(__version__)
-        elif __chk_ver != 100:
-            print(f"version {__chk_ver} is not support by runner {__version__}")
-            sys.exit(2)
-
-    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> bool:
-        super().on_exception(exc_type, exc_ins, traceback)
-        print_exception(exc_type, exc_ins, traceback)
-        return True
+import sys
+from types import TracebackType
+from typing import Optional, Type
+from traceback import print_exception
+
+from kola import __version__
+from kola.klvm import KoiLang, kola_command
+
+
+class BaseDebugger(KoiLang):
+    """
+    provide unified version checking and error suppression functions
+    """
+    __slots__ = []
+
+    @kola_command
+    def version(self, __chk_ver: Optional[int] = None) -> None:
+        if __chk_ver is None:
+            print(__version__)
+        elif __chk_ver < 100 or __chk_ver > 120:
+            print(f"version {__chk_ver} is not support by runner {__version__}")
+            sys.exit(2)
+
+    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> bool:
+        super().on_exception(exc_type, exc_ins, traceback)
+        print_exception(exc_type, exc_ins, traceback)
+        return True
```

### Comparing `KoiLang-1.1.0b2/kola/lib/debugger/default_runner.py` & `KoiLang-1.1.1/kola/lib/debugger/default_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""
-Copyright 2023 Ovizro
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-import os
-import re
-import sys
-from types import ModuleType
-from typing import Any, Dict, List, Optional, TypeVar, Union
-from typing_extensions import Literal
-
-from kola.exception import KoiLangCommandError
-from kola.klvm import Environment, kola_command, kola_text
-from kola.lib import KOLA_LIB_PATH, KolaSpec, collect_all, load_library, main_class_from_module
-from kola.lib.debugger.base import BaseDebugger
-
-
-T = TypeVar("T")
-
-
-FLAG_DEBUG = 1
-
-
-class KoiLangRunner(BaseDebugger):
-    """
-    default class for KoiLang module runner
-    """
-
-    var_pattern = re.compile(r"\$(\{)?(?P<name>[a-zA-Z_]\w*)(?(1)\}|)", re.ASCII)
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.flag = 0
-
-    @kola_command
-    def license(self) -> None:
-        print(__doc__)
-    
-    @kola_command(alias="raise")
-    def raises(self, *msg: str) -> None:
-        raise KoiLangCommandError(*msg)
-    
-    @kola_command
-    def pragma(self, *, debug: Optional[Literal["on", "off"]] = None) -> None:
-        if debug:
-            if debug == "on":
-                self.flag |= FLAG_DEBUG
-            elif debug == "off":
-                self.flag &= ~FLAG_DEBUG
-            else:
-                raise ValueError(f"illegal value '{debug}'")
-    
-    @kola_command
-    def echo(self, *text: str) -> None:
-        print(' '.join(text))
-    
-    @kola_command
-    def execute(self, source: str) -> None:
-        code = compile(source, "<kola_runner>", "single")
-        exec(code, {"kola_runner": self, "__vars__": self.vars})
-    
-    @kola_command(alias="export")
-    def set(self, **kwds) -> None:
-        self.vars.update(kwds)
-    
-    @kola_command
-    def exit(self, code: int = 0) -> None:
-        sys.exit(code)
-        
-    @kola_text
-    def text(self, text: str) -> None:
-        print(f"## [TEXT] {text}")
-    
-    @kola_command
-    def load(self, path: Union[str, bytes, os.PathLike], type: Optional[str] = None, **kwds: Any) -> None:
-        path = os.fsdecode(path)
-        if type is None:
-            if path.endswith(".kola"):
-                type = "kola"
-            else:
-                type = "script"
-        else:
-            type = type.lower()
-        if type == "kola":
-            self.load_kola(path, **kwds)
-        elif type in ["script", "lib"]:
-            self.load_script(path, **kwds)
-        else:
-            raise ValueError(f"invalid type name '{type}'")
-    
-    @kola_command
-    def load_kola(self, path: Union[str, bytes, os.PathLike], *, encoding: str = "utf-8", **kwds) -> None:
-        self.parse_file(path, encoding=encoding, **kwds)
-    
-    @kola_command(alias=["load_lib", "load_library"])
-    def load_script(self, name: str, lib_path: Optional[List[str]] = None) -> None:
-        kola_module = load_library(name, bases=lib_path or KOLA_LIB_PATH)
-        self.load_command_set(kola_module)
-    
-    def at_start(self) -> None:
-        self.vars = {}
-        self.flag = 0
-        self.loaded_class = set()
-    
-    def at_end(self) -> None:
-        super().at_end()
-        for i in self.loaded_class:
-            i.at_end(self)
-    
-    def get_var(self, key: str) -> Any:
-        if key == '__top__':
-            return self.top.__class__.__name__
-        elif key == "__dir__":
-            return ', '.join(self.raw_command_set)
-        elif key == "__name__":
-            return self.__class__.__name__
-        elif key == "__stack_info__":
-            env_names = []
-            top = self.top
-            while top is not self:
-                env_names.append(top.__class__.__name__)
-                top = top.back  # type: ignore
-            env_names.append("__init__")
-            return " -> ".join(env_names)
-        else:
-            return self.vars.get(key, None)
-    
-    def load_command_set(self, module: ModuleType) -> None:
-        cls = main_class_from_module(module)
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Load class: {cls}")
-        self.loaded_class.add(cls)
-        cls.at_start(self)
-        self.raw_command_set.update(
-            cls.generate_raw_commands()
-        )
-    
-    def format_text(self, argument: T) -> T:
-        if isinstance(argument, list):
-            return [self.format_text(i) for i in argument]  # type: ignore
-        elif isinstance(argument, dict):
-            return {k: self.format_text(v) for k, v in argument.items()}  # type: ignore
-        elif isinstance(argument, str):
-            return self.var_pattern.sub(
-                lambda match: str(self.get_var(match.group("name")) or ''),
-                argument
-            )
-        return argument
-    
-    def __kola_caller__(
-            self, command: Any, args: tuple, kwargs: Dict[str, Any],
-            *, bound_instance: Any = None, **kwds: Any) -> Any:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Run command: {command.__name__} ({(bound_instance or self).__class__.__name__})")
-        return super().__kola_caller__(
-            command,
-            tuple(self.format_text(i) for i in args),
-            self.format_text(kwargs),
-            bound_instance=bound_instance,
-            **kwds
-        )
-    
-    def push_end(self, __push_cache: Environment) -> None:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Push env: {__push_cache}")
-        return super().push_end(__push_cache)
-    
-    def pop_end(self, __env_cache: Environment) -> None:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Pop env: {__env_cache}")
-        return super().pop_end(__env_cache)
-
-
-__kola_spec__ = KolaSpec(
-    "Kola Runner",
-    collect_all(),
-    main_class=KoiLangRunner
-)
+"""
+Copyright 2023 Ovizro
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+import os
+import re
+import sys
+from types import ModuleType
+from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing_extensions import Literal
+
+from kola.exception import KoiLangCommandError
+from kola.klvm import Environment, kola_command, kola_text
+from kola.lib import KOLA_LIB_PATH, KolaSpec, collect_all, load_library, main_class_from_module
+from kola.lib.debugger.base import BaseDebugger
+
+
+T = TypeVar("T")
+
+
+FLAG_DEBUG = 1
+
+
+class KoiLangRunner(BaseDebugger):
+    """
+    default class for KoiLang module runner
+    """
+
+    var_pattern = re.compile(r"\$(\{)?(?P<name>[a-zA-Z_]\w*)(?(1)\}|)", re.ASCII)
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.flag = 0
+
+    @kola_command
+    def license(self) -> None:
+        print(__doc__)
+    
+    @kola_command(alias="raise")
+    def raises(self, *msg: str) -> None:
+        raise KoiLangCommandError(*msg)
+    
+    @kola_command
+    def pragma(self, *, debug: Optional[Literal["on", "off"]] = None) -> None:
+        if debug:
+            if debug == "on":
+                self.flag |= FLAG_DEBUG
+            elif debug == "off":
+                self.flag &= ~FLAG_DEBUG
+            else:
+                raise ValueError(f"illegal value '{debug}'")
+    
+    @kola_command
+    def echo(self, *text: str) -> None:
+        print(' '.join(text))
+    
+    @kola_command
+    def execute(self, source: str) -> None:
+        code = compile(source, "<kola_runner>", "single")
+        exec(code, {"kola_runner": self, "__vars__": self.vars})
+    
+    @kola_command(alias="export")
+    def set(self, **kwds) -> None:
+        self.vars.update(kwds)
+    
+    @kola_command
+    def exit(self, code: int = 0) -> None:
+        sys.exit(code)
+        
+    @kola_text
+    def text(self, text: str) -> None:
+        print(f"## [TEXT] {text}")
+    
+    @kola_command
+    def load(self, path: Union[str, bytes, os.PathLike], type: Optional[str] = None, **kwds: Any) -> None:
+        path = os.fsdecode(path)
+        if type is None:
+            if path.endswith(".kola"):
+                type = "kola"
+            else:
+                type = "script"
+        else:
+            type = type.lower()
+        if type == "kola":
+            self.load_kola(path, **kwds)
+        elif type in ["script", "lib"]:
+            self.load_script(path, **kwds)
+        else:
+            raise ValueError(f"invalid type name '{type}'")
+    
+    @kola_command
+    def load_kola(self, path: Union[str, bytes, os.PathLike], *, encoding: str = "utf-8", **kwds) -> None:
+        self.parse_file(path, encoding=encoding, **kwds)
+    
+    @kola_command(alias=["load_lib", "load_library"])
+    def load_script(self, name: str, lib_path: Optional[List[str]] = None) -> None:
+        kola_module = load_library(name, lib_path or KOLA_LIB_PATH)
+        self.load_command_set(kola_module)
+    
+    def at_start(self) -> None:
+        self.vars = {}
+        self.flag = 0
+        self.loaded_class = set()
+    
+    def at_end(self) -> None:
+        super().at_end()
+        for i in self.loaded_class:
+            i.at_end(self)
+    
+    def get_var(self, key: str) -> Any:
+        if key == '__top__':
+            return self.top.__class__.__name__
+        elif key == "__dir__":
+            return ', '.join(self.raw_command_set)
+        elif key == "__name__":
+            return self.__class__.__name__
+        elif key == "__stack_info__":
+            env_names = []
+            top = self.top
+            while top is not self:
+                env_names.append(top.__class__.__name__)
+                top = top.back  # type: ignore
+            env_names.append("__init__")
+            return " -> ".join(env_names)
+        else:
+            return self.vars.get(key, None)
+    
+    def load_command_set(self, module: ModuleType) -> None:
+        cls = main_class_from_module(module)
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Load class: {cls}")
+        self.loaded_class.add(cls)
+        cls.at_start(self)
+        self.raw_command_set.update(
+            cls.generate_raw_commands()
+        )
+    
+    def format_text(self, argument: T) -> T:
+        if isinstance(argument, list):
+            return [self.format_text(i) for i in argument]  # type: ignore
+        elif isinstance(argument, dict):
+            return {k: self.format_text(v) for k, v in argument.items()}  # type: ignore
+        elif isinstance(argument, str):
+            return self.var_pattern.sub(
+                lambda match: str(self.get_var(match.group("name")) or ''),
+                argument
+            )
+        return argument
+    
+    def __kola_caller__(
+            self, command: Any, args: tuple, kwargs: Dict[str, Any],
+            *, bound_instance: Any = None, **kwds: Any) -> Any:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Run command: {command.__name__} ({(bound_instance or self).__class__.__name__})")
+        return super().__kola_caller__(
+            command,
+            tuple(self.format_text(i) for i in args),
+            self.format_text(kwargs),
+            bound_instance=bound_instance,
+            **kwds
+        )
+    
+    def push_apply(self, __push_cache: Environment) -> None:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Push env: {__push_cache}")
+        return super().push_apply(__push_cache)
+    
+    def pop_apply(self, __env_cache: Environment) -> None:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Pop env: {__env_cache}")
+        return super().pop_apply(__env_cache)
+
+
+__kola_spec__ = KolaSpec(
+    "Kola Runner",
+    collect_all(),
+    main_class=KoiLangRunner
+)
```

### Comparing `KoiLang-1.1.0b2/kola/parser.c` & `KoiLang-1.1.1/kola/parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -1241,15 +1241,15 @@
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 typedef struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 
-/* "lexer.pxd":35
+/* "lexer.pxd":39
  *     cpdef void close(self)
  *     cdef void set_error(self, const char* text) except *
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil             # <<<<<<<<<<<<<<
  *     cdef Token next_token(self)
  * 
  */
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t {
@@ -1268,15 +1268,15 @@
  */
 struct __pyx_opt_args_4kola_6parser_6Parser_set_error {
   int __pyx_n;
   int errorno;
   int recovery;
 };
 
-/* "lexer.pxd":8
+/* "lexer.pxd":12
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 struct __pyx_obj_4kola_5lexer_Token {
@@ -1286,29 +1286,29 @@
   enum TokenSyn syn;
   PyObject *val;
   PyObject *raw_val;
   int lineno;
 };
 
 
-/* "lexer.pxd":20
+/* "lexer.pxd":24
  * 
  * 
  * cdef class LexerConfig:             # <<<<<<<<<<<<<<
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer
  */
 struct __pyx_obj_4kola_5lexer_LexerConfig {
   PyObject_HEAD
   LexerData *lexer_data;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
 };
 
 
-/* "lexer.pxd":26
+/* "lexer.pxd":30
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 struct __pyx_obj_4kola_5lexer_BaseLexer {
@@ -1316,30 +1316,30 @@
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtab;
   yyscan_t scanner;
   LexerData lexer_data;
   PyObject *encoding;
 };
 
 
-/* "lexer.pxd":39
+/* "lexer.pxd":43
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 struct __pyx_obj_4kola_5lexer_FileLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *_filenameo;
   PyObject *_filenameb;
   FILE *fp;
 };
 
 
-/* "lexer.pxd":49
+/* "lexer.pxd":53
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 struct __pyx_obj_4kola_5lexer_StringLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
@@ -1362,29 +1362,29 @@
   uint8_t stat;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
   PyObject *command_set;
 };
 
 
 
-/* "lexer.pxd":8
+/* "lexer.pxd":12
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_Token {
   int (*get_flag)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_Token *__pyx_vtabptr_4kola_5lexer_Token;
 
 
-/* "lexer.pxd":26
+/* "lexer.pxd":30
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 
@@ -1393,29 +1393,29 @@
   void (*set_error)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *);
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*next_syn)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
   struct __pyx_obj_4kola_5lexer_Token *(*next_token)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtabptr_4kola_5lexer_BaseLexer;
 
 
-/* "lexer.pxd":39
+/* "lexer.pxd":43
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_FileLexer {
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer __pyx_base;
 };
 static struct __pyx_vtabstruct_4kola_5lexer_FileLexer *__pyx_vtabptr_4kola_5lexer_FileLexer;
 
 
-/* "lexer.pxd":49
+/* "lexer.pxd":53
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_StringLexer {
@@ -8837,30 +8837,30 @@
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("kola.lexer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("kola.lexer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_Token = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "Token", sizeof(struct __pyx_obj_4kola_5lexer_Token), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_Token) __PYX_ERR(6, 8, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_Token = (struct __pyx_vtabstruct_4kola_5lexer_Token*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_Token); if (unlikely(!__pyx_vtabptr_4kola_5lexer_Token)) __PYX_ERR(6, 8, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_Token) __PYX_ERR(6, 12, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_Token = (struct __pyx_vtabstruct_4kola_5lexer_Token*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_Token); if (unlikely(!__pyx_vtabptr_4kola_5lexer_Token)) __PYX_ERR(6, 12, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_LexerConfig = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "LexerConfig", sizeof(struct __pyx_obj_4kola_5lexer_LexerConfig), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_LexerConfig) __PYX_ERR(6, 20, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_LexerConfig) __PYX_ERR(6, 24, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_BaseLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "BaseLexer", sizeof(struct __pyx_obj_4kola_5lexer_BaseLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_BaseLexer) __PYX_ERR(6, 26, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_BaseLexer = (struct __pyx_vtabstruct_4kola_5lexer_BaseLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_BaseLexer)) __PYX_ERR(6, 26, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_BaseLexer) __PYX_ERR(6, 30, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_BaseLexer = (struct __pyx_vtabstruct_4kola_5lexer_BaseLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_BaseLexer)) __PYX_ERR(6, 30, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_FileLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "FileLexer", sizeof(struct __pyx_obj_4kola_5lexer_FileLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_FileLexer) __PYX_ERR(6, 39, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_FileLexer = (struct __pyx_vtabstruct_4kola_5lexer_FileLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_FileLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_FileLexer)) __PYX_ERR(6, 39, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_FileLexer) __PYX_ERR(6, 43, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_FileLexer = (struct __pyx_vtabstruct_4kola_5lexer_FileLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_FileLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_FileLexer)) __PYX_ERR(6, 43, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_StringLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "StringLexer", sizeof(struct __pyx_obj_4kola_5lexer_StringLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_StringLexer) __PYX_ERR(6, 49, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_StringLexer = (struct __pyx_vtabstruct_4kola_5lexer_StringLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_StringLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_StringLexer)) __PYX_ERR(6, 49, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_StringLexer) __PYX_ERR(6, 53, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_StringLexer = (struct __pyx_vtabstruct_4kola_5lexer_StringLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_StringLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_StringLexer)) __PYX_ERR(6, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `KoiLang-1.1.0b2/kola/parser.pyi` & `KoiLang-1.1.1/kola/parser.pyi`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Any, Callable, Final, Generic, Tuple, TypeVar
-from typing_extensions import Protocol, Self
-from .lexer import BaseLexer, Token
-
-
-class SupportGetCommand(Protocol):
-    def __getitem__(self, __key: str) -> Callable: ...
-
-
-T_CmdSet = TypeVar("T_CmdSet", bound=SupportGetCommand)
-T_Lexer = TypeVar("T_Lexer", bound=BaseLexer)
-
-
-class Parser(Generic[T_Lexer, T_CmdSet]):
-    lexer: Final[T_Lexer]
-    command_set: Final[T_CmdSet]
-
-    def __init__(self, lexer: T_Lexer, command_set: T_CmdSet) -> None: ...
-    def push(self, token: Token) -> None: ...
-    def pop(self) -> Token: ...
-    def parse_args(self) -> Tuple[tuple, dict]: ...
-    def exec_once(self) -> Any: ...
-    def exec(self) -> None: ...
-    def eof(self) -> bool: ...
-    def __iter__(self) -> Self: ...
+from typing import Any, Callable, Final, Generic, Tuple, TypeVar
+from typing_extensions import Protocol, Self
+from .lexer import BaseLexer, Token
+
+
+class SupportGetCommand(Protocol):
+    def __getitem__(self, __key: str) -> Callable: ...
+
+
+T_CmdSet = TypeVar("T_CmdSet", bound=SupportGetCommand)
+T_Lexer = TypeVar("T_Lexer", bound=BaseLexer)
+
+
+class Parser(Generic[T_Lexer, T_CmdSet]):
+    lexer: Final[T_Lexer]
+    command_set: Final[T_CmdSet]
+
+    def __init__(self, lexer: T_Lexer, command_set: T_CmdSet) -> None: ...
+    def push(self, token: Token) -> None: ...
+    def pop(self) -> Token: ...
+    def parse_args(self) -> Tuple[tuple, dict]: ...
+    def exec_once(self) -> Any: ...
+    def exec(self) -> None: ...
+    def eof(self) -> bool: ...
+    def __iter__(self) -> Self: ...
     def __next__(self) -> Any: ...
```

### Comparing `KoiLang-1.1.0b2/kola/unicode_handler.c` & `KoiLang-1.1.1/kola/unicode_handler.c`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-#include "Python.h"
-#include "_cutil.h"
-
-#ifdef HAVE_WCHAR_H
-    #include <wchar.h>
-#endif
-
-PyObject* _decode_utf8(const char **sPtr, const char *end)
-{
-    const char *s;
-    const char *t;
-    t = s = *sPtr;
-    while (s < end && (*s & 0x80)) {
-        s++;
-    }
-    *sPtr = s;
-    return PyUnicode_DecodeUTF8(t, s - t, NULL);
-}
-
-// from cpython:string_parser.decode_unicode_with_escapes
-PyObject* decode_escapes(const char* s, Py_ssize_t len) {
-    PyObject *v = NULL;
-
-    /* check for integer overflow */
-    if ((uint64_t)len > SIZE_MAX / 6) {
-        return NULL;
-    }
-    /* "ä" (2 bytes) may become "\U000000E4" (10 bytes), or 1:5
-       "\ä" (3 bytes) may become "\u005c\U000000E4" (16 bytes), or ~1:6 */
-    PyObject *u = PyBytes_FromStringAndSize((char *)NULL, len * 6);
-    if (u == NULL) {
-        return NULL;
-    }
-
-    char *buf;
-    char *p;
-    p = buf = PyBytes_AsString(u);
-    if (p == NULL) {
-        return NULL;
-    }
-    const char *end = s + len;
-    while (s < end) {
-        if (*s == '\\') {
-            *p++ = *s++;
-            if (s >= end || *s & 0x80) {
-                strcpy(p, "u005c");
-                p += 5;
-                if (s >= end) {
-                    break;
-                }
-            } else if (s + 1 < end && *s == '\r' && s[1] == '\n') {
-                p--;
-                s += 2;
-                if (s >= end) {
-                    break;
-                }
-            } else if (*s == '\n') {
-                p--;
-                s++;
-                if (s >= end) {
-                    break;
-                }
-            }
-        }
-        if (*s & 0x80) {
-            PyObject *w;
-            int kind;
-            const void *data;
-            Py_ssize_t w_len;
-            Py_ssize_t i;
-            w = _decode_utf8(&s, end);
-            if (w == NULL) {
-                Py_DECREF(u);
-                return NULL;
-            }
-            kind = PyUnicode_KIND(w);
-            data = PyUnicode_DATA(w);
-            w_len = PyUnicode_GET_LENGTH(w);
-            for (i = 0; i < w_len; i++) {
-                Py_UCS4 chr = PyUnicode_READ(kind, data, i);
-                sprintf(p, "\\U%08x", chr);
-                p += 10;
-            }
-            /* Should be impossible to overflow */
-            assert(p - buf <= PyBytes_GET_SIZE(u));
-            Py_DECREF(w);
-        }
-        else {
-            *p++ = *s++;
-        }
-    }
-    len = p - buf;
-    s = buf;
-    v = PyUnicode_DecodeUnicodeEscape(s, len, NULL);
-    return v;
-}
-
-PyObject* filter_text(PyObject* string) {
-    Py_ssize_t len = PyUnicode_GET_LENGTH(string);
-    Py_ssize_t offset = 0;
-    for (Py_ssize_t i = 0; i < len; ++i) {
-        Py_UCS4 chr = PyUnicode_READ_CHAR(string, i);
-        if (chr == '\\') {
-            offset++;
-            Py_UCS4 tc = PyUnicode_READ_CHAR(string, ++i);
-            switch (tc) {
-            case '\n':
-                offset++;
-                break;
-            case '\r':
-                if (PyUnicode_READ_CHAR(string, i + 1) == '\n') {
-                    i++;
-                    offset += 2;
-                    break;
-                }
-            default:
-                if (PyUnicode_WriteChar(string, i - offset, '\\') == -1)
-                    goto bad;
-                --offset;
-                if (PyUnicode_WriteChar(string, i - offset, tc) == -1)
-                    goto bad;
-                break;
-            }
-        } else if (offset) {
-            if (PyUnicode_WriteChar(string, i - offset, chr) == -1) goto bad;
-        }
-    }
-    if (offset)
-        PyUnicode_Resize(&string, len - offset);
-    return string;
-bad:
-    return NULL;
-}
+#include "Python.h"
+#include "_cutil.h"
+
+#ifdef HAVE_WCHAR_H
+    #include <wchar.h>
+#endif
+
+PyObject* _decode_utf8(const char **sPtr, const char *end)
+{
+    const char *s;
+    const char *t;
+    t = s = *sPtr;
+    while (s < end && (*s & 0x80)) {
+        s++;
+    }
+    *sPtr = s;
+    return PyUnicode_DecodeUTF8(t, s - t, NULL);
+}
+
+// from cpython:string_parser.decode_unicode_with_escapes
+PyObject* decode_escapes(const char* s, Py_ssize_t len) {
+    PyObject *v = NULL;
+
+    /* check for integer overflow */
+    if ((uint64_t)len > SIZE_MAX / 6) {
+        return NULL;
+    }
+    /* "ä" (2 bytes) may become "\U000000E4" (10 bytes), or 1:5
+       "\ä" (3 bytes) may become "\u005c\U000000E4" (16 bytes), or ~1:6 */
+    PyObject *u = PyBytes_FromStringAndSize((char *)NULL, len * 6);
+    if (u == NULL) {
+        return NULL;
+    }
+
+    char *buf;
+    char *p;
+    p = buf = PyBytes_AsString(u);
+    if (p == NULL) {
+        return NULL;
+    }
+    const char *end = s + len;
+    while (s < end) {
+        if (*s == '\\') {
+            *p++ = *s++;
+            if (s >= end || *s & 0x80) {
+                strcpy(p, "u005c");
+                p += 5;
+                if (s >= end) {
+                    break;
+                }
+            } else if (s + 1 < end && *s == '\r' && s[1] == '\n') {
+                p--;
+                s += 2;
+                if (s >= end) {
+                    break;
+                }
+            } else if (*s == '\n') {
+                p--;
+                s++;
+                if (s >= end) {
+                    break;
+                }
+            }
+        }
+        if (*s & 0x80) {
+            PyObject *w;
+            int kind;
+            const void *data;
+            Py_ssize_t w_len;
+            Py_ssize_t i;
+            w = _decode_utf8(&s, end);
+            if (w == NULL) {
+                Py_DECREF(u);
+                return NULL;
+            }
+            kind = PyUnicode_KIND(w);
+            data = PyUnicode_DATA(w);
+            w_len = PyUnicode_GET_LENGTH(w);
+            for (i = 0; i < w_len; i++) {
+                Py_UCS4 chr = PyUnicode_READ(kind, data, i);
+                sprintf(p, "\\U%08x", chr);
+                p += 10;
+            }
+            /* Should be impossible to overflow */
+            assert(p - buf <= PyBytes_GET_SIZE(u));
+            Py_DECREF(w);
+        }
+        else {
+            *p++ = *s++;
+        }
+    }
+    len = p - buf;
+    s = buf;
+    v = PyUnicode_DecodeUnicodeEscape(s, len, NULL);
+    return v;
+}
+
+PyObject* filter_text(PyObject* string) {
+    Py_ssize_t len = PyUnicode_GET_LENGTH(string);
+    Py_ssize_t offset = 0;
+    for (Py_ssize_t i = 0; i < len; ++i) {
+        Py_UCS4 chr = PyUnicode_READ_CHAR(string, i);
+        if (chr == '\\') {
+            offset++;
+            Py_UCS4 tc = PyUnicode_READ_CHAR(string, ++i);
+            switch (tc) {
+            case '\n':
+                offset++;
+                break;
+            case '\r':
+                if (PyUnicode_READ_CHAR(string, i + 1) == '\n') {
+                    i++;
+                    offset += 2;
+                    break;
+                }
+            default:
+                if (PyUnicode_WriteChar(string, i - offset, '\\') == -1)
+                    goto bad;
+                --offset;
+                if (PyUnicode_WriteChar(string, i - offset, tc) == -1)
+                    goto bad;
+                break;
+            }
+        } else if (offset) {
+            if (PyUnicode_WriteChar(string, i - offset, chr) == -1) goto bad;
+        }
+    }
+    if (offset)
+        PyUnicode_Resize(&string, len - offset);
+    return string;
+bad:
+    return NULL;
+}
```

### Comparing `KoiLang-1.1.0b2/kola/writer.c` & `KoiLang-1.1.1/kola/writer.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0b2/kola/writer.pxd` & `KoiLang-1.1.1/kola/writer.pxd`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from libc.stdio cimport FILE
-from libc.stdint cimport uint8_t
-from ._cutil cimport *
-
-
-cdef enum ItemLevel:
-    BASE_ITEM
-    COMPLEX_ITEM
-    ARG_ITEM
-    FULL_CMD
-
-
-cdef class BaseWriterItem(object):
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class FormatItem(BaseWriterItem):
-    cdef readonly:
-        object value
-        str spec
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class ComplexArg(BaseWriterItem):
-    cdef readonly:
-        str name
-        object value
-        bint split_line
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class NewlineItem(BaseWriterItem):
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef NewlineItem i_newline
-
-
-cdef class BaseWriter:
-    cdef Py_ssize_t cur_indent
-    cdef readonly:
-        uint8_t indent
-        int command_threshold
-    cdef public bint line_beginning
-
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-    cpdef void close(self)
-    cpdef void inc_indent(self)
-    cpdef void dec_indent(self) except *
-    cdef void _write_indent(self) except *
-    cdef void _write_prefix(self, Py_ssize_t length) except *
-    cpdef void newline(self, bint concat_prev = *) except *
-    cpdef void prepare(self) except *
-    cdef void _write_text(self, str text) except *
-
-
-cdef class FileWriter(BaseWriter):
-    cdef FILE* fp
-    cdef readonly:
-        object path
-        str encoding
-    cpdef void close(self)
-    cpdef void prepare(self) except *
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-
-
-cdef class StringWriter(BaseWriter):
-    cdef:
-        bint _closed
-        _PyUnicodeWriter writer
-    
-    cpdef void close(self)
-    cpdef void prepare(self) except *
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-    cpdef str getvalue(self)
+from libc.stdio cimport FILE
+from libc.stdint cimport uint8_t
+from ._cutil cimport *
+
+
+cdef enum ItemLevel:
+    BASE_ITEM
+    COMPLEX_ITEM
+    ARG_ITEM
+    FULL_CMD
+
+
+cdef class BaseWriterItem(object):
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class FormatItem(BaseWriterItem):
+    cdef readonly:
+        object value
+        str spec
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class ComplexArg(BaseWriterItem):
+    cdef readonly:
+        str name
+        object value
+        bint split_line
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class NewlineItem(BaseWriterItem):
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef NewlineItem i_newline
+
+
+cdef class BaseWriter:
+    cdef Py_ssize_t cur_indent
+    cdef readonly:
+        uint8_t indent
+        int command_threshold
+    cdef public bint line_beginning
+
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+    cpdef void close(self)
+    cpdef void inc_indent(self)
+    cpdef void dec_indent(self) except *
+    cdef void _write_indent(self) except *
+    cdef void _write_prefix(self, Py_ssize_t length) except *
+    cpdef void newline(self, bint concat_prev = *) except *
+    cpdef void prepare(self) except *
+    cdef void _write_text(self, str text) except *
+
+
+cdef class FileWriter(BaseWriter):
+    cdef FILE* fp
+    cdef readonly:
+        object path
+        str encoding
+    cpdef void close(self)
+    cpdef void prepare(self) except *
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+
+
+cdef class StringWriter(BaseWriter):
+    cdef:
+        bint _closed
+        _PyUnicodeWriter writer
+    
+    cpdef void close(self)
+    cpdef void prepare(self) except *
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+    cpdef str getvalue(self)
```

### Comparing `KoiLang-1.1.0b2/setup.py` & `KoiLang-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""
-Copyright 2022 Ovizro
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-import os
-import re
-import sys
-import warnings
-from setuptools import setup, Extension
-
-try:
-    with open("README.md", encoding='utf-8') as f:
-        description = f.read()
-except OSError:
-    warnings.warn("Miss file 'README.md', using default description.", ResourceWarning)
-    description = "simple python module for KoiLang parsing"
-
-try:
-    with open("kola/version.py") as f:
-        version = re.search(r"__version__\s*=\s*\"(.*)\"\n", f.read()).group(1) # type: ignore
-except Exception as e:
-    raise ValueError("fail to read kola version") from e
-
-
-USE_CYTHON = "USE_CYTHON" in os.environ
-FILE_SUFFIX = ".pyx" if USE_CYTHON else ".c"
-
-extensions = [
-    Extension("kola.lexer", ["kola/lexer" + FILE_SUFFIX, "kola/unicode_handler.c"]),
-    Extension("kola.parser", ["kola/parser" + FILE_SUFFIX]),
-    Extension("kola.writer", ["kola/writer" + FILE_SUFFIX])
-]
-if USE_CYTHON:
-    from Cython.Build import cythonize
-    from Cython.Compiler import Options
-
-    Options.fast_fail = True
-    extensions = cythonize(extensions, annotate=True, compiler_directives={"language_level": "3"})
-
-
-setup(
-    name="KoiLang",
-    version=version,
-    description="simple python module for KoiLang parsing",
-    long_description=description,
-    long_description_content_type='text/markdown',
-
-    author="Ovizro",
-    author_email="Ovizro@hypercol.com",
-    maintainer="Ovizro",
-    maintainer_email="Ovizro@hypercol.com",
-    license="Apache 2.0",
-
-    url="https://github.com/Ovizro/Kola",
-    packages=["kola", "kola/klvm", "kola/lib", "kola/lib/debugger"],
-    python_requires=">=3.6",
-    package_data={'':["*.pyi", "*.pxd", "*.h"]},
-    install_requires=[
-        "typing_extensions>=4.0" if sys.version_info >= (3, 7)
-            else "typing_extensions>=4.0,<4.2"
-    ],
-    ext_modules=extensions,
-
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: C",
-        "Programming Language :: Cython",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Text Processing :: Markup"
-    ]
+"""
+Copyright 2023 Ovizro
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+import os
+import re
+import sys
+import warnings
+from setuptools import setup, Extension
+
+try:
+    with open("README.md", encoding='utf-8') as f:
+        description = f.read()
+except OSError:
+    warnings.warn("Miss file 'README.md', using default description.", ResourceWarning)
+    description = "simple python module for KoiLang parsing"
+
+try:
+    with open("kola/version.py") as f:
+        version = re.search(r"__version__\s*=\s*\"(.*)\"\n", f.read()).group(1) # type: ignore
+except Exception as e:
+    raise ValueError("fail to read kola version") from e
+
+
+USE_CYTHON = "USE_CYTHON" in os.environ
+FILE_SUFFIX = ".pyx" if USE_CYTHON else ".c"
+
+extensions = [
+    Extension("kola.lexer", ["kola/lexer" + FILE_SUFFIX, "kola/unicode_handler.c"]),
+    Extension("kola.parser", ["kola/parser" + FILE_SUFFIX]),
+    Extension("kola.writer", ["kola/writer" + FILE_SUFFIX])
+]
+if USE_CYTHON:
+    from Cython.Build import cythonize
+    from Cython.Compiler import Options
+
+    Options.fast_fail = True
+    extensions = cythonize(extensions, annotate=True, compiler_directives={"language_level": "3"})
+
+
+setup(
+    name="KoiLang",
+    version=version,
+    description="simple python module for KoiLang parsing",
+    long_description=description,
+    long_description_content_type='text/markdown',
+
+    author="Visecy",
+    author_email="Visecy@visecy.top",
+    maintainer="Ovizro",
+    maintainer_email="Ovizro@visecy.top",
+    license="Apache 2.0",
+
+    url="https://github.com/Ovizro/Kola",
+    packages=["kola", "kola/klvm", "kola/lib", "kola/lib/debugger"],
+    python_requires=">=3.6",
+    package_data={'':["*.pyi", "*.pxd", "*.h"]},
+    install_requires=[
+        "typing_extensions>=4.0" if sys.version_info >= (3, 7)
+            else "typing_extensions>=4.0,<4.2"
+    ],
+    ext_modules=extensions,
+
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: C",
+        "Programming Language :: Cython",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Text Processing :: Markup"
+    ]
 )
```

