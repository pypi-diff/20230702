# Comparing `tmp/TDhelper-2.6.5.tar.gz` & `tmp/TDhelper-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.6.5.tar", last modified: Sun Jul  2 05:10:55 2023, max compression
+gzip compressed data, was "TDhelper-2.6.6.tar", last modified: Sun Jul  2 08:13:45 2023, max compression
```

## Comparing `TDhelper-2.6.5.tar` & `TDhelper-2.6.6.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.6.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 05:10:55.426481 TDhelper-2.6.5/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.6.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Decorators/performance.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/classEvent/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Event/webEvent/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/MagicCls/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2023-06-21 18:42:32.000000 TDhelper-2.6.5/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Msg/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.386481 TDhelper-2.6.5/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Scheduler/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.386481 TDhelper-2.6.5/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.6.5/TDhelper/Spider/contentExtraction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.386481 TDhelper-2.6.5/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.6.5/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/apiCore.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.386481 TDhelper-2.6.5/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/bin/globalvar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/ring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.6.5/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.6.5/TDhelper/cache/webCache/webCacheFactory.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.6.5/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mongodb/objectId.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/mongodb/orm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      737 2023-06-24 17:18:04.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 03:52:59.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-06-23 03:56:02.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/attribute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      691 2023-06-23 17:33:22.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/field.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-06-23 03:57:59.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/field_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5506 2023-06-23 17:34:16.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/meta copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5811 2023-06-24 17:09:58.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/mongodb/orm/drives/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 04:05:47.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/drives/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-06-24 17:09:32.000000 TDhelper-2.6.5/TDhelper/db/mongodb/orm/drives/conn.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mongodb/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/db/mysql/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.396481 TDhelper-2.6.5/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/document/excel/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/excel/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/file.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/document/ini/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2023-06-21 18:37:27.000000 TDhelper-2.6.5/TDhelper/generic/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/classDocCfg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.6.5/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/dictHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/dynamic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-06-20 10:12:04.000000 TDhelper-2.6.5/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/dynamic/delete__test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2023-06-21 18:39:28.000000 TDhelper-2.6.5/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.6.5/TDhelper/generic/transformationType.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.406481 TDhelper-2.6.5/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2023-06-30 15:45:47.000000 TDhelper-2.6.5/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/m3u8_backup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/http/status/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6237 2023-07-02 05:05:24.000000 TDhelper-2.6.5/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12987 2023-07-02 04:00:18.000000 TDhelper-2.6.5/TDhelper/network/rpc/Client/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2023-07-02 05:10:28.000000 TDhelper-2.6.5/TDhelper/network/rpc/Core/obsolete_struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17131 2023-07-02 04:28:59.000000 TDhelper-2.6.5/TDhelper/network/rpc/Core/struct.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2023-07-02 04:48:59.000000 TDhelper-2.6.5/TDhelper/network/rpc/Core/token.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2023-06-30 10:08:12.000000 TDhelper-2.6.5/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.6.5/TDhelper/network/rpc/Server/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/rpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/model/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/socket/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/reflect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/control/device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/leg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.416481 TDhelper-2.6.5/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/people/vertebra.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/robot/struct/toe.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/shellScripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.6.5/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.6.5/TDhelper/shellScripts/saasHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/simulate/json.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/structs/dir.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.6.5/TDhelper/web/obsolete_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-21 15:54:46.000000 TDhelper-2.6.5/TDhelper/web/obsolete_permissionHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/web/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.6.5/TDhelper/web/utils/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/web/utils/event/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:41.000000 TDhelper-2.6.5/TDhelper/web/utils/event/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:34:09.000000 TDhelper-2.6.5/TDhelper/web/utils/event/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:58.000000 TDhelper-2.6.5/TDhelper/web/utils/event/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.426481 TDhelper-2.6.5/TDhelper/web/utils/permission/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:44.000000 TDhelper-2.6.5/TDhelper/web/utils/permission/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-06-22 13:22:33.000000 TDhelper-2.6.5/TDhelper/web/utils/permission/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2023-06-21 12:49:09.000000 TDhelper-2.6.5/TDhelper/web/utils/permission/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 05:10:55.376481 TDhelper-2.6.5/TDhelper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 05:10:55.000000 TDhelper-2.6.5/TDhelper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 05:10:55.426481 TDhelper-2.6.5/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-07-02 05:10:41.000000 TDhelper-2.6.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.6.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 08:13:45.036720 TDhelper-2.6.6/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.6.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.976720 TDhelper-2.6.6/TDhelper/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Decorators/performance.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/classEvent/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Event/webEvent/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/MagicCls/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2023-06-21 18:42:32.000000 TDhelper-2.6.6/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Msg/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Scheduler/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.6.6/TDhelper/Spider/contentExtraction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.6.6/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/apiCore.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/bin/globalvar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/ring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.6.6/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.6.6/TDhelper/cache/webCache/webCacheFactory.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.6.6/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/objectId.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.996720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      737 2023-06-24 17:18:04.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 03:52:59.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-06-23 03:56:02.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/attribute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      691 2023-06-23 17:33:22.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-06-23 03:57:59.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5506 2023-06-23 17:34:16.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5811 2023-06-24 17:09:58.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 04:05:47.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-06-24 17:09:32.000000 TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/conn.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mongodb/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/db/mysql/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/file.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.006720 TDhelper-2.6.6/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/document/ini/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2023-06-21 18:37:27.000000 TDhelper-2.6.6/TDhelper/generic/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/classDocCfg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.6.6/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dictHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-06-20 10:12:04.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/dynamic/delete__test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2023-06-21 18:39:28.000000 TDhelper-2.6.6/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.6.6/TDhelper/generic/transformationType.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2023-06-30 15:45:47.000000 TDhelper-2.6.6/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/m3u8_backup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/http/status/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/rpc/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.016720 TDhelper-2.6.6/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6457 2023-07-02 08:11:49.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12916 2023-07-02 08:06:37.000000 TDhelper-2.6.6/TDhelper/network/rpc/Client/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2023-07-02 05:10:28.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/obsolete_struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2023-07-02 08:07:50.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/struct.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2023-07-02 04:48:59.000000 TDhelper-2.6.6/TDhelper/network/rpc/Core/token.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2023-06-30 10:08:12.000000 TDhelper-2.6.6/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.6.6/TDhelper/network/rpc/Server/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/rpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/socket/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/reflect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/control/device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/leg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/people/vertebra.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/robot/struct/toe.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/shellScripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.6.6/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.6.6/TDhelper/shellScripts/saasHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/simulate/json.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.026720 TDhelper-2.6.6/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/structs/dir.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.6.6/TDhelper/web/obsolete_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-21 15:54:46.000000 TDhelper-2.6.6/TDhelper/web/obsolete_permissionHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.6.6/TDhelper/web/utils/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/event/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:41.000000 TDhelper-2.6.6/TDhelper/web/utils/event/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:34:09.000000 TDhelper-2.6.6/TDhelper/web/utils/event/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-21 18:33:58.000000 TDhelper-2.6.6/TDhelper/web/utils/event/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:45.036720 TDhelper-2.6.6/TDhelper/web/utils/permission/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:44.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-06-22 13:22:33.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2023-06-21 12:49:09.000000 TDhelper-2.6.6/TDhelper/web/utils/permission/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 08:13:44.986720 TDhelper-2.6.6/TDhelper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 08:13:44.000000 TDhelper-2.6.6/TDhelper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 08:13:45.036720 TDhelper-2.6.6/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-07-02 08:13:34.000000 TDhelper-2.6.6/setup.py
```

### Comparing `TDhelper-2.6.5/LICENSE` & `TDhelper-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/PKG-INFO` & `TDhelper-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.6.5
+Version: 2.6.6
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
-Metadata-Version: 2.1 Name: TDhelper Version: 2.6.5 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.6.6 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.6.5/README.md` & `TDhelper-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Decorators/log.py` & `TDhelper-2.6.6/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Decorators/performance.py` & `TDhelper-2.6.6/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Event/Event.py` & `TDhelper-2.6.6/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Event/classEvent/event.py` & `TDhelper-2.6.6/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.6.6/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.6.6/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.6.6/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/MagicCls/model.py` & `TDhelper-2.6.6/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/MagicCls/test.py` & `TDhelper-2.6.6/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Msg/AppPush.py` & `TDhelper-2.6.6/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Msg/Config.py` & `TDhelper-2.6.6/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Msg/Email.py` & `TDhelper-2.6.6/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.6.6/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Msg/SMS.py` & `TDhelper-2.6.6/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Scheduler/base.py` & `TDhelper-2.6.6/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.6.6/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Scheduler/interface.py` & `TDhelper-2.6.6/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Scheduler/log_config.py` & `TDhelper-2.6.6/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Scheduler/service.py` & `TDhelper-2.6.6/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.6.6/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.6.6/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.6.6/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.6.6/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/models/status.py` & `TDhelper-2.6.6/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/regex.py` & `TDhelper-2.6.6/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/Spider/spiderPools.py` & `TDhelper-2.6.6/TDhelper/Spider/spiderPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/apiCore.py` & `TDhelper-2.6.6/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/bin/globalvar.py` & `TDhelper-2.6.6/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/memcache.py` & `TDhelper-2.6.6/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/pools.py` & `TDhelper-2.6.6/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/ring.py` & `TDhelper-2.6.6/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/webCache/interface.py` & `TDhelper-2.6.6/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.6.6/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.6.6/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/Db/base.py` & `TDhelper-2.6.6/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/base.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/__init__.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/attribute.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/field.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/field.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/meta copy.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta copy.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/core/meta.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/core/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mongodb/orm/drives/conn.py` & `TDhelper-2.6.6/TDhelper/db/mongodb/orm/drives/conn.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.6.6/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.6.6/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/document/excel/model.py` & `TDhelper-2.6.6/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/document/file.py` & `TDhelper-2.6.6/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/document/ini/meta.py` & `TDhelper-2.6.6/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/__init__.py` & `TDhelper-2.6.6/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/classDocCfg.py` & `TDhelper-2.6.6/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.6.6/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/dictHelper.py` & `TDhelper-2.6.6/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.6.6/TDhelper/generic/dynamic/base/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/dynamic/delete__test.py` & `TDhelper-2.6.6/TDhelper/generic/dynamic/delete__test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/findAttribute.py` & `TDhelper-2.6.6/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/recursion.py` & `TDhelper-2.6.6/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/requier.py` & `TDhelper-2.6.6/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/standard_result.py` & `TDhelper-2.6.6/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/threadPools.py` & `TDhelper-2.6.6/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/generic/transformationType.py` & `TDhelper-2.6.6/TDhelper/generic/transformationType.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.6.6/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/RPC.py` & `TDhelper-2.6.6/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/RPC1.py` & `TDhelper-2.6.6/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/http_helper.py` & `TDhelper-2.6.6/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.6.6/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/m3u8.py` & `TDhelper-2.6.6/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.6.6/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Client/rpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,46 @@
 
 class client():
     __TOKEN_KEY__ = "api-token"
     __LOGGER__ = logging
     __service_exists__= lambda o,k: True if k in o.__dict__ else False
     __get_service__= lambda o,k: getattr(o,k) if o.__service_exists__(k) else None
     __token_manage:token_manage= None
+    __call_time_out=2
     @performance.performance_testing
-    def __init__(self, uri, path: str = "", service_conf: dict = {}, sniffer: str = "api/sniffer", services: list = [], token_key=None, logger: dict = None, try_count:int=5, try_sleep:int=3)->None:
+    def __init__(self, uri, path: str = "", service_conf: dict = {}, sniffer: str = "api/sniffer", services: list = [], token_key=None, logger: dict = None, try_count:int=5, try_sleep:int=3, call_time_out=2)->None:
         '''rpc client.
         
         params:
         
             uri - <class: string>: rpc gateway;
             
-            path - <class: list>: rpc init url path;
+            path - <class: str>: rpc init url path;
             
-            token - <class: string>: it's no use;
+            service_conf - <class: dict>: {"service_key":"","secret":""};
             
-            sniffer - <class: list>: rpc service sniffer path, get it with operator;
+            sniffer - <class: str>: rpc service sniffer path, get it with operator;
             
             services - <class: list>: get rpc service by service list, default all, default all; 
             
             token_key - <class: string>: key field  for rpc authorized. it is request headers field; validate in SAAS-CLI framework core.filter.access.py;
             
             logger - <class: dict>: logger configure dict;
             
             try_count - <class:int>: max count for service available sniffer, default 5;
             
             try_sleep -<class: int>: service available sniffer retry sleep time, default 3 second;
+            
+            call_time_out - <class:int> remote call time out, default 2 second; 
         '''
         if logger:
             self.__LOGGER__.basicConfig(level=logging.INFO)
             self.__LOGGER__.config.dictConfig(logger)
         self.__TOKEN_KEY__ = token_key if token_key else self.__TOKEN_KEY__
+        self.__call_time_out= call_time_out
         self.__token_manage= token_manage(uri,service_conf.get("service_key",""),service_conf.get("secret",""))
         header = {
             "access-source":"rpc"
         }
         if self.__token_manage.Token:
             header.update({self.__TOKEN_KEY__:self.__token_manage.Token})
         else:
@@ -68,15 +72,15 @@
                             ("/".join([uri,sniffer.lstrip("/")])))
         self.__context__ = self.__get_conf__(rpc_uri, header)
         if self.__context__:
             if self.__context__["msg"]:
                 self.__dict__["__srv_struct__"] = {}
                 for k, v in self.__context__["msg"].items():
                     self.__dict__["__srv_struct__"][k] = type(
-                        k, (RPC_SERVICE,), {}).create_by_cnf(v, self.__TOKEN_KEY__, self.__token_manage)
+                        k, (RPC_SERVICE,), {}).create_by_cnf(v, self.__TOKEN_KEY__, self.__token_manage,self.__call_time_out)
                     methods = [kv for kv in v['methods'].keys()]
                     self.__dict__[k] = type(k, (dynamic_creator,), {
                                             "__dynamic_methods__": methods, "__hook_method__": self.__call__})()
             else:
                 self.__LOGGER__.error("not found rpc method.%s"%self.__context__["msg"])
                 raise Exception("not found rpc method.%s"%self.__context__["msg"])
         else:
```

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Client/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     return require(cls).getType()
 
 class SRC(metaclass=Meta):
     """SRC
         service register center interface.
     Parameters:
         uris - <class:list>, rpc server apis.
-        token - <class:str>, rpc apis access token.
         server_cnf - <class:dict>, service conf.
         rpc_conf_header - <class:dict>, rpc configure general header struct. example :{
                     "name": "权限服务",
                     "description": "权限服务",
                     "key": "RPC_TEST",
                     "secret": "203920398409238408204324",
                     "protocol": "http://",
@@ -40,16 +39,16 @@
         **kwargs:
             token_key - <class:str>, access token key. it will auto assembly http header. default 'api-token'.
     Returns:
         None
     Raises:
         None
     """
-    def __init__(self, uris: list, token: str, server_cnf: dict = None, rpc_conf_header:dict={}, logger: "logging" = None,**kwargs):
-        self.__RPC_CNF__ = RPC_SERVICE_CONF(uris, token)
+    def __init__(self, uris: list, server_cnf: dict = None, rpc_conf_header:dict={}, logger: "logging" = None,**kwargs):
+        self.__RPC_CNF__ = RPC_SERVICE_CONF(uris)
         self.__token_manage__= token_manage(self.__RPC_CNF__.getUri(),rpc_conf_header.get("key"),rpc_conf_header.get('secret'))
         self.__logger_hander__ = logger if logger else self.__logger_hander__
         self.__rpc_server_cnf__ = server_cnf if server_cnf else self.__rpc_server_cnf__
         apiToken="api-token" if "token_key" not in kwargs else kwargs["token_key"]
         #self.__headers__[apiToken] = self.__token_manage__.Token#self.__RPC_CNF__.token
         self.__rpc_conf_header__= rpc_conf_header
         self.__headers__.update({apiToken:self.__token_manage__.Token})
```

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Core/obsolete_struct.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Core/obsolete_struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Core/struct.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,26 +208,28 @@
     host = None
     name: str = None
     description: str = None
     key: str = None
     secret: str = None
     protocol: str = "http://"
     methods = {}
+    __call_time_out=2
     __method_exists__= lambda o,k: True if k in o.__dict__ else False
     __token_manage:token_manage= None
-    def __init__(self, name=None, description=None, key=None, secret=None, protocol=None, host_cnf=None, methods_cnf=None, token_key="api-token",token_manage:token_manage=None):
+    def __init__(self, name=None, description=None, key=None, secret=None, protocol=None, host_cnf=None, methods_cnf=None, token_key="api-token",token_manage:token_manage=None,call_time_out=2):
         self.__TOKEN_KEY__ = token_key
         self.name = name
         self.description = description
         self.key = key
         self.secret = secret
         self.protocol = protocol
         self.host = HostManager()
         self.methods={}
         self.__token_manage= token_manage
+        self.__call_time_out= call_time_out
         if host_cnf:
             for item in host_cnf:
                 self.host.register(
                     get_key('serverId', item),
                     get_key("host", item),
                     int(get_key("port", item)),
                     get_key("sniffer", item),
@@ -292,24 +294,24 @@
         state = -1
         ret = ""
         if method_type.upper() == "GET":
             logging.info("access api:(%s), method(%s)." % (uri, method_type))
             state, ret = GET(uri=uri,
                              post_data=kwargs,
                              http_headers=http_headers,
-                             time_out=15)
+                             time_out=self.__call_time_out)
         elif method_type.upper() == "POST":
             logging.info("access api:(%s), method(%s), postdata:%s." %
                          (uri, method_type, kwargs))
             state, ret = POST(
                 uri,
                 kwargs["data"] if "data" in kwargs else None,
                 content_type=ContentType.JSON,
                 http_headers=http_headers,
-                time_out=15,
+                time_out=self.__call_time_out,
             )
         elif method_type.upper() == "PUT":
             logging.info("access api:(%s), method(%s),postdata:%s." %
                          (uri, method_type, kwargs))
             # 还没有写PUT方法
             raise Exception("urllib PUT方法还没写.")
         elif method_type.upper() == "DELETE":
@@ -318,20 +320,20 @@
                          (uri, method_type))
             if "data" in kwargs:
                 state, ret = DELETE(
                     uri,
                     post_data=kwargs["data"],
                     http_headers=method_type,
                     content_type=ContentType.JSON,
-                    time_out=15,
+                    time_out=self.__call_time_out,
                 )
             else:
                 state, ret = DELETE(uri=uri,
                                     http_headers=method_type,
-                                    time_out=15)
+                                    time_out=self.__call_time_out)
         else:
             return {"state": -1, "msg": "uri(%s),method type %s error." % (uri, method_type)}
         if state == 200:
             try:
                 ret = json.loads(str(ret, encoding="utf-8"))
                 return {"state": ret["state"], "msg": ret["msg"]}
             except Exception as e:
@@ -443,40 +445,40 @@
             uri = self.__hit_method__(key).uri.strip('/')
             return "".join([host, '/', uri, '/']),host_conf["serverId"]
         except Exception as e:
             logging.error(e)
             return None
 
     @classmethod
-    def create_by_cnf(self, cnf,token_key="api-token",token_manage:token_manage= None):
+    def create_by_cnf(self, cnf,token_key="api-token",token_manage:token_manage= None,call_time_out=2):
         if isinstance(cnf, str):
             try:
                 cnf = json.loads(cnf)
             except Exception as e:
                 raise e
         return RPC_SERVICE(
             name=get_key('name', cnf),
             description=get_key('description', cnf),
             key=get_key('key', cnf).upper(),
             secret=get_key('secret', cnf),
             protocol=get_key('protocol', cnf),
             host_cnf=get_key('hosts', cnf),
             methods_cnf=get_key('methods', cnf),
             token_key=token_key,
-            token_manage=token_manage
+            token_manage=token_manage,
+            call_time_out=call_time_out
         )
 
 
 class RPC_SERVICE_CONF:
     uris: list = []
-    token: str = None
 
-    def __init__(self, uris, token):
+    def __init__(self, uris):
         self.uris = uris
-        self.token = token
+        #self.token = token
         for offset in range(0, len(self.uris)):
             self.uris[offset] = self.uris[offset].strip("/")
 
     def getUri(self):
         offset = len(self.uris)-1
         if offset > 0:
             return self.uris[Random.randint(0, offset-1)]+"/"
```

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Core/token.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Core/token.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Generic/Host.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Server/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.6.6/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/__init__.py` & `TDhelper-2.6.6/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.6.6/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/client.py` & `TDhelper-2.6.6/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.6.6/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.6.6/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/socket/server.py` & `TDhelper-2.6.6/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/websocket/protocol.py` & `TDhelper-2.6.6/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/network/websocket/server.py` & `TDhelper-2.6.6/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/reflect.py` & `TDhelper-2.6.6/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/control/D_33890.py` & `TDhelper-2.6.6/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/control/device.py` & `TDhelper-2.6.6/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/people/__init__.py` & `TDhelper-2.6.6/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/people/leg.py` & `TDhelper-2.6.6/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.6.6/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.6.6/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/struct/ankle.py` & `TDhelper-2.6.6/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/struct/base.py` & `TDhelper-2.6.6/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/struct/hip.py` & `TDhelper-2.6.6/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/struct/knee.py` & `TDhelper-2.6.6/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/robot/struct/toe.py` & `TDhelper-2.6.6/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.6.6/TDhelper/shellScripts/saasHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/simulate/json.py` & `TDhelper-2.6.6/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/structs/dir.py` & `TDhelper-2.6.6/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/web/obsolete_permission.py` & `TDhelper-2.6.6/TDhelper/web/obsolete_permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/web/obsolete_permissionHelper.py` & `TDhelper-2.6.6/TDhelper/web/obsolete_permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/web/utils/permission/client.py` & `TDhelper-2.6.6/TDhelper/web/utils/permission/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper/web/utils/permission/server.py` & `TDhelper-2.6.6/TDhelper/web/utils/permission/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.6.6/TDhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.6.5
+Version: 2.6.6
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
-Metadata-Version: 2.1 Name: TDhelper Version: 2.6.5 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.6.6 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.6.5/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.6.6/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/TDhelper.egg-info/requires.txt` & `TDhelper-2.6.6/TDhelper.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.6.5/setup.py` & `TDhelper-2.6.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.6.5",
+    version="2.6.6",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

