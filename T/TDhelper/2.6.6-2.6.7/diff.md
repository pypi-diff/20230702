# Comparing `tmp/TDhelper-2.6.6.tar.gz` & `tmp/TDhelper-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.6.6.tar", last modified: Sun Jul  2 08:13:45 2023, max compression
+gzip compressed data, was "TDhelper-2.6.7.tar", last modified: Sun Jul  2 09:21:24 2023, max compression
```

## Comparing `TDhelper-2.6.6.tar` & `TDhelper-2.6.7.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.6.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 08:13:45.036720 TDhelper-2.6.6/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.6.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.976720 TDhelper-2.6.6/TDhelper/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/performance.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/webEvent/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2023-06-21 18:42:32.000000 TDhelper-2.6.6/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.6.6/TDhelper/Spider/contentExtraction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.6.6/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/apiCore.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/bin/globalvar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/ring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.6.6/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.6.6/TDhelper/cache/webCache/webCacheFactory.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.6.6/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/objectId.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      737 2023-06-24 17:18:04.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 03:52:59.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-06-23 03:56:02.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/attribute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      691 2023-06-23 17:33:22.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-06-23 03:57:59.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5506 2023-06-23 17:34:16.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5811 2023-06-24 17:09:58.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 04:05:47.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-06-24 17:09:32.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/conn.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/file.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2023-06-21 18:37:27.000000 TDhelper-2.6.6/TDhelper/generic/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/classDocCfg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.6.6/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dictHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-06-20 10:12:04.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/delete__test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2023-06-21 18:39:28.000000 TDhelper-2.6.6/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.6.6/TDhelper/generic/transformationType.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2023-06-30 15:45:47.000000 TDhelper-2.6.6/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/m3u8_backup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/status/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/rpc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6457 2023-07-02 08:11:49.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12916 2023-07-02 08:06:37.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2023-07-02 05:10:28.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/obsolete_struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2023-07-02 08:07:50.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/struct.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2023-07-02 04:48:59.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/token.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2023-06-30 10:08:12.000000 TDhelper-2.6.6/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/model/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/reflect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/leg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/vertebra.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/toe.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/shellScripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.6.6/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.6.6/TDhelper/shellScripts/saasHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/simulate/json.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/structs/dir.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/web/obsolete_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-21 15:54:46.000000 TDhelper-2.6.6/TDhelper/web/obsolete_permissionHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.6.6/TDhelper/web/utils/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/event/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:41.000000 TDhelper-2.6.6/TDhelper/web/utils/event/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:34:09.000000 TDhelper-2.6.6/TDhelper/web/utils/event/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:58.000000 TDhelper-2.6.6/TDhelper/web/utils/event/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/permission/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:44.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-06-22 13:22:33.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2023-06-21 12:49:09.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 08:13:45.036720 TDhelper-2.6.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-07-02 08:13:34.000000 TDhelper-2.6.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.6.7/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 09:21:24.326808 TDhelper-2.6.7/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.6.7/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.276808 TDhelper-2.6.7/TDhelper/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.276808 TDhelper-2.6.7/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Decorators/performance.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.276808 TDhelper-2.6.7/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.276808 TDhelper-2.6.7/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/classEvent/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.286808 TDhelper-2.6.7/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Event/webEvent/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.286808 TDhelper-2.6.7/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/MagicCls/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.286808 TDhelper-2.6.7/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2023-06-21 18:42:32.000000 TDhelper-2.6.7/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Msg/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.286808 TDhelper-2.6.7/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Scheduler/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.286808 TDhelper-2.6.7/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.6.7/TDhelper/Spider/contentExtraction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.6.7/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/apiCore.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/bin/globalvar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/ring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.6.7/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.6.7/TDhelper/cache/webCache/webCacheFactory.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.6.7/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mongodb/objectId.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/mongodb/orm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      737 2023-06-24 17:18:04.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 03:52:59.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-06-23 03:56:02.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/attribute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      691 2023-06-23 17:33:22.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/field.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-06-23 03:57:59.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/field_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5506 2023-06-23 17:34:16.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/meta copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5811 2023-06-24 17:09:58.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.296808 TDhelper-2.6.7/TDhelper/db/mongodb/orm/drives/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 04:05:47.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/drives/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-06-24 17:09:32.000000 TDhelper-2.6.7/TDhelper/db/mongodb/orm/drives/conn.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mongodb/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/db/mysql/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/document/excel/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/excel/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/file.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/document/ini/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2023-06-21 18:37:27.000000 TDhelper-2.6.7/TDhelper/generic/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/classDocCfg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.6.7/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/dictHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/dynamic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-06-20 10:12:04.000000 TDhelper-2.6.7/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/dynamic/delete__test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2023-06-21 18:39:28.000000 TDhelper-2.6.7/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.6.7/TDhelper/generic/transformationType.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.306808 TDhelper-2.6.7/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2023-06-30 15:45:47.000000 TDhelper-2.6.7/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/m3u8_backup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/http/status/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6457 2023-07-02 08:11:49.000000 TDhelper-2.6.7/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12916 2023-07-02 08:06:37.000000 TDhelper-2.6.7/TDhelper/network/rpc/Client/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2023-07-02 05:10:28.000000 TDhelper-2.6.7/TDhelper/network/rpc/Core/obsolete_struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2023-07-02 08:07:50.000000 TDhelper-2.6.7/TDhelper/network/rpc/Core/struct.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2023-07-02 04:48:59.000000 TDhelper-2.6.7/TDhelper/network/rpc/Core/token.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2023-06-30 10:08:12.000000 TDhelper-2.6.7/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.6.7/TDhelper/network/rpc/Server/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/rpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/socket/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/reflect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/control/device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.316808 TDhelper-2.6.7/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/leg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/people/vertebra.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/robot/struct/toe.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/shellScripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.6.7/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.6.7/TDhelper/shellScripts/saasHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/simulate/json.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/structs/dir.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.6.7/TDhelper/web/obsolete_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-21 15:54:46.000000 TDhelper-2.6.7/TDhelper/web/obsolete_permissionHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/web/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.6.7/TDhelper/web/utils/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/web/utils/event/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:41.000000 TDhelper-2.6.7/TDhelper/web/utils/event/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:34:09.000000 TDhelper-2.6.7/TDhelper/web/utils/event/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:58.000000 TDhelper-2.6.7/TDhelper/web/utils/event/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.326808 TDhelper-2.6.7/TDhelper/web/utils/permission/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:44.000000 TDhelper-2.6.7/TDhelper/web/utils/permission/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-06-22 13:22:33.000000 TDhelper-2.6.7/TDhelper/web/utils/permission/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2023-06-21 12:49:09.000000 TDhelper-2.6.7/TDhelper/web/utils/permission/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 09:21:24.276808 TDhelper-2.6.7/TDhelper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 09:21:24.000000 TDhelper-2.6.7/TDhelper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 09:21:24.326808 TDhelper-2.6.7/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-07-02 09:20:03.000000 TDhelper-2.6.7/setup.py
```

### Comparing `TDhelper-2.6.6/LICENSE` & `TDhelper-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/PKG-INFO` & `TDhelper-2.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.6.6
+Version: 2.6.7
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.6.6 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.6.7 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.6.6/README.md` & `TDhelper-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Decorators/log.py` & `TDhelper-2.6.7/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Decorators/performance.py` & `TDhelper-2.6.7/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Event/Event.py` & `TDhelper-2.6.7/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Event/classEvent/event.py` & `TDhelper-2.6.7/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.6.7/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.6.7/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.6.7/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/MagicCls/model.py` & `TDhelper-2.6.7/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/MagicCls/test.py` & `TDhelper-2.6.7/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Msg/AppPush.py` & `TDhelper-2.6.7/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Msg/Config.py` & `TDhelper-2.6.7/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Msg/Email.py` & `TDhelper-2.6.7/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.6.7/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Msg/SMS.py` & `TDhelper-2.6.7/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Scheduler/base.py` & `TDhelper-2.6.7/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.6.7/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Scheduler/interface.py` & `TDhelper-2.6.7/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Scheduler/log_config.py` & `TDhelper-2.6.7/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Scheduler/service.py` & `TDhelper-2.6.7/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.6.7/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.6.7/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.6.7/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.6.7/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.6.7/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.6.7/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/models/status.py` & `TDhelper-2.6.7/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/regex.py` & `TDhelper-2.6.7/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/Spider/spiderPools.py` & `TDhelper-2.6.7/TDhelper/Spider/spiderPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/apiCore.py` & `TDhelper-2.6.7/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/bin/globalvar.py` & `TDhelper-2.6.7/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/memcache.py` & `TDhelper-2.6.7/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/pools.py` & `TDhelper-2.6.7/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/ring.py` & `TDhelper-2.6.7/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/webCache/interface.py` & `TDhelper-2.6.7/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.6.7/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.6.7/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/Db/base.py` & `TDhelper-2.6.7/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/base.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/__init__.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/attribute.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/field.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta copy.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/meta copy.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/core/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/conn.py` & `TDhelper-2.6.7/TDhelper/db/mongodb/orm/drives/conn.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.6.7/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.6.7/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/document/excel/model.py` & `TDhelper-2.6.7/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/document/file.py` & `TDhelper-2.6.7/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/document/ini/meta.py` & `TDhelper-2.6.7/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/__init__.py` & `TDhelper-2.6.7/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/classDocCfg.py` & `TDhelper-2.6.7/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.6.7/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/dictHelper.py` & `TDhelper-2.6.7/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.6.7/TDhelper/generic/dynamic/base/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/dynamic/delete__test.py` & `TDhelper-2.6.7/TDhelper/generic/dynamic/delete__test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/findAttribute.py` & `TDhelper-2.6.7/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/recursion.py` & `TDhelper-2.6.7/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/requier.py` & `TDhelper-2.6.7/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/standard_result.py` & `TDhelper-2.6.7/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/threadPools.py` & `TDhelper-2.6.7/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/generic/transformationType.py` & `TDhelper-2.6.7/TDhelper/generic/transformationType.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.6.7/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/RPC.py` & `TDhelper-2.6.7/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/RPC1.py` & `TDhelper-2.6.7/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/http_helper.py` & `TDhelper-2.6.7/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.6.7/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/m3u8.py` & `TDhelper-2.6.7/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.6.7/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Client/rpc.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Client/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Core/obsolete_struct.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Core/obsolete_struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Core/struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Core/token.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Core/token.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Generic/Host.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Server/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.6.7/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/__init__.py` & `TDhelper-2.6.7/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.6.7/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/client.py` & `TDhelper-2.6.7/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.6.7/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.6.7/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/socket/server.py` & `TDhelper-2.6.7/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/websocket/protocol.py` & `TDhelper-2.6.7/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/network/websocket/server.py` & `TDhelper-2.6.7/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/reflect.py` & `TDhelper-2.6.7/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/control/D_33890.py` & `TDhelper-2.6.7/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/control/device.py` & `TDhelper-2.6.7/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/people/__init__.py` & `TDhelper-2.6.7/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/people/leg.py` & `TDhelper-2.6.7/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.6.7/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.6.7/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/struct/ankle.py` & `TDhelper-2.6.7/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/struct/base.py` & `TDhelper-2.6.7/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/struct/hip.py` & `TDhelper-2.6.7/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/struct/knee.py` & `TDhelper-2.6.7/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/robot/struct/toe.py` & `TDhelper-2.6.7/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.6.7/TDhelper/shellScripts/saasHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/simulate/json.py` & `TDhelper-2.6.7/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/structs/dir.py` & `TDhelper-2.6.7/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/web/obsolete_permission.py` & `TDhelper-2.6.7/TDhelper/web/obsolete_permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/web/obsolete_permissionHelper.py` & `TDhelper-2.6.7/TDhelper/web/obsolete_permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/web/utils/permission/client.py` & `TDhelper-2.6.7/TDhelper/web/utils/permission/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper/web/utils/permission/server.py` & `TDhelper-2.6.7/TDhelper/web/utils/permission/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.6.7/TDhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.6.6
+Version: 2.6.7
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.6.6 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.6.7 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.6.6/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.6.7/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/TDhelper.egg-info/requires.txt` & `TDhelper-2.6.7/TDhelper.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.6/setup.py` & `TDhelper-2.6.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.6.6",
+    version="2.6.7",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

