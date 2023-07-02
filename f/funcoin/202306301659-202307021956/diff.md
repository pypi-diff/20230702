# Comparing `tmp/funcoin-202306301659.tar.gz` & `tmp/funcoin-202307021956.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcoin-202306301659.tar", last modified: Fri Jun 30 08:59:32 2023, max compression
+gzip compressed data, was "funcoin-202307021956.tar", last modified: Sun Jul  2 11:56:04 2023, max compression
```

## Comparing `funcoin-202306301659.tar` & `funcoin-202307021956.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:57:07.000000 funcoin-202306301659/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      186 2023-06-30 08:59:32.103572 funcoin-202306301659/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       42 2023-06-30 08:58:32.000000 funcoin-202306301659/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.095572 funcoin-202306301659/funcoin/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/base/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin/base/db/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       44 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/db/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3132 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/db/mysql.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin/base/drive/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/base/drive/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/drive/job.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3605 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/drive/lanzou.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)   143360 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/base/drive/notecoin.db
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1005 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/drive/oss.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      874 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/drive/transform.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin/base/tables/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       96 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/tables/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1723 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/tables/kline.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1466 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/tables/strategy.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1805 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/base/tables/trade.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin/coins/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/coins/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/coins/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/coins/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6465 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/coins/base/file.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4855 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/coins/base/load.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/coins/okex/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/coins/okex/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      212 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/coins/okex/load.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/server/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/server/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/server/connect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/server/connect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      908 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/server/connect/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2433 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/server/download.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      129 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/server/notecoin_celery.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      283 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/server/notecoin_server.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2357 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/server/script.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1002 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/server/strategy.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/strategy/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       48 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/strategy/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/strategy/binance/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       26 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/strategy/binance/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6701 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/strategy/binance/auto.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1165 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/strategy/binance/example2.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3600 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/strategy/binance/strategy1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5549 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/strategy/binance/strategy2.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/task/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       79 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/task/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2807 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/task/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2180 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/task/load.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.103572 funcoin-202306301659/funcoin/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       24 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       82 2023-06-30 08:58:32.000000 funcoin-202306301659/funcoin/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1198 2023-06-30 08:57:07.000000 funcoin-202306301659/funcoin/utils/time.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:59:32.099572 funcoin-202306301659/funcoin.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      186 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1366 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      126 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/entry_points.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       21 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        8 2023-06-30 08:59:32.000000 funcoin-202306301659/funcoin.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 08:59:32.103572 funcoin-202306301659/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      627 2023-06-30 08:58:45.000000 funcoin-202306301659/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.491340 funcoin-202307021956/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:57:07.000000 funcoin-202307021956/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      186 2023-07-02 11:56:04.491340 funcoin-202307021956/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       42 2023-06-30 08:58:32.000000 funcoin-202307021956/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.483340 funcoin-202307021956/funcoin/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/base/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/base/db/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       44 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/db/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3131 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/base/db/mysql.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/base/drive/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/base/drive/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/drive/job.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3605 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/drive/lanzou.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)   143360 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/base/drive/notecoin.db
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1004 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/base/drive/oss.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      873 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/base/drive/transform.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/base/tables/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       96 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/tables/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1723 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/tables/kline.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1466 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/tables/strategy.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1805 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/base/tables/trade.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/coins/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/coins/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/coins/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/coins/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6465 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/coins/base/file.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4855 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/coins/base/load.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/coins/okex/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/coins/okex/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      211 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/coins/okex/load.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/server/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/server/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/server/connect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/server/connect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      908 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/server/connect/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2433 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/server/download.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      129 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/server/notecoin_celery.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      283 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/server/notecoin_server.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2357 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/server/script.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1002 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/server/strategy.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/strategy/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       48 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/strategy/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/strategy/binance/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       26 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/strategy/binance/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6700 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/strategy/binance/auto.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1164 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/strategy/binance/example2.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3600 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/strategy/binance/strategy1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5548 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/strategy/binance/strategy2.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin/task/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       79 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/task/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2806 2023-06-30 09:06:17.000000 funcoin-202307021956/funcoin/task/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2180 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/task/load.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.491340 funcoin-202307021956/funcoin/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       24 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       82 2023-06-30 08:58:32.000000 funcoin-202307021956/funcoin/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1198 2023-06-30 08:57:07.000000 funcoin-202307021956/funcoin/utils/time.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 11:56:04.487340 funcoin-202307021956/funcoin.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      186 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1366 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      126 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/entry_points.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       20 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        8 2023-07-02 11:56:04.000000 funcoin-202307021956/funcoin.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-02 11:56:04.491340 funcoin-202307021956/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      626 2023-06-30 09:06:32.000000 funcoin-202307021956/setup.py
```

### Comparing `funcoin-202306301659/LICENSE` & `funcoin-202307021956/LICENSE`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/base/db/mysql.py` & `funcoin-202307021956/funcoin/base/db/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pymysql
-from notesecret import read_secret
+from funsecret import read_secret
 from pymysql.cursors import DictCursor
 from sqlalchemy import MetaData, Table, create_engine, delete, inspect, select
 from sqlalchemy.dialects.mysql import insert
 
 engine_dict = {}
 meta_dict = {}
```

### Comparing `funcoin-202306301659/funcoin/base/drive/lanzou.py` & `funcoin-202307021956/funcoin/base/drive/lanzou.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/base/drive/notecoin.db` & `funcoin-202307021956/funcoin/base/drive/notecoin.db`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/base/drive/oss.py` & `funcoin-202307021956/funcoin/base/drive/oss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 
 import oss2
 from notefile.compress import tarfile
-from notesecret import read_secret
+from funsecret import read_secret
 
 global bucket
 bucket = None
 
 
 def get_bucket():
     global bucket
```

### Comparing `funcoin-202306301659/funcoin/base/drive/transform.py` & `funcoin-202307021956/funcoin/base/drive/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 import sys
 
-from notesecret import read_secret
+from funsecret import read_secret
 
 try:
     from mysql_to_sqlite3.cli import MySQLtoSQLite
 except Exception as e:
     print(e)
     subprocess.check_call([sys.executable, "-m", "pip", "install", "mysql-to-sqlite3"])
     from mysql_to_sqlite3.cli import MySQLtoSQLite
```

### Comparing `funcoin-202306301659/funcoin/base/tables/kline.py` & `funcoin-202307021956/funcoin/base/tables/kline.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/base/tables/strategy.py` & `funcoin-202307021956/funcoin/base/tables/strategy.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/base/tables/trade.py` & `funcoin-202307021956/funcoin/base/tables/trade.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/coins/base/file.py` & `funcoin-202307021956/funcoin/coins/base/file.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/coins/base/load.py` & `funcoin-202307021956/funcoin/coins/base/load.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/server/connect/base.py` & `funcoin-202307021956/funcoin/server/connect/base.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/server/download.py` & `funcoin-202307021956/funcoin/server/download.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/server/script.py` & `funcoin-202307021956/funcoin/server/script.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/server/strategy.py` & `funcoin-202307021956/funcoin/server/strategy.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/strategy/binance/auto.py` & `funcoin-202307021956/funcoin/strategy/binance/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from datetime import datetime, timedelta
 
 import ccxt
 import pandas as pd
 from funcoin.base.db.mysql import get_engine
-from notesecret import read_secret
+from funsecret import read_secret
 from noteworker import get_default_app
 from sqlalchemy.dialects.mysql import insert
 from tqdm import tqdm
 
 pd.set_option('display.max_columns', None)
 pd.set_option('display.max_rows', 500)
 pd.set_option('max_colwidth', 1000)
```

### Comparing `funcoin-202306301659/funcoin/strategy/binance/example2.py` & `funcoin-202307021956/funcoin/strategy/binance/example2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Python
 import time
 from asyncio import run
 
 import ccxt.pro as ccxtpro
-from notesecret import read_secret
+from funsecret import read_secret
 
 
 async def main():
     d = {
         'newUpdates': False,
         'apiKey': read_secret('coin', 'binance', 'api_key'),
         'secretKey': read_secret('coin', 'binance', 'secret_key')
```

### Comparing `funcoin-202306301659/funcoin/strategy/binance/strategy1.py` & `funcoin-202307021956/funcoin/strategy/binance/strategy1.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/strategy/binance/strategy2.py` & `funcoin-202307021956/funcoin/strategy/binance/strategy2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from asyncio import run
 
 import ccxt.pro as ccxtpro
 import pandas as pd
 from funcoin.base.tables.strategy import StrategyTable
 from funcoin.task import AccountTask, BaseTask
 from funcoin.utils import logger
-from notesecret import read_secret
+from funsecret import read_secret
 
 
 class Strategy2Task(BaseTask):
 
     def __init__(self, *args, **kwargs):
         super(Strategy2Task, self).__init__(*args, **kwargs)
         self.table = StrategyTable(db_suffix=self.exchange.name)
```

### Comparing `funcoin-202306301659/funcoin/task/base.py` & `funcoin-202307021956/funcoin/task/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 
 import ccxt
 import pandas as pd
 from funcoin.base.db.mysql import get_engine
-from notesecret import read_secret
+from funsecret import read_secret
 from sqlalchemy.dialects.mysql import DOUBLE
 
 
 class BaseTask:
     table_name = "base"
 
     def __init__(self, exchange=None, engine=None, *args, **kwargs):
```

### Comparing `funcoin-202306301659/funcoin/task/load.py` & `funcoin-202307021956/funcoin/task/load.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin/utils/time.py` & `funcoin-202307021956/funcoin/utils/time.py`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/funcoin.egg-info/SOURCES.txt` & `funcoin-202307021956/funcoin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcoin-202306301659/setup.py` & `funcoin-202307021956/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from setuptools import find_packages, setup
 
 
-install_requires = ['darkbuild', 'darksecret']
+install_requires = ['darkbuild', 'funsecret']
 
 
 setup(name='funcoin',
       version=time.strftime("%Y%m%d%H%M", time.localtime()),
       description='funcoin',
       author='bingtao',
       author_email='1007530194@qq.com',
```

