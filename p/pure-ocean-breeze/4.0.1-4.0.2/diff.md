# Comparing `tmp/pure_ocean_breeze-4.0.1.tar.gz` & `tmp/pure_ocean_breeze-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.1.tar", last modified: Sun Jul  2 17:24:58 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.2.tar", last modified: Sun Jul  2 17:30:46 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.1.tar` & `pure_ocean_breeze-4.0.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.395010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   263550 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.399010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.403010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:24:58.395010 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:24:58.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-02 17:24:58.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:24:58.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:24:58.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 17:24:58.000000 pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:24:58.407010 pure_ocean_breeze-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 17:24:48.000000 pure_ocean_breeze-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.238962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263550 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.238962 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/setup.py
```

### Comparing `pure_ocean_breeze-4.0.1/LICENSE` & `pure_ocean_breeze-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/PKG-INFO` & `pure_ocean_breeze-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.1
+Version: 4.0.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.1/README.md` & `pure_ocean_breeze-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-03 01:22:04"
-__version__ = "4.0.1"
+__updated__ = "2023-07-03 01:29:04"
+__version__ = "4.0.2"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.1
+Version: 4.0.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.1/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.1/setup.py` & `pure_ocean_breeze-4.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-03 01:21:54"
+__updated__ = "2023-07-03 01:28:50"
 
 from setuptools import setup
 import setuptools
 import re
 import os
 import sys
 
@@ -12,15 +12,15 @@
 
 def get_version(package):
     """Return package version as listed in `__version__` in `init.py`."""
     init_py = open(os.path.join(package, "__init__.py")).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 install_requires=[
-    "numpy",
+    # "numpy",
     "pandas<=1.5.3",
     "scipy",
     "statsmodels",
     "plotly",
     # "matplotlib",
     "pyarrow",
     "loguru",
```

