# Comparing `tmp/quorum-0.8.2.tar.gz` & `tmp/quorum-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quorum-0.8.2.tar", last modified: Wed Aug  9 10:03:47 2023, max compression
+gzip compressed data, was "dist/quorum-0.8.3.tar", last modified: Fri Apr  5 10:44:01 2024, max compression
```

## Comparing `quorum-0.8.2.tar` & `quorum-0.8.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 10:03:47.000000 quorum-0.8.2/
--rw-r--r--   0 root         (0) root         (0)       67 2023-08-09 10:03:47.000000 quorum-0.8.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 10:03:47.000000 quorum-0.8.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1533 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 10:03:35.000000 quorum-0.8.2/src/quorum.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2947 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum/
--rw-r--r--   0 root         (0) root         (0)     1446 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/common.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/export.py
--rw-r--r--   0 root         (0) root         (0)     8284 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/daemon.py
--rw-r--r--   0 root         (0) root         (0)    10401 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/structures.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/meta.py
--rw-r--r--   0 root         (0) root         (0)    14014 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/log.py
--rw-r--r--   0 root         (0) root         (0)    14572 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/data.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/defines.py
--rw-r--r--   0 root         (0) root         (0)    39989 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/base.py
--rw-r--r--   0 root         (0) root         (0)    21292 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/validation.py
--rw-r--r--   0 root         (0) root         (0)    14534 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/execution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 10:03:47.000000 quorum-0.8.2/src/quorum/test/
--rw-r--r--   0 root         (0) root         (0)     3637 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/export.py
--rw-r--r--   0 root         (0) root         (0)     7104 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/structures.py
--rw-r--r--   0 root         (0) root         (0)     4480 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/log.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/data.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/base.py
--rw-r--r--   0 root         (0) root         (0)    12229 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/validation.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/execution.py
--rw-r--r--   0 root         (0) root         (0)    30269 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/util.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/config.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/httpc.py
--rw-r--r--   0 root         (0) root         (0)    29867 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/model.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/amazon.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/typesf.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/crypt.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/acl.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/mail.py
--rw-r--r--   0 root         (0) root         (0)     4429 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/mock.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/jsonf.py
--rw-r--r--   0 root         (0) root         (0)     8653 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/mongodb.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/util.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/route.py
--rw-r--r--   0 root         (0) root         (0)     8312 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/config.py
--rw-r--r--   0 root         (0) root         (0)    13063 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/legacy.py
--rw-r--r--   0 root         (0) root         (0)    29352 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/httpc.py
--rw-r--r--   0 root         (0) root         (0)   118762 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/model.py
--rw-r--r--   0 root         (0) root         (0)     4468 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/extras.py
--rw-r--r--   0 root         (0) root         (0)     4504 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/observer.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/amazon.py
--rw-r--r--   0 root         (0) root         (0)    35346 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/typesf.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/storage.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/unit_test.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/formats.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/crypt.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/acl.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/date.py
--rw-r--r--   0 root         (0) root         (0)    11475 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/mail.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/session.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/amqp.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/pusherc.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/info.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/template.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/errors.py
--rw-r--r--   0 root         (0) root         (0)     7195 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/redisdb.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-08-09 10:03:30.000000 quorum-0.8.2/src/quorum/request.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-08-09 10:03:30.000000 quorum-0.8.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-08-09 10:03:30.000000 quorum-0.8.2/README.md
--rw-r--r--   0 root         (0) root         (0)     2947 2023-08-09 10:03:47.000000 quorum-0.8.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:44:01.000000 quorum-0.8.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:44:01.000000 quorum-0.8.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum/
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/request.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/unit_test.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/template.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/amqp.py
+-rw-r--r--   0 root         (0) root         (0)     5856 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/crypt.py
+-rw-r--r--   0 root         (0) root         (0)    29546 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/httpc.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/redisdb.py
+-rw-r--r--   0 root         (0) root         (0)    14236 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/execution.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/date.py
+-rw-r--r--   0 root         (0) root         (0)    36349 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/typesf.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/common.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/meta.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/mail.py
+-rw-r--r--   0 root         (0) root         (0)     9496 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/defines.py
+-rw-r--r--   0 root         (0) root         (0)     8952 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/mongodb.py
+-rw-r--r--   0 root         (0) root         (0)    14665 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/data.py
+-rw-r--r--   0 root         (0) root         (0)    40186 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/base.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/export.py
+-rw-r--r--   0 root         (0) root         (0)    12316 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/acl.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/jsonf.py
+-rw-r--r--   0 root         (0) root         (0)    22139 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/validation.py
+-rw-r--r--   0 root         (0) root         (0)     5332 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/session.py
+-rw-r--r--   0 root         (0) root         (0)     8062 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/route.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/config.py
+-rw-r--r--   0 root         (0) root         (0)     7418 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/storage.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/pusherc.py
+-rw-r--r--   0 root         (0) root         (0)     8109 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/info.py
+-rw-r--r--   0 root         (0) root         (0)     4213 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/formats.py
+-rw-r--r--   0 root         (0) root         (0)    10474 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/observer.py
+-rw-r--r--   0 root         (0) root         (0)    13891 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/log.py
+-rw-r--r--   0 root         (0) root         (0)    57561 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/util.py
+-rw-r--r--   0 root         (0) root         (0)   120287 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/model.py
+-rw-r--r--   0 root         (0) root         (0)    14954 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/legacy.py
+-rw-r--r--   0 root         (0) root         (0)     4283 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/extras.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/amazon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum/test/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/crypt.py
+-rw-r--r--   0 root         (0) root         (0)     8135 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/httpc.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/execution.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/typesf.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/mail.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/data.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/base.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/export.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/acl.py
+-rw-r--r--   0 root         (0) root         (0)    10530 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/validation.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/config.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/mock.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/log.py
+-rw-r--r--   0 root         (0) root         (0)    31353 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/util.py
+-rw-r--r--   0 root         (0) root         (0)    29363 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/model.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-05 10:43:43.000000 quorum-0.8.3/src/quorum/test/amazon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:43:48.000000 quorum-0.8.3/src/quorum.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-04-05 10:44:01.000000 quorum-0.8.3/src/quorum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-05 10:43:43.000000 quorum-0.8.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-05 10:44:01.000000 quorum-0.8.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-05 10:43:43.000000 quorum-0.8.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-04-05 10:44:01.000000 quorum-0.8.3/PKG-INFO
```

### Comparing `quorum-0.8.2/src/quorum.egg-info/SOURCES.txt` & `quorum-0.8.3/src/quorum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum-0.8.2/src/quorum.egg-info/PKG-INFO` & `quorum-0.8.3/src/quorum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum
-Version: 0.8.2
+Version: 0.8.3
 Summary: Quorum Extensions for Flask
 Home-page: http://flask-quorum.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [![Quorum Extensions for Flask](res/logo.png)](http://flask-quorum.hive.pt)
```

### Comparing `quorum-0.8.2/src/quorum/common.py` & `quorum-0.8.3/src/quorum/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,32 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
+
 def base():
     from . import base
+
     return base
 
+
 def model():
     from . import model
+
     return model
 
+
 def is_devel():
     return base().is_devel()
```

### Comparing `quorum-0.8.2/src/quorum/export.py` & `quorum-0.8.3/src/quorum/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -62,143 +53,149 @@
 
 JOIN = 4
 """ Join strategy for conflict solving in document collision, that
 basically adds new fields or updates existing fields in a previously
 existing document, this strategy does not remove extra fields existing
 in the previous document """
 
+
 class ExportManager(object):
 
     adapter = None
     single = None
     multiple = None
 
-    def __init__(self, adapter, single = (), multiple = ()):
+    def __init__(self, adapter, single=(), multiple=()):
         self.adapter = adapter
         self.single = single
         self.multiple = multiple
 
-    def import_data(self, file_path, policy = IGNORE):
+    def import_data(self, file_path, policy=IGNORE):
         temporary_path = tempfile.mkdtemp()
         base_path = temporary_path
         single_path = os.path.join(base_path, "settings")
 
         self._deploy_zip(file_path, temporary_path)
 
         for name, key in self.single:
             collection = self.adapter.collection(name)
             source_path = os.path.join(single_path, "%s.json" % name)
             file = open(source_path, "rb")
-            try: data = file.read()
-            finally: file.close()
-            self._import_single(
-                collection,
-                data,
-                key = key,
-                policy = policy
-            )
+            try:
+                data = file.read()
+            finally:
+                file.close()
+            self._import_single(collection, data, key=key, policy=policy)
 
         for name, key in self.multiple:
             source_directory = os.path.join(base_path, name)
-            if not os.path.exists(source_directory): continue
+            if not os.path.exists(source_directory):
+                continue
 
             collection = self.adapter.collection(name)
             items = os.listdir(source_directory)
             data = []
 
             for item in items:
                 value, _extension = os.path.splitext(item)
                 source_path = os.path.join(source_directory, item)
                 file = open(source_path, "rb")
-                try: _data = file.read()
-                finally: file.close()
+                try:
+                    _data = file.read()
+                finally:
+                    file.close()
 
                 data.append((value, _data))
 
-            self._import_multiple(
-                collection,
-                data,
-                key = key,
-                policy = policy
-            )
+            self._import_multiple(collection, data, key=key, policy=policy)
 
     def export_data(self, file_path):
         encoder = self.adapter.encoder()
         temporary_path = tempfile.mkdtemp()
         base_path = temporary_path
         single_path = os.path.join(base_path, "settings")
-        if not os.path.exists(single_path): os.makedirs(single_path)
+        if not os.path.exists(single_path):
+            os.makedirs(single_path)
 
         for name, key in self.single:
             collection = self.adapter.collection(name)
-            data = self._export_single(collection, key = key, encoder = encoder)
+            data = self._export_single(collection, key=key, encoder=encoder)
             target_path = os.path.join(single_path, "%s.json" % name)
             file = open(target_path, "wb")
-            try: file.write(data)
-            finally: file.close()
+            try:
+                file.write(data)
+            finally:
+                file.close()
 
         for name, key in self.multiple:
             collection = self.adapter.collection(name)
-            data = self._export_multiple(collection, key = key, encoder = encoder)
+            data = self._export_multiple(collection, key=key, encoder=encoder)
 
             target_directory = os.path.join(base_path, name)
-            if not os.path.exists(target_directory): os.makedirs(target_directory)
+            if not os.path.exists(target_directory):
+                os.makedirs(target_directory)
 
             for value, _data in data:
                 target_path = os.path.join(target_directory, "%s.json" % value)
                 file = open(target_path, "wb")
-                try: file.write(_data)
-                finally: file.close()
+                try:
+                    file.write(_data)
+                finally:
+                    file.close()
 
         self._create_zip(file_path, temporary_path)
 
-    def _import_single(self, collection, data, key, policy = IGNORE):
+    def _import_single(self, collection, data, key, policy=IGNORE):
         # loads the provided JSON data as a sequence of key value items
         # and then starts loading all the values into the data source
         data = data.decode("utf-8")
         data_s = json.loads(data)
         for _key, entity in data_s.items():
             # verifies if the "native" object id value for the database
             # definition exists and if that's the case tries to convert
             # the value from the "underlying" string value to object
             # identifier, defaulting to a string value if it fails, note
             # that in case the underlying identifiers does not exists a
             # new value is generated using the pre-defined strategy
             if "_id" in entity:
-                try: entity["_id"] = self.adapter.object_id(entity["_id"])
-                except Exception: entity["_id"] = entity["_id"]
-            else: entity["_id"] = self.adapter.object_id()
+                try:
+                    entity["_id"] = self.adapter.object_id(entity["_id"])
+                except Exception:
+                    entity["_id"] = entity["_id"]
+            else:
+                entity["_id"] = self.adapter.object_id()
 
             # retrieves the key value for the current entity to
             # be inserted and then tries to retrieve an existing
             # entity for the same key, to avoid duplicated entry
             value = entity.get(key, None)
-            if value: entity_e = collection.find_one({key : value})
-            else: entity_e = None
+            if value:
+                entity_e = collection.find_one({key: value})
+            else:
+                entity_e = None
 
             # in case there's no existing entity for the same key
             # (normal situation) only need to insert the new entity
             # otherwise must apply the selected conflict policy for
             # the resolution of the data source conflict
-            if not entity_e: collection.insert(entity)
-            elif policy == IGNORE: continue
+            if not entity_e:
+                collection.insert(entity)
+            elif policy == IGNORE:
+                continue
             elif policy == OVERWRITE:
-                collection.remove({key : value})
+                collection.remove({key: value})
                 collection.insert(entity)
             elif policy == DUPLICATE:
                 collection.insert(entity)
             elif policy == JOIN:
-                if "_id" in entity: del entity["_id"]
-                collection.update({
-                    "_id" : entity_e["_id"]
-                }, {
-                    "$set" : entity
-                })
+                if "_id" in entity:
+                    del entity["_id"]
+                collection.update({"_id": entity_e["_id"]}, {"$set": entity})
 
-    def _import_multiple(self, collection, data, key, policy = IGNORE):
+    def _import_multiple(self, collection, data, key, policy=IGNORE):
         # iterates over the complete set of data element to load
         # the JSON contents and then load the corresponding entity
         # value into the data source
         for _value, _data in data:
             # loads the current data in iteration from the file
             # as the entity to be loaded into the data source
             _data = _data.decode("utf-8")
@@ -207,104 +204,110 @@
             # verifies if the "native" object id value for the database
             # definition exists and if that's the case tries to convert
             # the value from the "underlying" string value to object
             # identifier, defaulting to a string value if it fails, note
             # that in case the underlying identifiers does not exists a
             # new value is generated using the pre-defined strategy
             if "_id" in entity:
-                try: entity["_id"] = self.adapter.object_id(entity["_id"])
-                except Exception: entity["_id"] = entity["_id"]
-            else: entity["_id"] = self.adapter.object_id()
+                try:
+                    entity["_id"] = self.adapter.object_id(entity["_id"])
+                except Exception:
+                    entity["_id"] = entity["_id"]
+            else:
+                entity["_id"] = self.adapter.object_id()
 
             # retrieves the key value for the current entity to
             # be inserted and then tries to retrieve an existing
             # entity for the same key, to avoid duplicated entry
             value = entity.get(key, None)
-            if value: entity_e = collection.find_one({key : value})
-            else: entity_e = None
+            if value:
+                entity_e = collection.find_one({key: value})
+            else:
+                entity_e = None
 
             # in case there's no existing entity for the same key
             # (normal situation) only need to insert the new entity
             # otherwise must apply the selected conflict policy for
             # the resolution of the data source conflict
-            if not entity_e: collection.insert(entity)
-            elif policy == IGNORE: continue
+            if not entity_e:
+                collection.insert(entity)
+            elif policy == IGNORE:
+                continue
             elif policy == OVERWRITE:
-                collection.remove({key : value})
+                collection.remove({key: value})
                 collection.insert(entity)
             elif policy == DUPLICATE:
                 collection.insert(entity)
             elif policy == JOIN:
-                if "_id" in entity: del entity["_id"]
-                collection.update({
-                    "_id" : entity_e["_id"]
-                }, {
-                    "$set" : entity
-                })
+                if "_id" in entity:
+                    del entity["_id"]
+                collection.update({"_id": entity_e["_id"]}, {"$set": entity})
 
-    def _export_single(self, collection, key = "_id", encoder = None):
+    def _export_single(self, collection, key="_id", encoder=None):
         entities = collection.find()
         _entities = {}
         for entity in entities:
             value = entity[key]
             value_s = self._to_key(value)
             _entities[value_s] = entity
-        data = json.dumps(_entities, cls = encoder)
+        data = json.dumps(_entities, cls=encoder)
         data = legacy.bytes(data)
         return data
 
-    def _export_multiple(self, collection, key = "_id", encoder = None):
+    def _export_multiple(self, collection, key="_id", encoder=None):
         entities = collection.find()
         for entity in entities:
             value = entity[key]
             value_s = self._to_key(value)
             value_s = self._escape_key(value_s)
-            _data = json.dumps(entity, cls = encoder)
+            _data = json.dumps(entity, cls=encoder)
             _data = legacy.bytes(_data)
             yield (value_s, _data)
 
     def _to_key(self, key):
         key_t = type(key)
-        if key_t in legacy.STRINGS: return key
+        if key_t in legacy.STRINGS:
+            return key
         key = legacy.UNICODE(key)
         return key
 
     def _escape_key(self, key):
         return key.replace(":", "_")
 
     def _deploy_zip(self, zip_path, path):
-        zip_file = zipfile.ZipFile(zip_path, mode = "r")
+        zip_file = zipfile.ZipFile(zip_path, mode="r")
 
-        try: zip_file.extractall(path)
-        finally: zip_file.close()
+        try:
+            zip_file.extractall(path)
+        finally:
+            zip_file.close()
 
     def _create_zip(self, zip_path, path):
         zip_file = zipfile.ZipFile(
-            zip_path,
-            mode = "w",
-            compression = zipfile.ZIP_DEFLATED,
-            allowZip64 = True
+            zip_path, mode="w", compression=zipfile.ZIP_DEFLATED, allowZip64=True
         )
 
         try:
             list = os.listdir(path)
             for name in list:
                 _path = os.path.join(path, name)
                 is_file = os.path.isfile(_path)
 
-                if is_file: zip_file.write(_path)
-                else: self.__add_to_zip(zip_file, _path, base = path)
+                if is_file:
+                    zip_file.write(_path)
+                else:
+                    self.__add_to_zip(zip_file, _path, base=path)
         finally:
             zip_file.close()
 
-    def __add_to_zip(self, zip_file, path, base = ""):
+    def __add_to_zip(self, zip_file, path, base=""):
         list = os.listdir(path)
         for name in list:
             _path = os.path.join(path, name)
-            _path_out = _path[len(base):]
+            _path_out = _path[len(base) :]
             _path_out = _path_out.replace("\\", "/")
             _path_out = _path_out.strip("/")
 
             if os.path.isfile(_path):
                 zip_file.write(_path, _path_out)
             elif os.path.isdir(_path):
-                self.__add_to_zip(zip_file, _path, base = base)
+                self.__add_to_zip(zip_file, _path, base=base)
```

### Comparing `quorum-0.8.2/src/quorum/daemon.py` & `quorum-0.8.3/src/quorum/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,27 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import sys
 import time
 import atexit
 import signal
 
+
 class Daemon(object):
     """
     A generic daemon class that provides the general
     daemon capabilities. In order to inherit the daemon
     capabilities override the run method.
     """
 
@@ -62,15 +54,17 @@
     """ The file path to the file to be used
     as the standard output of the created process """
 
     stderr = None
     """ The file path to the file to be used
     as the standard error of the created process """
 
-    def __init__(self, pid_file, stdin = "/dev/null", stdout = "/dev/null", stderr = "/dev/null"):
+    def __init__(
+        self, pid_file, stdin="/dev/null", stdout="/dev/null", stderr="/dev/null"
+    ):
         """
         Constructor of the class.
 
         :type pidfile: String
         :param pidfile: The path to the pid file.
         :type stdin: String
         :param stdin: The file path to the file to be used
@@ -84,15 +78,15 @@
         """
 
         self.pidfile = pid_file
         self.stdin = stdin
         self.stdout = stdout
         self.stderr = stderr
 
-    def daemonize(self, register = True):
+    def daemonize(self, register=True):
         """
         Do the UNIX double-fork magic, check Stevens "Advanced
         Programming in the UNIX Environment" for details (ISBN
         0201563177).
 
         This is considered the main method for the execution
         of the daemon strategy.
@@ -100,33 +94,35 @@
         :type register: bool
         :param register: If a cleanup function should be register for
         the at exit operation.
         :see: http://www.erlenstar.demon.co.uk/unix/faq_2.html#SEC16
         """
 
         try:
-            pid = os.fork() #@UndefinedVariable
-            if pid > 0: sys.exit(0)
+            pid = os.fork()  # @UndefinedVariable
+            if pid > 0:
+                sys.exit(0)
         except OSError as error:
             sys.stderr.write(
                 "first fork failed: %d (%s)\n" % (error.errno, error.strerror)
             )
             sys.exit(1)
 
         # decouples the current process from parent environment
         # should create a new group of execution
         os.chdir("/")
-        os.setsid() #@UndefinedVariable
+        os.setsid()  # @UndefinedVariable
         os.umask(0)
 
         try:
             # runs the second for and then exits from
             # the "second" parent process
-            pid = os.fork() #@UndefinedVariable
-            if pid > 0: sys.exit(0)
+            pid = os.fork()  # @UndefinedVariable
+            if pid > 0:
+                sys.exit(0)
         except OSError as error:
             sys.stderr.write(
                 "second fork failed: %d (%s)\n" % (error.errno, error.strerror)
             )
             sys.exit(1)
 
         # redirect standard file descriptors
@@ -142,15 +138,15 @@
         # write pidfile, updating the data in it
         # this should mark the process as running
         register and atexit.register(self.cleanup)
         register and signal.signal(signal.SIGTERM, self.cleanup_s)
         pid = str(os.getpid())
         open(self.pidfile, "wb+").write("%s\n" % pid)
 
-    def start(self, register = True):
+    def start(self, register=True):
         try:
             # checks for a pidfile to check if the daemon
             # already runs, in such case retrieves the pid
             # of the executing daemon
             pid_file = open(self.pidfile, "rb")
             pid_contents = pid_file.read().strip()
             pid = int(pid_contents)
@@ -164,15 +160,15 @@
         if pid:
             message = "pidfile %s already exists, daemon already running ?\n"
             sys.stderr.write(message % self.pidfile)
             sys.exit(1)
 
         # daemonizes the current process and then starts
         # the daemon structures (runs the process)
-        self.daemonize(register = register)
+        self.daemonize(register=register)
         self.run()
 
     def stop(self):
         try:
             # checks for a pidfile to check if the daemon
             # already runs, in such case retrieves the pid
             # of the executing daemon
@@ -186,15 +182,15 @@
         if not pid:
             message = "pidfile %s does not exist, daemon not running ?\n"
             sys.stderr.write(message % self.pidfile)
             return
 
         try:
             while True:
-                os.kill(pid, signal.SIGTERM) #@UndefinedVariable
+                os.kill(pid, signal.SIGTERM)  # @UndefinedVariable
                 time.sleep(0.1)
         except OSError as error:
             error = str(error)
             if error.find("No such process") > 0:
                 pid_exists = os.path.exists(self.pidfile)
                 pid_exists and os.remove(self.pidfile)
             else:
```

### Comparing `quorum-0.8.2/src/quorum/exceptions.py` & `quorum-0.8.3/src/quorum/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,26 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import uuid
 
 from . import common
 from . import legacy
 
+
 class BaseError(RuntimeError):
     """
     The base error class from which all the error
     classes should inherit, contains basic functionality
     to be inherited by all the "errors".
     """
 
@@ -62,42 +54,48 @@
         RuntimeError.__init__(self, message)
         self.message = message
         self.meta = None
         self._uid = None
 
     @property
     def uid(self):
-        if self._uid: return self._uid
+        if self._uid:
+            return self._uid
         self._uid = uuid.uuid4()
         return self._uid
 
     def set_meta(self, name, value):
-        if not self.meta: self.meta = {}
+        if not self.meta:
+            self.meta = {}
         self.meta[name] = value
 
     def del_meta(self, name):
-        if not self.meta: return
-        if not name in self.meta: return
+        if not self.meta:
+            return
+        if not name in self.meta:
+            return
         del self.meta[name]
 
+
 class ServerInitError(BaseError):
     """
     The server initialization error that represents a
     problem in the boot process for the server, this
     error should not be raised during server runtime.
     """
 
     server = None
     """ The name (description) of the server that raised
     the initialization problem """
 
-    def __init__(self, message, server = None):
+    def __init__(self, message, server=None):
         BaseError.__init__(self, message)
         self.server = server
 
+
 class ModuleNotFound(BaseError):
     """
     The module not found error that represents a
     problem created by the failure to load a required module.
     This kind of error should be handled accordingly.
     """
 
@@ -105,45 +103,49 @@
     """ The name (description) of the module that failed
     to load and raised the problem """
 
     def __init__(self, name):
         BaseError.__init__(self, "Failed to load '%s' module" % name)
         self.name = name
 
+
 class OperationalError(BaseError):
     """
     The operational error class that should represent any
     error resulting from a business logic error.
     """
 
     code = 500
     """ The code to be used in the consequent serialization
     of the error in an HTTP response """
 
-    def __init__(self, message, code = 500):
+    def __init__(self, message, code=500):
         BaseError.__init__(self, message)
         self.code = code
 
+
 class AssertionError(OperationalError):
     """
     Error raised for failure to meet any pre-condition or
     assertion for a certain data set.
     """
 
     pass
 
+
 class NotFoundError(OperationalError):
     """
     Error originated from an operation that was not able
     to be performed because it was not able to found the
     requested entity/value as defined by specification.
     """
 
-    def __init__(self, message, code = 404):
-        OperationalError.__init__(self, message, code = code)
+    def __init__(self, message, code=404):
+        OperationalError.__init__(self, message, code=code)
+
 
 class ValidationError(OperationalError):
     """
     Error raised when a validation on the model fails
     the error should associate a name in the model with
     a message describing the validation failure.
     """
@@ -158,38 +160,44 @@
 
     def __init__(self, errors, model):
         OperationalError.__init__(self, "Validation of submitted data failed", 400)
         self.errors = errors
         self.model = model
         self.set_meta("errors", self.errors)
 
-    def errors_s(self, encoding = "utf-8"):
-        if not self.errors: return ""
+    def errors_s(self, encoding="utf-8"):
+        if not self.errors:
+            return ""
         buffer = []
         is_first = True
         for name, errors in legacy.iteritems(self.errors):
             for error in errors:
                 is_bytes = legacy.is_bytes(error)
-                if is_bytes: error = error.decode(encoding)
-                if is_first: is_first = False
-                else: buffer.append(", ")
+                if is_bytes:
+                    error = error.decode(encoding)
+                if is_first:
+                    is_first = False
+                else:
+                    buffer.append(", ")
                 buffer.append(name)
                 buffer.append(" => ")
                 buffer.append(error)
         return legacy.u("").join(buffer)
 
+
 class NotImplementedError(OperationalError):
     """
     Error to be raised when a certain feature or route is not
     yet implemented or is not meant to be implemented at the
     defined abstraction level.
     """
 
-    def __init__(self, message, code = 501):
-        OperationalError.__init__(self, message, code = code)
+    def __init__(self, message, code=501):
+        OperationalError.__init__(self, message, code=code)
+
 
 class BaseInternalError(RuntimeError):
     """
     The base error class from which all the error
     classes should inherit, contains basic functionality
     to be inherited by all the internal "errors".
     """
@@ -204,27 +212,32 @@
     should be structured data ready to be serializable """
 
     def __init__(self, message):
         RuntimeError.__init__(self, message)
         self.message = message
         self.meta = None
 
-    def get_meta(self, name, default = None):
-        if not self.meta: return default
+    def get_meta(self, name, default=None):
+        if not self.meta:
+            return default
         return self.meta.get(name, default)
 
     def set_meta(self, name, value):
-        if not self.meta: self.meta = {}
+        if not self.meta:
+            self.meta = {}
         self.meta[name] = value
 
     def del_meta(self, name):
-        if not self.meta: return
-        if not name in self.meta: return
+        if not self.meta:
+            return
+        if not name in self.meta:
+            return
         del self.meta[name]
 
+
 class ValidationInternalError(BaseInternalError):
     """
     Error raised when a validation on the model fails
     the error should associate a name in the model with
     a message describing the validation failure.
     """
 
@@ -232,48 +245,53 @@
     """ The name of the attribute that failed
     the validation, for latter reference """
 
     def __init__(self, name, message):
         BaseInternalError.__init__(self, message)
         self.name = name
 
+
 class ValidationMultipleError(ValidationInternalError):
     """
     Exception/error considered to be equivalent to the
     validation internal error, with the exception that it
     may handle multiple errors at the same time.
     """
 
     errors = []
     """ The sequence containing the multiple errors associated
     with the validation multiple error """
 
-    def __init__(self, name = None, message = None):
+    def __init__(self, name=None, message=None):
         ValidationInternalError.__init__(self, name, message)
         self.errors = []
         self.set_meta("errors", self.errors)
 
     def add_error(self, name, message):
-        if not self.name: self.name = name
-        if not self.message: self.message = message
+        if not self.name:
+            self.name = name
+        if not self.message:
+            self.message = message
         self.errors.append((name, message))
 
     def add_exception(self, exception):
         self.add_error(exception.name, exception.message)
 
+
 class HTTPError(BaseError):
     """
     Error raised when an HTTP (client) related issue
     arises, most of the problems should occur during
     the communication between client and server.
     """
 
     def __init__(self, message):
         BaseError.__init__(self, message)
 
+
 class HTTPDataError(HTTPError):
     """
     Specialized HTTP error for data based stream where both
     the error code and message are known.
 
     A special error attribute is used store the original error
     that gave origin to this exception.
@@ -285,27 +303,33 @@
     of the underlying internal buffer """
 
     _data = None
     """ The underlying/internal data attribute that is
     going to be used to cache the binary contents of the
     error associated with this exception (data) stream """
 
-    def __init__(self, error, code = None, message = None, extended = None):
+    def __init__(self, error, code=None, message=None, extended=None):
         message = message or "Problem in the HTTP request"
-        if extended == None: extended = common.base().is_devel()
-        if code: message = "[%d] %s" % (code, message)
+        if extended == None:
+            extended = common.base().is_devel()
+        if code:
+            message = "[%d] %s" % (code, message)
         if extended:
-            data = self.read(error = error)
-            try: data = data.decode("utf-8")
-            except Exception: data = legacy.str(data)
-            if data: message = message + "\n" + data if message else data
+            data = self.read(error=error)
+            try:
+                data = data.decode("utf-8")
+            except Exception:
+                data = legacy.str(data)
+            if data:
+                message = message + "\n" + data if message else data
         HTTPError.__init__(self, message)
         self.code = code
         self.error = error
 
+
 class JSONError(HTTPError):
     """
     Error raised when a JSON based HTTP communication
     fails or is not accepted by the server pear.
     """
 
     data = None
@@ -314,13 +338,14 @@
 
     def __init__(self, data):
         HTTPError.__init__(self, "Problem requesting JSON data")
         self.data = data
 
     def __str__(self):
         exception_s = HTTPError.__str__(self)
-        if not self.data: exception_s
+        if not self.data:
+            exception_s
         exception = self.data.get("exception", {})
         return exception.get("message", exception_s)
 
     def get_data(self):
         return self.data
```

### Comparing `quorum-0.8.2/src/quorum/structures.py` & `quorum-0.8.3/src/quorum/structures.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,40 +18,33 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 
+
 class OrderedDict(dict):
 
-    def __init__(self, value = None, *args, **kwargs):
+    def __init__(self, value=None, *args, **kwargs):
         object.__init__(self, *args, **kwargs)
         self._list = list()
         self._dict = dict()
         self._items = dict()
         is_dict = isinstance(value, dict)
-        if not is_dict: return
+        if not is_dict:
+            return
         self._from_dict(value)
 
     def __str__(self):
         self._verify()
         return self._list.__str__()
 
     def __unicode__(self):
@@ -78,54 +71,55 @@
         self._verify()
         return self.delete(key)
 
     def __contains__(self, item):
         self._verify()
         return self._dict.__contains__(item)
 
-    def __iter__(self, verify = True):
-        self._verify(force = verify)
+    def __iter__(self, verify=True):
+        self._verify(force=verify)
         return self._list.__iter__()
 
-    def items(self, verify = True):
-        self._verify(force = verify)
+    def items(self, verify=True):
+        self._verify(force=verify)
         return self
 
-    def iteritems(self, verify = True):
-        self._verify(force = verify)
+    def iteritems(self, verify=True):
+        self._verify(force=verify)
         return self
 
     def item(self, key):
         self._verify()
         return self._items.__getitem__(key)
 
     def sort(self, *args, **kwargs):
         self._verify()
         return self._list.sort(*args, **kwargs)
 
     def append(self, value):
         self._verify()
         return self.push(value)
 
-    def pop(self, index = -1):
+    def pop(self, index=-1):
         self._verify()
         value = self._list.pop(index)
         key, _value = value
         del self._dict[key]
         del self._items[key]
         return value
 
     def push(self, value):
         self._verify()
         key, value = value
         self.set(key, value)
 
-    def get(self, key, default = None):
+    def get(self, key, default=None):
         self._verify()
-        if not key in self._dict: return default
+        if not key in self._dict:
+            return default
         return self._dict[key]
 
     def set(self, key, value):
         self._verify()
         if key in self:
             item = self.item(key)
             item[1] = value
@@ -143,15 +137,15 @@
         del self._items[key]
 
     def empty(self):
         del self._list[:]
         self._dict.clear()
         self._items.clear()
 
-    def _from_dict(self, base, empty = True):
+    def _from_dict(self, base, empty=True):
         """
         Builds the ordered dictionary from a base (unordered) one
         sorting all of its items accordingly.
 
         Notice that the reference to the base dictionary object
         is kept untouched so that any change in this dict implies
         also a change in the underlying base dictionary.
@@ -160,90 +154,101 @@
         :param base: The base dictionary to be used in the construction
         of this ordered one.
         :type clear: bool
         :param empty: If the current structure should be cleared
         to an empty state before using the dictionary.
         """
 
-        if empty: self.empty()
+        if empty:
+            self.empty()
         keys = list(base.keys())
         keys.sort()
         for key in keys:
             value = base[key]
             self.set(key, value)
-        if empty: self._dict = base
+        if empty:
+            self._dict = base
 
-    def _verify(self, force = False):
+    def _verify(self, force=False):
         """
         Runs the consistency check on the current structure so that
         if any change occurs in the base dictionary (either adding
         or removal) it gets reflected on the current ordered one.
 
         This method should be as efficient as possible as it's going
         to run on every single iteration process.
 
         :type force: bool
         :param force: Flag that control if the verification process
         should be executed if if the length of the structures is
         exactly the same.
         """
 
-        if not force and len(self._list) == len(self._dict): return
+        if not force and len(self._list) == len(self._dict):
+            return
 
         for value in list(self._list):
             key, _value = value
             exists = True
             exists &= key in self._dict
             exists &= key in self._items
-            if exists: continue
+            if exists:
+                continue
             self._list.remove(value)
 
-        if len(self._list) == len(self._dict): return
+        if len(self._list) == len(self._dict):
+            return
 
         for key, value in self._dict.items():
             item = [key, value]
-            if item in self._list: continue
+            if item in self._list:
+                continue
             self._list.append(item)
             self._items[key] = item
 
+
 class LazyDict(dict):
 
-    def __getitem__(self, key, force = False, resolve = False):
+    def __getitem__(self, key, force=False, resolve=False):
         value = dict.__getitem__(self, key)
-        if force: return value
-        if not isinstance(value, LazyValue): return value
-        return value.resolve(force = resolve)
+        if force:
+            return value
+        if not isinstance(value, LazyValue):
+            return value
+        return value.resolve(force=resolve)
 
-    def resolve(self, force = False):
+    def resolve(self, force=False):
         result = dict()
         for key in self:
-            value = self.__getitem__(key, resolve = force)
+            value = self.__getitem__(key, resolve=force)
             result[key] = value
         return result
 
-    def to_dict(self, force = True):
-        return self.resolve(force = force)
+    def to_dict(self, force=True):
+        return self.resolve(force=force)
+
 
 class LazyValue(object):
 
     def __init__(self, callable):
         self.callable = callable
 
     def __call__(self):
         return self.call()
 
-    def resolve(self, force = False):
+    def resolve(self, force=False):
         if hasattr(self, "_value") and not force:
             return self._value
         self._value = self.callable()
         return self._value
 
     def call(self):
         return self.resolve()
 
+
 class GeneratorFile(object):
     """
     File like class that encapsulates an underlying
     stream generator (first yield is size) into a
     file, to be used as a normal file.
 
     Notice that there are certain limitation to this
@@ -252,28 +257,31 @@
     """
 
     def __init__(self, generator):
         self._generator = generator
         self._size = next(generator)
         self._position = 0
 
-    def seek(self, offset, whence = os.SEEK_SET):
+    def seek(self, offset, whence=os.SEEK_SET):
         if whence == os.SEEK_SET:
             self._position = offset
         if whence == os.SEEK_CUR:
             self._position += offset
         if whence == os.SEEK_END:
             self._position = self._size + offset
 
     def tell(self):
         return self._position
 
     def read(self, size):
-        try: data = next(self._generator)
-        except StopIteration: data = b""
+        try:
+            data = next(self._generator)
+        except StopIteration:
+            data = b""
         return data
 
     def close(self):
         self._generator.close()
 
+
 lazy_dict = LazyDict
 lazy = LazyValue
```

### Comparing `quorum-0.8.2/src/quorum/meta.py` & `quorum-0.8.3/src/quorum/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,47 +18,42 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import legacy
 
+
 class Ordered(type):
     """
     Metaclass to be used for classes where the
     definition order of its attributes is critical
     for the correct process.
     """
 
     def __new__(cls, name, bases, attrs):
         new_cls = super(Ordered, cls).__new__(cls, name, bases, attrs)
-        new_cls._ordered = [(name, attrs.pop(name)) for name, value in\
-            legacy.eager(attrs.items()) if hasattr(value, "creation_counter")]
-        new_cls._ordered.sort(key = lambda item: item[1].creation_counter)
+        new_cls._ordered = [
+            (name, attrs.pop(name))
+            for name, value in legacy.eager(attrs.items())
+            if hasattr(value, "creation_counter")
+        ]
+        new_cls._ordered.sort(key=lambda item: item[1].creation_counter)
         new_cls._ordered = [name for name, value in new_cls._ordered]
         return new_cls
 
     def __init__(cls, name, bases, attrs):
         super(Ordered, cls).__init__(name, bases, attrs)
 
     def __cmp__(self, value):
-        return cmp(self.__name__, value.__name__) #@UndefinedVariable
+        return cmp(self.__name__, value.__name__)  # @UndefinedVariable
 
     def __lt__(self, value):
         return self.__name__.__lt__(value.__name__)
```

### Comparing `quorum-0.8.2/src/quorum/log.py` & `quorum-0.8.3/src/quorum/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import sys
@@ -60,71 +51,66 @@
 LOGGING_FORMAT_TID_T = "%%(asctime)s [%%(levelname)s] %s[%%(thread)d] %%(message)s"
 """ The format to be used for the logging operation in
 the app, these operations are going to be handled by
 multiple stream handlers, this version of the string
 includes the thread identification number and should be
 used for messages called from outside the main thread """
 
-LOGGING_EXTRA = "[%(name)s] " if config.conf("LOGGING_EXTRA", cast = bool) else ""
+LOGGING_EXTRA = "[%(name)s] " if config.conf("LOGGING_EXTRA", cast=bool) else ""
 """ The extra logging attributes that are going to be applied
 to the format strings to obtain the final on the logging """
 
-LOGGIGN_SYSLOG = "1 %%(asctime)s %%(hostname)s %s %%(process)d %%(thread)d \
-[quorumSDID@0 tid=\"%%(thread)d\"] %%(json)s"
+LOGGIGN_SYSLOG = '1 %%(asctime)s %%(hostname)s %s %%(process)d %%(thread)d \
+[quorumSDID@0 tid="%%(thread)d"] %%(json)s'
 """ The format to be used for the message sent using the syslog
 logger, should contain extra structured data """
 
 MAX_LENGTH = 10000
 """ The maximum amount of messages that are kept in
 memory until they are discarded, avoid a very large
 number for this value or else a large amount of memory
 may be used for logging purposes """
 
 SILENT = logging.CRITICAL + 1
 """ The "artificial" silent level used to silent a logger
 or an handler, this is used as an utility for debugging
 purposes more that a real feature for production systems """
 
-LEVELS = (
-    "DEBUG",
-    "INFO",
-    "WARNING",
-    "ERROR",
-    "CRITICAL"
-)
+LEVELS = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
 """ The sequence of levels from the least sever to the
 most sever this sequence may be used to find all the
 levels that are considered more sever that a level """
 
 LEVEL_ALIAS = {
-    "DEBU" : "DEBUG",
-    "WARN" : "WARNING",
-    "INF" : "INFO",
-    "ERR" : "ERROR",
-    "CRIT" : "CRITICAL"
+    "DEBU": "DEBUG",
+    "WARN": "WARNING",
+    "INF": "INFO",
+    "ERR": "ERROR",
+    "CRIT": "CRITICAL",
 }
 """ Map defining a series of alias that may be used latter
 for proper debug level resolution """
 
-SYSLOG_PORTS = dict(tcp = 601, udp = 514)
+SYSLOG_PORTS = dict(tcp=601, udp=514)
 """ Dictionary that maps the multiple transport protocol
 used by syslog with the appropriate default ports """
 
 LOGGING_FORMAT = LOGGING_FORMAT_T % LOGGING_EXTRA
 LOGGING_FORMAT_TID = LOGGING_FORMAT_TID_T % LOGGING_EXTRA
 
+
 class MemoryHandler(logging.Handler):
     """
     Logging handler that is used to store information in
     memory so that anyone else may consult it latter as
     long as the execution session is the same.
     """
 
-    def __init__(self, level = logging.NOTSET, max_length = MAX_LENGTH):
-        logging.Handler.__init__(self, level = level)
+    def __init__(self, level=logging.NOTSET, max_length=MAX_LENGTH):
+        logging.Handler.__init__(self, level=level)
         self.max_length = max_length
         self.messages = collections.deque()
         self.messages_l = dict()
 
         format = config.conf("LOGGING_FORMAT", None)
         format_base = format or LOGGING_FORMAT
         format_tid = format or LOGGING_FORMAT_TID
@@ -132,31 +118,34 @@
         formatter = ThreadFormatter(format_base)
         formatter.set_tid(format_tid)
         self.setFormatter(formatter)
 
     def get_messages_l(self, level):
         # in case the level is not found in the list of levels
         # it's not considered valid and so an empty list is returned
-        try: index = LEVELS.index(level)
-        except Exception: return collections.deque()
+        try:
+            index = LEVELS.index(level)
+        except Exception:
+            return collections.deque()
 
         # retrieves the complete set of levels that are considered
         # equal or more severe than the requested one
-        levels = LEVELS[:index + 1]
+        levels = LEVELS[: index + 1]
 
         # creates the list that will hold the various message
         # lists associated with the current severity level
         messages_l = collections.deque()
 
         # iterates over the complete set of levels considered
         # equal or less sever to add the respective messages
         # list to the list of message lists
         for level in levels:
             _messages_l = self.messages_l.get(level, None)
-            if _messages_l == None: _messages_l = collections.deque()
+            if _messages_l == None:
+                _messages_l = collections.deque()
             self.messages_l[level] = _messages_l
             messages_l.append(_messages_l)
 
         # returns the complete set of messages lists that
         # have a level equal or less severe that the one
         # that has been requested by argument
         return messages_l
@@ -174,60 +163,61 @@
         messages_l = self.get_messages_l(level)
 
         # inserts the message into the messages queue and in
         # case the current length of the message queue overflows
         # the one defined as maximum must pop message from queue
         self.messages.appendleft(message)
         messages_s = len(self.messages)
-        if messages_s > self.max_length: self.messages.pop()
+        if messages_s > self.max_length:
+            self.messages.pop()
 
         # iterates over all the messages list included in the retrieve
         # messages list to add the logging message to each of them
         for _messages_l in messages_l:
             # inserts the message into the proper level specific queue
             # and in case it overflows runs the same pop operation as
             # specified also for the more general queue
             _messages_l.appendleft(message)
             messages_s = len(_messages_l)
-            if messages_s > self.max_length: _messages_l.pop()
+            if messages_s > self.max_length:
+                _messages_l.pop()
 
     def clear(self):
         self.messages = collections.deque()
         self.messages_l = dict()
 
-    def get_latest(self, count = None, level = None):
+    def get_latest(self, count=None, level=None):
         count = count or 100
         is_level = level and not legacy.is_string(level)
-        if is_level: level = logging.getLevelName(level)
+        if is_level:
+            level = logging.getLevelName(level)
         level = level.upper() if level else level
         level = LEVEL_ALIAS.get(level, level)
         messages = self.messages_l.get(level, []) if level else self.messages
         slice = itertools.islice(messages, 0, count)
         return list(slice)
 
-    def flush_to_file(
-        self,
-        path,
-        count = None,
-        level = None,
-        reverse = True,
-        clear = True
-    ):
-        messages = self.get_latest(level = level, count = count or 65536)
-        if not messages: return
-        if reverse: messages.reverse()
+    def flush_to_file(self, path, count=None, level=None, reverse=True, clear=True):
+        messages = self.get_latest(level=level, count=count or 65536)
+        if not messages:
+            return
+        if reverse:
+            messages.reverse()
         is_path = isinstance(path, legacy.STRINGS)
         file = open(path, "wb") if is_path else path
         try:
             for message in messages:
-                message = legacy.bytes(message, "utf-8", force = True)
+                message = legacy.bytes(message, "utf-8", force=True)
                 file.write(message + b"\n")
         finally:
-            if is_path: file.close()
-        if clear: self.clear()
+            if is_path:
+                file.close()
+        if clear:
+            self.clear()
+
 
 class BaseFormatter(logging.Formatter):
     """
     The base Quorum logging formatted used to add some extra
     functionality on top of Python's base formatting infra-structure.
 
     Most of its usage focus on empowering the base record object
@@ -236,40 +226,43 @@
 
     def __init__(self, *args, **kwargs):
         self._wrap = kwargs.pop("wrap", False)
         logging.Formatter.__init__(self, *args, **kwargs)
 
     @classmethod
     def _wrap_record(cls, record):
-        if hasattr(record, "_wrapped"): return
+        if hasattr(record, "_wrapped"):
+            return
         record.hostname = socket.gethostname()
         record.json = json.dumps(
             dict(
-                message = str(record.msg),
-                hostname = record.hostname,
-                lineno = record.lineno,
-                module = record.module,
-                callable = record.funcName,
-                level = record.levelname,
-                thread = record.thread,
-                process = record.process,
-                logger = record.name
+                message=str(record.msg),
+                hostname=record.hostname,
+                lineno=record.lineno,
+                module=record.module,
+                callable=record.funcName,
+                level=record.levelname,
+                thread=record.thread,
+                process=record.process,
+                logger=record.name,
             )
         )
         record._wrapped = True
 
     def format(self, record):
         # runs the wrapping operation on the record so that more
         # information becomes available in it (as expected)
-        if self._wrap: self.__class__._wrap_record(record)
+        if self._wrap:
+            self.__class__._wrap_record(record)
 
         # runs the basic format operation on the record so that
         # it gets properly formatted into a plain string
         return logging.Formatter.format(self, record)
 
+
 class ThreadFormatter(BaseFormatter):
     """
     Custom formatter class that changing the default format
     behavior so that the thread identifier is printed when
     the threading printing the log records is not the main one.
     """
 
@@ -277,110 +270,127 @@
         BaseFormatter.__init__(self, *args, **kwargs)
         self._basefmt = BaseFormatter(*args, **kwargs)
         self._tidfmt = BaseFormatter(*args, **kwargs)
 
     def format(self, record):
         # runs the wrapping operation on the record so that more
         # information becomes available in it (as expected)
-        if self._wrap: self.__class__._wrap_record(record)
+        if self._wrap:
+            self.__class__._wrap_record(record)
 
         # retrieves the reference to the current thread and verifies
         # if it represent the current process main thread, then selects
         # the appropriate formating string taking that into account
         current = threading.current_thread()
         is_main = current.name == "MainThread"
-        if not is_main: return self._tidfmt.format(record)
+        if not is_main:
+            return self._tidfmt.format(record)
         return self._basefmt.format(record)
 
     def set_base(self, value, *args, **kwargs):
         self._basefmt = BaseFormatter(value, *args, **kwargs)
 
     def set_tid(self, value, *args, **kwargs):
         self._tidfmt = BaseFormatter(value, *args, **kwargs)
 
+
 def rotating_handler(
-    path = "quorum.log",
-    max_bytes = 1048576,
-    max_log = 5,
-    encoding = None,
-    delay = False
+    path="quorum.log", max_bytes=1048576, max_log=5, encoding=None, delay=False
 ):
     return logging.handlers.RotatingFileHandler(
-        path,
-        maxBytes = max_bytes,
-        backupCount = max_log,
-        encoding = encoding,
-        delay = delay
+        path, maxBytes=max_bytes, backupCount=max_log, encoding=encoding, delay=delay
     )
 
+
 def smtp_handler(
-    host = "localhost",
-    port = 25,
-    sender = "no-reply@quorum.com",
-    receivers = [],
-    subject = "Quorum logging",
-    username = None,
-    password = None,
-    stls = False
+    host="localhost",
+    port=25,
+    sender="no-reply@quorum.com",
+    receivers=[],
+    subject="Quorum logging",
+    username=None,
+    password=None,
+    stls=False,
 ):
     address = (host, port)
-    if username and password: credentials = (username, password)
-    else: credentials = None
+    if username and password:
+        credentials = (username, password)
+    else:
+        credentials = None
     has_secure = in_signature(logging.handlers.SMTPHandler.__init__, "secure")
-    if has_secure: kwargs = dict(secure = () if stls else None)
-    else: kwargs = dict()
+    if has_secure:
+        kwargs = dict(secure=() if stls else None)
+    else:
+        kwargs = dict()
     return logging.handlers.SMTPHandler(
-        address,
-        sender,
-        receivers,
-        subject,
-        credentials = credentials,
-        **kwargs
+        address, sender, receivers, subject, credentials=credentials, **kwargs
     )
 
+
 def in_signature(callable, name):
     has_full = hasattr(inspect, "getfullargspec")
-    if has_full: spec = inspect.getfullargspec(callable)
-    else: spec = inspect.getargspec(callable)
+    if has_full:
+        spec = inspect.getfullargspec(callable)
+    else:
+        spec = inspect.getargspec(callable)
     args, _varargs, kwargs = spec[:3]
     return (args and name in args) or (kwargs and "secure" in kwargs)
 
+
 def has_exception():
     info = sys.exc_info()
     return not info == (None, None, None)
 
-def debug(message, log_trace = False, *args, **kwargs):
+
+def debug(message, log_trace=False, *args, **kwargs):
     logger = common.base().get_log()
-    if not logger: return
+    if not logger:
+        return
     logger.debug(message, *args, **kwargs)
 
-def info(message, log_trace = False, *args, **kwargs):
+
+def info(message, log_trace=False, *args, **kwargs):
     logger = common.base().get_log()
-    if not logger: return
+    if not logger:
+        return
     logger.info(message, *args, **kwargs)
-    if not log_trace or not has_exception(): return
+    if not log_trace or not has_exception():
+        return
     lines = traceback.format_exc().splitlines()
-    for line in lines: logger.debug(line, *args, **kwargs)
+    for line in lines:
+        logger.debug(line, *args, **kwargs)
+
 
-def warning(message, log_trace = False, *args, **kwargs):
+def warning(message, log_trace=False, *args, **kwargs):
     logger = common.base().get_log()
-    if not logger: return
+    if not logger:
+        return
     logger.warning(message, *args, **kwargs)
-    if not log_trace or not has_exception(): return
+    if not log_trace or not has_exception():
+        return
     lines = traceback.format_exc().splitlines()
-    for line in lines: logger.info(line, *args, **kwargs)
+    for line in lines:
+        logger.info(line, *args, **kwargs)
 
-def error(message, log_trace = False, *args, **kwargs):
+
+def error(message, log_trace=False, *args, **kwargs):
     logger = common.base().get_log()
-    if not logger: return
+    if not logger:
+        return
     logger.error(message, *args, **kwargs)
-    if not log_trace or not has_exception(): return
+    if not log_trace or not has_exception():
+        return
     lines = traceback.format_exc().splitlines()
-    for line in lines: logger.warning(line, *args, **kwargs)
+    for line in lines:
+        logger.warning(line, *args, **kwargs)
+
 
-def critical(message, log_trace = False, *args, **kwargs):
+def critical(message, log_trace=False, *args, **kwargs):
     logger = common.base().get_log()
-    if not logger: return
+    if not logger:
+        return
     logger.critical(message, *args, **kwargs)
-    if not log_trace or not has_exception(): return
+    if not log_trace or not has_exception():
+        return
     lines = traceback.format_exc().splitlines()
-    for line in lines: logger.error(line, *args, **kwargs)
+    for line in lines:
+        logger.error(line, *args, **kwargs)
```

### Comparing `quorum-0.8.2/src/quorum/data.py` & `quorum-0.8.3/src/quorum/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -47,14 +38,15 @@
 
 from . import log
 from . import legacy
 from . import config
 from . import mongodb
 from . import exceptions
 
+
 class DataAdapter(object):
 
     def __init__(self, *args, **kwargs):
         self._inc = 0
         self._machine_bytes = self.__machine_bytes()
         self._inc_lock = threading.RLock()
 
@@ -85,48 +77,50 @@
 
     def drop_db(self, *args, **kwargs):
         raise exceptions.NotImplementedError()
 
     def drop_db_a(self, *args, **kwargs):
         raise exceptions.NotImplementedError()
 
-    def object_id(self, value = None):
-        if not value: return self._id()
+    def object_id(self, value=None):
+        if not value:
+            return self._id()
         if not len(value) == 24:
             raise exceptions.OperationalError(
-                message = "Expected object id of length 24 chars"
+                message="Expected object id of length 24 chars"
             )
         return value
 
     @property
     def name(self):
         cls = self.__class__
         return cls.name_g()
 
     def _id(self):
         token = struct.pack(">i", int(time.time()))
         token += self._machine_bytes
-        token += struct.pack(">H", os.getpid() % 0xffff)
+        token += struct.pack(">H", os.getpid() % 0xFFFF)
         self._inc_lock.acquire()
         try:
             token += struct.pack(">i", self._inc)[1:4]
-            self._inc = (self._inc + 1) % 0xffffff
+            self._inc = (self._inc + 1) % 0xFFFFFF
         except Exception:
             self._inc_lock.release()
         token_s = binascii.hexlify(token)
         token_s = legacy.str(token_s)
         return token_s
 
     def __machine_bytes(self):
         machine_hash = hashlib.md5()
         hostname = socket.gethostname()
         hostname = legacy.bytes(hostname)
         machine_hash.update(hostname)
         return machine_hash.digest()[0:3]
 
+
 class MongoAdapter(DataAdapter):
 
     def encoder(self):
         return mongodb.MongoEncoder
 
     def collection(self, name, *args, **kwargs):
         db = self.get_db()
@@ -152,21 +146,23 @@
 
     def drop_db(self, *args, **kwargs):
         return mongodb.drop_db()
 
     def drop_db_a(self, *args, **kwargs):
         return mongodb.drop_db_a()
 
-    def object_id(self, value = None):
-        if not value: return self._id()
+    def object_id(self, value=None):
+        if not value:
+            return self._id()
         return mongodb.object_id(value)
 
     def _id(self):
         return mongodb.object_id(None)
 
+
 class TinyAdapter(DataAdapter):
 
     def __init__(self, *args, **kwargs):
         DataAdapter.__init__(self, *args, **kwargs)
         self.file_path = config.conf("TINY_PATH", "db.json")
         self.storage = config.conf("TINY_STORAGE", "json")
         self.file_path = kwargs.get("file_path", self.file_path)
@@ -177,45 +173,50 @@
         table = db.table(name)
         return TinyCollection(self, name, table)
 
     def reset(self):
         pass
 
     def get_db(self):
-        if not self._db == None: return self._db
+        if not self._db == None:
+            return self._db
         method = getattr(self, "_get_db_%s" % self.storage)
         self._db = method()
         return self._db
 
     def drop_db(self, *args, **kwargs):
-        if self._db == None: return
+        if self._db == None:
+            return
         db = self.get_db()
-        if hasattr(db, "drop_tables"): db.drop_tables()
-        else: db.purge_tables()
+        if hasattr(db, "drop_tables"):
+            db.drop_tables()
+        else:
+            db.purge_tables()
         db.close()
         self._db = None
         method = getattr(self, "_drop_db_%s" % self.storage)
         method()
 
     def _get_db_json(self):
         import tinydb
+
         return tinydb.TinyDB(self.file_path)
 
     def _get_db_memory(self):
         import tinydb
-        return tinydb.TinyDB(
-            storage = tinydb.storages.MemoryStorage
-        )
+
+        return tinydb.TinyDB(storage=tinydb.storages.MemoryStorage)
 
     def _drop_db_json(self):
         os.remove(self.file_path)
 
     def _drop_db_memory(self):
         pass
 
+
 class Collection(object):
 
     def __init__(self, owner, name):
         self.owner = owner
         self.name = name
 
     def find(self, *args, **kwargs):
@@ -245,25 +246,27 @@
     def drop_indexes(self, *args, **kwargs):
         raise exceptions.NotImplementedError()
 
     def object_id(self, *args, **kwargs):
         return self.owner.object_id(*args, **kwargs)
 
     def log(self, operation, *args, **kwargs):
-        show_queries = config.conf("SHOW_QUERIES", False, cast = bool)
-        if not show_queries: return
+        show_queries = config.conf("SHOW_QUERIES", False, cast=bool)
+        if not show_queries:
+            return
         extra = kwargs or args
         log.debug(
-            "[%s] %10s -> %12s <-> %s" %\
-            (self.owner.name, operation, self.name, str(extra)[:2046])
+            "[%s] %10s -> %12s <-> %s"
+            % (self.owner.name, operation, self.name, str(extra)[:2046])
         )
 
     def _id(self, *args, **kwargs):
         return self.owner._id(*args, **kwargs)
 
+
 class MongoCollection(Collection):
 
     def __init__(self, owner, name, base):
         Collection.__init__(self, owner, name)
         self._base = base
 
     def find(self, *args, **kwargs):
@@ -302,29 +305,40 @@
         self.log("ensure_index", *args, **kwargs)
         direction = kwargs.pop("direction", True)
 
         is_simple = direction == "simple"
         is_all = direction == "all"
         is_default = direction in ("default", True)
         is_multiple = isinstance(direction, (list, tuple))
-        is_direction = not is_default and not is_all and not is_simple and\
-            (legacy.is_string(direction) or type(direction) == int)
+        is_direction = (
+            not is_default
+            and not is_all
+            and not is_simple
+            and (legacy.is_string(direction) or type(direction) == int)
+        )
         is_single = is_simple or is_direction
 
-        if is_all: kwargs["directions"] = "all"
-        if is_multiple: kwargs["directions"] = direction
-        if is_direction: args = list(args); args[0] = [(args[0], direction)]
-
-        if is_single: return mongodb._store_ensure_index(self._base, *args, **kwargs)
-        else: return mongodb._store_ensure_index_many(self._base, *args, **kwargs)
+        if is_all:
+            kwargs["directions"] = "all"
+        if is_multiple:
+            kwargs["directions"] = direction
+        if is_direction:
+            args = list(args)
+            args[0] = [(args[0], direction)]
+
+        if is_single:
+            return mongodb._store_ensure_index(self._base, *args, **kwargs)
+        else:
+            return mongodb._store_ensure_index_many(self._base, *args, **kwargs)
 
     def drop_indexes(self, *args, **kwargs):
         self.log("drop_indexes", *args, **kwargs)
         return self._base.drop_indexes()
 
+
 class TinyCollection(Collection):
 
     def __init__(self, owner, name, base):
         Collection.__init__(self, owner, name)
         self._base = base
 
     def find(self, *args, **kwargs):
@@ -348,25 +362,29 @@
         modification = args[1] if len(args) > 1 else dict()
         create = kwargs.get("new", False)
         condition = self._to_condition(filter)
         object = self._base.get(condition)
         found = True if object else False
         if not found and not create:
             raise exceptions.OperationalError("No object found")
-        if not found: object = dict(filter)
-        object = self._to_update(modification, object = object)
-        if found: self.update(filter, {"$set" : object})
-        else: self.insert(object)
+        if not found:
+            object = dict(filter)
+        object = self._to_update(modification, object=object)
+        if found:
+            self.update(filter, {"$set": object})
+        else:
+            self.insert(object)
         return dict(object)
 
     def insert(self, *args, **kwargs):
         self.log("insert", *args, **kwargs)
         object = args[0] if len(args) > 0 else dict()
         has_id = "_id" in object
-        if not has_id: object["_id"] = self._id()
+        if not has_id:
+            object["_id"] = self._id()
         self._base.insert(object)
         return object
 
     def update(self, *args, **kwargs):
         self.log("update", *args, **kwargs)
         filter = args[0] if len(args) > 0 else dict()
         updater = args[1] if len(args) > 1 else dict()
@@ -390,42 +408,48 @@
         self.log("ensure_index", *args, **kwargs)
 
     def drop_indexes(self, *args, **kwargs):
         self.log("drop_indexes", *args, **kwargs)
 
     def _to_condition(self, filter):
         import tinydb
+
         query = tinydb.Query()
         condition = query._id.exists()
         for name, value in legacy.iteritems(filter):
-            if name.startswith("$"): continue
+            if name.startswith("$"):
+                continue
             query = tinydb.Query()
             _condition = getattr(query, name).__eq__(value)
             condition &= _condition
         return condition
 
-    def _to_results(self, results, kwargs, build = True):
+    def _to_results(self, results, kwargs, build=True):
         sort = kwargs.get("sort", [])
         skip = kwargs.get("skip", 0)
         limit = kwargs.get("limit", None)
 
         limit = None if limit == 0 else limit
         reverse = sort[0][1] == -1 if sort else False
 
         def sorter(value):
             result = []
-            for item in sort: result.append(value[item[0]])
+            for item in sort:
+                result.append(value[item[0]])
             return tuple(result)
 
-        if sort: results.sort(key = sorter, reverse = reverse)
-        if skip or limit: results = results[slice(skip, skip + limit, 1)]
-        if build: results = [dict(result) for result in results]
+        if sort:
+            results.sort(key=sorter, reverse=reverse)
+        if skip or limit:
+            results = results[slice(skip, skip + limit, 1)]
+        if build:
+            results = [dict(result) for result in results]
         return results
 
-    def _to_update(self, modification, object = None):
+    def _to_update(self, modification, object=None):
         object = object or dict()
         increments = modification.get("$inc", {})
         mins = modification.get("$min", {})
         maxs = modification.get("$max", {})
         for name, increment in legacy.iteritems(increments):
             value = object.get(name, 0)
             value += increment
```

### Comparing `quorum-0.8.2/src/quorum/defines.py` & `quorum-0.8.3/src/quorum/defines.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,263 +18,228 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import re
 
 ITERABLES = (list, tuple)
 """ The tuple that defined the various base types
 that are considered to be generally "iterable" """
 
-MOBILE_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows (ce|phone)|xda|xiino", re.I | re.M)
+MOBILE_REGEX = re.compile(
+    r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows (ce|phone)|xda|xiino",
+    re.I | re.M,
+)
 """ The regular expression that is going to be used
 to validate the complete user agent string for mobile """
 
-TABLET_REGEX = re.compile(r"(android|bb\d+|meego).+mobile|avantgo|bada\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\.(browser|link)|vodafone|wap|windows (ce|phone)|xda|xiino|android|ipad|playbook|silk", re.I | re.M)
+TABLET_REGEX = re.compile(
+    r"(android|bb\d+|meego).+mobile|avantgo|bada\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\.(browser|link)|vodafone|wap|windows (ce|phone)|xda|xiino|android|ipad|playbook|silk",
+    re.I | re.M,
+)
 """ The regular expression that is going to be used
 to validate the complete user agent string for tablet """
 
-MOBILE_PREFIX_REGEX = re.compile(r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-", re.I | re.M)
+MOBILE_PREFIX_REGEX = re.compile(
+    r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-",
+    re.I | re.M,
+)
 """ The regular expression to test the base prefix
 of the user agent string for mobile browser """
 
-BROWSER_INFO = [dict(
-    identity = "Edge",
-    sub_string = "Edge"
-), dict(
-    identity = "Chrome",
-    sub_string = "Chrome"
-), dict(
-    identity = "Safari",
-    sub_string = "Safari"
-), dict(
-    identity = "Opera"
-), dict(
-    identity = "Firefox",
-    sub_string = "Firefox"
-), dict(
-    identity = "Explorer",
-    sub_string = "MSIE",
-    version_search = "MSIE "
-), dict(
-    identity = "AppleWebKit",
-    sub_string = "AppleWebKit"
-), dict(
-    identity = "Googlebot",
-    sub_string = "Googlebot",
-    interactive = False,
-    bot = True
-), dict(
-    identity = "Bingbot",
-    sub_string = "Bingbot",
-    interactive = False,
-    bot = True
-), dict(
-    identity = "DuckDuckBot",
-    sub_string = "DuckDuckBot",
-    interactive = False,
-    bot = True
-), dict(
-    identity = "netius",
-    sub_string = "netius",
-    interactive = False
-)]
+BROWSER_INFO = [
+    dict(identity="Edge", sub_string="Edge"),
+    dict(identity="Chrome", sub_string="Chrome"),
+    dict(identity="Safari", sub_string="Safari"),
+    dict(identity="Opera"),
+    dict(identity="Firefox", sub_string="Firefox"),
+    dict(identity="Explorer", sub_string="MSIE", version_search="MSIE "),
+    dict(identity="AppleWebKit", sub_string="AppleWebKit"),
+    dict(identity="Googlebot", sub_string="Googlebot", interactive=False, bot=True),
+    dict(identity="Bingbot", sub_string="Bingbot", interactive=False, bot=True),
+    dict(identity="DuckDuckBot", sub_string="DuckDuckBot", interactive=False, bot=True),
+    dict(identity="netius", sub_string="netius", interactive=False),
+]
 """ List that contains the complete information used
 for the parsing and identification of the browser information
 from a typical user agent string """
 
-OS_INFO = [dict(
-    identity = "Windows",
-    sub_string = "Win"
-), dict(
-    identity = "Mac",
-    sub_string = "Mac"
-), dict(
-    identity = "iPhone/iPod",
-    sub_string = "iPhone"
-), dict(
-    sub_string = "Linux",
-    identity = "Linux"
-)]
+OS_INFO = [
+    dict(identity="Windows", sub_string="Win"),
+    dict(identity="Mac", sub_string="Mac"),
+    dict(identity="iPhone/iPod", sub_string="iPhone"),
+    dict(sub_string="Linux", identity="Linux"),
+]
 """ List that contains the complete information used
 for the parsing and identification of the os information
 from a typical user agent string """
 
 WINDOWS_LOCALE = dict(
-    af = "Afrikaans",
-    sq = "Albanian",
-    am = "Amharic",
-    ar_DZ = "Arabic_Algeria",
-    ar_BH = "Arabic_Bahrain",
-    ar_EG = "Arabic_Egypt",
-    ar_IQ = "Arabic_Iraq",
-    ar_JO = "Arabic_Jordan",
-    ar_KW = "Arabic_Kuwait",
-    ar_LB = "Arabic_Lebanon",
-    ar_LY = "Arabic_Libya",
-    ar_MA = "Arabic_Morocco",
-    ar_OM = "Arabic_Oman",
-    ar_QA = "Arabic_Qatar",
-    ar_SA = "Arabic_Saudi Arabia",
-    ar_SY = "Arabic_Syria",
-    ar_TN = "Arabic_Tunisia",
-    ar_AE = "Arabic_United Arab Emirates",
-    ar_YE = "Arabic_Yemen",
-    hy = "Armenian",
-    az_AZ = "Azeri_Cyrillic",
-    eu = "Basque",
-    be = "Belarusian",
-    bn = "Bengali_Bangladesh",
-    bs = "Bosnian",
-    bg = "Bulgarian",
-    my = "Burmese",
-    ca = "Catalan",
-    zh_CN = "Chinese_China",
-    zh_HK = "Chinese_Hong Kong SAR",
-    zh_MO = "Chinese_Macau SAR",
-    zh_SG = "Chinese_Singapore",
-    zh_TW = "Chinese_Taiwan",
-    hr = "Croatian",
-    cs = "Czech",
-    da = "Danish",
-    dv = "Divehi; Dhivehi; Maldivian",
-    nl_BE = "Dutch_Belgium",
-    nl_NL = "Dutch_Netherlands",
-    en_AU = "English_Australia",
-    en_BZ = "English_Belize",
-    en_CA = "English_Canada",
-    en_CB = "English_Caribbean",
-    en_GB = "English_Great Britain",
-    en_IN = "English_India",
-    en_IE = "English_Ireland",
-    en_JM = "English_Jamaica",
-    en_NZ = "English_New Zealand",
-    en_PH = "English_Phillippines",
-    en_ZA = "English_Southern Africa",
-    en_TT = "English_Trinidad",
-    en_US = "English_United States",
-    et = "Estonian",
-    fo = "Faroese",
-    fa = "Farsi_Persian",
-    fi = "Finnish",
-    fr_BE = "French_Belgium",
-    fr_CA = "French_Canada",
-    fr_FR = "French_France",
-    fr_LU = "French_Luxembourg",
-    fr_CH = "French_Switzerland",
-    mk = "FYRO Macedonia",
-    gd_IE = "Gaelic_Ireland",
-    gd = "Gaelic_Scotland",
-    de_AT = "German_Austria",
-    de_DE = "German_Germany",
-    de_LI = "German_Liechtenstein",
-    de_LU = "German_Luxembourg",
-    de_CH = "German_Switzerland",
-    el = "Greek",
-    gn = "Guarani_Paraguay",
-    gu = "Gujarati",
-    he = "Hebrew",
-    hi = "Hindi",
-    hu = "Hungarian",
-    id = "Indonesian",
-    it_IT = "Italian_Italy",
-    it_CH = "Italian_Switzerland",
-    ja = "Japanese",
-    kn = "Kannada",
-    ks = "Kashmiri",
-    kk = "Kazakh",
-    km = "Khmer",
-    ko = "Korean",
-    lo = "Lao",
-    la = "Latin",
-    lv = "Latvian",
-    lt = "Lithuanian",
-    ms_BN = "Malay_Brunei",
-    ms_MY = "Malay_Malaysia",
-    ml = "Malayalam",
-    mt = "Maltese",
-    mi = "Maori",
-    mr = "Marathi",
-    mn = "Mongolian",
-    ne = "Nepali",
-    no_NO = "Norwegian_Bokml",
-    pl = "Polish",
-    pt_BR = "Portuguese_Brazil",
-    pt_PT = "Portuguese_Portugal",
-    pa = "Punjabi",
-    rm = "Raeto-Romance",
-    ro_MO = "Romanian_Moldova",
-    ro = "Romanian_Romania",
-    ru = "Russian",
-    ru_MO = "Russian_Moldova",
-    sa = "Sanskrit",
-    sr_SP = "Serbian_Cyrillic",
-    tn = "Setsuana",
-    sd = "Sindhi",
-    si = "Sinhala; Sinhalese",
-    sk = "Slovak",
-    sl = "Slovenian",
-    so = "Somali",
-    sb = "Sorbian",
-    es_AR = "Spanish_Argentina",
-    es_BO = "Spanish_Bolivia",
-    es_CL = "Spanish_Chile",
-    es_CO = "Spanish_Colombia",
-    es_CR = "Spanish_Costa Rica",
-    es_DO = "Spanish_Dominican Republic",
-    es_EC = "Spanish_Ecuador",
-    es_SV = "Spanish_El Salvador",
-    es_GT = "Spanish_Guatemala",
-    es_HN = "Spanish_Honduras",
-    es_MX = "Spanish_Mexico",
-    es_NI = "Spanish_Nicaragua",
-    es_PA = "Spanish_Panama",
-    es_PY = "Spanish_Paraguay",
-    es_PE = "Spanish_Peru",
-    es_PR = "Spanish_Puerto Rico",
-    es_ES = "Spanish_Spain (Traditional)",
-    es_UY = "Spanish_Uruguay",
-    es_VE = "Spanish_Venezuela",
-    sw = "Swahili",
-    sv_FI = "Swedish_Finland",
-    sv_SE = "Swedish_Sweden",
-    tg = "Tajik",
-    ta = "Tamil",
-    tt = "Tatar",
-    te = "Telugu",
-    th = "Thai",
-    bo = "Tibetan",
-    ts = "Tsonga",
-    tr = "Turkish",
-    tk = "Turkmen",
-    uk = "Ukrainian",
-    UTF_8 = "Unicode",
-    ur = "Urdu",
-    uz_UZ = "Uzbek_Cyrillic",
-    vi = "Vietnamese",
-    cy = "Welsh",
-    xh = "Xhosa",
-    yi = "Yiddish",
-    zu = "Zulu"
+    af="Afrikaans",
+    sq="Albanian",
+    am="Amharic",
+    ar_DZ="Arabic_Algeria",
+    ar_BH="Arabic_Bahrain",
+    ar_EG="Arabic_Egypt",
+    ar_IQ="Arabic_Iraq",
+    ar_JO="Arabic_Jordan",
+    ar_KW="Arabic_Kuwait",
+    ar_LB="Arabic_Lebanon",
+    ar_LY="Arabic_Libya",
+    ar_MA="Arabic_Morocco",
+    ar_OM="Arabic_Oman",
+    ar_QA="Arabic_Qatar",
+    ar_SA="Arabic_Saudi Arabia",
+    ar_SY="Arabic_Syria",
+    ar_TN="Arabic_Tunisia",
+    ar_AE="Arabic_United Arab Emirates",
+    ar_YE="Arabic_Yemen",
+    hy="Armenian",
+    az_AZ="Azeri_Cyrillic",
+    eu="Basque",
+    be="Belarusian",
+    bn="Bengali_Bangladesh",
+    bs="Bosnian",
+    bg="Bulgarian",
+    my="Burmese",
+    ca="Catalan",
+    zh_CN="Chinese_China",
+    zh_HK="Chinese_Hong Kong SAR",
+    zh_MO="Chinese_Macau SAR",
+    zh_SG="Chinese_Singapore",
+    zh_TW="Chinese_Taiwan",
+    hr="Croatian",
+    cs="Czech",
+    da="Danish",
+    dv="Divehi; Dhivehi; Maldivian",
+    nl_BE="Dutch_Belgium",
+    nl_NL="Dutch_Netherlands",
+    en_AU="English_Australia",
+    en_BZ="English_Belize",
+    en_CA="English_Canada",
+    en_CB="English_Caribbean",
+    en_GB="English_Great Britain",
+    en_IN="English_India",
+    en_IE="English_Ireland",
+    en_JM="English_Jamaica",
+    en_NZ="English_New Zealand",
+    en_PH="English_Phillippines",
+    en_ZA="English_Southern Africa",
+    en_TT="English_Trinidad",
+    en_US="English_United States",
+    et="Estonian",
+    fo="Faroese",
+    fa="Farsi_Persian",
+    fi="Finnish",
+    fr_BE="French_Belgium",
+    fr_CA="French_Canada",
+    fr_FR="French_France",
+    fr_LU="French_Luxembourg",
+    fr_CH="French_Switzerland",
+    mk="FYRO Macedonia",
+    gd_IE="Gaelic_Ireland",
+    gd="Gaelic_Scotland",
+    de_AT="German_Austria",
+    de_DE="German_Germany",
+    de_LI="German_Liechtenstein",
+    de_LU="German_Luxembourg",
+    de_CH="German_Switzerland",
+    el="Greek",
+    gn="Guarani_Paraguay",
+    gu="Gujarati",
+    he="Hebrew",
+    hi="Hindi",
+    hu="Hungarian",
+    id="Indonesian",
+    it_IT="Italian_Italy",
+    it_CH="Italian_Switzerland",
+    ja="Japanese",
+    kn="Kannada",
+    ks="Kashmiri",
+    kk="Kazakh",
+    km="Khmer",
+    ko="Korean",
+    lo="Lao",
+    la="Latin",
+    lv="Latvian",
+    lt="Lithuanian",
+    ms_BN="Malay_Brunei",
+    ms_MY="Malay_Malaysia",
+    ml="Malayalam",
+    mt="Maltese",
+    mi="Maori",
+    mr="Marathi",
+    mn="Mongolian",
+    ne="Nepali",
+    no_NO="Norwegian_Bokml",
+    pl="Polish",
+    pt_BR="Portuguese_Brazil",
+    pt_PT="Portuguese_Portugal",
+    pa="Punjabi",
+    rm="Raeto-Romance",
+    ro_MO="Romanian_Moldova",
+    ro="Romanian_Romania",
+    ru="Russian",
+    ru_MO="Russian_Moldova",
+    sa="Sanskrit",
+    sr_SP="Serbian_Cyrillic",
+    tn="Setsuana",
+    sd="Sindhi",
+    si="Sinhala; Sinhalese",
+    sk="Slovak",
+    sl="Slovenian",
+    so="Somali",
+    sb="Sorbian",
+    es_AR="Spanish_Argentina",
+    es_BO="Spanish_Bolivia",
+    es_CL="Spanish_Chile",
+    es_CO="Spanish_Colombia",
+    es_CR="Spanish_Costa Rica",
+    es_DO="Spanish_Dominican Republic",
+    es_EC="Spanish_Ecuador",
+    es_SV="Spanish_El Salvador",
+    es_GT="Spanish_Guatemala",
+    es_HN="Spanish_Honduras",
+    es_MX="Spanish_Mexico",
+    es_NI="Spanish_Nicaragua",
+    es_PA="Spanish_Panama",
+    es_PY="Spanish_Paraguay",
+    es_PE="Spanish_Peru",
+    es_PR="Spanish_Puerto Rico",
+    es_ES="Spanish_Spain (Traditional)",
+    es_UY="Spanish_Uruguay",
+    es_VE="Spanish_Venezuela",
+    sw="Swahili",
+    sv_FI="Swedish_Finland",
+    sv_SE="Swedish_Sweden",
+    tg="Tajik",
+    ta="Tamil",
+    tt="Tatar",
+    te="Telugu",
+    th="Thai",
+    bo="Tibetan",
+    ts="Tsonga",
+    tr="Turkish",
+    tk="Turkmen",
+    uk="Ukrainian",
+    UTF_8="Unicode",
+    ur="Urdu",
+    uz_UZ="Uzbek_Cyrillic",
+    vi="Vietnamese",
+    cy="Welsh",
+    xh="Xhosa",
+    yi="Yiddish",
+    zu="Zulu",
 )
 """ The map containing the associations between the
 normalized version/descriptor of the locale and the
 longer windows version of them so that it may be used
 when setting locales for windows based operative systems """
```

### Comparing `quorum-0.8.2/src/quorum/base.py` & `quorum-0.8.3/src/quorum/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -112,100 +103,100 @@
 internet explorer browser """
 
 CONTENT_OPTIONS = "nosniff"
 """ Default "X-Content-Type-Options" header value to be used to prevent
 the sniffing of content type values, ensuring that the browser sticks to
 value of content type provided by the server """
 
-ESCAPE_EXTENSIONS = (
-    ".xml",
-    ".html",
-    ".xhtml",
-    ".xml.tpl",
-    ".html.tpl",
-    ".xhtml.tpl"
-)
+ESCAPE_EXTENSIONS = (".xml", ".html", ".xhtml", ".xml.tpl", ".html.tpl", ".xhtml.tpl")
 """ The sequence containing the various extensions
 for which the autoescape mode will be enabled  by
 default as expected by the end developer """
 
 PLATFORM = "%s %d.%d.%d.%s %s" % (
     sys.subversion[0] if hasattr(sys, "subversion") else "CPython",
     sys.version_info[0],
     sys.version_info[1],
     sys.version_info[2],
     sys.version_info[3],
-    sys.platform
+    sys.platform,
 )
 """ Extra system information containing some of the details
 of the technical platform that is running the system, this
 string should be exposed carefully to avoid extra information
 from being exposed to outside agents """
 
+
 class Quorum(flask.Flask):
     """
     The top level application class that inherits from the
     flask based one. Should be responsible for the implementation
     of some of the modifications to the original application
     object infra-structure.
     """
 
     def select_jinja_autoescape(self, filename):
-        if filename == None: return False
-        if filename.endswith(ESCAPE_EXTENSIONS): return True
+        if filename == None:
+            return False
+        if filename.endswith(ESCAPE_EXTENSIONS):
+            return True
         return flask.Flask.select_jinja_autoescape(self, filename)
 
+
 def monkey():
     """
     Runs the dirty job of monkey patching the flask module
     so that some of its functions get redirected to new
     quorum functions that add extra behavior.
 
     This is an internal function and should be changed only
     when handling the internals of the quorum framework.
     """
 
     flask._render_template = flask.render_template
     flask.render_template = template.render_template
     json._default_encoder = util.JSONEncoder()
 
+
 def call_run():
     global RUN_CALLED
-    if RUN_CALLED: return
-    for _fname, f in RUN_F.items(): f()
+    if RUN_CALLED:
+        return
+    for _fname, f in RUN_F.items():
+        f()
     RUN_CALLED = True
 
-def run(server = None, fallback = "base"):
-    if not APP: raise exceptions.BaseError("Application not set or runnable")
+
+def run(server=None, fallback="base"):
+    if not APP:
+        raise exceptions.BaseError("Application not set or runnable")
 
     APP.logger.info(
-        "Booting %s %s (flask %s) (%s) ..." % (
-            info.NAME,
-            info.VERSION,
-            flask.__version__,
-            PLATFORM
-        )
+        "Booting %s %s (flask %s) (%s) ..."
+        % (info.NAME, info.VERSION, flask.__version__, PLATFORM)
     )
 
     server = config.conf("SERVER", server) or "base"
     runner = globals().get("run_" + server, None)
     runner_f = globals().get("run_" + fallback, None)
-    if not runner: raise exceptions.BaseError("Server '%s' not found" % server)
+    if not runner:
+        raise exceptions.BaseError("Server '%s' not found" % server)
 
     call_run()
 
-    try: runner()
+    try:
+        runner()
     except exceptions.ServerInitError as error:
         APP.logger.warning(
-            "Server '%s' failed to start (%s) falling back to '%s'" % (
-                server, legacy.UNICODE(error), fallback
-            )
+            "Server '%s' failed to start (%s) falling back to '%s'"
+            % (server, legacy.UNICODE(error), fallback)
         )
         runner_f and runner_f()
 
+
 def prepare_app():
     """
     Prepares the global application object encapsulating
     it with the proper decorators so that it is enabled
     with the proper features (eg: debugging capabilities).
 
     This method should be called and the returned application
@@ -214,42 +205,39 @@
     :rtype: Application
     :return: The decorated application object with the proper\
     capabilities enabled, this object should be used for the\
     serving operations instead of the global one.
     """
 
     app = APP
-    if app.debug: app = werkzeug.debug.DebuggedApplication(app, True)
+    if app.debug:
+        app = werkzeug.debug.DebuggedApplication(app, True)
     return app
 
+
 def run_base():
-    debug = config.conf("DEBUG", False, cast = bool)
-    reloader = config.conf("RELOADER", False, cast = bool)
+    debug = config.conf("DEBUG", False, cast=bool)
+    reloader = config.conf("RELOADER", False, cast=bool)
     host = config.conf("HOST", "127.0.0.1")
     port = int(config.conf("PORT", 5000))
     APP.run(
-        use_debugger = debug,
-        debug = debug,
-        use_reloader = reloader,
-        host = host,
-        port = port
+        use_debugger=debug, debug=debug, use_reloader=reloader, host=host, port=port
     )
 
+
 def run_netius():
-    try: import netius.servers
+    try:
+        import netius.servers
     except Exception as exception:
-        raise exceptions.ServerInitError(
-            legacy.UNICODE(exception),
-            server = "netius"
-        )
+        raise exceptions.ServerInitError(legacy.UNICODE(exception), server="netius")
 
     kwargs = dict()
     host = config.conf("HOST", "127.0.0.1")
     port = int(config.conf("PORT", 5000))
-    ipv6 = config.conf("IPV6", False, cast = bool)
+    ipv6 = config.conf("IPV6", False, cast=bool)
     ssl = int(config.conf("SSL", 0)) and True or False
     key_file = config.conf("KEY_FILE", None)
     cer_file = config.conf("CER_FILE", None)
     servers = config.conf_prefix("SERVER_")
     for name, value in servers.items():
         name_s = name.lower()[7:]
         kwargs[name_s] = value
@@ -262,57 +250,48 @@
 
     # creates the netius wsgi server reference using the provided
     # application object and the constructed keyword arguments
     # and then call the serve method starting the event loop with
     # the proper network configuration
     server = netius.servers.WSGIServer(app, **kwargs)
     server.serve(
-        host = host,
-        port = port,
-        ipv6 = ipv6,
-        ssl = ssl,
-        key_file = key_file,
-        cer_file = cer_file
+        host=host, port=port, ipv6=ipv6, ssl=ssl, key_file=key_file, cer_file=cer_file
     )
 
+
 def run_waitress():
-    try: import waitress
+    try:
+        import waitress
     except Exception as exception:
-        raise exceptions.ServerInitError(
-            legacy.UNICODE(exception),
-            server = "waitress"
-        )
+        raise exceptions.ServerInitError(legacy.UNICODE(exception), server="waitress")
 
     host = config.conf("HOST", "127.0.0.1")
     port = int(config.conf("PORT", 5000))
 
     # prepares the application object so that it becomes ready
     # to be executed by the server in the proper way
     app = prepare_app()
 
     # starts the serving process for the waitress server with
     # the proper network configuration values, note that no ssl
     # support is currently available for waitress
-    waitress.serve(
-        app,
-        host = host,
-        port = port
-    )
+    waitress.serve(app, host=host, port=port)
+
 
 def load(
-    app = None,
-    name = None,
-    locales = ("en_us",),
-    secret_key = None,
-    execution = True,
-    redis_session = False,
-    mongo_database = None,
-    logger = None,
-    models = None,
-    safe = False,
+    app=None,
+    name=None,
+    locales=("en_us",),
+    secret_key=None,
+    execution=True,
+    redis_session=False,
+    mongo_database=None,
+    logger=None,
+    models=None,
+    safe=False,
     **kwargs
 ):
     """
     Initial loader function responsible for the overriding of
     the flask loading system and for the loading of configuration.
 
     .. note::
@@ -355,25 +334,26 @@
     :rtype: Application
     :return: The application that is used by the loaded quorum environment in\
     case one was provided that is retrieved, otherwise the newly created one is\
     returned instead.
     """
 
     global APP
-    if APP: return APP
+    if APP:
+        return APP
 
     # runs the initial loading of the configuration from all
     # the currently available sources (eg: file, environment, etc.)
     load_all()
 
     # retrieves the value of all the configuration considered
     # to be base and that are going to be used in the loading
     # of the current application (with default values)
-    debug = config.conf("DEBUG", False, cast = bool)
-    reloader = config.conf("RELOADER", False, cast = bool)
+    debug = config.conf("DEBUG", False, cast=bool)
+    reloader = config.conf("RELOADER", False, cast=bool)
     level_s = config.conf("LEVEL", "WARNING")
     adapter_s = config.conf("ADAPTER", "mongo")
     name = config.conf("NAME", name)
     instance = config.conf("INSTANCE", None)
     force_ssl = config.conf("FORCE_SSL", False)
     redis_url = config.conf("REDISTOGO_URL", None)
     mongo_url = config.conf("MONGOHQ_URL", None)
@@ -396,16 +376,18 @@
 
     # retrieves the possible base URL configuration value and uses it
     # as the basis for the creation of the static URL values to be used
     # by the Flask infra-structure when using _external parameter
     base_url = config.conf("BASE_URL", None)
     if base_url:
         base_parse = legacy.urlparse(base_url)
-        if base_parse.port: server_name = "%s:%d" % (base_parse.hostname, base_parse.port)
-        else: server_name = "%s" % base_parse.hostname
+        if base_parse.port:
+            server_name = "%s:%d" % (base_parse.hostname, base_parse.port)
+        else:
+            server_name = "%s" % base_parse.hostname
         url_scheme = base_parse.scheme
         application_root = base_parse.path
     else:
         server_name, url_scheme, application_root = None, None, None
 
     # tries to retrieve the more specific URL related configuration values
     # defaulting to the base URL calculated ones in case they do not exist
@@ -420,16 +402,18 @@
     config.confs("SERVER_NAME", server_name)
     config.confs("APPLICATION_ROOT", application_root)
     config.confs("PREFERRED_URL_SCHEME", url_scheme)
 
     # retrieves some internal configuration value related with
     # the way that the sessions are going to be handled
     session_cookie_path = config.conf("SESSION_COOKIE_PATH", "/")
-    session_cookie_secure = config.conf("SESSION_COOKIE_SECURE", False, cast = bool)
-    session_refresh_request = config.conf("SESSION_REFRESH_EACH_REQUEST", False, cast = bool)
+    session_cookie_secure = config.conf("SESSION_COOKIE_SECURE", False, cast=bool)
+    session_refresh_request = config.conf(
+        "SESSION_REFRESH_EACH_REQUEST", False, cast=bool
+    )
 
     # re-sets a series of session related values according to quorum
     # predefined structure, this effectively enables sessions on
     # the client side to be handled in a predictable manner
     config.confs("SESSION_COOKIE_PATH", session_cookie_path)
     config.confs("SESSION_COOKIE_SECURE", session_cookie_secure)
     config.confs("SESSION_REFRESH_EACH_REQUEST", session_refresh_request)
@@ -459,15 +443,15 @@
 
     # loads the app configuration from the provided keyword arguments
     # map and from the current dictionary of configuration values
     # (value propagation) and then starts the logging process with the
     # requested logger and provided "verbosity" level
     load_app_config(app, kwargs)
     load_app_config(app, config.confd())
-    start_log(app, name = logger, level = level)
+    start_log(app, name=logger, level=level)
 
     # loads the various paths associated with the application into the
     # current environment to reduce the amount of issues related with
     # the importing of modules and other resources
     load_paths(app)
 
     # loads the complete set of bundle localized in the proper path into
@@ -475,15 +459,16 @@
     # take some time to be performed completely
     load_bundles(app)
 
     # converts the naming of the adapter into a capital case one and
     # then tries to retrieve the associated class for proper instantiation
     # in case the class is not found the default value is set instead
     adapter_s = adapter_s.capitalize() + "Adapter"
-    if not hasattr(data, adapter_s): adapter_s = "MongoAdapter"
+    if not hasattr(data, adapter_s):
+        adapter_s = "MongoAdapter"
     app.adapter = getattr(data, adapter_s)()
 
     # sets the various eval context filters as such by setting their eval
     # context filter flag to true the jinja infra-structure will handle
     # the rest of the operations so that it's properly used
     util.nl_to_br_jinja.evalcontextfilter = True
     util.nl_to_br_jinja.environmentfilter = True
@@ -515,51 +500,69 @@
     app.content_options = CONTENT_OPTIONS
     app.models = models
     app.module = module
     app.path = path
     app.secret_key = secret_key
     app.old_route = app.route
     app.route = route.route
-    app.jinja_options = dict(
-        finalize = finalize
-    )
+    app.jinja_options = dict(finalize=finalize)
     app._locale_d = locales[0]
 
     # takes a snapshot of the current timestamp as it's
     # considered to be the start time of the application
     app.start_time = time.time()
 
     # sets a series of conditional based attributes in both
     # the associated modules and the base app object (as expected)
-    if redis_url: redisdb.url = redis_url
-    if mongo_url: mongodb.url = mongo_url
-    if amqp_url: amqp.url = amqp_url
-    if amazon_id: amazon.id = amazon_id
-    if amazon_secret: amazon.secret = amazon_secret
-    if amazon_bucket: amazon.bucket_name = amazon_bucket
-    if pusher_app_id: pusherc.app_id = pusher_app_id
-    if pusher_key: pusherc.key = pusher_key
-    if pusher_secret: pusherc.secret = pusher_secret
-    if pusher_cluster: pusherc.cluster = pusher_cluster
-    if smtp_host: mail.SMTP_HOST = smtp_host
-    if smtp_user: mail.SMTP_USER = smtp_user
-    if smtp_password: mail.SMTP_PASSWORD = smtp_password
-    if execution: start_execution()
-    if redis_session: app.session_interface = session.RedisSessionInterface(url = redis_url)
-    if mongo_database: mongodb.database = mongo_database + suffix
-    if models: setup_models(models)
-    if force_ssl: extras.SSLify(app)
+    if redis_url:
+        redisdb.url = redis_url
+    if mongo_url:
+        mongodb.url = mongo_url
+    if amqp_url:
+        amqp.url = amqp_url
+    if amazon_id:
+        amazon.id = amazon_id
+    if amazon_secret:
+        amazon.secret = amazon_secret
+    if amazon_bucket:
+        amazon.bucket_name = amazon_bucket
+    if pusher_app_id:
+        pusherc.app_id = pusher_app_id
+    if pusher_key:
+        pusherc.key = pusher_key
+    if pusher_secret:
+        pusherc.secret = pusher_secret
+    if pusher_cluster:
+        pusherc.cluster = pusher_cluster
+    if smtp_host:
+        mail.SMTP_HOST = smtp_host
+    if smtp_user:
+        mail.SMTP_USER = smtp_user
+    if smtp_password:
+        mail.SMTP_PASSWORD = smtp_password
+    if execution:
+        start_execution()
+    if redis_session:
+        app.session_interface = session.RedisSessionInterface(url=redis_url)
+    if mongo_database:
+        mongodb.database = mongo_database + suffix
+    if models:
+        setup_models(models)
+    if force_ssl:
+        extras.SSLify(app)
 
     # verifies if the module that has called the method is not
     # of type main and in case it's not calls the runner methods
     # immediately so that the proper initialization is done, then
     # returns the app reference object to the caller method
-    if not module.__name__ == "__main__": call_run()
+    if not module.__name__ == "__main__":
+        call_run()
     return app
 
+
 def unload():
     """
     Unloads the current quorum instance, after this call
     no more access to the quorum facilities is allowed.
 
     A normal setup of the application would never require
     this function to be called directly.
@@ -572,111 +575,129 @@
     .. note::
 
         After the call to this method most of the functionally of quorum
         will become unavailable until further call to :func:`quorum.load`.
     """
 
     global APP
-    if not APP: return
+    if not APP:
+        return
 
-    if APP.models: teardown_models(APP.models)
+    if APP.models:
+        teardown_models(APP.models)
 
     APP = None
 
-def load_all(path = None):
+
+def load_all(path=None):
     load_config(3)
-    config.load_file(path = path)
+    config.load_file(path=path)
     config.load_env()
 
-def load_config(offset = 1, encoding = "utf-8"):
+
+def load_config(offset=1, encoding="utf-8"):
     element = inspect.stack()[offset]
     module = inspect.getmodule(element[0])
     base_folder = os.path.dirname(module.__file__)
-    config.load(path = base_folder, encoding = encoding)
+    config.load(path=base_folder, encoding=encoding)
+
 
 def load_app_config(app, configs):
     for name, value in configs.items():
         app.config[name] = value
 
+
 def load_paths(app):
-    if not app.root_path in sys.path: sys.path.insert(0, app.root_path)
+    if not app.root_path in sys.path:
+        sys.path.insert(0, app.root_path)
 
-def load_bundles(app, offset = 2):
+
+def load_bundles(app, offset=2):
     # creates the base dictionary that will handle all the loaded
     # bundle information and sets it in the current application
     # object reference so that may be used latter on
     bundles = dict()
     app.bundles = bundles
 
     # inspects the current stack to obtain the reference to the base
     # application module and then uses it to calculate the base path
     # for the application, from there re-constructs the path to the
     # bundle file and verifies its own existence
     element = inspect.stack()[offset]
     module = inspect.getmodule(element[0])
     base_folder = os.path.dirname(module.__file__)
     bundles_path = os.path.join(base_folder, "bundles")
-    if not os.path.exists(bundles_path): return
+    if not os.path.exists(bundles_path):
+        return
 
     # list the bundles directory files and iterates over each of the
     # files to load its own contents into the bundles "registry"
     paths = os.listdir(bundles_path)
     for path in paths:
         # joins the current (base) bundles path with the current path
         # in iteration to create the full path to the file and opens
         # it trying to read its JSON based contents
         path_f = os.path.join(bundles_path, path)
         file = open(path_f, "rb")
-        try: data_j = json.load(file)
-        except Exception: continue
-        finally: file.close()
+        try:
+            data_j = json.load(file)
+        except Exception:
+            continue
+        finally:
+            file.close()
 
         # unpacks the current path in iteration into the base name,
         # locale string and file extension to be used in the registration
         # of the data in the bundles registry
-        try: _base, locale, _extension = path.split(".", 2)
-        except Exception: continue
+        try:
+            _base, locale, _extension = path.split(".", 2)
+        except Exception:
+            continue
 
         # retrieves a possible existing map for the current locale in the
         # registry and updates such map with the loaded data, then re-updates
         # the reference to the locale in the current bundle registry
         bundle = bundles.get(locale, {})
         bundle.update(data_j)
         bundles[locale] = bundle
 
+
 def start_log(
     app,
-    name = None,
-    level = logging.WARN,
-    format_base = log.LOGGING_FORMAT,
-    format_tid = log.LOGGING_FORMAT_TID
+    name=None,
+    level=logging.WARN,
+    format_base=log.LOGGING_FORMAT,
+    format_tid=log.LOGGING_FORMAT_TID,
 ):
     # tries to retrieve some of the default configuration values
     # that are going to be used in the logger startup
     format = config.conf("LOGGING_FORMAT", None)
-    file_log = config.conf("FILE_LOG", False, cast = bool)
-    stream_log = config.conf("STREAM_LOG", True, cast = bool)
-    memory_log = config.conf("MEMORY_LOG", True, cast = bool)
+    file_log = config.conf("FILE_LOG", False, cast=bool)
+    stream_log = config.conf("STREAM_LOG", True, cast=bool)
+    memory_log = config.conf("MEMORY_LOG", True, cast=bool)
     syslog_host = config.conf("SYSLOG_HOST", None)
-    syslog_port = config.conf("SYSLOG_PORT", None, cast = int)
+    syslog_port = config.conf("SYSLOG_PORT", None, cast=int)
     syslog_proto = config.conf("SYSLOG_PROTO", "udp")
-    syslog_kwargs = dict(socktype = socket.SOCK_STREAM) if\
-        syslog_proto in ("tcp",) else dict()
+    syslog_kwargs = (
+        dict(socktype=socket.SOCK_STREAM) if syslog_proto in ("tcp",) else dict()
+    )
     syslog_log = True if syslog_host else False
 
     # tries to determine the default syslog port in case no port
     # is defined and syslog logging is enabled
     if not syslog_port and syslog_log:
         syslog_port = log.SYSLOG_PORTS.get(syslog_proto)
 
     # "resolves" the proper logger file path taking into account
     # the currently defined operative system, should uses the system
     # level path in case the operative system is unix based
-    if os.name == "nt": path_t = "%s"
-    else: path_t = "/var/log/%s"
+    if os.name == "nt":
+        path_t = "%s"
+    else:
+        path_t = "/var/log/%s"
     path = name and path_t % name
 
     # creates the map that is going to be used to store the
     # various handlers registered for the logger
     app.handlers = dict()
 
     # creates the formatter object from the provided string
@@ -707,58 +728,67 @@
         # in case there's an error creating the file handler for
         # the logger prints an error message indicating the problem
         sys.stderr.write("Problem starting logging for file '%s'\n" % path)
         file_handler = None
 
     # adds the various created handler to the current logger so that
     # they are going to be used when using the logger for output
-    if stream_handler: logger.addHandler(stream_handler)
-    if memory_handler: logger.addHandler(memory_handler)
-    if file_handler: logger.addHandler(file_handler)
+    if stream_handler:
+        logger.addHandler(stream_handler)
+    if memory_handler:
+        logger.addHandler(memory_handler)
+    if file_handler:
+        logger.addHandler(file_handler)
 
     # for each of the handlers adds them to the handlers map in case
     # they are valid and defined (no problem in construction)
-    if stream_handler: app.handlers["stream"] = stream_handler
-    if memory_handler: app.handlers["memory"] = memory_handler
-    if file_handler: app.handlers["file"] = file_handler
+    if stream_handler:
+        app.handlers["stream"] = stream_handler
+    if memory_handler:
+        app.handlers["memory"] = memory_handler
+    if file_handler:
+        app.handlers["file"] = file_handler
 
     # iterates over the complete set of handlers currently
     # registered in the logger to properly set the formatter
     # and the level for all of them (as specified)
     for handler in logger.handlers:
         handler.setFormatter(formatter)
         handler.setLevel(level)
 
     # determines if the creation of the syslog handler is required and
     # it that the case created it setting the appropriate formatter to it
-    syslog_handler = logging.handlers.SysLogHandler(
-        (syslog_host, syslog_port), **syslog_kwargs
-    ) if syslog_log else None if syslog_log else None
+    syslog_handler = (
+        logging.handlers.SysLogHandler((syslog_host, syslog_port), **syslog_kwargs)
+        if syslog_log
+        else None if syslog_log else None
+    )
 
     # in case the syslog handler has been created creates the appropriate
     # formatter for it, sets the level and adds it to the logger
     if syslog_handler:
         syslog_formatter = log.BaseFormatter(
             log.LOGGIGN_SYSLOG % APP.name if APP else "quorum",
-            datefmt = "%Y-%m-%dT%H:%M:%S.000000+00:00",
-            wrap = True
+            datefmt="%Y-%m-%dT%H:%M:%S.000000+00:00",
+            wrap=True,
         )
         syslog_handler.setLevel(level)
         syslog_handler.setFormatter(syslog_formatter)
         logger.addHandler(syslog_handler)
         app.handlers["syslog"] = syslog_handler
 
     # runs the extra logging step for the current state, meaning that
     # some more handlers may be created according to the logging config
     extra_logging(logger, level, formatter)
 
     # sets the current logger in the top level app value so that
     # this logger is going to be used as the quorum logger
     app.logger_q = logger
 
+
 def extra_logging(logger, level, formatter):
     """
     Loads the complete set of logging handlers defined in the
     current logging value, should be a map of definitions.
 
     This handlers will latter be used for piping the various
     logging messages to certain output channels.
@@ -777,172 +807,210 @@
     :param formatter: The logging formatter instance to be set in\
     the handler for formatting messages to the output.
     """
 
     # verifies if the logging attribute of the current instance is
     # defined and in case it's not returns immediately
     logging = config.conf("LOGGING", None)
-    if not logging: return
+    if not logging:
+        return
 
     # iterates over the complete set of handler configuration in the
     # logging to create the associated handler instances
     for _config in logging:
         # gathers the base information on the current handler configuration
         # running also the appropriate transformation on the level
         name = _config.get("name", None)
         __level = _config.get("level", level)
         __level = _level(__level)
 
         # "clones" the configuration dictionary and then removes the base
         # values so that they do not interfere with the building
         _config = dict(_config)
-        if "level" in _config: del _config["level"]
-        if "name" in _config: del _config["name"]
+        if "level" in _config:
+            del _config["level"]
+        if "name" in _config:
+            del _config["name"]
 
         # retrieves the proper building, skipping the current loop in case
         # it does not exits and then builds the new handler instance, setting
         # the proper level and formatter and then adding it to the logger
-        if not hasattr(log, name + "_handler"): continue
+        if not hasattr(log, name + "_handler"):
+            continue
         builder = getattr(log, name + "_handler")
         handler = builder(**_config)
         handler.setLevel(__level)
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
-def get_app(app = None):
+
+def get_app(app=None):
     return app or APP
 
-def get_adapter(app = None):
+
+def get_adapter(app=None):
     return APP and APP.adapter
 
-def get_log(app = None):
+
+def get_log(app=None):
     app = app or APP
-    if not app: return None
+    if not app:
+        return None
     is_custom = hasattr(app, "logger_q")
     return app.logger_q if is_custom else app.logger
 
-def get_level(app = None):
-    logger = get_log(app = app)
-    if not logger: return None
+
+def get_level(app=None):
+    logger = get_log(app=app)
+    if not logger:
+        return None
     return logger.level
 
-def get_handlers(app = None):
-    logger = get_log(app = app)
-    if not logger: return None
+
+def get_handlers(app=None):
+    logger = get_log(app=app)
+    if not logger:
+        return None
     return logger.handlers
 
-def get_handler(name, app = None):
+
+def get_handler(name, app=None):
     app = app or APP
-    if not app: return None
+    if not app:
+        return None
     return app.handlers.get(name, None)
 
-def get_bundle(name, app = None, split = True):
+
+def get_bundle(name, app=None, split=True):
     app = app or APP
-    if not app: return None
+    if not app:
+        return None
     bundle = app.bundles.get(name, None)
-    if bundle: return bundle
+    if bundle:
+        return bundle
     if split and name:
         base = name.split("_", 1)[0]
         bundle = app.bundles.get(base, None)
-        if bundle: return bundle
+        if bundle:
+            return bundle
     name = _best_locale(name)
     return app.bundles.get(name, None)
 
-def is_devel(app = None):
-    level = get_level(app = app)
-    if not level: return False
+
+def is_devel(app=None):
+    level = get_level(app=app)
+    if not level:
+        return False
     return level < logging.INFO
 
+
 def finalize(value):
     # returns an empty string as value representation
     # for unset values, this is the default representation
     # to be used in the template engine
-    if value == None: return ""
+    if value == None:
+        return ""
     return value
 
+
 def before_request():
     flask.request.args_s = util.load_form(flask.request.args)
     flask.request.form_s = util.load_form(flask.request.form)
     flask.request.locale = util.load_locale(APP.locales)
     util.set_locale()
 
+
 def after_request(response):
-    if APP.safe: util.reset_locale()
+    if APP.safe:
+        util.reset_locale()
     util.anotate_async(response)
     util.anotate_secure(response)
     return response
 
+
 def context_processor():
     return dict(
-        acl = acl.check_login,
-        conf = config.conf,
-        locale = util.to_locale,
-        nl_to_br = util.nl_to_br,
-        sp_to_nbsp = util.sp_to_nbsp,
-        date_time = util.date_time,
-        time = time,
-        datetime = datetime,
-        zip = zip
+        acl=acl.check_login,
+        conf=config.conf,
+        locale=util.to_locale,
+        nl_to_br=util.nl_to_br,
+        sp_to_nbsp=util.sp_to_nbsp,
+        date_time=util.date_time,
+        time=time,
+        datetime=datetime,
+        zip=zip,
     )
 
+
 def start_execution():
     # creates the thread that it's going to be used to
     # execute the various background tasks and starts
     # it, providing the mechanism for execution
     execution.background_t = execution.ExecutionThread()
     background_t = execution.background_t
     background_t.start()
 
+
 @atexit.register
 def stop_execution():
     # stop the execution thread so that it's possible to
     # the process to return the calling
     background_t = execution.background_t
     background_t and background_t.stop()
 
+
 def setup_models(models):
-    _models_c = models_c(models = models)
-    for model_c in _models_c: model_c.setup()
+    _models_c = models_c(models=models)
+    for model_c in _models_c:
+        model_c.setup()
+
 
 def teardown_models(models):
-    _models_c = models_c(models = models)
-    for model_c in _models_c: model_c.teardown()
+    _models_c = models_c(models=models)
+    for model_c in _models_c:
+        model_c.teardown()
 
-def models_c(models = None):
+
+def models_c(models=None):
     # retrieves the proper models defaulting to the current
     # application models in case they are not defined, note
     # that in case the model is not defined an empty list is
     # going to be returned (fallback process)
     models = models or APP.models
-    if not models: return []
+    if not models:
+        return []
 
     # creates the list that will hold the various model
     # class discovered through module analysis
     models_c = []
 
     # iterates over the complete set of items in the models
     # modules to find the ones that inherit from the base
     # model class for those are the real models
     for _name, value in models.__dict__.items():
         # verifies if the current value in iteration inherits
         # from the top level model in case it does not continues
         # the loop as there's nothing to be done
-        try: is_valid = issubclass(value, model.Model)
-        except Exception: is_valid = False
-        if not is_valid: continue
+        try:
+            is_valid = issubclass(value, model.Model)
+        except Exception:
+            is_valid = False
+        if not is_valid:
+            continue
 
         # adds the current value in iteration as a new class
         # to the list that hold the various model classes
         models_c.append(value)
 
     # returns the list containing the various model classes
     # to the caller method as expected by definition
     return models_c
 
-def resolve(identifier = "_id", counters = True):
+
+def resolve(identifier="_id", counters=True):
     # creates the list that will hold the definition of the current
     # model classes with a sequence of name and identifier values
     entities = []
 
     # retrieves the complete set of model classes registered
     # for the current application and for each of them retrieves
     # the name of it and creates a tuple with the name and the
@@ -952,32 +1020,38 @@
     for model_c in _models_c:
         name = model_c._name()
         tuple = (name, identifier)
         entities.append(tuple)
 
     # in case the counters flag is defined the counters tuple containing
     # the counters table name and identifier is added to the entities list
-    if counters: entities.append(("counters", identifier))
+    if counters:
+        entities.append(("counters", identifier))
 
     # returns the resolution list to the caller method as requested
     # by the call to this method
     return entities
 
+
 def templates_path():
     return os.path.join(APP.root_path, APP.template_folder)
 
+
 def bundles_path():
     return os.path.join(APP.root_path, "bundles")
 
+
 def base_path(*args, **kwargs):
     return os.path.join(APP.root_path, *args)
 
+
 def has_context():
     return flask.has_app_context()
 
+
 def ensure_context(function):
     """
     Decorator that makes sure that the underlying execution
     method/function is run inside a valid flask app context.
 
     In case there's currently no app context defined it uses
     the global Application reference to create a new one.
@@ -1000,20 +1074,23 @@
                 result = function(*args, **kwargs)
         else:
             result = function(*args, **kwargs)
         return result
 
     return interceptor
 
+
 def onrun(function):
     fname = function.__name__
-    if fname in RUN_F: return
+    if fname in RUN_F:
+        return
     RUN_F[fname] = function
     return function
 
+
 def _level(level):
     """
     Converts the provided logging level value into the best
     representation of it, so that it may be used to update
     a logger's level of representation.
 
     This method takes into account the current interpreter
@@ -1025,28 +1102,35 @@
     :rtype: int
     :return: The best representation of the level so that it may
     be used freely for the setting of logging levels under the
     current running interpreter.
     """
 
     level_t = type(level)
-    if level_t == int: return level
-    if level == None: return level
-    if level == "SILENT": return log.SILENT
+    if level_t == int:
+        return level
+    if level == None:
+        return level
+    if level == "SILENT":
+        return log.SILENT
     if hasattr(logging, "_checkLevel"):
         return logging._checkLevel(level)
     return logging.getLevelName(level)
 
-def _best_locale(locale, app = None):
-    if not locale: return locale
+
+def _best_locale(locale, app=None):
+    if not locale:
+        return locale
     app = app or APP
     for _locale in app.locales:
         is_valid = _locale.startswith(locale)
-        if not is_valid: continue
+        if not is_valid:
+            continue
         return _locale
     return locale
 
+
 # runs the monkey patching of the flask module so that it
 # may be used according to the quorum specification, this
 # is used in order to avoid minimal effort in the conversion
 # of old flask based applications (reverse compatibility)
 monkey()
```

### Comparing `quorum-0.8.2/src/quorum/validation.py` & `quorum-0.8.3/src/quorum/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import re
@@ -69,15 +60,16 @@
 """ The email regex used to validate
 if the provided value is in fact an email """
 
 URL_REGEX = re.compile(URL_REGEX_VALUE)
 """ The URL regex used to validate
 if the provided value is in fact an URL/URI """
 
-def validate(method = None, methods = [], object = None, ctx = None, build = True):
+
+def validate(method=None, methods=[], object=None, ctx=None, build=True):
     # uses the provided method to retrieves the complete
     # set of methods to be used for validation, this provides
     # an extra level of indirection
     methods = method() if method else methods
     errors = []
 
     # verifies if the provided object is valid in such case creates
@@ -92,329 +84,454 @@
         # "load" it as JSON data, in case it fails gracefully
         # handles the failure setting the value as an empty map
         data_j = util.request_json()
 
         # uses all the values referencing data in the request to try
         # to populate the object this way it may be constructed using
         # any of theses strategies (easier for the developer)
-        for name, value in data_j.items(): object[name] = value
-        for name, value in flask.request.files.items(): object[name] = value
-        for name, value in flask.request.form.items(): object[name] = value
-        for name, value in flask.request.args.items(): object[name] = value
+        for name, value in data_j.items():
+            object[name] = value
+        for name, value in flask.request.files.items():
+            object[name] = value
+        for name, value in flask.request.form.items():
+            object[name] = value
+        for name, value in flask.request.args.items():
+            object[name] = value
 
     # iterates over the complete set of methods registered for validation
     # and runs them expecting exceptions to be raised from them, each adding
     # new errors to the current errors stack
     for method in methods:
-        try: method(object, ctx = ctx)
+        try:
+            method(object, ctx=ctx)
         except exceptions.ValidationMultipleError as error:
             errors.extend(error.errors)
         except exceptions.ValidationInternalError as error:
             errors.append((error.name, error.message))
 
     # creates the map that will be used to store the association between the
     # field name of the object and the validation errors associated with it
     errors_map = dict()
     for name, message in errors:
-        if not name in errors_map: errors_map[name] = []
+        if not name in errors_map:
+            errors_map[name] = []
         _errors = errors_map[name]
         _errors.append(message)
 
     # returns both the newly created errors map that associates each of the
     # model name with the sequence of errors and the validated object (state)
     return errors_map, object
 
-def validate_b(method = None, methods = [], object = None, ctx = None, build = True):
+
+def validate_b(method=None, methods=[], object=None, ctx=None, build=True):
     errors_map, object = validate(
-        method = method,
-        methods = methods,
-        object = object,
-        ctx = ctx,
-        build = build
+        method=method, methods=methods, object=object, ctx=ctx, build=build
     )
     result = False if errors_map else True
     return result
 
-def validate_e(method = None, methods = [], object = None, ctx = None, build = True):
+
+def validate_e(method=None, methods=[], object=None, ctx=None, build=True):
     errors_map, object = validate(
-        method = method,
-        methods = methods,
-        object = object,
-        ctx = ctx,
-        build = build
+        method=method, methods=methods, object=object, ctx=ctx, build=build
     )
-    if not errors_map: return
+    if not errors_map:
+        return
     raise exceptions.ValidationError(errors_map, object)
 
+
 def safe(comparision):
-    try: return comparision()
-    except TypeError: return False
+    try:
+        return comparision()
+    except TypeError:
+        return False
+
 
-def eq(name, value_c, message = "must be equal to %s", locale = True):
+def eq(name, value_c, message="must be equal to %s", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == value_c: return True
+        if value == None:
+            return True
+        if value == value_c:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % str(value_c))
+
     return validation
 
-def gt(name, value_c, message = "must be greater than %s", locale = True):
+
+def gt(name, value_c, message="must be greater than %s", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if safe(lambda: value > value_c): return True
+        if value == None:
+            return True
+        if safe(lambda: value > value_c):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % str(value_c))
+
     return validation
 
-def gte(name, value_c, message = "must be greater than or equal to %s", locale = True):
+
+def gte(name, value_c, message="must be greater than or equal to %s", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if safe(lambda: value >= value_c): return True
+        if value == None:
+            return True
+        if safe(lambda: value >= value_c):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % str(value_c))
+
     return validation
 
-def lt(name, value_c, message = "must be less than %s", locale = True):
+
+def lt(name, value_c, message="must be less than %s", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if safe(lambda: value < value_c): return True
+        if value == None:
+            return True
+        if safe(lambda: value < value_c):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % str(value_c))
+
     return validation
 
-def lte(name, value_c, message = "must be less than or equal to %s", locale = True):
+
+def lte(name, value_c, message="must be less than or equal to %s", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if safe(lambda: value <= value_c): return True
+        if value == None:
+            return True
+        if safe(lambda: value <= value_c):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % str(value_c))
+
     return validation
 
-def not_null(name, message = "value is not set", locale = True):
+
+def not_null(name, message="value is not set", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if not value == None: return True
+        if not value == None:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def not_empty(name, message = "value is empty", locale = True):
+
+def not_empty(name, message="value is empty", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if len(value): return True
+        if value == None:
+            return True
+        if len(value):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def not_false(name, message = "value is false", locale = True):
+
+def not_false(name, message="value is false", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if not value == False: return True
+        if value == None:
+            return True
+        if not value == False:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_in(name, values, message = "value is not in set", locale = True):
+
+def is_in(name, values, message="value is not in set", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value in values: return True
+        if value == None:
+            return True
+        if value in values:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_upper(name, message = "value contains lower cased characters", locale = True):
+
+def is_upper(name, message="value contains lower cased characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if value == value.upper(): return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if value == value.upper():
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_lower(name, message = "value contains upper cased characters", locale = True):
+
+def is_lower(name, message="value contains upper cased characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if value == value.lower(): return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if value == value.lower():
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_simple(name, message = "value contains invalid characters", locale = True):
+
+def is_simple(name, message="value contains invalid characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if SIMPLE_REGEX.match(value): return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if SIMPLE_REGEX.match(value):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_email(name, message = "value is not a valid email", locale = True):
+
+def is_email(name, message="value is not a valid email", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if EMAIL_REGEX.match(value): return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if EMAIL_REGEX.match(value):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_url(name, message = "value is not a valid URL", locale = True):
+
+def is_url(name, message="value is not a valid URL", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if URL_REGEX.match(value): return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if URL_REGEX.match(value):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def is_regex(name, regex, message = "value has incorrect format", locale = True):
+
+def is_regex(name, regex, message="value has incorrect format", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
+        if value == None:
+            return True
+        if value == "":
+            return True
         match = re.match(regex, value)
-        if match: return True
+        if match:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def field_eq(name, field, message = "must be equal to %s", locale = True):
+
+def field_eq(name, field, message="must be equal to %s", locale=True):
     def validation(object, ctx):
         name_v = object.get(name, None)
         field_v = object.get(field, None)
-        if name_v == None: return True
-        if field_v == None: return True
-        if name_v == field_v: return True
+        if name_v == None:
+            return True
+        if field_v == None:
+            return True
+        if name_v == field_v:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % field)
+
     return validation
 
-def field_gt(name, field, message = "must be greater than %s", locale = True):
+
+def field_gt(name, field, message="must be greater than %s", locale=True):
     def validation(object, ctx):
         name_v = object.get(name, None)
         field_v = object.get(field, None)
-        if name_v == None: return True
-        if field_v == None: return True
-        if safe(lambda: name_v > field_v): return True
+        if name_v == None:
+            return True
+        if field_v == None:
+            return True
+        if safe(lambda: name_v > field_v):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % field)
+
     return validation
 
-def field_gte(name, field, message = "must be greater or equal than %s", locale = True):
+
+def field_gte(name, field, message="must be greater or equal than %s", locale=True):
     def validation(object, ctx):
         name_v = object.get(name, None)
         field_v = object.get(field, None)
-        if name_v == None: return True
-        if field_v == None: return True
-        if safe(lambda: name_v >= field_v): return True
+        if name_v == None:
+            return True
+        if field_v == None:
+            return True
+        if safe(lambda: name_v >= field_v):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % field)
+
     return validation
 
-def field_lt(name, field, message = "must be less than %s", locale = True):
+
+def field_lt(name, field, message="must be less than %s", locale=True):
     def validation(object, ctx):
         name_v = object.get(name, None)
         field_v = object.get(field, None)
-        if name_v == None: return True
-        if field_v == None: return True
-        if safe(lambda: name_v < field_v): return True
+        if name_v == None:
+            return True
+        if field_v == None:
+            return True
+        if safe(lambda: name_v < field_v):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % field)
+
     return validation
 
-def field_lte(name, field, message = "must be less or equal than %s", locale = True):
+
+def field_lte(name, field, message="must be less or equal than %s", locale=True):
     def validation(object, ctx):
         name_v = object.get(name, None)
         field_v = object.get(field, None)
-        if name_v == None: return True
-        if field_v == None: return True
-        if safe(lambda: name_v <= field_v): return True
+        if name_v == None:
+            return True
+        if field_v == None:
+            return True
+        if safe(lambda: name_v <= field_v):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % field)
+
     return validation
 
-def string_gt(name, size, message = "must be larger than %d characters", locale = True):
+
+def string_gt(name, size, message="must be larger than %d characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if len(value) > size: return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if len(value) > size:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % size)
+
     return validation
 
-def string_lt(name, size, message = "must be smaller than %d characters", locale = True):
+
+def string_lt(name, size, message="must be smaller than %d characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if len(value) < size: return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if len(value) < size:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % size)
+
     return validation
 
-def string_eq(name, size, message = "must be exactly %d characters", locale = True):
+
+def string_eq(name, size, message="must be exactly %d characters", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
-        if len(value) == size: return True
+        if value == None:
+            return True
+        if value == "":
+            return True
+        if len(value) == size:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l % size)
+
     return validation
 
-def equals(first_name, second_name, message = "value is not equal to %s", locale = True):
+
+def equals(first_name, second_name, message="value is not equal to %s", locale=True):
     def validation(object, ctx):
         first_value = object.get(first_name, None)
         second_value = object.get(second_name, None)
-        if first_value == None: return True
-        if second_value == None: return True
-        if first_value == second_value: return True
+        if first_value == None:
+            return True
+        if second_value == None:
+            return True
+        if first_value == second_value:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(first_name, message_l % second_name)
+
     return validation
 
-def not_past(name, message = "date is in the past", locale = True):
+
+def not_past(name, message="date is in the past", locale=True):
     def validation(object, ctx):
         value = object.get(name, None)
-        if value == None: return True
-        if value >= datetime.datetime.utcnow(): return True
+        if value == None:
+            return True
+        if value >= datetime.datetime.utcnow():
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def not_duplicate(name, collection, message = "value is duplicate", locale = True):
+
+def not_duplicate(name, collection, message="value is duplicate", locale=True):
     def validation(object, ctx):
         _id = object.get("_id", None)
         value = object.get(name, None)
-        if value == None: return True
-        if value == "": return True
+        if value == None:
+            return True
+        if value == "":
+            return True
         adapter = common.base().get_adapter()
         _collection = adapter.collection(collection)
-        item = _collection.find_one({name : value})
-        if not item: return True
-        if str(item["_id"]) == str(_id): return True
+        item = _collection.find_one({name: value})
+        if not item:
+            return True
+        if str(item["_id"]) == str(_id):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def all_different(name, name_ref = None, message = "has duplicates", locale = True):
+
+def all_different(name, name_ref=None, message="has duplicates", locale=True):
     def validation(object, ctx):
         # uses the currently provided context to retrieve
         # the definition of the name to be validation and
         # in it's a valid relation type tries to retrieve
         # the underlying referenced name otherwise default
         # to the provided one or the id name
         cls = ctx.__class__
@@ -423,38 +540,47 @@
         _name_ref = name_ref or (hasattr(type, "_name") and type._name or "id")
 
         # tries to retrieve both the value for the identifier
         # in the current object and the values of the sequence
         # that is going to be used for all different matching in
         # case any of them does not exist returns valid
         value = object.get(name, None)
-        if value == None: return True
-        if len(value) == 0: return True
+        if value == None:
+            return True
+        if len(value) == 0:
+            return True
 
         # verifies if the sequence is in fact a proxy object and
         # contains the ids attribute in case that's the case the
         # ids attributes is retrieved as the sequence instead
-        if hasattr(value, "ids"): values = value.ids
+        if hasattr(value, "ids"):
+            values = value.ids
 
         # otherwise this is a normal sequence and the it must be
         # iterates to check if the reference name should be retrieve
         # or if the concrete values should be used instead
-        else: values = [getattr(_value, _name_ref) if hasattr(_value, _name_ref) else _value\
-            for _value in value]
+        else:
+            values = [
+                getattr(_value, _name_ref) if hasattr(_value, _name_ref) else _value
+                for _value in value
+            ]
 
         # creates a set structure from the the sequence of values
         # and in case the size of the sequence and the set are the
         # same the sequence is considered to not contain duplicates
         values_set = set(values)
-        if len(value) == len(values_set): return True
+        if len(value) == len(values_set):
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
-def no_self(name, name_ref = None, message = "contains self", locale = True):
+
+def no_self(name, name_ref=None, message="contains self", locale=True):
     def validation(object, ctx):
         # uses the currently provided context to retrieve
         # the definition of the name to be validation and
         # in it's a valid relation type tries to retrieve
         # the underlying referenced name otherwise default
         # to the provided one or the id name
         cls = ctx.__class__
@@ -464,32 +590,41 @@
 
         # tries to retrieve both the value for the identifier
         # in the current object and the values of the sequence
         # that is going to be used for existence matching in
         # case any of them does not exist returns valid
         _id = object.get(_name_ref, None)
         value = object.get(name, None)
-        if _id == None: return True
-        if value == None: return True
+        if _id == None:
+            return True
+        if value == None:
+            return True
 
         # verifies if the sequence is in fact a proxy object and
         # contains the ids attribute in case that's the case the
         # ids attributes is retrieved as the sequence instead
-        if hasattr(value, "ids"): values = value.ids
+        if hasattr(value, "ids"):
+            values = value.ids
 
         # otherwise this is a normal sequence and the it must be
         # iterates to check if the reference name should be retrieve
         # or if the concrete values should be used instead
-        else: values = [getattr(_value, _name_ref) if hasattr(_value, _name_ref) else _value\
-            for _value in value]
+        else:
+            values = [
+                getattr(_value, _name_ref) if hasattr(_value, _name_ref) else _value
+                for _value in value
+            ]
 
         # verifies if the current identifier value exists in the
         # sequence and if that's the case raises the validation
         # exception indicating the validation problem
         exists = _id in values
-        if not exists: return True
+        if not exists:
+            return True
         message_l = _to_locale(message) if locale else message
         raise exceptions.ValidationInternalError(name, message_l)
+
     return validation
 
+
 def _to_locale(value):
     return util.to_locale(value)
```

### Comparing `quorum-0.8.2/src/quorum/execution.py` & `quorum-0.8.3/src/quorum/execution.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import time
@@ -56,14 +47,15 @@
 this amount should be small enough to provide some
 resolution level to the schedule execution """
 
 background_t = None
 """ The background execution task to be started by
 the quorum execution system (global value) """
 
+
 class ExecutionThread(threading.Thread):
     """
     The thread to be used in the execution of "random"
     "callables" for a provided time, this thread contains
     a series of thread safe method for operating over
     the work tuples.
     """
@@ -83,15 +75,15 @@
     work to be executed """
 
     def __init__(self):
         """
         Constructor of the class.
         """
 
-        threading.Thread.__init__(self, name = "Execution")
+        threading.Thread.__init__(self, name="Execution")
 
         self.daemon = True
         self.work_list = []
         self.work_lock = threading.RLock()
 
     def run(self):
         # iterates continuously (executing work)
@@ -113,15 +105,16 @@
 
             try:
                 # iterates continuously to execute all the
                 # work that can be executed in the work list
                 while True:
                     # in case there is no work pending to be
                     # executed must exist immediately
-                    if not self.work_list: break
+                    if not self.work_list:
+                        break
 
                     # retrieves the current work tuple to
                     # be used and executes it in case the
                     # time has passed (should be executed)
                     _time, callable, callback, args, kwargs = self.work_list[0]
                     if _time < current_time:
                         execution_list.append((callable, callback, args, kwargs))
@@ -143,63 +136,71 @@
                 # executes the "callable" and logs the error in case the
                 # execution fails (must be done to log the error) then
                 # sets the error flag with the exception variable
                 try:
                     callable(*args, **kwargs)
                 except Exception as exception:
                     error = exception
-                    log.warning(str(exception), log_trace = True)
+                    log.warning(str(exception), log_trace=True)
 
                 # calls the callback method with the currently set error
                 # in order to notify the runtime about the problem, only
                 # calls the callback in case such method is defined
-                callback and callback(error = error)
+                callback and callback(error=error)
 
             # sleeps for a while so that the process may
             # released for different tasks
             time.sleep(SLEEP_TIME)
 
     def stop(self):
         self.run_flag = False
 
-    def insert_work(self, callable, args = [], kwargs = {}, target_time = None, callback = None):
+    def insert_work(
+        self, callable, args=[], kwargs={}, target_time=None, callback=None
+    ):
         target_time = target_time or time.time()
         work = (target_time, callable, callback, args, kwargs)
         self.work_lock.acquire()
-        try: heapq.heappush(self.work_list, work)
-        finally: self.work_lock.release()
+        try:
+            heapq.heappush(self.work_list, work)
+        finally:
+            self.work_lock.release()
 
-def background(timeout = None):
+
+def background(timeout=None):
 
     def decorator(function):
         _timeout = timeout or 0.0
 
-        def schedule(error = None, force = False):
-            if timeout == None and not force: return
+        def schedule(error=None, force=False):
+            if timeout == None and not force:
+                return
             target = time.time() + _timeout
             insert_work(function, target, schedule)
 
         # retrieves the name of the function and in
         # case the name already exists in the global
         # list of background execution tasks returns
         # immediately (nothing to be done, duplicate)
         fname = function.__name__
         exists = fname in BACKGROUND
-        if exists: return function
+        if exists:
+            return function
 
         # runs the scheduling operation on the task and
         # then adds the function name to the list of already
         # registered names
-        schedule(force = True)
+        schedule(force=True)
         BACKGROUND.append(fname)
         return function
 
     return decorator
 
-def insert_work(callable, args = [], kwargs = {}, target_time = None, callback = None):
+
+def insert_work(callable, args=[], kwargs={}, target_time=None, callback=None):
     """
     Runs the provided callable (function, method, etc) in a separated
     thread context under submission of a queue system.
     It's possible to control the runtime for the execution with the
     ``target_time`` argument and it's also possible to be notified
     of the end of the execution providing a callable to the ``callback``
     parameter.
@@ -224,120 +225,123 @@
     :type callback: Function
     :param callback: The callback function to be called upon finishing the\
     execution of the callable, in case an error (exception) on executing\
     the callback the error is passed as error argument.
     """
 
     background_t.insert_work(
-        callable,
-        args = args,
-        kwargs = kwargs,
-        target_time = target_time,
-        callback = callback
+        callable, args=args, kwargs=kwargs, target_time=target_time, callback=callback
     )
 
+
 def interval_work(
-    callable,
-    args = [],
-    kwargs = {},
-    callback = None,
-    initial = None,
-    interval = 60,
-    eval = None
+    callable, args=[], kwargs={}, callback=None, initial=None, interval=60, eval=None
 ):
     initial = initial or (eval and eval()) or time.time()
     composed = build_composed(callable, initial, interval, eval, callback)
     insert_work(
-        composed,
-        args = args,
-        kwargs = kwargs,
-        target_time = initial,
-        callback = callback
+        composed, args=args, kwargs=kwargs, target_time=initial, callback=callback
     )
     return initial
 
-def seconds_work(callable, offset = 0, *args, **kwargs):
+
+def seconds_work(callable, offset=0, *args, **kwargs):
     eval = lambda: seconds_eval(offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
+
 
-def minutes_work(callable, offset = 0, *args, **kwargs):
+def minutes_work(callable, offset=0, *args, **kwargs):
     eval = lambda: minutes_eval(offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
+
 
-def hourly_work(callable, offset = 0, *args, **kwargs):
+def hourly_work(callable, offset=0, *args, **kwargs):
     eval = lambda: hourly_eval(offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
 
-def daily_work(callable, offset = 0, *args, **kwargs):
+
+def daily_work(callable, offset=0, *args, **kwargs):
     eval = lambda: daily_eval(offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
+
 
-def weekly_work(callable, weekday = 4, offset = 0, *args, **kwargs):
+def weekly_work(callable, weekday=4, offset=0, *args, **kwargs):
     eval = lambda: weekly_eval(weekday, offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
 
-def monthly_work(callable, monthday = 1, offset = 0, *args, **kwargs):
+
+def monthly_work(callable, monthday=1, offset=0, *args, **kwargs):
     eval = lambda: monthly_eval(monthday, offset)
-    return interval_work(callable, eval = eval, *args, **kwargs)
+    return interval_work(callable, eval=eval, *args, **kwargs)
+
 
-def seconds_eval(offset, now = None):
+def seconds_eval(offset, now=None):
     now = now or datetime.datetime.utcnow()
-    next = now + datetime.timedelta(seconds = offset)
+    next = now + datetime.timedelta(seconds=offset)
     next_tuple = next.utctimetuple()
     return calendar.timegm(next_tuple)
 
-def minutes_eval(offset, now = None):
+
+def minutes_eval(offset, now=None):
     now = now or datetime.datetime.utcnow()
     current = datetime.datetime(
-        year = now.year,
-        month = now.month,
-        day = now.day,
-        hour = now.hour,
-        minute = now.minute
+        year=now.year, month=now.month, day=now.day, hour=now.hour, minute=now.minute
     )
-    next = current + datetime.timedelta(minutes = 1, seconds = offset)
+    next = current + datetime.timedelta(minutes=1, seconds=offset)
     next_tuple = next.utctimetuple()
     return calendar.timegm(next_tuple)
 
-def hourly_eval(offset, now = None):
+
+def hourly_eval(offset, now=None):
     now = now or datetime.datetime.utcnow()
-    current = datetime.datetime(year = now.year, month = now.month, day = now.day, hour = now.hour)
-    next = current + datetime.timedelta(hours = 1, seconds = offset)
+    current = datetime.datetime(
+        year=now.year, month=now.month, day=now.day, hour=now.hour
+    )
+    next = current + datetime.timedelta(hours=1, seconds=offset)
     next_tuple = next.utctimetuple()
     return calendar.timegm(next_tuple)
 
-def daily_eval(offset, now = None):
+
+def daily_eval(offset, now=None):
     now = now or datetime.datetime.utcnow()
-    today = datetime.datetime(year = now.year, month = now.month, day = now.day)
-    tomorrow = today + datetime.timedelta(days = 1, seconds = offset)
+    today = datetime.datetime(year=now.year, month=now.month, day=now.day)
+    tomorrow = today + datetime.timedelta(days=1, seconds=offset)
     tomorrow_tuple = tomorrow.utctimetuple()
     return calendar.timegm(tomorrow_tuple)
 
-def weekly_eval(weekday, offset, now = None):
+
+def weekly_eval(weekday, offset, now=None):
     now = now or datetime.datetime.utcnow()
-    today = datetime.datetime(year = now.year, month = now.month, day = now.day)
+    today = datetime.datetime(year=now.year, month=now.month, day=now.day)
     distance = (weekday - today.weekday()) % 7
-    weekday = today + datetime.timedelta(days = distance, seconds = offset)
-    if weekday < now: weekday += datetime.timedelta(days = 7)
+    weekday = today + datetime.timedelta(days=distance, seconds=offset)
+    if weekday < now:
+        weekday += datetime.timedelta(days=7)
     weekday_tuple = weekday.utctimetuple()
     return calendar.timegm(weekday_tuple)
 
-def monthly_eval(monthday, offset, now = None):
+
+def monthly_eval(monthday, offset, now=None):
     now = now or datetime.datetime.utcnow()
-    next_year, next_month = (now.year + 1, 1) if now.month == 12 else (now.year, now.month + 1)
-    if now.day > monthday: month, year = (next_month, next_year)
-    else: month, year = (now.month, now.year)
-    monthday = datetime.datetime(year = year, month = month, day = monthday)
-    monthday = monthday + datetime.timedelta(seconds = offset)
+    next_year, next_month = (
+        (now.year + 1, 1) if now.month == 12 else (now.year, now.month + 1)
+    )
+    if now.day > monthday:
+        month, year = (next_month, next_year)
+    else:
+        month, year = (now.month, now.year)
+    monthday = datetime.datetime(year=year, month=month, day=monthday)
+    monthday = monthday + datetime.timedelta(seconds=offset)
     if monthday < now:
-        monthday = datetime.datetime(year = next_year, month = next_month, day = monthday.day)
-        monthday += datetime.timedelta(seconds = offset)
+        monthday = datetime.datetime(year=next_year, month=next_month, day=monthday.day)
+        monthday += datetime.timedelta(seconds=offset)
     monthday_tuple = monthday.utctimetuple()
     return calendar.timegm(monthday_tuple)
 
+
 def build_composed(callable, target_time, interval, eval, callback):
 
     def composed(*args, **kwargs):
         try:
             # runs the initial callable, propagating the provided normal arguments
             # and keyword based ones to the callable as it's expected by the current
             # underlying running logic (and by the specification)
@@ -351,26 +355,28 @@
             else:
                 # retrieves the current time value as the final value of execution, then
                 # calculates the delta value and uses it to verify if the current work is
                 # allowed for initial based time delta calculus (avoiding queue starvation)
                 final = time.time()
                 delta = final - target_time
                 is_valid = delta < interval
-                if is_valid: next_time = target_time + interval
-                else: next_time = final + interval
+                if is_valid:
+                    next_time = target_time + interval
+                else:
+                    next_time = final + interval
 
             # builds a new callable (composed) method taking into account the state and
             # inserts the work unit again into the queue of processing
             composed = build_composed(callable, next_time, interval, eval, callback)
             insert_work(
                 composed,
-                args = args,
-                kwargs = kwargs,
-                target_time = next_time,
-                callback = callback
+                args=args,
+                kwargs=kwargs,
+                target_time=next_time,
+                callback=callback,
             )
 
         # returns the current result from the original callable to the calling method,
         # this is the expected behavior from the scheduler point of view
         return result
 
     return composed
```

### Comparing `quorum-0.8.2/src/quorum/test/export.py` & `quorum-0.8.3/src/quorum/test/export.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,106 +18,92 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
 
 import quorum
 
+
 class ExportTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(name = __name__)
+            quorum.load(name=__name__)
         except Exception:
             self.skip()
 
     def tearDown(self):
         try:
             adapter = quorum.get_adapter()
             adapter.drop_db()
-        except Exception: pass
-        finally: quorum.unload()
+        except Exception:
+            pass
+        finally:
+            quorum.unload()
 
     @quorum.secured
     def test_import_single(self):
         structure = {
-            "person:id" : dict(_id = "person:id", seq = 11),
-            "account:id" : dict(_id = "account:id", seq = 33)
+            "person:id": dict(_id="person:id", seq=11),
+            "account:id": dict(_id="account:id", seq=33),
         }
         data = json.dumps(structure)
         data = quorum.legacy.bytes(data)
 
         adapter = quorum.get_adapter()
-        manager = quorum.export.ExportManager(
-            adapter,
-            multiple = quorum.resolve()
-        )
+        manager = quorum.export.ExportManager(adapter, multiple=quorum.resolve())
 
         collection = adapter.collection("counter")
-        manager._import_single(collection, data, key = "_id")
+        manager._import_single(collection, data, key="_id")
 
         values = collection.find()
         values = [value for value in values]
 
         self.assertEqual(type(values), list)
         self.assertEqual(len(values), 2)
 
-        value = collection.find_one(dict(_id = "person:id"))
+        value = collection.find_one(dict(_id="person:id"))
 
         self.assertEqual(value["seq"], 11)
 
     @quorum.secured
     def test_import_multiple(self):
         data = [
             (
                 "person:id",
                 quorum.legacy.bytes(
-                    json.dumps(dict(_id = "person:id", seq = 11)),
-                    encoding = "utf-8"
-                )
+                    json.dumps(dict(_id="person:id", seq=11)), encoding="utf-8"
+                ),
             ),
             (
                 "account:id",
                 quorum.legacy.bytes(
-                    json.dumps(dict(_id = "account:id", seq = 33)),
-                    encoding = "utf-8"
-                )
-            )
+                    json.dumps(dict(_id="account:id", seq=33)), encoding="utf-8"
+                ),
+            ),
         ]
 
         adapter = quorum.get_adapter()
-        manager = quorum.export.ExportManager(
-            adapter,
-            multiple = quorum.resolve()
-        )
+        manager = quorum.export.ExportManager(adapter, multiple=quorum.resolve())
 
         collection = adapter.collection("counter")
-        manager._import_multiple(collection, data, key = "_id")
+        manager._import_multiple(collection, data, key="_id")
 
         values = collection.find()
         values = [value for value in values]
 
         self.assertEqual(type(values), list)
         self.assertEqual(len(values), 2)
 
-        value = collection.find_one(dict(_id = "person:id"))
+        value = collection.find_one(dict(_id="person:id"))
 
         self.assertEqual(value["seq"], 11)
```

### Comparing `quorum-0.8.2/src/quorum/test/structures.py` & `quorum-0.8.3/src/quorum/test/structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class OrderedDictTest(quorum.TestCase):
 
     @quorum.secured
     def test_basic(self):
         struct = quorum.OrderedDict()
 
         struct["first"] = 1
@@ -65,15 +57,15 @@
 
         self.assertEqual(next(iterator), ["first", 1])
         self.assertEqual(next(iterator), ["second", 2])
         self.assertEqual(next(iterator), ["third", 3])
 
     @quorum.secured
     def test_build(self):
-        base = dict(first = 1, second = 2, third = 3)
+        base = dict(first=1, second=2, third=3)
 
         struct = quorum.OrderedDict(base)
 
         self.assertEqual(struct._dict, base)
 
         iterator = iter(struct)
 
@@ -176,59 +168,65 @@
         struct.push(["first", 1])
         struct.push(["second", 2])
         struct.push(["third", 3])
 
         self.assertEqual(repr(struct), "[['first', 1], ['second', 2], ['third', 3]]")
         self.assertEqual(str(struct), "[['first', 1], ['second', 2], ['third', 3]]")
 
+
 class LazyDictTest(quorum.TestCase):
 
     @quorum.secured
     def test_lazy(self):
         struct = quorum.LazyDict()
 
         struct["first"] = quorum.LazyValue(lambda: 2)
 
-        self.assertEqual(isinstance(struct.__getitem__("first", True), quorum.LazyValue), True)
+        self.assertEqual(
+            isinstance(struct.__getitem__("first", True), quorum.LazyValue), True
+        )
         self.assertEqual(struct["first"], 2)
 
     @quorum.secured
     def test_resolve(self):
         struct = quorum.LazyDict(
-            first = quorum.LazyValue(lambda: 1),
-            second = quorum.LazyValue(lambda: 2)
+            first=quorum.LazyValue(lambda: 1), second=quorum.LazyValue(lambda: 2)
         )
 
-        resolved = struct.resolve(force = True)
+        resolved = struct.resolve(force=True)
 
         self.assertNotEqual(type(struct) == dict, True)
-        self.assertNotEqual(struct, dict(first = 1, second = 2))
+        self.assertNotEqual(struct, dict(first=1, second=2))
         self.assertEqual(type(resolved) == dict, True)
-        self.assertEqual(resolved, dict(first = 1, second = 2))
+        self.assertEqual(resolved, dict(first=1, second=2))
 
         resolved = struct.to_dict()
 
         self.assertNotEqual(type(struct) == dict, True)
-        self.assertNotEqual(struct, dict(first = 1, second = 2))
+        self.assertNotEqual(struct, dict(first=1, second=2))
         self.assertEqual(type(resolved) == dict, True)
-        self.assertEqual(resolved, dict(first = 1, second = 2))
+        self.assertEqual(resolved, dict(first=1, second=2))
 
     @quorum.secured
     def test_naming(self):
         struct = quorum.lazy_dict()
 
         struct["first"] = quorum.lazy(lambda: 2)
 
-        self.assertEqual(isinstance(struct.__getitem__("first", True), quorum.lazy), True)
+        self.assertEqual(
+            isinstance(struct.__getitem__("first", True), quorum.lazy), True
+        )
         self.assertEqual(struct["first"], 2)
 
     @quorum.secured
     def test_concrete(self):
         struct = quorum.lazy_dict()
 
         struct["first"] = quorum.lazy(lambda: 1)
         struct["second"] = 2
 
-        self.assertEqual(isinstance(struct.__getitem__("first", True), quorum.lazy), True)
+        self.assertEqual(
+            isinstance(struct.__getitem__("first", True), quorum.lazy), True
+        )
         self.assertEqual(struct["first"], 1)
         self.assertEqual(isinstance(struct.__getitem__("second", True), int), True)
         self.assertEqual(struct["second"], 2)
```

### Comparing `quorum-0.8.2/src/quorum/test/log.py` & `quorum-0.8.3/src/quorum/test/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,85 +18,71 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import logging
 
 import quorum
 
+
 class LogTest(quorum.TestCase):
 
     @quorum.secured
     def test_memory_handler(self):
         memory_handler = quorum.MemoryHandler()
         formatter = logging.Formatter("%(message)s")
         memory_handler.setFormatter(formatter)
 
         latest = memory_handler.get_latest()
         self.assertEqual(len(latest), 0)
         self.assertEqual(latest, [])
 
         record = logging.makeLogRecord(
-            dict(
-                msg = "hello world",
-                levelname = logging.getLevelName(logging.INFO)
-            )
+            dict(msg="hello world", levelname=logging.getLevelName(logging.INFO))
         )
         memory_handler.emit(record)
         latest = memory_handler.get_latest()
 
         self.assertEqual(len(latest), 1)
         self.assertEqual(latest, ["hello world"])
 
         record = logging.makeLogRecord(
-            dict(
-                msg = "hello world 2",
-                levelname = logging.getLevelName(logging.ERROR)
-            )
+            dict(msg="hello world 2", levelname=logging.getLevelName(logging.ERROR))
         )
         memory_handler.emit(record)
         latest = memory_handler.get_latest()
 
         self.assertEqual(len(latest), 2)
         self.assertEqual(latest, ["hello world 2", "hello world"])
 
-        latest = memory_handler.get_latest(level = logging.ERROR)
+        latest = memory_handler.get_latest(level=logging.ERROR)
 
         self.assertEqual(len(latest), 1)
         self.assertEqual(latest, ["hello world 2"])
 
-        latest = memory_handler.get_latest(level = logging.CRITICAL)
+        latest = memory_handler.get_latest(level=logging.CRITICAL)
 
         self.assertEqual(len(latest), 0)
         self.assertEqual(latest, [])
 
-        latest = memory_handler.get_latest(level = logging.INFO)
+        latest = memory_handler.get_latest(level=logging.INFO)
 
         self.assertEqual(len(latest), 2)
         self.assertEqual(latest, ["hello world 2", "hello world"])
 
-        latest = memory_handler.get_latest(count = 1, level = logging.INFO)
+        latest = memory_handler.get_latest(count=1, level=logging.INFO)
 
         self.assertEqual(len(latest), 1)
         self.assertEqual(latest, ["hello world 2"])
 
     @quorum.secured
     def test_memory_handler_file(self):
         memory_handler = quorum.MemoryHandler()
@@ -104,41 +90,35 @@
         memory_handler.setFormatter(formatter)
 
         latest = memory_handler.get_latest()
         self.assertEqual(len(latest), 0)
         self.assertEqual(latest, [])
 
         record = logging.makeLogRecord(
-            dict(
-                msg = "hello world",
-                levelname = logging.getLevelName(logging.INFO)
-            )
+            dict(msg="hello world", levelname=logging.getLevelName(logging.INFO))
         )
         memory_handler.emit(record)
         record = logging.makeLogRecord(
-            dict(
-                msg = "hello world 2",
-                levelname = logging.getLevelName(logging.INFO)
-            )
+            dict(msg="hello world 2", levelname=logging.getLevelName(logging.INFO))
         )
         memory_handler.emit(record)
 
         file = quorum.legacy.BytesIO()
 
-        memory_handler.flush_to_file(file, clear = False)
+        memory_handler.flush_to_file(file, clear=False)
 
         file.seek(0)
         contents = file.read()
 
         self.assertEqual(contents, b"hello world\nhello world 2\n")
 
         file = quorum.legacy.BytesIO()
 
-        memory_handler.flush_to_file(file, reverse = False)
+        memory_handler.flush_to_file(file, reverse=False)
 
         file.seek(0)
         contents = file.read()
 
         self.assertEqual(contents, b"hello world 2\nhello world\n")
 
-        latest = memory_handler.get_latest(count = 1)
+        latest = memory_handler.get_latest(count=1)
         self.assertEqual(len(latest), 0)
```

### Comparing `quorum-0.8.2/src/quorum/test/data.py` & `quorum-0.8.3/src/quorum/test/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,31 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class DataTest(quorum.TestCase):
 
     @quorum.secured
     def test_id(self):
         adapter = quorum.DataAdapter()
         identifier = adapter._id()
```

### Comparing `quorum-0.8.2/src/quorum/test/base.py` & `quorum-0.8.3/src/quorum/test/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,99 +18,91 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class BaseTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(name = __name__)
+            quorum.load(name=__name__)
         except Exception:
             self.skip()
 
     def tearDown(self):
         quorum.unload()
 
     @quorum.secured
     def test_locale(self):
         app = quorum.get_app()
         app.locales = ("en_us", "pt_pt", "es_es")
-        app.bundles["en_us"] = dict(hello = "Hello")
-        app.bundles["pt_pt"] = dict(hello = "Olá")
-        app.bundles["fr"] = dict(hello = "Bonjour")
+        app.bundles["en_us"] = dict(hello="Hello")
+        app.bundles["pt_pt"] = dict(hello="Olá")
+        app.bundles["fr"] = dict(hello="Bonjour")
 
-        result = quorum.to_locale("hello", locale = "en-us")
+        result = quorum.to_locale("hello", locale="en-us")
         self.assertEqual(result, "Hello")
 
-        result = quorum.to_locale("hello", locale = "pt_pt")
+        result = quorum.to_locale("hello", locale="pt_pt")
         self.assertEqual(result, "Olá")
 
-        result = quorum.to_locale("hello", locale = "pt-pt")
+        result = quorum.to_locale("hello", locale="pt-pt")
         self.assertNotEqual(result, "Olá")
         self.assertEqual(result, "Hello")
 
-        result = quorum.to_locale("hello", locale = "fr_fr")
+        result = quorum.to_locale("hello", locale="fr_fr")
         self.assertEqual(result, "Bonjour")
 
-        result = quorum.to_locale("hello", locale = "fr")
+        result = quorum.to_locale("hello", locale="fr")
         self.assertEqual(result, "Bonjour")
 
-        result = quorum.to_locale("hello", locale = "es_es")
+        result = quorum.to_locale("hello", locale="es_es")
         self.assertNotEqual(result, "Hola")
         self.assertEqual(result, "Hello")
 
-        app.bundles["es_es"] = dict(hello = "Hola")
+        app.bundles["es_es"] = dict(hello="Hola")
 
-        result = quorum.to_locale("hello", locale = "es_es")
+        result = quorum.to_locale("hello", locale="es_es")
         self.assertEqual(result, "Hola")
 
-        result = quorum.to_locale("hello", locale = "en")
+        result = quorum.to_locale("hello", locale="en")
         self.assertEqual(result, "Hello")
 
-        result = quorum.to_locale("hello", locale = "pt")
+        result = quorum.to_locale("hello", locale="pt")
         self.assertEqual(result, "Olá")
 
-        result = quorum.to_locale("hello", locale = "es")
+        result = quorum.to_locale("hello", locale="es")
         self.assertEqual(result, "Hola")
 
-        result = quorum.to_locale("bye", locale = "en_us")
+        result = quorum.to_locale("bye", locale="en_us")
         self.assertEqual(result, "bye")
 
-        result = quorum.to_locale("bye", locale = "cn")
+        result = quorum.to_locale("bye", locale="cn")
         self.assertEqual(result, "bye")
 
-        app.bundles["en_us"].update(bye = "Bye")
+        app.bundles["en_us"].update(bye="Bye")
 
-        result = quorum.to_locale("bye", locale = "en_us")
+        result = quorum.to_locale("bye", locale="en_us")
         self.assertEqual(result, "Bye")
 
-        result = quorum.to_locale("bye", locale = "pt_pt")
+        result = quorum.to_locale("bye", locale="pt_pt")
         self.assertEqual(result, "Bye")
 
-        result = quorum.to_locale("bye", locale = "pt_pt", fallback = False)
+        result = quorum.to_locale("bye", locale="pt_pt", fallback=False)
         self.assertEqual(result, "bye")
 
     @quorum.secured
     def test_context(self):
 
         def without_context():
             return quorum.has_context()
```

### Comparing `quorum-0.8.2/src/quorum/test/validation.py` & `quorum-0.8.3/src/quorum/test/validation.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,425 +18,331 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import datetime
 
 import quorum
 
+
 class ValidationTest(quorum.TestCase):
 
     @quorum.secured
     def test_eq_number(self):
         methods = [quorum.eq("age", 2)]
 
-        object = dict(age = 2)
+        object = dict(age=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2.0)
+        object = dict(age=2.0)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 3)
+        object = dict(age=3)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = "2")
+        object = dict(age="2")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = 2.01)
+        object = dict(age=2.01)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_eq_string(self):
         methods = [quorum.eq("name", "John Doe")]
 
-        object = dict(name = "John Doe")
+        object = dict(name="John Doe")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = "john doe")
+        object = dict(name="john doe")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(name = "JohnDoe")
+        object = dict(name="JohnDoe")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(name = 2)
+        object = dict(name=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(name = 2.0)
+        object = dict(name=2.0)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(name = True)
+        object = dict(name=True)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_gt(self):
         methods = [quorum.gt("age", 2)]
 
-        object = dict(age = 3)
+        object = dict(age=3)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2.01)
+        object = dict(age=2.01)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2)
+        object = dict(age=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = "2")
+        object = dict(age="2")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
-        if quorum.legacy.PYTHON_3: self.assertFalse(result)
-        else: self.assertTrue(result)
+        if quorum.legacy.PYTHON_3:
+            self.assertFalse(result)
+        else:
+            self.assertTrue(result)
 
-        object = dict(age = 1.99)
+        object = dict(age=1.99)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_gte(self):
         methods = [quorum.gte("age", 2)]
 
-        object = dict(age = 3)
+        object = dict(age=3)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2)
+        object = dict(age=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2.01)
+        object = dict(age=2.01)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2.00)
+        object = dict(age=2.00)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = "2")
+        object = dict(age="2")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
-        if quorum.legacy.PYTHON_3: self.assertFalse(result)
-        else: self.assertTrue(result)
+        if quorum.legacy.PYTHON_3:
+            self.assertFalse(result)
+        else:
+            self.assertTrue(result)
 
-        object = dict(age = 1.99)
+        object = dict(age=1.99)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_lt(self):
         methods = [quorum.lt("age", 2)]
 
-        object = dict(age = 1)
+        object = dict(age=1)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 1.99)
+        object = dict(age=1.99)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2)
+        object = dict(age=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = "2")
+        object = dict(age="2")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = 2.01)
+        object = dict(age=2.01)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_lte(self):
         methods = [quorum.lte("age", 2)]
 
-        object = dict(age = 1)
+        object = dict(age=1)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2)
+        object = dict(age=2)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 1.99)
+        object = dict(age=1.99)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = 2.00)
+        object = dict(age=2.00)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(age = "2")
+        object = dict(age="2")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(age = 2.01)
+        object = dict(age=2.01)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_not_null(self):
         methods = [quorum.not_null("name")]
 
-        object = dict(name = "John Doe")
+        object = dict(name="John Doe")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = 1)
+        object = dict(name=1)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = 1.0)
+        object = dict(name=1.0)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = False)
+        object = dict(name=False)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = "")
+        object = dict(name="")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = None)
+        object = dict(name=None)
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_not_empty(self):
         methods = [quorum.not_empty("name")]
 
-        object = dict(name = "John Doe")
+        object = dict(name="John Doe")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = [1, 2, 3])
+        object = dict(name=[1, 2, 3])
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(name = "")
+        object = dict(name="")
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
-        object = dict(name = [])
+        object = dict(name=[])
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
 
     @quorum.secured
     def test_not_past(self):
         methods = [quorum.not_past("time")]
 
-        object = dict(time = datetime.datetime(2200, 1, 1))
+        object = dict(time=datetime.datetime(2200, 1, 1))
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertTrue(result)
 
-        object = dict(time = datetime.datetime(2001, 1, 1))
+        object = dict(time=datetime.datetime(2001, 1, 1))
         result = quorum.validation.validate_b(
-            methods = methods,
-            object = object,
-            build = False
+            methods=methods, object=object, build=False
         )
         self.assertFalse(result)
```

### Comparing `quorum-0.8.2/src/quorum/test/util.py` & `quorum-0.8.3/src/quorum/test/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,38 +18,30 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import string
 
 import quorum
 
+
 class UtilTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(name = __name__)
+            quorum.load(name=__name__)
         except Exception:
             self.skip()
 
     def tearDown(self):
         quorum.unload()
 
     @quorum.secured
@@ -61,245 +53,355 @@
         self.assertEqual(result, [("name", 1)])
 
         result = quorum.to_sort("name:ascending,age:descending")
         self.assertEqual(result, [("name", 1), ("age", -1)])
 
     @quorum.secured
     def test_is_mobile(self):
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_mobile(user_agent = "Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1")
+        result = quorum.is_mobile(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_mobile(user_agent = "")
+        result = quorum.is_mobile(user_agent="")
         self.assertEqual(result, False)
 
     @quorum.secured
     def test_is_tablet(self):
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_tablet(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36")
+        result = quorum.is_tablet(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_tablet(user_agent = "")
+        result = quorum.is_tablet(user_agent="")
         self.assertEqual(result, False)
 
     @quorum.secured
     def test_is_browser(self):
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136")
+        result = quorum.is_browser(
+            user_agent="Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_browser(user_agent = "DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)")
+        result = quorum.is_browser(
+            user_agent="DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_browser(user_agent = "netius/1.1.10")
+        result = quorum.is_browser(user_agent="netius/1.1.10")
         self.assertEqual(result, False)
 
-        result = quorum.is_browser(user_agent = "netius/1.1b")
+        result = quorum.is_browser(user_agent="netius/1.1b")
         self.assertEqual(result, False)
 
-        result = quorum.is_browser(user_agent = "")
+        result = quorum.is_browser(user_agent="")
         self.assertEqual(result, False)
 
     @quorum.secured
     def test_is_bot(self):
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 6_1_3 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Mobile/10B329"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (Linux; Android 4.0.4; Galaxy Nexus Build/IMM76B) AppleWebKit/535.19 (KHTML, like Gecko) Chrome/18.0.1025.133 Mobile Safari/535.19"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (Linux; U; Android 4.1.1; en-gb; Build/KLP) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Safari/534.30"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_4) AppleWebKit/600.7.12 (KHTML, like Gecko) Version/8.0.7 Safari/600.7.12"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136")
+        result = quorum.is_bot(
+            user_agent="Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136"
+        )
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)")
+        result = quorum.is_bot(
+            user_agent="DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)"
+        )
         self.assertEqual(result, True)
 
-        result = quorum.is_bot(user_agent = "netius/1.1.10")
+        result = quorum.is_bot(user_agent="netius/1.1.10")
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "netius/1.1b")
+        result = quorum.is_bot(user_agent="netius/1.1b")
         self.assertEqual(result, False)
 
-        result = quorum.is_bot(user_agent = "")
+        result = quorum.is_bot(user_agent="")
         self.assertEqual(result, False)
 
     @quorum.secured
     def test_browser_info(self):
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136")
-        self.assertEqual(result, dict(
-            name = "Edge",
-            version = "12.10136",
-            version_f = 12.10136,
-            version_i = 12,
-            interactive = True,
-            bot = False,
-            os = "Windows"
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36")
-        self.assertEqual(result, dict(
-            name = "Chrome",
-            version = "62.0.3202.75",
-            version_f = 62.0,
-            version_i = 62,
-            interactive = True,
-            bot = False,
-            os = "Windows"
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1")
-        self.assertEqual(result, dict(
-            name = "Safari",
-            version = "601.1",
-            version_f = 601.1,
-            version_i = 601,
-            interactive = True,
-            bot = False,
-            os = "Mac"
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:56.0) Gecko/20100101 Firefox/56.0")
-        self.assertEqual(result, dict(
-            name = "Firefox",
-            version = "56.0",
-            version_f = 56.0,
-            version_i = 56,
-            interactive = True,
-            bot = False,
-            os = "Windows"
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0)")
-        self.assertEqual(result, dict(
-            name = "Explorer",
-            version = "8.0",
-            version_f = 8.0,
-            version_i = 8,
-            interactive = True,
-            bot = False,
-            os = "Windows"
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)")
-        self.assertEqual(result, dict(
-            name = "Googlebot",
-            version = "2.1",
-            version_f = 2.1,
-            version_i = 2,
-            interactive = False,
-            bot = True
-        ))
-
-        result = quorum.browser_info(user_agent = "Mozilla/5.0 (compatible; Bingbot/2.0; +http://www.bing.com/bingbot.htm)")
-        self.assertEqual(result, dict(
-            name = "Bingbot",
-            version = "2.0",
-            version_f = 2.0,
-            version_i = 2,
-            interactive = False,
-            bot = True
-        ))
-
-        result = quorum.browser_info(user_agent = "DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)")
-        self.assertEqual(result, dict(
-            name = "DuckDuckBot",
-            version = "1.0",
-            version_f = 1.0,
-            version_i = 1,
-            interactive = False,
-            bot = True
-        ))
-
-        result = quorum.browser_info(user_agent = "netius/1.1.10")
-        self.assertEqual(result, dict(
-            name = "netius",
-            version = "1.1.10",
-            version_f = 1.1,
-            version_i = 1,
-            interactive = False,
-            bot = False
-        ))
-
-        result = quorum.browser_info(user_agent = "netius/1.1b")
-        self.assertEqual(result, dict(
-            name = "netius",
-            version = "1.1b",
-            version_f = 0,
-            version_i = 0,
-            interactive = False,
-            bot = False
-        ))
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10136"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Edge",
+                version="12.10136",
+                version_f=12.10136,
+                version_i=12,
+                interactive=True,
+                bot=False,
+                os="Windows",
+            ),
+        )
 
-        result = quorum.browser_info(user_agent = "APIs-Google (+https://developers.google.com/webmasters/APIs-Google.html)")
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/62.0.3202.75 Safari/537.36"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Chrome",
+                version="62.0.3202.75",
+                version_f=62.0,
+                version_i=62,
+                interactive=True,
+                bot=False,
+                os="Windows",
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (iPad; CPU OS 9_3_2 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13F69 Safari/601.1"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Safari",
+                version="601.1",
+                version_f=601.1,
+                version_i=601,
+                interactive=True,
+                bot=False,
+                os="Mac",
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:56.0) Gecko/20100101 Firefox/56.0"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Firefox",
+                version="56.0",
+                version_f=56.0,
+                version_i=56,
+                interactive=True,
+                bot=False,
+                os="Windows",
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.0; Trident/4.0)"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Explorer",
+                version="8.0",
+                version_f=8.0,
+                version_i=8,
+                interactive=True,
+                bot=False,
+                os="Windows",
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Googlebot",
+                version="2.1",
+                version_f=2.1,
+                version_i=2,
+                interactive=False,
+                bot=True,
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="Mozilla/5.0 (compatible; Bingbot/2.0; +http://www.bing.com/bingbot.htm)"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="Bingbot",
+                version="2.0",
+                version_f=2.0,
+                version_i=2,
+                interactive=False,
+                bot=True,
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)"
+        )
+        self.assertEqual(
+            result,
+            dict(
+                name="DuckDuckBot",
+                version="1.0",
+                version_f=1.0,
+                version_i=1,
+                interactive=False,
+                bot=True,
+            ),
+        )
+
+        result = quorum.browser_info(user_agent="netius/1.1.10")
+        self.assertEqual(
+            result,
+            dict(
+                name="netius",
+                version="1.1.10",
+                version_f=1.1,
+                version_i=1,
+                interactive=False,
+                bot=False,
+            ),
+        )
+
+        result = quorum.browser_info(user_agent="netius/1.1b")
+        self.assertEqual(
+            result,
+            dict(
+                name="netius",
+                version="1.1b",
+                version_f=0,
+                version_i=0,
+                interactive=False,
+                bot=False,
+            ),
+        )
+
+        result = quorum.browser_info(
+            user_agent="APIs-Google (+https://developers.google.com/webmasters/APIs-Google.html)"
+        )
         self.assertEqual(result, None)
 
     @quorum.secured
     def test_camel_to_underscore(self):
         result = quorum.camel_to_underscore(None)
         self.assertEqual(result, None)
 
@@ -328,53 +430,44 @@
         self.assertEqual(type(result), str)
         self.assertEqual(result, "")
 
         result = quorum.camel_to_readable("HelloWorld")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
-        result = quorum.camel_to_readable("HelloWorld", lower = True)
+        result = quorum.camel_to_readable("HelloWorld", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.camel_to_readable("HelloWorld", lower = True, capitalize = True)
+        result = quorum.camel_to_readable("HelloWorld", lower=True, capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
         result = quorum.camel_to_readable("HELLOWorld")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HELLO World")
 
-        result = quorum.camel_to_readable("HELLOWorld", lower = True)
+        result = quorum.camel_to_readable("HELLOWorld", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.camel_to_readable(
-            "HELLOWorld",
-            lower = True,
-            capitalize = True
-        )
+        result = quorum.camel_to_readable("HELLOWorld", lower=True, capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
         result = quorum.camel_to_readable("HELLOWorldHELLOWorld")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HELLO World HELLO World")
 
-        result = quorum.camel_to_readable(
-            "HELLOWorldHELLOWorld",
-            lower = True
-        )
+        result = quorum.camel_to_readable("HELLOWorldHELLOWorld", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world hello world")
 
         result = quorum.camel_to_readable(
-            "HELLOWorldHELLOWorld",
-            lower = True,
-            capitalize = True
+            "HELLOWorldHELLOWorld", lower=True, capitalize=True
         )
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World Hello World")
 
     @quorum.secured
     def test_underscore_to_camel(self):
         result = quorum.underscore_to_camel(None)
@@ -384,63 +477,63 @@
         self.assertEqual(type(result), str)
         self.assertEqual(result, "")
 
         result = quorum.underscore_to_camel("hello_world")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorld")
 
-        result = quorum.underscore_to_camel("hello_world", lower = True)
+        result = quorum.underscore_to_camel("hello_world", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorld")
 
         result = quorum.underscore_to_camel("hello_world_hello_world")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorldHelloWorld")
 
-        result = quorum.underscore_to_camel("hello_world_hello_world", lower = True)
+        result = quorum.underscore_to_camel("hello_world_hello_world", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorldHelloWorld")
 
         result = quorum.underscore_to_camel("hello_world_")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorld")
 
-        result = quorum.underscore_to_camel("hello_world_", lower = True)
+        result = quorum.underscore_to_camel("hello_world_", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorld")
 
         result = quorum.underscore_to_camel("__hello_world__")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorld")
 
-        result = quorum.underscore_to_camel("__hello_world__", lower = True)
+        result = quorum.underscore_to_camel("__hello_world__", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorld")
 
         result = quorum.underscore_to_camel("__hello___world__")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorld")
 
-        result = quorum.underscore_to_camel("__hello___world__", lower = True)
+        result = quorum.underscore_to_camel("__hello___world__", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorld")
 
         result = quorum.underscore_to_camel("__hello___WORLD__")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWORLD")
 
-        result = quorum.underscore_to_camel("__hello___WORLD__", lower = True)
+        result = quorum.underscore_to_camel("__hello___WORLD__", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWORLD")
 
         result = quorum.underscore_to_camel("HelloWorld")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "HelloWorld")
 
-        result = quorum.underscore_to_camel("HelloWorld", lower = True)
+        result = quorum.underscore_to_camel("HelloWorld", lower=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "helloWorld")
 
     @quorum.secured
     def test_underscore_to_readable(self):
         result = quorum.underscore_to_readable(None)
         self.assertEqual(result, None)
@@ -449,81 +542,82 @@
         self.assertEqual(type(result), str)
         self.assertEqual(result, "")
 
         result = quorum.underscore_to_readable("hello_world")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.underscore_to_readable("hello_world", capitalize = True)
+        result = quorum.underscore_to_readable("hello_world", capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
         result = quorum.underscore_to_readable("hello_world_hello_world")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world hello world")
 
-        result = quorum.underscore_to_readable("hello_world_hello_world", capitalize = True)
+        result = quorum.underscore_to_readable(
+            "hello_world_hello_world", capitalize=True
+        )
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World Hello World")
 
         result = quorum.underscore_to_readable("hello_world_")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.underscore_to_readable("hello_world_", capitalize = True)
+        result = quorum.underscore_to_readable("hello_world_", capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
         result = quorum.underscore_to_readable("__hello_world__")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.underscore_to_readable("__hello_world__", capitalize = True)
+        result = quorum.underscore_to_readable("__hello_world__", capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
         result = quorum.underscore_to_readable("__hello___world__")
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello world")
 
-        result = quorum.underscore_to_readable("__hello___world__", capitalize = True)
+        result = quorum.underscore_to_readable("__hello___world__", capitalize=True)
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello World")
 
-        result = quorum.underscore_to_readable("__hello___world__", capitalize = True, separator = "-")
+        result = quorum.underscore_to_readable(
+            "__hello___world__", capitalize=True, separator="-"
+        )
         self.assertEqual(type(result), str)
         self.assertEqual(result, "Hello-World")
 
     @quorum.secured
     def test_generate_identifier(self):
-        identifier = quorum.generate_identifier(
-            size = 16,
-            chars = string.ascii_uppercase
-        )
+        identifier = quorum.generate_identifier(size=16, chars=string.ascii_uppercase)
         self.assertEqual(len(identifier), 16)
         for char in identifier:
             self.assertTrue(char in string.ascii_uppercase)
 
     @quorum.secured
     def test_escape(self):
-        result = quorum.escape("foo,bar", ",", escape = "$")
+        result = quorum.escape("foo,bar", ",", escape="$")
         self.assertEqual(result, "foo$,bar")
 
-        result = quorum.escape("foo$,bar", ",", escape = "$")
+        result = quorum.escape("foo$,bar", ",", escape="$")
         self.assertEqual(result, "foo$$$,bar")
 
     @quorum.secured
     def test_unescape(self):
-        result = quorum.unescape("foo$,bar", escape = "$")
+        result = quorum.unescape("foo$,bar", escape="$")
         self.assertEqual(result, "foo,bar")
 
-        result = quorum.unescape("foo$$,bar", escape = "$")
+        result = quorum.unescape("foo$$,bar", escape="$")
         self.assertEqual(result, "foo$,bar")
 
-        result = quorum.unescape("$$foo$,bar$$$$", escape = "$")
+        result = quorum.unescape("$$foo$,bar$$$$", escape="$")
         self.assertEqual(result, "$foo,bar$$")
 
     @quorum.secured
     def test_count_unescape(self):
         result = quorum.count_unescape("foo:bar", ":")
         self.assertEqual(result, 1)
 
@@ -546,36 +640,36 @@
         self.assertEqual(result, 0)
 
     @quorum.secured
     def test_split_unescape(self):
         result = quorum.split_unescape("foo bar")
         self.assertEqual(result, ["foo", "bar"])
 
-        result = quorum.split_unescape("foo bar hello world", max = 2)
+        result = quorum.split_unescape("foo bar hello world", max=2)
         self.assertEqual(result, ["foo", "bar", "hello world"])
 
         result = quorum.split_unescape("foo,bar", ",")
         self.assertEqual(result, ["foo", "bar"])
 
-        result = quorum.split_unescape("foo$,bar", ",", escape = "$")
+        result = quorum.split_unescape("foo$,bar", ",", escape="$")
         self.assertEqual(result, ["foo,bar"])
 
-        result = quorum.split_unescape("foo$$,bar", ",", escape = "$", unescape = True)
+        result = quorum.split_unescape("foo$$,bar", ",", escape="$", unescape=True)
         self.assertEqual(result, ["foo$", "bar"])
 
-        result = quorum.split_unescape("foo$$,bar", ",", escape = "$", unescape = False)
+        result = quorum.split_unescape("foo$$,bar", ",", escape="$", unescape=False)
         self.assertEqual(result, ["foo$$", "bar"])
 
-        result = quorum.split_unescape("foo$", ",", escape = "$", unescape = True)
+        result = quorum.split_unescape("foo$", ",", escape="$", unescape=True)
         self.assertEqual(result, ["foo$"])
 
-        result = quorum.split_unescape("foo\\\\\\:bar", ":", unescape = True)
+        result = quorum.split_unescape("foo\\\\\\:bar", ":", unescape=True)
         self.assertEqual(result, ["foo\\:bar"])
 
-        result = quorum.split_unescape("foo\\\\:bar", ":", unescape = True)
+        result = quorum.split_unescape("foo\\\\:bar", ":", unescape=True)
         self.assertEqual(result, ["foo\\", "bar"])
 
     @quorum.secured
     def test_is_content_type(self):
         result = quorum.is_content_type("text/plain", "text/plain")
         self.assertEqual(result, True)
 
@@ -611,27 +705,29 @@
         self.assertEqual(result[0], ["text/plain", "text/json"])
         self.assertEqual(result[1], dict())
 
         result = quorum.parse_content_type("text/plain+json; charset=utf-8")
         self.assertEqual(type(result), tuple)
         self.assertEqual(len(result), 2)
         self.assertEqual(result[0], ["text/plain", "text/json"])
-        self.assertEqual(result[1], dict(charset = "utf-8"))
+        self.assertEqual(result[1], dict(charset="utf-8"))
 
         result = quorum.parse_content_type("text/plain+json   ; charset=utf-8")
         self.assertEqual(type(result), tuple)
         self.assertEqual(len(result), 2)
         self.assertEqual(result[0], ["text/plain", "text/json"])
-        self.assertEqual(result[1], dict(charset = "utf-8"))
+        self.assertEqual(result[1], dict(charset="utf-8"))
 
-        result = quorum.parse_content_type("text/plain+json; charset=utf-8; boundary=hello;")
+        result = quorum.parse_content_type(
+            "text/plain+json; charset=utf-8; boundary=hello;"
+        )
         self.assertEqual(type(result), tuple)
         self.assertEqual(len(result), 2)
         self.assertEqual(result[0], ["text/plain", "text/json"])
-        self.assertEqual(result[1], dict(charset = "utf-8", boundary = "hello"))
+        self.assertEqual(result[1], dict(charset="utf-8", boundary="hello"))
 
         result = quorum.parse_content_type("")
         self.assertEqual(type(result), tuple)
         self.assertEqual(len(result), 2)
         self.assertEqual(result[0], [])
         self.assertEqual(result[1], dict())
 
@@ -655,45 +751,45 @@
         result = quorum.verify("hello" == "hello")
         self.assertEqual(result, None)
 
         self.assertRaises(quorum.AssertionError, lambda: quorum.verify(1 == 2))
 
         self.assertRaises(
             quorum.OperationalError,
-            lambda: quorum.verify(1 == 2, exception = quorum.OperationalError)
+            lambda: quorum.verify(1 == 2, exception=quorum.OperationalError),
         )
 
     @quorum.secured
     def test_verify_equal(self):
         result = quorum.verify_equal(1, 1)
         self.assertEqual(result, None)
 
         result = quorum.verify_equal("hello", "hello")
         self.assertEqual(result, None)
 
         self.assertRaises(quorum.AssertionError, lambda: quorum.verify_equal(1, 2))
 
         self.assertRaises(
             quorum.OperationalError,
-            lambda: quorum.verify_equal(1, 2, exception = quorum.OperationalError)
+            lambda: quorum.verify_equal(1, 2, exception=quorum.OperationalError),
         )
 
     @quorum.secured
     def test_verify_not_equal(self):
         result = quorum.verify_not_equal(1, 2)
         self.assertEqual(result, None)
 
         result = quorum.verify_not_equal("hello", "world")
         self.assertEqual(result, None)
 
         self.assertRaises(quorum.AssertionError, lambda: quorum.verify_not_equal(1, 1))
 
         self.assertRaises(
             quorum.OperationalError,
-            lambda: quorum.verify_not_equal(1, 1, exception = quorum.OperationalError)
+            lambda: quorum.verify_not_equal(1, 1, exception=quorum.OperationalError),
         )
 
     @quorum.secured
     def test_verify_type(self):
         result = quorum.verify_type("hello", str)
         self.assertEqual(result, None)
 
@@ -703,36 +799,41 @@
         result = quorum.verify_type(None, int)
         self.assertEqual(result, None)
 
         self.assertRaises(quorum.AssertionError, lambda: quorum.verify_type(1, str))
 
         self.assertRaises(
             quorum.OperationalError,
-            lambda: quorum.verify_type(1, str, exception = quorum.OperationalError)
+            lambda: quorum.verify_type(1, str, exception=quorum.OperationalError),
         )
 
-        self.assertRaises(quorum.AssertionError, lambda: quorum.verify_type(None, str, null = False))
+        self.assertRaises(
+            quorum.AssertionError, lambda: quorum.verify_type(None, str, null=False)
+        )
 
         self.assertRaises(
             quorum.OperationalError,
-            lambda: quorum.verify_type(None, str, null = False, exception = quorum.OperationalError)
+            lambda: quorum.verify_type(
+                None, str, null=False, exception=quorum.OperationalError
+            ),
         )
 
     @quorum.secured
     def test_verify_many(self):
         result = quorum.verify_many((1 == 1, 2 == 2, 3 == 3))
         self.assertEqual(result, None)
 
         result = quorum.verify_many(("hello" == "hello",))
         self.assertEqual(result, None)
 
         self.assertRaises(quorum.AssertionError, lambda: quorum.verify_many((1 == 2,)))
 
-        self.assertRaises(quorum.AssertionError, lambda: quorum.verify_many((1 == 1, 1 == 2)))
+        self.assertRaises(
+            quorum.AssertionError, lambda: quorum.verify_many((1 == 1, 1 == 2))
+        )
 
         self.assertRaises(
             quorum.OperationalError,
             lambda: quorum.verify_many(
-                (1 == 1, 1 == 2),
-                exception = quorum.OperationalError
-            )
+                (1 == 1, 1 == 2), exception=quorum.OperationalError
+            ),
         )
```

### Comparing `quorum-0.8.2/src/quorum/test/config.py` & `quorum-0.8.3/src/quorum/test/mail.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,72 +18,46 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-import quorum
+import quorum.mail
 
-class ConfigTest(quorum.TestCase):
 
-    @quorum.secured
-    def test_basic(self):
-        quorum.confs("NAME", "name")
-        result = quorum.conf("NAME")
+class MailTest(quorum.TestCase):
 
-        self.assertEqual(result, "name")
+    def setUp(self):
+        try:
+            quorum.load(name=__name__)
+        except Exception:
+            self.skip()
 
-        result = quorum.conf("NAME", cast = str)
+    def tearDown(self):
+        quorum.unload()
 
-        self.assertEqual(result, "name")
+    @quorum.secured
+    def test_format(self):
+        result = quorum.mail._format("João Magalhães <joamag@hive.pt>")
         self.assertEqual(type(result), str)
+        self.assertEqual(
+            result, "=?utf-8?q?Jo=C3=A3o_Magalh=C3=A3es?= <joamag@hive.pt>"
+        )
 
-        result = quorum.conf("NAME", cast = "str")
-
-        self.assertEqual(result, "name")
+        result = quorum.mail._format("João Magalhães <joamag@hive.pt>")
         self.assertEqual(type(result), str)
+        self.assertEqual(
+            result, "=?utf-8?q?Jo=C3=A3o_Magalh=C3=A3es?= <joamag@hive.pt>"
+        )
 
-        quorum.confs("AGE", "10")
-        result = quorum.conf("AGE", cast = int)
-
-        self.assertEqual(result, 10)
-        self.assertEqual(type(result), int)
-
-        result = quorum.conf("AGE", cast = "int")
-
-        self.assertEqual(result, 10)
-        self.assertEqual(type(result), int)
-
-        result = quorum.conf("AGE", cast = str)
-
-        self.assertEqual(result, "10")
+        result = quorum.mail._format("若昂·马加良斯 <joamag@hive.pt>")
         self.assertEqual(type(result), str)
-
-        result = quorum.conf("HEIGHT")
-
-        self.assertEqual(result, None)
-
-    def test_none(self):
-        quorum.confs("AGE", None)
-        result = quorum.conf("AGE", cast = int)
-
-        self.assertEqual(result, None)
-
-        result = quorum.conf("HEIGHT", cast = int)
-
-        self.assertEqual(result, None)
+        self.assertEqual(
+            result, "=?utf-8?b?6Iul5piCwrfpqazliqDoia/mlq8=?= <joamag@hive.pt>"
+        )
```

### Comparing `quorum-0.8.2/src/quorum/test/httpc.py` & `quorum-0.8.3/src/quorum/test/httpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,25 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import threading
 
 import quorum
 
+
 class HTTPCTest(quorum.TestCase):
 
     def setUp(self):
         quorum.TestCase.setUp(self)
         self.httpbin = quorum.conf("HTTPBIN", "httpbin.org")
 
     @quorum.secured
@@ -59,94 +51,99 @@
 
         self.assertEqual(result_single, "Basic dXNlcm5hbWU6dXNlcm5hbWU=")
         self.assertEqual(quorum.legacy.is_string(result), True)
         self.assertEqual(result_single, result_multiple)
 
     @quorum.secured
     def test__parse_url(self):
-        url, scheme, host, authorization, params = quorum.httpc._parse_url("http://hive.pt/")
+        url, scheme, host, authorization, params = quorum.httpc._parse_url(
+            "http://hive.pt/"
+        )
 
         self.assertEqual(url, "http://hive.pt:80/")
         self.assertEqual(scheme, "http")
         self.assertEqual(host, "hive.pt")
         self.assertEqual(authorization, None)
         self.assertEqual(params, {})
 
-        url, scheme, host, authorization, params = quorum.httpc._parse_url("http://username@hive.pt/")
+        url, scheme, host, authorization, params = quorum.httpc._parse_url(
+            "http://username@hive.pt/"
+        )
 
         self.assertEqual(url, "http://hive.pt:80/")
         self.assertEqual(scheme, "http")
         self.assertEqual(host, "hive.pt")
         self.assertEqual(authorization, None)
         self.assertEqual(params, {})
 
-        url, scheme, host, authorization, params = quorum.httpc._parse_url("http://username:password@hive.pt/")
+        url, scheme, host, authorization, params = quorum.httpc._parse_url(
+            "http://username:password@hive.pt/"
+        )
 
         self.assertEqual(url, "http://hive.pt:80/")
         self.assertEqual(scheme, "http")
         self.assertEqual(host, "hive.pt")
         self.assertEqual(authorization, "dXNlcm5hbWU6cGFzc3dvcmQ=")
         self.assertEqual(params, {})
 
-        url, scheme, host, authorization, params = quorum.httpc._parse_url("http://username:password@hive.pt/hello/world")
+        url, scheme, host, authorization, params = quorum.httpc._parse_url(
+            "http://username:password@hive.pt/hello/world"
+        )
 
         self.assertEqual(url, "http://hive.pt:80/hello/world")
         self.assertEqual(scheme, "http")
         self.assertEqual(host, "hive.pt")
         self.assertEqual(authorization, "dXNlcm5hbWU6cGFzc3dvcmQ=")
         self.assertEqual(params, {})
 
-        url, scheme, host, authorization, params = quorum.httpc._parse_url("http://username:password@hive.pt/hello/world?hello=world")
+        url, scheme, host, authorization, params = quorum.httpc._parse_url(
+            "http://username:password@hive.pt/hello/world?hello=world"
+        )
 
         self.assertEqual(url, "http://hive.pt:80/hello/world")
         self.assertEqual(scheme, "http")
         self.assertEqual(host, "hive.pt")
         self.assertEqual(authorization, "dXNlcm5hbWU6cGFzc3dvcmQ=")
-        self.assertEqual(params, dict(hello = ["world"]))
+        self.assertEqual(params, dict(hello=["world"]))
 
     @quorum.secured
     def test_redirect(self):
         quoted = quorum.legacy.quote("https://%s/" % self.httpbin)
         _data, response = quorum.get_json(
             "https://%s/redirect-to?url=%s" % (self.httpbin, quoted),
-            handle = True,
-            redirect = True
+            handle=True,
+            redirect=True,
         )
 
         code = response.getcode()
         self.assertNotEqual(code, 302)
         self.assertEqual(code, 200)
 
         _data, response = quorum.get_json(
-            "https://%s/relative-redirect/2" % self.httpbin,
-            handle = True,
-            redirect = True
+            "https://%s/relative-redirect/2" % self.httpbin, handle=True, redirect=True
         )
 
         code = response.getcode()
         self.assertNotEqual(code, 302)
         self.assertEqual(code, 200)
 
     @quorum.secured
     def test_timeout(self):
         self.assertRaises(
             BaseException,
             lambda: quorum.get_json(
                 "https://%s/delay/3" % self.httpbin,
-                handle = True,
-                redirect = True,
-                timeout = 1
-            )
+                handle=True,
+                redirect=True,
+                timeout=1,
+            ),
         )
 
         data, response = quorum.get_json(
-            "https://%s/delay/1" % self.httpbin,
-            handle = True,
-            redirect = True,
-            timeout = 30
+            "https://%s/delay/1" % self.httpbin, handle=True, redirect=True, timeout=30
         )
 
         code = response.getcode()
         self.assertEqual(code, 200)
         self.assertNotEqual(len(data), 0)
         self.assertNotEqual(data, None)
 
@@ -155,47 +152,44 @@
         file = quorum.get_f("https://%s/image/png" % self.httpbin)
 
         self.assertEqual(file.file_name, "default")
         self.assertEqual(file.mime, "image/png")
         self.assertEqual(len(file.data) > 100, True)
         self.assertEqual(len(file.data_b64) > 100, True)
 
-        file = quorum.get_f("https://%s/image/png" % self.httpbin, name = "dummy")
+        file = quorum.get_f("https://%s/image/png" % self.httpbin, name="dummy")
 
         self.assertEqual(file.file_name, "dummy")
         self.assertEqual(file.mime, "image/png")
         self.assertEqual(len(file.data) > 100, True)
         self.assertEqual(len(file.data_b64) > 100, True)
 
     @quorum.secured
     def test_generator(self):
-        def text_g(message = [b"hello", b" ", b"world"]):
+        def text_g(message=[b"hello", b" ", b"world"]):
             yield sum(len(value) for value in message)
             for value in message:
                 yield value
 
         data, response = quorum.post_json(
-            "https://%s/post" % self.httpbin,
-            data = text_g(),
-            handle = True,
-            reuse = False
+            "https://%s/post" % self.httpbin, data=text_g(), handle=True, reuse=False
         )
 
         code = response.getcode()
         self.assertNotEqual(code, 302)
         self.assertEqual(code, 200)
         self.assertEqual(data["data"], "hello world")
 
     @quorum.secured
     def test_file(self):
         data, response = quorum.post_json(
             "https://%s/post" % self.httpbin,
-            data = quorum.legacy.BytesIO(b"hello world"),
-            handle = True,
-            reuse = False
+            data=quorum.legacy.BytesIO(b"hello world"),
+            handle=True,
+            reuse=False,
         )
 
         code = response.getcode()
         self.assertNotEqual(code, 302)
         self.assertEqual(code, 200)
         self.assertEqual(data["data"], "hello world")
 
@@ -207,24 +201,24 @@
         for index in range(10):
             result = dict()
             results.append(result)
 
             def generate(index):
                 def caller():
                     data, response = quorum.get_json(
-                        "https://%s/ip" % self.httpbin,
-                        handle = True
+                        "https://%s/ip" % self.httpbin, handle=True
                     )
                     result = results[index]
                     result["data"] = data
                     result["response"] = response
+
                 return caller
 
             callable = generate(index)
-            thread = threading.Thread(target = callable, name = "TestMultithread")
+            thread = threading.Thread(target=callable, name="TestMultithread")
             thread.start()
             threads.append(thread)
 
         for thread, result in zip(threads, results):
             thread.join()
 
             response = result["response"]
@@ -232,16 +226,15 @@
             self.assertNotEqual(code, 302)
             self.assertEqual(code, 200)
 
     @quorum.secured
     def test_error(self):
         self.assertRaises(
             quorum.HTTPDataError,
-            lambda: quorum.get("https://%s/status/404" % self.httpbin)
+            lambda: quorum.get("https://%s/status/404" % self.httpbin),
         )
 
     @quorum.secured
     def test_invalid(self):
         self.assertRaises(
-            BaseException,
-            lambda: quorum.get("https://invalidlargedomain.org/")
+            BaseException, lambda: quorum.get("https://invalidlargedomain.org/")
         )
```

### Comparing `quorum-0.8.2/src/quorum/test/model.py` & `quorum-0.8.3/src/quorum/test/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,55 +18,45 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
 from . import mock
 
+
 class ModelTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(
-                name = __name__,
-                mongo_database = "test",
-                models = mock
-            )
+            quorum.load(name=__name__, mongo_database="test", models=mock)
         except Exception:
             self.skip()
 
     def tearDown(self):
         try:
             adapter = quorum.get_adapter()
             adapter.drop_db()
-        except Exception: pass
-        finally: quorum.unload()
+        except Exception:
+            pass
+        finally:
+            quorum.unload()
 
     @quorum.secured
     def test_basic(self):
-        person = mock.Person(fill = False)
+        person = mock.Person(fill=False)
         person.name = "Name"
 
         self.assertEqual(person.name, "Name")
         self.assertEqual(person["name"], "Name")
         self.assertEqual(len(person), 1)
 
         person["age"] = 20
@@ -89,23 +79,23 @@
         self.assertRaises(AttributeError, lambda: person.age)
         self.assertRaises(KeyError, lambda: person["age"])
 
         self.assertEqual(bool(person), False)
 
     @quorum.secured
     def test_find(self):
-        result = mock.Person.find(age = 1)
+        result = mock.Person.find(age=1)
         self.assertEqual(len(result), 0)
 
         person = mock.Person()
         person.age = 1
         person.name = "Name"
         person.save()
 
-        result = mock.Person.find(age = 1)
+        result = mock.Person.find(age=1)
         self.assertEqual(len(result), 1)
         self.assertEqual(result[0].age, 1)
 
     @quorum.secured
     def test_count(self):
         result = mock.Person.count()
         self.assertEqual(result, 0)
@@ -118,29 +108,30 @@
         result = mock.Person.count()
         self.assertEqual(result, 1)
 
     @quorum.secured
     def test_count_find(self):
         adapter = quorum.get_adapter()
         if not adapter.name in ("mongo",):
-            if not hasattr(self, "skipTest"): return
+            if not hasattr(self, "skipTest"):
+                return
             self.skipTest("Adapter is not supported")
 
         result = mock.Person.count()
         self.assertEqual(result, 0)
 
         person = mock.Person()
         person.age = 1
         person.name = "Name"
         person.save()
 
-        result = mock.Person.count(**dict(find_d = ["name:eq:Name"]))
+        result = mock.Person.count(**dict(find_d=["name:eq:Name"]))
         self.assertEqual(result, 1)
 
-        result = mock.Person.count(**dict(find_d = ["name:eq:OtherName"]))
+        result = mock.Person.count(**dict(find_d=["name:eq:OtherName"]))
         self.assertEqual(result, 0)
 
     @quorum.secured
     def test_delete(self):
         result = mock.Person.count()
         self.assertEqual(result, 0)
 
@@ -173,22 +164,22 @@
         result = person.advance("age")
         self.assertEqual(result, 2)
         self.assertEqual(person.age, 2)
 
         person = person.reload()
         self.assertEqual(person.age, 2)
 
-        result = person.advance("age", delta = 2)
+        result = person.advance("age", delta=2)
         self.assertEqual(result, 4)
         self.assertEqual(person.age, 4)
 
         person = person.reload()
         self.assertEqual(person.age, 4)
 
-        result = person.advance("age", delta = -2)
+        result = person.advance("age", delta=-2)
         self.assertEqual(result, 2)
         self.assertEqual(person.age, 2)
 
         person = person.reload()
         self.assertEqual(person.age, 2)
 
     @quorum.secured
@@ -228,15 +219,15 @@
 
         person.age = 20
         person.hidden = "Hidden"
 
         self.assertEqual(person.age, 20)
         self.assertEqual(person.hidden, "Hidden")
 
-        person_m = person.map(all = True)
+        person_m = person.map(all=True)
 
         self.assertEqual(isinstance(person_m, dict), True)
         self.assertEqual(person_m["identifier"], 1)
         self.assertEqual(person_m["identifier_safe"], 1)
         self.assertEqual(person_m["name"], "Name")
         self.assertEqual(person_m["age"], 20)
         self.assertEqual(person_m["hidden"], "Hidden")
@@ -249,34 +240,34 @@
         cat.save()
 
         self.assertEqual(cat.identifier, 1)
 
         person.cats = [cat]
         person.save()
 
-        person_m = person.map(resolve = True, all = True)
+        person_m = person.map(resolve=True, all=True)
 
         self.assertEqual(isinstance(person_m, dict), True)
         self.assertEqual(isinstance(person_m["cats"], list), True)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(person_m["cats"][0]["identifier"], 1)
         self.assertEqual(person_m["cats"][0]["identifier_safe"], 1)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(person.cats[0].name, "NameCat")
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
-        person_m = person.map(all = True)
+        person_m = person.map(all=True)
 
         self.assertEqual(person_m["cats"][0], 1)
 
-        person_m = person.map(resolve = True, all = True)
+        person_m = person.map(resolve=True, all=True)
 
         self.assertEqual(isinstance(person_m, dict), True)
         self.assertEqual(isinstance(person_m["cats"], list), True)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(person_m["cats"][0]["identifier"], 1)
         self.assertEqual(person_m["cats"][0]["identifier_safe"], 1)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
@@ -362,41 +353,41 @@
         other.save()
 
         result = mock.Person.find()
 
         self.assertEqual(result[0].identifier, person.identifier)
         self.assertEqual(result[1].identifier, other.identifier)
 
-        result = mock.Person.find(sort = [("identifier", -1)])
+        result = mock.Person.find(sort=[("identifier", -1)])
 
         self.assertEqual(result[0].identifier, other.identifier)
         self.assertEqual(result[1].identifier, person.identifier)
 
-        result = mock.Person.get(sort = [("identifier", -1)])
+        result = mock.Person.get(sort=[("identifier", -1)])
 
         self.assertEqual(result.identifier, other.identifier)
 
     @quorum.secured
     def test_range(self):
         for index in range(10):
             person = mock.Person()
             person.name = "Name%d" % index
             person.save()
 
-        result = mock.Person.find(limit = 5)
+        result = mock.Person.find(limit=5)
 
         self.assertEqual(len(result), 5)
         self.assertEqual(result[0].name, "Name0")
 
-        result = mock.Person.find(skip = 2, limit = 5)
+        result = mock.Person.find(skip=2, limit=5)
 
         self.assertEqual(len(result), 5)
         self.assertEqual(result[0].name, "Name2")
 
-        result = mock.Person.find(skip = 3, limit = 20)
+        result = mock.Person.find(skip=3, limit=20)
 
         self.assertEqual(len(result), 7)
         self.assertEqual(result[0].name, "Name3")
 
     @quorum.secured
     def test_references(self):
         person = mock.Person()
@@ -412,93 +403,89 @@
 
         cat.friend = cat_friend
         cat.save()
 
         person.cats = [cat]
         person.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(person.cats[0].name, "NameCat")
 
         person.cats = mock.Person.cats["type"]([cat])
         person.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(person.cats.is_resolved(), False)
         self.assertEqual(person.car, None)
         self.assertEqual(person.cats[0].name, "NameCat")
 
-        person = mock.Person.get(identifier = 1, map = True)
+        person = mock.Person.get(identifier=1, map=True)
 
         self.assertEqual(isinstance(person, dict), True)
         self.assertEqual(isinstance(person["cats"], list), True)
         self.assertEqual(isinstance(person["cats"][0], int), True)
         self.assertEqual(len(person["cats"]), 1)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats",))
+        person = mock.Person.get(identifier=1, eager=("cats",))
 
         self.assertEqual(isinstance(person.cats, quorum.References), True)
         self.assertEqual(isinstance(person.cats[0].friend, quorum.Reference), True)
         self.assertEqual(person.cats.is_resolved(), True)
         self.assertEqual(person.cats[0].friend.is_resolved(), False)
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(person.cats[0].name, "NameCat")
 
-        person = mock.Person.get(
-            identifier = 1,
-            map = True,
-            eager = ("cats",)
-        )
+        person = mock.Person.get(identifier=1, map=True, eager=("cats",))
 
         self.assertEqual(isinstance(person, dict), True)
         self.assertEqual(isinstance(person["cats"], list), True)
         self.assertEqual(isinstance(person["cats"][0], dict), True)
         self.assertEqual(isinstance(person["cats"], quorum.References), False)
-        self.assertEqual(isinstance(person["cats"][0]["friend"], quorum.Reference), False)
+        self.assertEqual(
+            isinstance(person["cats"][0]["friend"], quorum.Reference), False
+        )
         self.assertEqual(len(person["cats"]), 1)
         self.assertEqual(person["cats"][0]["name"], "NameCat")
         self.assertEqual(person["cats"][0]["friend"], 2)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats.friend",))
+        person = mock.Person.get(identifier=1, eager=("cats.friend",))
 
         self.assertEqual(isinstance(person.cats, quorum.References), True)
         self.assertEqual(isinstance(person.cats[0].friend, quorum.Reference), True)
         self.assertEqual(person.cats.is_resolved(), True)
         self.assertEqual(person.cats[0].friend.is_resolved(), True)
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(person.cats[0].name, "NameCat")
         self.assertEqual(person.cats[0].friend.name, "NameCatFriend")
 
-        person = mock.Person.get(
-            identifier = 1,
-            map = True,
-            eager = ("cats.friend",)
-        )
+        person = mock.Person.get(identifier=1, map=True, eager=("cats.friend",))
 
         self.assertEqual(isinstance(person, dict), True)
         self.assertEqual(isinstance(person["cats"], list), True)
         self.assertEqual(isinstance(person["cats"][0], dict), True)
         self.assertEqual(isinstance(person["cats"][0]["friend"], dict), True)
         self.assertEqual(isinstance(person["cats"], quorum.References), False)
-        self.assertEqual(isinstance(person["cats"][0]["friend"], quorum.Reference), False)
+        self.assertEqual(
+            isinstance(person["cats"][0]["friend"], quorum.Reference), False
+        )
         self.assertEqual(person["cats"][0]["name"], "NameCat")
         self.assertEqual(person["cats"][0]["friend"]["name"], "NameCatFriend")
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         person.cats = []
         person.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(len(person.cats), 0)
 
-        person = mock.Person.get(map = True, eager = ("cats",))
+        person = mock.Person.get(map=True, eager=("cats",))
 
         self.assertEqual(isinstance(person, dict), True)
         self.assertEqual(isinstance(person["cats"], list), True)
         self.assertEqual(len(person["cats"]), 0)
 
     @quorum.secured
     def test_eager(self):
@@ -514,68 +501,68 @@
         garage.name = "Garage"
         garage.save()
 
         address = mock.Address()
         address.street = "Address"
         address.save()
 
-        person = mock.Person.get(identifier = 1, eager_l = True)
+        person = mock.Person.get(identifier=1, eager_l=True)
         person.car = car
         person.save()
 
-        car = mock.Car.get(identifier = 1, eager_l = True)
+        car = mock.Car.get(identifier=1, eager_l=True)
         car.garage = garage
         car.save()
 
-        garage = mock.Garage.get(identifier = 1, eager_l = True)
+        garage = mock.Garage.get(identifier=1, eager_l=True)
         garage.address = address
         garage.save()
 
-        person = mock.Person.get(identifier = 1, eager_l = True)
+        person = mock.Person.get(identifier=1, eager_l=True)
 
         self.assertEqual(isinstance(person.car, quorum.Reference), True)
         self.assertEqual(person.car.is_resolved(), True)
         self.assertEqual(person.car.name, "Car")
         self.assertEqual(person.car.garage.is_resolved(), True)
         self.assertEqual(person.car.garage.name, "Garage")
         self.assertEqual(person.car.garage.address.is_resolved(), True)
         self.assertEqual(person.car.garage.address.street, "Address")
 
-        person = mock.Person.get(identifier = 1, eager_l = False)
+        person = mock.Person.get(identifier=1, eager_l=False)
 
         self.assertEqual(isinstance(person.car, quorum.Reference), True)
         self.assertEqual(person.car.is_resolved(), False)
         self.assertEqual(person.car.name, "Car")
         self.assertEqual(person.car.garage.is_resolved(), False)
         self.assertEqual(person.car.garage.name, "Garage")
         self.assertEqual(person.car.garage.address.is_resolved(), False)
         self.assertEqual(person.car.garage.address.street, "Address")
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(isinstance(person.car, quorum.Reference), True)
         self.assertEqual(person.car.is_resolved(), False)
         self.assertEqual(person.car.name, "Car")
         self.assertEqual(person.car.garage.is_resolved(), False)
         self.assertEqual(person.car.garage.name, "Garage")
         self.assertEqual(person.car.garage.address.is_resolved(), False)
         self.assertEqual(person.car.garage.address.street, "Address")
 
-        person = mock.Person.get(identifier = 1, map = True)
+        person = mock.Person.get(identifier=1, map=True)
 
         self.assertEqual(person["car"]["name"], "Car")
         self.assertEqual(person["car"]["garage"]["name"], "Garage")
         self.assertEqual(person["car"]["garage"]["address"]["street"], "Address")
 
-        person = mock.Person.get(identifier = 1, eager_l = True)
+        person = mock.Person.get(identifier=1, eager_l=True)
 
         person.car.name = "CarChanged"
         person.car.save()
 
-        person = mock.Person.get(identifier = 1, eager_l = True)
+        person = mock.Person.get(identifier=1, eager_l=True)
 
         self.assertEqual(person.car.name, "CarChanged")
 
         father = mock.Person()
         father.name = "Father"
         father.save()
 
@@ -585,15 +572,15 @@
 
         father.car = car_father
         father.save()
 
         person.father = father
         person.save()
 
-        person = mock.Person.get(identifier = 1, eager_l = True)
+        person = mock.Person.get(identifier=1, eager_l=True)
 
         self.assertEqual(isinstance(person.father, quorum.Reference), True)
         self.assertEqual(person.father.is_resolved(), False)
         self.assertEqual(person.car.is_resolved(), True)
 
         person.father.resolve()
 
@@ -613,30 +600,30 @@
         person.name = "Name"
         person.save()
 
         car = mock.Car()
         car.name = "Car"
         car.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
         person.car = car
         person.save()
 
         self.assertEqual(isinstance(person.car, quorum.Reference), False)
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(isinstance(person.car, quorum.Reference), True)
         self.assertEqual(person.car.is_resolvable(), True)
         self.assertEqual(person.car == None, False)
         self.assertEqual(person.car.name, "Car")
 
         car.delete()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         self.assertEqual(isinstance(person.car, quorum.Reference), True)
         self.assertEqual(person.car.is_resolvable(), False)
         self.assertEqual(person.car == None, False)
 
     @quorum.secured
     def test_exists(self):
@@ -645,76 +632,76 @@
 
         self.assertEqual(person.exists(), False)
 
         person.save()
 
         self.assertEqual(person.exists(), True)
 
-        person = mock.Person.get(name = "Name")
+        person = mock.Person.get(name="Name")
 
         self.assertEqual(person.exists(), True)
 
         person.delete()
 
         self.assertEqual(person.exists(), False)
 
     @quorum.secured
     def test_fill(self):
-        first = mock.Person(fill = True)
-        second = mock.Person(fill = True)
+        first = mock.Person(fill=True)
+        second = mock.Person(fill=True)
 
         self.assertEqual(first.info, {})
         self.assertEqual(second.info, {})
         self.assertNotEqual(id(first.info), id(second.info))
 
     @quorum.secured
     def test_wrap(self):
-        person = mock.Person.wrap(dict(name = "Person"))
+        person = mock.Person.wrap(dict(name="Person"))
         self.assertEqual(person.name, "Person")
 
-        person = mock.Person.wrap(dict(other = "Other"))
+        person = mock.Person.wrap(dict(other="Other"))
         self.assertEqual(person.other, "Other")
 
     @quorum.secured
     def test_meta(self):
         self.assertEqual(quorum.Model._to_meta(str), "string")
         self.assertEqual(quorum.Model._to_meta(bool), "bool")
         self.assertEqual(quorum.Model._to_meta("text"), "text")
         self.assertEqual(quorum.Model._to_meta("longtext"), "longtext")
         self.assertEqual(quorum.Model._to_meta(mock.Person.father["type"]), "reference")
 
     @quorum.secured
     def test_meta_map(self):
         method = quorum.model.METAS["map"]
 
-        map = dict(hello = "world")
+        map = dict(hello="world")
         result = method(map, {})
 
         self.assertEqual(type(result), str)
-        self.assertEqual(result, "{\"hello\": \"world\"}")
+        self.assertEqual(result, '{"hello": "world"}')
 
-        map = dict(mundo = "olá")
+        map = dict(mundo="olá")
 
         self.assertEqual(type(result), str)
-        self.assertEqual(method(map, {}), "{\"mundo\": \"olá\"}")
+        self.assertEqual(method(map, {}), '{"mundo": "olá"}')
 
     @quorum.secured
     def test_meta_longmap(self):
         method = quorum.model.METAS["longmap"]
 
-        map = dict(hello = "world")
+        map = dict(hello="world")
         result = method(map, {})
 
         self.assertEqual(type(result), str)
-        self.assertEqual(result, "{\"hello\": \"world\"}")
+        self.assertEqual(result, '{"hello": "world"}')
 
-        map = dict(mundo = "olá")
+        map = dict(mundo="olá")
 
         self.assertEqual(type(result), str)
-        self.assertEqual(method(map, {}), "{\"mundo\": \"olá\"}")
+        self.assertEqual(method(map, {}), '{"mundo": "olá"}')
 
     @quorum.secured
     def test_is_unset(self):
         person = mock.Person()
         person.name = "Name"
         person.save()
 
@@ -762,87 +749,87 @@
 
         cat.friend = cat_friend
         cat.save()
 
         person.cats = [cat]
         person.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
         person_m = person.map_v()
 
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(isinstance(person.cats[0], dict), True)
         self.assertEqual(person.cats[0]["friend"]["name"], "NameCatFriend")
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(isinstance(person_m["cats"][0]["friend"], dict), True)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
         self.assertEqual(person_m["cats"][0]["friend"]["name"], "NameCatFriend")
 
         person = person.reload()
-        person_m = person.map_v(resolve = False)
+        person_m = person.map_v(resolve=False)
 
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(isinstance(person.cats[0], int), 1)
         self.assertEqual(person.cats[0], 1)
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], int), True)
         self.assertEqual(person_m["cats"][0], 1)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats",))
-        person_m = person.map_v(resolve = False)
+        person = mock.Person.get(identifier=1, eager=("cats",))
+        person_m = person.map_v(resolve=False)
 
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(isinstance(person.cats[0], dict), True)
         self.assertEqual(person.cats[0]["friend"], 2)
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(isinstance(person_m["cats"][0]["friend"], int), True)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
         self.assertEqual(person_m["cats"][0]["friend"], 2)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats",))
-        person_m = person.map_v(resolve = False, evaluator = "map_v")
+        person = mock.Person.get(identifier=1, eager=("cats",))
+        person_m = person.map_v(resolve=False, evaluator="map_v")
 
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(isinstance(person.cats[0], dict), True)
         self.assertEqual(person.cats[0]["friend"], 2)
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(isinstance(person_m["cats"][0]["friend"], int), True)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
         self.assertEqual(person_m["cats"][0]["friend"], 2)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats",))
-        person_m = person.map_v(clone = True, resolve = False)
+        person = mock.Person.get(identifier=1, eager=("cats",))
+        person_m = person.map_v(clone=True, resolve=False)
 
         self.assertEqual(isinstance(person.cats, quorum.References), True)
         self.assertEqual(person.cats.is_resolved(), True)
         self.assertEqual(isinstance(person.cats[0].friend, quorum.Reference), True)
         self.assertEqual(person.cats[0].friend.is_resolved(), False)
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(isinstance(person_m["cats"][0]["friend"], int), True)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
         self.assertEqual(person_m["cats"][0]["friend"], 2)
 
-        person = mock.Person.get(identifier = 1, eager = ("cats.friend",))
-        person_m = person.map_v(resolve = False)
+        person = mock.Person.get(identifier=1, eager=("cats.friend",))
+        person_m = person.map_v(resolve=False)
 
         self.assertEqual(len(person.cats), 1)
         self.assertEqual(isinstance(person.cats[0], dict), True)
         self.assertEqual(person.cats[0]["friend"]["name"], "NameCatFriend")
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
         self.assertEqual(isinstance(person_m["cats"][0]["friend"], dict), True)
         self.assertEqual(person_m["cats"][0]["name"], "NameCat")
         self.assertEqual(person_m["cats"][0]["friend"]["name"], "NameCatFriend")
 
-        person = mock.Person.get(identifier = 1, eager = ("cats.friend",))
-        person_m = person.map_v(clone = True, resolve = False)
+        person = mock.Person.get(identifier=1, eager=("cats.friend",))
+        person_m = person.map_v(clone=True, resolve=False)
 
         self.assertEqual(isinstance(person.cats, quorum.References), True)
         self.assertEqual(person.cats.is_resolved(), True)
         self.assertEqual(isinstance(person.cats[0].friend, quorum.Reference), True)
         self.assertEqual(person.cats[0].friend.is_resolved(), True)
         self.assertEqual(len(person_m["cats"]), 1)
         self.assertEqual(isinstance(person_m["cats"][0], dict), True)
@@ -864,22 +851,22 @@
         person_c.save()
 
         self.assertEqual(id(person_c.model), id(person.model))
         self.assertEqual(person_c.model, person.model)
         self.assertEqual(person_c.identifier, 2)
         self.assertEqual(person_c.name, "NameC")
 
-        person_c = person.clone(reset = False)
+        person_c = person.clone(reset=False)
 
         self.assertEqual(id(person_c.model), id(person.model))
         self.assertEqual(person_c.model, person.model)
         self.assertEqual(person_c.identifier, 2)
         self.assertEqual(person_c.name, "NameC")
 
-        person_c = person.clone(deep = True)
+        person_c = person.clone(deep=True)
         person_c.name = "NameC2"
         person_c.save()
 
         self.assertNotEqual(id(person_c.model), id(person.model))
         self.assertNotEqual(person_c.model, person.model)
         self.assertEqual(person_c.identifier, 3)
         self.assertEqual(person_c.name, "NameC2")
```

### Comparing `quorum-0.8.2/src/quorum/test/amazon.py` & `quorum-0.8.3/src/quorum/test/amazon.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,44 +18,39 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class AmazonTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(name = __name__)
+            quorum.load(name=__name__)
             quorum.get_amazon()
         except Exception:
             self.skip()
 
     def tearDown(self):
-        try: quorum.clear_amazon_bucket()
-        except Exception: pass
-        finally: quorum.unload()
+        try:
+            quorum.clear_amazon_bucket()
+        except Exception:
+            pass
+        finally:
+            quorum.unload()
 
     @quorum.secured
     def test_connect(self):
         connection = quorum.get_amazon()
         self.assertNotEqual(connection, None)
 
     @quorum.secured
```

### Comparing `quorum-0.8.2/src/quorum/test/typesf.py` & `quorum-0.8.3/src/quorum/test/typesf.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,51 +18,41 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
 from . import mock
 
+
 class TypesfTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            quorum.load(
-                name = __name__,
-                mongo_database = "test",
-                models = mock
-            )
+            quorum.load(name=__name__, mongo_database="test", models=mock)
         except Exception:
             self.skip()
 
     def tearDown(self):
         try:
             adapter = quorum.get_adapter()
             adapter.drop_db()
-        except Exception: pass
-        finally: quorum.unload()
+        except Exception:
+            pass
+        finally:
+            quorum.unload()
 
     @quorum.secured
     def test_reference(self):
         person = mock.Person()
         person.name = "Name"
         person.car = mock.Person.car["type"]("")
 
@@ -120,26 +110,26 @@
 
     @quorum.secured
     def test_references(self):
         person = mock.Person()
         person.name = "Name"
         person.cats = mock.Person.cats["type"]([1, 2, 3])
 
-        self.assertEqual(mock.Cat(identifier = 1) in person.cats, True)
-        self.assertEqual(mock.Cat(identifier = 3) in person.cats, True)
-        self.assertNotEqual(mock.Cat(identifier = 4) in person.cats, True)
+        self.assertEqual(mock.Cat(identifier=1) in person.cats, True)
+        self.assertEqual(mock.Cat(identifier=3) in person.cats, True)
+        self.assertNotEqual(mock.Cat(identifier=4) in person.cats, True)
         self.assertNotEqual(person.cats, None)
         self.assertNotEqual(person.cats, [])
         self.assertNotEqual(person.cats, "cars")
         self.assertEqual(isinstance(person.cats, quorum.References), True)
         self.assertEqual(len(person.cats), 3)
 
     @quorum.secured
     def test_file(self):
-        file_m = dict(name = "hello", data = b"SGVsbG8gV29ybGQ=")
+        file_m = dict(name="hello", data=b"SGVsbG8gV29ybGQ=")
         file = quorum.File(file_m)
 
         self.assertEqual(type(file.file_name), str)
         self.assertEqual(type(file.data_b64), str)
         self.assertEqual(type(file.data), quorum.legacy.BYTES)
         self.assertEqual(file.file_name, "hello")
         self.assertEqual(file.data, b"Hello World")
@@ -153,28 +143,28 @@
         self.assertEqual(type(file.data), quorum.legacy.BYTES)
         self.assertEqual(file.file_name, "default")
         self.assertEqual(file.data, b"Hello World")
         self.assertEqual(file.data_b64, "SGVsbG8gV29ybGQ=")
 
     @quorum.secured
     def test_encrypted(self):
-        encrypted = quorum.encrypted(key = b"hello key")
+        encrypted = quorum.encrypted(key=b"hello key")
         result = encrypted("hello world")
 
         self.assertEqual(str(result), "hello world")
         self.assertEqual(result.value, "hello world")
         self.assertEqual(result.encrypted, "vGgMtFgyMVwH3uE=:encrypted")
 
         result = encrypted("vGgMtFgyMVwH3uE=:encrypted")
 
         self.assertEqual(str(result), "hello world")
         self.assertEqual(result.value, "hello world")
         self.assertEqual(result.encrypted, "vGgMtFgyMVwH3uE=:encrypted")
 
-        encrypted = quorum.encrypted(key = None)
+        encrypted = quorum.encrypted(key=None)
         result = encrypted("hello world")
 
         self.assertEqual(str(result), "hello world")
         self.assertEqual(result.value, "hello world")
         self.assertEqual(result.value, "hello world")
 
         result = encrypted("vGgMtFgyMVwH3uE=:encrypted")
@@ -202,15 +192,15 @@
         brother.save()
 
         person.car = car
         person.father = father
         person.brother = brother
         person.save()
 
-        person = mock.Person.get(identifier = 1)
+        person = mock.Person.get(identifier=1)
 
         result = person.json_v()
 
         self.assertEqual(type(result), dict)
         self.assertEqual(result["name"], "Name")
 
         result = person.car.json_v()
```

### Comparing `quorum-0.8.2/src/quorum/test/crypt.py` & `quorum-0.8.3/src/quorum/test/crypt.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,31 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class CryptTest(quorum.TestCase):
 
     @quorum.secured
     def test_rc4(self):
         rc4 = quorum.RC4(b"hello key")
         result = rc4.encrypt(b"hello world")
```

### Comparing `quorum-0.8.2/src/quorum/test/acl.py` & `quorum-0.8.3/src/quorum/test/acl.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,179 +18,127 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import flask
 
 import quorum
 
+
 class ACLTest(quorum.TestCase):
 
     def setUp(self):
         try:
-            self.app = quorum.load(
-                name = __name__,
-                secret_key = "secret"
-            )
+            self.app = quorum.load(name=__name__, secret_key="secret")
             self.app.config["APPLICATION_ROOT"] = "/"
         except Exception:
             self.skip()
 
     def tearDown(self):
         quorum.unload()
 
     @quorum.secured
     def test_check_login(self):
         with self.app.test_client() as client:
             client.get("/")
 
             flask.session["tokens"] = ["*"]
-            result = quorum.check_login(token = "admin")
+            result = quorum.check_login(token="admin")
             self.assertEqual(result, True)
-            self.assertEqual(flask.session["tokens"], {"*" : True})
+            self.assertEqual(flask.session["tokens"], {"*": True})
 
             flask.session["tokens"] = []
-            result = quorum.check_login(token = "admin")
+            result = quorum.check_login(token="admin")
             self.assertEqual(result, False)
             self.assertEqual(flask.session["tokens"], {})
 
             flask.session["tokens"] = ["admin"]
-            result = quorum.check_login(token = "admin")
+            result = quorum.check_login(token="admin")
             self.assertEqual(result, True)
-            self.assertEqual(flask.session["tokens"], {"admin" : True})
+            self.assertEqual(flask.session["tokens"], {"admin": True})
 
             flask.session["tokens"] = ["admin.read"]
-            result = quorum.check_login(token = "admin")
+            result = quorum.check_login(token="admin")
             self.assertEqual(result, False)
-            result = quorum.check_login(token = "admin.read")
+            result = quorum.check_login(token="admin.read")
             self.assertEqual(result, True)
-            self.assertEqual(flask.session["tokens"], {
-                "admin" : {
-                    "read" : True
-                }
-            })
+            self.assertEqual(flask.session["tokens"], {"admin": {"read": True}})
 
             flask.session["tokens"] = ["admin.*"]
-            result = quorum.check_login(token = "admin.read")
+            result = quorum.check_login(token="admin.read")
             self.assertEqual(result, True)
-            self.assertEqual(flask.session["tokens"], {
-                "admin" : {
-                    "*" : True
-                }
-            })
+            self.assertEqual(flask.session["tokens"], {"admin": {"*": True}})
 
             flask.session["tokens"] = ["admin", "admin.write"]
-            result = quorum.check_login(token = "admin.read")
+            result = quorum.check_login(token="admin.read")
             self.assertEqual(result, False)
-            self.assertEqual(flask.session["tokens"], {
-                "admin" : {
-                    "_" : True,
-                    "write" : True
-                }
-            })
+            self.assertEqual(
+                flask.session["tokens"], {"admin": {"_": True, "write": True}}
+            )
 
             flask.session["tokens"] = ["admin.write", "admin.*"]
-            result = quorum.check_login(token = "admin.read")
+            result = quorum.check_login(token="admin.read")
             self.assertEqual(result, True)
-            self.assertEqual(flask.session["tokens"], {
-                "admin" : {
-                    "write" : True,
-                    "*" : True
-                }
-            })
+            self.assertEqual(
+                flask.session["tokens"], {"admin": {"write": True, "*": True}}
+            )
 
             del flask.session["tokens"]
-            result = quorum.check_login(token = "admin.read")
+            result = quorum.check_login(token="admin.read")
             self.assertEqual(result, False)
             self.assertEqual("tokens" in flask.session, False)
 
     @quorum.secured
     def test_check_tokens(self):
-        result = quorum.check_tokens(("admin", "user"), tokens_m = {"*" : True})
+        result = quorum.check_tokens(("admin", "user"), tokens_m={"*": True})
         self.assertEqual(result, True)
 
-        result = quorum.check_tokens(("admin", "user"), tokens_m = {})
+        result = quorum.check_tokens(("admin", "user"), tokens_m={})
         self.assertEqual(result, False)
 
-        result = quorum.check_tokens(("admin", "user"), tokens_m = {"admin" : True})
+        result = quorum.check_tokens(("admin", "user"), tokens_m={"admin": True})
         self.assertEqual(result, False)
 
     @quorum.secured
     def test_check_token(self):
-        result = quorum.check_token("admin", tokens_m = {"*" : True})
+        result = quorum.check_token("admin", tokens_m={"*": True})
         self.assertEqual(result, True)
 
-        result = quorum.check_token("admin", tokens_m = {})
+        result = quorum.check_token("admin", tokens_m={})
         self.assertEqual(result, False)
 
-        result = quorum.check_token("admin", tokens_m = {"admin" : True})
+        result = quorum.check_token("admin", tokens_m={"admin": True})
         self.assertEqual(result, True)
 
-        result = quorum.check_token("admin.read", tokens_m = {
-            "admin" : {
-                "read" : True
-            }
-        })
+        result = quorum.check_token("admin.read", tokens_m={"admin": {"read": True}})
         self.assertEqual(result, True)
 
-        result = quorum.check_token("admin", tokens_m = {
-            "admin" : {
-                "read" : True
-            }
-        })
+        result = quorum.check_token("admin", tokens_m={"admin": {"read": True}})
         self.assertEqual(result, False)
 
-        result = quorum.check_token("admin.read", tokens_m = {
-            "admin" : {
-                "*" : True
-            }
-        })
+        result = quorum.check_token("admin.read", tokens_m={"admin": {"*": True}})
         self.assertEqual(result, True)
 
-        result = quorum.check_token(None, tokens_m = {})
+        result = quorum.check_token(None, tokens_m={})
         self.assertEqual(result, True)
 
     def test_to_tokens_m(self):
         result = quorum.to_tokens_m(["admin"])
-        self.assertEqual(result, {"admin" : True})
+        self.assertEqual(result, {"admin": True})
 
         result = quorum.to_tokens_m(["admin", "admin.read"])
-        self.assertEqual(result, {
-            "admin" : {
-                "_" : True,
-                "read" : True
-            }
-        })
+        self.assertEqual(result, {"admin": {"_": True, "read": True}})
 
         result = quorum.to_tokens_m(["admin.read", "admin"])
-        self.assertEqual(result, {
-            "admin" : {
-                "_" : True,
-                "read" : True
-            }
-        })
+        self.assertEqual(result, {"admin": {"_": True, "read": True}})
 
         result = quorum.to_tokens_m(["admin", "admin.*"])
-        self.assertEqual(result, {
-            "admin" : {
-                "_" : True,
-                "*" : True
-            }
-        })
+        self.assertEqual(result, {"admin": {"_": True, "*": True}})
```

### Comparing `quorum-0.8.2/src/quorum/test/__init__.py` & `quorum-0.8.3/src/quorum/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
+__author__ = "João Magalhães <joamag@hive.pt>"
+""" The author(s) of the module """
 
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
+
+NAME = "quorum"
+VERSION = "0.8.3"
+AUTHOR = "Hive Solutions Lda."
+EMAIL = "development@hive.pt"
+DESCRIPTION = "Quorum Extensions for Flask"
+LICENSE = "Apache License, Version 2.0"
+KEYWORDS = "quorum flask"
+URL = "http://flask-quorum.hive.pt"
+COPYRIGHT = "2008-2022 Hive Solutions Lda."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quorum-0.8.2/src/quorum/jsonf.py` & `quorum-0.8.3/src/quorum/jsonf.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,34 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
 
 from . import base
 
+
 def load_json(*args, **kwargs):
     path = base.base_path(*args, **kwargs)
     file = open(path, "rb")
-    try: data = file.read()
-    finally: file.close()
+    try:
+        data = file.read()
+    finally:
+        file.close()
     data = data.decode("utf-8")
     data = json.loads(data)
     return data
```

### Comparing `quorum-0.8.2/src/quorum/util.py` & `quorum-0.8.3/src/quorum/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -66,130 +57,143 @@
 
 ALL_CAP_REGEX = re.compile("([a-z0-9])([A-Z])")
 """ The generalized transition from lower case to
 upper case letter regex that will provide a way of
 putting the underscore in the middle of the transition """
 
 SORT_MAP = {
-    "1" : 1,
-    "-1" : -1,
-    "ascending" : 1,
-    "descending" : -1,
+    "1": 1,
+    "-1": -1,
+    "ascending": 1,
+    "descending": -1,
 }
 """ The map associating the normalized (text) way of
 representing sorting with the current infra-structure
 number way of representing the same information """
 
 CASTERS = {
-    list : lambda v: [y for y in itertools.chain(*[split_unescape(x, ",").split(",") for x in v])],
-    bool : lambda v: v if isinstance(v, bool) else\
-        not v in ("", "0", "false", "False"),
-    dict : lambda v: json.loads(v) if legacy.is_string(v) else dict(v)
+    list: lambda v: [
+        y for y in itertools.chain(*[split_unescape(x, ",").split(",") for x in v])
+    ],
+    bool: lambda v: v if isinstance(v, bool) else not v in ("", "0", "false", "False"),
+    dict: lambda v: json.loads(v) if legacy.is_string(v) else dict(v),
 }
 """ The map associating the various data types with a proper custom
 caster to be used for special data types (more complex) under some
 of the simple casting operations """
 
 defines = defines
 
+
 def to_limit(limit_s):
     limit = int(limit_s)
-    if limit < 0: return 0
+    if limit < 0:
+        return 0
     return limit
 
+
 def to_find(find_s):
-    if not find_s: return []
+    if not find_s:
+        return []
     find_t = type(find_s)
-    if find_t == list: return find_s
+    if find_t == list:
+        return find_s
     return [find_s]
 
+
 def to_sort(sort_s):
     sort_l = []
     sorts = sort_s.split(",")
     for sort_i in sorts:
         values = sort_i.split(":", 1)
-        if len(values) == 1: values.append("descending")
+        if len(values) == 1:
+            values.append("descending")
         name, direction = values
-        if name == "default": return None
+        if name == "default":
+            return None
         values[1] = SORT_MAP.get(direction, 1)
         sort_l.append(tuple(values))
     return sort_l
 
+
 ALIAS = {
-    "context" : "find_d",
-    "filters" : "find_d",
-    "filters[]" : "find_d",
-    "filter_def" : "find_d",
-    "filter_string" : "find_s",
-    "filter_name" : "find_n",
-    "filter_operator" : "find_o",
-    "insensitive" : "find_i",
-    "order" : "sort",
-    "offset" : "skip",
-    "start_record" : "skip",
-    "number_records" : "limit"
+    "context": "find_d",
+    "filters": "find_d",
+    "filters[]": "find_d",
+    "filter_def": "find_d",
+    "filter_string": "find_s",
+    "filter_name": "find_n",
+    "filter_operator": "find_o",
+    "insensitive": "find_i",
+    "order": "sort",
+    "offset": "skip",
+    "start_record": "skip",
+    "number_records": "limit",
 }
 """ The map containing the various attribute alias
 between the normalized manned and the quorum manner """
 
 FIND_TYPES = dict(
-    skip = int,
-    limit = to_limit,
-    find_s = legacy.UNICODE,
-    find_d = to_find,
-    find_i = bool,
-    find_t = legacy.UNICODE,
-    find_n = legacy.UNICODE,
-    find_o = legacy.UNICODE,
-    sort = to_sort,
-    meta = bool,
-    fields = list
+    skip=int,
+    limit=to_limit,
+    find_s=legacy.UNICODE,
+    find_d=to_find,
+    find_i=bool,
+    find_t=legacy.UNICODE,
+    find_n=legacy.UNICODE,
+    find_o=legacy.UNICODE,
+    sort=to_sort,
+    meta=bool,
+    fields=list,
 )
 """ The map associating the various find fields with
 their respective types, note that in case a special
 conversion operation is required the associated value
 may represent a conversion function instead """
 
-FIND_DEFAULTS = dict(
-    limit = 10
-)
+FIND_DEFAULTS = dict(limit=10)
 """ The map that defines the various default values
 for a series of find related attributes """
 
+
 def is_iterable(object):
     return isinstance(object, defines.ITERABLES)
 
-def request_json(request = None, encoding = "utf-8"):
+
+def request_json(request=None, encoding="utf-8"):
     # retrieves the proper request object, either the provided
     # request or the default flask request object and then in
     # case the the JSON data is already in the request properties
     # it is used (cached value) otherwise continues with the parse
     request = request or flask.request
     try:
         if "_data_j" in request.properties:
             return request.properties["_data_j"]
-    except RuntimeError: pass
+    except RuntimeError:
+        pass
 
     # retrieves the current request data and tries to
     # "load" it as JSON data, in case it fails gracefully
     # handles the failure setting the value as an empty map
     data = request.data
     try:
         is_bytes = legacy.is_bytes(data)
-        if is_bytes: data = data.decode(encoding)
+        if is_bytes:
+            data = data.decode(encoding)
         data_j = json.loads(data)
     except Exception:
         data_j = {}
     request.properties["_data_j"] = data_j
 
     # returns the JSON data object to the caller method so that it
     # may be used as the parsed value (post information)
     return data_j
 
-def get_field(name, default = None, cast = None, strip = False):
+
+def get_field(name, default=None, cast=None, strip=False):
     # tries to retrieve the JSON based representation of the provided
     # request from all the possible sources, this is required because
     # it's going to be used to try to retrieve a field from it
     data_j = request_json()
 
     # tries to retrieve the requested field from all the requested sources
     # the order of retrieval should respect the importance of each of the
@@ -197,256 +201,306 @@
     value = data_j.get(name, default)
     value = flask.request.files.get(name, value)
     value = flask.request.form.get(name, value)
     value = flask.request.args.get(name, value)
 
     # in case the strip flag is enabled an "extra" strip operation is applied
     # to the retrieved value (as requested), avoiding extra spaces
-    if strip: value = value.strip()
+    if strip:
+        value = value.strip()
 
     # in case a cast operation is defined, tries to retrieve a possible
     # indirect/custom caster for the current cast operation
-    if cast: cast = CASTERS.get(cast, cast)
+    if cast:
+        cast = CASTERS.get(cast, cast)
 
     # in case the cast type value is set and the value is not invalid tries
     # to cast the value into the requested cast type
-    if cast and not value in (None, ""): value = cast(value)
+    if cast and not value in (None, ""):
+        value = cast(value)
 
     # returns the final value to the caller method to be used, note that the
     # caller method should be aware of the sources used in the field retrieval
     return value
 
-def get_object(
-    object = None,
-    alias = False,
-    page = False,
-    find = False,
-    norm = True,
-    **kwargs
-):
+
+def get_object(object=None, alias=False, page=False, find=False, norm=True, **kwargs):
     # verifies if the provided object is valid in such case creates
     # a copy of it and uses it as the base object for validation
     # otherwise used an empty map (form validation)
     object = object and copy.copy(object) or {}
 
     # retrieves the current request data and tries to
     # "load" it as JSON data, in case it fails gracefully
     # handles the failure setting the value as an empty map
-    try: data_j = request_json()
-    except RuntimeError: data_j = dict()
+    try:
+        data_j = request_json()
+    except RuntimeError:
+        data_j = dict()
 
     # retrieves the reference to the file objects currently
     # present in the request, note that in case a runtime
     # error occurs (eg: out of context) fails gracefully
-    try: files = flask.request.files
-    except RuntimeError: files = dict()
+    try:
+        files = flask.request.files
+    except RuntimeError:
+        files = dict()
 
     # retrieves the reference to the form objects currently
     # present in the request, note that in case a runtime
     # error occurs (eg: out of context) fails gracefully
-    try: form_s = flask.request.form_s #@UndefinedVariable
-    except RuntimeError: form_s = dict()
+    try:
+        form_s = flask.request.form_s  # @UndefinedVariable
+    except RuntimeError:
+        form_s = dict()
 
     # retrieves the reference to the arguments objects currently
     # present in the request, note that in case a runtime
     # error occurs (eg: out of context) fails gracefully
-    try: args_s = flask.request.args_s #@UndefinedVariable
-    except RuntimeError: args_s = dict()
+    try:
+        args_s = flask.request.args_s  # @UndefinedVariable
+    except RuntimeError:
+        args_s = dict()
 
     # uses all the values referencing data in the request to try
     # to populate the object this way it may be constructed using
     # any of theses strategies (easier for the developer)
-    for name, value in data_j.items(): object[name] = value
-    for name, value in files.items(): object[name] = value
-    for name, value in form_s.items(): object[name] = value
-    for name, value in args_s.items(): object[name] = value
+    for name, value in data_j.items():
+        object[name] = value
+    for name, value in files.items():
+        object[name] = value
+    for name, value in form_s.items():
+        object[name] = value
+    for name, value in args_s.items():
+        object[name] = value
 
     # in case the alias flag is set tries to resolve the attribute
     # alias and in case the find types are set converts the find
     # based attributes using the currently defined mapping map
-    if alias: resolve_alias(object)
-    if page: page_types(object)
-    if find: find_types(object)
-    if find: find_defaults(object, kwargs)
+    if alias:
+        resolve_alias(object)
+    if page:
+        page_types(object)
+    if find:
+        find_types(object)
+    if find:
+        find_defaults(object, kwargs)
 
     # in case the normalization flag is set runs the normalization
     # of the provided object so that sequences are properly handled
     # as defined in the specification (this allows multiple references)
-    if norm: norm_object(object)
+    if norm:
+        norm_object(object)
 
     # returns the constructed object to the caller method this object
     # should be a structured representation of the data in the request
     return object
 
-def is_mobile(user_agent = None):
+
+def is_mobile(user_agent=None):
     """
     Verifies if the current user agent string represents a
     mobile agent, for that a series of regular expressions
     are matched against the user agent string.
 
     :type user_agent: String
     :param user_agent: The string containing the user agent
     value that is going to be verified against a series of
     regular expressions for mobile verification.
     :rtype: bool
     :return: If the current user agent string represents a
     mobile browser or a regular (desktop) one.
     """
 
-    user_agent = flask.request.headers.get("User-Agent", "")\
-        if user_agent == None else user_agent
+    user_agent = (
+        flask.request.headers.get("User-Agent", "")
+        if user_agent == None
+        else user_agent
+    )
     prefix = user_agent[:4]
     mobile = defines.MOBILE_REGEX.search(user_agent)
     mobile_prefix = defines.MOBILE_PREFIX_REGEX.search(prefix)
     is_mobile = True if mobile or mobile_prefix else False
     return is_mobile
 
-def is_tablet(user_agent = None):
+
+def is_tablet(user_agent=None):
     """
     Verifies if the current user agent string represents a
     tablet agent, for that a series of regular expressions
     are matched against the user agent string.
 
     :type user_agent: String
     :param user_agent: The string containing the user agent
     value that is going to be verified against a series of
     regular expressions for tablet verification.
     :rtype: bool
     :return: If the current user agent string represents a
     tablet browser or a regular (desktop) one.
     """
 
-    user_agent = flask.request.headers.get("User-Agent", "")\
-        if user_agent == None else user_agent
+    user_agent = (
+        flask.request.headers.get("User-Agent", "")
+        if user_agent == None
+        else user_agent
+    )
     prefix = user_agent[:4]
     tablet = defines.TABLET_REGEX.search(user_agent)
     mobile_prefix = defines.MOBILE_PREFIX_REGEX.search(prefix)
     is_tablet = True if tablet or mobile_prefix else False
     return is_tablet
 
-def is_browser(user_agent = None):
+
+def is_browser(user_agent=None):
     """
     Verifies if the provided user agent string represents a
     browser (interactive) agent, for that a series of verifications
     are going to be performed against the user agent string.
 
     :type user_agent: String
     :param user_agent: The string containing the user agent
     value that is going to be verified for browser presence.
     :rtype: bool
     :return: If the provided user agent string represents an
     interactive browser or not.
     """
 
-    user_agent = flask.request.headers.get("User-Agent", "")\
-        if user_agent == None else user_agent
-    info = browser_info(user_agent = user_agent)
-    if not info: return False
+    user_agent = (
+        flask.request.headers.get("User-Agent", "")
+        if user_agent == None
+        else user_agent
+    )
+    info = browser_info(user_agent=user_agent)
+    if not info:
+        return False
     interactive = info.get("interactive", False)
-    if not interactive: return False
+    if not interactive:
+        return False
     return True
 
-def is_bot(user_agent = None):
+
+def is_bot(user_agent=None):
     """
     Verifies if the provided user agent string represents a
     bot (automated) agent, for that a series of verifications
     are going to be performed against the user agent string.
 
     :type user_agent: String
     :param user_agent: The string containing the user agent
     value that is going to be verified for bot presence.
     :rtype: bool
     :return: If the provided user agent string represents an
     automated bot or not.
     """
 
-    user_agent = flask.request.headers.get("User-Agent", "")\
-        if user_agent == None else user_agent
-    info = browser_info(user_agent = user_agent)
-    if not info: return False
+    user_agent = (
+        flask.request.headers.get("User-Agent", "")
+        if user_agent == None
+        else user_agent
+    )
+    info = browser_info(user_agent=user_agent)
+    if not info:
+        return False
     bot = info.get("bot", False)
-    if not bot: return False
+    if not bot:
+        return False
     return True
 
-def browser_info(user_agent = None):
+
+def browser_info(user_agent=None):
     """
     Retrieves a dictionary containing information about the browser
     and the operative system associated with the provided user agent.
 
     The retrieval of the information depends on the kind of user
     agent string provided, as coverage is limited.
 
     :type user_agent: String
     :param user_agent: The HTTP based user agent string to be processed.
     :rtype: Dictionary
     :return: The dictionary/map containing the information processed from
     the provided user agent.
     """
 
-    user_agent = flask.request.headers.get("User-Agent", "")\
-        if user_agent == None else user_agent
+    user_agent = (
+        flask.request.headers.get("User-Agent", "")
+        if user_agent == None
+        else user_agent
+    )
 
     info = dict()
 
     for browser_i in defines.BROWSER_INFO:
         identity = browser_i["identity"]
         sub_string = browser_i.get("sub_string", identity)
         version_search = browser_i.get("version_search", sub_string + "/")
         interactive = browser_i.get("interactive", True)
         bot = browser_i.get("bot", False)
 
-        if not sub_string in user_agent: continue
-        if not version_search in user_agent: continue
+        if not sub_string in user_agent:
+            continue
+        if not version_search in user_agent:
+            continue
 
         version_i = user_agent.index(version_search) + len(version_search)
         version = user_agent[version_i:].split(" ", 1)[0].strip(" ;")
-        try: version_f = float(".".join(version.split(".")[:2]))
-        except ValueError: version_f = 0.0
-        try: version_i = int(version_f)
-        except ValueError: version_f = 0
+        try:
+            version_f = float(".".join(version.split(".")[:2]))
+        except ValueError:
+            version_f = 0.0
+        try:
+            version_i = int(version_f)
+        except ValueError:
+            version_f = 0
 
         info.update(
-            name = identity,
-            version = version,
-            version_f = version_f,
-            version_i = version_i,
-            interactive = interactive,
-            bot = bot
+            name=identity,
+            version=version,
+            version_f=version_f,
+            version_i=version_i,
+            interactive=interactive,
+            bot=bot,
         )
         break
 
     for os_i in defines.OS_INFO:
         identity = os_i["identity"]
         sub_string = os_i.get("sub_string", identity)
 
-        if not sub_string in user_agent: continue
+        if not sub_string in user_agent:
+            continue
 
-        info.update(os = identity)
+        info.update(os=identity)
         break
 
     return info if info else None
 
+
 def resolve_alias(object):
     for name, value in legacy.eager(object.items()):
-        if not name in ALIAS: continue
+        if not name in ALIAS:
+            continue
         _alias = ALIAS[name]
         object[_alias] = value
         del object[name]
 
-def page_types(object, size = 50):
+
+def page_types(object, size=50):
     page = object.get("page", 1)
     size = object.get("size", size)
     sorter = object.get("sorter", None)
     direction = object.get("direction", "descending")
     page = int(page)
     size = int(size)
     offset = page - 1
     object["skip"] = offset * size
     object["limit"] = size
-    if sorter: object["sort"] = "%s:%s" % (sorter, direction)
+    if sorter:
+        object["sort"] = "%s:%s" % (sorter, direction)
+
 
 def find_types(object):
     # iterates over all the name and values of the object
     # trying to convert each of the find types into the
     # appropriate representation for the infra-structure
     for name, value in legacy.eager(object.items()):
         # in case the current find name is not present
@@ -461,47 +515,57 @@
         # method retrieving the resulting value
         find_type = FIND_TYPES[name]
         value = find_type(value)
 
         # in case the value resulting from the conversion
         # is invalid the name is removed from the find object
         # because it's not considered to be valid
-        if value == None: del object[name]
-        else: object[name] = value
+        if value == None:
+            del object[name]
+        else:
+            object[name] = value
+
 
 def find_defaults(object, kwargs):
     for name, value in legacy.iteritems(kwargs):
-        if name in object: continue
-        if not name in FIND_TYPES: continue
+        if name in object:
+            continue
+        if not name in FIND_TYPES:
+            continue
         object[name] = value
 
     for name, value in legacy.iteritems(FIND_DEFAULTS):
-        if name in object: continue
+        if name in object:
+            continue
         object[name] = value
 
+
 def norm_object(object):
     # iterates over all the key value association in the
     # object, trying to find the ones that refer sequences
     # so that they may be normalized
     for name, value in legacy.eager(object.items()):
         # verifies if the current name references a sequence
         # and if that's not the case continues the loop trying
         # to find any other sequence based value
-        if not name.endswith("[]"): continue
+        if not name.endswith("[]"):
+            continue
 
         # removes the current reference to the name as the value
         # is not in the valid structure and then normalizes the
         # name by removing the extra sequence indication value
         del object[name]
         name = name[:-2]
 
         # in case the current value is not valid (empty) the object
         # is set with an empty list for the current iteration as this
         # is considered to be the default value
-        if not value: object[name] = []; continue
+        if not value:
+            object[name] = []
+            continue
 
         # retrieves the normalized and linearized list of leafs
         # for the current value and ten verifies the size of each
         # of its values and uses it to measure the number of
         # dictionary elements that are going to be contained in
         # the sequence to be "generated", then uses this (size)
         # value to pre-generate the complete set of dictionaries
@@ -520,14 +584,15 @@
         # are contained in the sequence (normalization process)
         for _name, _value in leafs_l:
             for index in range(size):
                 _object = list[index]
                 _name_l = _name.split(".")
                 set_object(_object, _name_l, _value[index])
 
+
 def set_object(object, name_l, value):
     """
     Sets a composite value in an object, allowing for
     dynamic setting of random size key values.
 
     This method is useful for situations where one wants
     to set a value at a randomly defined depth inside
@@ -550,25 +615,27 @@
     # retrieves the first name in the names list this is the
     # value that is going to be used for the current iteration
     name = name_l[0]
 
     # in case the length of the current names list has reached
     # one this is the final iteration and so the value is set
     # at the current naming point
-    if len(name_l) == 1: object[name] = value
+    if len(name_l) == 1:
+        object[name] = value
 
     # otherwise this is a "normal" step and so a new map must
     # be created/retrieved and the iteration step should be
     # performed on this new map as it's set on the current naming
     # place (recursion step)
     else:
         map = object.get(name, {})
         object[name] = map
         set_object(map, name_l[1:], value)
 
+
 def leafs(object):
     """
     Retrieves a list containing a series of tuples that
     each represent a leaf of the current object structure.
 
     A leaf is the last element of an object that is not a
     map, the other intermediary maps are considered to be
@@ -606,21 +673,23 @@
             leafs_l.extend(_leafs)
 
         # otherwise this is a leaf node and so the leaf tuple
         # node must be constructed with the current value
         # (properly validated for sequence presence)
         else:
             value_t = type(value)
-            if not value_t == list: value = [value]
+            if not value_t == list:
+                value = [value]
             leafs_l.append((name, value))
 
     # returns the list of leaf nodes that was "just" created
     # to the caller method so that it may be used there
     return leafs_l
 
+
 def load_form(form):
     # creates the map that is going to hold the "structured"
     # version of the form with key value associations
     form_s = dict()
 
     # iterates over all the form items to parse their values
     # and populate the form structured version of it, note that
@@ -629,16 +698,17 @@
     # same name they are considered as a list, otherwise they are
     # considered as a single value
     for name in form:
         # retrieves the value (as a list) for the current name, then
         # in case the sequence is larger than one element sets it,
         # otherwise retrieves and sets the value as the first element
         value = form.getlist(name)
-        value = value[0] if isinstance(value, (list, tuple)) and\
-            len(value) == 1 else value
+        value = (
+            value[0] if isinstance(value, (list, tuple)) and len(value) == 1 else value
+        )
 
         # splits the complete name into its various components
         # and retrieves both the final (last) element and the
         # various partial elements from it
         names = name.split(".")
         final = names[-1]
         partials = names[:-1]
@@ -658,120 +728,143 @@
         struct[final] = value
 
     # retrieves the final "normalized" form structure containing
     # a series of chained maps resulting from the parsing of the
     # linear version of the attribute names
     return form_s
 
-def load_locale(available, fallback = "en_us"):
+
+def load_locale(available, fallback="en_us"):
     # tries to gather the best locale value using the currently
     # available strategies and in case the retrieved local is part
     # of the valid locales for the app returns the locale, otherwise
     # returns the fallback value instead
-    locale = get_locale(fallback = fallback)
+    locale = get_locale(fallback=fallback)
     language = locale.split("_", 1)[0]
-    if locale in available: return locale
-    if language in available: return locale
+    if locale in available:
+        return locale
+    if language in available:
+        return locale
     return fallback
 
-def get_locale(fallback = "en_us"):
+
+def get_locale(fallback="en_us"):
     # tries to retrieve the locale value from the provided URL
     # parameters (this is the highest priority) and in case it
     # exists returns this locale immediately
     locale = flask.request.args.get("locale", None)
-    if locale: return locale
+    if locale:
+        return locale
 
     # uses the currently loaded session to try to gather the locale
     # value from it and in case it's valid and exists returns it
     locale = flask.session.get("locale", None)
-    if locale: return locale
+    if locale:
+        return locale
 
     # gathers the complete set of language values set in the accept
     # language header and in case there's at least one value returned
     # returns the first of these values as the locale
     langs = get_langs()
-    if langs: return langs[0]
+    if langs:
+        return langs[0]
 
     # in case this code entry is reached all the strategies for locale
     # retrieval have failed and so the fallback value is returned
     return fallback
 
+
 def get_langs():
     # gathers the value of the accept language header and in case
     # it's not defined returns immediately as no language can be
     # determined using the currently provided headers
     accept_language = flask.request.headers.get("Accept-Language", None)
-    if not accept_language: return ()
+    if not accept_language:
+        return ()
 
     # starts the list that is going to be used to store the various
     # languages "recovered" from the accept language header, note that
     # the order of these languages should be from the most relevant to
     # the least relevant as defined in HTTP specification
     langs = []
 
     # splits the accept language header into the various components of
     # it and then iterates over each of them splitting each of the
     # components into the proper language string and priority
     parts = accept_language.split(",")
     for part in parts:
         values = part.split(";", 1)
         value_l = len(values)
-        if value_l == 1: lang, = values
-        else: lang, _priority = values
+        if value_l == 1:
+            (lang,) = values
+        else:
+            lang, _priority = values
         lang = lang.replace("-", "_")
         lang = lang.lower()
         langs.append(lang)
 
     # returns the complete list of languages that have been extracted
     # from the accept language header these list may be empty in case
     # the header was not parsed correctly or there's no contents in it
     return langs
 
+
 def set_locale():
     # normalizes the current locale string by converting the
     # last part of the locale string to an uppercase representation
     # and then re-joining the various components of it
-    values = flask.request.locale.split("_", 1) #@UndefinedVariable
-    if len(values) > 1: values[1] = values[1].upper()
+    values = flask.request.locale.split("_", 1)  # @UndefinedVariable
+    if len(values) > 1:
+        values[1] = values[1].upper()
     locale_n = "_".join(values)
     locale_n = str(locale_n)
 
     # in case the current operative system is windows based an
     # extra locale conversion operation must be performed, after
     # than the proper setting of the os locale is done with the
     # fallback for exception being silent (non critical)
-    if os.name == "nt": locale_n = defines.WINDOWS_LOCALE.get(locale_n, "")
-    else: locale_n += ".utf8"
-    try: locale.setlocale(locale.LC_ALL, locale_n)
-    except Exception: pass
+    if os.name == "nt":
+        locale_n = defines.WINDOWS_LOCALE.get(locale_n, "")
+    else:
+        locale_n += ".utf8"
+    try:
+        locale.setlocale(locale.LC_ALL, locale_n)
+    except Exception:
+        pass
+
 
 def reset_locale():
     locale.setlocale(locale.LC_ALL, "")
 
+
 def anotate_async(response):
     # verifies if the current response contains the location header
     # meaning that a redirection will occur, and if that's not the
     # case this function returns immediately to avoid problems
-    if not "Location" in response.headers: return
+    if not "Location" in response.headers:
+        return
 
     # checks if the current request is "marked" as asynchronous, for
     # such cases a special redirection process is applies to avoid the
     # typical problems with automated redirection using "ajax"
     is_async = True if flask.request.headers.get("X-Async") else False
     is_async = True if get_field("async") else is_async
-    if is_async: response.status_code = 280
+    if is_async:
+        response.status_code = 280
+
 
 def anotate_secure(response):
     # retrieves the reference to the master application object to be used
     # in some of the verification
     app = common.base().APP
 
     # verifies if the secure headers flag is set in the current application
     # and if that's not the case returns the control flow immediately
-    if not app.secure_headers: return
+    if not app.secure_headers:
+        return
 
     # sets the multiple secure header values taking into account if they
     # are defined or not in the current application context
     if app.allow_origin:
         response.headers["Access-Control-Allow-Origin"] = app.allow_origin
     if app.allow_headers:
         response.headers["Access-Control-Allow-Headers"] = app.allow_headers
@@ -782,22 +875,20 @@
     if app.frame_options:
         response.headers["X-Frame-Options"] = app.frame_options
     if app.xss_protection:
         response.headers["X-XSS-Protection"] = app.xss_protection
     if app.content_options:
         response.headers["X-Content-Type-Options"] = app.content_options
 
+
 def run_thread(function, *args, **kwargs):
-    return threading.Thread(
-        target = function,
-        args = args,
-        kwargs = kwargs
-    ).start()
+    return threading.Thread(target=function, args=args, kwargs=kwargs).start()
+
 
-def camel_to_underscore(camel, separator = "_", lower = True):
+def camel_to_underscore(camel, separator="_", lower=True):
     """
     Converts the provided camel cased based value into
     a normalized underscore based string.
 
     An optional lower parameter may be used to avoid the case
     of the letters from being lower cased.
 
@@ -814,21 +905,24 @@
     :param lower: If the letter casing should be changed while
     convert the value from camel to underscore.
     :rtype: String
     :return: The underscore based string resulting from the
     conversion of the provided camel cased one.
     """
 
-    if not camel: return camel
+    if not camel:
+        return camel
     value = FIRST_CAP_REGEX.sub(r"\1" + separator + r"\2", camel)
     value = ALL_CAP_REGEX.sub(r"\1" + separator + r"\2", value)
-    if lower: value = value.lower()
+    if lower:
+        value = value.lower()
     return value
 
-def camel_to_readable(camel, lower = False, capitalize = False):
+
+def camel_to_readable(camel, lower=False, capitalize=False):
     """
     Converts the given camel cased oriented string value
     into a readable one meaning that the returned value
     is a set of strings separated by spaces.
 
     This method may be used to convert class names into
     something that is readable by an end user.
@@ -843,19 +937,21 @@
     :param capitalize: If all of the words should be capitalized
     or if instead only the first one should.
     :rtype: String
     :return: The final human readable string that may be
     used to display a value to an end user.
     """
 
-    if not camel: return camel
-    underscore = camel_to_underscore(camel, lower = lower)
-    return underscore_to_readable(underscore, capitalize = capitalize)
+    if not camel:
+        return camel
+    underscore = camel_to_underscore(camel, lower=lower)
+    return underscore_to_readable(underscore, capitalize=capitalize)
 
-def underscore_to_camel(underscore, lower = False):
+
+def underscore_to_camel(underscore, lower=False):
     """
     Converts the provided underscore cased based value into
     a normalized camel cased string.
     An optional lower parameter may be provided to obtain a
     lower came case version of the string.
     This is useful as most of the python string standards
     are compliant with the underscore strategy.
@@ -866,20 +962,23 @@
     :param lower: If the the first letter of the resulting camel
     case string should be lower case (lower camel case).
     :rtype: String
     :return: The camel case based string resulting from the
     conversion of the provided underscore cased one.
     """
 
-    if not underscore: return underscore
-    camel = underscore_to_readable(underscore, capitalize = True, separator = "")
-    if not lower: return camel
+    if not underscore:
+        return underscore
+    camel = underscore_to_readable(underscore, capitalize=True, separator="")
+    if not lower:
+        return camel
     return camel[0].lower() + camel[1:]
 
-def underscore_to_readable(underscore, capitalize = False, separator = " "):
+
+def underscore_to_readable(underscore, capitalize=False, separator=" "):
     """
     Converts the given underscore oriented string value
     into a readable one meaning that the returned value
     is a set of strings separated by spaces.
 
     This method may be used to class attributes into
     something that is readable by an end user.
@@ -894,22 +993,26 @@
     :param separator: The separator to be used to join the multiple
     parts of the resulting readable tokens.
     :rtype: String
     :return: The final human readable string that may be
     used to display a value to an end user.
     """
 
-    if not underscore: return underscore
+    if not underscore:
+        return underscore
     parts = underscore.split("_")
     parts = [part for part in parts if part]
-    if capitalize: parts = [part[0].upper() + part[1:] for part in parts]
-    else: parts[0] = parts[0][0].upper() + parts[0][1:]
+    if capitalize:
+        parts = [part[0].upper() + part[1:] for part in parts]
+    else:
+        parts[0] = parts[0][0].upper() + parts[0][1:]
     return separator.join(parts)
 
-def generate_identifier(size = 16, chars = string.ascii_uppercase + string.digits):
+
+def generate_identifier(size=16, chars=string.ascii_uppercase + string.digits):
     """
     Generates a random identifier (may be used as password) with
     the provided constrains of length and character ranges.
 
     This function may be used in the generation of random based
     keys for both passwords and API keys.
 
@@ -922,15 +1025,16 @@
     :rtype: String
     :return: The randomly generated identifier obeying to the
     provided constrains.
     """
 
     return "".join(random.choice(chars) for _index in range(size))
 
-def to_locale(value, locale = None, default = None, fallback = True):
+
+def to_locale(value, locale=None, default=None, fallback=True):
     """
     Utility function used to localize the provided value according
     to the currently loaded set of bundles, the bundles are loaded
     at the application start time from the proper sources.
 
     The (target) locale value for the translation may be provided or
     in case it's not the locale associated with the current request
@@ -956,41 +1060,41 @@
     :rtype: String
     :return: The localized value for the current environment or the
     proper (original) value in case no localization was possible.
     """
 
     value_t = type(value)
     is_sequence = value_t in (list, tuple)
-    if is_sequence: return _serialize([
-        to_locale(
-            value,
-            locale = locale,
-            default = default,
-            fallback = fallback
-        ) for value in value
-    ])
+    if is_sequence:
+        return _serialize(
+            [
+                to_locale(value, locale=locale, default=default, fallback=fallback)
+                for value in value
+            ]
+        )
     has_context = common.base().has_context()
-    locale = locale or (flask.request.locale if has_context else None) #@UndefinedVariable
+    locale = locale or (
+        flask.request.locale if has_context else None
+    )  # @UndefinedVariable
     if locale:
         bundle = common.base().get_bundle(locale) or {}
         result = bundle.get(value, None)
-        if not result == None: return result
+        if not result == None:
+            return result
         language = locale.split("_", 1)[0]
         bundle = common.base().get_bundle(language) or {}
         result = bundle.get(value, None)
-        if not result == None: return result
+        if not result == None:
+            return result
     app = common.base().APP
-    if fallback and app: return to_locale(
-        value,
-        locale = app._locale_d,
-        default = default,
-        fallback = False
-    )
+    if fallback and app:
+        return to_locale(value, locale=app._locale_d, default=default, fallback=False)
     return value if default == None else default
 
+
 def nl_to_br(value):
     """
     Replaces the occurrences of the newline character in the
     string with the HTML break line character.
 
     This is useful for one trying to convert a plain text
     representation of a string into HTML representation.
@@ -1001,14 +1105,15 @@
     :rtype: String
     :return: The string containing the newline characters replaced
     with line breaking HTML tags.
     """
 
     return value.replace("\n", "<br/>\n")
 
+
 def nl_to_br_jinja(eval_ctx, value):
     """
     Optimized version of the function that replaces newline
     characters with the HTML break lines that handles the
     autoescape properties of the jinja engine.
 
     :type eval_ctx: Context
@@ -1019,19 +1124,22 @@
     :param value: The base value that is going to be used in
     the conversion to the html value.
     :rtype: String
     :return: The string containing the newline characters replaced
     with line breaking HTML tags.
     """
 
-    if eval_ctx.autoescape: value = legacy.UNICODE(jinja2.escape(value))
+    if eval_ctx.autoescape:
+        value = legacy.UNICODE(jinja2.escape(value))
     value = nl_to_br(value)
-    if eval_ctx.autoescape: value = jinja2.Markup(value)
+    if eval_ctx.autoescape:
+        value = jinja2.Markup(value)
     return value
 
+
 def sp_to_nbsp(value):
     """
     Replaces the occurrences of the space character in the
     string with the HTML non breaking space character.
 
     This is useful for one trying to convert a plain text
     representation of a string into HTML representation.
@@ -1042,14 +1150,15 @@
     :rtype: String
     :return: The string containing the space characters replaced
     with non breaking space characters for HTML.
     """
 
     return value.replace(" ", "&nbsp;")
 
+
 def sp_to_nbsp_jinja(eval_ctx, value):
     """
     Optimized version of the function that replaces space
     characters with the HTML non breaking space characters
     that handles the autoescape properties of the jinja engine.
 
     :type eval_ctx: Context
@@ -1060,20 +1169,23 @@
     :param value: The base value that is going to be used in
     the conversion to the HTML value.
     :rtype: String
     :return: The string containing the space characters replaced
     with non breaking space characters for HTML.
     """
 
-    if eval_ctx.autoescape: value = legacy.UNICODE(jinja2.escape(value))
+    if eval_ctx.autoescape:
+        value = legacy.UNICODE(jinja2.escape(value))
     value = sp_to_nbsp(value)
-    if eval_ctx.autoescape: value = jinja2.Markup(value)
+    if eval_ctx.autoescape:
+        value = jinja2.Markup(value)
     return value
 
-def unset(value, default = "", empty = False, extra = ()):
+
+def unset(value, default="", empty=False, extra=()):
     """
     Verifies if the provided value is not unset (by default) testing
     it against the unset and None values.
 
     If an extra set of values is provided does values are also going
     to be used in the comparison against the unset value.
 
@@ -1089,22 +1201,28 @@
     :type extra: Tuple
     :param extra: A tuple that represents the multiple values that are
     going to be considered to be unset ones.
     :rtype: String
     :return: The processed string value according to the unset validation.
     """
 
-    if empty and extra: extra = tuple(list(extra) + [""])
-    elif empty and not extra: extra = ("",)
-    if isinstance(value, jinja2.Undefined): return default
-    if value in (None,): return default
-    if value in extra: return default
+    if empty and extra:
+        extra = tuple(list(extra) + [""])
+    elif empty and not extra:
+        extra = ("",)
+    if isinstance(value, jinja2.Undefined):
+        return default
+    if value in (None,):
+        return default
+    if value in extra:
+        return default
     return value
 
-def date_time(value, format = "%d/%m/%Y"):
+
+def date_time(value, format="%d/%m/%Y"):
     """
     Formats the value provided as a date string according to the
     provided date format.
 
     Assumes that the provided value represents a float string
     and that may be used as the based timestamp for conversion.
 
@@ -1119,25 +1237,28 @@
     :return: The resulting date time string that may be used
     to represent the provided value.
     """
 
     # tries to convert the provided string value into a float
     # in case it fails the proper string value is returned
     # immediately as a fallback procedure
-    try: value_f = float(value)
-    except Exception: return value
+    try:
+        value_f = float(value)
+    except Exception:
+        return value
 
     # creates the date time structure from the provided float
     # value and then formats the date time according to the
     # provided format and returns the resulting string
     date_time_s = datetime.datetime.utcfromtimestamp(value_f)
     date_time_s = date_time_s.strftime(format)
     is_unicode = legacy.is_unicode(date_time_s)
     return date_time_s if is_unicode else date_time_s.decode("utf-8")
 
+
 def quote(value, *args, **kwargs):
     """
     Quotes the passed value according to the defined
     standard for URL escaping, the value is first encoded
     into the expected UTF-8 encoding as defined by standard.
 
     This method should be used instead of a direct call to
@@ -1148,17 +1269,19 @@
     according to the URL escaping scheme.
     :rtype: String
     :return: The quoted value according to the URL scheme this
     value may be safely used in urls.
     """
 
     is_unicode = isinstance(value, legacy.UNICODE)
-    if is_unicode: value = value.encode("utf-8")
+    if is_unicode:
+        value = value.encode("utf-8")
     return legacy.quote(value, *args, **kwargs)
 
+
 def unquote(value, *args, **kwargs):
     """
     Unquotes the provided value according to the URL scheme
     the resulting value should be an unicode string representing
     the same value, the intermediary string value from the decoding
     should be an UTF-8 based value.
 
@@ -1171,18 +1294,20 @@
     :rtype: String
     :return: The unquoted value extracted as an unicode
     string that the represents the same value.
     """
 
     value = legacy.unquote(value, *args, **kwargs)
     is_bytes = type(value) == legacy.BYTES
-    if is_bytes: value = value.decode("utf-8")
+    if is_bytes:
+        value = value.decode("utf-8")
     return value
 
-def escape(value, char, escape = "\\"):
+
+def escape(value, char, escape="\\"):
     """
     Escapes the provided string value according to the requested
     target character and escape value. Meaning that all the characters
     are going to be replaced by the escape plus character sequence.
 
     :type value: String
     :param value: The string that is going to have the target characters
@@ -1193,15 +1318,16 @@
     :param escape: The character to be used for escaping (normally`\`).
     :rtype: String
     :return: The final string with the target character properly escaped.
     """
 
     return value.replace(escape, escape + escape).replace(char, escape + char)
 
-def unescape(value, escape = "\\"):
+
+def unescape(value, escape="\\"):
     """
     Unescapes the provided string value using the provided escape
     character as the reference for the unescape operation.
 
     This is considered to be a very expensive operation and so it
     should be used carefully.
 
@@ -1219,15 +1345,16 @@
                 result.append(next(iterator))
             except StopIteration:
                 result.append(escape)
         else:
             result.append(char)
     return "".join(result)
 
-def count_unescape(value, sub, escape = "\\"):
+
+def count_unescape(value, sub, escape="\\"):
     """
     Runs the sub string count operation on an escaped string
     so that it takes into account the escaped values avoiding
     them for the count operation.
 
     :type value: String
     :param value: The base string value to have the number of
@@ -1251,15 +1378,16 @@
                 next(iterator)
             except StopIteration:
                 pass
         elif char == sub:
             count += 1
     return count
 
-def split_unescape(value, delimiter = " ", max = -1, escape = "\\", unescape = True):
+
+def split_unescape(value, delimiter=" ", max=-1, escape="\\", unescape=True):
     """
     Splits the provided string around the delimiter character that
     has been provided and allows proper escaping of it using the
     provided escape character.
 
     This is considered to be a very expensive operation when compared
     to the simple split operation and so it should be used carefully.
@@ -1287,27 +1415,30 @@
     result = []
     current = []
     iterator = iter(value)
     count = 0
     for char in iterator:
         if char == escape:
             try:
-                if not unescape: current.append(escape)
+                if not unescape:
+                    current.append(escape)
                 current.append(next(iterator))
             except StopIteration:
-                if unescape: current.append(escape)
+                if unescape:
+                    current.append(escape)
         elif char == delimiter and not count == max:
             result.append("".join(current))
             current = []
             count += 1
         else:
             current.append(char)
     result.append("".join(current))
     return result
 
+
 def is_content_type(data, target):
     """
     Verifies if the any of the provided mime types (target) is
     valid for the provided content type string.
 
     :type data: String
     :param data: The content type string to be parsed and matched
@@ -1316,23 +1447,27 @@
     :param target: The tuple containing the multiple mime type values
     to be verified against the content type mime strings.
     :rtype: bool
     :return: If any of the provided mime types is considered valid
     for the content type.
     """
 
-    if not isinstance(target, (list, tuple)): target = (target,)
+    if not isinstance(target, (list, tuple)):
+        target = (target,)
     mime, _extra = parse_content_type(data)
     for item in target:
         type, _sub_type = item.split("/")
         wildcard = type + "/*"
-        if item in mime: return True
-        if wildcard in mime: return True
+        if item in mime:
+            return True
+        if wildcard in mime:
+            return True
     return False
 
+
 def parse_content_type(data):
     """
     Parses the provided content type string retrieving both the multiple
     mime types associated with the resource and the extra key to value
     items associated with the string in case they are defined (it's optional).
 
     :type data: String
@@ -1347,27 +1482,29 @@
     # creates the list of final normalized mime types and the
     # dictionary to store the extra values.
     types = []
     extra_m = dict()
 
     # in case no valid type has been sent returns the values
     # immediately to avoid further problems
-    if not data: return types, extra_m
+    if not data:
+        return types, extra_m
 
     # extracts the mime and the extra parts from the data string
     # they are the basis of the processing method
     data = data.strip(";")
     parts = data.split(";")
     mime = parts[0]
     extra = parts[1:]
     mime = mime.strip()
 
     # runs a series of verifications on the base mime value and in
     # case it's not valid returns the default values immediately
-    if not "/" in mime: return types, extra_m
+    if not "/" in mime:
+        return types, extra_m
 
     # strips the complete set of valid extra values, note
     # that these values are going to be processed as key
     # to value items
     extra = [value.strip() for value in extra if extra]
 
     # splits the complete mime type into its type and sub
@@ -1380,95 +1517,84 @@
     # add the new full items to the types list (normalization)
     for sub_type in sub_types:
         types.append(type + "/" + sub_type)
 
     # goes through all of the extra key to value items
     # and converts them into proper dictionary values
     for extra_item in extra:
-        if not "=" in extra_item: continue
+        if not "=" in extra_item:
+            continue
         extra_item = extra_item.strip()
         key, value = extra_item.split("=")
         extra_m[key] = value
 
     # returns the final tuple containing both the normalized
     # mime types for the content and the extra key to value items
     return types, extra_m
 
-def verify(condition, message = None, code = None, exception = None, **kwargs):
-    if condition: return
+
+def verify(condition, message=None, code=None, exception=None, **kwargs):
+    if condition:
+        return
     exception = exception or exceptions.AssertionError
     kwargs = dict(kwargs)
-    if not code == None: kwargs["code"] = code
-    raise exception(
-        message or "Assertion of data failed",
-        **kwargs
-    )
+    if not code == None:
+        kwargs["code"] = code
+    raise exception(message or "Assertion of data failed", **kwargs)
 
-def verify_equal(first, second, message = None, code = None, exception = None, **kwargs):
+
+def verify_equal(first, second, message=None, code=None, exception=None, **kwargs):
     message = message or "Expected %s got %s" % (repr(second), repr(first))
     return verify(
-        first == second,
-        message = message,
-        code = code,
-        exception = exception,
-        **kwargs
+        first == second, message=message, code=code, exception=exception, **kwargs
     )
 
-def verify_not_equal(first, second, message = None, code = None, exception = None, **kwargs):
+
+def verify_not_equal(first, second, message=None, code=None, exception=None, **kwargs):
     message = message or "Expected %s not equal to %s" % (repr(first), repr(second))
     return verify(
-        not first == second,
-        message = message,
-        code = code,
-        exception = exception,
-        **kwargs
+        not first == second, message=message, code=code, exception=exception, **kwargs
     )
 
-def verify_type(value, types, null = True, message = None, code = None, exception = None, **kwargs):
+
+def verify_type(
+    value, types, null=True, message=None, code=None, exception=None, **kwargs
+):
     message = message or "Expected %s to have type %s" % (repr(value), repr(types))
     return verify(
         (null and value == None) or isinstance(value, types),
-        message = message,
-        code = code,
-        exception = exception,
+        message=message,
+        code=code,
+        exception=exception,
         **kwargs
     )
 
-def verify_many(sequence, message = None, code = None, exception = None, **kwargs):
+
+def verify_many(sequence, message=None, code=None, exception=None, **kwargs):
     for condition in sequence:
-        verify(
-            condition,
-            message = message,
-            code = code,
-            exception = exception,
-            **kwargs
-        )
+        verify(condition, message=message, code=code, exception=exception, **kwargs)
+
 
-def execute(args, command = None, path = None, shell = True, encoding = None):
-    if not encoding: encoding = sys.getfilesystemencoding()
-    if command: args = command.split(" ")
+def execute(args, command=None, path=None, shell=True, encoding=None):
+    if not encoding:
+        encoding = sys.getfilesystemencoding()
+    if command:
+        args = command.split(" ")
     process = subprocess.Popen(
-        args,
-        stdout = subprocess.PIPE,
-        stderr = subprocess.PIPE,
-        shell = shell,
-        cwd = path
+        args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=shell, cwd=path
     )
     code = process.wait()
     stdout = process.stdout.read()
     stderr = process.stderr.read()
     stdout = stdout.decode(encoding)
     stderr = stderr.decode(encoding)
-    return dict(
-        stdout = stdout,
-        stderr = stderr,
-        code = code
-    )
+    return dict(stdout=stdout, stderr=stderr, code=code)
 
-def deprecated(message = "Function %s is now deprecated"):
+
+def deprecated(message="Function %s is now deprecated"):
     """
     Decorator that marks a certain function or method as
     deprecated so that whenever such function is called
     an output messaged warns the developer about the
     deprecation (incentive).
 
     :type message: String
@@ -1482,33 +1608,34 @@
     def decorator(function):
 
         name = function.__name__ if hasattr(function, "__name__") else None
 
         @functools.wraps(function)
         def interceptor(*args, **kwargs):
             warnings.simplefilter("always", DeprecationWarning)
-            warnings.warn(
-                message % name,
-                category = DeprecationWarning,
-                stacklevel = 2
-            )
+            warnings.warn(message % name, category=DeprecationWarning, stacklevel=2)
             warnings.simplefilter("default", DeprecationWarning)
             return function(*args, **kwargs)
 
         return interceptor
 
     return decorator
 
+
 def _serialize(value):
-    if value in legacy.STRINGS: return value
+    if value in legacy.STRINGS:
+        return value
     return json.dumps(value)
 
+
 class JSONEncoder(json.JSONEncoder):
 
     def __init__(self, *args, **kwargs):
         self.permissive = kwargs.pop("permissive", True)
         json.JSONEncoder.__init__(self, *args, **kwargs)
 
     def default(self, obj, **kwargs):
-        if hasattr(obj, "json_v"): return obj.json_v()
-        if self.permissive: return str(obj)
+        if hasattr(obj, "json_v"):
+            return obj.json_v()
+        if self.permissive:
+            return str(obj)
         return json.JSONEncoder.default(self, obj, **kwargs)
```

### Comparing `quorum-0.8.2/src/quorum/route.py` & `quorum-0.8.3/src/quorum/route.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
@@ -44,131 +35,132 @@
 from . import log
 from . import model
 from . import common
 from . import legacy
 from . import mongodb
 from . import exceptions
 
+
 def route(*args, **kwargs):
     # verifies if the request decorator should be of type
     # JSON serializer in case it should not returns the old
     # route decorator (default behavior)
     is_json = kwargs.get("json", False)
-    if not is_json: return common.base().APP.old_route(*args, **kwargs)
+    if not is_json:
+        return common.base().APP.old_route(*args, **kwargs)
 
     # removes the JSON keyword argument from the list of arguments
     # (to avoid errors) and then calls the old route method to obtain
     # the "normal" decorator
     del kwargs["json"]
     decorator = common.base().APP.old_route(*args, **kwargs)
 
     # creates the "new" route decorator maker method that should
     # override the old one and create a new decorator that
     # serializes all the unhandled exceptions as JSON
     def _route(function):
         def _decorator(*args, **kwargs):
-            try: result = function(*args, **kwargs)
+            try:
+                result = function(*args, **kwargs)
             except exceptions.OperationalError as exception:
                 # runs the default handling of the user exception in the flask
                 # infra-structure so that the proper exception callbacks are called
                 # in case they exist and are properly registered
                 common.base().APP.handle_user_exception(exception)
 
                 # prints a warning message to the current logger about the exception
                 # that is being handled, note that the traceback is also logger, allowing
                 # further debugging information to be printed (extra traceability)
                 log.info(
-                    "Operational problem while routing request - %s" % legacy.UNICODE(exception),
-                    log_trace = True
+                    "Operational problem while routing request - %s"
+                    % legacy.UNICODE(exception),
+                    log_trace=True,
                 )
 
                 # retrieves the formatted version of the traceback information and then
                 # splits this information into the various lines that are contained in it
                 formatted = traceback.format_exc()
                 lines = formatted.splitlines()
 
                 # creates a new response object containing the information about the exception
                 # this is going to include the proper exception message, code and also the set
                 # of lines that compose the traceback of the exception
                 return flask.Response(
-                    json.dumps({
-                        "exception" : {
-                            "name" : exception.__class__.__name__,
-                            "message" : exception.message,
-                            "code" : exception.code,
-                            "traceback" : lines
+                    json.dumps(
+                        {
+                            "exception": {
+                                "name": exception.__class__.__name__,
+                                "message": exception.message,
+                                "code": exception.code,
+                                "traceback": lines,
+                            }
                         }
-                    }),
-                    status = exception.code,
-                    mimetype = "application/json"
+                    ),
+                    status=exception.code,
+                    mimetype="application/json",
                 )
             except Exception as exception:
                 # runs the default handling of the user exception in the flask
                 # infra-structure so that the proper exception callbacks are called
                 # in case they exist and are properly registered
                 common.base().APP.handle_user_exception(exception)
 
                 # prints a warning message to the current logger about the exception
                 # that is being handled, note that the traceback is also logger, allowing
                 # further debugging information to be printed (extra traceability)
                 log.warning(
                     "Problem while routing request - %s" % legacy.UNICODE(exception),
-                    log_trace = True
+                    log_trace=True,
                 )
 
                 # retrieves the formatted version of the traceback information and then
                 # splits this information into the various lines that are contained in it
                 formatted = traceback.format_exc()
                 lines = formatted.splitlines()
 
                 # creates the response object that is going to be returned to the client indicating
                 # that an undefined exception has just been raised, note that the error code
                 # is the internal server error one (undefined exception)
                 return flask.Response(
-                    json.dumps({
-                        "exception" : {
-                            "name" : exception.__class__.__name__,
-                            "message" : str(exception),
-                            "code" : 500,
-                            "traceback" : lines
+                    json.dumps(
+                        {
+                            "exception": {
+                                "name": exception.__class__.__name__,
+                                "message": str(exception),
+                                "code": 500,
+                                "traceback": lines,
+                            }
                         }
-                    }),
-                    status = 500,
-                    mimetype = "application/json"
+                    ),
+                    status=500,
+                    mimetype="application/json",
                 )
 
             # retrieves the type for the result that was returned from the
             # concrete method and in case the result is either a MongoDB object,
             # a dictionary or a sequence it's serialized as JSON, then returns
             # the result to the caller method
             result_t = type(result)
             if isinstance(result, model.Model):
-                result = flask.Response(
-                    json.dumps(result),
-                    mimetype = "application/json"
-                )
+                result = flask.Response(json.dumps(result), mimetype="application/json")
             elif mongodb.is_mongo(result):
-                result = flask.Response(
-                    json.dumps(result),
-                    mimetype = "application/json"
-                )
+                result = flask.Response(json.dumps(result), mimetype="application/json")
             elif result_t in (dict, list, tuple, type(None)):
-                result = flask.Response(
-                    json.dumps(result),
-                    mimetype = "application/json"
-                )
+                result = flask.Response(json.dumps(result), mimetype="application/json")
             return result
 
         # verifies if the base value is set in the function for such
         # situations (double decoration) the base value should be set
         # as the already existing base decorator method otherwise keeps
         # using the clojure based one
         has_base = hasattr(function, "_base")
-        if has_base: _base = function._base
-        else: _base = _decorator
+        if has_base:
+            _base = function._base
+        else:
+            _base = _decorator
 
         # updates the decorates with the base value, this is going to be
         # the clojure based new view function, then in case this is a new
         # decorator updates the name of the decorator name with the name
         # of the base function (view function) that is getting decorated
         # so that the original name persists (otherwise a problem would
         # occur in werkzeug)
```

### Comparing `quorum-0.8.2/src/quorum/config.py` & `quorum-0.8.3/src/quorum/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -56,27 +47,23 @@
 the home directory contents to a different directory """
 
 IMPORT_NAMES = ("$import", "$include", "$IMPORT", "$INCLUDE")
 """ The multiple possible definitions of the special configuration
 name that references a list of include files to be loaded """
 
 CASTS = {
-    bool : lambda v: v if isinstance(v, bool) else v in ("1", "true", "True"),
-    list : lambda v: v if isinstance(v, list) else v.split(";") if v else [],
-    tuple : lambda v: v if isinstance(v, tuple) else tuple(v.split(";") if v else [])
+    bool: lambda v: v if isinstance(v, bool) else v in ("1", "true", "True"),
+    list: lambda v: v if isinstance(v, list) else v.split(";") if v else [],
+    tuple: lambda v: v if isinstance(v, tuple) else tuple(v.split(";") if v else []),
 }
 """ The map containing the various cast method
 operation associated with the various data types,
 they provide a different type of casting strategy """
 
-ENV_ENCODINGS = (
-    "utf-8",
-    sys.getdefaultencoding(),
-    sys.getfilesystemencoding()
-)
+ENV_ENCODINGS = ("utf-8", sys.getdefaultencoding(), sys.getfilesystemencoding())
 """ The sequence of encodings that are going to
 be used to try to decode possible byte based strings
 for the various environment variable values """
 
 config_g = {}
 """ The map containing the various global wide
 configuration for the current application """
@@ -91,185 +78,219 @@
 """ Global reference to the paths to the directory considered
 to be the home on in terms of configuration, this value should
 be set on the initial loading of the ".home" file """
 
 if not isinstance(__builtins__, dict):
     __builtins__ = __builtins__.__dict__
 
-def conf(name, default = None, cast = None, ctx = None):
+
+def conf(name, default=None, cast=None, ctx=None):
     config = ctx["config"] if ctx else config_g
     cast = _cast_r(cast)
     value = config.get(name, default)
-    if cast and not value == None: value = cast(value)
+    if cast and not value == None:
+        value = cast(value)
     return value
 
-def conf_prefix(prefix, ctx = None):
+
+def conf_prefix(prefix, ctx=None):
     config = ctx["config"] if ctx else config_g
     config_prefix = dict()
     for name, value in config.items():
-        if not name.startswith(prefix): continue
+        if not name.startswith(prefix):
+            continue
         config_prefix[name] = value
     return config_prefix
 
-def conf_suffix(suffix, ctx = None):
+
+def conf_suffix(suffix, ctx=None):
     config = ctx["config"] if ctx else config_g
     config_suffix = dict()
     for name, value in config.items():
-        if not name.endswith(suffix): continue
+        if not name.endswith(suffix):
+            continue
         config_suffix[name] = value
     return config_suffix
 
-def confs(name, value, ctx = None):
+
+def confs(name, value, ctx=None):
     config = ctx["config"] if ctx else config_g
     config[name] = value
 
-def confr(name, ctx = None):
+
+def confr(name, ctx=None):
     config = ctx["config"] if ctx else config_g
-    if not name in config: return
+    if not name in config:
+        return
     del config[name]
 
-def confd(ctx = None):
+
+def confd(ctx=None):
     config = ctx["config"] if ctx else config_g
     return config
 
+
 def confctx():
-    return dict(config = dict(), config_f = dict())
+    return dict(config=dict(), config_f=dict())
 
-def load(names = (FILE_NAME,), path = None, encoding = "utf-8", ctx = None):
+
+def load(names=(FILE_NAME,), path=None, encoding="utf-8", ctx=None):
     paths = []
     homes = get_homes()
     for home in homes:
         paths += [
             os.path.join(home),
             os.path.join(home, ".config"),
         ]
     paths += [sys.prefix]
     paths.append(path)
     for path in paths:
         for name in names:
-            load_file(name = name, path = path, encoding = encoding, ctx = ctx)
-    load_env(ctx = ctx)
+            load_file(name=name, path=path, encoding=encoding, ctx=ctx)
+    load_env(ctx=ctx)
+
 
-def load_file(name = FILE_NAME, path = None, encoding = "utf-8", ctx = None):
+def load_file(name=FILE_NAME, path=None, encoding="utf-8", ctx=None):
     config = ctx["config"] if ctx else config_g
     _config_f = ctx["config_f"] if ctx else config_f
 
-    if path: path = os.path.normpath(path)
-    if path: file_path = os.path.join(path, name)
-    else: file_path = name
+    if path:
+        path = os.path.normpath(path)
+    if path:
+        file_path = os.path.join(path, name)
+    else:
+        file_path = name
 
     file_path = os.path.abspath(file_path)
     file_path = os.path.normpath(file_path)
     base_path = os.path.dirname(file_path)
 
     exists = os.path.exists(file_path)
-    if not exists: return
+    if not exists:
+        return
 
     exists = file_path in _config_f
-    if exists: _config_f.remove(file_path)
+    if exists:
+        _config_f.remove(file_path)
     _config_f.append(file_path)
 
     file = open(file_path, "rb")
-    try: data = file.read()
-    finally: file.close()
-    if not data: return
+    try:
+        data = file.read()
+    finally:
+        file.close()
+    if not data:
+        return
 
     data = data.decode(encoding)
     data_j = json.loads(data)
 
-    _load_includes(base_path, data_j, encoding = encoding)
+    _load_includes(base_path, data_j, encoding=encoding)
 
     for key, value in data_j.items():
-        if not _is_valid(key): continue
+        if not _is_valid(key):
+            continue
         config[key] = value
 
-def load_env(ctx = None):
+
+def load_env(ctx=None):
     _config = ctx["config"] if ctx else config_g
 
     config = dict(os.environ)
     homes = get_homes()
 
     for home in homes:
         _load_includes(home, config)
 
     for key, value in legacy.iteritems(config):
-        if not _is_valid(key): continue
+        if not _is_valid(key):
+            continue
         _config[key] = value
         is_bytes = legacy.is_bytes(value)
-        if not is_bytes: continue
+        if not is_bytes:
+            continue
         for encoding in ENV_ENCODINGS:
-            try: value = value.decode(encoding)
-            except UnicodeDecodeError: pass
-            else: break
+            try:
+                value = value.decode(encoding)
+            except UnicodeDecodeError:
+                pass
+            else:
+                break
         _config[key] = value
 
-def get_homes(
-    file_path = HOME_FILE,
-    default = "~",
-    encoding = "utf-8",
-    force_default = False
-):
+
+def get_homes(file_path=HOME_FILE, default="~", encoding="utf-8", force_default=False):
     global homes
-    if homes: return homes
+    if homes:
+        return homes
 
     homes = os.environ.get("HOMES", None)
     homes = homes.split(";") if homes else homes
-    if not homes == None: return homes
+    if not homes == None:
+        return homes
 
     default = os.path.expanduser(default)
     default = os.path.abspath(default)
     default = os.path.normpath(default)
     homes = [default]
 
     file_path = os.path.expanduser(file_path)
     file_path = os.path.normpath(file_path)
     exists = os.path.exists(file_path)
-    if not exists: return homes
+    if not exists:
+        return homes
 
-    if not force_default: del homes[:]
+    if not force_default:
+        del homes[:]
 
     file = open(file_path, "rb")
-    try: data = file.read()
-    finally: file.close()
+    try:
+        data = file.read()
+    finally:
+        file.close()
 
     data = data.decode("utf-8")
     data = data.strip()
     paths = data.splitlines()
     paths = [path.strip() for path in paths]
 
     for path in paths:
         path = path.strip()
-        if not path: continue
+        if not path:
+            continue
         path = os.path.expanduser(path)
         path = os.path.abspath(path)
         path = os.path.normpath(path)
         homes.append(path)
 
     return homes
 
+
 def _cast_r(cast):
     is_string = type(cast) in legacy.STRINGS
-    if is_string: cast = __builtins__.get(cast, None)
-    if not cast: return None
+    if is_string:
+        cast = __builtins__.get(cast, None)
+    if not cast:
+        return None
     return CASTS.get(cast, cast)
 
-def _load_includes(base_path, config, encoding = "utf-8"):
+
+def _load_includes(base_path, config, encoding="utf-8"):
     includes = ()
 
     for alias in IMPORT_NAMES:
         includes = config.get(alias, includes)
 
     if legacy.is_string(includes):
         includes = includes.split(";")
 
     for include in includes:
-        load_file(
-            name = include,
-            path = base_path,
-            encoding = encoding
-        )
+        load_file(name=include, path=base_path, encoding=encoding)
+
 
 def _is_valid(key):
-    if key in IMPORT_NAMES: return False
+    if key in IMPORT_NAMES:
+        return False
     return True
 
+
 load()
```

### Comparing `quorum-0.8.2/src/quorum/httpc.py` & `quorum-0.8.3/src/quorum/httpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -65,36 +56,40 @@
 considered to be sequence based for python """
 
 AUTH_ERRORS = (401, 403, 440, 499)
 """ The sequence that defines the various HTTP errors
 considered to be authentication related and for which a
 new authentication try will be performed """
 
-def file_g(path, chunk = 40960):
+
+def file_g(path, chunk=40960):
     yield os.path.getsize(path)
     file = open(path, "rb")
     try:
         while True:
             data = file.read(chunk)
-            if not data: break
+            if not data:
+                break
             yield data
     finally:
         file.close()
 
+
 def get_f(*args, **kwargs):
     name = kwargs.pop("name", "default")
     kwargs["handle"] = kwargs.get("handle", True)
     kwargs["redirect"] = kwargs.get("redirect", True)
     data, response = get_json(*args, **kwargs)
     info = response.info()
     mime = info.get("Content-Type", None)
     file_tuple = (name, mime, data)
     return typesf.File(file_tuple)
 
-def get(url, auth_callback = None, **kwargs):
+
+def get(url, auth_callback=None, **kwargs):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _get(url, **kwargs)
@@ -107,496 +102,513 @@
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
+
 def get_json(
     url,
-    headers = None,
-    handle = None,
-    redirect = None,
-    silent = None,
-    timeout = None,
-    auth_callback = None,
+    headers=None,
+    handle=None,
+    redirect=None,
+    silent=None,
+    timeout=None,
+    auth_callback=None,
     **kwargs
 ):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _get_json(
                 url,
-                headers = headers,
-                handle = handle,
-                silent = silent,
-                redirect = redirect,
-                timeout = timeout,
+                headers=headers,
+                handle=handle,
+                silent=silent,
+                redirect=redirect,
+                timeout=timeout,
                 **kwargs
             )
         except legacy.HTTPError as error:
             if error.code in AUTH_ERRORS and auth_callback:
                 _try_auth(auth_callback, kwargs)
             else:
                 data_r = error.read()
-                data_r = legacy.str(data_r, encoding = "utf-8")
+                data_r = legacy.str(data_r, encoding="utf-8")
                 data_s = json.loads(data_r)
                 raise exceptions.JSONError(data_s)
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
+
 def post_json(
     url,
-    data = None,
-    data_j = None,
-    data_m = None,
-    headers = None,
-    mime = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    auth_callback = None,
+    data=None,
+    data_j=None,
+    data_m=None,
+    headers=None,
+    mime=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
+    auth_callback=None,
     **kwargs
 ):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _post_json(
                 url,
-                data = data,
-                data_j = data_j,
-                data_m = data_m,
-                headers = headers,
-                mime = mime,
-                handle = handle,
-                silent = silent,
-                redirect = redirect,
-                timeout = timeout,
+                data=data,
+                data_j=data_j,
+                data_m=data_m,
+                headers=headers,
+                mime=mime,
+                handle=handle,
+                silent=silent,
+                redirect=redirect,
+                timeout=timeout,
                 **kwargs
             )
         except legacy.HTTPError as error:
             if error.code in AUTH_ERRORS and auth_callback:
                 _try_auth(auth_callback, kwargs)
             else:
                 data_r = error.read()
-                data_r = legacy.str(data_r, encoding = "utf-8")
+                data_r = legacy.str(data_r, encoding="utf-8")
                 data_s = json.loads(data_r)
                 raise exceptions.JSONError(data_s)
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
+
 def put_json(
     url,
-    data = None,
-    data_j = None,
-    data_m = None,
-    headers = None,
-    mime = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    auth_callback = None,
+    data=None,
+    data_j=None,
+    data_m=None,
+    headers=None,
+    mime=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
+    auth_callback=None,
     **kwargs
 ):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _put_json(
                 url,
-                data = data,
-                data_j = data_j,
-                data_m = data_m,
-                headers = headers,
-                mime = mime,
-                handle = handle,
-                silent = silent,
-                redirect = redirect,
-                timeout = timeout,
+                data=data,
+                data_j=data_j,
+                data_m=data_m,
+                headers=headers,
+                mime=mime,
+                handle=handle,
+                silent=silent,
+                redirect=redirect,
+                timeout=timeout,
                 **kwargs
             )
         except legacy.HTTPError as error:
             if error.code in AUTH_ERRORS and auth_callback:
                 _try_auth(auth_callback, kwargs)
             else:
                 data_r = error.read()
-                data_r = legacy.str(data_r, encoding = "utf-8")
+                data_r = legacy.str(data_r, encoding="utf-8")
                 data_s = json.loads(data_r)
                 raise exceptions.JSONError(data_s)
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
+
 def delete_json(
     url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    auth_callback = None,
+    headers=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
+    auth_callback=None,
     **kwargs
 ):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _delete_json(
                 url,
-                headers = headers,
-                handle = handle,
-                silent = silent,
-                redirect = redirect,
-                timeout = timeout,
+                headers=headers,
+                handle=handle,
+                silent=silent,
+                redirect=redirect,
+                timeout=timeout,
                 **kwargs
             )
         except legacy.HTTPError as error:
             if error.code in AUTH_ERRORS and auth_callback:
                 _try_auth(auth_callback, kwargs)
             else:
                 data_r = error.read()
-                data_r = legacy.str(data_r, encoding = "utf-8")
+                data_r = legacy.str(data_r, encoding="utf-8")
                 data_s = json.loads(data_r)
                 raise exceptions.JSONError(data_s)
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
+
 def patch_json(
     url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    auth_callback = None,
+    headers=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
+    auth_callback=None,
     **kwargs
 ):
     # starts the variable holding the number of
     # retrieves to be used
     retries = 5
 
     while True:
         try:
             return _patch_json(
                 url,
-                headers = headers,
-                handle = handle,
-                silent = silent,
-                redirect = redirect,
-                timeout = timeout,
+                headers=headers,
+                handle=handle,
+                silent=silent,
+                redirect=redirect,
+                timeout=timeout,
                 **kwargs
             )
         except legacy.HTTPError as error:
             if error.code in AUTH_ERRORS and auth_callback:
                 _try_auth(auth_callback, kwargs)
             else:
                 data_r = error.read()
-                data_r = legacy.str(data_r, encoding = "utf-8")
+                data_r = legacy.str(data_r, encoding="utf-8")
                 data_s = json.loads(data_r)
                 raise exceptions.JSONError(data_s)
 
         # decrements the number of retries and checks if the
         # number of retries has reached the limit
         retries -= 1
         if retries == 0:
             raise exceptions.HTTPError("Data retrieval not possible")
 
-def basic_auth(username, password = None):
-    if not password: password = username
+
+def basic_auth(username, password=None):
+    if not password:
+        password = username
     authorization = _authorization(username, password)
     return "Basic %s" % authorization
 
-def _try_auth(auth_callback, params, headers = None):
-    if not auth_callback: raise
-    if headers == None: headers = dict()
+
+def _try_auth(auth_callback, params, headers=None):
+    if not auth_callback:
+        raise
+    if headers == None:
+        headers = dict()
     auth_callback(params, headers)
 
+
 def _get(url, **kwargs):
     values = kwargs or dict()
     data = _urlencode(values)
     url = url + "?" + data if data else url
     file = _resolve(url, "GET", {}, None, False, TIMEOUT)
     contents = file.read()
     return contents
 
+
 def _get_json(
-    url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    **kwargs
+    url, headers=None, handle=None, silent=None, redirect=None, timeout=None, **kwargs
 ):
     return _method_empty(
         "GET",
         url,
-        headers = headers,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout,
+        headers=headers,
+        handle=handle,
+        silent=silent,
+        redirect=redirect,
+        timeout=timeout,
         **kwargs
     )
 
+
 def _post_json(
     url,
-    data = None,
-    data_j = None,
-    data_m = None,
-    headers = None,
-    mime = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
+    data=None,
+    data_j=None,
+    data_m=None,
+    headers=None,
+    mime=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
     **kwargs
 ):
     return _method_payload(
         "POST",
         url,
-        data = data,
-        data_j = data_j,
-        data_m = data_m,
-        headers = headers,
-        mime = mime,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout,
+        data=data,
+        data_j=data_j,
+        data_m=data_m,
+        headers=headers,
+        mime=mime,
+        handle=handle,
+        silent=silent,
+        redirect=redirect,
+        timeout=timeout,
         **kwargs
     )
 
+
 def _put_json(
     url,
-    data = None,
-    data_j = None,
-    data_m = None,
-    headers = None,
-    mime = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
+    data=None,
+    data_j=None,
+    data_m=None,
+    headers=None,
+    mime=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
     **kwargs
 ):
     return _method_payload(
         "PUT",
         url,
-        data = data,
-        data_j = data_j,
-        data_m = data_m,
-        headers = headers,
-        mime = mime,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout,
+        data=data,
+        data_j=data_j,
+        data_m=data_m,
+        headers=headers,
+        mime=mime,
+        handle=handle,
+        silent=silent,
+        redirect=redirect,
+        timeout=timeout,
         **kwargs
     )
 
+
 def _delete_json(
-    url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    **kwargs
+    url, headers=None, handle=None, silent=None, redirect=None, timeout=None, **kwargs
 ):
     return _method_empty(
         "DELETE",
         url,
-        headers = headers,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout,
+        headers=headers,
+        handle=handle,
+        silent=silent,
+        redirect=redirect,
+        timeout=timeout,
         **kwargs
     )
 
+
 def _patch_json(
-    url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    **kwargs
+    url, headers=None, handle=None, silent=None, redirect=None, timeout=None, **kwargs
 ):
     return _method_empty(
         "PATCH",
         url,
-        headers = headers,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout,
+        headers=headers,
+        handle=handle,
+        silent=silent,
+        redirect=redirect,
+        timeout=timeout,
         **kwargs
     )
 
+
 def _method_empty(
     name,
     url,
-    headers = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
+    headers=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
     **kwargs
 ):
-    if handle == None: handle = False
-    if silent == None: silent = False
-    if redirect == None: redirect = False
-    if timeout == None: timeout = TIMEOUT
+    if handle == None:
+        handle = False
+    if silent == None:
+        silent = False
+    if redirect == None:
+        redirect = False
+    if timeout == None:
+        timeout = TIMEOUT
     values = kwargs or dict()
     url, scheme, host, authorization, extra = _parse_url(url)
-    if extra: values.update(extra)
+    if extra:
+        values.update(extra)
     data = _urlencode(values)
     headers = dict(headers) if headers else dict()
-    if host: headers["host"] = host
-    if authorization: headers["Authorization"] = "Basic %s" % authorization
+    if host:
+        headers["host"] = host
+    if authorization:
+        headers["Authorization"] = "Basic %s" % authorization
     url = url + "?" + data if data else url
     url = str(url)
     file = _resolve(url, name, headers, None, silent, timeout)
-    try: result = file.read()
-    finally: file.close()
+    try:
+        result = file.read()
+    finally:
+        file.close()
     info = file.info()
     location = info.get("Location", None) if redirect else None
-    if location: return _redirect(
-        location,
-        scheme,
-        host,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout
-    )
+    if location:
+        return _redirect(
+            location,
+            scheme,
+            host,
+            handle=handle,
+            silent=silent,
+            redirect=redirect,
+            timeout=timeout,
+        )
     result = _result(result, info)
     return (result, file) if handle else result
 
+
 def _method_payload(
     name,
     url,
-    data = None,
-    data_j = None,
-    data_m = None,
-    headers = None,
-    mime = None,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None,
-    **kwargs
-):
-    if handle == None: handle = False
-    if silent == None: silent = False
-    if redirect == None: redirect = False
-    if timeout == None: timeout = TIMEOUT
+    data=None,
+    data_j=None,
+    data_m=None,
+    headers=None,
+    mime=None,
+    handle=None,
+    silent=None,
+    redirect=None,
+    timeout=None,
+    **kwargs
+):
+    if handle == None:
+        handle = False
+    if silent == None:
+        silent = False
+    if redirect == None:
+        redirect = False
+    if timeout == None:
+        timeout = TIMEOUT
     values = kwargs or dict()
 
     url, scheme, host, authorization, extra = _parse_url(url)
-    if extra: values.update(extra)
+    if extra:
+        values.update(extra)
     data_e = _urlencode(values)
 
     if not data == None:
         url = url + "?" + data_e if data_e else url
     elif not data_j == None:
         data = json.dumps(data_j)
         url = url + "?" + data_e if data_e else url
         mime = mime or "application/json"
     elif not data_m == None:
         url = url + "?" + data_e if data_e else url
-        content_type, data = _encode_multipart(
-            data_m, mime = mime, doseq = True
-        )
+        content_type, data = _encode_multipart(data_m, mime=mime, doseq=True)
         mime = content_type
     elif data_e:
         data = data_e
         mime = mime or "application/x-www-form-urlencoded"
 
-    if legacy.is_unicode(data): data = legacy.bytes(data, force = True)
+    if legacy.is_unicode(data):
+        data = legacy.bytes(data, force=True)
 
-    if not data: length = 0
-    elif legacy.is_bytes(data): length = len(data)
-    else: length = -1
+    if not data:
+        length = 0
+    elif legacy.is_bytes(data):
+        length = len(data)
+    else:
+        length = -1
 
     headers = dict(headers) if headers else dict()
-    if not length == -1: headers["Content-Length"] = length
-    if mime: headers["Content-Type"] = mime
-    if host: headers["Host"] = host
-    if authorization: headers["Authorization"] = "Basic %s" % authorization
+    if not length == -1:
+        headers["Content-Length"] = length
+    if mime:
+        headers["Content-Type"] = mime
+    if host:
+        headers["Host"] = host
+    if authorization:
+        headers["Authorization"] = "Basic %s" % authorization
     url = str(url)
 
     file = _resolve(url, name, headers, data, silent, timeout)
-    try: result = file.read()
-    finally: file.close()
+    try:
+        result = file.read()
+    finally:
+        file.close()
 
     info = file.info()
 
     location = info.get("Location", None) if redirect else None
-    if location: return _redirect(
-        location,
-        scheme,
-        host,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout
-    )
+    if location:
+        return _redirect(
+            location,
+            scheme,
+            host,
+            handle=handle,
+            silent=silent,
+            redirect=redirect,
+            timeout=timeout,
+        )
 
     result = _result(result, info)
     return (result, file) if handle else result
 
+
 def _redirect(
-    location,
-    scheme,
-    host,
-    handle = None,
-    silent = None,
-    redirect = None,
-    timeout = None
+    location, scheme, host, handle=None, silent=None, redirect=None, timeout=None
 ):
     is_relative = location.startswith("/")
-    if is_relative: location = scheme + "://" + host + location
+    if is_relative:
+        location = scheme + "://" + host + location
     return get_json(
-        location,
-        handle = handle,
-        silent = silent,
-        redirect = redirect,
-        timeout = timeout
+        location, handle=handle, silent=silent, redirect=redirect, timeout=timeout
     )
 
+
 def _resolve(*args, **kwargs):
     # obtains the reference to the global set of variables, so
     # that it's possible to obtain the proper resolver method
     # according to the requested client
     _global = globals()
 
     # tries to retrieve the global configuration values that
@@ -608,254 +620,291 @@
     # compared with the global configuration ones
     client = kwargs.pop("client", client)
 
     # tries to retrieve the reference to the resolve method for the
     # current client and then runs it, retrieve then the final result,
     # note that the result structure may be engine dependent
     resolver = _global.get("_resolve_" + client, _resolve_legacy)
-    try: result = resolver(*args, **kwargs)
-    except ImportError: result = _resolve_legacy(*args, **kwargs)
+    try:
+        result = resolver(*args, **kwargs)
+    except ImportError:
+        result = _resolve_legacy(*args, **kwargs)
     return result
 
+
 def _resolve_legacy(url, method, headers, data, silent, timeout, **kwargs):
     is_generator = not data == None and legacy.is_generator(data)
-    if is_generator: next(data); data = b"".join(data)
+    if is_generator:
+        next(data)
+        data = b"".join(data)
     is_file = hasattr(data, "tell")
-    if is_file: data = data.read()
+    if is_file:
+        data = data.read()
     opener = legacy.build_opener(legacy.HTTPHandler)
-    request = legacy.Request(url, data = data, headers = headers)
+    request = legacy.Request(url, data=data, headers=headers)
     request.get_method = lambda: method
-    return opener.open(request, timeout = timeout)
+    return opener.open(request, timeout=timeout)
+
 
 def _resolve_requests(url, method, headers, data, silent, timeout, **kwargs):
     import requests
 
     # verifies if the provided data is a generator, assumes that if the
     # data is not invalid and is of type generator then it's a generator
     # and then if that's the case encapsulates this size based generator
     # into a generator based file-like object so that it can be used inside
     # the request infra-structure (as it accepts only file objects)
     is_generator = not data == None and legacy.is_generator(data)
-    if is_generator: data = structures.GeneratorFile(data)
+    if is_generator:
+        data = structures.GeneratorFile(data)
 
     method = method.lower()
     caller = getattr(requests, method)
-    result = caller(url, headers = headers, data = data, timeout = timeout)
+    result = caller(url, headers=headers, data=data, timeout=timeout)
     response = HTTPResponse(
-        data = result.content,
-        code = result.status_code,
-        headers = result.headers
+        data=result.content, code=result.status_code, headers=result.headers
     )
     code = response.getcode()
     is_error = _is_error(code)
-    if is_error: raise legacy.HTTPError(
-        url, code, "HTTP retrieval problem", None, response
-    )
+    if is_error:
+        raise legacy.HTTPError(url, code, "HTTP retrieval problem", None, response)
     return response
 
+
 def _resolve_netius(url, method, headers, data, silent, timeout, **kwargs):
     import netius.clients
+
     silent = silent or False
     silent |= not common.is_devel()
     level = logging.CRITICAL if silent else logging.DEBUG
     level = kwargs.get("level", level)
     result = netius.clients.HTTPClient.method_s(
         method,
         url,
-        headers = headers,
-        data = data,
-        asynchronous = False,
-        timeout = timeout,
-        level = level
+        headers=headers,
+        data=data,
+        asynchronous=False,
+        timeout=timeout,
+        level=level,
     )
     response = netius.clients.HTTPClient.to_response(result)
     code = response.getcode()
     is_error = _is_error(code)
-    if is_error: raise legacy.HTTPError(
-        url, code, "HTTP retrieval problem", None, response
-    )
+    if is_error:
+        raise legacy.HTTPError(url, code, "HTTP retrieval problem", None, response)
     return response
 
+
 def _parse_url(url):
     parse = legacy.urlparse(url)
     scheme = parse.scheme
     secure = scheme == "https"
     default = 443 if secure else 80
     port = parse.port or default
     url = parse.scheme + "://" + parse.hostname + ":" + str(port) + parse.path
-    if port in (80, 443): host = parse.hostname
-    else: host = parse.hostname + ":" + str(port)
+    if port in (80, 443):
+        host = parse.hostname
+    else:
+        host = parse.hostname + ":" + str(port)
     authorization = _authorization(parse.username, parse.password)
     params = _params(parse.query)
     return (url, scheme, host, authorization, params)
 
-def _result(data, info = {}, force = False, strict = False):
+
+def _result(data, info={}, force=False, strict=False):
     # tries to retrieve the content type value from the headers
     # info and verifies if the current data is JSON encoded, so
     # that it gets automatically decoded for such cases
     content_type = info.get("Content-Type", None) or ""
-    is_json = util.is_content_type(
-        content_type,
-        (
-            "application/json",
-            "text/json",
-            "text/javascript"
+    is_json = (
+        util.is_content_type(
+            content_type, ("application/json", "text/json", "text/javascript")
         )
-    ) or force
+        or force
+    )
 
     # verifies if the current result set is JSON encoded and in
     # case it's decodes it and loads it as JSON otherwise returns
     # the "raw" data to the caller method as expected, note that
     # the strict flag is used to determine if the exception should
     # be re-raised to the upper level in case of value error
-    if is_json and legacy.is_bytes(data): data = data.decode("utf-8")
-    try: data = json.loads(data) if is_json else data
+    if is_json and legacy.is_bytes(data):
+        data = data.decode("utf-8")
+    try:
+        data = json.loads(data) if is_json else data
     except ValueError:
-        if strict: raise
+        if strict:
+            raise
     return data
 
+
 def _params(query):
     # creates the dictionary that is going to be used to store the
     # complete information regarding the parameters in query
     params = dict()
 
     # validates that the provided query value is valid and if
     # that's not the case returns the created parameters immediately
     # (empty parameters are returned)
-    if not query: return params
+    if not query:
+        return params
 
     # splits the query value around the initial parameter separator
     # symbol and iterates over each of them to parse them and create
     # the proper parameters dictionary (of lists)
     query_s = query.split("&")
     for part in query_s:
         parts = part.split("=", 1)
-        if len(parts) == 1: value = ""
-        else: value = parts[1]
+        if len(parts) == 1:
+            value = ""
+        else:
+            value = parts[1]
         key = parts[0]
         key = legacy.unquote_plus(key)
         value = legacy.unquote_plus(value)
         param = params.get(key, [])
         param.append(value)
         params[key] = param
 
     # returns the final parameters dictionary to the caller method
     # so that it may be used as a proper structure representation
     return params
 
-def _urlencode(values, as_string = True):
+
+def _urlencode(values, as_string=True):
     # creates the list that will hold the final tuple of values
     # (without the unset and invalid values)
     final = []
 
     # verifies if the provided value is a sequence and in case it's
     # not converts it into a sequence (assuming a map)
     is_sequence = isinstance(values, (list, tuple))
-    if not is_sequence: values = values.items()
+    if not is_sequence:
+        values = values.items()
 
     # iterates over all the items in the values sequence to
     # try to filter the values that are not valid
     for key, value in values:
         # creates the list that will hold the valid values
         # of the current key in iteration (sanitized values)
         _values = []
 
         # in case the current data type of the key is unicode
         # the value must be converted into a string using the
         # default utf encoding strategy (as defined)
-        if type(key) == legacy.UNICODE: key = key.encode("utf-8")
+        if type(key) == legacy.UNICODE:
+            key = key.encode("utf-8")
 
         # verifies the type of the current value and in case
         # it's sequence based converts it into a list using
         # the conversion method otherwise creates a new list
         # and includes the value in it
         value_t = type(value)
-        if value_t in SEQUENCE_TYPES: value = list(value)
-        else: value = [value]
+        if value_t in SEQUENCE_TYPES:
+            value = list(value)
+        else:
+            value = [value]
 
         # iterates over all the values in the current sequence
         # and adds the valid values to the sanitized sequence,
         # this includes the conversion from unicode string into
         # a simple string using the default utf encoder
         for _value in value:
-            if _value == None: continue
+            if _value == None:
+                continue
             is_string = type(_value) in legacy.STRINGS
-            if not is_string: _value = str(_value)
+            if not is_string:
+                _value = str(_value)
             is_unicode = type(_value) == legacy.UNICODE
-            if is_unicode: _value = _value.encode("utf-8")
+            if is_unicode:
+                _value = _value.encode("utf-8")
             _values.append(_value)
 
         # sets the sanitized list of values as the new value for
         # the key in the final dictionary of values
         final.append((key, _values))
 
     # in case the "as string" flag is not set the ended key to value
     # dictionary should be returned to the called method and not the
     # "default" linear and string based value
-    if not as_string: return final
+    if not as_string:
+        return final
 
     # runs the encoding with sequence support on the final map
     # of sanitized values and returns the encoded result to the
     # caller method as the encoded value
-    return legacy.urlencode(final, doseq = True)
+    return legacy.urlencode(final, doseq=True)
 
-def _quote(values, plus = False, safe = "/"):
+
+def _quote(values, plus=False, safe="/"):
     method = legacy.quote_plus if plus else legacy.quote
-    values = _urlencode(values, as_string = False)
+    values = _urlencode(values, as_string=False)
 
     final = dict()
 
     for key, value in values.items():
-        key = method(key, safe = safe)
-        value = method(value[0], safe = safe)
+        key = method(key, safe=safe)
+        value = method(value[0], safe=safe)
         final[key] = value
 
     return final
 
+
 def _authorization(username, password):
-    if not username: return None
-    if not password: return None
+    if not username:
+        return None
+    if not password:
+        return None
     payload = "%s:%s" % (username, password)
     payload = legacy.bytes(payload)
     authorization = base64.b64encode(payload)
     authorization = legacy.str(authorization)
     return authorization
 
-def _encode_multipart(fields, mime = None, doseq = False):
+
+def _encode_multipart(fields, mime=None, doseq=False):
     mime = mime or "multipart/form-data"
-    boundary = _create_boundary(fields, doseq = doseq)
+    boundary = _create_boundary(fields, doseq=doseq)
     boundary_b = legacy.bytes(boundary)
 
     buffer = []
 
     for key, values in fields.items():
         is_list = doseq and type(values) == list
         values = values if is_list else [values]
 
         for value in values:
-            if value == None: continue
+            if value == None:
+                continue
 
             if isinstance(value, dict):
                 header_l = []
                 data = None
                 for key, item in value.items():
-                    if key == "data": data = item
-                    else: header_l.append("%s: %s" % (key, item))
+                    if key == "data":
+                        data = item
+                    else:
+                        header_l.append("%s: %s" % (key, item))
                 value = data
                 header = "\r\n".join(header_l)
             elif isinstance(value, tuple):
                 content_type = None
-                if len(value) == 2: name, contents = value
-                else: name, content_type, contents = value
-                header = "Content-Disposition: form-data; name=\"%s\"; filename=\"%s\"" %\
-                    (key, name)
-                if content_type: header += "\r\nContent-Type: %s" % content_type
+                if len(value) == 2:
+                    name, contents = value
+                else:
+                    name, content_type, contents = value
+                header = 'Content-Disposition: form-data; name="%s"; filename="%s"' % (
+                    key,
+                    name,
+                )
+                if content_type:
+                    header += "\r\nContent-Type: %s" % content_type
                 value = contents
             else:
-                header = "Content-Disposition: form-data; name=\"%s\"" % key
+                header = 'Content-Disposition: form-data; name="%s"' % key
                 value = _encode(value)
 
             header = _encode(header)
             value = _encode(value)
 
             buffer.append(b"--" + boundary_b)
             buffer.append(header)
@@ -865,60 +914,79 @@
     buffer.append(b"--" + boundary_b + b"--")
     buffer.append(b"")
     body = b"\r\n".join(buffer)
     content_type = "%s; boundary=%s" % (mime, boundary)
 
     return content_type, body
 
-def _create_boundary(fields, size = 32, doseq = False):
+
+def _create_boundary(fields, size=32, doseq=False):
     while True:
         base = "".join(random.choice(RANGE) for _value in range(size))
         boundary = "----------" + base
-        result = _try_boundary(fields, boundary, doseq = doseq)
-        if result: break
+        result = _try_boundary(fields, boundary, doseq=doseq)
+        if result:
+            break
 
     return boundary
 
-def _try_boundary(fields, boundary, doseq = False):
+
+def _try_boundary(fields, boundary, doseq=False):
     boundary_b = legacy.bytes(boundary)
 
     for key, values in fields.items():
         is_list = doseq and type(values) == list
         values = values if is_list else [values]
 
         for value in values:
-            if isinstance(value, dict): name = ""; value = value.get("data", b"")
+            if isinstance(value, dict):
+                name = ""
+                value = value.get("data", b"")
             elif isinstance(value, tuple):
-                if len(value) == 2: name = value[0] or ""; value = value[1] or b""
-                else: name = value[0] or ""; value = value[2] or b""
-            else: name = ""; value = _encode(value)
-
-            if not key.find(boundary) == -1: return False
-            if not name.find(boundary) == -1: return False
-            if not value.find(boundary_b) == -1: return False
+                if len(value) == 2:
+                    name = value[0] or ""
+                    value = value[1] or b""
+                else:
+                    name = value[0] or ""
+                    value = value[2] or b""
+            else:
+                name = ""
+                value = _encode(value)
+
+            if not key.find(boundary) == -1:
+                return False
+            if not name.find(boundary) == -1:
+                return False
+            if not value.find(boundary_b) == -1:
+                return False
 
     return True
 
+
 def _is_error(code):
     return code // 100 in (4, 5) if code else True
 
-def _encode(value, encoding = "utf-8"):
+
+def _encode(value, encoding="utf-8"):
     value_t = type(value)
-    if value_t == legacy.BYTES: return value
-    elif value_t == legacy.UNICODE: return value.encode(encoding)
+    if value_t == legacy.BYTES:
+        return value
+    elif value_t == legacy.UNICODE:
+        return value.encode(encoding)
     return legacy.bytes(str(value))
 
+
 class HTTPResponse(object):
     """
     Compatibility object to be used by HTTP libraries that do
     not support the legacy HTTP response object as a return
     for any of their structures.
     """
 
-    def __init__(self, data = None, code = 200, status = None, headers = None):
+    def __init__(self, data=None, code=200, status=None, headers=None):
         self.data = data
         self.code = code
         self.status = status
         self.headers = headers
 
     def read(self):
         return self.data
```

### Comparing `quorum-0.8.2/src/quorum/model.py` & `quorum-0.8.3/src/quorum/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import re
@@ -61,188 +52,181 @@
 evaluation, this is required to avoid miss behavior """
 
 RE = lambda v: [i for i in v if not i == ""]
 """ Simple lambda function that removes any
 empty element from the provided list values """
 
 BUILDERS = {
-    legacy.UNICODE : lambda v: v.decode("utf-8") if\
-        isinstance(v, legacy.BYTES) else legacy.UNICODE(v),
-    list : lambda v: RE(v) if isinstance(v, list) else\
-        (json.loads(v) if isinstance(v, legacy.UNICODE) else RE([v])),
-    dict : lambda v: json.loads(v) if isinstance(v, legacy.UNICODE) else dict(v),
-    bool : lambda v: v if isinstance(v, bool) else\
-        not v in ("", "0", "false", "False")
+    legacy.UNICODE: lambda v: (
+        v.decode("utf-8") if isinstance(v, legacy.BYTES) else legacy.UNICODE(v)
+    ),
+    list: lambda v: (
+        RE(v)
+        if isinstance(v, list)
+        else (json.loads(v) if isinstance(v, legacy.UNICODE) else RE([v]))
+    ),
+    dict: lambda v: json.loads(v) if isinstance(v, legacy.UNICODE) else dict(v),
+    bool: lambda v: v if isinstance(v, bool) else not v in ("", "0", "false", "False"),
 }
 """ The map associating the various types with the
 custom builder functions to be used when applying
 the types function, this is relevant for the built-in
 types that are meant to avoid using the default constructor """
 
 BUILDERS_META = dict(
-    text = BUILDERS[legacy.UNICODE],
-    country = BUILDERS[legacy.UNICODE],
-    longtext = BUILDERS[legacy.UNICODE],
-    map = BUILDERS[dict],
-    longmap = BUILDERS[dict],
-    date = lambda v: float(v),
-    datetetime = lambda v: float(v),
-    file = None
+    text=BUILDERS[legacy.UNICODE],
+    country=BUILDERS[legacy.UNICODE],
+    longtext=BUILDERS[legacy.UNICODE],
+    map=BUILDERS[dict],
+    longmap=BUILDERS[dict],
+    date=lambda v: float(v),
+    datetetime=lambda v: float(v),
+    file=None,
 )
 """ Map equivalent to the builders map but appliable
 for meta based type naming, this map should be used as
 an extension to the base builder map """
 
 METAS = dict(
-    text = lambda v, d, c = None: v,
-    enum = lambda v, d, c = None: d["enum"].get(v, None),
-    list = lambda v, d, c = None:\
-        json.dumps(v, ensure_ascii = False, cls = c._encoder() if c else None),
-    map = lambda v, d, c = None:\
-        json.dumps(v, ensure_ascii = False, cls = c._encoder() if c else None),
-    longmap = lambda v, d, c = None:\
-        json.dumps(v, ensure_ascii = False, cls = c._encoder() if c else None),
-    date = lambda v, d, c = None:\
-        datetime.datetime.utcfromtimestamp(float(v)).strftime("%d %b %Y"),
-    datetime = lambda v, d, c = None:\
-        datetime.datetime.utcfromtimestamp(float(v)).strftime("%d %b %Y %H:%M:%S")
+    text=lambda v, d, c=None: v,
+    enum=lambda v, d, c=None: d["enum"].get(v, None),
+    list=lambda v, d, c=None: json.dumps(
+        v, ensure_ascii=False, cls=c._encoder() if c else None
+    ),
+    map=lambda v, d, c=None: json.dumps(
+        v, ensure_ascii=False, cls=c._encoder() if c else None
+    ),
+    longmap=lambda v, d, c=None: json.dumps(
+        v, ensure_ascii=False, cls=c._encoder() if c else None
+    ),
+    date=lambda v, d, c=None: datetime.datetime.utcfromtimestamp(float(v)).strftime(
+        "%d %b %Y"
+    ),
+    datetime=lambda v, d, c=None: datetime.datetime.utcfromtimestamp(float(v)).strftime(
+        "%d %b %Y %H:%M:%S"
+    ),
 )
 """ The map that contains the various mapping functions
 for the meta types that may be described for a field under
 the current model specification, the resulting value for
 each of these functions should preferably be a string """
 
 TYPE_DEFAULTS = {
-    legacy.BYTES : None,
-    legacy.UNICODE : None,
-    int : None,
-    float : None,
-    bool : False,
-    list : lambda: [],
-    dict : lambda: {}
+    legacy.BYTES: None,
+    legacy.UNICODE: None,
+    int: None,
+    float: None,
+    bool: False,
+    list: lambda: [],
+    dict: lambda: {},
 }
 """ The default values to be set when a type
 conversion fails for the provided string value
 the resulting value may be returned when a validation
 fails an so it must be used carefully """
 
 TYPE_META = {
-    typesf.File : "file",
-    typesf.Files : "files",
-    typesf.Reference : "reference",
-    typesf.References : "references",
-    legacy.BYTES : "string",
-    legacy.UNICODE : "string",
-    int : "number",
-    float : "float",
+    typesf.File: "file",
+    typesf.Files: "files",
+    typesf.Reference: "reference",
+    typesf.References: "references",
+    legacy.BYTES: "string",
+    legacy.UNICODE: "string",
+    int: "number",
+    float: "float",
     bool: "bool",
-    list : "list",
-    dict : "map"
+    list: "list",
+    dict: "map",
 }
 """ Dictionary that defines the default mapping for each
 of the base data types against the associated default meta
 values for each for them, these meta type values are going
 to be used mostly for presentation purposes """
 
-TYPE_REFERENCES = (
-    typesf.Reference,
-    typesf.References
-)
+TYPE_REFERENCES = (typesf.Reference, typesf.References)
 """ The various data types that are considered to be references
 so that they are lazy loaded from the data source, these kind
 of types should be compliant to a common interface so that they
 may be used "blindly" from an external entity """
 
 REVERSE = dict(
-    descending = "ascending",
-    ascending = "descending",
+    descending="ascending",
+    ascending="descending",
 )
 """ The reverse order dictionary that maps a certain
 order direction (as a string) with the opposite one
 this may be used to "calculate" the reverse value """
 
-DIRTY_PARAMS = (
-    "map",
-    "rules",
-    "meta",
-    "build",
-    "skip",
-    "limit",
-    "sort",
-    "raise_e"
-)
+DIRTY_PARAMS = ("map", "rules", "meta", "build", "skip", "limit", "sort", "raise_e")
 """ The set containing the complete set of parameter names for
 the parameters that are considered to be dirty and that should
 be cleaned from any query operation on the data source, otherwise
 serious consequences may occur """
 
 OPERATORS = {
-    "eq" : None,
-    "equals" : None,
-    "ne" : "$ne",
-    "not_equals" : "$ne",
-    "in" : "$in",
-    "nin" : "$nin",
-    "not_in" : "$nin",
-    "like" : "$regex",
-    "likei" : "$regex",
-    "llike" : "$regex",
-    "llikei" : "$regex",
-    "rlike" : "$regex",
-    "rlikei" : "$regex",
-    "gt" : "$gt",
-    "greater" : "$gt",
-    "gte" : "$gte",
-    "greater_equal" : "$gte",
-    "lt" : "$lt",
-    "lesser" : "$lt",
-    "lte" : "$lte",
-    "lesser_equal" : "$lte",
-    "null" : None,
-    "is_null" : None,
-    "not_null" : "$ne",
-    "is_not_null" : "$ne",
-    "contains" : "$all"
+    "eq": None,
+    "equals": None,
+    "ne": "$ne",
+    "not_equals": "$ne",
+    "in": "$in",
+    "nin": "$nin",
+    "not_in": "$nin",
+    "like": "$regex",
+    "likei": "$regex",
+    "llike": "$regex",
+    "llikei": "$regex",
+    "rlike": "$regex",
+    "rlikei": "$regex",
+    "gt": "$gt",
+    "greater": "$gt",
+    "gte": "$gte",
+    "greater_equal": "$gte",
+    "lt": "$lt",
+    "lesser": "$lt",
+    "lte": "$lte",
+    "lesser_equal": "$lte",
+    "null": None,
+    "is_null": None,
+    "not_null": "$ne",
+    "is_not_null": "$ne",
+    "contains": "$all",
 }
 """ The map containing the mapping association between the
 normalized version of the operators and the infra-structure
 specific value for each of this operations, note that some
 of the values don't have a valid mapping for this operations
 the operator must be ignored and not used explicitly """
 
 VALUE_METHODS = {
-    "in" : lambda v, t: [t(v) for v in v.split(";")],
-    "not_in" : lambda v, t: [t(v) for v in v.split(";")],
-    "like" : lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + ".*$",
-    "likei" : lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + ".*$",
-    "llike" : lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + "$",
-    "llikei" : lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + "$",
-    "rlike" : lambda v, t: "^" + legacy.UNICODE(re.escape(v)) + ".*$",
-    "rlikei" : lambda v, t: "^" + legacy.UNICODE(re.escape(v)) + ".*$",
-    "null" : lambda v, t: None,
-    "is_null" : lambda v, t: None,
-    "not_null" : lambda v, t: None,
-    "is_not_null" : lambda v, t: None,
-    "contains" : lambda v, t: [t(v) for v in v.split(";")]
+    "in": lambda v, t: [t(v) for v in v.split(";")],
+    "not_in": lambda v, t: [t(v) for v in v.split(";")],
+    "like": lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + ".*$",
+    "likei": lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + ".*$",
+    "llike": lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + "$",
+    "llikei": lambda v, t: "^.*" + legacy.UNICODE(re.escape(v)) + "$",
+    "rlike": lambda v, t: "^" + legacy.UNICODE(re.escape(v)) + ".*$",
+    "rlikei": lambda v, t: "^" + legacy.UNICODE(re.escape(v)) + ".*$",
+    "null": lambda v, t: None,
+    "is_null": lambda v, t: None,
+    "not_null": lambda v, t: None,
+    "is_not_null": lambda v, t: None,
+    "contains": lambda v, t: [t(v) for v in v.split(";")],
 }
 """ Map that associates each of the normalized operations with
 an inline function that together with the data type maps the
 the base string based value into the target normalized value """
 
-INSENSITIVE = {
-    "likei" : True,
-    "llikei" : True,
-    "rlikei" : True
-}
+INSENSITIVE = {"likei": True, "llikei": True, "rlikei": True}
 """ The map that associates the various operators with the boolean
 values that define if an insensitive base search should be used
 instead of the "typical" sensitive search """
 
 BUILDERS.update(BUILDERS_META)
 
+
 class Model(legacy.with_meta(meta.Ordered, observer.Observable)):
     """
     Abstract model class from which all the models should
     directly or indirectly inherit. Should provide the
     basic infra-structure for the persistence of data using
     a plain key value storage engine.
 
@@ -252,70 +236,84 @@
 
     _extra_methods = []
     """ Special sequence of tuples (names and functions) that is
     used at instance creation time to bind the provided methods
     to the newly created instance, this is required for the dynamic
     addition of instance methods to models """
 
-    def __init__(self, model = None, **kwargs):
+    def __init__(self, model=None, **kwargs):
         fill = kwargs.pop("fill", True)
         model = model or {}
-        if fill: model = self.__class__.fill(model)
+        if fill:
+            model = self.__class__.fill(model)
         self.__dict__["_events"] = {}
         self.__dict__["_extras"] = []
         self.__dict__["model"] = model
         self.__dict__["ref"] = kwargs.pop("ref", None)
-        for name, value in kwargs.items(): setattr(self, name, value)
+        for name, value in kwargs.items():
+            setattr(self, name, value)
         for name, method in self.__class__._extra_methods:
-            if legacy.PYTHON_3: bound_method = types.MethodType(method, self)
-            else: bound_method = types.MethodType(method, self, self.__class__)
+            if legacy.PYTHON_3:
+                bound_method = types.MethodType(method, self)
+            else:
+                bound_method = types.MethodType(method, self, self.__class__)
             setattr(self, name, bound_method)
         observer.Observable.__init__(self)
 
     def __str__(self):
         cls = self.__class__
         default = cls.default()
-        if not default: return cls._name()
-        if not default in self.model: return cls._name()
+        if not default:
+            return cls._name()
+        if not default in self.model:
+            return cls._name()
         value = self.model[default]
-        if value == None: value = ""
+        if value == None:
+            value = ""
         is_string = legacy.is_str(value)
         return value if is_string else str(value)
 
     def __unicode__(self):
         cls = self.__class__
         default = cls.default()
-        if not default: return cls._name()
+        if not default:
+            return cls._name()
         value = self.model[default]
-        if value == None: value = ""
+        if value == None:
+            value = ""
         is_unicode = legacy.is_unicode(value)
         return value if is_unicode else legacy.UNICODE(value)
 
     def __getattribute__(self, name):
         try:
             model = object.__getattribute__(self, "model")
-            if name in model: return model[name]
-        except AttributeError: pass
+            if name in model:
+                return model[name]
+        except AttributeError:
+            pass
         cls = object.__getattribute__(self, "__class__")
         definition = cls.definition()
-        if name in definition: raise AttributeError(
-            "attribute '%s' is not set" % name
-        )
+        if name in definition:
+            raise AttributeError("attribute '%s' is not set" % name)
         return object.__getattribute__(self, name)
 
     def __setattr__(self, name, value):
         is_base = name in self.__dict__
-        if is_base: self.__dict__[name] = value
-        else: self.model[name] = value
+        if is_base:
+            self.__dict__[name] = value
+        else:
+            self.model[name] = value
 
     def __delattr__(self, name):
         try:
             model = object.__getattribute__(self, "model")
-            if name in model: del model[name]
-        except AttributeError: pass
+            if name in model:
+                del model[name]
+        except AttributeError:
+            pass
 
     def __len__(self):
         return self.model.__len__()
 
     def __getitem__(self, key):
         return self.model.__getitem__(key)
 
@@ -333,20 +331,20 @@
 
     def __bool__(self):
         return len(self.model) > 0
 
     @classmethod
     def new(
         cls,
-        model = None,
-        form = True,
-        safe = True,
-        build = False,
-        fill = True,
-        new = True,
+        model=None,
+        form=True,
+        safe=True,
+        build=False,
+        fill=True,
+        new=True,
         **kwargs
     ):
         """
         Creates a new instance of the model applying the provided model
         map to it after the instantiation of the class.
 
         The optional form flag controls if the form context data should be
@@ -388,34 +386,32 @@
         :param new: In case this value is valid the resulting instance is expected
         to be considered as new meaning that no identifier attributes are set.
         :rtype: Model
         :return: The new model instance resulting from the apply of the provided
         model and after the proper validations are performed on it.
         """
 
-        if model == None: model = util.get_object() if form else dict(kwargs)
-        if fill: model = cls.fill(model, safe = not new)
-        instance = cls(fill = False)
-        instance.apply(model, form = form, safe_a = safe)
-        if build: cls.build(instance.model, map = False)
-        if new: instance.assert_is_new()
+        if model == None:
+            model = util.get_object() if form else dict(kwargs)
+        if fill:
+            model = cls.fill(model, safe=not new)
+        instance = cls(fill=False)
+        instance.apply(model, form=form, safe_a=safe)
+        if build:
+            cls.build(instance.model, map=False)
+        if new:
+            instance.assert_is_new()
         return instance
 
     @classmethod
-    def old(cls, model = None, form = True, safe = True, build = False):
-        return cls.new(
-            model = model,
-            form = form,
-            safe = safe,
-            build = build,
-            new = False
-        )
+    def old(cls, model=None, form=True, safe=True, build=False):
+        return cls.new(model=model, form=form, safe=safe, build=build, new=False)
 
     @classmethod
-    def wrap(cls, models, build = True, handler = None, **kwargs):
+    def wrap(cls, models, build=True, handler=None, **kwargs):
         """
         "Wraps" the provided sequence (or single set) of model based data into a
         sequence of models (or a single model) so that proper business logic may
         be used for operations on top of that data.
 
         In case the extra handler argument is passed it's going to be called for
         each model that is going to be "wrapped" allowing an extra "layer" for
@@ -440,174 +436,185 @@
         operation to be performed at runtime.
         :rtype: List
         :return: The sequence of models (or single model) representing the provided
         set of dictionary models that were sent as arguments.
         """
 
         is_sequence = isinstance(models, (list, tuple))
-        if not is_sequence: models = [models]
+        if not is_sequence:
+            models = [models]
         wrapping = []
         for model in models:
-            if not isinstance(model, dict): continue
-            _model = cls(model = model, **kwargs)
+            if not isinstance(model, dict):
+                continue
+            _model = cls(model=model, **kwargs)
             handler and handler(_model.model)
-            build and cls.build(_model.model, map = False)
+            build and cls.build(_model.model, map=False)
             wrapping.append(_model)
-        if is_sequence: return wrapping
-        else: return wrapping[0] if wrapping else None
+        if is_sequence:
+            return wrapping
+        else:
+            return wrapping[0] if wrapping else None
 
     @classmethod
-    def singleton(
-        cls,
-        model = None,
-        form = True,
-        safe = True,
-        build = False,
-        *args,
-        **kwargs
-    ):
-        instance = cls.get(raise_e = False, *args, **kwargs)
+    def singleton(cls, model=None, form=True, safe=True, build=False, *args, **kwargs):
+        instance = cls.get(raise_e=False, *args, **kwargs)
         if instance:
-            instance.apply(model, form = form, safe_a = safe)
+            instance.apply(model, form=form, safe_a=safe)
         else:
-            instance = cls.old(
-                model = model,
-                form = form,
-                safe = safe,
-                build = build
-            )
+            instance = cls.old(model=model, form=form, safe=safe, build=build)
         return instance
 
     @classmethod
     def get(cls, *args, **kwargs):
-        fields,\
-        eager,\
-        eager_l,\
-        map,\
-        rules,\
-        meta,\
-        build,\
-        fill,\
-        resolve_a,\
-        skip,\
-        limit,\
-        sort,\
-        raise_e = cls._get_attrs(kwargs, (
-            ("fields", None),
-            ("eager", None),
-            ("eager_l", None),
-            ("map", False),
-            ("rules", True),
-            ("meta", False),
-            ("build", True),
-            ("fill", True),
-            ("resolve_a", None),
-            ("skip", 0),
-            ("limit", 0),
-            ("sort", None),
-            ("raise_e", True)
-        ))
+        (
+            fields,
+            eager,
+            eager_l,
+            map,
+            rules,
+            meta,
+            build,
+            fill,
+            resolve_a,
+            skip,
+            limit,
+            sort,
+            raise_e,
+        ) = cls._get_attrs(
+            kwargs,
+            (
+                ("fields", None),
+                ("eager", None),
+                ("eager_l", None),
+                ("map", False),
+                ("rules", True),
+                ("meta", False),
+                ("build", True),
+                ("fill", True),
+                ("resolve_a", None),
+                ("skip", 0),
+                ("limit", 0),
+                ("sort", None),
+                ("raise_e", True),
+            ),
+        )
 
         # in case there's a sort field and the safe search mode is enabled
         # we must add sorting by the `_id` field so that the retrieval is
         # considered to be deterministic, otherwise some DB implementations
         # will not respect the same sorting sequence across different calls
         if sort and (skip or limit):
-            if not isinstance(sort, list): sort = list(sort)
+            if not isinstance(sort, list):
+                sort = list(sort)
             sort.append(["_id", 1])
 
-        if eager_l == None: eager_l = map
-        if resolve_a == None: resolve_a = map
-        if eager_l: eager = cls._eager_b(eager)
-        fields = cls._sniff(fields, rules = rules)
+        if eager_l == None:
+            eager_l = map
+        if resolve_a == None:
+            resolve_a = map
+        if eager_l:
+            eager = cls._eager_b(eager)
+        fields = cls._sniff(fields, rules=rules)
         collection = cls._collection()
-        model = collection.find_one(
-            kwargs,
-            fields,
-            skip = skip,
-            limit = limit,
-            sort = sort
-        )
+        model = collection.find_one(kwargs, fields, skip=skip, limit=limit, sort=sort)
         if not model and raise_e:
             is_devel = common.is_devel()
-            if is_devel: message = "%s not found for %s" % (cls.__name__, str(kwargs))
-            else: message = "%s not found" % cls.__name__
+            if is_devel:
+                message = "%s not found for %s" % (cls.__name__, str(kwargs))
+            else:
+                message = "%s not found" % cls.__name__
             raise exceptions.NotFoundError(message)
-        if not model and not raise_e: return model
+        if not model and not raise_e:
+            return model
         cls.types(model)
-        if fill: cls.fill(model, safe = rules)
-        if build: cls.build(model, map = map, rules = rules, meta = meta)
-        if eager: model = cls._eager(model, eager, map = map)
-        if resolve_a: model = cls._resolve_all(model, resolve = False)
-        return model if map else cls.old(model = model, safe = False)
+        if fill:
+            cls.fill(model, safe=rules)
+        if build:
+            cls.build(model, map=map, rules=rules, meta=meta)
+        if eager:
+            model = cls._eager(model, eager, map=map)
+        if resolve_a:
+            model = cls._resolve_all(model, resolve=False)
+        return model if map else cls.old(model=model, safe=False)
 
     @classmethod
     def find(cls, *args, **kwargs):
-        fields,\
-        eager,\
-        eager_l,\
-        map,\
-        rules,\
-        meta,\
-        build,\
-        fill,\
-        resolve_a,\
-        skip,\
-        limit,\
-        sort,\
-        raise_e = cls._get_attrs(kwargs, (
-            ("fields", None),
-            ("eager", None),
-            ("eager_l", False),
-            ("map", False),
-            ("rules", True),
-            ("meta", False),
-            ("build", True),
-            ("fill", True),
-            ("resolve_a", None),
-            ("skip", 0),
-            ("limit", 0),
-            ("sort", None),
-            ("raise_e", False)
-        ))
+        (
+            fields,
+            eager,
+            eager_l,
+            map,
+            rules,
+            meta,
+            build,
+            fill,
+            resolve_a,
+            skip,
+            limit,
+            sort,
+            raise_e,
+        ) = cls._get_attrs(
+            kwargs,
+            (
+                ("fields", None),
+                ("eager", None),
+                ("eager_l", False),
+                ("map", False),
+                ("rules", True),
+                ("meta", False),
+                ("build", True),
+                ("fill", True),
+                ("resolve_a", None),
+                ("skip", 0),
+                ("limit", 0),
+                ("sort", None),
+                ("raise_e", False),
+            ),
+        )
 
         # in case there's a sort field and the safe search mode is enabled
         # we must add sorting by the `_id` field so that the search is
         # considered to be deterministic, otherwise some DB implementations
         # will not respect the same sorting sequence across different calls
         if sort and (skip or limit):
-            if not isinstance(sort, list): sort = list(sort)
+            if not isinstance(sort, list):
+                sort = list(sort)
             sort.append(["_id", 1])
 
-        if resolve_a == None: resolve_a = map
-        if eager_l: eager = cls._eager_b(eager)
+        if resolve_a == None:
+            resolve_a = map
+        if eager_l:
+            eager = cls._eager_b(eager)
 
         cls._find_s(kwargs)
         cls._find_d(kwargs)
 
-        fields = cls._sniff(fields, rules = rules)
+        fields = cls._sniff(fields, rules=rules)
         collection = cls._collection()
-        models = collection.find(
-            kwargs,
-            fields,
-            skip = skip,
-            limit = limit,
-            sort = sort
-        )
+        models = collection.find(kwargs, fields, skip=skip, limit=limit, sort=sort)
         if not models and raise_e:
             is_devel = common.is_devel()
-            if is_devel: message = "%s not found for %s" % (cls.__name__, str(kwargs))
-            else: message = "%s not found" % cls.__name__
+            if is_devel:
+                message = "%s not found for %s" % (cls.__name__, str(kwargs))
+            else:
+                message = "%s not found" % cls.__name__
             raise exceptions.NotFoundError(message)
         models = [cls.types(model) for model in models]
-        if fill: models = [cls.fill(model, safe = rules) for model in models]
-        if build: [cls.build(model, map = map, rules = rules, meta = meta) for model in models]
-        if eager: models = cls._eager(models, eager, map = map)
-        if resolve_a: models = [cls._resolve_all(model, resolve = False) for model in models]
-        models = models if map else [cls.old(model = model, safe = False) for model in models]
+        if fill:
+            models = [cls.fill(model, safe=rules) for model in models]
+        if build:
+            [cls.build(model, map=map, rules=rules, meta=meta) for model in models]
+        if eager:
+            models = cls._eager(models, eager, map=map)
+        if resolve_a:
+            models = [cls._resolve_all(model, resolve=False) for model in models]
+        models = (
+            models if map else [cls.old(model=model, safe=False) for model in models]
+        )
         return models
 
     @classmethod
     def count(cls, *args, **kwargs):
         cls._clean_attrs(kwargs)
 
         cls._find_s(kwargs)
@@ -624,15 +631,15 @@
             if hasattr(collection, "count_documents"):
                 result = collection.count_documents()
             else:
                 result = collection.count()
         return result
 
     @classmethod
-    def paginate(cls, skip = 0, limit = 1, *args, **kwargs):
+    def paginate(cls, skip=0, limit=1, *args, **kwargs):
         # counts the total number of references according to the
         # current filter value and then uses this value together
         # with the skip value to calculate both the number of pages
         # available for the current filter and the current page index
         # (note that the index is one index based)
         total = cls.count(*args, **kwargs)
         count = total / float(limit)
@@ -641,103 +648,119 @@
         index = skip / float(limit)
         index = math.floor(index)
         index = int(index) + 1
 
         # calculates the proper size of the current page being requested
         # taking into account the total number of values and the limit
         size = total % limit if index == count else limit
-        if size == 0 and total > 0: size = limit
-        if total == 0: size = 0
+        if size == 0 and total > 0:
+            size = limit
+        if total == 0:
+            size = 0
 
         # creates the base structure for the page populating with the
         # base values that may be used for display of the page
         page = dict(
-            count = count,
-            index = index,
-            start = skip + 1,
-            end = skip + limit,
-            size = size,
-            total = total,
-            sorter = flask.request.args_s.get("sorter", None),
-            direction = flask.request.args_s.get("direction", "descending")
+            count=count,
+            index=index,
+            start=skip + 1,
+            end=skip + limit,
+            size=size,
+            total=total,
+            sorter=flask.request.args_s.get("sorter", None),
+            direction=flask.request.args_s.get("direction", "descending"),
         )
 
         def generate(**kwargs):
             # creates the linear parameters list that is going to hold multiple
             # key and value tuple representing the multiple parameters
             params_l = []
 
             # creates a copy of the current definition of the parameters and for each
             # of the exclusion parameters removes it from the current structure
             params = dict(flask.request.args_s)
-            if "async" in params: del params["async"]
+            if "async" in params:
+                del params["async"]
 
             # retrieves the "special" sorter keyword based argument and the equivalent
             # values for the current page in handling, this values are going to be used
             # for the calculus of the direction value (in case it's required)
             sorter = kwargs.get("sorter", None)
             _sorter = page["sorter"]
             direction = page["direction"]
             reverse = REVERSE.get(direction, "descending")
 
             # verifies if the sorter value is defined in the arguments and if that's
             # the case verifies if it's the same as the current one if that the case
             # the direction must be reversed otherwise the default direction is set
-            if sorter and sorter == _sorter: params["direction"] = reverse
-            elif sorter: params["direction"] = "descending"
+            if sorter and sorter == _sorter:
+                params["direction"] = reverse
+            elif sorter:
+                params["direction"] = "descending"
 
             # "copies" the complete set of values from the provided keyword
             # based arguments into the parameters map, properly converting them
             # into the proper string value (avoiding possible problems)
-            for key, value in kwargs.items(): params[key] = str(value)
+            for key, value in kwargs.items():
+                params[key] = str(value)
 
             # iterates over the complete set of parameters to be sent to linearize
             # them into a sequence of tuples ready to be converted into quoted string
             for key, value in params.items():
                 is_list = isinstance(value, (list, tuple))
-                if not is_list: value = [value]
-                for _value in value: params_l.append((key, _value))
+                if not is_list:
+                    value = [value]
+                for _value in value:
+                    params_l.append((key, _value))
 
             # converts the multiple parameters to be used into a linear
             # quoted manner so they they may be used as query string values
-            query = [util.quote(key) + "=" + util.quote(value) for key, value in params_l]
+            query = [
+                util.quote(key) + "=" + util.quote(value) for key, value in params_l
+            ]
             query = "&".join(query)
             return "?" + query if query else query
 
         # updates the current page structure so that the (query) generation
         # method is exposed in order to modify the current query
         page["query"] = generate
         return page
 
     @classmethod
     def delete_c(cls, *args, **kwargs):
         collection = cls._collection()
         collection.remove(kwargs)
 
     @classmethod
-    def ordered(cls, filter = dict):
+    def ordered(cls, filter=dict):
         is_sequence = isinstance(filter, (list, tuple))
-        if not is_sequence: filter = (filter,)
+        if not is_sequence:
+            filter = (filter,)
 
         ordered = list(cls._ordered)
 
         for name, value in cls.__dict__.items():
-            if name.startswith("_"): continue
-            if not name == name.lower(): continue
-            if not isinstance(value, filter): continue
-            if name in ordered: continue
+            if name.startswith("_"):
+                continue
+            if not name == name.lower():
+                continue
+            if not isinstance(value, filter):
+                continue
+            if name in ordered:
+                continue
             ordered.append(name)
 
         return ordered
 
     @classmethod
     def methods(cls):
         # in case the methods are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_methods" in cls.__dict__: return cls._methods
+        if "_methods" in cls.__dict__:
+            return cls._methods
 
         # starts the list that will hold the various method names
         # for the class, note that this value will be ordered
         # according to the class level and the definition order
         methods = []
 
         # retrieves the complete model hierarchy for the current model
@@ -745,32 +768,28 @@
         # in a top to bottom approach strategy
         hierarchy = cls.hierarchy()
 
         # iterates over the complete model hierarchy and retrieves the
         # ordered set of attributes from it extending the retrieved methods
         # list with the value for each of the model levels
         for _cls in hierarchy:
-            ordered = _cls.ordered(
-                filter = (
-                    types.FunctionType,
-                    classmethod
-                )
-            )
+            ordered = _cls.ordered(filter=(types.FunctionType, classmethod))
             methods.extend(ordered)
 
         # saves the retrieved set of methods in the current model definition
         # and then returns the value to the caller method as requested
         cls._methods = methods
         return methods
 
     @classmethod
     def fields(cls):
         # in case the fields are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_fields" in cls.__dict__: return cls._fields
+        if "_fields" in cls.__dict__:
+            return cls._fields
 
         # starts the list that will hold the various field names
         # for the class, note that this value will be ordered
         # according to the class level and the definition order
         fields = []
 
         # retrieves the complete model hierarchy for the current model
@@ -790,15 +809,16 @@
         cls._fields = fields
         return fields
 
     @classmethod
     def definition(cls):
         # in case the definition is already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_definition" in cls.__dict__: return cls._definition
+        if "_definition" in cls.__dict__:
+            return cls._definition
 
         # creates the map that will hold the complete definition of
         # the current model
         definition = {}
 
         # retrieves the complete model hierarchy for the current model
         # this should allow the method to retrieve the complete set
@@ -806,20 +826,25 @@
         hierarchy = cls.hierarchy()
 
         # iterates over all the classes in the hierarchy to creates the
         # map that will contain the various names of the current model
         # associated with its definition map
         for _cls in hierarchy:
             for name, value in _cls.__dict__.items():
-                if name.startswith("_"): continue
-                if not name == name.lower(): continue
-                if not isinstance(value, dict): continue
-                if name in definition: raise exceptions.OperationalError(
-                    "Duplicated attribute '%s' in '%s' hierarchy" % (name, _cls.__name__)
-                )
+                if name.startswith("_"):
+                    continue
+                if not name == name.lower():
+                    continue
+                if not isinstance(value, dict):
+                    continue
+                if name in definition:
+                    raise exceptions.OperationalError(
+                        "Duplicated attribute '%s' in '%s' hierarchy"
+                        % (name, _cls.__name__)
+                    )
                 definition[name] = value
 
         # sets the "default" definition for the based identifier
         # (underlying identifier attribute)
         definition["_id"] = dict()
 
         # saves the currently generated definition under the current
@@ -827,15 +852,16 @@
         cls._definition = definition
         return definition
 
     @classmethod
     def definition_extended(cls):
         # in case the definition extended is already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_definition_extended" in cls.__dict__: return cls._definition_extended
+        if "_definition_extended" in cls.__dict__:
+            return cls._definition_extended
 
         # retrieves the base definition dictionary and duplicated it adding
         # the element present in the set of extra definition (overridable on
         # a per model basis, providing extension)
         definition_extended = dict(cls.definition())
         definition_extended.update(cls.extra_definition())
 
@@ -844,64 +870,68 @@
         cls._definition_extended = definition_extended
         return definition_extended
 
     @classmethod
     def links(cls):
         # in case the links are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_links" in cls.__dict__: return cls._links
+        if "_links" in cls.__dict__:
+            return cls._links
 
         # creates the list that will hold the complete set of method
         # names for links type methods
         links = []
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be link oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are links
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_link"): continue
+            if not hasattr(method, "_link"):
+                continue
             reference = hasattr(method, "__self__") and method.__self__
             is_instance = False if reference else True
             method._link["instance"] = is_instance
             links.append(method._link)
 
         # sorts the various links taking into account the name of
         # the link, this is considered the pre-defined order
-        links.sort(key = lambda item: item["name"])
+        links.sort(key=lambda item: item["name"])
 
         # saves the list of link method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._links = links
         return links
 
     @classmethod
     def links_m(cls):
         # in case the links are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_links_m" in cls.__dict__: return cls._links_m
+        if "_links_m" in cls.__dict__:
+            return cls._links_m
 
         # creates the map that will hold the complete set of method
         # names for links type methods
         links_m = dict()
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be link oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are links
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_link"): continue
+            if not hasattr(method, "_link"):
+                continue
             links_m[method.__name__] = method._link
 
         # saves the map of link method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._links_m = links_m
         return links_m
 
@@ -910,64 +940,68 @@
         links_m = cls.links_m()
         return links_m.get(name, None)
 
     @classmethod
     def operations(cls):
         # in case the operations are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_operations" in cls.__dict__: return cls._operations
+        if "_operations" in cls.__dict__:
+            return cls._operations
 
         # creates the list that will hold the complete set of method
         # names for operations type methods
         operations = []
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be operation oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are operations
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_operation"): continue
+            if not hasattr(method, "_operation"):
+                continue
             reference = hasattr(method, "__self__") and method.__self__
             is_instance = False if reference else True
             method._operation["instance"] = is_instance
             operations.append(method._operation)
 
         # sorts the various operations taking into account the name of
         # the operation, this is considered the pre-defined order
-        operations.sort(key = lambda item: item["name"])
+        operations.sort(key=lambda item: item["name"])
 
         # saves the list of operation method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._operations = operations
         return operations
 
     @classmethod
     def operations_m(cls):
         # in case the operations are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_operations_m" in cls.__dict__: return cls._operations_m
+        if "_operations_m" in cls.__dict__:
+            return cls._operations_m
 
         # creates the map that will hold the complete set of method
         # names for operations type methods
         operations_m = dict()
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be operation oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are operations
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_operation"): continue
+            if not hasattr(method, "_operation"):
+                continue
             operations_m[method.__name__] = method._operation
 
         # saves the map of operation method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._operations_m = operations_m
         return operations_m
 
@@ -976,64 +1010,68 @@
         operations_m = cls.operations_m()
         return operations_m.get(name, None)
 
     @classmethod
     def views(cls):
         # in case the views are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_views" in cls.__dict__: return cls._views
+        if "_views" in cls.__dict__:
+            return cls._views
 
         # creates the list that will hold the complete set of method
         # names for views type methods
         views = []
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be view oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are views
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_view"): continue
+            if not hasattr(method, "_view"):
+                continue
             reference = hasattr(method, "__self__") and method.__self__
             is_instance = False if reference else True
             method._view["instance"] = is_instance
             views.append(method._view)
 
         # sorts the various views taking into account the name of
         # the view, this is considered the pre-defined order
-        views.sort(key = lambda item: item["name"])
+        views.sort(key=lambda item: item["name"])
 
         # saves the list of view method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._views = views
         return views
 
     @classmethod
     def views_m(cls):
         # in case the views are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_views_m" in cls.__dict__: return cls._views_m
+        if "_views_m" in cls.__dict__:
+            return cls._views_m
 
         # creates the map that will hold the complete set of method
         # names for views type methods
         views_m = dict()
 
         # retrieves the complete set of method names for the current
         # class this is going to be used to determine the ones that
         # are considered to be view oriented
         methods = cls.methods()
 
         # iterates over the complete set of method names for the current
         # class hierarchy to determine the ones that are views
         for name in methods:
             method = getattr(cls, name)
-            if not hasattr(method, "_view"): continue
+            if not hasattr(method, "_view"):
+                continue
             views_m[method.__name__] = method._view
 
         # saves the map of view method names defined under the current
         # class and then returns the contents of it to the caller method
         cls._views_m = views_m
         return views_m
 
@@ -1041,25 +1079,28 @@
     def view(cls, name):
         views_m = cls.views_m()
         return views_m.get(name, None)
 
     @classmethod
     def definition_n(cls, name):
         definition = cls.definition_extended()
-        if not name in definition: return {}
+        if not name in definition:
+            return {}
         return definition[name]
 
     @classmethod
-    def register(cls, lazy = False):
-        if lazy: return
+    def register(cls, lazy=False):
+        if lazy:
+            return
         cls.setup()
 
     @classmethod
-    def unregister(cls, lazy = False):
-        if lazy: return
+    def unregister(cls, lazy=False):
+        if lazy:
+            return
         cls.teardown()
 
     @classmethod
     def setup(cls):
         cls._build_indexes()
 
     @classmethod
@@ -1094,17 +1135,19 @@
     @classmethod
     def show_names(cls):
         _names = []
         names = cls.base_names()
         definition = cls.definition()
         for name in names:
             value = definition.get(name, None)
-            if value == None: continue
+            if value == None:
+                continue
             is_private = value.get("private", False)
-            if is_private: continue
+            if is_private:
+                continue
             _names.append(name)
         return _names
 
     @classmethod
     def list_names(cls):
         return cls.show_names()
 
@@ -1121,41 +1164,47 @@
         return None
 
     @classmethod
     def extra_definition(cls):
         return {}
 
     @classmethod
-    def build(cls, model, map = False, rules = True, meta = False):
-        if rules: cls.rules(model, map)
+    def build(cls, model, map=False, rules=True, meta=False):
+        if rules:
+            cls.rules(model, map)
         cls._build(model, map)
-        if meta: cls._meta(model, map)
+        if meta:
+            cls._meta(model, map)
 
     @classmethod
     def rules(cls, model, map):
         for name, _value in legacy.eager(model.items()):
             definition = cls.definition_n(name)
             is_private = definition.get("private", False)
-            if not is_private: continue
+            if not is_private:
+                continue
             del model[name]
 
     @classmethod
     def types(cls, model):
         definition = cls.definition()
 
         for name, value in legacy.eager(model.items()):
-            if name == "_id": continue
-            if value == None: continue
-            if not name in definition: continue
+            if name == "_id":
+                continue
+            if value == None:
+                continue
+            if not name in definition:
+                continue
             model[name] = cls.cast(name, value)
 
         return model
 
     @classmethod
-    def fill(cls, model = None, safe = False):
+    def fill(cls, model=None, safe=False):
         """
         Fills the current model with the proper values so that
         no values are unset as this would violate the model definition
         integrity. This is required when retrieving an object(s) from
         the data source (as some of them may be incomplete).
 
         :type model: Model
@@ -1167,43 +1216,50 @@
         operation meaning that under some conditions no unit fill
         operation is going to be applied (eg: retrieval operations).
         """
 
         model = model or dict()
         definition = cls.definition()
         for name, _definition in definition.items():
-            if name in model: continue
-            if name in ("_id",): continue
+            if name in model:
+                continue
+            if name in ("_id",):
+                continue
             private = _definition.get("private", False)
             increment = _definition.get("increment", False)
-            if private and safe: continue
-            if increment: continue
+            if private and safe:
+                continue
+            if increment:
+                continue
             if "initial" in _definition:
                 initial = _definition["initial"]
                 model[name] = initial
             else:
                 _type = _definition.get("type")
                 default = type_d(_type, None)
                 default = _type._default() if hasattr(_type, "_default") else default
                 model[name] = default
 
         return model
 
     @classmethod
-    def cast(cls, name, value, safe = True):
+    def cast(cls, name, value, safe=True):
         definition = cls.definition()
-        if not name in definition: return value
-        if value == None: return value
+        if not name in definition:
+            return value
+        if value == None:
+            return value
         _definition = cls.definition_n(name)
         _type = _definition.get("type", legacy.UNICODE)
         builder = BUILDERS.get(_type, _type)
         try:
             return builder(value) if builder else value
         except Exception:
-            if not safe: raise
+            if not safe:
+                raise
             default = type_d(_type, None)
             default = _type._default() if hasattr(_type, "_default") else default
             return default
 
     @classmethod
     def to_description(cls, name):
         """
@@ -1234,20 +1290,21 @@
 
         # tries to retrieve the info dictionary for the attribute
         # name and then uses it to retrieve the possible manual
         # description value for the field, returning immediately
         # the value if there's success
         info = cls.definition_n(name)
         description = info.get("description", None)
-        if description: return description
+        if description:
+            return description
 
         # because there's no explicit description defined
         # runs the automatic underscore to readable conversion
         # and sets the value on the field info dictionary
-        description = util.underscore_to_readable(name, capitalize = True)
+        description = util.underscore_to_readable(name, capitalize=True)
         info["description"] = description
         return description
 
     @classmethod
     def to_observations(cls, name):
         # runs the (possibly) recursive class resolution process
         # so that in case the provided name is namespace based,
@@ -1261,15 +1318,16 @@
         info = cls.definition_n(name)
         return info.get("observations", None)
 
     @classmethod
     def all_parents(cls):
         # in case the all parents are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_all_parents" in cls.__dict__: return cls._all_parents
+        if "_all_parents" in cls.__dict__:
+            return cls._all_parents
 
         # creates the list to hold the various parent
         # entity classes, populated recursively
         all_parents = []
 
         # retrieves the parent entity classes from
         # the current class
@@ -1297,15 +1355,16 @@
         # entity classes
         return all_parents
 
     @classmethod
     def hierarchy(cls):
         # in case the hierarchy are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_hierarchy" in cls.__dict__: return cls._hierarchy
+        if "_hierarchy" in cls.__dict__:
+            return cls._hierarchy
 
         # retrieves the complete set of parents for the current class
         # and then adds the current class to it
         all_parents = cls.all_parents()
         hierarchy = all_parents + [cls]
 
         # saves the current hierarchy list under the class and then
@@ -1313,69 +1372,74 @@
         cls._hierarchy = hierarchy
         return hierarchy
 
     @classmethod
     def increments(cls):
         # in case the increments are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_increments" in cls.__dict__: return cls._increments
+        if "_increments" in cls.__dict__:
+            return cls._increments
 
         # creates the list that will hold the various names that are
         # meant to be automatically incremented
         increments = []
 
         # retrieves the map containing the definition of the class with
         # the name of the fields associated with their definition
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type increment
         for name in definition:
             _definition = cls.definition_n(name)
             is_increment = _definition.get("increment", False)
-            if not is_increment: continue
+            if not is_increment:
+                continue
             increments.append(name)
 
         # saves the increment list under the class and then
         # returns the sequence to the caller method
         cls._increments = increments
         return increments
 
     @classmethod
     def indexes(cls):
         # in case the indexes are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_indexes" in cls.__dict__: return cls._indexes
+        if "_indexes" in cls.__dict__:
+            return cls._indexes
 
         # creates the list that will hold the various names that are
         # meant to be indexed in the data source
         indexes = []
 
         # retrieves the map containing the definition of the class with
         # the name of the fields associated with their definition
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type index
         for name in definition:
             _definition = cls.definition_n(name)
             direction = _definition.get("index", False)
-            if not direction: continue
+            if not direction:
+                continue
             indexes.append((name, direction))
 
         # saves the index list under the class and then
         # returns the sequence to the caller method
         cls._indexes = indexes
         return indexes
 
     @classmethod
     def safes(cls):
         # in case the safes are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_safes" in cls.__dict__: return cls._safes
+        if "_safes" in cls.__dict__:
+            return cls._safes
 
         # creates the list that will hold the various names that are
         # meant to be safe values in the data source, the underlying
         # identifier is set as the initial safe value of a model
         safes = ["_id"]
 
         # retrieves the map containing the definition of the class with
@@ -1383,81 +1447,87 @@
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type safe
         for name in definition:
             _definition = cls.definition_n(name)
             is_safe = _definition.get("safe", False)
-            if not is_safe: continue
+            if not is_safe:
+                continue
             safes.append(name)
 
         # saves the safes list under the class and then
         # returns the sequence to the caller method
         cls._safes = safes
         return safes
 
     @classmethod
     def immutables(cls):
         # in case the immutables are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_immutables" in cls.__dict__: return cls._immutables
+        if "_immutables" in cls.__dict__:
+            return cls._immutables
 
         # creates the list that will hold the various names that are
         # meant to be immutable values in the data source
         immutables = []
 
         # retrieves the map containing the definition of the class with
         # the name of the fields associated with their definition
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type immutable
         for name in definition:
             _definition = cls.definition_n(name)
             is_immutable = _definition.get("immutable", False)
-            if not is_immutable: continue
+            if not is_immutable:
+                continue
             immutables.append(name)
 
         # saves the immutables list under the class and then
         # returns the sequence to the caller method
         cls._immutables = immutables
         return immutables
 
     @classmethod
     def eagers(cls):
         # in case the eagers are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_eagers" in cls.__dict__: return cls._eagers
+        if "_eagers" in cls.__dict__:
+            return cls._eagers
 
         # creates the list that will hold the various names that are
         # meant to be eager values in the data source
         eagers = []
 
         # retrieves the map containing the definition of the class with
         # the name of the fields associated with their definition
         definition = cls.definition()
 
         # iterate over all the names in the definition to retrieve their
         # definition and check if their are of type eager
         for name in definition:
             _definition = cls.definition_n(name)
             is_eager = _definition.get("eager", False)
-            if not is_eager: continue
+            if not is_eager:
+                continue
             eagers.append(name)
 
         # saves the eagers list under the class and then
         # returns the sequence to the caller method
         cls._eagers = eagers
         return eagers
 
     @classmethod
     def default(cls):
         # in case the default are already "cached" in the current
         # class (fast retrieval) returns immediately
-        if "_default" in cls.__dict__: return cls._default
+        if "_default" in cls.__dict__:
+            return cls._default
 
         # retrieves the complete hierarchy of the model to be used
         # for the retrieval of the lowest possible default value for
         # the current class hierarchy
         hierarchy = cls.hierarchy()
 
         # creates the value that is going to store the default value for
@@ -1470,32 +1540,34 @@
         for _cls in reversed(hierarchy):
             for name in legacy.eager(_cls.__dict__.keys()):
                 # retrieves the definition map for the current name an in
                 # case the default value is set considers it default otherwise
                 # continues the loop, nothing to be done
                 _definition = cls.definition_n(name)
                 is_default = _definition.get("default", False)
-                if not is_default: continue
+                if not is_default:
+                    continue
 
                 # in case the default value is found sets its name in the
                 # current default value and then breaks the loop
                 default = name
                 break
 
             # in case the default value has been found must break the external
             # loop as nothing else remains to be found
-            if default: break
+            if default:
+                break
 
         # saves the default value (name) under the class and then
         # returns the sequence to the caller method
         cls._default = default
         return default
 
     @classmethod
-    def filter_merge(cls, name, filter, kwargs, operator = None):
+    def filter_merge(cls, name, filter, kwargs, operator=None):
         # retrieves a possible previous filter defined for the
         # provided name in case it does exist must concatenate
         # that previous value in a join statement according to
         # the currently defined operator
         filter_p = kwargs.get(name, None)
         if filter_p or not operator == None:
             # defaults the operator for the join of the names to the
@@ -1505,17 +1577,20 @@
             util.verify(operator in ("$and", "$or"))
 
             # retrieves the and references for the current arguments
             # and appends the two filter values (current and previous)
             # then deletes the current name reference in the arguments
             # and updates the name value to the and value
             filter_a = kwargs.get(operator, [])
-            if filter_p: filter = filter_a + [{name : filter}, {name : filter_p}]
-            else: filter = filter_a + [{name : filter}]
-            if name in kwargs: del kwargs[name]
+            if filter_p:
+                filter = filter_a + [{name: filter}, {name: filter_p}]
+            else:
+                filter = filter_a + [{name: filter}]
+            if name in kwargs:
+                del kwargs[name]
             name = operator
 
         # sets the currently defined filter structures in the keyword
         # based arguments map for the currently defined name
         kwargs[name] = filter
 
     @classmethod
@@ -1528,58 +1603,63 @@
 
     @classmethod
     def is_attached(cls):
         return True
 
     @classmethod
     def is_concrete(cls):
-        if not "is_abstract" in cls.__dict__: return True
+        if not "is_abstract" in cls.__dict__:
+            return True
         return not cls.is_abstract()
 
     @classmethod
     def is_child(cls, parent):
         return issubclass(cls, parent)
 
     @classmethod
     def is_equal(cls, other):
-        if not cls._name() == other._name(): return False
-        if not cls.__name__ == other.__name__: return False
+        if not cls._name() == other._name():
+            return False
+        if not cls.__name__ == other.__name__:
+            return False
         return True
 
     @classmethod
     def assert_is_attached_g(cls):
-        if cls.is_attached(): return
+        if cls.is_attached():
+            return
         raise exceptions.OperationalError("Model is not attached")
 
     @classmethod
     def assert_is_concrete_g(cls):
-        if cls.is_concrete(): return
+        if cls.is_concrete():
+            return
         raise exceptions.OperationalError("Model is not concrete")
 
     @classmethod
     def assert_is_child_g(cls, parent):
-        if cls.is_child(parent): return
+        if cls.is_child(parent):
+            return
         raise exceptions.OperationalError("Model is not child of %s" % parent)
 
     @classmethod
     def _build(cls, model, map):
         pass
 
     @classmethod
-    def _meta(cls, model, map, safe = True):
+    def _meta(cls, model, map, safe=True):
         # iterates over the complete set of keys and values for the
         # current model map to try to compute the associated meta value
         # for all of its attributes (should use some computation)
         for key, value in legacy.items(model):
             # verifies if the current value in iteration is either
             # unset (none) or an unloaded  reference, if that's the
             # case the value is considered "invalid" not to be encoded
             is_reference = isinstance(value, TYPE_REFERENCES)
-            is_invalid = value == None or\
-                (is_reference and not value.is_resolved())
+            is_invalid = value == None or (is_reference and not value.is_resolved())
 
             # retrieves the definition for the current key in iteration
             # so that it's possible to apply the mapper
             definition = cls.definition_n(key)
 
             # resolves the proper meta value for the key, meaning that if
             # the type of the current field is a class all the mro of it
@@ -1588,82 +1668,88 @@
             meta = cls._solve(key)
             mapper = METAS.get(meta, None)
 
             # in case there's a valid mapper function and the value is not
             # invalid calls the proper mapper function otherwise runs the
             # default (fallback) operation for meta retrieval
             try:
-                if mapper and not is_invalid: value = mapper(value, definition, cls)
-                else: value = value if is_invalid else legacy.UNICODE(value)
+                if mapper and not is_invalid:
+                    value = mapper(value, definition, cls)
+                else:
+                    value = value if is_invalid else legacy.UNICODE(value)
             except Exception:
-                if not safe: raise
+                if not safe:
+                    raise
                 value = None
 
             # sets the final meta value in the model, so that it may be
             # latter retrieved.
             model[key + "_meta"] = value
 
     @classmethod
-    def _sniff(cls, fields, rules = False):
+    def _sniff(cls, fields, rules=False):
         fields = fields or cls.fields()
         fields = list(fields)
-        if not rules: return fields
+        if not rules:
+            return fields
         for field in list(fields):
             definition = cls.definition_n(field)
             is_private = definition.get("private", False)
-            if is_private: fields.remove(field)
+            if is_private:
+                fields.remove(field)
         return fields
 
     @classmethod
     def _solve(cls, name):
         definition = cls.definition_n(name)
         type = definition.get("type", legacy.UNICODE)
         for cls in type.mro():
             base = TYPE_META.get(cls, None)
-            if base: break
+            if base:
+                break
         return definition.get("meta", base)
 
     @classmethod
     def _adapter(cls):
         return common.base().get_adapter()
 
     @classmethod
     def _encoder(cls):
         adapter = cls._adapter()
         encoder = adapter.encoder()
         return encoder
 
     @classmethod
-    def _collection(cls, name = None):
+    def _collection(cls, name=None):
         name = name or cls._name()
         adapter = cls._adapter()
         collection = adapter.collection(name)
         return collection
 
     @classmethod
     def _name(cls):
         # retrieves the class object for the current instance and then
         # converts it into lower case value in order to serve as the
         # name of the collection to be used
         name = cls.__name__.lower()
         return name
 
     @classmethod
-    def _under(cls, plural = True):
-        return cls._underscore(plural = plural)
+    def _under(cls, plural=True):
+        return cls._underscore(plural=plural)
 
     @classmethod
-    def _underscore(cls, plural = True):
+    def _underscore(cls, plural=True):
         camel = cls._plural() if plural else cls._singular()
         return util.camel_to_underscore(camel)
 
     @classmethod
-    def _readable(cls, plural = False):
+    def _readable(cls, plural=False):
         camel = cls._plural() if plural else cls._singular()
-        return util.camel_to_readable(camel, capitalize = True)
+        return util.camel_to_readable(camel, capitalize=True)
 
     @classmethod
     def _singular(cls):
         return cls.__name__
 
     @classmethod
     def _plural(cls):
@@ -1688,26 +1774,32 @@
         :return: The resulting model with the required relations loaded.
         """
 
         # verifies if the provided model instance is a sequence and if
         # that's the case runs the recursive eager loading of names and
         # returns the resulting sequence to the caller method
         is_list = isinstance(model, (list, tuple))
-        if is_list: return [cls._eager(_model, names, *args, **kwargs) for _model in model]
+        if is_list:
+            return [cls._eager(_model, names, *args, **kwargs) for _model in model]
 
         # iterates over the complete set of names that are meant to be
         # eager loaded from the model and runs the "resolution" process
         # for each of them so that they are properly eager loaded
         for name in names:
             _model = model
             for part in name.split("."):
                 is_sequence = isinstance(_model, (list, tuple))
-                if is_sequence: _model = [cls._res(value, part, *args, **kwargs) for value in _model]
-                else: _model = cls._res(_model, part, *args, **kwargs)
-                if not _model: break
+                if is_sequence:
+                    _model = [
+                        cls._res(value, part, *args, **kwargs) for value in _model
+                    ]
+                else:
+                    _model = cls._res(_model, part, *args, **kwargs)
+                if not _model:
+                    break
 
         # returns the resulting model to the caller method, most of the
         # times this model should have not been touched
         return model
 
     @classmethod
     def _res(cls, model, part, *args, **kwargs):
@@ -1728,35 +1820,39 @@
         :rtype: Dictionary/Object
         :return: The resolved part that may be either a map or an object
         depending on the resolution strategy.
         """
 
         # in case the provided is not valid returns it (no resolution is
         # possible) otherwise gather the base value for resolution
-        if not model: return model
+        if not model:
+            return model
         value = model[part]
 
         # check the data type of the requested name for resolution
         # and in case it's not valid and not a reference returns it
         # immediately, no resolution to be performed
         is_reference = isinstance(value, TYPE_REFERENCES)
-        if not value and not is_reference: return value
+        if not value and not is_reference:
+            return value
 
         # in case the value is a reference type object then runs
         # the resolve operation effectively resolving the values
         # (this is considered a very expensive operation), notice
         # that this operation is going to respect the map vs. instance
         # kind of resolution process so the data type of the resulting
         # value is going to depend on that
-        if is_reference: value = value.resolve(eager_l = True, *args, **kwargs)
+        if is_reference:
+            value = value.resolve(eager_l=True, *args, **kwargs)
 
         # in case the map resolution process was requested an explicit
         # set of the resolved value is required (implicit resolution
         # using `resolve()`) is not enough to ensure proper type structure
-        if kwargs.get("map", False): model[part] = value
+        if kwargs.get("map", False):
+            model[part] = value
 
         # returns the "final" (possibly resolved) value to the caller method
         # ready to be used for possible merging processes
         return value
 
     @classmethod
     def _res_cls(cls, name):
@@ -1772,15 +1868,16 @@
         :return: The target class that represents the reference attribute
         described by the namespace (path) based name and the name of the
         final attribute contained in it.
         """
 
         # in case the provided name is a simple one this is a direct attribute
         # of the current class and the expected tuple is returned immediately
-        if not "." in name: return cls, name
+        if not "." in name:
+            return cls, name
 
         # splits the namespace recursive name and then iterates over the multiple
         # relation attributes to retrieve their respective targets
         name_s = name.split(".")
         for part in name_s[:-1]:
             info = getattr(cls, part) if hasattr(cls, part) else dict()
             part_type = info.get("type", None)
@@ -1802,17 +1899,18 @@
             value = kwargs[attr]
             del kwargs[attr]
             _attrs.append(value)
 
         return _attrs
 
     @classmethod
-    def _clean_attrs(cls, kwargs, dirty = DIRTY_PARAMS):
+    def _clean_attrs(cls, kwargs, dirty=DIRTY_PARAMS):
         for key in dirty:
-            if not key in kwargs: continue
+            if not key in kwargs:
+                continue
             del kwargs[key]
 
     @classmethod
     def _find_s(cls, kwargs):
         # tries to retrieve the find name value from the provided
         # named arguments defaulting to an unset value otherwise
         find_n = kwargs.pop("find_n", None)
@@ -1836,29 +1934,31 @@
             del kwargs["find_t"]
         else:
             find_t = "both"
 
         # in case the find string is currently not defined in the
         # named arguments map returns immediately as nothing is
         # meant to be done on this method
-        if not "find_s" in kwargs: return
+        if not "find_s" in kwargs:
+            return
 
         # retrieves the find string into a local variable, then
         # removes the find string from the named arguments map
         # so that it's not going to be erroneously used by the
         # underlying find infra-structure
         find_s = kwargs["find_s"]
         del kwargs["find_s"]
 
         # retrieves the "name" of the attribute that is considered
         # to be the default (representation) for the model in case
         # there's none returns immediately, as it's not possible
         # to proceed with the filter creation
         default = find_n or cls.default()
-        if not default: return
+        if not default:
+            return
 
         # constructs the proper right and left parts of the regex
         # that is going to be constructed for the matching of the
         # value, this is achieved by checking the find type
         right = "^" if find_t == "right" else ""
         left = "$" if find_t == "left" else ""
 
@@ -1869,19 +1969,21 @@
         default_t = definition.get("type", legacy.UNICODE)
 
         try:
             # in case the target date type for the default field is
             # string the both sides wildcard regex is used for the
             # search otherwise the search value to be used is the
             # exact match of the value (required type conversion)
-            if default_t in legacy.STRINGS: find_v = {
-                "$regex" : right + re.escape(find_s) + left,
-                "$options": "i" if find_i else ""
-            }
-            else: find_v = default_t(find_s)
+            if default_t in legacy.STRINGS:
+                find_v = {
+                    "$regex": right + re.escape(find_s) + left,
+                    "$options": "i" if find_i else "",
+                }
+            else:
+                find_v = default_t(find_s)
         except Exception:
             # in case there's an error in the conversion for
             # the target type value sets the search value as
             # invalid (not going to be used in filter)
             find_v = None
 
         # in case there's a valid find value to be used sets
@@ -1892,15 +1994,16 @@
             cls.filter_merge(default, find_v, kwargs)
 
     @classmethod
     def _find_d(cls, kwargs):
         # in case the find definition is currently not defined in the
         # named arguments map returns immediately as nothing is
         # meant to be done on this method
-        if not "find_d" in kwargs: return
+        if not "find_d" in kwargs:
+            return
 
         # tries to retrieve the value of the operator that is going
         # to be used to "join" the multiple find parts (find values)
         find_o = kwargs.pop("find_o", None)
 
         # retrieves the find definition into a local variable, then
         # removes the find definition from the named arguments map
@@ -1908,39 +2011,44 @@
         # underlying find infra-structure
         find_d = kwargs["find_d"]
         del kwargs["find_d"]
 
         # verifies that the data type for the find definition is a
         # valid sequence and in case its not converts it into one
         # so that it may be used in sequence valid logic
-        if not isinstance(find_d, list): find_d = [find_d]
+        if not isinstance(find_d, list):
+            find_d = [find_d]
 
         # iterates over all the filters defined in the filter definition
         # so that they may be used to update the provided arguments with
         # the filter defined in each of their lines
         for filter in find_d:
             # in case the filter is not valid (unset or invalid) it's going
             # to be ignored as no valid information is present
-            if not filter: continue
+            if not filter:
+                continue
 
             # splits the filter string into its three main components
             # the name, operator and value, that are going to be processed
             # as defined by the specification to create the filter
             result = filter.split(":", 2)
-            if len(result) == 2: result.append(None)
+            if len(result) == 2:
+                result.append(None)
             name, operator, value = result
 
             # retrieves the definition for the filter attribute and uses
             # it to retrieve it's target data type that is going to be
             # used for the proper conversion, note that in case the base
             # type resolution method exists it's used (recursive resolution)
             definition = cls.definition_n(name)
             name_t = definition.get("type", legacy.UNICODE)
-            if hasattr(name_t, "_btype"): name_t = name_t._btype()
-            if name in ("_id",): name_t = cls._adapter().object_id
+            if hasattr(name_t, "_btype"):
+                name_t = name_t._btype()
+            if name in ("_id",):
+                name_t = cls._adapter().object_id
 
             # determines if the current filter operation should be performed
             # using a case insensitive based approach to the search, by default
             # all of the operations are considered to be case sensitive
             insensitive = INSENSITIVE.get(operator, False)
 
             # retrieves the method that is going to be used for value mapping
@@ -1948,29 +2056,33 @@
             # the operator into the domain specific operator
             value_method = VALUE_METHODS.get(operator, None)
             operator = OPERATORS.get(operator, operator)
 
             # in case there's a custom value mapped retrieved uses it to convert
             # the string based value into the target specific value for the query
             # otherwise uses the data type for the search field for value conversion
-            if value_method: value = value_method(value, name_t)
+            if value_method:
+                value = value_method(value, name_t)
             else:
-                try: value = name_t(value)
-                except ValueError: value = None
+                try:
+                    value = name_t(value)
+                except ValueError:
+                    value = None
 
             # constructs the custom find value using a key and value map value
             # in case the operator is defined otherwise (operator not defined)
             # the value is used directly, then merges this find value into the
             # current set of filters for the provided (keyword) arguments
-            find_v = {operator : value} if operator else value
-            if insensitive: find_v["$options"] = "i"
-            cls.filter_merge(name, find_v, kwargs, operator = find_o)
+            find_v = {operator: value} if operator else value
+            if insensitive:
+                find_v["$options"] = "i"
+            cls.filter_merge(name, find_v, kwargs, operator=find_o)
 
     @classmethod
-    def _bases(cls, subclass = None):
+    def _bases(cls, subclass=None):
         """
         Retrieves the complete set of base (parent) classes for
         the current class, this method is safe as it removes any
         class that does not inherit from the entity class.
 
         Please note that this function only retrieves the set of
         direct parents of the class and not the complete hierarchy.
@@ -1992,70 +2104,50 @@
         # the current class and in case the observable is
         # not in the bases set returns the set immediately
         # as the top level model has not been reached yet,
         # note that the various base classes are filtered
         # according to their inheritance from the provided
         # (model) class to be applied as filter
         bases = cls.__bases__
-        if subclass: bases = [base for base in bases if issubclass(base, subclass)]
-        if not bases == Model.__bases__: return bases
+        if subclass:
+            bases = [base for base in bases if issubclass(base, subclass)]
+        if not bases == Model.__bases__:
+            return bases
 
         # returns an empty tuple to the caller method as the
         # top level class has been reached and the class is
         # considered to have no "valid" base classes
         return ()
 
     @classmethod
     def _increment(cls, name):
         _name = cls._name() + ":" + name
-        store = cls._collection(name = "counters")
+        store = cls._collection(name="counters")
         value = store.find_and_modify(
-            {
-                "_id" : _name
-            },
-            {
-                "$inc" : {
-                    "seq" : 1
-                }
-            },
-            new = True,
-            upsert = True
+            {"_id": _name}, {"$inc": {"seq": 1}}, new=True, upsert=True
         )
-        value = value or store.find_one({
-            "_id" : _name
-        })
+        value = value or store.find_one({"_id": _name})
         return value["seq"]
 
     @classmethod
     def _ensure_min(cls, name, value):
         _name = cls._name() + ":" + name
-        store = cls._collection(name = "counters")
+        store = cls._collection(name="counters")
         value = store.find_and_modify(
-            {
-                "_id" : _name
-            },
-            {
-                "$max" : {
-                    "seq" : value
-                }
-            },
-            new = True,
-            upsert = True
+            {"_id": _name}, {"$max": {"seq": value}}, new=True, upsert=True
         )
-        value = value or store.find_one({
-            "_id" : _name
-        })
+        value = value or store.find_one({"_id": _name})
         return value["seq"]
 
     @classmethod
     def _build_indexes(cls):
         indexes = cls.indexes()
         collection = cls._collection()
         for index, direction in indexes:
-            collection.ensure_index(index, direction = direction)
+            collection.ensure_index(index, direction=direction)
 
     @classmethod
     def _destroy_indexes(cls):
         collection = cls._collection()
         collection.drop_indexes()
 
     @classmethod
@@ -2075,60 +2167,67 @@
         :return: The "final" resolved tuple that may be used for the eager
         loaded operation performance.
         """
 
         eager = list(eager) if eager else []
         eagers = cls.eagers()
         eager.extend(eagers)
-        if not eager: return eager
+        if not eager:
+            return eager
         eager = tuple(set(eager))
         return eager
 
     @classmethod
     def _resolve_all(cls, model, *args, **kwargs):
         definition = cls.definition()
         for name, value in legacy.eager(model.items()):
-            if not name in definition: continue
+            if not name in definition:
+                continue
             model[name] = cls._resolve(name, value, *args, **kwargs)
         return model
 
     @classmethod
     def _resolve(cls, name, value, *args, **kwargs):
         # verifies if the current value is an iterable one in case
         # it is runs the evaluate method for each of the values to
         # try to resolve them into the proper representation
         is_iterable = isinstance(value, (list, tuple))
-        if is_iterable: return [cls._resolve(name, value, *args, **kwargs) for value in value]
+        if is_iterable:
+            return [cls._resolve(name, value, *args, **kwargs) for value in value]
 
         # in case the current instance is a dictionary then, and in case
         # there's a target class (typical for reference like types) recursion
         # steps must be token, allowing proper normalized and resolved data
         # to exist in the complete deep and nested data hierarchy, this is
         # relevant only when the underlying structure is map oriented
         if isinstance(value, dict):
             info = getattr(cls, name)
             part_type = info.get("type", None)
-            if hasattr(part_type, "_target") :
+            if hasattr(part_type, "_target"):
                 _cls = part_type._target()
                 return _cls._resolve_all(value, *args, **kwargs)
 
         # verifies if the map value recursive approach should be used
         # for the element and if that's the case calls the proper method
         # otherwise uses the provided (raw value)
-        if not hasattr(value, "map_v"): return value
+        if not hasattr(value, "map_v"):
+            return value
         return value.map_v(*args, **kwargs)
 
     @classmethod
     def _to_meta(cls, base):
-        if isinstance(base, str): return base
+        if isinstance(base, str):
+            return base
         is_class = inspect.isclass(type)
-        if not is_class: base = base.__class__
+        if not is_class:
+            base = base.__class__
         for cls in base.mro():
             result = TYPE_META.get(cls, None)
-            if not result: continue
+            if not result:
+                continue
             return result
         return base
 
     @property
     def request(self):
         return flask.request
 
@@ -2136,34 +2235,32 @@
     def session(self):
         return flask.session
 
     @property
     def logger(self):
         return None
 
-    def val(self, name, default = None):
+    def val(self, name, default=None):
         return self.model.get(name, default)
 
     def json_v(self, *args, **kwargs):
         return self.model
 
     def map_v(self, *args, **kwargs):
         cls = self.__class__
         clone = kwargs.pop("clone", False)
         resolve = kwargs.get("resolve", True)
         evaluator = kwargs.get("evaluator", "map_v")
-        if clone: base = self.clone(reset = False, deep = True)
-        else: base = self
-        return cls._resolve_all(
-            base.model,
-            resolve = resolve,
-            evaluator = evaluator
-        )
+        if clone:
+            base = self.clone(reset=False, deep=True)
+        else:
+            base = self
+        return cls._resolve_all(base.model, resolve=resolve, evaluator=evaluator)
 
-    def build_m(self, model = None, rules = True):
+    def build_m(self, model=None, rules=True):
         """
         Builds the currently defined model, this should run
         additional computation for the current model creating
         new (calculated) attributes and deleting other.
 
         The extra rules parameters allows for the (security) rules
         to be applied to the model, used this with care to avoid
@@ -2179,17 +2276,17 @@
         :type rules: bool
         :param rules: If the (security) rules should be applied to
         the model that is going to be built.
         """
 
         cls = self.__class__
         model = model or self.model
-        cls.build(model, rules = rules)
+        cls.build(model, rules=rules)
 
-    def apply(self, model = None, form = True, safe = None, safe_a = True):
+    def apply(self, model=None, form=True, safe=None, safe_a=True):
         # calls the complete set of event handlers for the current
         # apply operation, this should trigger changes in the model
         self.pre_apply()
 
         # retrieves the reference to the class associated
         # with the current instance
         cls = self.__class__
@@ -2198,52 +2295,57 @@
         # builds a new map that will hold these values
         safe = safe or {}
 
         # verifies if the base safe rules should be applied
         # to the current map of safe attributes
         if safe_a:
             safes = cls.safes()
-            for _safe in safes: safe[_safe] = True
+            for _safe in safes:
+                safe[_safe] = True
 
         # retrieves the object loading it from all the available
         # sources and then iterates over all the of the model
         # values setting the values in the current instance's model
         # then runs the type casting/conversion operation in it
-        if model == None: model = util.get_object() if form else dict()
+        if model == None:
+            model = util.get_object() if form else dict()
         for name, value in legacy.eager(model.items()):
             is_safe = safe.get(name, False)
-            if is_safe: continue
+            if is_safe:
+                continue
             self.model[name] = value
         cls = self.__class__
         cls.types(self.model)
 
         # calls the complete set of event handlers for the current
         # apply operation, this should trigger changes in the model
         self.post_apply()
 
         # returns the instance that has just been used for the apply
         # operation, this may be used for chaining operations
         return self
 
-    def copy(self, build = False, rules = True):
+    def copy(self, build=False, rules=True):
         cls = self.__class__
         _copy = copy.deepcopy(self)
-        build and cls.build(_copy.model, map = False, rules = rules)
+        build and cls.build(_copy.model, map=False, rules=rules)
         return _copy
 
-    def clone(self, reset = True, deep = False):
+    def clone(self, reset=True, deep=False):
         cls = self.__class__
         model = dict(self.model) if deep else self.model
-        if not reset: return cls(model = model)
+        if not reset:
+            return cls(model=model)
         indexes = cls.increments()
         indexes = indexes + cls.unique_names() + ["_id"]
         for index in indexes:
-            if not index in model: continue
+            if not index in model:
+                continue
             del model[index]
-        return cls(model = model)
+        return cls(model=model)
 
     def validate_extra(self, name):
         """
         Adds a new validate method to the current set of
         validate methods to be executed on the next validation
         execution. Note this validate method will only be used
         on the next validation execution, after that execution
@@ -2271,15 +2373,16 @@
         update permissions for situations where only creation is allowed.
 
         The method raises an exception if the current instance is not
         considered to be a new one causing the current control flow to
         be returned to the caller method until catching of exception.
         """
 
-        if self.is_new(): return
+        if self.is_new():
+            return
         raise exceptions.OperationalError("Instance is not new, identifier is set")
 
     def assert_is_attached(self):
         cls = self.__class__
         cls.assert_is_attached_g()
 
     def assert_is_concrete(self):
@@ -2288,211 +2391,212 @@
 
     def assert_is_child(self, parent):
         cls = self.__class__
         cls.assert_is_child_g(parent)
 
     def save(
         self,
-        validate = True,
-        verify = True,
-        is_new = None,
-        increment_a = None,
-        immutables_a = None,
-        pre_validate = True,
-        pre_save = True,
-        pre_create = True,
-        pre_update = True,
-        post_validate = True,
-        post_save = True,
-        post_create = True,
-        post_update = True,
-        before_callbacks = [],
-        after_callbacks = []
+        validate=True,
+        verify=True,
+        is_new=None,
+        increment_a=None,
+        immutables_a=None,
+        pre_validate=True,
+        pre_save=True,
+        pre_create=True,
+        pre_update=True,
+        post_validate=True,
+        post_save=True,
+        post_create=True,
+        post_update=True,
+        before_callbacks=[],
+        after_callbacks=[],
     ):
         # ensures that the current instance is associated with
         # a concrete model, ready to be persisted in database
-        if verify: self.assert_is_concrete()
+        if verify:
+            self.assert_is_concrete()
 
         # checks if the instance to be saved is a new instance
         # or if this is an update operation and then determines
         # series of default values taking that into account
-        if is_new == None: is_new = self.is_new()
-        if increment_a == None: increment_a = is_new
-        if immutables_a == None: immutables_a = not is_new
+        if is_new == None:
+            is_new = self.is_new()
+        if increment_a == None:
+            increment_a = is_new
+        if immutables_a == None:
+            immutables_a = not is_new
 
         # runs the validation process in the current model, this
         # should ensure that the model is ready to be saved in the
         # data source, without corruption of it, only run this process
         # in case the validate flag is correctly set
         validate and self._validate(
-            pre_validate = pre_validate,
-            post_validate = post_validate
+            pre_validate=pre_validate, post_validate=post_validate
         )
 
         # calls the complete set of event handlers for the current
         # save operation, this should trigger changes in the model
-        if pre_save: self.pre_save()
-        if pre_create and is_new: self.pre_create()
-        if pre_update and not is_new: self.pre_update()
+        if pre_save:
+            self.pre_save()
+        if pre_create and is_new:
+            self.pre_create()
+        if pre_update and not is_new:
+            self.pre_update()
 
         # filters the values that are present in the current model
         # so that only the valid ones are stored in, invalid values
         # are going to be removed, note that if the operation is an
         # update operation and the "immutable rules" also apply, the
         # returned value is normalized meaning that for instance if
         # any relation is loaded the reference value is returned instead
         # of the loaded relation values (required for persistence)
         model = self._filter(
-            increment_a = increment_a,
-            immutables_a = immutables_a,
-            normalize = True
+            increment_a=increment_a, immutables_a=immutables_a, normalize=True
         )
 
         # in case the current model is not new must create a new
         # model instance and remove the main identifier from it
-        if not is_new: _model = copy.copy(model); del _model["_id"]
+        if not is_new:
+            _model = copy.copy(model)
+            del _model["_id"]
 
         # calls the complete set of callbacks that should be called
         # before the concrete data store save operation
-        for callback in before_callbacks: callback(self, model)
+        for callback in before_callbacks:
+            callback(self, model)
 
         # retrieves the reference to the store object to be used and
         # uses it to store the current model data
         store = self._get_store()
         if is_new:
             store.insert(model)
-            self.apply(model, safe_a = False)
+            self.apply(model, safe_a=False)
         else:
-            store.update({"_id" : model["_id"]}, {"$set" : _model})
+            store.update({"_id": model["_id"]}, {"$set": _model})
 
         # calls the complete set of callbacks that should be called
         # after the concrete data store save operation
-        for callback in after_callbacks: callback(self, model)
+        for callback in after_callbacks:
+            callback(self, model)
 
         # calls the post save event handlers in order to be able to
         # execute appropriate post operations
-        if post_save: self.post_save()
-        if post_create and is_new: self.post_create()
-        if post_update and not is_new: self.post_update()
+        if post_save:
+            self.post_save()
+        if post_create and is_new:
+            self.post_create()
+        if post_update and not is_new:
+            self.post_update()
 
         # returns the instance that has just been used for the save
         # operation, this may be used for chaining operations
         return self
 
     def delete(
         self,
-        verify = True,
-        pre_delete = True,
-        post_delete = True,
-        before_callbacks = [],
-        after_callbacks = []
+        verify=True,
+        pre_delete=True,
+        post_delete=True,
+        before_callbacks=[],
+        after_callbacks=[],
     ):
         # ensures that the current instance is associated with
         # a concrete model, ready to be persisted in database
-        if verify: self.assert_is_concrete()
+        if verify:
+            self.assert_is_concrete()
 
         # calls the complete set of event handlers for the current
         # delete operation, this should trigger changes in the model
-        if pre_delete: self.pre_delete()
+        if pre_delete:
+            self.pre_delete()
 
         # calls the complete set of callbacks that should be called
         # before the concrete data store delete operation
-        for callback in before_callbacks: callback(self)
+        for callback in before_callbacks:
+            callback(self)
 
         # retrieves the reference to the store object to be able to
         # execute the removal command for the current model
         store = self._get_store()
-        store.remove({"_id" : self._id})
+        store.remove({"_id": self._id})
 
         # calls the underlying delete handler that may be used to extend
         # the default delete functionality
         self._delete()
 
         # calls the complete set of callbacks that should be called
         # after the concrete data store delete operation
-        for callback in after_callbacks: callback(self)
+        for callback in after_callbacks:
+            callback(self)
 
         # calls the complete set of event handlers for the current
         # delete operation, this should trigger changes in the model
-        if post_delete: self.post_delete()
+        if post_delete:
+            self.post_delete()
 
-    def approve(self, model = None, type = None):
+    def approve(self, model=None, type=None):
         # retrieves the class associated with the instance
         # that is going to be sent for approval
         cls = self.__class__
 
         # determines the proper method naming suffix to be
         # used for the requested type of approval/validation
         suffix = "_" + type if type else ""
 
         # retrieves the proper (target) method for validation
         # and then runs the inner validate method for it
         method = getattr(cls, "validate" + suffix)
-        self._validate(model = model, method = method)
+        self._validate(model=model, method=method)
 
         # returns the instance that has just been used for the approve
         # operation, this may be used for chaining operations
         return self
 
-    def advance(self, name, delta = 1):
+    def advance(self, name, delta=1):
         store = self._get_store()
         value = store.find_and_modify(
-            {
-                "_id" : self._id
-            },
-            {
-                "$inc" : {
-                    name : delta
-                }
-            },
-            new = True
+            {"_id": self._id}, {"$inc": {name: delta}}, new=True
         )
-        value = value or store.find_one({
-            "_id" : self._id
-        })
+        value = value or store.find_one({"_id": self._id})
         _value = value[name]
         setattr(self, name, _value)
         return _value
 
     def reload(self, *args, **kwargs):
         is_new = self.is_new()
-        if is_new: exceptions.OperationalError("Can't reload a new model entity")
+        if is_new:
+            exceptions.OperationalError("Can't reload a new model entity")
         cls = self.__class__
-        return cls.get(_id = self._id, *args, **kwargs)
+        return cls.get(_id=self._id, *args, **kwargs)
 
     def exists(self):
         is_new = self.is_new()
-        if is_new: return False
-        entity = self.get(_id = self._id, raise_e = False)
+        if is_new:
+            return False
+        entity = self.get(_id=self._id, raise_e=False)
         return True if entity else False
 
-    def map(
-        self,
-        increment_a = False,
-        resolve = False,
-        all = False,
-        evaluator = "map_v"
-    ):
+    def map(self, increment_a=False, resolve=False, all=False, evaluator="map_v"):
         model = self._filter(
-            increment_a = increment_a,
-            resolve = resolve,
-            all = all,
-            evaluator = evaluator
+            increment_a=increment_a, resolve=resolve, all=all, evaluator=evaluator
         )
         return model
 
-    def dumps(self, encode = True):
+    def dumps(self, encode=True):
         cls = self.__class__
         encoder = cls._encoder() if encode else None
-        return json.dumps(self.model, cls = encoder)
+        return json.dumps(self.model, cls=encoder)
 
     def unwrap(self, **kwargs):
         default = kwargs.get("default", False)
-        if default: return self.map()
-        else: return dict()
+        if default:
+            return self.map()
+        else:
+            return dict()
 
     def pre_validate(self):
         self.trigger("pre_validate")
 
     def pre_save(self):
         self.trigger("pre_save")
 
@@ -2528,88 +2632,81 @@
 
     def _get_store(self):
         return self.__class__._collection()
 
     def _delete(self):
         pass
 
-    def _validate(
-        self,
-        model = None,
-        method = None,
-        pre_validate = True,
-        post_validate = True
-    ):
+    def _validate(self, model=None, method=None, pre_validate=True, post_validate=True):
         # calls the event handler for the validation process this
         # should setup the operations for a correct validation
-        if pre_validate: self.pre_validate()
+        if pre_validate:
+            self.pre_validate()
 
         # starts the model reference with the current model in
         # case none is defined
         model = model or self.model
 
         # retrieves the class associated with the current instance
         # to be able to retrieve the correct validate methods
         cls = self.__class__
 
         # checks if the current model is new (create operation)
         # and sets the proper validation methods retrieval method
         is_new = self.is_new()
-        if is_new: method = method or cls.validate_new
-        else: method = method or cls.validate
+        if is_new:
+            method = method or cls.validate_new
+        else:
+            method = method or cls.validate
 
         # runs the validation process on the various arguments
         # provided to the account and in case an error is returned
         # raises a validation error to the upper layers
         errors, object = validation.validate(
-            method,
-            object = model,
-            ctx = self,
-            build = False
+            method, object=model, ctx=self, build=False
         )
 
         # iterates over the complete set of extra validate method
         # and runs their validations for the current model context
         # adding their errors to the existing map (appending) this
         # will make sure that these extra validation remains transparent
         # from an end-user point of view (as expected)
         for extra in self._extras:
             _errors, _object = validation.validate(
-                extra,
-                object = model,
-                ctx = self,
-                build = False
+                extra, object=model, ctx=self, build=False
             )
             for key, value in _errors.items():
                 errors_l = errors.get(key, [])
                 _errors_l = value
                 errors_l.extend(_errors_l)
                 errors[key] = errors_l
 
         # empties the extras list so that the methods that have been
         # set there are not going to be used in any further validation
         del self._extras[:]
 
         # in case the errors map is not empty or invalid there are
         # errors and they should be encapsulated around a validation
         # error and raises to the top layer for handling
-        if errors: raise exceptions.ValidationError(errors, self)
+        if errors:
+            raise exceptions.ValidationError(errors, self)
 
         # calls the event handler for the validation process this
         # should finish the operations from a correct validation
-        if post_validate: self.post_validate()
+        if post_validate:
+            self.post_validate()
 
     def _filter(
         self,
-        increment_a = True,
-        immutables_a = False,
-        normalize = False,
-        resolve = False,
-        all = False,
-        evaluator = "json_v"
+        increment_a=True,
+        immutables_a=False,
+        normalize=False,
+        resolve=False,
+        all=False,
+        evaluator="json_v",
     ):
         # creates the model that will hold the "filtered" model
         # with all the items that conform with the class specification
         model = {}
 
         # retrieves the class associated with the current instance
         # to be able to retrieve the correct definition methods
@@ -2629,91 +2726,103 @@
         # apply the filter is not a new operation (update operation)
         immutables = cls.immutables()
 
         # iterates over all the increment fields and increments their
         # fields so that a new value is set on the model, note that if
         # the increment apply is unset the increment operation is ignored
         for name in increments:
-            if not increment_a: continue
+            if not increment_a:
+                continue
             if name in self.model:
                 model[name] = cls._ensure_min(name, self.model[name])
             else:
                 model[name] = cls._increment(name)
 
         # iterates over all the model items to filter the ones
         # that are not valid for the current class context
         for name, value in legacy.eager(self.model.items()):
-            if not name in definition: continue
-            if immutables_a and name in immutables: continue
-            value = self._evaluate(name, value, evaluator = evaluator)
+            if not name in definition:
+                continue
+            if immutables_a and name in immutables:
+                continue
+            value = self._evaluate(name, value, evaluator=evaluator)
             model[name] = value
 
         # in case the normalize flag is set must iterate over all
         # items to try to normalize the values by calling the reference
         # value this will returns the reference index value instead of
         # the normal value that would prevent normalization
         if normalize:
             for name, value in legacy.eager(self.model.items()):
-                if not name in definition: continue
-                if not hasattr(value, "ref_v"): continue
+                if not name in definition:
+                    continue
+                if not hasattr(value, "ref_v"):
+                    continue
                 model[name] = value.ref_v()
 
         # in case the resolution flag is set, it means that a recursive
         # approach must be performed for the resolution of values that
         # implement the map value (recursive resolution) method, this is
         # a complex (and possible computational expensive) process that
         # may imply access to the base data source
         if resolve:
             for name, value in legacy.eager(self.model.items()):
-                if not name in definition: continue
+                if not name in definition:
+                    continue
                 model[name] = cls._resolve(name, value)
 
         # in case the all flag is set the extra fields (not present
         # in definition) must also be used to populate the resulting
         # (filtered) map so that it contains the complete set of values
         # present in the base map of the current instance
         if all:
             for name, value in legacy.eager(self.model.items()):
-                if name in model: continue
+                if name in model:
+                    continue
                 model[name] = value
 
         # returns the model containing the "filtered" items resulting
         # from the validation of the items against the model class
         return model
 
-    def _evaluate(self, name, value, evaluator = "json_v"):
+    def _evaluate(self, name, value, evaluator="json_v"):
         # verifies if the current value is an iterable one in case
         # it is runs the evaluate method for each of the values to
         # try to resolve them into the proper representation, note
         # that both base iterable values (lists and dictionaries) and
         # objects that implement the evaluator method are not considered
         # to be iterables and normal operation applies
         is_iterable = hasattr(value, "__iter__")
-        is_iterable = is_iterable and not isinstance(value, ITERABLES) and\
-           (not hasattr(value, evaluator) or not evaluator)
-        if is_iterable: return [
-            self._evaluate(name, value, evaluator = evaluator) for\
-            value in value
-        ]
+        is_iterable = (
+            is_iterable
+            and not isinstance(value, ITERABLES)
+            and (not hasattr(value, evaluator) or not evaluator)
+        )
+        if is_iterable:
+            return [self._evaluate(name, value, evaluator=evaluator) for value in value]
 
         # verifies the current value's class is sub class of the model
         # class and in case it's extracts the relation name from the
         # value and sets it as the value in iteration
         is_model = issubclass(value.__class__, Model)
         if is_model:
             meta = getattr(self.__class__, name)
             _type = meta.get("type", legacy.BYTES)
             _name = _type._name
             value = getattr(value, _name)
 
         # iterates over all the values and retrieves the map value for
         # each of them in case the value contains a map value retrieval
         # method otherwise uses the normal value returning it to the caller
-        method = getattr(value, evaluator) if evaluator and hasattr(value, evaluator) else None
-        value = method(resolve = False) if method else value
+        method = (
+            getattr(value, evaluator)
+            if evaluator and hasattr(value, evaluator)
+            else None
+        )
+        value = method(resolve=False) if method else value
         return value
 
     def _res_entity(self, name, *args, **kwargs):
         """
         Tries to retrieve the relation entity value associated with the
         provided namespace based name.
 
@@ -2729,15 +2838,16 @@
         :rtype: Tuple
         :return: A tuple containing both the final leaf entity instance and
         the final single level name to be used to retrieve the attribute.
         """
 
         # in case the provided name is a simple one this is a direct attribute
         # of the current entity and so the expected values are returned
-        if not "." in name: return self, name
+        if not "." in name:
+            return self, name
 
         # sets the initial entity value for iteration as the current instance
         # (root node) and then splits the name around its components
         entity = self
         name_s = name.split(".")
 
         # runs the iterative process to obtain the final leaf entity by using
@@ -2745,28 +2855,30 @@
         for part in name_s[:-1]:
             entity = entity[part].resolve(*args, **kwargs)
 
         # returns the final tuple containing both the leaf entity and the
         # final name of the attribute on the leaf node
         return entity, name_s[-1]
 
+
 class LocalModel(Model):
     """
     Concrete model aimed at cases where data source based
     persistence is not required, while the remainder model
     features are useful.
 
     Typical uses cases involve API based validation or local
     transient model usage.
     """
 
     @classmethod
     def is_attached(cls):
         return False
 
+
 class Field(dict):
     """
     Top level field class that should be used for the
     definition of the various fields of the model, a
     dictionary may be sued alternatively but some of the
     ordering features and other are going o be lost.
     """
@@ -2779,32 +2891,35 @@
 
     def __init__(self, *args, **kwargs):
         dict.__init__(self, *args, **kwargs)
         self.creation_counter = Field.creation_counter
         Field.creation_counter += 1
 
     def __getattr__(self, name):
-        if name in self: return self[name]
+        if name in self:
+            return self[name]
         raise AttributeError("'%s' not found" % name)
 
+
 class Action(dict):
     """
     The abstract class that defines an action to be performed
     by an end used this should be used as a placeholder for
     the generic logic of any action.
 
     The base interface should conform with the dictionary
     interface in order to provide backwards compatibility.
     """
 
     def __getattr__(self, name):
-        if name in self: return self[name]
+        if name in self:
+            return self[name]
         raise AttributeError("'%s' not found" % name)
 
-    def cast(self, values, keyword = False):
+    def cast(self, values, keyword=False):
         """
         Runs the "casting" operation for a series of provided
         values, the order sequence of the provided values is
         relevant and should conform with the specified order
         for the operation parameters.
 
         :type values: List
@@ -2829,57 +2944,59 @@
         parameters = self.get("parameters", [])
         for value, parameters in zip(values, parameters):
             name = parameters[1]
             type = parameters[2]
             cast = type
             is_default = value in (None, "")
             cast = BUILDERS.get(cast, cast)
-            if cast and not is_default: value = cast(value)
-            if is_default: value = type_d(type, value)
-            if keyword: casted[name] = value
-            else: casted.append(value)
+            if cast and not is_default:
+                value = cast(value)
+            if is_default:
+                value = type_d(type, value)
+            if keyword:
+                casted[name] = value
+            else:
+                casted.append(value)
 
         # returns the final list/map of casted values to the caller method
         # so that it may be used safely in the context
         return casted
 
+
 class Link(Action):
     """
     Internal link class used to encapsulate some of the
     internal concepts associated with a link, providing
     an easy to use structure at runtime.
     """
 
     pass
 
+
 class Operation(Action):
     """
     Logical structure representing an operation, should
     provide a simple interface for interaction with the
     operation and inputs/outputs of it.
     """
 
     pass
 
+
 class View(Action):
     """
     Definition associated with a model that represents
     the information to be used for the display of associated
     set of elements/items of a model.
     """
 
     pass
 
-def link(
-    name = None,
-    description = None,
-    parameters = (),
-    context = False,
-    devel = False
-):
+
+def link(name=None, description=None, parameters=(), context=False, devel=False):
     """
     Decorator function to be used to "annotate" the provided
     function as an link (string) that is able to change the user
     agent to a location of a certain interest.
 
     Proper usage of the link definition/decoration is context
     based and should vary based on application.
@@ -2902,33 +3019,34 @@
     :rtype: Function
     :return: The decorator function that is going to be used to
     generated the final function to be called.
     """
 
     def decorator(function, *args, **kwargs):
         function._link = Link(
-            method = function.__name__,
-            name = name or function.__name__,
-            description = description,
-            parameters = parameters,
-            context = context,
-            devel = devel
+            method=function.__name__,
+            name=name or function.__name__,
+            description=description,
+            parameters=parameters,
+            context=context,
+            devel=devel,
         )
         return function
 
     return decorator
 
+
 def operation(
-    name = None,
-    description = None,
-    parameters = (),
-    kwargs = None,
-    factory = False,
-    level = 1,
-    devel = False
+    name=None,
+    description=None,
+    parameters=(),
+    kwargs=None,
+    factory=False,
+    level=1,
+    devel=False,
 ):
     """
     Decorator function to be used to "annotate" the provided
     function as an operation that is able to change the current
     entity state and behavior.
 
     Proper usage of the operation definition/decoration is context
@@ -2962,34 +3080,30 @@
     generated the final function to be called.
     """
 
     _kwargs = kwargs
 
     def decorator(function, *args, **kwargs):
         function._operation = Operation(
-            method = function.__name__,
-            name = name or function.__name__,
-            description = description,
-            parameters = parameters,
-            kwargs = _kwargs,
-            factory = factory,
-            level = level,
-            devel = devel
+            method=function.__name__,
+            name=name or function.__name__,
+            description=description,
+            parameters=parameters,
+            kwargs=_kwargs,
+            factory=factory,
+            level=level,
+            devel=devel,
         )
 
         return function
 
     return decorator
 
-def view(
-    name = None,
-    description = None,
-    parameters = (),
-    devel = False
-):
+
+def view(name=None, description=None, parameters=(), devel=False):
     """
     Decorator function to be used to "annotate" the provided
     function as an view that is able to return a set of configurations
     for the proper display of associated information.
 
     Proper usage of the view definition/decoration is context
     based and should vary based on application.
@@ -3009,26 +3123,27 @@
     :rtype: Function
     :return: The decorator function that is going to be used to
     generated the final function to be called.
     """
 
     def decorator(function, *args, **kwargs):
         function._view = View(
-            method = function.__name__,
-            name = name or function.__name__,
-            description = description,
-            parameters = parameters,
-            devel = devel
+            method=function.__name__,
+            name=name or function.__name__,
+            description=description,
+            parameters=parameters,
+            devel=devel,
         )
 
         return function
 
     return decorator
 
-def type_d(type, default = None):
+
+def type_d(type, default=None):
     """
     Retrieves the default (initial) value for the a certain
     provided data type falling back to the provided default
     value in case it's not possible to retrieve a new valid
     default for value for the type.
 
     The process of retrieval of the default value to a certain
@@ -3044,19 +3159,22 @@
     :param default: The default value to be returned in case it's
     not possible to retrieve a better one.
     :rtype: Object
     :return: The "final" default value for the data type according
     to the best possible strategy.
     """
 
-    if not type in TYPE_DEFAULTS: return default
+    if not type in TYPE_DEFAULTS:
+        return default
     default = TYPE_DEFAULTS[type]
-    if not hasattr(default, "__call__"): return default
+    if not hasattr(default, "__call__"):
+        return default
     return default()
 
+
 def is_unset(value):
     """
     Verifies if the provided value is unset trying the multiple
     approaches available for such verification, notice that some
     of the verifications imply resolution (data source access) and
     as such are considered to be very expensive.
 
@@ -3065,13 +3183,15 @@
     value, if it's a reference an expensive operation of resolution
     may be performed.
     :rtype: bool
     :return: If the provided value is unset/invalid according to the
     underlying promises of the data type of the provided value.
     """
 
-    if value == None: return True
-    if isinstance(value, typesf.Reference) and\
-        not value.is_resolvable(): return True
+    if value == None:
+        return True
+    if isinstance(value, typesf.Reference) and not value.is_resolvable():
+        return True
     return False
 
+
 field = Field
```

### Comparing `quorum-0.8.2/src/quorum/extras.py` & `quorum-0.8.3/src/quorum/extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,42 +18,34 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import flask
 
 YEAR_IN_SECS = 31536000
 """ The number of seconds that exist in a
 complete year (365 days) """
 
+
 class SSLify(object):
     """
     Secures your flask app by enabling the forcing
     of the protocol in the HTTP connection.
     """
 
-    def __init__(self, app, age = YEAR_IN_SECS, subdomains = False):
+    def __init__(self, app, age=YEAR_IN_SECS, subdomains=False):
         """
         Constructor of the class.
 
         :type app: App
         :param app: The application object to be used in the
         in SSL operation for the forcing of the protocol.
         :type age: int
@@ -90,15 +82,16 @@
         Returns the proper hsts policy.
 
         :rtype: String
         :return: The proper hsts policy string value.
         """
 
         hsts_policy = "max-age={0}".format(self.hsts_age)
-        if self.hsts_include_subdomains: hsts_policy += "; includeSubDomains"
+        if self.hsts_include_subdomains:
+            hsts_policy += "; includeSubDomains"
 
         return hsts_policy
 
     def redirect_to_ssl(self):
         """
         Redirect incoming requests to HTTPS in case the current
         protocol is not considered secure.
@@ -109,19 +102,21 @@
         :rtype: Request
         :return: The changed request containing the redirect
         instruction in case it's required.
         """
 
         criteria = [
             flask.request.is_secure,
-            flask.request.headers.get("X-Forwarded-Proto", "http") == "https"
+            flask.request.headers.get("X-Forwarded-Proto", "http") == "https",
         ]
 
-        if any(criteria): return
-        if not flask.request.url.startswith("http://"): return
+        if any(criteria):
+            return
+        if not flask.request.url.startswith("http://"):
+            return
 
         url = flask.request.url.replace("http://", "https://", 1)
         request = flask.redirect(url)
         return request
 
     def set_hsts_header(self, response):
         """
```

### Comparing `quorum-0.8.2/src/quorum/observer.py` & `quorum-0.8.3/src/quorum/observer.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,31 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class Observable(object):
     """
     The base class that implements the observable
     patter allowing the object to handle a series of
     event in a dynamic fashion.
 
     The class should be able to handle both context
@@ -64,73 +56,89 @@
     def name_f(cls, name):
         cls_name = cls.__name__
         cls_name = util.camel_to_underscore(cls_name)
         name_f = cls_name + "." + name
         return name_f
 
     @classmethod
-    def bind_g(cls, name, method, oneshot = False):
-        if oneshot: method.oneshot = oneshot
+    def bind_g(cls, name, method, oneshot=False):
+        if oneshot:
+            method.oneshot = oneshot
         name_f = cls.name_f(name)
         methods = cls._events_g.get(name_f, [])
         methods.append(method)
         cls._events_g[name_f] = methods
 
     @classmethod
-    def unbind_g(cls, name, method = None):
+    def unbind_g(cls, name, method=None):
         name_f = cls.name_f(name)
         methods = cls._events_g.get(name_f, [])
-        if method: methods.remove(method)
-        else: del methods[:]
+        if method:
+            methods.remove(method)
+        else:
+            del methods[:]
 
     @classmethod
     def trigger_g(cls, name, *args, **kwargs):
         oneshots = None
         name_f = cls.name_f(name)
         methods = cls._events_g.get(name_f, [])
         for method in methods:
             method(*args, **kwargs)
-            if not hasattr(method, "oneshot"): continue
-            if not method.oneshot: continue
+            if not hasattr(method, "oneshot"):
+                continue
+            if not method.oneshot:
+                continue
             oneshots = [] if oneshots == None else oneshots
             oneshots.append(method)
-        if not oneshots: return
-        for oneshot in oneshots: cls.unbind_g(name, oneshot)
+        if not oneshots:
+            return
+        for oneshot in oneshots:
+            cls.unbind_g(name, oneshot)
 
     def build(self):
         pass
 
     def destroy(self):
         self.unbind_all()
 
-    def bind(self, name, method, oneshot = False):
-        if oneshot: method.oneshot = oneshot
+    def bind(self, name, method, oneshot=False):
+        if oneshot:
+            method.oneshot = oneshot
         methods = self._events.get(name, [])
         methods.append(method)
         self._events[name] = methods
 
-    def unbind(self, name, method = None):
+    def unbind(self, name, method=None):
         methods = self._events.get(name, [])
-        if method: methods.remove(method)
-        else: del methods[:]
+        if method:
+            methods.remove(method)
+        else:
+            del methods[:]
 
     def unbind_all(self):
-        if not hasattr(self, "_events"): return
-        for methods in self._events.values(): del methods[:]
+        if not hasattr(self, "_events"):
+            return
+        for methods in self._events.values():
+            del methods[:]
         self._events.clear()
 
     def trigger(self, name, *args, **kwargs):
         cls = self.__class__
         self.trigger_l(name, cls, *args, **kwargs)
 
     def trigger_l(self, name, level, *args, **kwargs):
         oneshots = None
         methods = self._events.get(name, [])
         for method in methods:
             method(*args, **kwargs)
-            if not hasattr(method, "oneshot"): continue
-            if not method.oneshot: continue
+            if not hasattr(method, "oneshot"):
+                continue
+            if not method.oneshot:
+                continue
             oneshots = [] if oneshots == None else oneshots
             oneshots.append(method)
         level.trigger_g(name, self, *args, **kwargs)
-        if not oneshots: return
-        for oneshot in oneshots: self.unbind(name, oneshot)
+        if not oneshots:
+            return
+        for oneshot in oneshots:
+            self.unbind(name, oneshot)
```

### Comparing `quorum-0.8.2/src/quorum/amazon.py` & `quorum-0.8.3/src/quorum/amazon.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,34 +18,27 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 from . import exceptions
 
-try: import boto
-except ImportError: boto = None
+try:
+    import boto
+except ImportError:
+    boto = None
 
 connection = None
 """ The global wide connection to the amazon server
 that is meant to be used across sessions """
 
 bucket = None
 """ The global bucket reference to be used to create
@@ -60,49 +53,61 @@
 """ The secret of the client that is going to be used in the
 connections to be established to the amazon servers """
 
 bucket_name = None
 """ The name of the bucket to be used to create and retrieve
 keys from the amazon services """
 
+
 def get_connection():
     global connection
-    if boto == None: raise exceptions.ModuleNotFound("boto")
-    if connection: return connection
+    if boto == None:
+        raise exceptions.ModuleNotFound("boto")
+    if connection:
+        return connection
     connection = _boto().connect_s3(id, secret)
     return connection
 
+
 def get_bucket():
     global bucket
     connection = get_connection()
-    if bucket: return bucket
+    if bucket:
+        return bucket
     bucket = connection.get_bucket(bucket_name)
     return bucket
 
+
 def clear_bucket():
     bucket = get_bucket()
     keys = bucket.get_all_keys()
-    for key in keys: key.delete()
+    for key in keys:
+        key.delete()
+
 
 def get_key(name):
     bucket = get_bucket()
     key = _boto().s3.key.Key(bucket)
     key.key = name
     return key
 
+
 def exists_key(name):
     bucket = get_bucket()
     key = _boto().s3.key.Key(bucket)
     key.key = name
     return key.exists()
 
+
 def delete_key(name):
     bucket = get_bucket()
     bucket.delete_key(name)
 
-def _boto(verify = True):
-    if verify: util.verify(
-        not boto == None,
-        message = "Boto library not available",
-        exception = exceptions.OperationalError
-    )
+
+def _boto(verify=True):
+    if verify:
+        util.verify(
+            not boto == None,
+            message="Boto library not available",
+            exception=exceptions.OperationalError,
+        )
     return boto
```

### Comparing `quorum-0.8.2/src/quorum/typesf.py` & `quorum-0.8.3/src/quorum/typesf.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import uuid
@@ -45,22 +36,24 @@
 from . import crypt
 from . import legacy
 from . import common
 from . import config
 from . import storage
 from . import exceptions
 
+
 class AbstractType(object):
 
     def json_v(self, *args, **kwargs):
         return str(self)
 
     def map_v(self, *args, **kwargs):
         return self.json_v()
 
+
 class Type(AbstractType):
 
     def __init__(self, value):
         cls = self.__class__
         self.loads(value)
 
     def json_v(self, *args, **kwargs):
@@ -68,33 +61,39 @@
 
     def loads(self, value):
         raise exceptions.NotImplementedError()
 
     def dumps(self):
         raise exceptions.NotImplementedError()
 
+
 class File(AbstractType):
 
     def __init__(self, file):
-        if isinstance(file, legacy.BYTES): self.build_d(file)
-        elif isinstance(file, dict): self.build_b64(file)
-        elif isinstance(file, tuple): self.build_t(file)
-        elif isinstance(file, File): self.build_i(file)
-        else: self.build_f(file)
+        if isinstance(file, legacy.BYTES):
+            self.build_d(file)
+        elif isinstance(file, dict):
+            self.build_b64(file)
+        elif isinstance(file, tuple):
+            self.build_t(file)
+        elif isinstance(file, File):
+            self.build_i(file)
+        else:
+            self.build_f(file)
 
     def __repr__(self):
         return "<File: %s>" % self.file_name
 
     def __str__(self):
         return self.file_name
 
     def __len__(self):
         return self.size
 
-    def build_d(self, file_d, name = "default"):
+    def build_d(self, file_d, name="default"):
         self.build_t((name, None, file_d))
 
     def build_b64(self, file_m):
         name = file_m["name"]
         data_b64 = file_m["data"]
         hash = file_m.get("hash", None)
         mime = file_m.get("mime", None)
@@ -177,44 +176,46 @@
         self.etag = None
         self.guid = self._guid()
         self.params = None
         self.engine = None
 
         self._load()
 
-    def read(self, size = None):
+    def read(self, size=None):
         engine = self._engine()
-        return engine.read(self, size = size)
+        return engine.read(self, size=size)
 
-    def seek(self, offset = None):
+    def seek(self, offset=None):
         engine = self._engine()
-        return engine.seek(self, offset = offset)
+        return engine.seek(self, offset=offset)
 
     def delete(self):
         engine = self._engine()
         return engine.delete(self)
 
     def cleanup(self):
         engine = self._engine()
         return engine.cleanup(self)
 
     def json_v(self, *args, **kwargs):
-        if not self.is_valid(): return None
+        if not self.is_valid():
+            return None
         store = kwargs.get("store", True)
-        if store: self._store()
+        if store:
+            self._store()
         data = self.data_b64 if self.is_stored() else None
         return dict(
-            name = self.file_name,
-            data = data,
-            hash = self.hash,
-            mime = self.mime,
-            etag = self.etag,
-            guid = self.guid,
-            params = self.params,
-            engine = self.engine
+            name=self.file_name,
+            data=data,
+            hash=self.hash,
+            mime=self.mime,
+            etag=self.etag,
+            guid=self.guid,
+            params=self.params,
+            engine=self.engine,
         )
 
     def is_seekable(self):
         engine = self._engine()
         return engine.is_seekable()
 
     def is_stored(self):
@@ -224,35 +225,37 @@
     def is_valid(self):
         return self.file_name or (self.data or self.data_b64)
 
     def is_empty(self):
         return self.size <= 0
 
     def _hash(self, data):
-        if not data: return None
+        if not data:
+            return None
         hash = hashlib.sha256(data)
         digest = hash.hexdigest()
         return digest
 
     def _etag(self, data):
-        if not data: return None
+        if not data:
+            return None
         hash = hashlib.md5(data)
         digest = hash.hexdigest()
         return digest
 
     def _guid(self):
         return str(uuid.uuid4())
 
-    def _load(self, force = False):
+    def _load(self, force=False):
         engine = self._engine()
-        engine.load(self, force = force)
+        engine.load(self, force=force)
 
-    def _store(self, force = False):
+    def _store(self, force=False):
         engine = self._engine()
-        engine.store(self, force = force)
+        engine.store(self, force=force)
 
     def _compute(self):
         """
         Computes a series of "calculated" attributes related with
         the data associated with the current file, these values may
         include: length, hash values, etag, etc.
 
@@ -263,22 +266,26 @@
         self.data_b64 = base64.b64encode(self.data)
         self.data_b64 = legacy.str(self.data_b64)
         self.hash = self._hash(self.data)
         self.size = len(self.data)
         self.etag = self._etag(self.data)
 
     def _engine(self):
-        if not self.engine: return storage.BaseEngine
+        if not self.engine:
+            return storage.BaseEngine
         return getattr(storage, self.engine.capitalize() + "Engine")
 
+
 class Files(AbstractType):
 
     def __init__(self, files):
-        if isinstance(files, Files): self.build_i(files)
-        else: self.build_f(files)
+        if isinstance(files, Files):
+            self.build_i(files)
+        else:
+            self.build_f(files)
 
     def __repr__(self):
         return "<Files: %d files>" % len(self._files)
 
     def __len__(self):
         return self._files.__len__()
 
@@ -293,28 +300,32 @@
 
     def build_i(self, files):
         self._files = files._files
 
     def build_f(self, files):
         self._files = []
         base = self.base()
-        if not type(files) == list: files = [files]
+        if not type(files) == list:
+            files = [files]
         for file in files:
             _file = base(file)
-            if not _file.is_valid(): continue
+            if not _file.is_valid():
+                continue
             self._files.append(_file)
 
     def json_v(self, *args, **kwargs):
         return [file.json_v(*args, **kwargs) for file in self._files]
 
     def is_empty(self):
         return len(self._files) == 0
 
     def _load(self):
-        for file in self._files: file._load()
+        for file in self._files:
+            file._load()
+
 
 class ImageFile(File):
 
     def build_b64(self, file_m):
         File.build_b64(self, file_m)
         self.width = file_m.get("width", 0)
         self.height = file_m.get("height", 0)
@@ -335,117 +346,140 @@
         self._ensure_all()
 
     def build_f(self, file):
         File.build_f(self, file)
         self._ensure_all()
 
     def json_v(self, *args, **kwargs):
-        if not self.is_valid(): return None
+        if not self.is_valid():
+            return None
         value = File.json_v(self, *args, **kwargs)
         value.update(
-            width = self.width,
-            height = self.height,
-            format = self.format,
-            kwargs = self.kwargs
+            width=self.width, height=self.height, format=self.format, kwargs=self.kwargs
         )
         return value
 
     def _ensure_all(self):
         self._ensure_size()
         self._ensure_mime()
         self._ensure_kwargs()
 
     def _ensure_size(self):
-        if hasattr(self, "width") and self.width and\
-            hasattr(self, "height") and self.height: return
+        if (
+            hasattr(self, "width")
+            and self.width
+            and hasattr(self, "height")
+            and self.height
+        ):
+            return
         self.width, self.height = self._size()
 
     def _ensure_mime(self):
-        if hasattr(self, "format") and self.format and\
-            hasattr(self, "mime") and self.mime: return
+        if (
+            hasattr(self, "format")
+            and self.format
+            and hasattr(self, "mime")
+            and self.mime
+        ):
+            return
         self.format, self.mime = self._mime()
 
     def _ensure_kwargs(self):
-        if hasattr(self, "kwargs"): return
+        if hasattr(self, "kwargs"):
+            return
         self.kwargs = dict()
 
     def _size(self):
-        try: return self._size_image()
-        except Exception: return self._size_default()
+        try:
+            return self._size_image()
+        except Exception:
+            return self._size_default()
 
     def _size_image(self):
-        if self.data: return self._size_pil()
-        else: return self._size_default()
+        if self.data:
+            return self._size_pil()
+        else:
+            return self._size_default()
 
     def _size_pil(self):
         import PIL.Image
+
         buffer = legacy.BytesIO(self.data)
         try:
             image = PIL.Image.open(buffer)
             size = image.size
         finally:
             buffer.close()
         return size
 
     def _size_default(self):
         return (0, 0)
 
     def _mime(self):
-        try: return self._mime_image()
-        except Exception: return self._mime_default()
+        try:
+            return self._mime_image()
+        except Exception:
+            return self._mime_default()
 
     def _mime_image(self):
-        if self.data: return self._mime_pil()
-        else: return self._mime_default()
+        if self.data:
+            return self._mime_pil()
+        else:
+            return self._mime_default()
 
     def _mime_pil(self):
         import PIL.Image
+
         buffer = legacy.BytesIO(self.data)
         try:
             image = PIL.Image.open(buffer)
             format = image.format.lower()
             mime = PIL.Image.MIME[image.format]
         finally:
             buffer.close()
         return format, mime
 
     def _mime_default(self):
         return None, "application/octet-stream"
 
+
 class ImageFiles(Files):
 
     def base(self):
         return ImageFile
 
-def image(width = None, height = None, format = "png", **kwargs):
+
+def image(width=None, height=None, format="png", **kwargs):
 
     class _ImageFile(ImageFile):
 
         RGB_FORMATS = ("jpg", "jpeg")
         """ The set of format that are considered to be
         RGB based and should be handled with special care """
 
         def build_b64(self, file_m):
             ImageFile.build_b64(self, file_m)
 
             # verifies if there's valid data in the current file
             # if that's not the case there's nothing remaining to
             # be done (not going to process the file)
-            if not self.data_b64: return
+            if not self.data_b64:
+                return
 
             # determines if a resize operation is required for the
             # current image data, if that's not the case returns the
             # control flow immediately (nothing to be done)
             need_resize = self.need_resize(
-                width_o = self.width,
-                height_o = self.height,
-                format_o = self.format,
-                kwargs_o = self.kwargs
+                width_o=self.width,
+                height_o=self.height,
+                format_o=self.format,
+                kwargs_o=self.kwargs,
             )
-            if not need_resize: return
+            if not need_resize:
+                return
 
             # decodes the base 64 based data and then runs the resize
             # operation with the current data re-encoding it back to
             # the base 64 model to be used in the map storage
             data_b64 = legacy.bytes(self.data_b64)
             data = base64.b64decode(data_b64)
             data = self.resize(data)
@@ -463,47 +497,52 @@
             file_m["kwargs"] = kwargs
 
             # removes a series of keys from the file map as
             # they are no longer reliable and may reflect
             # different values from the ones contained in data
             # theses should be update by the "ensure" methods
             for name in ("width", "height", "format"):
-                if name in file_m: del file_m[name]
+                if name in file_m:
+                    del file_m[name]
 
             # runs the rebuilding of the information taking into
             # account the new information from the file
             ImageFile.build_b64(self, file_m)
 
         def build_t(self, file_t):
             # unpacks the file tuple into its component to be
             # used for the format and size ensure operations
             name, content_type, data = file_t
 
             # tries to run the resize operation to ensure that
             # the proper size and format is present in the data
-            try: _data = self.resize(data) if data else data
-            except Exception: _data = data
+            try:
+                _data = self.resize(data) if data else data
+            except Exception:
+                _data = data
 
             # updates the parameters attributes in the instance so
             # that the new file is marked with proper values
             self.kwargs = kwargs
 
             # creates the "new" file tuple with the newly resized
             # image data and runs the parent tuple build method
             file_t = (name, content_type, _data)
             ImageFile.build_t(self, file_t)
 
-        def resize(self, data = None):
+        def resize(self, data=None):
             import PIL.Image
 
             data = data or self.data
-            if not data: return data
+            if not data:
+                return data
 
             is_resized = True if width or height else False
-            if not is_resized: return data
+            if not is_resized:
+                return data
 
             params = kwargs.get("params", {})
             background = kwargs.get("background", "ffffff")
 
             size = (width, height)
             in_buffer = legacy.BytesIO(data)
             out_buffer = legacy.BytesIO()
@@ -516,46 +555,49 @@
             finally:
                 in_buffer.close()
                 out_buffer.close()
 
             return data
 
         def need_resize(
-            self,
-            width_o = None,
-            height_o = None,
-            format_o = None,
-            kwargs_o = None
+            self, width_o=None, height_o=None, format_o=None, kwargs_o=None
         ):
-            if width and not width == width_o: return True
-            if height and not height == height_o: return True
-            if format and not format == format_o: return True
-            if kwargs and not kwargs == kwargs_o: return True
+            if width and not width == width_o:
+                return True
+            if height and not height == height_o:
+                return True
+            if format and not format == format_o:
+                return True
+            if kwargs and not kwargs == kwargs_o:
+                return True
             return False
 
         def _resize(self, image, size):
             import PIL.Image
 
             # unpacks the provided tuple containing the size dimension into the
             # with and the height an in case one of these values is not defined
             # an error is raises indicating the problem
             width, height = size
-            if not height and not width: raise AttributeError("invalid values")
+            if not height and not width:
+                raise AttributeError("invalid values")
 
             # retrieves the size of the loaded image and uses the values to calculate
             # the aspect ration of the provided image, this value is going to be
             # used latter for some of the resizing calculus
             image_width, image_height = image.size
             image_ratio = float(image_width) / float(image_height)
 
             # in case one of the size dimensions has not been specified
             # it must be calculated from the base values taking into account
             # that the aspect ration should be preserved
-            if not height: height = int(image_height * width / float(image_width))
-            if not width: width = int(image_width * height / float(image_height))
+            if not height:
+                height = int(image_height * width / float(image_width))
+            if not width:
+                width = int(image_width * height / float(image_height))
 
             # re-constructs the size tuple with the new values for the width
             # the height that have been calculated from the ratios
             size = (width, height)
 
             # calculates the target aspect ration for the image that is going
             # to be resized, this value is going to be used in the comparison
@@ -589,81 +631,90 @@
             cls = self.__class__
 
             # converts the target format into the lower based version
             # (normalization) and verifies if it's considered to be
             # an RGB only format, if that's not the case there's nothing
             # remaining to be done (no conversion required)
             format = format.lower()
-            if not format in cls.RGB_FORMATS: return image
+            if not format in cls.RGB_FORMATS:
+                return image
 
             # in case the format/mode of the original image is already
             # RGB there's no need to run the conversion process
-            if image.mode == "RGB": return image
+            if image.mode == "RGB":
+                return image
 
             # creates a new RGB based image with the target size and
             # with the provided background and copies it as the target
             new = PIL.Image.new("RGB", (image.width, image.height), "#" + background)
             new.paste(image, image)
             return new
 
     return _ImageFile
 
-def images(width = None, height = None, format = "png", **kwargs):
 
-    image_c = image(
-        width = width,
-        height = height,
-        format = format,
-        **kwargs
-    )
+def images(width=None, height=None, format="png", **kwargs):
+
+    image_c = image(width=width, height=height, format=format, **kwargs)
 
     class _ImageFiles(ImageFiles):
 
         def base(self):
             return image_c
 
     return _ImageFiles
 
+
 class Reference(AbstractType):
     pass
 
-def reference(target, name = None, dumpall = False):
+
+def reference(target, name=None, dumpall=False):
     name = name or "id"
     target_t = type(target)
     is_reference = target_t in legacy.STRINGS
     reserved = ("id", "_target", "_object", "_type", "__dict__")
 
     class _Reference(Reference):
 
         _name = name
         """ The name of the key (join) attribute for the
         reference that is going to be created, this name
         may latter be used to cast the value """
 
         def __init__(self, id):
             self.__start__()
-            if isinstance(id, _Reference): self.build_i(id)
-            elif isinstance(id, self._target): self.build_o(id)
-            else: self.build(id)
+            if isinstance(id, _Reference):
+                self.build_i(id)
+            elif isinstance(id, self._target):
+                self.build_o(id)
+            else:
+                self.build(id)
 
         def __str__(self):
             self.resolve()
             has_str = hasattr(self._object, "__str__")
-            if has_str: return self._object.__str__()
-            else: return str(self._object) or str()
+            if has_str:
+                return self._object.__str__()
+            else:
+                return str(self._object) or str()
 
         def __unicode__(self):
             self.resolve()
             has_unicode = hasattr(self._object, "__unicode__")
-            if has_unicode: return self._object.__unicode__()
-            else: return legacy.UNICODE(self._object) or legacy.UNICODE()
+            if has_unicode:
+                return self._object.__unicode__()
+            else:
+                return legacy.UNICODE(self._object) or legacy.UNICODE()
 
         def __eq__(self, other):
-            if other == None: return self.id in ("", b"", None)
-            if isinstance(other, Reference): return self.equals(other)
+            if other == None:
+                return self.id in ("", b"", None)
+            if isinstance(other, Reference):
+                return self.equals(other)
             return id(self) == id(other)
 
         def __ne__(self, other):
             return not self.__eq__(other)
 
         def __len__(self):
             is_empty = self.id in ("", b"", None)
@@ -671,65 +722,75 @@
 
         def __bool__(self):
             is_empty = self.id in ("", b"", None)
             return not is_empty
 
         def __getattr__(self, name):
             is_magic = name.startswith("__") and name.endswith("__")
-            if is_magic: return Reference.__getattr__(name)
+            if is_magic:
+                return Reference.__getattr__(name)
             self.resolve()
             exists = hasattr(self._object, name)
-            if exists: return getattr(self._object, name)
+            if exists:
+                return getattr(self._object, name)
             raise AttributeError("'%s' not found" % name)
 
         def __setattr__(self, name, value):
             # in case the name that is being set is not part of the reserved
             # names for the reference underlying structure the object resolution
             # is triggered to make sure the underlying object exists and is loaded
-            if not name in reserved: self.resolve()
+            if not name in reserved:
+                self.resolve()
 
             # verifies if the reference object exists in the current
             # reference instance, that's the case if the object name is
             # defined in the dictionary and the referenced object contains
             # an attribute with the name referred, for those situations
             # defers the setting of the attribute to the reference object
             exists = "_object" in self.__dict__ and hasattr(self._object, name)
-            if exists: return setattr(self._object, name, value)
+            if exists:
+                return setattr(self._object, name, value)
 
             # otherwise this is a normal attribute setting and the current
             # object's dictionary must be changed so that the new value is set
             self.__dict__[name] = value
 
         def __start__(self):
-            if is_reference: self._target = self.__class__._target()
-            else: self._target = target
+            if is_reference:
+                self._target = self.__class__._target()
+            else:
+                self._target = target
             util.verify(self._target)
             meta = getattr(self._target, name)
             self._type = meta.get("type", legacy.UNICODE)
 
         @classmethod
         def _default(cls):
             return cls(None)
 
         @classmethod
         def _target(cls):
-            if is_reference: return getattr(common.base().APP.models, target)
+            if is_reference:
+                return getattr(common.base().APP.models, target)
             return target
 
         @classmethod
         def _btype(cls):
-            if is_reference: _target = cls._target()
-            else: _target = target
+            if is_reference:
+                _target = cls._target()
+            else:
+                _target = target
             meta = getattr(_target, name)
             return meta.get("type", legacy.UNICODE)
 
-        def build(self, id, cast = True):
+        def build(self, id, cast=True):
             is_unset = id in ("", b"", None)
             cast = cast and not is_unset
-            if cast: id = self._target.cast(name, id)
+            if cast:
+                id = self._target.cast(name, id)
             self.id = id
             self._object = None
 
         def build_i(self, reference):
             self.id = reference.id
             self._object = reference._object
 
@@ -737,36 +798,41 @@
             self.id = getattr(object, self._name)
             self._object = object
 
         def ref_v(self, *args, **kwargs):
             return self.val()
 
         def json_v(self, *args, **kwargs):
-            if dumpall: return self.resolve()
+            if dumpall:
+                return self.resolve()
             return self.val()
 
         def map_v(self, *args, **kwargs):
             resolve = kwargs.get("resolve", True)
             value = self.resolve() if resolve else self._object
-            if resolve and not value: return value
-            if not value: return self.val()
+            if resolve and not value:
+                return value
+            if not value:
+                return self.val()
             return value.map(*args, **kwargs)
 
         def val(self, *args, **kwargs):
             is_empty = self.id in ("", b"", None)
-            if is_empty: return None
+            if is_empty:
+                return None
             return self._type(self.id)
 
         def resolve(self, *args, **kwargs):
             # verifies if the underlying object reference exists
             # in the current names dictionary and if it exists
             # verifies if it's valid (value is valid) if that's
             # the case returns the current value immediately
             exists = "_object" in self.__dict__
-            if exists and self._object: return self._object
+            if exists and self._object:
+                return self._object
 
             # verifies if there's an id value currently set in
             # the reference in case it does not exists sets the
             # object value in the current instance with a none
             # value and then returns this (invalid value)
             if not self.id:
                 _object = None
@@ -787,49 +853,56 @@
             # sets the resolved object (using the current id attribute)
             # in the current instance's dictionary and then returns this
             # value to the caller method as the resolved value
             self.__dict__["_object"] = _object
             return _object
 
         def equals(self, other):
-            if not self.__class__ == other.__class__: return False
-            if not self._target == other._target: return False
-            if not self.id == other.id: return False
+            if not self.__class__ == other.__class__:
+                return False
+            if not self._target == other._target:
+                return False
+            if not self.id == other.id:
+                return False
             return True
 
         def is_resolved(self):
             exists = "_object" in self.__dict__
             return True if exists and self._object else False
 
         def is_resolvable(self):
             self.resolve()
             return False if self._object == None else True
 
     return _Reference
 
+
 class References(AbstractType):
     pass
 
-def references(target, name = None, dumpall = False):
+
+def references(target, name=None, dumpall=False):
     name = name or "id"
     target_t = type(target)
     is_reference = target_t in legacy.STRINGS
-    reference_c = reference(target, name = name, dumpall = dumpall)
+    reference_c = reference(target, name=name, dumpall=dumpall)
 
     class _References(References):
 
         _name = name
         """ The name of the key (join) attribute for the
         reference that is going to be created, this name
         may latter be used to cast the value """
 
         def __init__(self, ids):
             self.__start__()
-            if isinstance(ids, _References): self.build_i(ids)
-            else: self.build(ids)
+            if isinstance(ids, _References):
+                self.build_i(ids)
+            else:
+                self.build(ids)
 
         def __len__(self):
             return self.objects.__len__()
 
         def __iter__(self):
             return self.objects.__iter__()
 
@@ -839,16 +912,18 @@
         def __getitem__(self, key):
             return self.objects.__getitem__(key)
 
         def __contains__(self, item):
             return self.contains(item)
 
         def __start__(self):
-            if is_reference: self._target = self.__class__._target()
-            else: self._target = target
+            if is_reference:
+                self._target = self.__class__._target()
+            else:
+                self._target = target
             util.verify(self._target)
 
         @classmethod
         def _default(cls):
             return cls([])
 
         @classmethod
@@ -858,15 +933,16 @@
         @classmethod
         def _btype(cls):
             return reference_c._btype()
 
         def build(self, ids):
             is_valid = not ids == None
             is_iterable = util.is_iterable(ids)
-            if is_valid and not is_iterable: ids = [ids]
+            if is_valid and not is_iterable:
+                ids = [ids]
 
             self.ids = ids
             self.objects = []
             self.objects_m = {}
 
             self.set_ids(self.ids)
 
@@ -875,15 +951,16 @@
             self.objects = references.objects
             self.objects_m = references.objects_m
 
         def set_ids(self, ids):
             ids = ids or []
             self.ids = []
             for id in ids:
-                if id == "" or id == None: continue
+                if id == "" or id == None:
+                    continue
                 object = reference_c(id)
                 object_id = object.id
                 self.ids.append(object_id)
                 self.objects.append(object)
                 self.objects_m[object_id] = object
 
         def ref_v(self, *args, **kwargs):
@@ -902,73 +979,81 @@
             return [object.val() for object in self.objects]
 
         def resolve(self, *args, **kwargs):
             return [object.resolve(*args, **kwargs) for object in self.objects]
 
         def find(self, *args, **kwargs):
             kwargs = dict(kwargs)
-            kwargs[name] = {"$in" : [self._target.cast(name, _id) for _id in self.ids]}
+            kwargs[name] = {"$in": [self._target.cast(name, _id) for _id in self.ids]}
             return self._target.find(*args, **kwargs)
 
         def paginate(self, *args, **kwargs):
             kwargs = dict(kwargs)
-            kwargs[name] = {"$in" : [self._target.cast(name, _id) for _id in self.ids]}
+            kwargs[name] = {"$in": [self._target.cast(name, _id) for _id in self.ids]}
             return self._target.paginate(*args, **kwargs)
 
         def is_empty(self):
             ids_l = len(self.ids)
             return ids_l == 0
 
         def append(self, id):
             is_object = hasattr(id, self._name)
-            if is_object: id = getattr(id, self._name)
+            if is_object:
+                id = getattr(id, self._name)
             object = reference_c(id)
             self.ids.append(id)
             self.objects.append(object)
             self.objects_m[id] = object
 
         def remove(self, id):
             is_object = hasattr(id, self._name)
-            if is_object: id = getattr(id, self._name)
+            if is_object:
+                id = getattr(id, self._name)
             object = self.objects_m[id]
             self.ids.remove(id)
             self.objects.remove(object)
             del self.objects_m[id]
 
         def contains(self, id):
             is_object = hasattr(id, self._name)
-            if is_object: id = getattr(id, self._name)
+            if is_object:
+                id = getattr(id, self._name)
             return id in self.objects_m
 
         def is_resolved(self):
-            if not self.objects: return True
+            if not self.objects:
+                return True
             return self.objects[0].is_resolved()
 
     return _References
 
+
 class Encrypted(AbstractType):
 
     PADDING = ":encrypted"
 
-def encrypted(cipher = "spritz", key = None, encoding = "utf-8"):
+
+def encrypted(cipher="spritz", key=None, encoding="utf-8"):
     key = key or None
 
     class _Encrypted(Encrypted):
 
         def __init__(self, value):
             cls = self.__class__
             util.verify(
-                isinstance(value, legacy.ALL_STRINGS) or\
-                isinstance(value, Encrypted)
+                isinstance(value, legacy.ALL_STRINGS) or isinstance(value, Encrypted)
             )
             self.key = key or config.conf("SECRET", None)
             self.key = legacy.bytes(self.key)
-            if isinstance(value, Encrypted): self.build_i(value)
-            elif value.endswith(cls.PADDING): self.build_e(value)
-            else: self.build(value)
+            if isinstance(value, Encrypted):
+                self.build_i(value)
+            elif value.endswith(cls.PADDING):
+                self.build_e(value)
+            else:
+                self.build(value)
 
         def __str__(self):
             return self.value
 
         def __unicode__(self):
             return self.value
 
@@ -993,32 +1078,35 @@
             self.key = instance.key
             self.value = instance.value
             self.encrypted = instance.encrypted
 
         def json_v(self, *args, **kwargs):
             return self.encrypted
 
-        def _encrypt(self, value, strict = False):
-            if not self.key and not strict: return value
+        def _encrypt(self, value, strict=False):
+            if not self.key and not strict:
+                return value
             cls = self.__class__
-            value = legacy.bytes(value, encoding = encoding)
+            value = legacy.bytes(value, encoding=encoding)
             cipher_i = crypt.Cipher.new(cipher, self.key)
             encrypted = cipher_i.encrypt(value)
             encrypted = base64.b64encode(encrypted)
-            encrypted = legacy.str(encrypted, encoding = encoding)
+            encrypted = legacy.str(encrypted, encoding=encoding)
             return encrypted + cls.PADDING
 
-        def _decrypt(self, value, strict = False):
-            if not self.key and not strict: return value
+        def _decrypt(self, value, strict=False):
+            if not self.key and not strict:
+                return value
             cls = self.__class__
             util.verify(value.endswith(cls.PADDING))
-            value = value[:-len(cls.PADDING)]
+            value = value[: -len(cls.PADDING)]
             value = legacy.bytes(value)
             value = base64.b64decode(value)
             cipher_i = crypt.Cipher.new(cipher, self.key)
             decrypted = cipher_i.decrypt(value)
-            decrypted = legacy.str(decrypted, encoding = encoding)
+            decrypted = legacy.str(decrypted, encoding=encoding)
             return decrypted
 
     return _Encrypted
 
+
 secure = encrypted()
```

### Comparing `quorum-0.8.2/src/quorum/storage.py` & `quorum-0.8.3/src/quorum/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,27 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import tempfile
 
 from . import config
 from . import exceptions
 
+
 class StorageEngine(object):
 
     @classmethod
     def load(cls, file, *args, **kwargs):
         raise exceptions.NotImplementedError()
 
     @classmethod
@@ -77,29 +69,34 @@
     def is_stored(self):
         return False
 
     @classmethod
     def _compute(cls, file, *args, **kwargs):
         file._compute(*args, **kwargs)
 
+
 class BaseEngine(StorageEngine):
 
     @classmethod
     def load(cls, file, *args, **kwargs):
         force = kwargs.get("force", False)
-        if not file.file_name: return
-        if file.data and not force: return
+        if not file.file_name:
+            return
+        if file.data and not force:
+            return
 
         path = tempfile.mkdtemp()
         path_f = os.path.join(path, file.file_name)
         file.file.save(path_f)
 
         handle = open(path_f, "rb")
-        try: file.data = handle.read()
-        finally: handle.close()
+        try:
+            file.data = handle.read()
+        finally:
+            handle.close()
 
         cls._compute()
 
     @classmethod
     def store(cls, file, *args, **kwargs):
         pass
 
@@ -109,102 +106,112 @@
 
     @classmethod
     def read(cls, file, *args, **kwargs):
         # tries to determine the requested size for# the file
         # reading in case none is defined the handled flag
         # handling is ignored and the data returned immediately
         size = kwargs.get("size", None)
-        if not size: return file.data
+        if not size:
+            return file.data
 
         # verifies if the handled flag is already set (data)
         # has been already retrieved and if that's not the
         # case sets the handled flag and returns the data
         handled = hasattr(file, "_handled")
         file._handled = True
-        if not handled: return file.data
+        if not handled:
+            return file.data
 
         # runs the final cleanup operation and returns an empty
         # value to end the reading sequence
         cls.cleanup(file)
         return None
 
     @classmethod
     def cleanup(cls, file, *args, **kwargs):
-        if not hasattr(file, "handled"): return
+        if not hasattr(file, "handled"):
+            return
         del file._handled
 
     @classmethod
     def is_stored(self):
         return True
 
+
 class FsEngine(StorageEngine):
 
     @classmethod
     def store(cls, file, *args, **kwargs):
         file_path = cls._file_path(file)
         handle = open(file_path, "wb")
-        try: handle.write(file.data)
-        finally: handle.close()
+        try:
+            handle.write(file.data)
+        finally:
+            handle.close()
 
     @classmethod
     def load(cls, file, *args, **kwargs):
         cls._compute(file)
 
     @classmethod
     def delete(cls, file, *args, **kwargs):
-        file_path = cls._file_path(file, ensure = False)
+        file_path = cls._file_path(file, ensure=False)
         os.remove(file_path)
 
     @classmethod
     def read(cls, file, *args, **kwargs):
         data = None
         size = kwargs.get("size", None)
         handle = cls._handle(file)
-        try: data = handle.read(size or -1)
+        try:
+            data = handle.read(size or -1)
         finally:
             is_final = True if not size or not data else False
             is_final and cls.cleanup(file)
         return data
 
     @classmethod
     def seek(cls, file, *args, **kwargs):
         offset = kwargs.get("offset", None)
-        if offset == None: return
+        if offset == None:
+            return
         handle = cls._handle(file)
         handle.seek(offset)
 
     @classmethod
     def cleanup(cls, file, *args, **kwargs):
-        if not hasattr(file, "_handle"): return
+        if not hasattr(file, "_handle"):
+            return
         file._handle.close()
         del file._handle
 
     @classmethod
     def is_seekable(self):
         return True
 
     @classmethod
     def _compute(cls, file):
-        file_path = cls._file_path(file, ensure = False)
+        file_path = cls._file_path(file, ensure=False)
         size = os.path.getsize(file_path)
         mtime = os.path.getmtime(file_path)
         file.hash = str(mtime)
         file.size = size
         file.etag = str(mtime)
 
     @classmethod
     def _handle(cls, file):
-        file_path = cls._file_path(file, ensure = False)
+        file_path = cls._file_path(file, ensure=False)
         handle = hasattr(file, "_handle") and file._handle
-        if not handle: handle = open(file_path, "rb")
+        if not handle:
+            handle = open(file_path, "rb")
         file._handle = handle
         return handle
 
     @classmethod
-    def _file_path(cls, file, ensure = True, base = None):
+    def _file_path(cls, file, ensure=True, base=None):
         # verifies that the standard params value is defined and
         # if that's no the case defaults the value, then tries to
         # retrieve a series of parameters for file path discovery
         params = file.params or {}
         file_path = params.get("file_path", None)
 
         # tries to resolve the base path that is going to be used
@@ -220,15 +227,17 @@
         file_path = os.path.expanduser(file_path)
         file_path = os.path.normpath(file_path)
         dir_path = os.path.dirname(file_path)
 
         # verifies if the ensure flag is not set of if the directory
         # path associated with the current file path exists and if
         # that's the case returns the file path immediately
-        if not ensure: return file_path
-        if os.path.exists(dir_path): return file_path
+        if not ensure:
+            return file_path
+        if os.path.exists(dir_path):
+            return file_path
 
         # creates the directories (concrete and parents) as requested
         # and then returns the "final" file path value to the caller
         # method so that it can be used for reading or writing
         os.makedirs(dir_path)
         return file_path
```

### Comparing `quorum-0.8.2/src/quorum/unit_test.py` & `quorum-0.8.3/src/quorum/unit_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,46 +18,41 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import unittest
 
+
 def secured(function):
 
     def decorator(self, *args, **kwargs):
-        if self._skip: self._skipped.append(function.__name__); return
+        if self._skip:
+            self._skipped.append(function.__name__)
+            return
         return function(self, *args, **kwargs)
 
     return decorator
 
+
 class TestCase(unittest.TestCase):
 
     _skip = False
 
     _skipped = []
 
-    def __init__(self, methodName = "runTest"):
-        unittest.TestCase.__init__(self, methodName = methodName)
+    def __init__(self, methodName="runTest"):
+        unittest.TestCase.__init__(self, methodName=methodName)
 
         self._skip = False
         self._skipped = []
 
     def skip(self):
         self._skip = True
```

### Comparing `quorum-0.8.2/src/quorum/formats.py` & `quorum-0.8.3/src/quorum/formats.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,43 +18,39 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import legacy
 from . import exceptions
 
-try: import xlrd
-except ImportError: xlrd = None
+try:
+    import xlrd
+except ImportError:
+    xlrd = None
 
-def xlsx_to_map(file_path, keys = (), types = (), ignore_header = True):
+
+def xlsx_to_map(file_path, keys=(), types=(), ignore_header=True):
     # verifies if the xlrd module has been correctly loaded
     # and in case it's not raises an exception indicating so
-    if xlrd == None: raise exceptions.ModuleNotFound("xlrd")
+    if xlrd == None:
+        raise exceptions.ModuleNotFound("xlrd")
 
     # in case the (data types) sequence is not defined creates
     # a tuple of unset types to fill the values
-    if not types: types = tuple([None] * len(keys))
+    if not types:
+        types = tuple([None] * len(keys))
 
     # creates the list structure that is going to store the
     # complete set of parsed items according to the provided
     # keys list specification
     items = []
 
     # opens the workbook in the provided file path for reading
@@ -69,37 +65,40 @@
 
     # iterates over the complete set of valid rows in the sheet
     # to process its contents, the valid rows are the ones that
     # contain any sort of data
     for row in range(sheet.nrows):
         # in case the ignore header flag is set and the current
         # row index is zero must continue the loop ignoring it
-        if row == 0 and ignore_header: continue
+        if row == 0 and ignore_header:
+            continue
 
         # creates the map that is going to be used in the construction
         # of the item elements and then iterates over all the expected
         # key values to populate it
         item = {}
         cell = 0
         for key, type in zip(keys, types):
             cell_s = sheet.cell(row, cell)
             raw = xlsx_raw(cell_s)
             value = cell_s.value
-            if type: value = type(raw)
+            if type:
+                value = type(raw)
             item[key] = value
             cell += 1
 
         # adds the item map that has been constructed to the list of
         # parsed items for the current spreadsheet
         items.append(item)
 
     # returns the final list of map items resulting from the parsing
     # of the spreadsheet file containing key to value assignments
     return items
 
+
 def xlsx_raw(cell_s):
     """
     Sanitizes the string value for the cell, taking into
     consideration integers and strings as different data types,
     the returning value is always a string.
 
     :type cell_s: Cell
@@ -108,12 +107,16 @@
     value should be returned.
     :rtype: String
     :return: The sanitized string value from the cell value
     ready to be used.
     """
 
     is_str = cell_s.ctype == xlrd.XL_CELL_TEXT
-    if is_str: return cell_s.value
-    try: is_int = cell_s.value == int(cell_s.value)
-    except ValueError: is_int = False
-    if is_int: return legacy.UNICODE(int(cell_s.value))
+    if is_str:
+        return cell_s.value
+    try:
+        is_int = cell_s.value == int(cell_s.value)
+    except ValueError:
+        is_int = False
+    if is_int:
+        return legacy.UNICODE(int(cell_s.value))
     return legacy.UNICODE(cell_s.value)
```

### Comparing `quorum-0.8.2/src/quorum/crypt.py` & `quorum-0.8.3/src/quorum/crypt.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,57 +18,51 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import array
 
 from . import legacy
 from . import exceptions
 
+
 class Cipher(object):
 
     def __init__(self, key):
         self.key = key
 
     @classmethod
     def new(cls, cipher, key):
         cipher = cls._cipher(cipher)
         return cipher(key)
 
     @classmethod
     def _cipher(cls, name):
         for subclass in cls.__subclasses__():
-            if not subclass.__name__.lower() == name: continue
+            if not subclass.__name__.lower() == name:
+                continue
             return subclass
         return None
 
     def encrypt(self, data):
         raise exceptions.NotImplementedError()
 
     def decrypt(self, data):
         raise exceptions.NotImplementedError()
 
+
 class RC4(Cipher):
     """
     Class that implements the basis for the
     encryption using the RC4 stream cipher.
 
     The implementation of the algorithm follows
     the typical implementation details.
@@ -115,14 +109,15 @@
         self.j = 0
 
         x = 0
         for i in range(256):
             x = (x + self.box[i] + legacy.ord(self.key[i % len(self.key)])) % 256
             self.box[i], self.box[x] = self.box[x], self.box[i]
 
+
 class Spritz(Cipher):
     """
     Class that implements the basis for the
     encryption using the Spritz stream cipher
     a variation of the original RC4 cipher.
 
     The implementation of the algorithm follows
@@ -146,50 +141,59 @@
         data = bytearray(data)
         sequezing = self.squeeze(len(data))
         out = bytearray(self._add(b1, -b2) for b1, b2 in zip(data, sequezing))
         return bytes(out)
 
     def absorb(self, data):
         data = bytearray(data)
-        for byte in data: self._absorb_byte(byte)
+        for byte in data:
+            self._absorb_byte(byte)
 
     def shuffle(self):
         self.whip(512)
         self.crush()
         self.whip(512)
         self.crush()
         self.whip(512)
         self.a = 0
 
     def whip(self, r):
-        for _ in range(r): self._update()
+        for _ in range(r):
+            self._update()
         self.w = self._add(self.w, 2)
 
     def crush(self):
         for v in range(128):
-            if self.S[v] <= self.S[255 - v]: continue
+            if self.S[v] <= self.S[255 - v]:
+                continue
             self._swap(v, 255 - v)
 
     def squeeze(self, r):
-        if self.a > 0: self.shuffle()
+        if self.a > 0:
+            self.shuffle()
         return bytearray([self.drip() for _ in range(r)])
 
     def drip(self):
-        if self.a > 0: self.shuffle()
+        if self.a > 0:
+            self.shuffle()
         self._update()
         return self._output()
 
     def _update(self):
         self.i = self._add(self.i, self.w)
         self.j = self._add(self.k, self.S[self._add(self.j, self.S[self.i])])
         self.k = self._add(self.i, self.k, self.S[self.j])
         self._swap(self.i, self.j)
 
     def _output(self):
-        self.z = self.S[self._add(self.j, self.S[self._add(self.i, self.S[self._add(self.z, self.k)])])]
+        self.z = self.S[
+            self._add(
+                self.j, self.S[self._add(self.i, self.S[self._add(self.z, self.k)])]
+            )
+        ]
         return self.z
 
     def _add(self, *args):
         return sum(args) % 256
 
     def _swap(self, i1, i2):
         self.S[i1], self.S[i2] = self.S[i2], self.S[i1]
@@ -200,14 +204,15 @@
         self.k = 0
         self.z = 0
         self.a = 0
         self.w = 1
         self.S = bytearray(range(256))
 
     def _absorb_byte(self, byte):
-        self._absorb_nibble(byte & 0xf)
+        self._absorb_nibble(byte & 0xF)
         self._absorb_nibble(byte >> 4)
 
     def _absorb_nibble(self, nibble):
-        if self.a == 128: self.shuffle()
+        if self.a == 128:
+            self.shuffle()
         self._swap(self.a, 128 + nibble)
         self.a = self._add(self.a, 1)
```

### Comparing `quorum-0.8.2/src/quorum/acl.py` & `quorum-0.8.3/src/quorum/acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
@@ -44,146 +35,166 @@
 from . import log
 
 SEQUENCE_TYPES = (list, tuple)
 """ The tuple defining the various data types in
 python that are considered to be representing a
 logical sequence """
 
+
 def check_basic_auth(username, password):
     authorization = flask.request.authorization
-    if not authorization: return False
-    if not authorization.username == username: return False
-    if not authorization.password == password: return False
+    if not authorization:
+        return False
+    if not authorization.username == username:
+        return False
+    if not authorization.password == password:
+        return False
     return True
 
-def check_login(token = None):
+
+def check_login(token=None):
     # retrieves the data type of the token and creates the
     # tokens sequence value taking into account its type
-    if isinstance(token, SEQUENCE_TYPES): tokens = token
-    else: tokens = (token,)
+    if isinstance(token, SEQUENCE_TYPES):
+        tokens = token
+    else:
+        tokens = (token,)
 
     # in case the username value is set in session and there's
     # no token to be validated returns valid and in case the checking
     # of the complete set of tokens is valid also returns valid
-    if check_user() and not token: return True
-    if check_tokens(tokens): return True
+    if check_user() and not token:
+        return True
+    if check_tokens(tokens):
+        return True
 
     # returns the default value as invalid because if all the
     # validation procedures have failed the check is invalid
     return False
 
+
 def check_user():
     # runs the multiple verification strategies available an
     # in case at least one of them succeeds the user is considered
     # to be currently authenticated
-    if "username" in flask.session: return True
-    if hasattr(flask, "tokens_p"): return True
+    if "username" in flask.session:
+        return True
+    if hasattr(flask, "tokens_p"):
+        return True
 
     # by default the user is considered to be not authenticated, all
     # of the tests for authentication have failed
     return False
 
-def check_token(token, tokens_m = None):
+
+def check_token(token, tokens_m=None):
     # in case the provided token is invalid or empty the method
     # return immediately in success (simple validation)
-    if not token: return True
+    if not token:
+        return True
 
     # tries to retrieve the tokens map from the provided argument
     # defaulting to the session one in case none is provided
-    if tokens_m == None: tokens_m = get_tokens_m()
+    if tokens_m == None:
+        tokens_m = get_tokens_m()
 
     # splits the provided token string into its parts, note that
     # a namespace is defined around the dot character
     token_l = token.split(".")
 
     # iterates over the complete set of parts in the token list
     # of parts to validate the complete chain of values against
     # the map of token parts (namespace validation)
     for token_p in token_l:
-        if not isinstance(tokens_m, dict): return False
-        if "*" in tokens_m and tokens_m["*"] == True: return True
-        if not token_p in tokens_m: return False
+        if not isinstance(tokens_m, dict):
+            return False
+        if "*" in tokens_m and tokens_m["*"] == True:
+            return True
+        if not token_p in tokens_m:
+            return False
         tokens_m = tokens_m[token_p]
 
     # determines if the final tokens map value is a dictionary
     # and "selects" the proper validation result accordingly
     is_dict = isinstance(tokens_m, dict)
     result = tokens_m.get("_", False) if is_dict else tokens_m
 
     # verifies if the "final" result value is valid and returns
     # the final validation result accordingly
     return True if result == True else False
 
-def check_tokens(tokens, tokens_m = None):
+
+def check_tokens(tokens, tokens_m=None):
     # iterates over the complete set of tokens that are going
     # to be validated against the current context and if any of
     # them fails an invalid result is returned otherwise a valid
     # result is returned (indicating that all is valid)
     for token in tokens:
-        if not check_token(token, tokens_m = tokens_m): return False
+        if not check_token(token, tokens_m=tokens_m):
+            return False
     return True
 
-def ensure_basic_auth(username, password, json_s = False):
+
+def ensure_basic_auth(username, password, json_s=False):
     check = check_basic_auth(username, password)
-    if check: return
+    if check:
+        return
 
     log.info("Unauthorized for operation")
 
-    if json_s: return flask.Response(
-            json.dumps({
-                "exception" : {
-                    "message" : "Unauthorized for operation"
-                }
-            }),
-            status = 401,
-            mimetype = "application/json"
+    if json_s:
+        return flask.Response(
+            json.dumps({"exception": {"message": "Unauthorized for operation"}}),
+            status=401,
+            mimetype="application/json",
         )
     else:
         return flask.redirect(
             flask.url_for(
-                "login",
-                next = flask.request.path,
-                error = "Session expired or invalid"
+                "login", next=flask.request.path, error="Session expired or invalid"
             )
         )
 
-def ensure_login(token = None, json_s = False):
-    if check_login(token = token): return None
+
+def ensure_login(token=None, json_s=False):
+    if check_login(token=token):
+        return None
 
     log.info("Not enough permissions for operation")
 
     if json_s:
         return flask.Response(
-            json.dumps({
-                "exception" : {
-                    "message" : "Not enough permissions for operation"
-                }
-            }),
-            status = 403,
-            mimetype = "application/json"
+            json.dumps(
+                {"exception": {"message": "Not enough permissions for operation"}}
+            ),
+            status=403,
+            mimetype="application/json",
         )
     else:
         return flask.redirect(
             flask.url_for(
-                "login",
-                next = flask.request.path,
-                error = "Session expired or invalid"
+                "login", next=flask.request.path, error="Session expired or invalid"
             )
         )
 
+
 def ensure_user(username):
     _username = flask.session.get("username", None)
-    if not _username == None and username == _username: return
+    if not _username == None and username == _username:
+        return
     raise RuntimeError("Permission denied")
 
+
 def ensure_session(object):
-    if object.get("sesion_id", None) == flask.session.get("session_id", None): return
+    if object.get("sesion_id", None) == flask.session.get("session_id", None):
+        return
     raise RuntimeError("Permission denied")
 
-def ensure(token = None, json = False):
+
+def ensure(token=None, json=False):
     """
     Decorator that provides support for verifying the current
     session login and permission (token oriented).
 
     The basic (login) verification ensures that the username
     session variable is set to a not null value (user logged in).
 
@@ -205,22 +216,24 @@
     """
 
     def decorator(function):
 
         @functools.wraps(function)
         def interceptor(*args, **kwargs):
             ensure = ensure_login(token, json)
-            if ensure: return ensure
+            if ensure:
+                return ensure
             return function(*args, **kwargs)
 
         return interceptor
 
     return decorator
 
-def ensure_auth(username, password, json = False):
+
+def ensure_auth(username, password, json=False):
     """
     Decorator that provides support for verifying the current
     request basic authentication information for the provided
     username and password.
 
     An optional JSON parameter may be set in case the return
     error value should be returned as a JSON response instead
@@ -240,22 +253,24 @@
     """
 
     def decorator(function):
 
         @functools.wraps(function)
         def interceptor(*args, **kwargs):
             ensure = ensure_basic_auth(username, password, json)
-            if ensure: return ensure
+            if ensure:
+                return ensure
             return function(*args, **kwargs)
 
         return interceptor
 
     return decorator
 
-def get_tokens_m(set = True):
+
+def get_tokens_m(set=True):
     """
     Retrieves the map of tokens from the current session so that
     they can be used for proper ACL validation.
 
     In case the current session contains a sequence based representation
     of the tokens they are converted to their equivalent map value.
 
@@ -274,46 +289,51 @@
     if set == None:
         set = False if hasattr(flask, "tokens_p") else True
 
     # tries to retrieve the "provider method "for the tokens under the
     # current request an in case it's not available used the default
     # one (simple session access)
     try:
-        if hasattr(flask, "tokens_p"): tokens_m = flask.tokens_p()
-        else: tokens_m = flask.session.get("tokens", {})
+        if hasattr(flask, "tokens_p"):
+            tokens_m = flask.tokens_p()
+        else:
+            tokens_m = flask.session.get("tokens", {})
     except Exception:
         return dict()
 
     # verifies if the resulting value is either a map or a sequence,
     # going to be used for decisions on normalization
     is_map = isinstance(tokens_m, dict)
     is_sequence = isinstance(tokens_m, (list, tuple))
 
     # if the tokens value is already a map then an immediate return
     # is going to be performed (it is a valid tokens map)
-    if is_map: return tokens_m
+    if is_map:
+        return tokens_m
 
     # in case the value present in the tokens value is a sequence
     # it must be properly converted into the equivalent map value
     if is_sequence:
         # converts the tokens sequence into a map version of it
         # so that proper structured verification is possible
         tokens_m = to_tokens_m(tokens_m)
 
         # in case the set flag is set the tokens map should
         # be set in the request session (may be dangerous)
         # and then returns the tokens map to the caller method
-        if set: flask.session["tokens"] = tokens_m
+        if set:
+            flask.session["tokens"] = tokens_m
         return tokens_m
 
     # returns the "default" empty tokens map as it was not possible
     # to retrieve any information regarding tokens from the
     # current context and environment
     return dict()
 
+
 def to_tokens_m(tokens):
     # creates a new map to be used to store tokens map that is
     # going to be created from the list/sequence version
     tokens_m = dict()
 
     # iterates over the complete set of tokens in the
     # sequence to properly add their namespace parts
@@ -322,18 +342,21 @@
         tokens_c = tokens_m
         token_l = token.split(".")
         head, tail = token_l[:-1], token_l[-1]
 
         for token_p in head:
             current = tokens_c.get(token_p, {})
             is_dict = isinstance(current, dict)
-            if not is_dict: current = {"_" : current}
+            if not is_dict:
+                current = {"_": current}
             tokens_c[token_p] = current
             tokens_c = current
 
         leaf = tokens_c.get(tail, None)
-        if leaf and isinstance(leaf, dict): leaf["_"] = True
-        else: tokens_c[tail] = True
+        if leaf and isinstance(leaf, dict):
+            leaf["_"] = True
+        else:
+            tokens_c[tail] = True
 
     # returns the final map version of the token to the caller
     # method so that it may be used for structure verification
     return tokens_m
```

### Comparing `quorum-0.8.2/src/quorum/date.py` & `quorum-0.8.3/src/quorum/date.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,41 +18,36 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-def format_delta(time_delta, count = 2):
+
+def format_delta(time_delta, count=2):
     days = time_delta.days
     hours, remainder = divmod(time_delta.seconds, 3600)
     minutes, seconds = divmod(remainder, 60)
     delta_s = ""
     if days > 0:
         delta_s += "%dd " % days
         count -= 1
-    if count == 0: return delta_s.strip()
+    if count == 0:
+        return delta_s.strip()
     if hours > 0:
         delta_s += "%dh " % hours
         count -= 1
-    if count == 0: return delta_s.strip()
+    if count == 0:
+        return delta_s.strip()
     if minutes > 0:
         delta_s += "%dm " % minutes
         count -= 1
-    if count == 0: return delta_s.strip()
+    if count == 0:
+        return delta_s.strip()
     delta_s += "%ds" % seconds
     return delta_s.strip()
```

### Comparing `quorum-0.8.2/src/quorum/mail.py` & `quorum-0.8.3/src/quorum/mail.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -50,30 +41,31 @@
 
 from . import httpc
 from . import config
 from . import common
 from . import legacy
 from . import execution
 
+
 def send_mail(
-    app = None,
-    subject = "",
-    sender = None,
-    receivers = [],
-    data = None,
-    plain = None,
-    rich = None,
-    context = {},
-    encoding = "utf-8",
-    host = None,
-    port = None,
-    username = None,
-    password = None,
-    stls = False,
-    safe = True
+    app=None,
+    subject="",
+    sender=None,
+    receivers=[],
+    data=None,
+    plain=None,
+    rich=None,
+    context={},
+    encoding="utf-8",
+    host=None,
+    port=None,
+    username=None,
+    password=None,
+    stls=False,
+    safe=True,
 ):
     """
     Sends an email message using the provided :rst:dir:`SMTP_HOST`,
     :rst:dir:`SMTP_USER` and :rst:dir:`SMTP_PASSWORD` configurations.
 
     The email message is sent under the ``alternative`` mime
     type so that both the plain text and the rich text (HTML)
@@ -152,38 +144,40 @@
     data = data or "This part of the email is empty"
 
     # tries to retrieve the URL based definition of the SMTP
     # settings so that they may be used for configuration
     url = config.conf("SMTP_URL", None)
     url_p = legacy.urlparse(url) if url else None
     if url_p:
-        host_p, port_p, user_p, password_p, stls_p =\
-        url_p.hostname,\
-        url_p.port,\
-        url_p.username,\
-        url_p.password,\
-        url_p.scheme == "smtps"
+        host_p, port_p, user_p, password_p, stls_p = (
+            url_p.hostname,
+            url_p.port,
+            url_p.username,
+            url_p.password,
+            url_p.scheme == "smtps",
+        )
     else:
-        host_p, port_p, user_p, password_p, stls_p =\
-        None, None, None, None, None
+        host_p, port_p, user_p, password_p, stls_p = None, None, None, None, None
 
     # runs the defaulting operation for host and port definition
     # that haven't been set (should follow SMTP defaults)
-    if host_p == None: host_p = "localhost"
-    if port_p == None: port_p = 25
+    if host_p == None:
+        host_p = "localhost"
+    if port_p == None:
+        port_p = 25
 
     # tries to retrieve the various configuration values that are going
     # to be used for the establishment of the SMTP connection, taking
     # into account both the provided parameters and the configuration
     # variables currently defined for the environment
     host = host or config.conf("SMTP_HOST", host_p)
-    port = port or config.conf("SMTP_PORT", port_p, cast = int)
+    port = port or config.conf("SMTP_PORT", port_p, cast=int)
     username = username or config.conf("SMTP_USER", user_p)
     password = password or config.conf("SMTP_PASSWORD", password_p)
-    stls = password or stls or config.conf("SMTP_STARTTLS", stls_p, cast = bool)
+    stls = password or stls or config.conf("SMTP_STARTTLS", stls_p, cast=bool)
 
     # sets the sender with the SMTP user value in case no values
     # has been provided (expected behavior)
     sender = sender or username
 
     # tries to run the template resolution process, by using this approach
     # it's possible to retrieve remote based templates (dynamic loading)
@@ -194,50 +188,54 @@
     # and rich text object retrieving the final data to be sent
     plain_data = plain and _render(app, plain, **context) or data
     html_data = rich and _render(app, rich, **context) or data
 
     # verifies the existence of data (both plain and HTML) and in
     # there's data it should be encoded using the currently provided
     # one so that the raw data is used instead of the unicode one
-    if plain_data: plain_data = plain_data.encode(encoding)
-    if html_data: html_data = html_data.encode(encoding)
+    if plain_data:
+        plain_data = plain_data.encode(encoding)
+    if html_data:
+        html_data = html_data.encode(encoding)
 
     # creates the mime's multipart object with the appropriate header
     # values set and in the alternative model (for HTML compatibility)
     message = _multipart()
     message["Subject"] = subject
     message["From"] = _format(sender)
     message["To"] = ", ".join(_format(receiver) for receiver in receivers)
 
     # creates both the plain text and the rich text (HTML) objects
     # from the provided data and then attached them to the message
     # (multipart alternative) that is the base structure
-    plain = plain_data and _plain(plain_data, encoding = encoding)
-    html = html_data and _html(html_data, encoding = encoding)
+    plain = plain_data and _plain(plain_data, encoding=encoding)
+    html = html_data and _html(html_data, encoding=encoding)
     plain and message.attach(plain)
     html and message.attach(html)
 
     # converts the created message into a plain string value and then
     # in case the safe flag is active replaces the proper newline
     # sequences so that the mail string is made standard
     contents = message.as_string()
     if safe:
         contents = contents.replace("\r\n", "\n")
         contents = contents.replace("\n", "\r\n")
 
     # creates the connection with the SMTP server and starts the tls
     # connection to send the created email message
-    server = smtplib.SMTP(host, port = port)
+    server = smtplib.SMTP(host, port=port)
     try:
-        if stls: server.starttls()
+        if stls:
+            server.starttls()
         server.login(username, password)
         server.sendmail(sender, receivers, contents)
     finally:
         server.quit()
 
+
 def send_mail_a(*args, **kwargs):
     """
     Asynchronous call to the :func:`quorum.send_mail` function that
     is executed in a different thread from the current one. The currently
     loaded queue system is used for the sending of the email, for more
     information check on :func:`quorum.run_background` .
 
@@ -245,43 +243,54 @@
 
         The arguments to be send for this function are the same as the one
         present in the original :func:`quorum.send_mail` function.
     """
 
     execution.insert_work(send_mail, args, kwargs)
 
+
 def _multipart():
     return email.mime.multipart.MIMEMultipart("alternative")
 
-def _plain(contents, encoding = "utf-8"):
+
+def _plain(contents, encoding="utf-8"):
     return email.mime.text.MIMEText(contents, "plain", encoding)
 
-def _html(contents, encoding = "utf-8"):
+
+def _html(contents, encoding="utf-8"):
     return email.mime.text.MIMEText(contents, "html", encoding)
 
-def _format(address, encoding = "utf-8"):
+
+def _format(address, encoding="utf-8"):
     address_name, address_email = email.utils.parseaddr(address)
-    if legacy.is_bytes(address_name): address_name = address_name.decode(encoding)
-    address_name = email.header.Header(address_name, charset = encoding)
+    if legacy.is_bytes(address_name):
+        address_name = address_name.decode(encoding)
+    address_name = email.header.Header(address_name, charset=encoding)
     address_name = address_name.encode()
     address_email = str(address_email)
     return "%s <%s>" % (address_name, address_email)
 
+
 def _try_resolve(template_name):
-    if not template_name: return template_name
-    if not template_name.startswith(("http://", "https://")): return template_name
+    if not template_name:
+        return template_name
+    if not template_name.startswith(("http://", "https://")):
+        return template_name
     contents = httpc.get(template_name)
     base_name = os.path.basename(template_name)
     base_split = base_name.split(".", 1)
     base_extension = "." + base_split[1] if len(base_split) > 1 else ""
     file_name = str(uuid.uuid4()) + base_extension
     file_path = os.path.join(common.base().templates_path(), file_name)
     if not os.path.exists(common.base().templates_path()):
         os.makedirs(common.base().templates_path())
     file = open(file_path, "wb")
-    try: file.write(contents)
-    finally: file.close()
+    try:
+        file.write(contents)
+    finally:
+        file.close()
     return file_name
 
+
 def _render(app, template_name, **context):
     template = app.jinja_env.get_or_select_template(template_name)
     return flask.templating._render(template, context, app)
```

### Comparing `quorum-0.8.2/src/quorum/session.py` & `quorum-0.8.3/src/quorum/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import uuid
@@ -42,108 +33,112 @@
 import pickle
 import datetime
 
 import werkzeug.datastructures
 
 from . import redisdb
 
+
 class RedisSession(werkzeug.datastructures.CallbackDict, flask.sessions.SessionMixin):
 
-    def __init__(self, initial = None, sid = None, new = False):
-        def on_update(self): self.modified = True
+    def __init__(self, initial=None, sid=None, new=False):
+        def on_update(self):
+            self.modified = True
+
         werkzeug.datastructures.CallbackDict.__init__(self, initial, on_update)
 
         self.sid = sid
         self.new = new
         self.modified = False
 
+
 class RedisSessionInterface(flask.sessions.SessionInterface):
 
     serializer = pickle
     """ The serializer to be used for the values
     contained in the session (used on top of the class) """
 
     session_class = RedisSession
     """ The class to be used to encapsulate a session
     the generated object will be serialized """
 
-    def __init__(self, _redis = None, prefix = "session:", url = None):
-        if _redis == None: _redis = redisdb._get_connection(url)
+    def __init__(self, _redis=None, prefix="session:", url=None):
+        if _redis == None:
+            _redis = redisdb._get_connection(url)
 
         self.redis = _redis
         self.prefix = prefix
 
     def generate_sid(self):
         return str(uuid.uuid4())
 
     def get_redis_expiration_time(self, app, session):
-        if session.permanent: return app.permanent_session_lifetime
-        return datetime.timedelta(days = 1)
+        if session.permanent:
+            return app.permanent_session_lifetime
+        return datetime.timedelta(days=1)
 
     def get_seconds(self, delta):
-        return (delta.microseconds + (delta.seconds + delta.days * 24 * 3600) * 10 ** 6) / 10 ** 6
+        return (
+            delta.microseconds + (delta.seconds + delta.days * 24 * 3600) * 10**6
+        ) / 10**6
 
     def open_session(self, app, request):
         # tries to retrieve the session identifier from the
         # application cookie (or from parameters) in case
         # none is found generates a new one using the default
         # strategy and returns a new session object with that
         # session identifier
         sid = request.args.get("sid", request.args.get("session_id"))
         sid = sid or request.form.get("sid", request.form.get("session_id"))
         sid = sid or request.cookies.get(app.session_cookie_name)
         if not sid:
             sid = self.generate_sid()
-            return self.session_class(sid = sid)
+            return self.session_class(sid=sid)
 
         # tries to retrieve the session value from Redis in
         # case the values is successfully found loads it using
         # the serializer and returns the session object
         value = self.redis.get(self.prefix + sid)
         if not value == None:
             data = self.serializer.loads(value)
-            return self.session_class(data, sid = sid)
+            return self.session_class(data, sid=sid)
 
         # returns a new session object with an already existing
         # session identifier, but not found in data source (Redis)
-        return self.session_class(sid = sid, new = True)
+        return self.session_class(sid=sid, new=True)
 
     def save_session(self, app, session, response):
         # retrieves the domain associated with the cookie to
         # be able to correctly modify it
         domain = self.get_cookie_domain(app)
 
         # in case the session is no longer valid must delete
         # the reference in the Redis object and delete the cookie
         # from the current response object
         if not session:
             self.redis.delete(self.prefix + session.sid)
-            if session.modified: response.delete_cookie(
-                app.session_cookie_name,
-                domain = domain
-            )
+            if session.modified:
+                response.delete_cookie(app.session_cookie_name, domain=domain)
             return
 
         # retrieves the Redis expiration date from the provided
         # session object and the expiration value for the cookie
         # and then serializes the dictionary version of the session
         # so that it may be set as a string value in Redis
         redis_expire = self.get_redis_expiration_time(app, session)
         cookie_expire = self.get_expiration_time(app, session)
         value = self.serializer.dumps(dict(session))
         total_seconds = self.get_seconds(redis_expire)
         self.redis.setex(
-            self.prefix + session.sid,
-            value = value,
-            time = int(total_seconds)
+            self.prefix + session.sid, value=value, time=int(total_seconds)
         )
 
         # sets the proper cookie value (with session identifier) in the
         # response object so that the client may be able to re-use the
         # session object latter for operations
         response.set_cookie(
             app.session_cookie_name,
             session.sid,
-            expires = cookie_expire,
-            httponly = True,
-            domain = domain
+            expires=cookie_expire,
+            httponly=True,
+            domain=domain,
         )
```

### Comparing `quorum-0.8.2/src/quorum/amqp.py` & `quorum-0.8.3/src/quorum/amqp.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,75 +18,75 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 from . import legacy
 from . import exceptions
 
-try: import pika
-except ImportError: pika = None
+try:
+    import pika
+except ImportError:
+    pika = None
 
 TIMEOUT = 100
 """ The time the retrieval of a connection waits before
 returning this avoid possible problems with the current
 implementation of the blocking client """
 
 connection = None
 """ The global wide connection to the AMQP server
 that is meant to be used across sessions """
 
 url = "amqp://guest:guest@localhost"
 """ The global variable containing the URL to be used
 for the connection with the service """
 
-def get_connection(force = False, timeout = TIMEOUT):
+
+def get_connection(force=False, timeout=TIMEOUT):
     global connection
-    if pika == None: raise exceptions.ModuleNotFound("pika")
-    if not force and connection: return connection
+    if pika == None:
+        raise exceptions.ModuleNotFound("pika")
+    if not force and connection:
+        return connection
     url_p = legacy.urlparse(url)
     parameters = _pika().ConnectionParameters(
-        host = url_p.hostname,
-        virtual_host = url_p.path or "/",
-        credentials = _pika().PlainCredentials(url_p.username, url_p.password)
+        host=url_p.hostname,
+        virtual_host=url_p.path or "/",
+        credentials=_pika().PlainCredentials(url_p.username, url_p.password),
     )
     parameters.socket_timeout = timeout
     connection = _pika().BlockingConnection(parameters)
     connection = _set_fixes(connection)
     return connection
 
+
 def properties(*args, **kwargs):
     return _pika().BasicProperties(*args, **kwargs)
 
+
 def _set_fixes(connection):
     def disconnect():
         connection.socket.close()
 
     if not hasattr(connection, "disconnect"):
         connection.disconnect = disconnect
     return connection
 
-def _pika(verify = True):
-    if verify: util.verify(
-        not pika == None,
-        message = "Pika library not available",
-        exception = exceptions.OperationalError
-    )
+
+def _pika(verify=True):
+    if verify:
+        util.verify(
+            not pika == None,
+            message="Pika library not available",
+            exception=exceptions.OperationalError,
+        )
     return pika
```

### Comparing `quorum-0.8.2/src/quorum/pusherc.py` & `quorum-0.8.3/src/quorum/pusherc.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,34 +18,27 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 from . import exceptions
 
-try: import pusher
-except ImportError: pusher = None
+try:
+    import pusher
+except ImportError:
+    pusher = None
 
 pusher_c = None
 """ The global pusher connection object to be used along
 multiple communications from the server side, when a client
 requests the pusher object this is the one returned (if cached) """
 
 app_id = None
@@ -61,28 +54,31 @@
 """ The secret key value that should be used by the publisher to
 authenticate it "against" the pusher service """
 
 cluster = None
 """ The cluster (datacenter) that should be used in the client
 connection that is going to be established """
 
+
 def get_pusher():
     global pusher_c
-    if pusher_c: return pusher_c
-    if pusher == None: raise exceptions.ModuleNotFound("pusher")
+    if pusher_c:
+        return pusher_c
+    if pusher == None:
+        raise exceptions.ModuleNotFound("pusher")
     kwargs = dict()
-    if cluster: kwargs["cluster"] = cluster
+    if cluster:
+        kwargs["cluster"] = cluster
     pusher_c = _pusher().Pusher(
-        app_id = str(app_id),
-        key = str(key),
-        secret = str(secret),
-        **kwargs
+        app_id=str(app_id), key=str(key), secret=str(secret), **kwargs
     )
     return pusher_c
 
-def _pusher(verify = True):
-    if verify: util.verify(
-        not pusher == None,
-        message = "Pusher library not available",
-        exception = exceptions.OperationalError
-    )
+
+def _pusher(verify=True):
+    if verify:
+        util.verify(
+            not pusher == None,
+            message="Pusher library not available",
+            exception=exceptions.OperationalError,
+        )
     return pusher
```

### Comparing `quorum-0.8.2/src/quorum/template.py` & `quorum-0.8.3/src/quorum/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,43 +18,36 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import flask
 
 from . import common
 
+
 def render_template(template_name_or_list, **context):
     # runs the resolution process in the provided template name
     # so that the proper name is going to be used when rendering
     # the template, then retrieves the underlying flask render
     # template function and calls it with the new resolved name
     template_name_or_list = template_resolve(template_name_or_list)
     render_template = getattr(flask, "_render_template")
     return render_template(template_name_or_list, **context)
 
+
 def template_resolve(template):
     """
     Resolves the provided template path, using the currently
     defined locale. It tries to find the best match for the
     template file falling back to the default (provided) template
     path in case the best one could not be found.
 
@@ -71,15 +64,17 @@
     # part so that it's possible to re-construct the name with the proper
     # locale naming part included in the name
     fbase, name = os.path.split(template)
     fname, extension = name.split(".", 1)
 
     # retrieves both the complete locale set under the current request and
     # the language base value for the same locale (to be used as fallback)
-    locale = flask.request.locale if hasattr(flask.request, "locale") else None  #@UndefinedVariable
+    locale = (
+        flask.request.locale if hasattr(flask.request, "locale") else None
+    )  # @UndefinedVariable
     language = locale.split("_", 1)[0] if locale else None
 
     # sets the fallback name as the "original" template path, because
     # that's the default and expected behavior for the template engine
     fallback = template
 
     # retrieves the base templates path from the base infra-structure this
@@ -88,48 +83,53 @@
     templates_path = common.base().templates_path()
 
     # iterates over the complete set of locale values eligible for the
     # resolution (this also takes into account the base language)
     for _locale in (locale, language):
         # in case the current value in iteration is not valid (not set
         # or empty) then the current iteration is not required
-        if not _locale: continue
+        if not _locale:
+            continue
 
         # creates the base file name for the target (locale based) template
         # and then joins the file name with the proper base path to create
         # the "full" target file name
         target = fname + "." + _locale + "." + extension
         target = fbase + "/" + target if fbase else target
 
         # "joins" the target path and the templates (base) path to create
         # the full path to the target template, then verifies if it exists
         # and in case it does sets it as the template name
         target_f = os.path.join(templates_path, target)
-        if os.path.exists(target_f): return target
+        if os.path.exists(target_f):
+            return target
 
     # runs the same operation for the fallback template name and verifies
     # for its existence in case it exists uses it as the resolved value
     fallback_f = os.path.join(templates_path, fallback)
-    if os.path.exists(fallback_f): return fallback
+    if os.path.exists(fallback_f):
+        return fallback
 
     # retrieves the reference to the currently loaded app so that its
     # properties are going to be used in the locales resolution
     app = common.base().APP
 
     # retrieves the current list of locales for he application and removes
     # any previously "visited" locale value (redundant) so that the list
     # represents the non visited locales by order of preference
     locales = list(app.locales)
-    if locale in locales: locales.remove(flask.request.locale)
+    if locale in locales:
+        locales.remove(flask.request.locale)
 
     # iterates over the complete list of locales trying to find the any
     # possible existing template that is compatible with the specification
     # note that the order of iteration should be associated with priority
     for locale in locales:
         target = fname + "." + locale + "." + extension
         target = fbase + "/" + target if fbase else target
         target_f = os.path.join(templates_path, target)
-        if os.path.exists(target_f): return target
+        if os.path.exists(target_f):
+            return target
 
     # returns the fallback value as the last option available, note that
     # for this situation the resolution process is considered failed
     return fallback
```

### Comparing `quorum-0.8.2/src/quorum/errors.py` & `quorum-0.8.3/src/quorum/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,64 +18,52 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
 import flask
 import functools
 
 from . import exceptions
 
+
 def errors_json(function):
 
     @functools.wraps(function)
     def interceptor(*args, **kwargs):
         try:
             return function(*args, **kwargs)
         except exceptions.ValidationError as error:
             invalid_m = {}
             for name, _errors in error.errors.items():
                 invalid_m[name] = _errors[0]
 
             return flask.Response(
-                json.dumps({
-                    "error" : error.message,
-                    "invalid" : invalid_m,
-                    "exception" : {
-                        "message" : error.message,
-                        "errors" : error.errors
+                json.dumps(
+                    {
+                        "error": error.message,
+                        "invalid": invalid_m,
+                        "exception": {"message": error.message, "errors": error.errors},
                     }
-                }),
-                status = error.code,
-                mimetype = "application/json"
+                ),
+                status=error.code,
+                mimetype="application/json",
             )
         except exceptions.OperationalError as error:
             return flask.Response(
-                json.dumps({
-                    "error" : error.message,
-                    "exception" : {
-                        "message" : error.message
-                    }
-                }),
-                status = error.code,
-                mimetype = "application/json"
+                json.dumps(
+                    {"error": error.message, "exception": {"message": error.message}}
+                ),
+                status=error.code,
+                mimetype="application/json",
             )
 
     return interceptor
```

### Comparing `quorum-0.8.2/src/quorum/redisdb.py` & `quorum-0.8.3/src/quorum/redisdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,48 +18,42 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import json
 import shelve
 
 from . import util
 from . import config
 from . import exceptions
 
-try: import redis
-except ImportError: redis = None
+try:
+    import redis
+except ImportError:
+    redis = None
 
 connection = None
 """ The global connection object that should persist
 the connection relation with the database service """
 
 url = None
 """ The global variable containing the URL to be used
 for the connection with the service """
 
+
 class RedisMemory(object):
     """
     "Local" in memory stub object that simulates
     the Redis interface, useful for debugging.
 
     This memory interface may create problems in
     a multiple process environment (non shared memory).
@@ -77,82 +71,88 @@
         name_s = str(name)
         return self.values.get(name_s)
 
     def set(self, name, value):
         name_s = str(name)
         self.values[name_s] = value
 
-    def setex(self, name, value, time = None):
+    def setex(self, name, value, time=None):
         self.set(name, value)
 
     def delete(self, name):
-        if not name in self.values: return
+        if not name in self.values:
+            return
         del self.values[name]
 
+
 class RedisShelve(RedisMemory):
     """
     "Local" in persistent stub object that simulates
     the Redis interface, useful for debugging.
 
     This shelve interface requires a writable path
     where its persistent file may be written.
     """
 
-    def __init__(self, path = "redis.shelve"):
+    def __init__(self, path="redis.shelve"):
         RedisMemory.__init__(self)
         self.db_path = path
         self.open_db()
 
     def close(self):
         self.values.close()
 
-    def set(self, name, value, secure = None):
+    def set(self, name, value, secure=None):
         RedisMemory.set(self, name, value)
         if secure == None:
             secure = self.db_secure()
         if secure:
             self.values.close()
             self.open_db()
         else:
             self.values.sync()
 
     def delete(self, name):
         name_s = str(name)
-        if not name_s in self.values: return
+        if not name_s in self.values:
+            return
         del self.values[name_s]
 
     def open_db(self):
         base_path = config.conf("SESSION_FILE_PATH", "")
         file_path = os.path.join(base_path, self.db_path)
-        self.values = shelve.open(
-            file_path,
-            protocol = 2,
-            writeback = True
-        )
+        self.values = shelve.open(file_path, protocol=2, writeback=True)
 
     def db_type(self):
         shelve_cls = type(self.values.dict)
         shelve_dbm = shelve_cls.__name__
         return shelve_dbm
 
     def db_secure(self):
         return self.db_type() == "dbm"
 
+
 def get_connection():
     return _get_connection(url)
 
+
 def dumps(*args):
     return json.dumps(*args)
 
+
 def _get_connection(url):
     global connection
-    if redis == None: raise exceptions.ModuleNotFound("redis")
-    if not connection: connection = url and _redis().from_url(url) or RedisShelve()
+    if redis == None:
+        raise exceptions.ModuleNotFound("redis")
+    if not connection:
+        connection = url and _redis().from_url(url) or RedisShelve()
     return connection
 
-def _redis(verify = True):
-    if verify: util.verify(
-        not redis == None,
-        message = "RedisPy library not available",
-        exception = exceptions.OperationalError
-    )
+
+def _redis(verify=True):
+    if verify:
+        util.verify(
+            not redis == None,
+            message="RedisPy library not available",
+            exception=exceptions.OperationalError,
+        )
     return redis
```

### Comparing `quorum-0.8.2/src/quorum/request.py` & `quorum-0.8.3/src/quorum/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,30 +18,22 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import flask
 
+
 class Request(flask.Request):
 
-    def __init__(self, environ, populate_request = True, shallow = False):
+    def __init__(self, environ, populate_request=True, shallow=False):
         flask.Request.__init__(self, environ, populate_request, shallow)
 
         self.properties = {}
```

### Comparing `quorum-0.8.2/setup.py` & `quorum-0.8.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Flask Quorum. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -47,47 +38,42 @@
 QUORUM_DIR = os.path.join(SRC_DIR, "quorum")
 sys.path.insert(0, SRC_DIR)
 sys.path.insert(0, QUORUM_DIR)
 
 import info
 
 setuptools.setup(
-    name = info.NAME,
-    version = info.VERSION,
-    author = info.AUTHOR,
-    author_email = info.EMAIL,
-    description = info.DESCRIPTION,
-    license = info.LICENSE,
-    keywords = info.KEYWORDS,
-    url = info.URL,
-    zip_safe = True,
-    packages = [
-        "quorum",
-        "quorum.test"
-    ],
-    test_suite = "quorum.test",
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    install_requires = [
-        "flask"
-    ],
-    classifiers = [
+    name=info.NAME,
+    version=info.VERSION,
+    author=info.AUTHOR,
+    author_email=info.EMAIL,
+    description=info.DESCRIPTION,
+    license=info.LICENSE,
+    keywords=info.KEYWORDS,
+    url=info.URL,
+    zip_safe=True,
+    packages=["quorum", "quorum.test"],
+    test_suite="quorum.test",
+    package_dir={"": os.path.normpath("src")},
+    install_requires=["flask"],
+    classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
-    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
-    long_description_content_type = "text/markdown"
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `quorum-0.8.2/README.md` & `quorum-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `quorum-0.8.2/PKG-INFO` & `quorum-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum
-Version: 0.8.2
+Version: 0.8.3
 Summary: Quorum Extensions for Flask
 Home-page: http://flask-quorum.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [![Quorum Extensions for Flask](res/logo.png)](http://flask-quorum.hive.pt)
```

