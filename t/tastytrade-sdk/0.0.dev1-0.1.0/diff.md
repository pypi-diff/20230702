# Comparing `tmp/tastytrade-sdk-0.0.dev1.tar.gz` & `tmp/tastytrade_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-sdk-0.0.dev1.tar", last modified: Sun May  7 01:57:12 2023, max compression
+gzip compressed data, was "tastytrade_sdk-0.1.0.tar", max compression
```

## Comparing `tastytrade-sdk-0.0.dev1.tar` & `tastytrade_sdk-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.388528 tastytrade-sdk-0.0.dev1/
--rw-r--r--   0 aaron      (501) staff       (20)      447 2023-05-07 01:57:12.388366 tastytrade-sdk-0.0.dev1/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)        0 2023-05-06 05:56:32.000000 tastytrade-sdk-0.0.dev1/README.md
--rw-r--r--   0 aaron      (501) staff       (20)      470 2023-05-07 01:57:00.000000 tastytrade-sdk-0.0.dev1/pyproject.toml
--rw-r--r--   0 aaron      (501) staff       (20)       38 2023-05-07 01:57:12.388566 tastytrade-sdk-0.0.dev1/setup.cfg
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.387338 tastytrade-sdk-0.0.dev1/tastytrade_sdk/
--rw-r--r--   0 aaron      (501) staff       (20)      430 2023-05-06 22:20:51.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     1097 2023-05-06 16:42:26.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/api.py
--rw-r--r--   0 aaron      (501) staff       (20)      393 2023-05-06 16:49:48.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/watchlists.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.388187 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/
--rw-r--r--   0 aaron      (501) staff       (20)      447 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)      254 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 aaron      (501) staff       (20)        1 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 aaron      (501) staff       (20)       15 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1056 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/LICENSE
+-rw-r--r--   0        0        0      492 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0      784 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      516 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     4166 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      421 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0      914 2023-07-02 04:27:28.565817 tastytrade_sdk-0.1.0/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.0/PKG-INFO
```

