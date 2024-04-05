# Comparing `tmp/TDhelper-2.7.3.tar.gz` & `tmp/TDhelper-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.7.3.tar", last modified: Sun Mar 31 03:09:43 2024, max compression
+gzip compressed data, was "TDhelper-2.7.4.tar", last modified: Fri Apr  5 16:36:21 2024, max compression
```

## Comparing `TDhelper-2.7.3.tar` & `TDhelper-2.7.4.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2024-03-30 13:11:32.000000 TDhelper-2.7.3/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-03-31 03:09:43.926119 TDhelper-2.7.3/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2024-03-30 13:11:32.000000 TDhelper-2.7.3/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Decorators/performance.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/classEvent/meta.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Event/webEvent/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/MagicCls/test.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Msg/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Scheduler/service.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8542 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/Spider/contentExtraction.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/apiCore.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/bin/globalvar.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/ring.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2964 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/cache/webCache/webCacheFactory.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1116 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mongodb/objectId.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/mongodb/orm/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/attribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      691 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/field.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      194 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/field_type.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5506 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/meta copy.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5811 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/meta.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.896119 TDhelper-2.7.3/TDhelper/db/mongodb/orm/drives/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/drives/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1356 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/db/mongodb/orm/drives/conn.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mongodb/setting.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/db/mysql/setting.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/document/excel/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/excel/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3942 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/file.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      309 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/document/ini/test.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/classDocCfg.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/dictHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/dynamic/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/dynamic/delete__test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/generic/transformationType.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/m3u8_backup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/http/status/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.906119 TDhelper-2.7.3/TDhelper/network/rpc/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6574 2024-03-30 16:07:57.000000 TDhelper-2.7.3/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13184 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Client/service.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Core/obsolete_struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Core/struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1844 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Core/token.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Generic/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/network/rpc/Server/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/rpc/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/model/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/socket/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/reflect.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.916119 TDhelper-2.7.3/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/control/device.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/leg.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/people/vertebra.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/robot/struct/toe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/shellScripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/shellScripts/saasHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/simulate/json.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/structs/dir.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.3/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/obsolete_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/obsolete_permissionHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/web/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/web/utils/event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/event/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/event/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/event/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.926119 TDhelper-2.7.3/TDhelper/web/utils/permission/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/permission/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/permission/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2024-03-30 15:55:54.000000 TDhelper-2.7.3/TDhelper/web/utils/permission/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 03:09:43.886119 TDhelper-2.7.3/TDhelper.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       62 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-03-31 03:09:43.000000 TDhelper-2.7.3/TDhelper.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-31 03:09:43.926119 TDhelper-2.7.3/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1021 2024-03-31 03:09:39.000000 TDhelper-2.7.3/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2024-03-30 13:11:32.000000 TDhelper-2.7.4/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-04-05 16:36:21.751746 TDhelper-2.7.4/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2024-03-30 13:11:32.000000 TDhelper-2.7.4/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.631746 TDhelper-2.7.4/TDhelper/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.641746 TDhelper-2.7.4/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Decorators/performance.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.641746 TDhelper-2.7.4/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.641746 TDhelper-2.7.4/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/classEvent/meta.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.651746 TDhelper-2.7.4/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Event/webEvent/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.651746 TDhelper-2.7.4/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/MagicCls/test.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.651746 TDhelper-2.7.4/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Msg/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.651746 TDhelper-2.7.4/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Scheduler/service.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8542 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/Spider/contentExtraction.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/apiCore.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/bin/globalvar.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/ring.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2964 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/cache/webCache/webCacheFactory.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/db/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.671746 TDhelper-2.7.4/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1116 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mongodb/objectId.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/db/mongodb/orm/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/attribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      691 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/field.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      194 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/field_type.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5506 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/meta copy.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5811 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/meta.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/db/mongodb/orm/drives/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/drives/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1356 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/db/mongodb/orm/drives/conn.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mongodb/setting.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/db/mysql/setting.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/document/excel/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/excel/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3942 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/file.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.701746 TDhelper-2.7.4/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      309 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/document/ini/test.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/classDocCfg.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/dictHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/dynamic/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/dynamic/delete__test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/generic/transformationType.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.711746 TDhelper-2.7.4/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/m3u8_backup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.721746 TDhelper-2.7.4/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/http/status/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.721746 TDhelper-2.7.4/TDhelper/network/rpc/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.721746 TDhelper-2.7.4/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6799 2024-04-05 16:35:12.000000 TDhelper-2.7.4/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13184 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/rpc/Client/service.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/rpc/Core/obsolete_struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/rpc/Core/struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2299 2024-04-05 16:34:24.000000 TDhelper-2.7.4/TDhelper/network/rpc/Core/token.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Generic/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/network/rpc/Server/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/rpc/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/model/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/socket/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/reflect.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/control/device.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/leg.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.731746 TDhelper-2.7.4/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/people/vertebra.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/robot/struct/toe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/shellScripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/shellScripts/saasHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/simulate/json.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/structs/dir.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.4/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/obsolete_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/obsolete_permissionHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/web/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/web/utils/event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/event/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/event/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/event/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.751746 TDhelper-2.7.4/TDhelper/web/utils/permission/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/permission/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/permission/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2024-03-30 15:55:54.000000 TDhelper-2.7.4/TDhelper/web/utils/permission/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 16:36:21.641746 TDhelper-2.7.4/TDhelper.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       62 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-05 16:36:21.000000 TDhelper-2.7.4/TDhelper.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-05 16:36:21.751746 TDhelper-2.7.4/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1021 2024-04-05 16:36:09.000000 TDhelper-2.7.4/setup.py
```

### Comparing `TDhelper-2.7.3/LICENSE` & `TDhelper-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/PKG-INFO` & `TDhelper-2.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.7.3
+Version: 2.7.4
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
-Metadata-Version: 2.1 Name: TDhelper Version: 2.7.3 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.7.4 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.7.3/README.md` & `TDhelper-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Decorators/log.py` & `TDhelper-2.7.4/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Decorators/performance.py` & `TDhelper-2.7.4/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Event/Event.py` & `TDhelper-2.7.4/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Event/classEvent/event.py` & `TDhelper-2.7.4/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.7.4/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.7.4/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.7.4/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/MagicCls/model.py` & `TDhelper-2.7.4/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/MagicCls/test.py` & `TDhelper-2.7.4/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Msg/AppPush.py` & `TDhelper-2.7.4/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Msg/Config.py` & `TDhelper-2.7.4/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Msg/Email.py` & `TDhelper-2.7.4/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.7.4/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Msg/SMS.py` & `TDhelper-2.7.4/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Scheduler/base.py` & `TDhelper-2.7.4/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.7.4/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Scheduler/interface.py` & `TDhelper-2.7.4/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Scheduler/log_config.py` & `TDhelper-2.7.4/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Scheduler/service.py` & `TDhelper-2.7.4/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.7.4/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.7.4/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.7.4/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.7.4/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.7.4/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.7.4/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/models/status.py` & `TDhelper-2.7.4/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/regex.py` & `TDhelper-2.7.4/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/Spider/spiderPools.py` & `TDhelper-2.7.4/TDhelper/Spider/spiderPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/apiCore.py` & `TDhelper-2.7.4/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/bin/globalvar.py` & `TDhelper-2.7.4/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/memcache.py` & `TDhelper-2.7.4/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/pools.py` & `TDhelper-2.7.4/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/ring.py` & `TDhelper-2.7.4/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/webCache/interface.py` & `TDhelper-2.7.4/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.7.4/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.7.4/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/Db/base.py` & `TDhelper-2.7.4/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/base.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/__init__.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/attribute.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/field.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/field.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/meta copy.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/meta copy.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/core/meta.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/core/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mongodb/orm/drives/conn.py` & `TDhelper-2.7.4/TDhelper/db/mongodb/orm/drives/conn.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.7.4/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.7.4/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/document/excel/model.py` & `TDhelper-2.7.4/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/document/file.py` & `TDhelper-2.7.4/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/document/ini/meta.py` & `TDhelper-2.7.4/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/__init__.py` & `TDhelper-2.7.4/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/classDocCfg.py` & `TDhelper-2.7.4/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.7.4/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/dictHelper.py` & `TDhelper-2.7.4/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.7.4/TDhelper/generic/dynamic/base/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/dynamic/delete__test.py` & `TDhelper-2.7.4/TDhelper/generic/dynamic/delete__test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/findAttribute.py` & `TDhelper-2.7.4/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/recursion.py` & `TDhelper-2.7.4/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/requier.py` & `TDhelper-2.7.4/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/standard_result.py` & `TDhelper-2.7.4/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/threadPools.py` & `TDhelper-2.7.4/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/generic/transformationType.py` & `TDhelper-2.7.4/TDhelper/generic/transformationType.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.7.4/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/RPC.py` & `TDhelper-2.7.4/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/RPC1.py` & `TDhelper-2.7.4/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/http_helper.py` & `TDhelper-2.7.4/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.7.4/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/m3u8.py` & `TDhelper-2.7.4/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.7.4/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Client/rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,21 @@
             self.__LOGGER__.config.dictConfig(logger)
         self.__TOKEN_KEY__ = token_key if token_key else self.__TOKEN_KEY__
         self.__call_time_out= call_time_out
         self.__token_manage= token_manage(uri,service_conf.get("service_key",""),service_conf.get("secret",""))
         header = {
             "access-source":"rpc"
         }
-        if self.__token_manage.Token:
-            header.update({self.__TOKEN_KEY__:self.__token_manage.Token})
+        if self.__token_manage.Status:
+            if self.__token_manage.Token:
+                header.update({self.__TOKEN_KEY__:self.__token_manage.Token})
+            else:
+                raise Exception("rpc generate token error.%s"%self.__token_manage.ErrMsg)
+        else:
+            raise Exception(self.__token_manage.ErrMsg)
         uri = uri.rstrip("/")
         rpc_uri ="/".join([uri,path.lstrip("/")])
         if services:
             rpc_uri += "?key="+",".join(services)
         rpc_server_state = False
         for v in range(0, try_count):
             body = self.__get_conf__("/".join([uri,sniffer.lstrip("/")]), header)
```

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Client/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Core/obsolete_struct.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Core/obsolete_struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Core/struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Generic/Host.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Server/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.7.4/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/__init__.py` & `TDhelper-2.7.4/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.7.4/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/client.py` & `TDhelper-2.7.4/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.7.4/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.7.4/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/socket/server.py` & `TDhelper-2.7.4/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/websocket/protocol.py` & `TDhelper-2.7.4/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/network/websocket/server.py` & `TDhelper-2.7.4/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/reflect.py` & `TDhelper-2.7.4/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/control/D_33890.py` & `TDhelper-2.7.4/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/control/device.py` & `TDhelper-2.7.4/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/people/__init__.py` & `TDhelper-2.7.4/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/people/leg.py` & `TDhelper-2.7.4/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.7.4/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.7.4/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/struct/ankle.py` & `TDhelper-2.7.4/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/struct/base.py` & `TDhelper-2.7.4/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/struct/hip.py` & `TDhelper-2.7.4/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/struct/knee.py` & `TDhelper-2.7.4/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/robot/struct/toe.py` & `TDhelper-2.7.4/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.7.4/TDhelper/shellScripts/saasHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/simulate/json.py` & `TDhelper-2.7.4/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/structs/dir.py` & `TDhelper-2.7.4/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/web/obsolete_permission.py` & `TDhelper-2.7.4/TDhelper/web/obsolete_permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/web/obsolete_permissionHelper.py` & `TDhelper-2.7.4/TDhelper/web/obsolete_permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/web/utils/permission/client.py` & `TDhelper-2.7.4/TDhelper/web/utils/permission/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper/web/utils/permission/server.py` & `TDhelper-2.7.4/TDhelper/web/utils/permission/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.7.4/TDhelper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.7.3
+Version: 2.7.4
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
-Metadata-Version: 2.1 Name: TDhelper Version: 2.7.3 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.7.4 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.7.3/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.7.4/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.3/setup.py` & `TDhelper-2.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.7.3",
+    version="2.7.4",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

