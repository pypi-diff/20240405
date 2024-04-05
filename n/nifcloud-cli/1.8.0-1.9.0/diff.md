# Comparing `tmp/nifcloud-cli-1.8.0.tar.gz` & `tmp/nifcloud-cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifcloud-cli-1.8.0.tar", last modified: Thu Aug 10 07:48:13 2023, max compression
+gzip compressed data, was "nifcloud-cli-1.9.0.tar", last modified: Fri Sep 29 06:41:33 2023, max compression
```

## Comparing `nifcloud-cli-1.8.0.tar` & `nifcloud-cli-1.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.076953 nifcloud-cli-1.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/bin/nifcloud
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.076953 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-10 07:48:13.000000 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-10 07:48:13.000000 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-10 07:48:13.000000 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-10 07:48:13.000000 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-10 07:48:13.000000 nifcloud-cli-1.8.0/nifcloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.076953 nifcloud-cli-1.8.0/nifcloudcli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/clidriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.076953 nifcloud-cli-1.8.0/nifcloudcli/customizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.080953 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/addmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/customizations/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.080953 nifcloud-cli-1.8.0/nifcloudcli/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/_retry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/cli.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/computing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.080953 nifcloud-cli-1.8.0/nifcloudcli/data/computing/3.0/
--rw-r--r--   0 runner    (1001) docker     (123)   756272 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/computing/3.0/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/computing/3.0/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/dns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.080953 nifcloud-cli-1.8.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/endpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/ess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.080953 nifcloud-cli-1.8.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/
--rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/v1/
--rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/v1/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/v1/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/nas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/nas/N2016-02-24/
--rw-r--r--   0 runner    (1001) docker     (123)    29599 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/nas/N2016-02-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)   133419 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/script/2015-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/script/2015-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/sdk-default-configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/service-activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/service-activity/2020-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.072952 nifcloud-cli-1.8.0/nifcloudcli/data/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/data/storage/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/data/storage/2006-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:48:13.084953 nifcloud-cli-1.8.0/nifcloudcli/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/nifcloudcli/topics/topic-tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-10 07:48:13.088953 nifcloud-cli-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-10 07:48:02.000000 nifcloud-cli-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/bin/nifcloud
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-09-29 06:41:33.000000 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-09-29 06:41:33.000000 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 06:41:33.000000 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-09-29 06:41:33.000000 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-29 06:41:33.000000 nifcloud-cli-1.9.0/nifcloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/clidriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/customizations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/addmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/customizations/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/_retry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/cli.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/computing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/data/computing/3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)   866228 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/computing/3.0/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20674 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/computing/3.0/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/dns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.499305 nifcloud-cli-1.9.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (127)    23643 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/endpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/ess/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/
+-rw-r--r--   0 runner    (1001) docker     (127)    30881 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)   113166 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/v1/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/v1/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/nas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/nas/N2016-02-24/
+-rw-r--r--   0 runner    (1001) docker     (127)    33565 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/nas/N2016-02-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (127)   146066 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/script/2015-09-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/script/2015-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/sdk-default-configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/service-activity/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/service-activity/2020-11-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.495304 nifcloud-cli-1.9.0/nifcloudcli/data/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/data/storage/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    95151 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/data/storage/2006-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/nifcloudcli/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/nifcloudcli/topics/topic-tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-29 06:41:33.503305 nifcloud-cli-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2023-09-29 06:41:21.000000 nifcloud-cli-1.9.0/setup.py
```

### Comparing `nifcloud-cli-1.8.0/LICENSE` & `nifcloud-cli-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/PKG-INFO` & `nifcloud-cli-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nifcloud==1.9.0
+Requires-Dist: awscli==1.29.1
+Requires-Dist: pyyaml==5.3.1
 
 # nifcloud-cli
 
 [![Test](https://github.com/nifcloud/nifcloud-cli/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-cli/actions?query=workflow%3ATest)
 [![PyPI](https://badge.fury.io/py/nifcloud-cli.svg)](https://pypi.org/project/nifcloud-cli)
 
 Universal Command Line Interface for NIFCLOUD Services
```

### Comparing `nifcloud-cli-1.8.0/README.md` & `nifcloud-cli-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloud_cli.egg-info/PKG-INFO` & `nifcloud-cli-1.9.0/nifcloud_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nifcloud==1.9.0
+Requires-Dist: awscli==1.29.1
+Requires-Dist: pyyaml==5.3.1
 
 # nifcloud-cli
 
 [![Test](https://github.com/nifcloud/nifcloud-cli/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-cli/actions?query=workflow%3ATest)
 [![PyPI](https://badge.fury.io/py/nifcloud-cli.svg)](https://pypi.org/project/nifcloud-cli)
 
 Universal Command Line Interface for NIFCLOUD Services
```

### Comparing `nifcloud-cli-1.8.0/nifcloud_cli.egg-info/SOURCES.txt` & `nifcloud-cli-1.9.0/nifcloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/clidriver.py` & `nifcloud-cli-1.9.0/nifcloudcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/commands.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/commands.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/addmodel.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/addmodel.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/configure.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/configure.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/get.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/get.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/list.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/list.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/configure/set.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/configure/set.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/customizations/waiters.py` & `nifcloud-cli-1.9.0/nifcloudcli/customizations/waiters.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/_retry.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/cli.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/computing/3.0/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/computing/3.0/service-2.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875000000000005%*

 * *Differences: {"'operations'": "{'AllocateAddress': {'documentation': "*

 * *                 "'<p>付替IPアドレスを割り当てます。1回のリクエストで、１つのグローバルIPアドレスまたはプライベートIPアドレスが割り当てられます。</p><p>割り当てられるIPアドレスは、ニフクラにより決定されます。</p><p>サーバーを指定した場合、共通グローバル/共通プライベートの固定IPアドレスが付替IPアドレスに変更されます。</p>'}, "*

 * *                 "'AssociateAddress': {'documentation': "*

 * *                 "'<p>指定したサーバーへ付替IPアドレスを追加します。</p><p>元々サーバーに割り当てられていたIPアドレスは、付替IPアドレス設定中は確保された状態となり、付替IPアドレス解除時に再設定されます。</p><p>また付替IPアドレスの反映には、サーバーの再起動が必要になります。</p><p>再起動オプションをfalseで指定する場合はサーバー停止時のみ選択可能 […]*

```diff
@@ -8,3108 +8,3347 @@
         "serviceId": "computing",
         "signatureVersion": "v2",
         "uid": "computing-2016-11-15",
         "xmlNamespace": "https://computing.api.nifcloud.com/api/"
     },
     "operations": {
         "AllocateAddress": {
+            "documentation": "<p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u5272\u308a\u5f53\u3066\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\uff11\u3064\u306e\u30b0\u30ed\u30fc\u30d0\u30ebIP\u30a2\u30c9\u30ec\u30b9\u307e\u305f\u306f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8IP\u30a2\u30c9\u30ec\u30b9\u304c\u5272\u308a\u5f53\u3066\u3089\u308c\u307e\u3059\u3002</p><p>\u5272\u308a\u5f53\u3066\u3089\u308c\u308bIP\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u30cb\u30d5\u30af\u30e9\u306b\u3088\u308a\u6c7a\u5b9a\u3055\u308c\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001\u5171\u901a\u30b0\u30ed\u30fc\u30d0\u30eb/\u5171\u901a\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8\u306e\u56fa\u5b9aIP\u30a2\u30c9\u30ec\u30b9\u304c\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306b\u5909\u66f4\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AllocateAddressRequest"
             },
             "name": "AllocateAddress",
             "output": {
                 "shape": "AllocateAddressResult"
             }
         },
         "AssociateAddress": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3078\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u5143\u3005\u30b5\u30fc\u30d0\u30fc\u306b\u5272\u308a\u5f53\u3066\u3089\u308c\u3066\u3044\u305fIP\u30a2\u30c9\u30ec\u30b9\u306f\u3001\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u8a2d\u5b9a\u4e2d\u306f\u78ba\u4fdd\u3055\u308c\u305f\u72b6\u614b\u3068\u306a\u308a\u3001\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u89e3\u9664\u6642\u306b\u518d\u8a2d\u5b9a\u3055\u308c\u307e\u3059\u3002</p><p>\u307e\u305f\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u53cd\u6620\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p><p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u30b5\u30fc\u30d0\u30fc\u3078\u8ffd\u52a0\u3059\u308b\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u3082\u3042\u308a\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u304c\u6b63\u3057\u304f\u30b5\u30fc\u30d0\u30fc\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cipType\u300d\u3082\u3057\u304f\u306fAPI\u300cDescribeAddresses\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceId\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AssociateAddressRequest"
             },
             "name": "AssociateAddress",
             "output": {
                 "shape": "AssociateAddressResult"
             }
         },
         "AssociateMultiIpAddressGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3078\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u5272\u308a\u5f53\u3066\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3078\u306e\u53cd\u6620\u306b\u306f\u3001\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AssociateMultiIpAddressGroupRequest"
             },
             "name": "AssociateMultiIpAddressGroup",
             "output": {
                 "shape": "AssociateMultiIpAddressGroupResult"
             }
         },
         "AssociateRouteTable": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3078\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u8a2d\u5b9a\u3059\u308b\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AssociateRouteTableRequest"
             },
             "name": "AssociateRouteTable",
             "output": {
                 "shape": "AssociateRouteTableResult"
             }
         },
         "AssociateUsers": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u6a5f\u80fd\u3092\u6307\u5b9a\u3057\u305f\u30e6\u30fc\u30b6\u30fc\u306b\u5171\u6709\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AssociateUsersRequest"
             },
             "name": "AssociateUsers",
             "output": {
                 "shape": "AssociateUsersResultWrapper"
             }
         },
         "AttachIsoImage": {
+            "documentation": "<p>ISO\u30a4\u30e1\u30fc\u30b8\u3092\u30b5\u30fc\u30d0\u30fc\u306b\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p><p>ISO\u30a4\u30e1\u30fc\u30b8\u30fb\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u305d\u308c\u305e\u308cISO\u30a4\u30e1\u30fc\u30b8ID\u30fb\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u8a2d\u5b9a\u3059\u308b\u30b5\u30fc\u30d0\u30fc\u306f\u3001ISO\u30a4\u30e1\u30fc\u30b8\u3068\u540c\u4e00\u30be\u30fc\u30f3\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AttachIsoImageRequest"
             },
             "name": "AttachIsoImage",
             "output": {
                 "shape": "AttachIsoImageResult"
             }
         },
         "AttachNetworkInterface": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306b\u8ffd\u52a0NIC\u3092\u63a5\u7d9a\u3057\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u8ffd\u52a0NIC\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30a4\u30f3\u30bf\u30fc\u30d5\u30a7\u30fc\u30b9ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u8ffd\u52a0NIC\u306e\u63a5\u7d9a\u306e\u53cd\u6620\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AttachNetworkInterfaceRequest"
             },
             "name": "AttachNetworkInterface",
             "output": {
                 "shape": "AttachNetworkInterfaceResult"
             }
         },
         "AttachVolume": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u3092\u30b5\u30fc\u30d0\u30fc\u3078\u63a5\u7d9a\u3057\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30c7\u30a3\u30b9\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AttachVolumeRequest"
             },
             "name": "AttachVolume",
             "output": {
                 "shape": "AttachVolumeResult"
             }
         },
         "AuthorizeSecurityGroupIngress": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3078\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u8a31\u53ef\u30eb\u30fc\u30eb\u306e\u8a31\u53ef\u30d7\u30ed\u30c8\u30b3\u30eb\u304cTCP\u304bUDP\u306e\u5834\u5408\u3001\u8a31\u53ef\u30dd\u30fc\u30c8\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002\u30dd\u30fc\u30c8\u3092\u5358\u4e00\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u307f\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002\u30dd\u30fc\u30c8\u3092\u7bc4\u56f2\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u7d42\u4e86\u30dd\u30fc\u30c8\u306b\u306f\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u5024\u4ee5\u4e0a\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u8a31\u53ef\u30eb\u30fc\u30eb\u306e\u8ffd\u52a0\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u9069\u7528\u6e08\u307f\u300d\u306e\u5834\u5408\u3001\u8ffd\u52a0\u3057\u305f\u8a31\u53ef\u30eb\u30fc\u30eb\u304c\u6b63\u3057\u304f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cipPermissions\u300d\u307e\u305f\u306f\u300cgroups\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "AuthorizeSecurityGroupIngressRequest"
             },
             "name": "AuthorizeSecurityGroupIngress",
             "output": {
                 "shape": "AuthorizeSecurityGroupIngressResult"
             }
         },
         "CancelCopyInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306e\u4f5c\u6210\uff08\u30b3\u30d4\u30fc\u306b\u3088\u308b\u4f5c\u6210\uff09\u3092\u30ad\u30e3\u30f3\u30bb\u30eb\u3057\u307e\u3059\u3002</p><p>\u4f5c\u6210\u5f85\u3061\u306e\u30b5\u30fc\u30d0\u30fc\u306e\u307f\u6307\u5b9a\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CancelCopyInstancesRequest"
             },
             "name": "CancelCopyInstances",
             "output": {
                 "shape": "CancelCopyInstancesResult"
             }
         },
         "CancelUpload": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u30a4\u30f3\u30dd\u30fc\u30c8\u306e\u51e6\u7406\u3092\u30ad\u30e3\u30f3\u30bb\u30eb\u3057\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u6e08\u307f\u306eVMDK\u30d5\u30a1\u30a4\u30eb\u306f\u524a\u9664\u3055\u308c\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u30bf\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30bf\u30b9\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CancelUploadRequest"
             },
             "name": "CancelUpload",
             "output": {
                 "shape": "CancelUploadResult"
             }
         },
         "ClearLoadBalancerSession": {
+            "documentation": "<p>\u30bb\u30c3\u30b7\u30e7\u30f3\u56fa\u5b9a\u30aa\u30d7\u30b7\u30e7\u30f3\u304c\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30bb\u30c3\u30b7\u30e7\u30f3\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ClearLoadBalancerSessionRequest"
             },
             "name": "ClearLoadBalancerSession",
             "output": {
                 "shape": "ClearLoadBalancerSessionResultWrapper"
             }
         },
         "ConfigureHealthCheck": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u5b9f\u884c\u7d50\u679c\u306f\u3001API\u300cDescribeInstanceHealth\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p> <h5 id=\"\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u969b\u306e\u30b5\u30fc\u30d0\u30fc\u5207\u308a\u96e2\u3057\u6642\u9593\u306b\u3064\u3044\u3066\">\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u969b\u306e\u30b5\u30fc\u30d0\u30fc\u5207\u308a\u96e2\u3057\u6642\u9593\u306b\u3064\u3044\u3066</h5> <ul> <li>\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u5fdc\u7b54\u6642\u9593\u304c\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u3092\u8d85\u3048\u305f\u5834\u5408\u306b\u30b5\u30fc\u30d0\u30fc\u3092\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304b\u3089\u5207\u308a\u96e2\u3057\u307e\u3059\u3002</li> <li>\u8a2d\u5b9a\u3055\u308c\u308b\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u6642\u9593\u306b\u3064\u3044\u3066\u306f\u3001<a href=\"https://pfs.nifcloud.com/service/lb_l4.htm\">\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\uff08L4\uff09\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306b\u3064\u3044\u3066</a>\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</li> <li>\u8a2d\u5b9a\u3055\u308c\u305f\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u6642\u9593\u306f\u3001\u300cDescribeLoadBalancers\u300d\u306e Timeout \u3067\u78ba\u8a8d\u304c\u3067\u304d\u307e\u3059\u3002</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ConfigureHealthCheckRequest"
             },
             "name": "ConfigureHealthCheck",
             "output": {
                 "shape": "ConfigureHealthCheckResultWrapper"
             }
         },
         "CopyFromBackupInstance": {
+            "documentation": "<p>\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3067\u4f5c\u6210\u3055\u308c\u305f\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u30b3\u30d4\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30b3\u30d4\u30fc\u3092\u884c\u3046\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b3\u30d4\u30fc\u3067\u4f5c\u6210\u3055\u308c\u305f\u30b5\u30fc\u30d0\u30fc\u306f\u3001\u505c\u6b62\u72b6\u614b\u3067\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CopyFromBackupInstanceRequest"
             },
             "name": "CopyFromBackupInstance",
             "output": {
                 "shape": "CopyFromBackupInstanceResult"
             }
         },
         "CopyInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306e\u30b3\u30d4\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u505c\u6b62\u4e2d\u3082\u3057\u304f\u306f\u8d77\u52d5\u4e2d\u306e\u30b5\u30fc\u30d0\u30fc\u306e\u307f\u6307\u5b9a\u304c\u3067\u304d\u307e\u3059\u3002\u30b3\u30d4\u30fc\u5f8c\u306e\u30b5\u30fc\u30d0\u30fc\u540d\u306f\u3001\u6307\u5b9a\u3057\u305f\u30b3\u30d4\u30fc\u5f8c\u306e\u30b5\u30fc\u30d0\u30fc\u540d\u306e\u5f8c\u308d\u306b\u300c-\u9023\u756a\u300d\u304c\u4ed8\u52a0\u3055\u308c\u305f\u540d\u79f0\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u304c\u63a5\u7d9a\u3057\u3066\u3044\u308b\u30b5\u30fc\u30d0\u30fc\u306e\u30b3\u30d4\u30fc\u306f\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3068\u540c\u4e00\u30be\u30fc\u30f3\u3067\u306e\u307f\u5b9f\u884c\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CopyInstancesRequest"
             },
             "name": "CopyInstances",
             "output": {
                 "shape": "CopyInstancesResult"
             }
         },
         "CreateBackupInstances": {
+            "documentation": "<p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30b5\u30fc\u30d0\u30fc\u306e\u3001\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4f5c\u6210\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateBackupInstancesRequest"
             },
             "name": "CreateBackupInstances",
             "output": {
                 "shape": "CreateBackupInstancesResult"
             }
         },
         "CreateCustomerGateway": {
+            "documentation": "<p>\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateCustomerGatewayRequest"
             },
             "name": "CreateCustomerGateway",
             "output": {
                 "shape": "CreateCustomerGatewayResult"
             }
         },
         "CreateDhcpOptions": {
+            "documentation": "<p>DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateDhcpOptionsRequest"
             },
             "name": "CreateDhcpOptions",
             "output": {
                 "shape": "CreateDhcpOptionsResult"
             }
         },
         "CreateImage": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u30a4\u30e1\u30fc\u30b8\u5316\u3057\u3001\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u3068\u3057\u3066\u4fdd\u5b58\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u30a4\u30e1\u30fc\u30b8\u5316\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u304c\u505c\u6b62\u4e2d\u3082\u3057\u304f\u306f\u8d77\u52d5\u4e2d\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306e\u4f5c\u6210\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cimageState\u300d\u3092\u78ba\u8a8d\u3057\u300cpending\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u3001\u307e\u305f\u306f\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u3057\u305f\u5834\u5408\u306f\u3001API\u300cDescribeImages\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cimageState\u300d\u3067\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u304c\u63a5\u7d9a\u3057\u3066\u3044\u308b\u30b5\u30fc\u30d0\u30fc\u306e\u30a4\u30e1\u30fc\u30b8\u5316\u306f\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3068\u540c\u4e00\u30be\u30fc\u30f3\u3067\u306e\u307f\u5b9f\u884c\u53ef\u80fd\u3067\u3059\u3002 \u30a4\u30e1\u30fc\u30b8\u5316\u5143\u30b5\u30fc\u30d0\u30fc\u3092\u6b8b\u3055\u306a\u3044\u5834\u5408\u306f\u3001\u95a2\u9023\u3059\u308b\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u8a2d\u5b9a\u3082\u3042\u308f\u305b\u3066\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateImageRequest"
             },
             "name": "CreateImage",
             "output": {
                 "shape": "CreateImageResult"
             }
         },
         "CreateInstanceBackupRule": {
+            "documentation": "<p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u4f5c\u6210\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u4f5c\u6210\u6642\u306b1\u3064\u306e\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u30022\u3064\u76ee\u4ee5\u964d\u306e\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u306f\u300cTimeSlotId\u300d\u3067\u6307\u5b9a\u3057\u305f\u5b9f\u884c\u6642\u9593\u5e2f\u306b\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p><p>\u624b\u52d5\u3067\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4f5c\u6210\u3059\u308b\u5834\u5408\u306f\u3001<a href=\"https://docs.nifcloud.com/cp/api/CreateBackupInstances.htm\">CreateBackupInstances</a>\u3092\u5b9f\u65bd\u3059\u308b\u3053\u3068\u3067\u4f5c\u6210\u3067\u304d\u307e\u3059\u3002</p><p>2\u56de\u76ee\u4ee5\u964d\u306e\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u306e\u4f5c\u6210\u306f\u3001\u521d\u56de\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u306e\u4f5c\u6210\u5b8c\u4e86\u5f8c\u306b\u53ef\u80fd\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u300cBackupInstanceMaxCount\u300d\u3067\u6307\u5b9a\u3057\u305f\u4fdd\u6301\u3059\u308b\u6700\u5927\u4e16\u4ee3\u6570\u3092\u8d85\u3048\u305f\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u304c\u4f5c\u6210\u3055\u308c\u305f\u5834\u5408\u3001\u6700\u3082\u53e4\u3044\u5897\u5206\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u306f\u524a\u9664\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateInstanceBackupRuleRequest"
             },
             "name": "CreateInstanceBackupRule",
             "output": {
                 "shape": "CreateInstanceBackupRuleResult"
             }
         },
         "CreateKeyPair": {
+            "documentation": "<p>SSH\u30ad\u30fc\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>SSH\u30ad\u30fc\u306b\u306f\u3001SSH\u30ad\u30fc\u540d\u304a\u3088\u3073\u30d1\u30b9\u30ef\u30fc\u30c9\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002SSH\u30ad\u30fc\u540d\u306b\u306f\u3001\u540c\u3058\u30e6\u30fc\u30b6\u30fc\u304c\u4f5c\u308b\u30ad\u30fc\u306e\u3046\u3061\u3001\u4e00\u610f\u3068\u306a\u308b\u6587\u5b57\u5217\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305fSSH\u30ad\u30fc\u30da\u30a2\u306e\u30d5\u30a3\u30f3\u30ac\u30fc\u30d7\u30ea\u30f3\u30c8\u304c\u4e00\u81f4\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306e\u78ba\u8a8d\u65b9\u6cd5\u306f\u3001<a href=\"https://docs.nifcloud.com/cp/api/DescribeKeyPairs.htm\">DescribeKeyPairs</a>\u306e\u51e6\u7406\u6982\u8981\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateKeyPairRequest"
             },
             "name": "CreateKeyPair",
             "output": {
                 "shape": "CreateKeyPairResult"
             }
         },
         "CreateLoadBalancer": {
+            "documentation": "<p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u5b9a\u7fa9\u3092\u4f5c\u6210\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30dd\u30fc\u30c8\u5b9a\u7fa9\u3092\u4f5c\u6210\u3067\u304d\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u5b9a\u7fa9\u306e\u4f5c\u6210\u306b\u6210\u529f\u3057\u305f\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300cRegisterInstancesWithLoadBalancer\u300d\uff08\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\uff09</li> <li>API\u300cConfigureHealthCheck\u300d\uff08\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u8a2d\u5b9a\uff09</li> </ul> <p>\u30d5\u30a3\u30eb\u30bf\u30fc\u306e\u8a2d\u5b9a\u306f\u3001\u300c\u3059\u3079\u3066\u306e\u30a2\u30af\u30bb\u30b9\u3092\u8a31\u53ef\u3059\u308b\u300d\u306b\u306a\u3063\u3066\u3044\u307e\u3059\u3002\u5909\u66f4\u3092\u884c\u3046\u5834\u5408\u306f\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300cSetFilterForLoadBalancer\u300d\uff08\u30d5\u30a3\u30eb\u30bf\u30fc\u8a2d\u5b9a\uff09</li> </ul> <p>Listeners.member.n.Protocol\u3068Listeners.member.n.LoadBalancerPort\u3092\u4e21\u65b9\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001Listeners.member.n.LoadBalancerPort\u306e\u6307\u5b9a\u304c\u512a\u5148\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateLoadBalancerRequest"
             },
             "name": "CreateLoadBalancer",
             "output": {
                 "shape": "CreateLoadBalancerResultWrapper"
             }
         },
         "CreateMultiIpAddressGroup": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u4f5c\u6210\u5f8c\u3001\u30b5\u30fc\u30d0\u30fc\u306b\u5272\u308a\u5f53\u3066\u308b\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300c<a href=\"https://docs.nifcloud.com/cp/api/AssociateMultiIpAddressGroup.htm\">AssociateMultiIpAddressGroup</a>\u300d</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateMultiIpAddressGroupRequest"
             },
             "name": "CreateMultiIpAddressGroup",
             "output": {
                 "shape": "CreateMultiIpAddressGroupResult"
             }
         },
         "CreateNetworkInterface": {
+            "documentation": "<p>\u8ffd\u52a0NIC\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u8ffd\u52a0NIC\u3092\u4f5c\u6210\u3067\u304d\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u306e\u4f5c\u6210\u306b\u306f\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cstatus\u300d\u3092\u78ba\u8a8d\u3057\u300cprocessing\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u3001\u307e\u305f\u306f\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u3057\u305f\u5834\u5408\u306fAPI\u300cDescribeNetworkInterfaces\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cstatus\u300d\u3067\u8ffd\u52a0NIC\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>API\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cNiftyNetworkId\u300d\u306e\u6307\u5b9a\u3067\u304d\u308b\u306e\u306f\u3001\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30e6\u30cb\u30fc\u30afID\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateNetworkInterfaceRequest"
             },
             "name": "CreateNetworkInterface",
             "output": {
                 "shape": "CreateNetworkInterfaceResult"
             }
         },
         "CreateRemoteAccessVpnGateway": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateRemoteAccessVpnGatewayRequest"
             },
             "name": "CreateRemoteAccessVpnGateway",
             "output": {
                 "shape": "CreateRemoteAccessVpnGatewayResult"
             }
         },
         "CreateRemoteAccessVpnGatewayUsers": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u30e6\u30fc\u30b6\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateRemoteAccessVpnGatewayUsersRequest"
             },
             "name": "CreateRemoteAccessVpnGatewayUsers",
             "output": {
                 "shape": "CreateRemoteAccessVpnGatewayUsersResult"
             }
         },
         "CreateRoute": {
+            "documentation": "<p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306b\u9069\u7528\u3059\u308b\u30eb\u30fc\u30c8\u60c5\u5831\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateRouteRequest"
             },
             "name": "CreateRoute",
             "output": {
                 "shape": "CreateRouteResult"
             }
         },
         "CreateRouteTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3059\u308b\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u65b0\u898f\u4f5c\u6210\u3092\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateRouteTableRequest"
             },
             "name": "CreateRouteTable",
             "output": {
                 "shape": "CreateRouteTableResult"
             }
         },
         "CreateSecurityGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u4f5c\u6210\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30d6\u30ed\u30fc\u30c9\u30ad\u30e3\u30b9\u30c8\u901a\u4fe1\u30ed\u30b0\u306e\u6291\u6b62\u72b6\u614b\u306f\u3001true\uff08\u6291\u6b62\uff09\u3067\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateSecurityGroupRequest"
             },
             "name": "CreateSecurityGroup",
             "output": {
                 "shape": "CreateSecurityGroupResult"
             }
         },
         "CreateSslCertificate": {
+            "documentation": "<p>SSL\u8a3c\u660e\u66f8\u306e\u65b0\u898f\u4f5c\u6210\u307e\u305f\u306f\u66f4\u65b0\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cfqdnId\u300d\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cfqdnId\u300d\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001SSL\u8a3c\u660e\u66f8\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u307e\u305f\u7533\u8acb\u6cd5\u4eba\u60c5\u5831\u3092\u767b\u9332\u3059\u308b\u306b\u306f\u3001API\u300cRegisterCorporateInfoForCertificate\u300d\u3092\u5b9f\u884c\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateSslCertificateRequest"
             },
             "name": "CreateSslCertificate",
             "output": {
                 "shape": "CreateSslCertificateResult"
             }
         },
         "CreateVolume": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u524a\u9664\u6e08\u307f\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u305f\u3001\u7ba1\u7406\u5916\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u305f\u3001\u8d77\u52d5\u4e2d\uff65\u505c\u6b62\u4e2d\u4ee5\u5916\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u305f\u306a\u3069\u3001\u7121\u52b9\u306a\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002 \u540c\u69d8\u306b\u3001\u30c7\u30a3\u30b9\u30af\u30b5\u30a4\u30ba\u304a\u3088\u3073\u30c7\u30a3\u30b9\u30af\u30bf\u30a4\u30d7\u306b\u898f\u5b9a\u5916\u306e\u5024\u3092\u6307\u5b9a\u3057\u305f\u3001\u3059\u3067\u306b\u5b58\u5728\u3059\u308b\u30c7\u30a3\u30b9\u30af\u540d\u3092\u6307\u5b9a\u3057\u305f\u3001\u5229\u7528\u6599\u91d1\u30bf\u30a4\u30d7\u306b\u7121\u52b9\u306a\u5024\u3092\u6307\u5b9a\u3057\u305f\u306a\u3069\u306e\u5834\u5408\u306f\u3001\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305f\u30c7\u30a3\u30b9\u30af\u306e\u30be\u30fc\u30f3\u306f\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3068\u540c\u4e00\u306e\u30be\u30fc\u30f3\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateVolumeRequest"
             },
             "name": "CreateVolume",
             "output": {
                 "shape": "CreateVolumeResult"
             }
         },
         "CreateVpnConnection": {
+            "documentation": "<p>VPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u8a2d\u5b9a\uff08\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3068\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u9593\uff09\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30c8\u30f3\u30cd\u30eb\u30e2\u30fc\u30c9\u3092\u300cManaged\u300d\u306b\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001\u4ee5\u4e0b\u306e\u9805\u76ee\u306f\u6307\u5b9a\u304c\u3067\u304d\u307e\u305b\u3093\u3002</p> <ul> <li>NiftyTunnel.TunnelId\u3001NiftyTunnel.PeerTunnelId\u3001NiftyTunnel.SessionId\u3001NiftyTunnel.PeerSessionId\u3001NiftyTunnel.SourcePort\u3001NiftyTunnel.DestinationPort</li> </ul> <p>\u307e\u305f\u30c8\u30f3\u30cd\u30eb\u30e2\u30fc\u30c9\u304c\u300cUnmanaged\u300d\u3067\u304b\u3064\u30ab\u30d7\u30bb\u30eb\u5316\u304c\u300cIP\u300d\u306e\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306e\u9805\u76ee\u306f\u6307\u5b9a\u304c\u3067\u304d\u307e\u305b\u3093\u3002</p> <ul> <li>NiftyTunnel.SourcePort\u3001NiftyTunnel.DestinationPort</li> </ul> <p>\u307e\u305f\u30c8\u30f3\u30cd\u30eb\u30bf\u30a4\u30d7\u304c\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u306a\u3044\u5834\u5408\u306f\u3001MTU\u30b5\u30a4\u30ba\u306f\u6307\u5b9a\u304c\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateVpnConnectionRequest"
             },
             "name": "CreateVpnConnection",
             "output": {
                 "shape": "CreateVpnConnectionResult"
             }
         },
         "CreateVpnGateway": {
+            "documentation": "<p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "CreateVpnGatewayRequest"
             },
             "name": "CreateVpnGateway",
             "output": {
                 "shape": "CreateVpnGatewayResult"
             }
         },
         "DeleteCustomerGateway": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305f\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteCustomerGatewayRequest"
             },
             "name": "DeleteCustomerGateway",
             "output": {
                 "shape": "DeleteCustomerGatewayResult"
             }
         },
         "DeleteDhcpOptions": {
+            "documentation": "<p>DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteDhcpOptionsRequest"
             },
             "name": "DeleteDhcpOptions",
             "output": {
                 "shape": "DeleteDhcpOptionsResult"
             }
         },
         "DeleteImage": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u3092\u9078\u629e\u3057\u3066\u4f5c\u6210\u3055\u308c\u305f\u30b5\u30fc\u30d0\u30fc\u306eOS\u30a4\u30e1\u30fc\u30b8\u540d\u306f\u3001\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306e\u524a\u9664\u304c\u5b8c\u4e86\u3059\u308b\u3068\u3001\u30a4\u30e1\u30fc\u30b8\u5316\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306eOS\u540d\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteImageRequest"
             },
             "name": "DeleteImage",
             "output": {
                 "shape": "DeleteImageResult"
             }
         },
         "DeleteInstanceBackupRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteInstanceBackupRuleRequest"
             },
             "name": "DeleteInstanceBackupRule",
             "output": {
                 "shape": "DeleteInstanceBackupRuleResult"
             }
         },
         "DeleteIsoImage": {
+            "documentation": "<p>ISO\u30a4\u30e1\u30fc\u30b8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306b\u8a2d\u5b9a\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u524a\u9664\u3067\u304d\u306a\u3044\u305f\u3081\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u89e3\u9664\u3057\u305f\u306e\u3061\u524a\u9664\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>ISO\u30a4\u30e1\u30fc\u30b8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001ISO\u30a4\u30e1\u30fc\u30b8ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteIsoImageRequest"
             },
             "name": "DeleteIsoImage",
             "output": {
                 "shape": "DeleteIsoImageResult"
             }
         },
         "DeleteKeyPair": {
+            "documentation": "<p>SSH\u30ad\u30fc\u306e\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>SSH\u30ad\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSH\u30ad\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteKeyPairRequest"
             },
             "name": "DeleteKeyPair",
             "output": {
                 "shape": "DeleteKeyPairResult"
             }
         },
         "DeleteLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30dd\u30fc\u30c8\u5b9a\u7fa9\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u95a2\u9023\u3059\u308b\u30d5\u30a3\u30eb\u30bf\u30fc\u8a2d\u5b9a\u30fb\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\u30fb\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u8a2d\u5b9a\u3082\u3042\u308f\u305b\u3066\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteLoadBalancerRequest"
             },
             "name": "DeleteLoadBalancer",
             "output": {
                 "shape": "DeleteLoadBalancerResultWrapper"
             }
         },
         "DeleteMultiIpAddressGroup": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteMultiIpAddressGroupRequest"
             },
             "name": "DeleteMultiIpAddressGroup",
             "output": {
                 "shape": "DeleteMultiIpAddressGroupResult"
             }
         },
         "DeleteNetworkInterface": {
+            "documentation": "<p>\u8ffd\u52a0NIC\u306e\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u8ffd\u52a0NIC\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30a4\u30f3\u30bf\u30fc\u30d5\u30a7\u30fc\u30b9ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteNetworkInterfaceRequest"
             },
             "name": "DeleteNetworkInterface",
             "output": {
                 "shape": "DeleteNetworkInterfaceResult"
             }
         },
         "DeleteRemoteAccessVpnGateway": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRemoteAccessVpnGatewayRequest"
             },
             "name": "DeleteRemoteAccessVpnGateway",
             "output": {
                 "shape": "DeleteRemoteAccessVpnGatewayResult"
             }
         },
         "DeleteRemoteAccessVpnGatewayConnections": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRemoteAccessVpnGatewayConnectionsRequest"
             },
             "name": "DeleteRemoteAccessVpnGatewayConnections",
             "output": {
                 "shape": "DeleteRemoteAccessVpnGatewayConnectionsResult"
             }
         },
         "DeleteRemoteAccessVpnGatewayUsers": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304b\u3089\u30e6\u30fc\u30b6\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRemoteAccessVpnGatewayUsersRequest"
             },
             "name": "DeleteRemoteAccessVpnGatewayUsers",
             "output": {
                 "shape": "DeleteRemoteAccessVpnGatewayUsersResult"
             }
         },
         "DeleteRoute": {
+            "documentation": "<p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306b\u9069\u7528\u3055\u308c\u305f\u30eb\u30fc\u30c8\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRouteRequest"
             },
             "name": "DeleteRoute",
             "output": {
                 "shape": "DeleteRouteResult"
             }
         },
         "DeleteRouteTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3059\u308b\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306e\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteRouteTableRequest"
             },
             "name": "DeleteRouteTable",
             "output": {
                 "shape": "DeleteRouteTableResult"
             }
         },
         "DeleteSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u524a\u9664\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteSecurityGroupRequest"
             },
             "name": "DeleteSecurityGroup",
             "output": {
                 "shape": "DeleteSecurityGroupResult"
             }
         },
         "DeleteSslCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\uff08fqdnId\uff09\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteSslCertificateRequest"
             },
             "name": "DeleteSslCertificate",
             "output": {
                 "shape": "DeleteSslCertificateResult"
             }
         },
         "DeleteVolume": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30c7\u30a3\u30b9\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u524a\u9664\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteVolumeRequest"
             },
             "name": "DeleteVolume",
             "output": {
                 "shape": "DeleteVolumeResult"
             }
         },
         "DeleteVpnConnection": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305fVPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u63a5\u7d9a\u3055\u308c\u3066\u3044\u308b\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteVpnConnectionRequest"
             },
             "name": "DeleteVpnConnection",
             "output": {
                 "shape": "DeleteVpnConnectionResult"
             }
         },
         "DeleteVpnGateway": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeleteVpnGatewayRequest"
             },
             "name": "DeleteVpnGateway",
             "output": {
                 "shape": "DeleteVpnGatewayResult"
             }
         },
         "DeregisterInstancesFromLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304b\u3089\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002\u81ea\u5206\u304c\u6240\u6709\u3057\u3066\u3044\u306a\u3044\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u3001\u300c\u30cb\u30d5\u30af\u30e9ID.\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u300d\u306e\u5f62\u5f0f\u3067\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u81ea\u5206\u304c\u6240\u6709\u3057\u3066\u3044\u306a\u3044\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u3001\u300c\u30cb\u30d5\u30af\u30e9ID.\u30b5\u30fc\u30d0\u30fc\u540d\u300d\u306e\u5f62\u5f0f\u3067\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeregisterInstancesFromLoadBalancerRequest"
             },
             "name": "DeregisterInstancesFromLoadBalancer",
             "output": {
                 "shape": "DeregisterInstancesFromLoadBalancerResultWrapper"
             }
         },
         "DeregisterInstancesFromSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u306f\u305a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u30b5\u30fc\u30d0\u30fc\u3092\u306f\u305a\u3059\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u9069\u7528\u6e08\u307f\u300d\u306e\u5834\u5408\u3001\u306f\u305a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u304c\u6b63\u3057\u304f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstancesSet\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DeregisterInstancesFromSecurityGroupRequest"
             },
             "name": "DeregisterInstancesFromSecurityGroup",
             "output": {
                 "shape": "DeregisterInstancesFromSecurityGroupResult"
             }
         },
         "DescribeAddresses": {
+            "documentation": "<p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u4ed8\u66ff\u30b0\u30ed\u30fc\u30d0\u30ebIP\u30a2\u30c9\u30ec\u30b9\u30fb\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8IP\u30a2\u30c9\u30ec\u30b9\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u307e\u305f\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c*\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001 \u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeAddressesRequest"
             },
             "name": "DescribeAddresses",
             "output": {
                 "shape": "DescribeAddressesResult"
             }
         },
         "DescribeAssociatedUsers": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u6a5f\u80fd\u306e\u5171\u6709\u30e6\u30fc\u30b6\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeAssociatedUsersRequest"
             },
             "name": "DescribeAssociatedUsers",
             "output": {
                 "shape": "DescribeAssociatedUsersResultWrapper"
             }
         },
         "DescribeAvailabilityZones": {
+            "documentation": "<p>\u5229\u7528\u53ef\u80fd\u306a\u30be\u30fc\u30f3\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u304c\u5229\u7528\u53ef\u80fd\u306a\u30be\u30fc\u30f3\u3067\u306f\u3001securityGroupSupported\u30bf\u30b0\u306btrue\u304c\u8fd4\u308a\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u4f5c\u6210\u6642\u306b\u30be\u30fc\u30f3\u3092\u7701\u7565\u3057\u305f\u5834\u5408\u3001isDefault\u30bf\u30b0\u304ctrue\u306e\u30be\u30fc\u30f3\u306b\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeAvailabilityZonesRequest"
             },
             "name": "DescribeAvailabilityZones",
             "output": {
                 "shape": "DescribeAvailabilityZonesResult"
             }
         },
         "DescribeCustomerGateways": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001\u4e0b\u8a18\u306e\u901a\u308a\u3067\u3059\u3002</p> <ul> <li>ip-address</li> <li>nifty-customer-gateway-name</li> <li>nifty-customer-gateway-description</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeCustomerGatewaysRequest"
             },
             "name": "DescribeCustomerGateways",
             "output": {
                 "shape": "DescribeCustomerGatewaysResult"
             }
         },
         "DescribeDhcpOptions": {
+            "documentation": "<p>DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>DHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eDHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001 \u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001key\u3001value\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeDhcpOptionsRequest"
             },
             "name": "DescribeDhcpOptions",
             "output": {
                 "shape": "DescribeDhcpOptionsResult"
             }
         },
         "DescribeImages": {
+            "documentation": "<p>OS\u30a4\u30e1\u30fc\u30b8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7279\u5b9a\u306eOS\u30a4\u30e1\u30fc\u30b8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001OS\u30a4\u30e1\u30fc\u30b8ID\u307e\u305f\u306fOS\u30a4\u30e1\u30fc\u30b8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002OS\u30a4\u30e1\u30fc\u30b8\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eOS\u30a4\u30e1\u30fc\u30b8\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeImagesRequest"
             },
             "name": "DescribeImages",
             "output": {
                 "shape": "DescribeImagesResult"
             }
         },
         "DescribeInstanceAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306e\u8a73\u7d30\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30b5\u30fc\u30d0\u30fc\u306e1\u3064\u306e\u8a73\u7d30\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeInstanceAttributeRequest"
             },
             "name": "DescribeInstanceAttribute",
             "output": {
                 "shape": "DescribeInstanceAttributeResult"
             }
         },
         "DescribeInstanceBackupRuleActivities": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u30a4\u30d9\u30f3\u30c8\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u53d6\u5f97\u3059\u308b\u30a4\u30d9\u30f3\u30c8\u30ed\u30b0\u60c5\u5831\u306f\u3001\u30a4\u30d9\u30f3\u30c8\u958b\u59cb\u65e5\u6642\u306e\u964d\u9806\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeInstanceBackupRuleActivitiesRequest"
             },
             "name": "DescribeInstanceBackupRuleActivities",
             "output": {
                 "shape": "DescribeInstanceBackupRuleActivitiesResult"
             }
         },
         "DescribeInstanceBackupRules": {
+            "documentation": "<p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeInstanceBackupRulesRequest"
             },
             "name": "DescribeInstanceBackupRules",
             "output": {
                 "shape": "DescribeInstanceBackupRulesResult"
             }
         },
         "DescribeInstanceHealth": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u7d50\u679c\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306f\u3001API\u300cConfigureHealthCheck\u300d\u3067\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u81ea\u5206\u304c\u6240\u6709\u3057\u3066\u3044\u306a\u3044\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u3001\u300c\u30cb\u30d5\u30af\u30e9ID.\u30b5\u30fc\u30d0\u30fc\u540d\u300d\u306e\u5f62\u5f0f\u3067\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u5bfe\u8c61\u3068\u3057\u3066\u3001\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u7d50\u679c\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeInstanceHealthRequest"
             },
             "name": "DescribeInstanceHealth",
             "output": {
                 "shape": "DescribeInstanceHealthResultWrapper"
             }
         },
         "DescribeInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8907\u6570\u306e\u30b5\u30fc\u30d0\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30b5\u30fc\u30d0\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeInstancesRequest"
             },
             "name": "DescribeInstances",
             "output": {
                 "shape": "DescribeInstancesResult"
             }
         },
         "DescribeIsoImages": {
+            "documentation": "<p>ISO\u30a4\u30e1\u30fc\u30b8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>ISO\u30a4\u30e1\u30fc\u30b8ID\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eISO\u30a4\u30e1\u30fc\u30b8\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0 \u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1 \u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217niftycloud\u00a5?\u00a5\u00a5 \u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeIsoImagesRequest"
             },
             "name": "DescribeIsoImages",
             "output": {
                 "shape": "DescribeIsoImagesResult"
             }
         },
         "DescribeKeyPairs": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSH\u30ad\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>SSH\u30ad\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSH\u30ad\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002SSH\u30ad\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306eSSH\u30ad\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ad\u30fc\u30da\u30a2\u306e\u30d5\u30a3\u30f3\u30ac\u30fc\u30d7\u30ea\u30f3\u30c8\u304c\u4e00\u81f4\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306f\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300ckeyFingerprint\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u79d8\u5bc6\u9375\u306b\u5bfe\u3057\u3001\u4ee5\u4e0b\u306e\u30b3\u30de\u30f3\u30c9\u3092\u5b9f\u884c\u3057\u305f\u5834\u5408\u306b\u53d6\u5f97\u3059\u308bfingerprint\u306e\u5024\u3068DescribeKeyPairs\u3067\u8fd4\u5374\u3055\u308c\u308bKeyFingerprint\u306e\u5024\u304c\u540c\u4e00\u3067\u3042\u308c\u3070\u3001\u30ad\u30fc\u30da\u30a2\u306e\u30d5\u30a3\u30f3\u30ac\u30fc\u30d7\u30ea\u30f3\u30c8\u304c\u4e00\u81f4\u3057\u3066\u3044\u308b\u3053\u3068\u304c\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>CreateKeyPair\u3067\u4f5c\u6210\u3057\u305f\u5834\u5408\uff1a</p><p>\u300copenssl rsa -in <span class=\"math inline\"><em>\u79d8</em><em>\u5bc6</em><em>\u9375</em><em>\u30d5</em><em>\u30a1</em><em>\u30a4</em><em>\u30eb</em>\u2005\u2212\u2005<em>p</em><em>u</em><em>b</em><em>o</em><em>u</em><em>t</em>\u2005\u2212\u2005<em>o</em><em>u</em><em>t</em><em>f</em><em>o</em><em>r</em><em>m</em><em>D</em><em>E</em><em>R</em>\u2005\u2212\u2005<em>p</em><em>a</em><em>s</em><em>s</em><em>i</em><em>n</em><em>p</em><em>a</em><em>s</em><em>s</em>:</span>{\u30d1\u30b9\u30d5\u30ec\u30fc\u30ba} | openssl md5 -c\u300d</p><p>ImportKeyPair\u3092\u5229\u7528\u3057\u305f\u969b\u306f\u3001\u9375\u5f62\u5f0f\u306b\u3042\u308f\u305b\u3066\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>SSH-RSA\u306e\u5834\u5408\uff1a\u300copenssl rsa -in <span class=\"math inline\"><em>\u79d8</em><em>\u5bc6</em><em>\u9375</em><em>\u30d5</em><em>\u30a1</em><em>\u30a4</em><em>\u30eb</em>\u2005\u2212\u2005<em>p</em><em>u</em><em>b</em><em>o</em><em>u</em><em>t</em>\u2005\u2212\u2005<em>o</em><em>u</em><em>t</em><em>f</em><em>o</em><em>r</em><em>m</em><em>D</em><em>E</em><em>R</em>\u2005\u2212\u2005<em>p</em><em>a</em><em>s</em><em>s</em><em>i</em><em>n</em><em>p</em><em>a</em><em>s</em><em>s</em>:</span>{\u30d1\u30b9\u30d5\u30ec\u30fc\u30ba} | openssl md5 ?c\u300d</p><p>SSH-DSA\u306e\u5834\u5408\uff1a\u300copenssl dsa -in <span class=\"math inline\"><em>\u79d8</em><em>\u5bc6</em><em>\u9375</em><em>\u30d5</em><em>\u30a1</em><em>\u30a4</em><em>\u30eb</em>\u2005\u2212\u2005<em>p</em><em>u</em><em>b</em><em>o</em><em>u</em><em>t</em>\u2005\u2212\u2005<em>o</em><em>u</em><em>t</em><em>f</em><em>o</em><em>r</em><em>m</em><em>D</em><em>E</em><em>R</em>\u2005\u2212\u2005<em>p</em><em>a</em><em>s</em><em>s</em><em>i</em><em>n</em><em>p</em><em>a</em><em>s</em><em>s</em>:</span>{\u30d1\u30b9\u30d5\u30ec\u30fc\u30ba} | openssl md5 ?c\u300d</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeKeyPairsRequest"
             },
             "name": "DescribeKeyPairs",
             "output": {
                 "shape": "DescribeKeyPairsResult"
             }
         },
         "DescribeLoadBalancers": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p> <h5 id=\"\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u969b\u306e\u30b5\u30fc\u30d0\u30fc\u5207\u308a\u96e2\u3057\u6642\u9593\u306b\u3064\u3044\u3066\">\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u969b\u306e\u30b5\u30fc\u30d0\u30fc\u5207\u308a\u96e2\u3057\u6642\u9593\u306b\u3064\u3044\u3066</h5> <ul> <li>\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u5fdc\u7b54\u6642\u9593\u304c\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u3092\u8d85\u3048\u305f\u5834\u5408\u306b\u30b5\u30fc\u30d0\u30fc\u3092\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304b\u3089\u5207\u308a\u96e2\u3057\u307e\u3059\u3002</li> <li>\u8a2d\u5b9a\u3055\u308c\u308b\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u6642\u9593\u306b\u3064\u3044\u3066\u306f\u3001<a href=\"https://pfs.nifcloud.com/service/lb_l4.htm\">\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\uff08L4\uff09\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306b\u3064\u3044\u3066</a>\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeLoadBalancersRequest"
             },
             "name": "DescribeLoadBalancers",
             "output": {
                 "shape": "DescribeLoadBalancersResultWrapper"
             }
         },
         "DescribeMultiIpAddressGroups": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8907\u6570\u306e\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeMultiIpAddressGroupsRequest"
             },
             "name": "DescribeMultiIpAddressGroups",
             "output": {
                 "shape": "DescribeMultiIpAddressGroupsResult"
             }
         },
         "DescribeNetworkInterfaces": {
+            "documentation": "<p>\u8ffd\u52a0NIC\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u8ffd\u52a0NIC\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u306e\u60c5\u5831\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u8ffd\u52a0NIC\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30a4\u30f3\u30bf\u30fc\u30d5\u30a7\u30fc\u30b9ID\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u8ffd\u52a0NIC\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\\\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217niftycloud\u00a5?\u00a5\u00a5 \u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001attachment.instance-id\u3001description\u3001nifty-network-name\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeNetworkInterfacesRequest"
             },
             "name": "DescribeNetworkInterfaces",
             "output": {
                 "shape": "DescribeNetworkInterfacesResult"
             }
         },
         "DescribeRegions": {
+            "documentation": "<p>\u5229\u7528\u53ef\u80fd\u306a\u30ea\u30fc\u30b8\u30e7\u30f3\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRegionsRequest"
             },
             "name": "DescribeRegions",
             "output": {
                 "shape": "DescribeRegionsResult"
             }
         },
         "DescribeRemoteAccessVpnGatewayActivities": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRemoteAccessVpnGatewayActivitiesRequest"
             },
             "name": "DescribeRemoteAccessVpnGatewayActivities",
             "output": {
                 "shape": "DescribeRemoteAccessVpnGatewayActivitiesResult"
             }
         },
         "DescribeRemoteAccessVpnGatewayClientConfig": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30af\u30e9\u30a4\u30a2\u30f3\u30c8\u8a2d\u5b9a\u30d5\u30a1\u30a4\u30eb\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002<br> \u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u304c v2.0.0 \u672a\u6e80\u306e\u5834\u5408\u3001\u5229\u7528\u3067\u304d\u307e\u305b\u3093</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRemoteAccessVpnGatewayClientConfigRequest"
             },
             "name": "DescribeRemoteAccessVpnGatewayClientConfig",
             "output": {
                 "shape": "DescribeRemoteAccessVpnGatewayClientConfigResult"
             }
         },
         "DescribeRemoteAccessVpnGatewayConnections": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRemoteAccessVpnGatewayConnectionsRequest"
             },
             "name": "DescribeRemoteAccessVpnGatewayConnections",
             "output": {
                 "shape": "DescribeRemoteAccessVpnGatewayConnectionsResult"
             }
         },
         "DescribeRemoteAccessVpnGateways": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRemoteAccessVpnGatewaysRequest"
             },
             "name": "DescribeRemoteAccessVpnGateways",
             "output": {
                 "shape": "DescribeRemoteAccessVpnGatewaysResult"
             }
         },
         "DescribeResources": {
+            "documentation": "<p>\u30ea\u30bd\u30fc\u30b9\u306e\u5229\u7528\u72b6\u6cc1\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>\u30b3\u30f3\u30c8\u30ed\u30fc\u30eb\u30d1\u30cd\u30eb\u753b\u9762\u306e\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9\u306b\u5f53\u305f\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeResourcesRequest"
             },
             "name": "DescribeResources",
             "output": {
                 "shape": "DescribeResourcesResult"
             }
         },
         "DescribeRouteTables": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID \u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0 \u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1 \u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217niftycloud\u00a5?\u00a5\u00a5 \u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002 \u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001association.router-name\u3001route.destination-cidr-block\u3001route.ip-address \u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeRouteTablesRequest"
             },
             "name": "DescribeRouteTables",
             "output": {
                 "shape": "DescribeRouteTablesResult"
             }
         },
         "DescribeSecurityActivities": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>ActivityDate\u306b\u201dall\u201d\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001Range\u8a2d\u5b9a\u3092\u7121\u8996\u3057\u4fdd\u5b58\u3055\u308c\u3066\u3044\u308b\u30ed\u30b0\u3092\u5168\u4ef6\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>(\u3053\u306e\u5834\u5408\u306b\u8fd4\u5374\u3055\u308c\u308b\u30ed\u30b0\u306e\u4ef6\u6570\u306b\u3064\u3044\u3066\u306f <a href=\"https://docs.nifcloud.com/cp/spec/fw/log.htm#%E3%83%AD%E3%82%B0%E4%BF%9D%E5%AD%98%E6%9C%9F%E9%96%93%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6\">\u6280\u8853\u4ed5\u69d8/\u5236\u9650\u5024 \u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\uff1a\u30ed\u30b0</a> \u3092\u3054\u53c2\u7167\u304f\u3060\u3055\u3044\u3002)</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeSecurityActivitiesRequest"
             },
             "name": "DescribeSecurityActivities",
             "output": {
                 "shape": "DescribeSecurityActivitiesResult"
             }
         },
         "DescribeSecurityGroups": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeSecurityGroupsRequest"
             },
             "name": "DescribeSecurityGroups",
             "output": {
                 "shape": "DescribeSecurityGroupsResult"
             }
         },
         "DescribeServiceStatus": {
+            "documentation": "<p>\u30b5\u30fc\u30d3\u30b9\u306e\u7a3c\u50cd\u60c5\u5831\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>\u30b3\u30f3\u30c8\u30ed\u30fc\u30eb\u30d1\u30cd\u30eb\u753b\u9762\u306e\u30c0\u30c3\u30b7\u30e5\u30dc\u30fc\u30c9\u306b\u5f53\u305f\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeServiceStatusRequest"
             },
             "name": "DescribeServiceStatus",
             "output": {
                 "shape": "DescribeServiceStatusResult"
             }
         },
         "DescribeSslCertificateAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u306e\u8a73\u7d30\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306eSSL\u8a3c\u660e\u66f8\u306e1\u3064\u306e\u8a73\u7d30\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\uff08fqdnId\uff09\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeSslCertificateAttributeRequest"
             },
             "name": "DescribeSslCertificateAttribute",
             "output": {
                 "shape": "DescribeSslCertificateAttributeResult"
             }
         },
         "DescribeSslCertificates": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\uff08fqdnId\uff09\u307e\u305f\u306fFQDN\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eSSL\u8a3c\u660e\u66f8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeSslCertificatesRequest"
             },
             "name": "DescribeSslCertificates",
             "output": {
                 "shape": "DescribeSslCertificatesResult"
             }
         },
         "DescribeUploads": {
+            "documentation": "<p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u4e2d\u306e\u30bf\u30b9\u30af\u60c5\u5831\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u30bf\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30bf\u30b9\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30bf\u30b9\u30afID\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001\u6307\u5b9a\u3057\u305fID\u306e\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u30bf\u30b9\u30af\u306e\u60c5\u5831\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p><p>\u30bf\u30b9\u30afID\u3092\u6307\u5b9a\u3057\u306a\u304b\u3063\u305f\u5834\u5408\u306f\u3001\u73fe\u5728\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u30fb\u30a4\u30f3\u30dd\u30fc\u30c8\u4e2d\u306e\u3059\u3079\u3066\u306e\u30bf\u30b9\u30af\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeUploadsRequest"
             },
             "name": "DescribeUploads",
             "output": {
                 "shape": "DescribeUploadsResult"
             }
         },
         "DescribeUsage": {
+            "documentation": "<p>\u30ea\u30bd\u30fc\u30b9\u306e\u5229\u7528\u72b6\u6cc1\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>\u5b58\u5728\u3059\u308b\u60c5\u5831\u306e\u307f\u3001\u30ec\u30b9\u30dd\u30f3\u30b9\u5185\u306b\u30bf\u30b0\u304c\u751f\u6210\u3055\u308c\u307e\u3059\u3002</p><p>\u53d6\u5f97\u5bfe\u8c61\u30ea\u30fc\u30b8\u30e7\u30f3\u3092\u8a2d\u5b9a\u3057\u305f\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u5229\u7528\u60c5\u5831\u306a\u3069\u305d\u306e\u30ea\u30fc\u30b8\u30e7\u30f3\u306b\u5c5e\u3059\u308b\u500b\u5225\u60c5\u5831\u3092\u3001\u6307\u5b9a\u3057\u306a\u304b\u3063\u305f\u5834\u5408\u306fSSL\u8a3c\u660e\u66f8\u5229\u7528\u60c5\u5831\u306a\u3069\u30ea\u30fc\u30b8\u30e7\u30f3\u5171\u901a\u60c5\u5831\u3068\u6771\u65e5\u672c\u30ea\u30fc\u30b8\u30e7\u30f3\u306e\u500b\u5225\u60c5\u5831\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>IsCharge=true\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001\u30ec\u30b9\u30dd\u30f3\u30b9\u306e\u5404\u30ea\u30bd\u30fc\u30b9\u306b\u5bfe\u3057\u3066\u5229\u7528\u6599\u91d1\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeUsageRequest"
             },
             "name": "DescribeUsage",
             "output": {
                 "shape": "DescribeUsageResult"
             }
         },
         "DescribeUserActivities": {
+            "documentation": "<p>API\u304a\u3088\u3073\u30b3\u30f3\u30c8\u30ed\u30fc\u30eb\u30d1\u30cd\u30eb\u306e\u5229\u7528\u5c65\u6b74\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002\u30b3\u30f3\u30c8\u30ed\u30fc\u30eb\u30d1\u30cd\u30eb\u753b\u9762\u306e\u30ed\u30b0\u53d6\u5f97\u306b\u5f53\u305f\u308a\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30a2\u30ab\u30a6\u30f3\u30c8\u306e\u5b50\u30a2\u30ab\u30a6\u30f3\u30c8\u3067\u306f\u3001\u81ea\u8eab\u306e\u5229\u7528\u5c65\u6b74\u306e\u307f\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p><p>\u53d6\u5f97\u958b\u59cb\u4f4d\u7f6e\u306f1\u304c\u6700\u65b0\u30ec\u30b3\u30fc\u30c9\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeUserActivitiesRequest"
             },
             "name": "DescribeUserActivities",
             "output": {
                 "shape": "DescribeUserActivitiesResult"
             }
         },
         "DescribeVolumes": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30c7\u30a3\u30b9\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002<br> \u524a\u9664\u6e08\u307f\u306e\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3057\u305f\u3001\u7ba1\u7406\u5916\u306e\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3057\u305f\u306a\u3069\u3001\u7121\u52b9\u306a\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30c7\u30a3\u30b9\u30af\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeVolumesRequest"
             },
             "name": "DescribeVolumes",
             "output": {
                 "shape": "DescribeVolumesResult"
             }
         },
         "DescribeVpnConnections": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305fVPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>VPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001VPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>VPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306eVPN\u30b3\u30cd\u30af\u30b7\u30e7\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002</p><p>\u300c*\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001 \u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001\u4e0b\u8a18\u306e\u901a\u308a\u3067\u3059\u3002</p> <ul> <li>customer-gateway-configuration</li> <li>nifty-customer-gateway-name</li> <li>route.destination-cidr-block</li> <li>nifty-vpn-gateway-name</li> <li>nifty-vpn-connection-description</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeVpnConnectionsRequest"
             },
             "name": "DescribeVpnConnections",
             "output": {
                 "shape": "DescribeVpnConnectionsResult"
             }
         },
         "DescribeVpnGateways": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001\u4e0b\u8a18\u306e\u901a\u308a\u3067\u3059\u3002</p> <ul> <li>nifty-vpn-gateway-name</li> <li>nifty-vpn-gateway-description</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DescribeVpnGatewaysRequest"
             },
             "name": "DescribeVpnGateways",
             "output": {
                 "shape": "DescribeVpnGatewaysResult"
             }
         },
         "DetachIsoImage": {
+            "documentation": "<p>ISO\u30a4\u30e1\u30fc\u30b8\u3092\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>ISO\u30a4\u30e1\u30fc\u30b8\u30fb\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u305d\u308c\u305e\u308cISO\u30a4\u30e1\u30fc\u30b8ID\u30fb\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DetachIsoImageRequest"
             },
             "name": "DetachIsoImage",
             "output": {
                 "shape": "DetachIsoImageResult"
             }
         },
         "DetachNetworkInterface": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u306b\u63a5\u7d9a\u3057\u305f\u8ffd\u52a0NIC\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u306e\u89e3\u9664\u306e\u53cd\u6620\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DetachNetworkInterfaceRequest"
             },
             "name": "DetachNetworkInterface",
             "output": {
                 "shape": "DetachNetworkInterfaceResult"
             }
         },
         "DetachVolume": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u3068\u30b5\u30fc\u30d0\u30fc\u306e\u63a5\u7d9a\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30c7\u30a3\u30b9\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u540d\u3092\u6307\u5b9a\u305b\u305a\u306b\u89e3\u9664\u3059\u308b\u3068\u3001\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u306e\u3059\u3079\u3066\u306e\u63a5\u7d9a\u60c5\u5831\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u8d77\u52d5\u4e2d\u306e\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u30c7\u30a3\u30b9\u30af\u3092\u89e3\u9664\u3059\u308b\u5834\u5408\u3001OS\u4e0a\u3067\u5fc5\u305a\u5bfe\u8c61\u30c7\u30a3\u30b9\u30af\u306e\u8a8d\u8b58\u3092\u5916\u3057\u3066\u304b\u3089\u5b9f\u884c\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>OS\u304c\u5bfe\u8c61\u30c7\u30a3\u30b9\u30af\u3092\u8a8d\u8b58\u3057\u305f\u307e\u307e\u89e3\u9664\u3059\u308b\u3068\u3001\u30b5\u30fc\u30d0\u30fc\u304c\u7570\u5e38\u306a\u72b6\u614b\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u306e\u8a8d\u8b58\u3092\u5916\u3059\u306b\u306f\u3001\u4e0b\u8a18\u30da\u30fc\u30b8\u306e\u624b\u9806\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p><p><a href=\"https://docs.nifcloud.com/cp/guide/index.htm#mount\">\u30e6\u30fc\u30b6\u30fc\u30ac\u30a4\u30c9\uff1a\u30c7\u30a3\u30b9\u30af\u306e\u8a8d\u8b58\u3092\u5916\u3059\u8a2d\u5b9a\u65b9\u6cd5\uff08\u30a2\u30f3\u30de\u30a6\u30f3\u30c8\u624b\u9806\uff09\uff1aLinux\u7cfbOS\u306e\u5834\u5408</a></p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DetachVolumeRequest"
             },
             "name": "DetachVolume",
             "output": {
                 "shape": "DetachVolumeResult"
             }
         },
         "DisassociateAddress": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u3092\u89e3\u9664\u3059\u308b\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u3082\u3042\u308a\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u89e3\u9664\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002\u307e\u305f\u3001\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u304c\u6b63\u3057\u304f\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u89e3\u9664\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cipType\u300d\u3082\u3057\u304f\u306fAPI\u300cDescribeAddresses\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceId\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DisassociateAddressRequest"
             },
             "name": "DisassociateAddress",
             "output": {
                 "shape": "DisassociateAddressResult"
             }
         },
         "DisassociateMultiIpAddressGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u306e\u5272\u308a\u5f53\u3066\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3078\u306e\u53cd\u6620\u306b\u306f\u3001\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u518d\u8d77\u52d5\u30aa\u30d7\u30b7\u30e7\u30f3\u3092false\u3067\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u6642\u306e\u307f\u9078\u629e\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DisassociateMultiIpAddressGroupRequest"
             },
             "name": "DisassociateMultiIpAddressGroup",
             "output": {
                 "shape": "DisassociateMultiIpAddressGroupResult"
             }
         },
         "DisassociateRouteTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DisassociateRouteTableRequest"
             },
             "name": "DisassociateRouteTable",
             "output": {
                 "shape": "DisassociateRouteTableResult"
             }
         },
         "DissociateUsers": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u6a5f\u80fd\u304b\u3089\u3001\u6307\u5b9a\u3057\u305f\u30e6\u30fc\u30b6\u30fc\u306e\u5171\u6709\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DissociateUsersRequest"
             },
             "name": "DissociateUsers",
             "output": {
                 "shape": "DissociateUsersResultWrapper"
             }
         },
         "DownloadSslCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u3092\u30c0\u30a6\u30f3\u30ed\u30fc\u30c9\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001SSL\u8a3c\u660e\u66f8\u306e\u30ad\u30fc\u30fbCA\u30fb\u8a3c\u660e\u66f8\u306e\u3044\u305a\u308c\u304b\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\uff08FqdnId\uff09\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305fSSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u72b6\u6cc1\u306b\u3088\u308a\u3001\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30eb\u304c\u30c0\u30a6\u30f3\u30ed\u30fc\u30c9\u3067\u304d\u306a\u3044\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "DownloadSslCertificateRequest"
             },
             "name": "DownloadSslCertificate",
             "output": {
                 "shape": "DownloadSslCertificateResult"
             }
         },
         "ExtendVolumeSize": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u306e\u30b5\u30a4\u30ba\u3092100GB\u62e1\u5f35\u3057\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u306f\u30b5\u30fc\u30d0\u30fc\u306b\u63a5\u7d9a\u3057\u3066\u3044\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u3092\u5b9f\u884c\u3057\u305f\u5f8c\u3001\u30b2\u30b9\u30c8OS\u5074\u3067\u30d5\u30a1\u30a4\u30eb\u30b7\u30b9\u30c6\u30e0\u306e\u62e1\u5f35\u3092\u884c\u3046\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30c7\u30a3\u30b9\u30af\u306e\u30b5\u30a4\u30ba\u3092\u7e2e\u5c0f\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ExtendVolumeSizeRequest"
             },
             "name": "ExtendVolumeSize",
             "output": {
                 "shape": "ExtendVolumeSizeResult"
             }
         },
         "ImportInstance": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fOVF\u30d5\u30a1\u30a4\u30eb\u306e\u60c5\u5831\u306b\u57fa\u3065\u3044\u3066\u3001\u30b5\u30fc\u30d0\u30fc\u30a4\u30f3\u30dd\u30fc\u30c8\u3092\u4e88\u7d04\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u30671\u53f0\u306e\u30b5\u30fc\u30d0\u30fc\u304c\u4e88\u7d04\u53ef\u80fd\u3067\u3059\u3002</p><p>\u30a4\u30e1\u30fc\u30b8\uff08VMDK\u30d5\u30a1\u30a4\u30eb\uff09\u306f\u3001\u5225\u9014\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u9818\u57df\u3078\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u3066\u304f\u3060\u3055\u3044\uff08\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u306b\u542b\u307e\u308c\u308b\u30bf\u30b9\u30afID\u3092\u6307\u5b9a\u3057\u307e\u3059\uff09\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u4f5c\u6210\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30a4\u30f3\u30dd\u30fc\u30c8\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306f\u901a\u5e38\u307b\u304b\u306e\u30b5\u30fc\u30d0\u30fc\u4f5c\u6210\u3068\u540c\u69d8\u306b\u8ab2\u91d1\u3055\u308c\u307e\u3059\u304c\u3001\u30cb\u30d5\u30af\u30e9\u306e\u57fa\u672c\u30c7\u30a3\u30b9\u30af\u5bb9\u91cf\uff08Linux:30GB\u3001Windows:80GB\uff09\u3092\u8d85\u3048\u308b\u30c7\u30a3\u30b9\u30af\u3092\u6301\u3064\u5834\u5408\u306f100GB\u5358\u4f4d\u3067\u8ffd\u52a0\u6599\u91d1\u304c\u767a\u751f\u3057\u307e\u3059\u3002</p><p>\u30a4\u30f3\u30dd\u30fc\u30c8\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306f\u3001API\u304b\u3089\u306e\u524a\u9664\u304c\u53ef\u80fd\u3067\u3059\u3002</p><p>API\u304b\u3089\u306e\u524a\u9664\u3092\u7981\u6b62\u3057\u305f\u3044\u5834\u5408\u306f\u3001\u30a4\u30f3\u30dd\u30fc\u30c8\u5b8c\u4e86\u5f8c\u306bAPI\u300cModifyInstanceAttribute\u300d\u3092\u5b9f\u884c\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ImportInstanceRequest"
             },
             "name": "ImportInstance",
             "output": {
                 "shape": "ImportInstanceResult"
             }
         },
         "ImportKeyPair": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSH\u516c\u958b\u9375\u3092\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u3066\u767b\u9332\u3057\u307e\u3059\u3002SSH\u30ad\u30fc\u540d\u306b\u306f\u3001\u540c\u3058\u30e6\u30fc\u30b6\u30fc\u304c\u4f5c\u308b\u30ad\u30fc\u306e\u3046\u3061\u3001\u4e00\u610f\u3068\u306a\u308b\u6587\u5b57\u5217\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>SSH-RSA\u304a\u3088\u3073SSH-DSA\u306e\u516c\u958b\u9375\u5f62\u5f0f\u306b\u5bfe\u5fdc\u3057\u3066\u3044\u307e\u3059\u3002</p><p>\u63a8\u5968\u3059\u308b\u516c\u958b\u9375\u65b9\u5f0f\u306f\u3000SSH-RSA 2048bit\u9375\u3067\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u305fSSH\u30ad\u30fc\u30da\u30a2\u306e\u30d5\u30a3\u30f3\u30ac\u30fc\u30d7\u30ea\u30f3\u30c8\u304c\u4e00\u81f4\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306e\u78ba\u8a8d\u65b9\u6cd5\u306f\u3001<a href=\"https://docs.nifcloud.com/cp/api/DescribeKeyPairs.htm\">DescribeKeyPairs</a>\u306e\u51e6\u7406\u6982\u8981\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ImportKeyPairRequest"
             },
             "name": "ImportKeyPair",
             "output": {
                 "shape": "ImportKeyPairResult"
             }
         },
         "IncreaseMultiIpAddressCount": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3067\u5229\u7528\u3067\u304d\u308bIP\u30a2\u30c9\u30ec\u30b9\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u4ee5\u4e0b\u306e\u5834\u5408\u3001\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p> <ul> <li>\u51e6\u7406\u4e2d\u306e\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3057\u305f\u3001\u7ba1\u7406\u5916\u306e\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3057\u305f\u306a\u3069\u3001\u7121\u52b9\u306a\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "IncreaseMultiIpAddressCountRequest"
             },
             "name": "IncreaseMultiIpAddressCount",
             "output": {
                 "shape": "IncreaseMultiIpAddressCountResult"
             }
         },
         "ModifyImageAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30a4\u30e1\u30fc\u30b8ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyImageAttributeRequest"
             },
             "name": "ModifyImageAttribute",
             "output": {
                 "shape": "ModifyImageAttributeResult"
             }
         },
         "ModifyInstanceAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30b5\u30fc\u30d0\u30fc\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bf\u30a4\u30d7\u306e\u66f4\u65b0\u306b\u3064\u3044\u3066\u3001\u30db\u30c3\u30c8\u30b9\u30b1\u30fc\u30eb\u30a2\u30c3\u30d7\u304c\u53ef\u80fd\u306a\u30b5\u30fc\u30d0\u30fc\u3067\u3042\u308c\u3070\u3001\u30ea\u30af\u30a8\u30b9\u30c8\u300cNiftyReboot=false\u3001Force=true\u300d\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3067\u3001\u8d77\u52d5\u4e2d\u306e\u72b6\u614b\u306e\u307e\u307e\u3001\u66f4\u65b0\u304c\u53ef\u80fd\u3067\u3059\u3002\u30db\u30c3\u30c8\u30b9\u30b1\u30fc\u30eb\u30a2\u30c3\u30d7\u304c\u53ef\u80fd\u306a\u30b5\u30fc\u30d0\u30fc\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300chotAdd\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002\u305f\u3060\u3057\u30b5\u30fc\u30d0\u30fc\u30bf\u30a4\u30d7\u306e\u5024\u306b\u3088\u3063\u3066\u306f\u3001\u300chotAdd\u300d\u304c\u53ef\u80fd\u3068\u306a\u3063\u3066\u3044\u3066\u3082\u66f4\u65b0\u3067\u304d\u306a\u3044\u30b5\u30fc\u30d0\u30fc\u30bf\u30a4\u30d7\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyInstanceAttributeRequest"
             },
             "name": "ModifyInstanceAttribute",
             "output": {
                 "shape": "ModifyInstanceAttributeResult"
             }
         },
         "ModifyInstanceBackupRuleAttribute": {
+            "documentation": "<p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u5c5e\u6027\u60c5\u5831\u306e\u66f4\u65b0\u3092\u884c\u3044\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u30671\u3064\u306e\u5c5e\u6027\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyInstanceBackupRuleAttributeRequest"
             },
             "name": "ModifyInstanceBackupRuleAttribute",
             "output": {
                 "shape": "ModifyInstanceBackupRuleAttributeResult"
             }
         },
         "ModifyMultiIpAddressGroupAttribute": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u66f4\u65b0\u3092\u884c\u3044\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u30671\u3064\u306e\u5c5e\u6027\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyMultiIpAddressGroupAttributeRequest"
             },
             "name": "ModifyMultiIpAddressGroupAttribute",
             "output": {
                 "shape": "ModifyMultiIpAddressGroupAttributeResult"
             }
         },
         "ModifyNetworkInterfaceAttribute": {
+            "documentation": "<p>\u8ffd\u52a0NIC\u306e\u5c5e\u6027\u60c5\u5831\u306e\u66f4\u65b0\u3092\u884c\u3044\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8ffd\u52a0NIC\u306e1\u3064\u306e\u5c5e\u6027\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u8ffd\u52a0NIC\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u8ffd\u52a0NIC\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30a4\u30f3\u30bf\u30fc\u30d5\u30a7\u30fc\u30b9ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyNetworkInterfaceAttributeRequest"
             },
             "name": "ModifyNetworkInterfaceAttribute",
             "output": {
                 "shape": "ModifyNetworkInterfaceAttributeResult"
             }
         },
         "ModifyRemoteAccessVpnGatewayAttribute": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e1\u3064\u306e\u5c5e\u6027\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyRemoteAccessVpnGatewayAttributeRequest"
             },
             "name": "ModifyRemoteAccessVpnGatewayAttribute",
             "output": {
                 "shape": "ModifyRemoteAccessVpnGatewayAttributeResult"
             }
         },
         "ModifyRemoteAccessVpnGatewayUserAttribute": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u30e6\u30fc\u30b6\u30fc\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002 \u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u304c v1.0.0 \u306e\u5834\u5408\u3001\u5229\u7528\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyRemoteAccessVpnGatewayUserAttributeRequest"
             },
             "name": "ModifyRemoteAccessVpnGatewayUserAttribute",
             "output": {
                 "shape": "ModifyRemoteAccessVpnGatewayUserAttributeResult"
             }
         },
         "ModifySslCertificateAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306eSSL\u8a3c\u660e\u66f8\u306e1\u3064\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\uff08fqdnId\uff09\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifySslCertificateAttributeRequest"
             },
             "name": "ModifySslCertificateAttribute",
             "output": {
                 "shape": "ModifySslCertificateAttributeResult"
             }
         },
         "ModifyVolumeAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30c7\u30a3\u30b9\u30af\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30c7\u30a3\u30b9\u30af\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u5229\u7528\u6599\u91d1\u30bf\u30a4\u30d7\u306e\u66f4\u65b0\u306f\u6b21\u6708\u304b\u3089\u9069\u7528\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ModifyVolumeAttributeRequest"
             },
             "name": "ModifyVolumeAttribute",
             "output": {
                 "shape": "ModifyVolumeAttributeResult"
             }
         },
         "NiftyAssociateImage": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u306b\u5bfe\u3057\u3066\u914d\u5e03\u5148\u8a2d\u5b9a\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u6307\u5b9a\u3057\u305f\u914d\u5e03\u5148\u306e\u5185\u5bb9\u306f\u4e0a\u66f8\u304d\u66f4\u65b0\u3055\u308c\u307e\u3059\u306e\u3067\u3001\u9069\u7528\u3057\u305f\u3044\u3059\u3079\u3066\u306e\u300c\u30cb\u30d5\u30af\u30e9ID\u300d\u3092\u8a2d\u5b9a\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u30a4\u30e1\u30fc\u30b8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30a4\u30e1\u30fc\u30b8ID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>IsRedistribute\u306fisPublic\u3092false\u3067\u6307\u5b9a\u3057\u305f\u3068\u304d\u306e\u307f\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyAssociateImageRequest"
             },
             "name": "NiftyAssociateImage",
             "output": {
                 "shape": "NiftyAssociateImageResult"
             }
         },
         "NiftyAssociateNatTable": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3078NAT\u30c6\u30fc\u30d6\u30eb\u3092\u8a2d\u5b9a\u3059\u308b\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyAssociateNatTableRequest"
             },
             "name": "NiftyAssociateNatTable",
             "output": {
                 "shape": "NiftyAssociateNatTableResult"
             }
         },
         "NiftyAssociateRouteTableWithElasticLoadBalancer": {
+            "documentation": "<p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyAssociateRouteTableWithElasticLoadBalancerRequest"
             },
             "name": "NiftyAssociateRouteTableWithElasticLoadBalancer",
             "output": {
                 "shape": "NiftyAssociateRouteTableWithElasticLoadBalancerResult"
             }
         },
         "NiftyAssociateRouteTableWithVpnGateway": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3078\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u8a2d\u5b9a\u3059\u308b\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002\u307e\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyAssociateRouteTableWithVpnGatewayRequest"
             },
             "name": "NiftyAssociateRouteTableWithVpnGateway",
             "output": {
                 "shape": "NiftyAssociateRouteTableWithVpnGatewayResult"
             }
         },
         "NiftyConfigureElasticLoadBalancerHealthCheck": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u30d1\u30b9\u3001\u304a\u3088\u3073\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u671f\u5f85\u5024\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u30d7\u30ed\u30c8\u30b3\u30eb\u304c\u300cHTTP\u300d\u3082\u3057\u304f\u306f\u300cHTTPS\u300d\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u8a2d\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u5185\u5bb9\u306f\u3001API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeElasticLoadBalancers.htm\">NiftyDescribeElasticLoadBalancers</a>\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u5b9f\u884c\u7d50\u679c\u306f\u3001API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeInstanceElasticLoadBalancerHealth.htm\">NiftyDescribeInstanceElasticLoadBalancerHealth</a>\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyConfigureElasticLoadBalancerHealthCheckRequest"
             },
             "name": "NiftyConfigureElasticLoadBalancerHealthCheck",
             "output": {
                 "shape": "NiftyConfigureElasticLoadBalancerHealthCheckResultWrapper"
             }
         },
         "NiftyCreateAlarm": {
+            "documentation": "<p>\u57fa\u672c\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>FunctionName\u306b\u6a5f\u80fd\u540d\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3067\u30b5\u30fc\u30d0\u30fc\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3001\u30c7\u30a3\u30b9\u30af\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u5bfe\u3057\u3066\u76e3\u8996\u3059\u308b\u30eb\u30fc\u30eb\u3092\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u4ee5\u5916\u306e\u76e3\u8996\u30eb\u30fc\u30eb\u306f\u30be\u30fc\u30f3\u6bce\u306e\u4f5c\u6210\u306b\u306a\u308a\u307e\u3059\u3002\u4f5c\u6210\u3055\u308c\u305f\u30eb\u30fc\u30eb\u306e\u8a2d\u5b9a\u304b\u3089\u30a2\u30e9\u30fc\u30c8\u304c\u4e0a\u304c\u3063\u305f\u5834\u5408\u3001EmailAddress\u306e\u30e1\u30fc\u30eb\u30a2\u30c9\u30ec\u30b9\u306b\u30a2\u30e9\u30fc\u30c8\u30e1\u30fc\u30eb\u304c\u9001\u4fe1\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateAlarmRequest"
             },
             "name": "NiftyCreateAlarm",
             "output": {
                 "shape": "NiftyCreateAlarmResult"
             }
         },
         "NiftyCreateAutoScalingGroup": {
+            "documentation": "<p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u3092\u65b0\u898f\u4f5c\u6210\u3059\u308b\u306b\u306f\u3001\u81ea\u8eab\u3067\u4f5c\u6210\u3057\u305f\u30a4\u30e1\u30fc\u30b8\uff08\u8ffd\u52a0\u30c7\u30a3\u30b9\u30af\u306a\u3057\uff09\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u6307\u5b9a\u3057\u305f\u30a4\u30e1\u30fc\u30b8\u304c\u5b58\u5728\u3059\u308b\u30be\u30fc\u30f3\u306b\u5bfe\u3057\u3066\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateAutoScalingGroupRequest"
             },
             "name": "NiftyCreateAutoScalingGroup",
             "output": {
                 "shape": "NiftyCreateAutoScalingGroupResult"
             }
         },
         "NiftyCreateDhcpConfig": {
+            "documentation": "<p>DHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateDhcpConfigRequest"
             },
             "name": "NiftyCreateDhcpConfig",
             "output": {
                 "shape": "NiftyCreateDhcpConfigResult"
             }
         },
         "NiftyCreateDhcpIpAddressPool": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u306b\u3001\u81ea\u52d5\u5272\u308a\u5f53\u3066IP\u30a2\u30c9\u30ec\u30b9\u306e\u8a2d\u5b9a\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateDhcpIpAddressPoolRequest"
             },
             "name": "NiftyCreateDhcpIpAddressPool",
             "output": {
                 "shape": "NiftyCreateDhcpIpAddressPoolResult"
             }
         },
         "NiftyCreateDhcpStaticMapping": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u306b\u3001\u624b\u52d5\u5272\u308a\u5f53\u3066IP\u30a2\u30c9\u30ec\u30b9\u306e\u8a2d\u5b9a\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateDhcpStaticMappingRequest"
             },
             "name": "NiftyCreateDhcpStaticMapping",
             "output": {
                 "shape": "NiftyCreateDhcpStaticMappingResult"
             }
         },
         "NiftyCreateElasticLoadBalancer": {
+            "documentation": "<p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30dd\u30fc\u30c8\u5b9a\u7fa9\u3092\u4f5c\u6210\u3067\u304d\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u4f5c\u6210\u5f8c\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u8ffd\u52a0\u3059\u308b\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyRegisterInstancesWithElasticLoadBalancer.htm\">NiftyRegisterInstancesWithElasticLoadBalancer</a>\u300d\uff08\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\uff09</li> </ul> <p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3067SSL\u30a2\u30af\u30bb\u30e9\u30ec\u30fc\u30bf\u30fc\u8a2d\u5b9a\u3092\u3059\u308b\u5834\u5408\u306f\u3001\u30d7\u30ed\u30c8\u30b3\u30eb\u300cHTTPS\u300d\u3068SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\u3092\u6307\u5b9a\u3057\u3066\u4f5c\u6210\u3057\u3066\u304f\u3060\u3055\u3044\u3002SSL\u30a2\u30af\u30bb\u30e9\u30ec\u30fc\u30bf\u30fc\u8a2d\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u30d7\u30ed\u30c8\u30b3\u30eb\u300cTCP\u300d\u3067\u5fc5\u8981\u30dd\u30fc\u30c8\u3092\u6307\u5b9a\u3057\u3066\u4f5c\u6210\u3057\u3066\u3044\u305f\u3060\u304f\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306e\u8a2d\u5b9a\u3067\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u30d1\u30b9\u3001\u304a\u3088\u3073\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u671f\u5f85\u5024\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u30d7\u30ed\u30c8\u30b3\u30eb\u304c\u300cHTTP\u300d\u3082\u3057\u304f\u306f\u300cHTTPS\u300d\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u5185\u5bb9\u306f\u3001API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeElasticLoadBalancers.htm\">NiftyDescribeElasticLoadBalancers</a>\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateElasticLoadBalancerRequest"
             },
             "name": "NiftyCreateElasticLoadBalancer",
             "output": {
                 "shape": "NiftyCreateElasticLoadBalancerResultWrapper"
             }
         },
         "NiftyCreateInstanceSnapshot": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u306b\u5bfe\u3057\u3066\u3001\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u4f5c\u6210\u306b\u306f\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateInstanceSnapshotRequest"
             },
             "name": "NiftyCreateInstanceSnapshot",
             "output": {
                 "shape": "NiftyCreateInstanceSnapshotResult"
             }
         },
         "NiftyCreateNatRule": {
+            "documentation": "<p>NAT\u30c6\u30fc\u30d6\u30eb\u306b\u9069\u7528\u3059\u308bNAT\u30eb\u30fc\u30eb\u60c5\u5831\u3092\u4f5c\u6210\u3059\u308b\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateNatRuleRequest"
             },
             "name": "NiftyCreateNatRule",
             "output": {
                 "shape": "NiftyCreateNatRuleResult"
             }
         },
         "NiftyCreateNatTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3059\u308bNAT\u30c6\u30fc\u30d6\u30eb\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateNatTableRequest"
             },
             "name": "NiftyCreateNatTable",
             "output": {
                 "shape": "NiftyCreateNatTableResult"
             }
         },
         "NiftyCreatePrivateLan": {
+            "documentation": "<p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreatePrivateLanRequest"
             },
             "name": "NiftyCreatePrivateLan",
             "output": {
                 "shape": "NiftyCreatePrivateLanResult"
             }
         },
         "NiftyCreateRouter": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u306b\u5272\u308a\u5f53\u3066\u308b\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30cd\u30c3\u30c8\u30ef\u30fc\u30afID\u307e\u305f\u306f\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u306e\u30be\u30fc\u30f3\u306f\u6307\u5b9a\u3057\u305f\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3068\u540c\u4e00\u306e\u30be\u30fc\u30f3\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateRouterRequest"
             },
             "name": "NiftyCreateRouter",
             "output": {
                 "shape": "NiftyCreateRouterResult"
             }
         },
         "NiftyCreateSeparateInstanceRule": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u4f5c\u6210\u3059\u308b\u969b\u306b\u306f\u3001\u30be\u30fc\u30f3\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30011\u3064\u306e\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306b\u9069\u7528\u53ef\u80fd\u306a\u30b5\u30fc\u30d0\u30fc\u306e\u4e0a\u9650\u6570\u306f\u30012\u53f0\u3068\u306a\u308a\u307e\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u4f5c\u6210\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002<br> API\u300cNiftyDescribeSeparateInstanceRules\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cseparateInstanceRuleStatus\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u540d\u3068\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u4e21\u65b9\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u512a\u5148\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateSeparateInstanceRuleRequest"
             },
             "name": "NiftyCreateSeparateInstanceRule",
             "output": {
                 "shape": "NiftyCreateSeparateInstanceRuleResult"
             }
         },
         "NiftyCreateWebProxy": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u306b\u5bfe\u3057\u3066Web\u30d7\u30ed\u30ad\u30b7\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u53d7\u3051\u5074\uff0f\u8fc2\u56de\u5148\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u3068\u7d10\u4ed8\u304d\u306e\u3042\u308b\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3092\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyCreateWebProxyRequest"
             },
             "name": "NiftyCreateWebProxy",
             "output": {
                 "shape": "NiftyCreateWebProxyResult"
             }
         },
         "NiftyDeleteAlarm": {
+            "documentation": "<p>\u57fa\u672c\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u76e3\u8996\u30eb\u30fc\u30eb\u540d\u304a\u3088\u3073\u6a5f\u80fd\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteAlarmRequest"
             },
             "name": "NiftyDeleteAlarm",
             "output": {
                 "shape": "NiftyDeleteAlarmResult"
             }
         },
         "NiftyDeleteAutoScalingGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u306e\u5b9a\u7fa9\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u3092\u524a\u9664\u3059\u308b\u3068\u3001\u4f5c\u6210\u3055\u308c\u305f\u30b9\u30b1\u30fc\u30eb\u30a2\u30a6\u30c8\u30b5\u30fc\u30d0\u30fc\u3082\u524a\u9664\u3055\u308c\u307e\u3059\u3002\u30b9\u30b1\u30fc\u30eb\u30a2\u30a6\u30c8\u30b5\u30fc\u30d0\u30fc\u304c\u5b58\u5728\u3059\u308b\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u524a\u9664\u3059\u308b\u5834\u5408\u3001\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u524a\u9664\u304c\u5b8c\u4e86\u3059\u308b\u307e\u3067\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteAutoScalingGroupRequest"
             },
             "name": "NiftyDeleteAutoScalingGroup",
             "output": {
                 "shape": "NiftyDeleteAutoScalingGroupResult"
             }
         },
         "NiftyDeleteDhcpConfig": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteDhcpConfigRequest"
             },
             "name": "NiftyDeleteDhcpConfig",
             "output": {
                 "shape": "NiftyDeleteDhcpConfigResult"
             }
         },
         "NiftyDeleteDhcpIpAddressPool": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u304b\u3089\u3001\u81ea\u52d5\u5272\u308a\u5f53\u3066IP\u30a2\u30c9\u30ec\u30b9\u306e\u8a2d\u5b9a\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteDhcpIpAddressPoolRequest"
             },
             "name": "NiftyDeleteDhcpIpAddressPool",
             "output": {
                 "shape": "NiftyDeleteDhcpIpAddressPoolResult"
             }
         },
         "NiftyDeleteDhcpStaticMapping": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u304b\u3089\u3001\u624b\u52d5\u5272\u308a\u5f53\u3066IP\u30a2\u30c9\u30ec\u30b9\u306e\u8a2d\u5b9a\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteDhcpStaticMappingRequest"
             },
             "name": "NiftyDeleteDhcpStaticMapping",
             "output": {
                 "shape": "NiftyDeleteDhcpStaticMappingResult"
             }
         },
         "NiftyDeleteElasticLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30dd\u30fc\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u95a2\u9023\u3059\u308b\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\u30fb\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u8a2d\u5b9a\u306a\u3069\u3082\u3042\u308f\u305b\u3066\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteElasticLoadBalancerRequest"
             },
             "name": "NiftyDeleteElasticLoadBalancer",
             "output": {
                 "shape": "NiftyDeleteElasticLoadBalancerResultWrapper"
             }
         },
         "NiftyDeleteInstanceSnapshot": {
+            "documentation": "<p>\u4f5c\u6210\u6e08\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u524a\u9664\u3059\u308b\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8ID\u3082\u3057\u304f\u306f\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u540d\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u53d6\u5f97\u5f8c\u306b\u767a\u751f\u3057\u305f\u5dee\u5206\u3092\u30de\u30fc\u30b8\u3059\u308b\u305f\u3081\u3001\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u524a\u9664\u306b\u306f\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u524a\u9664\u51e6\u7406\u72b6\u6cc1\u306f\u3001API\u300cNiftyDescribeInstanceSnapshots\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteInstanceSnapshotRequest"
             },
             "name": "NiftyDeleteInstanceSnapshot",
             "output": {
                 "shape": "NiftyDeleteInstanceSnapshotResult"
             }
         },
         "NiftyDeleteNatRule": {
+            "documentation": "<p>NAT\u30c6\u30fc\u30d6\u30eb\u306b\u9069\u7528\u3055\u308c\u305fNAT\u30eb\u30fc\u30eb\u60c5\u5831\u3092\u524a\u9664\u3059\u308b\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteNatRuleRequest"
             },
             "name": "NiftyDeleteNatRule",
             "output": {
                 "shape": "NiftyDeleteNatRuleResult"
             }
         },
         "NiftyDeleteNatTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3059\u308bNAT\u30c6\u30fc\u30d6\u30eb\u306e\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteNatTableRequest"
             },
             "name": "NiftyDeleteNatTable",
             "output": {
                 "shape": "NiftyDeleteNatTableResult"
             }
         },
         "NiftyDeletePrivateLan": {
+            "documentation": "<p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306e\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeletePrivateLanRequest"
             },
             "name": "NiftyDeletePrivateLan",
             "output": {
                 "shape": "NiftyDeletePrivateLanResult"
             }
         },
         "NiftyDeleteRouter": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteRouterRequest"
             },
             "name": "NiftyDeleteRouter",
             "output": {
                 "shape": "NiftyDeleteRouterResult"
             }
         },
         "NiftyDeleteSeparateInstanceRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u524a\u9664\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeSeparateInstanceRules.htm\">NiftyDescribeSeparateInstanceRules</a>\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cseparateInstanceRuleStatus\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteSeparateInstanceRuleRequest"
             },
             "name": "NiftyDeleteSeparateInstanceRule",
             "output": {
                 "shape": "NiftyDeleteSeparateInstanceRuleResult"
             }
         },
         "NiftyDeleteWebProxy": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305fWeb\u30d7\u30ed\u30ad\u30b7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeleteWebProxyRequest"
             },
             "name": "NiftyDeleteWebProxy",
             "output": {
                 "shape": "NiftyDeleteWebProxyResult"
             }
         },
         "NiftyDeregisterInstancesFromElasticLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304b\u3089\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002\u307e\u305f\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeregisterInstancesFromElasticLoadBalancerRequest"
             },
             "name": "NiftyDeregisterInstancesFromElasticLoadBalancer",
             "output": {
                 "shape": "NiftyDeregisterInstancesFromElasticLoadBalancerResultWrapper"
             }
         },
         "NiftyDeregisterInstancesFromSeparateInstanceRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u304b\u3089\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u306f\u305a\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeregisterInstancesFromSeparateInstanceRuleRequest"
             },
             "name": "NiftyDeregisterInstancesFromSeparateInstanceRule",
             "output": {
                 "shape": "NiftyDeregisterInstancesFromSeparateInstanceRuleResult"
             }
         },
         "NiftyDeregisterRoutersFromSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u30eb\u30fc\u30bf\u30fc\u3092\u306f\u305a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306f\u305a\u3059\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u540d\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u30eb\u30fc\u30bf\u30fc\u3092\u306f\u305a\u3059\u51e6\u7406\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeregisterRoutersFromSecurityGroupRequest"
             },
             "name": "NiftyDeregisterRoutersFromSecurityGroup",
             "output": {
                 "shape": "NiftyDeregisterRoutersFromSecurityGroupResult"
             }
         },
         "NiftyDeregisterVpnGatewaysFromSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u306f\u305a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u304b\u3089\u306f\u305a\u3059\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4ID\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u306f\u305a\u3059\u51e6\u7406\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDeregisterVpnGatewaysFromSecurityGroupRequest"
             },
             "name": "NiftyDeregisterVpnGatewaysFromSecurityGroup",
             "output": {
                 "shape": "NiftyDeregisterVpnGatewaysFromSecurityGroupResult"
             }
         },
         "NiftyDescribeAlarmHistory": {
+            "documentation": "<p>\u30a2\u30e9\u30fc\u30c8\u5c65\u6b74\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ea\u30fc\u30b8\u30e7\u30f3/\u30be\u30fc\u30f3/\u30bb\u30eb\u306b\u5229\u7528\u5236\u9650\u304c\u304b\u304b\u3063\u3066\u3044\u308b\u76e3\u8996\u30eb\u30fc\u30eb\u306e\u30a2\u30e9\u30fc\u30e0\u5c65\u6b74\u306f\u8fd4\u5374\u3055\u308c\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeAlarmHistoryRequest"
             },
             "name": "NiftyDescribeAlarmHistory",
             "output": {
                 "shape": "NiftyDescribeAlarmHistoryResult"
             }
         },
         "NiftyDescribeAlarmRulesActivities": {
+            "documentation": "<p>\u76e3\u8996\u30eb\u30fc\u30eb\u306e\u76e3\u8996\u9805\u76ee\u6bce\u306b\u3001\u30ea\u30bd\u30fc\u30b9\u7570\u5e38\u767a\u751f\u3068\u89e3\u9664\u306e\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ea\u30fc\u30b8\u30e7\u30f3/\u30be\u30fc\u30f3/\u30bb\u30eb\u306b\u5229\u7528\u5236\u9650\u304c\u304b\u304b\u3063\u3066\u3044\u308b\u76e3\u8996\u30eb\u30fc\u30eb\u30ed\u30b0\u60c5\u5831\u306f\u8fd4\u5374\u3057\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeAlarmRulesActivitiesRequest"
             },
             "name": "NiftyDescribeAlarmRulesActivities",
             "output": {
                 "shape": "NiftyDescribeAlarmRulesActivitiesResult"
             }
         },
         "NiftyDescribeAlarms": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u57fa\u672c\u76e3\u8996\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u76e3\u8996\u30eb\u30fc\u30eb\u540d\u304a\u3088\u3073\u6a5f\u80fd\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u76e3\u8996\u30eb\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeAlarmsRequest"
             },
             "name": "NiftyDescribeAlarms",
             "output": {
                 "shape": "NiftyDescribeAlarmsResult"
             }
         },
         "NiftyDescribeAlarmsPartitions": {
+            "documentation": "<p>\u76e3\u8996\u30eb\u30fc\u30eb\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u304c\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u3001\u6307\u5b9a\u3055\u308c\u305f\u30b5\u30fc\u30d0\u30fc\u304c\u5272\u308a\u5f53\u3066\u3089\u308c\u3066\u3044\u308b\u76e3\u8996\u30eb\u30fc\u30eb\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u60c5\u5831\u306e\u307f\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u3059\u3079\u3066\u306e\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u3092\u76e3\u8996\u5bfe\u8c61\u306b\u3057\u305f\u5834\u5408\u3001\u5f53API\u3067\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u60c5\u5831\u304c\u53d6\u5f97\u3055\u308c\u308b\u3088\u3046\u306b\u306a\u308b\u307e\u3067\u3001\u6700\u5927\u306710\u5206\u304b\u304b\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeAlarmsPartitionsRequest"
             },
             "name": "NiftyDescribeAlarmsPartitions",
             "output": {
                 "shape": "NiftyDescribeAlarmsPartitionsResult"
             }
         },
         "NiftyDescribeAutoScalingGroups": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u306e\u5b9a\u7fa9\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u306e\u5b9a\u7fa9\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeAutoScalingGroupsRequest"
             },
             "name": "NiftyDescribeAutoScalingGroups",
             "output": {
                 "shape": "NiftyDescribeAutoScalingGroupsResult"
             }
         },
         "NiftyDescribeCorporateInfoForCertificate": {
+            "documentation": "<p>\u767b\u9332\u3055\u308c\u3066\u3044\u308b\u7533\u8acb\u6cd5\u4eba\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7533\u8acb\u6cd5\u4eba\u60c5\u5831\u304c\u672a\u767b\u9332\u306e\u5834\u5408\u306f\u3001\u7a7a\u306e\u60c5\u5831\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeCorporateInfoForCertificateRequest"
             },
             "name": "NiftyDescribeCorporateInfoForCertificate",
             "output": {
                 "shape": "NiftyDescribeCorporateInfoForCertificateResult"
             }
         },
         "NiftyDescribeDhcpConfigs": {
+            "documentation": "<p>DHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>DHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001DHCP\u30b3\u30f3\u30d5\u30a3\u30b0ID\u304c\u5fc5\u8981\u3067\u3059\u3002DHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eDHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002</p><p>\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\\\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001ipaddress-pool-start, ipaddress-pool-stop, ipaddress-pool-description, static-mapping-ipaddress, static-mapping-macaddress, static-mapping-description\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeDhcpConfigsRequest"
             },
             "name": "NiftyDescribeDhcpConfigs",
             "output": {
                 "shape": "NiftyDescribeDhcpConfigsResult"
             }
         },
         "NiftyDescribeDhcpStatus": {
+            "documentation": "<p>DHCP\u3067\u306eIP\u6255\u3044\u51fa\u3057\u72b6\u614b\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeDhcpStatusRequest"
             },
             "name": "NiftyDescribeDhcpStatus",
             "output": {
                 "shape": "NiftyDescribeDhcpStatusResult"
             }
         },
         "NiftyDescribeElasticLoadBalancers": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306e\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeElasticLoadBalancersRequest"
             },
             "name": "NiftyDescribeElasticLoadBalancers",
             "output": {
                 "shape": "NiftyDescribeElasticLoadBalancersResultWrapper"
             }
         },
         "NiftyDescribeInstanceElasticLoadBalancerHealth": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u3001\u30b5\u30fc\u30d0\u30fc\u306e\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u7d50\u679c\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u306f\u3001API \u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyConfigureElasticLoadBalancerHealthCheck.htm\">NiftyConfigureElasticLoadBalancerHealthCheck</a>\u300d\u3067\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u5bfe\u8c61\u3068\u3057\u3066\u3001\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u7d50\u679c\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeInstanceElasticLoadBalancerHealthRequest"
             },
             "name": "NiftyDescribeInstanceElasticLoadBalancerHealth",
             "output": {
                 "shape": "NiftyDescribeInstanceElasticLoadBalancerHealthResultWrapper"
             }
         },
         "NiftyDescribeInstanceSnapshots": {
+            "documentation": "<p>\u4f5c\u6210\u6e08\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeInstanceSnapshotsRequest"
             },
             "name": "NiftyDescribeInstanceSnapshots",
             "output": {
                 "shape": "NiftyDescribeInstanceSnapshotsResult"
             }
         },
         "NiftyDescribeLoadBalancerSSLPolicies": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u5bfe\u3057\u3066\u9069\u7528\u53ef\u80fd\u306aSSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u306e\u30c6\u30f3\u30d7\u30ec\u30fc\u30c8\u4e00\u89a7\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeLoadBalancerSSLPoliciesRequest"
             },
             "name": "NiftyDescribeLoadBalancerSSLPolicies",
             "output": {
                 "shape": "NiftyDescribeLoadBalancerSSLPoliciesResultWrapper"
             }
         },
         "NiftyDescribeNatTables": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fNAT\u30c6\u30fc\u30d6\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u3059\u3079\u3066\u306eNAT\u30c6\u30fc\u30d6\u30eb\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002</p><p>\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001 \u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001\u4e0b\u8a18\u306e\u901a\u308a\u3067\u3059\u3002</p> <ul> <li>nat-rule.description</li> <li>nat-rule.destination.address</li> <li>nat-rule.source.address</li> <li>nat-rule.translation.address</li> <li>nt-rule.outbound-interface.network-name</li> <li>nat-rule.inbound-interface.network-name</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeNatTablesRequest"
             },
             "name": "NiftyDescribeNatTables",
             "output": {
                 "shape": "NiftyDescribeNatTablesResult"
             }
         },
         "NiftyDescribePerformanceChart": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u3001\u30c7\u30a3\u30b9\u30af\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u7a3c\u50cd\u72b6\u6cc1\u3092\u8868\u793a\u3057\u305f\u30c1\u30e3\u30fc\u30c8\u306e\u30c7\u30fc\u30bf\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u5bfe\u8c61\u30b5\u30fc\u30d0\u30fc\u304c\u505c\u6b62\u3055\u308c\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3055\u308c\u307e\u305b\u3093\u3002<br> \u30fbCPU\u4f7f\u7528\u7387<br> \u30fb\u30e1\u30e2\u30ea\u4f7f\u7528\u7387<br> \u30fb\u30c7\u30a3\u30b9\u30af\u4f7f\u7528\u7387<br> \u30fb\u30c7\u30a3\u30b9\u30af\u30d1\u30fc\u30c6\u30a3\u30b7\u30e7\u30f3\u4f7f\u7528\u7387</p><p>\u30c1\u30e3\u30fc\u30c8\u51fa\u529b\u3092\u671f\u9593\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u6700\u65b024\u6642\u9593\u306e10\u5206\u9593\u9694\u306e\u30c7\u30fc\u30bf\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p><p>\u30c1\u30e3\u30fc\u30c8\u51fa\u529b\u3092\u671f\u9593\u6307\u5b9a\u3059\u308b\u5834\u5408\u3001\u671f\u9593\u304c7\u65e5\u9593\u307e\u3067\u306a\u308930\u5206\u9593\u9694\u306e\u30c7\u30fc\u30bf\u3001\u305d\u308c\u4ee5\u964d\u306f1\u65e5\u9593\u9694\u306e\u30c7\u30fc\u30bf\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p><p>\u6307\u5b9a\u53ef\u80fd\u306a\u958b\u59cb\u65e5\u306f\u3001\u5f53\u6708\u304b\u3089\uff15\u30ab\u6708\u524d\u306e\u6708\u521d\u65e5\u307e\u3067\u6307\u5b9a\u53ef\u80fd\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u4f8b. 2020/08/11 \u306e\u5834\u5408\u3001 2020/03/01 \u3092\u958b\u59cb\u65e5\u3068\u3057\u3066\u6307\u5b9a\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribePerformanceChartRequest"
             },
             "name": "NiftyDescribePerformanceChart",
             "output": {
                 "shape": "NiftyDescribePerformanceChartResult"
             }
         },
         "NiftyDescribePrivateLans": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217nifty\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217nifty?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001private-lan-name\u3001description\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribePrivateLansRequest"
             },
             "name": "NiftyDescribePrivateLans",
             "output": {
                 "shape": "NiftyDescribePrivateLansResult"
             }
         },
         "NiftyDescribeRouters": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u306e\u60c5\u5831\u306e\u53d6\u5f97\u3092\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30eb\u30fc\u30bf\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0 \u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001\u300c?\u300d\u306f1 \u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u00a5\u2217niftycloud\u00a5?\u00a5\u00a5 \u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u3001router-name\u3001description \u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeRoutersRequest"
             },
             "name": "NiftyDescribeRouters",
             "output": {
                 "shape": "NiftyDescribeRoutersResult"
             }
         },
         "NiftyDescribeScalingActivities": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u306e\u30ed\u30b0\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u306e\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeScalingActivitiesRequest"
             },
             "name": "NiftyDescribeScalingActivities",
             "output": {
                 "shape": "NiftyDescribeScalingActivitiesResult"
             }
         },
         "NiftyDescribeSeparateInstanceRules": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u306f\u3001\u53d6\u5f97\u53ef\u80fd\u306a\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeSeparateInstanceRulesRequest"
             },
             "name": "NiftyDescribeSeparateInstanceRules",
             "output": {
                 "shape": "NiftyDescribeSeparateInstanceRulesResult"
             }
         },
         "NiftyDescribeVpnGatewayActivities": {
+            "documentation": "<p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u63a5\u7d9a\u30ed\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u63a5\u7d9a\u30ed\u30b0\u306e\u30a8\u30e9\u30fc\u306b\u3064\u3044\u3066\u306f\u3001\u8a72\u5f53\u7b87\u6240\u306e\u884c\u6570\u3068\u30a8\u30e9\u30fc\u30b3\u30fc\u30c9\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4ID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeVpnGatewayActivitiesRequest"
             },
             "name": "NiftyDescribeVpnGatewayActivities",
             "output": {
                 "shape": "NiftyDescribeVpnGatewayActivitiesResult"
             }
         },
         "NiftyDescribeWebProxies": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308bWeb\u30d7\u30ed\u30ad\u30b7\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u53d6\u5f97\u3067\u304d\u308b\u3059\u3079\u3066\u306e\u30eb\u30fc\u30bf\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u306e\u5024\u300cFilter.n.Value.m\u300d\u3092\u6307\u5b9a\u3059\u308b\u969b\u3001\u30ef\u30a4\u30eb\u30c9\u30ab\u30fc\u30c9\u6587\u5b57\uff08\u66d6\u6627\u691c\u7d22\uff09\u6307\u5b9a\u53ef\u80fd\u3067\u3059\u3002\u300c\u2217\u300d\u306f0\u500b\u4ee5\u4e0a\u4efb\u610f\u6587\u5b57\u3001 \u300c?\u300d\u306f1\u500b\u4efb\u610f\u6587\u5b57\u3001\u300c\u00a5\u300d\u306f\u30a8\u30b9\u30b1\u30fc\u30d7\u5909\u63db\u6587\u5b57\uff08\u300c\u2217niftycloud\u00a5?\u00a5\u00a5\u300d\u306f\u300c\u2217niftycloud?\u00a5\u300d\u3092\u691c\u7d22\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u66d6\u6627\u691c\u7d22\u304c\u6307\u5b9a\u53ef\u80fd\u306a\u7d5e\u308a\u8fbc\u307f\u6761\u4ef6\u306e\u9805\u76ee\u540d\u306f\u3001\u4e0b\u8a18\u306e\u901a\u308a\u3067\u3059\u3002</p> <ul> <li>router-name</li> <li>listen-network-name</li> <li>listen-port</li> <li>proxy-bypass-network-name</li> <li>option-name-server</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDescribeWebProxiesRequest"
             },
             "name": "NiftyDescribeWebProxies",
             "output": {
                 "shape": "NiftyDescribeWebProxiesResult"
             }
         },
         "NiftyDisableDhcp": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306b\u5bfe\u3057\u3066DHCP\u6a5f\u80fd\u3092\u7121\u52b9\u5316\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDisableDhcpRequest"
             },
             "name": "NiftyDisableDhcp",
             "output": {
                 "shape": "NiftyDisableDhcpResult"
             }
         },
         "NiftyDisassociateNatTable": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305fNAT\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDisassociateNatTableRequest"
             },
             "name": "NiftyDisassociateNatTable",
             "output": {
                 "shape": "NiftyDisassociateNatTableResult"
             }
         },
         "NiftyDisassociateRouteTableFromElasticLoadBalancer": {
+            "documentation": "<p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304b\u3089\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u8a2d\u5b9a\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDisassociateRouteTableFromElasticLoadBalancerRequest"
             },
             "name": "NiftyDisassociateRouteTableFromElasticLoadBalancer",
             "output": {
                 "shape": "NiftyDisassociateRouteTableFromElasticLoadBalancerResult"
             }
         },
         "NiftyDisassociateRouteTableFromVpnGateway": {
+            "documentation": "<p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyDisassociateRouteTableFromVpnGatewayRequest"
             },
             "name": "NiftyDisassociateRouteTableFromVpnGateway",
             "output": {
                 "shape": "NiftyDisassociateRouteTableFromVpnGatewayResult"
             }
         },
         "NiftyEnableDhcp": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306b\u5bfe\u3057\u3066\u3001DHCP\u6a5f\u80fd\u3092\u6709\u52b9\u5316\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyEnableDhcpRequest"
             },
             "name": "NiftyEnableDhcp",
             "output": {
                 "shape": "NiftyEnableDhcpResult"
             }
         },
         "NiftyModifyAddressAttribute": {
+            "documentation": "<p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u57fa\u672c\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyAddressAttributeRequest"
             },
             "name": "NiftyModifyAddressAttribute",
             "output": {
                 "shape": "NiftyModifyAddressAttributeResult"
             }
         },
         "NiftyModifyCustomerGatewayAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305f\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u30671\u3064\u306e\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30ab\u30b9\u30bf\u30de\u30fc\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30e1\u30e2\u306e\u5909\u66f4\u306b\u304a\u3044\u3066\u3001\u66f4\u65b0\u5024\u306b\u4f55\u3082\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u7a7a\u306e\u60c5\u5831\u3067\u66f4\u65b0\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyCustomerGatewayAttributeRequest"
             },
             "name": "NiftyModifyCustomerGatewayAttribute",
             "output": {
                 "shape": "NiftyModifyCustomerGatewayAttributeResult"
             }
         },
         "NiftyModifyElasticLoadBalancerAttributes": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>Sorry\u30da\u30fc\u30b8\u30aa\u30d7\u30b7\u30e7\u30f3\u306f\u3001\u30d7\u30ed\u30c8\u30b3\u30eb\u300cHTTP\u300d\u307e\u305f\u306f\u300cHTTPS\u300d\u306e\u5834\u5408\u306b\u5229\u7528\u304c\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyElasticLoadBalancerAttributesRequest"
             },
             "name": "NiftyModifyElasticLoadBalancerAttributes",
             "output": {
                 "shape": "NiftyModifyElasticLoadBalancerAttributesResult"
             }
         },
         "NiftyModifyInstanceSnapshotAttribute": {
+            "documentation": "<p>\u4f5c\u6210\u6e08\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306b\u5bfe\u3059\u308b\u30e1\u30e2\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u30e1\u30e2\u3092\u66f4\u65b0\u3059\u308b\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8ID\u307e\u305f\u306f\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u540d\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyInstanceSnapshotAttributeRequest"
             },
             "name": "NiftyModifyInstanceSnapshotAttribute",
             "output": {
                 "shape": "NiftyModifyInstanceSnapshotAttributeResult"
             }
         },
         "NiftyModifyKeyPairAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSH\u30ad\u30fc\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>SSH\u30ad\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSH\u30ad\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyKeyPairAttributeRequest"
             },
             "name": "NiftyModifyKeyPairAttribute",
             "output": {
                 "shape": "NiftyModifyKeyPairAttributeResult"
             }
         },
         "NiftyModifyPrivateLanAttribute": {
+            "documentation": "<p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306e\u57fa\u672c\u60c5\u5831\u306e\u5909\u66f4\u3092\u884c\u3044\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyPrivateLanAttributeRequest"
             },
             "name": "NiftyModifyPrivateLanAttribute",
             "output": {
                 "shape": "NiftyModifyPrivateLanAttributeResult"
             }
         },
         "NiftyModifyRouterAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30eb\u30fc\u30bf\u30fc\u30b5\u30fc\u30d0\u30fc\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u540d\u3082\u3057\u304f\u306f\u30eb\u30fc\u30bf\u30fc\u30bf\u30a4\u30d7\u3092\u66f4\u65b0\u6642\u3001\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyRouterAttributeRequest"
             },
             "name": "NiftyModifyRouterAttribute",
             "output": {
                 "shape": "NiftyModifyRouterAttributeResult"
             }
         },
         "NiftyModifyVpnGatewayAttribute": {
+            "documentation": "<p>\u6307\u5b9a\u3055\u308c\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4ID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30bf\u30a4\u30d7\u306e\u66f4\u65b0\u6642\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyVpnGatewayAttributeRequest"
             },
             "name": "NiftyModifyVpnGatewayAttribute",
             "output": {
                 "shape": "NiftyModifyVpnGatewayAttributeResult"
             }
         },
         "NiftyModifyWebProxyAttribute": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305fWeb\u30d7\u30ed\u30ad\u30b7\u306e\u8a73\u7d30\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306eWeb\u30d7\u30ed\u30ad\u30b7\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u53d7\u3051\u5074\uff0f\u8fc2\u56de\u5148\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u3068\u7d10\u4ed8\u304d\u306e\u3042\u308b\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3092\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u53d7\u3051\u5074\uff0f\u8fc2\u56de\u5148\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3001\u53d7\u3051\u5074\u30dd\u30fc\u30c8\u3001DNS\u30b5\u30fc\u30d0\u30fc\u306e\u30a2\u30c9\u30ec\u30b9\u306e\u66f4\u65b0\u6642\u3001\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyModifyWebProxyAttributeRequest"
             },
             "name": "NiftyModifyWebProxyAttribute",
             "output": {
                 "shape": "NiftyModifyWebProxyAttributeResult"
             }
         },
         "NiftyRebootRouters": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3092\u518d\u8d77\u52d5\u3092\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID \u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u306e\u518d\u8d77\u52d5\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u30eb\u30fc\u30bf\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u3001API\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cstate\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRebootRoutersRequest"
             },
             "name": "NiftyRebootRouters",
             "output": {
                 "shape": "NiftyRebootRoutersResult"
             }
         },
         "NiftyRebootVpnGateways": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u518d\u8d77\u52d5\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u518d\u8d77\u52d5\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u3001API\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cstate\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRebootVpnGatewaysRequest"
             },
             "name": "NiftyRebootVpnGateways",
             "output": {
                 "shape": "NiftyRebootVpnGatewaysResult"
             }
         },
         "NiftyRegisterInstancesWithElasticLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30b5\u30fc\u30d0\u30fc\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRegisterInstancesWithElasticLoadBalancerRequest"
             },
             "name": "NiftyRegisterInstancesWithElasticLoadBalancer",
             "output": {
                 "shape": "NiftyRegisterInstancesWithElasticLoadBalancerResultWrapper"
             }
         },
         "NiftyRegisterInstancesWithSeparateInstanceRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3078\u9069\u7528\u3057\u307e\u3059\u30021\u3064\u306e\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306b\u9069\u7528\u53ef\u80fd\u306a\u30b5\u30fc\u30d0\u30fc\u306e\u4e0a\u9650\u6570\u306f\u30012\u53f0\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRegisterInstancesWithSeparateInstanceRuleRequest"
             },
             "name": "NiftyRegisterInstancesWithSeparateInstanceRule",
             "output": {
                 "shape": "NiftyRegisterInstancesWithSeparateInstanceRuleResult"
             }
         },
         "NiftyRegisterPortWithElasticLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30dd\u30fc\u30c8\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30dd\u30fc\u30c8\u306e\u8ffd\u52a0\u306b\u6210\u529f\u3057\u305f\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI \u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyRegisterInstancesWithElasticLoadBalancer.htm\">NiftyRegisterInstancesWithElasticLoadBalancer</a>\u300d\uff08\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\uff09</li> <li>API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyConfigureElasticLoadBalancerHealthCheck.htm\">NiftyConfigureElasticLoadBalancerHealthCheck</a>\u300d\uff08\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u8a2d\u5b9a\uff09</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRegisterPortWithElasticLoadBalancerRequest"
             },
             "name": "NiftyRegisterPortWithElasticLoadBalancer",
             "output": {
                 "shape": "NiftyRegisterPortWithElasticLoadBalancerResultWrapper"
             }
         },
         "NiftyRegisterRoutersWithSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u3001\u30eb\u30fc\u30bf\u30fc\u3078\u9069\u7528\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3078\u9069\u7528\u3059\u308b\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u540d\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30eb\u30fc\u30bf\u30fc\u9069\u7528\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cgroupStatus\u300d\u306b\u3066\u9069\u7528\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRegisterRoutersWithSecurityGroupRequest"
             },
             "name": "NiftyRegisterRoutersWithSecurityGroup",
             "output": {
                 "shape": "NiftyRegisterRoutersWithSecurityGroupResult"
             }
         },
         "NiftyRegisterVpnGatewaysWithSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3078\u9069\u7528\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3078\u9069\u7528\u3059\u308b\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u9069\u7528\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cgroupStatus\u300d\u306b\u3066\u9069\u7528\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRegisterVpnGatewaysWithSecurityGroupRequest"
             },
             "name": "NiftyRegisterVpnGatewaysWithSecurityGroup",
             "output": {
                 "shape": "NiftyRegisterVpnGatewaysWithSecurityGroupResult"
             }
         },
         "NiftyReleaseRouterBackupState": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306e\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u72b6\u614b\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReleaseRouterBackupStateRequest"
             },
             "name": "NiftyReleaseRouterBackupState",
             "output": {
                 "shape": "NiftyReleaseRouterBackupStateResult"
             }
         },
         "NiftyReleaseVpnGatewayBackupState": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u72b6\u614b\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReleaseVpnGatewayBackupStateRequest"
             },
             "name": "NiftyReleaseVpnGatewayBackupState",
             "output": {
                 "shape": "NiftyReleaseVpnGatewayBackupStateResult"
             }
         },
         "NiftyReplaceDhcpConfig": {
+            "documentation": "<p>DHCP\u30b3\u30f3\u30d5\u30a3\u30b0\u306e\u5165\u308c\u66ff\u3048\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u5165\u308c\u66ff\u3048\u524d\u3068\u540c\u4e00\u306e\u30b3\u30f3\u30d5\u30a3\u30b0ID\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001\u66f4\u65b0\u305b\u305a\u306b\u6b63\u5e38\u7d42\u4e86\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceDhcpConfigRequest"
             },
             "name": "NiftyReplaceDhcpConfig",
             "output": {
                 "shape": "NiftyReplaceDhcpConfigResult"
             }
         },
         "NiftyReplaceDhcpOption": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u767b\u9332\u3055\u308c\u305fDHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u3092\u89e3\u9664\u3057\u3001\u6307\u5b9a\u3057\u305fDHCP\u30aa\u30d7\u30b7\u30e7\u30f3\u306b\u5165\u308c\u66ff\u3048\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceDhcpOptionRequest"
             },
             "name": "NiftyReplaceDhcpOption",
             "output": {
                 "shape": "NiftyReplaceDhcpOptionResult"
             }
         },
         "NiftyReplaceElasticLoadBalancerLatestVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u5165\u308c\u66ff\u3048\u307e\u3059\u3002</p><p>\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u5165\u308c\u66ff\u308f\u308b\u5bfe\u8c61\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u3064\u3044\u3066\u306f\u3001\u5bfe\u8c61\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u8a2d\u5b9a\u3057\u3066\u3042\u308b\u5168\u3066\u306e\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u304c\u5bfe\u8c61\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u5165\u308c\u66ff\u3048\u308b\u969b\u306f\u3001\u901a\u4fe1\u65ad\u3092\u4f34\u3044\u307e\u3059\u3002\u901a\u4fe1\u65ad\u3068\u306a\u308b\u6642\u9593\u306b\u3064\u3044\u3066\u306f\u3001\u30b5\u30fc\u30d3\u30b9\u4ed5\u69d8\u30da\u30fc\u30b8\u3092\u3054\u53c2\u7167\u304f\u3060\u3055\u3044\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u304c\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u304b\u3069\u3046\u304b\u306f\u3001API\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeElasticLoadBalancers.htm\">NiftyDescribeElasticLoadBalancers</a>\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300c<a href=\"https://docs.nifcloud.com/cp/api/NiftyDescribeElasticLoadBalancers.htm#IsLatest\">IsLatest</a>\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u3068\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u4e21\u65b9\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u512a\u5148\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceElasticLoadBalancerLatestVersionRequest"
             },
             "name": "NiftyReplaceElasticLoadBalancerLatestVersion",
             "output": {
                 "shape": "NiftyReplaceElasticLoadBalancerLatestVersionResultWrapper"
             }
         },
         "NiftyReplaceElasticLoadBalancerListenerSSLCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u5bfe\u3057\u3066SSL\u8a3c\u660e\u66f8\u3092\u5165\u308c\u66ff\u3048\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u307e\u305f\u306f\u3001\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u30e6\u30cb\u30fc\u30afID\u30fb\u30d7\u30ed\u30c8\u30b3\u30eb\u30fb\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u756a\u53f7\u30fb\u5b9b\u5148\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u6709\u52b9\u300d\u304b\u3064\u3001\u6570\u91cf\u7121\u5236\u9650\u306e\u8a3c\u660e\u66f8\u306e\u307f\u8a2d\u5b9a\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceElasticLoadBalancerListenerSSLCertificateRequest"
             },
             "name": "NiftyReplaceElasticLoadBalancerListenerSSLCertificate",
             "output": {
                 "shape": "NiftyReplaceElasticLoadBalancerListenerSSLCertificateResultWrapper"
             }
         },
         "NiftyReplaceNatRule": {
+            "documentation": "<p>NAT\u30c6\u30fc\u30d6\u30eb\u306b\u767b\u9332\u3055\u308c\u305fNAT\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3057\u305fNAT\u30eb\u30fc\u30eb\u306b\u5165\u308c\u66ff\u3048\u308b\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceNatRuleRequest"
             },
             "name": "NiftyReplaceNatRule",
             "output": {
                 "shape": "NiftyReplaceNatRuleResult"
             }
         },
         "NiftyReplaceNatTableAssociation": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30eb\u30fc\u30c8NAT\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u3001\u6307\u5b9a\u3057\u305fNAT\u30c6\u30fc\u30d6\u30eb\u306b\u5165\u308c\u66ff\u3048\u307e\u3059\u3002</p><p>NAT\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001NAT\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceNatTableAssociationRequest"
             },
             "name": "NiftyReplaceNatTableAssociation",
             "output": {
                 "shape": "NiftyReplaceNatTableAssociationResult"
             }
         },
         "NiftyReplaceRouteTableAssociationWithElasticLoadBalancer": {
+            "documentation": "<p>\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3059\u308b\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceRouteTableAssociationWithElasticLoadBalancerRequest"
             },
             "name": "NiftyReplaceRouteTableAssociationWithElasticLoadBalancer",
             "output": {
                 "shape": "NiftyReplaceRouteTableAssociationWithElasticLoadBalancerResult"
             }
         },
         "NiftyReplaceRouteTableAssociationWithVpnGateway": {
+            "documentation": "<p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3078\u306e\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u8a2d\u5b9a\u5165\u308c\u66ff\u3048\u3092\u884c\u3046\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u3001\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306b\u5165\u308c\u66ff\u3048\u308b\u3002\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceRouteTableAssociationWithVpnGatewayRequest"
             },
             "name": "NiftyReplaceRouteTableAssociationWithVpnGateway",
             "output": {
                 "shape": "NiftyReplaceRouteTableAssociationWithVpnGatewayResult"
             }
         },
         "NiftyReplaceRouterLatestVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3092\u306e\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u306e\u306b\u5165\u308c\u66ff\u3048\u3057\u307e\u3059\u3002\u5165\u66ff\u524d\u306e\u30eb\u30fc\u30bf\u30fc\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3068\u3057\u3066\u4e00\u5b9a\u671f\u9593\u4fdd\u6301\u3055\u308c\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u65e2\u306b\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceRouterLatestVersionRequest"
             },
             "name": "NiftyReplaceRouterLatestVersion",
             "output": {
                 "shape": "NiftyReplaceRouterLatestVersionResult"
             }
         },
         "NiftyReplaceVpnGatewayLatestVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6700\u65b0\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u5165\u308c\u66ff\u3048\u307e\u3059\u3002</p><p>\u5165\u66ff\u524d\u306e\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306f\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3068\u3057\u3066\u4e00\u5b9a\u671f\u9593\u4fdd\u6301\u3055\u308c\u307e\u3059\u3002\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u65e2\u306b\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyReplaceVpnGatewayLatestVersionRequest"
             },
             "name": "NiftyReplaceVpnGatewayLatestVersion",
             "output": {
                 "shape": "NiftyReplaceVpnGatewayLatestVersionResult"
             }
         },
         "NiftyRestoreInstanceSnapshot": {
+            "documentation": "<p>\u4f5c\u6210\u6e08\u30ef\u30f3\u30c7\u30a4\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u304b\u3089\u306e\u30ea\u30b9\u30c8\u30a2\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30ea\u30b9\u30c8\u30a2\u3059\u308b\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u6307\u5b9a\u3059\u308b\u306b\u306f\u3001\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8ID\u307e\u305f\u306f\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u540d\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRestoreInstanceSnapshotRequest"
             },
             "name": "NiftyRestoreInstanceSnapshot",
             "output": {
                 "shape": "NiftyRestoreInstanceSnapshotResult"
             }
         },
         "NiftyRestoreRouterPreviousVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u3092\u3001\u4ee5\u524d\u306e\u65e7\u30d0\u30fc\u30b8\u30e7\u30f3\uff08\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u72b6\u614b\uff09\u306b\u5dee\u3057\u623b\u3057\u307e\u3059\u3002 \u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRestoreRouterPreviousVersionRequest"
             },
             "name": "NiftyRestoreRouterPreviousVersion",
             "output": {
                 "shape": "NiftyRestoreRouterPreviousVersionResult"
             }
         },
         "NiftyRestoreVpnGatewayPreviousVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u3001\u65e7\u30d0\u30fc\u30b8\u30e7\u30f3\uff08\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u72b6\u614b\uff09\u306b\u5dee\u3057\u623b\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRestoreVpnGatewayPreviousVersionRequest"
             },
             "name": "NiftyRestoreVpnGatewayPreviousVersion",
             "output": {
                 "shape": "NiftyRestoreVpnGatewayPreviousVersionResult"
             }
         },
         "NiftyRetryImportInstance": {
+            "documentation": "<p>VM\u30a4\u30f3\u30dd\u30fc\u30c8\u30a8\u30e9\u30fc\u3068\u306a\u3063\u305fVM\u306b\u5bfe\u3057\u3066\u3001\u518d\u30a4\u30f3\u30dd\u30fc\u30c8\u51e6\u7406\u3092\u5b9f\u884c\u3057\u307e\u3059\u3002</p><p>VM\u30a4\u30f3\u30dd\u30fc\u30c8\u30a8\u30e9\u30fc\u306e\u30b5\u30fc\u30d0\u30fc\u306e\u307f\u6307\u5b9a\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u307e\u305f\u306f\u30b5\u30fc\u30d0\u30fc\u30e6\u30cb\u30fc\u30afID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyRetryImportInstanceRequest"
             },
             "name": "NiftyRetryImportInstance",
             "output": {
                 "shape": "NiftyRetryImportInstanceResult"
             }
         },
         "NiftySetLoadBalancerSSLPoliciesOfListener": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30ea\u30b9\u30ca\u30fc\u306b\u5bfe\u3057\u3066SSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u306e\u8a2d\u5b9a\u3092\u884c\u3044\u307e\u3059\u3002<br> \u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002<br> \u307e\u305f\u3001SSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u306e\u30c6\u30f3\u30d7\u30ec\u30fc\u30c8ID\u3001\u3082\u3057\u304f\u306f\u30c6\u30f3\u30d7\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002<br> \u5bfe\u8c61\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u9069\u7528\u53ef\u80fd\u306aSSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u306b\u3064\u3044\u3066\u306f\u3001\u300cNiftyDescribeLoadBalancerSSLPolicies\u300d\u3067\u78ba\u8a8d\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftySetLoadBalancerSSLPoliciesOfListenerRequest"
             },
             "name": "NiftySetLoadBalancerSSLPoliciesOfListener",
             "output": {
                 "shape": "NiftySetLoadBalancerSSLPoliciesOfListenerResult"
             }
         },
         "NiftyUnsetLoadBalancerSSLPoliciesOfListener": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30ea\u30b9\u30ca\u30fc\u306b\u5bfe\u3057\u3066SSL\u30bb\u30ad\u30e5\u30ea\u30c6\u30a3\u30dd\u30ea\u30b7\u30fc\u8a2d\u5b9a\u306e\u89e3\u9664\u3092\u884c\u3044\u307e\u3059\u3002<br> \u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUnsetLoadBalancerSSLPoliciesOfListenerRequest"
             },
             "name": "NiftyUnsetLoadBalancerSSLPoliciesOfListener",
             "output": {
                 "shape": "NiftyUnsetLoadBalancerSSLPoliciesOfListenerResult"
             }
         },
         "NiftyUpdateAlarm": {
+            "documentation": "<p>\u57fa\u672c\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u76e3\u8996\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u3001\u76e3\u8996\u30eb\u30fc\u30eb\u540d\u304a\u3088\u3073\u6a5f\u80fd\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u5bfe\u8c61\u30ea\u30bd\u30fc\u30b9\u3001\u76e3\u8996\u30eb\u30fc\u30eb\u3001\u901a\u77e5\u5148\u30e1\u30fc\u30eb\u30a2\u30c9\u30ec\u30b9\u306e\u66f4\u65b0\u304c\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u3001\u65e2\u5b58\u306e\u5185\u5bb9\u3092\u7834\u68c4\u3057\u3001\u6307\u5b9a\u3057\u305f\u5185\u5bb9\u3067\u518d\u8a2d\u5b9a\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateAlarmRequest"
             },
             "name": "NiftyUpdateAlarm",
             "output": {
                 "shape": "NiftyUpdateAlarmResult"
             }
         },
         "NiftyUpdateAutoScalingGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u306e\u5b9a\u7fa9\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u65e2\u5b58\u306e\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u60c5\u5831\u306b\u5bfe\u3057\u3001\u6307\u5b9a\u3055\u308c\u305f\u5024\u3067\u30aa\u30fc\u30c8\u30b9\u30b1\u30fc\u30eb\u5b9a\u7fa9\u304c\u66f4\u65b0\u3055\u308c\u308b\u305f\u3081\u3001\u66f4\u65b0\u3057\u306a\u3044\u5024\u3082\u8a2d\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u305f\u3060\u3057\u30a4\u30e1\u30fc\u30b8ID\u306f\u4f8b\u5916\u7684\u306b\u7701\u7565\u53ef\u80fd\u3068\u3057\u3001\u7701\u7565\u6642\u306f\u5909\u66f4\u3057\u306a\u3044\u52d5\u4f5c\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u30a4\u30e1\u30fc\u30b8\u3092\u5909\u66f4\u3059\u308b\u5834\u5408\u3001\u5897\u8a2d\u30c7\u30a3\u30b9\u30af\u4ed8\u304d\u306e\u30a4\u30e1\u30fc\u30b8\u306f\u4f7f\u7528\u3067\u304d\u307e\u305b\u3093\u3002\u307e\u305f\u3001\u5909\u66f4\u524d\u306e\u30a4\u30e1\u30fc\u30b8\u3068\u7570\u306a\u308b\u30be\u30fc\u30f3\u306e\u30a4\u30e1\u30fc\u30b8\u3082\u4f7f\u7528\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateAutoScalingGroupRequest"
             },
             "name": "NiftyUpdateAutoScalingGroup",
             "output": {
                 "shape": "NiftyUpdateAutoScalingGroupResult"
             }
         },
         "NiftyUpdateElasticLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30de\u30eb\u30c1\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateElasticLoadBalancerRequest"
             },
             "name": "NiftyUpdateElasticLoadBalancer",
             "output": {
                 "shape": "NiftyUpdateElasticLoadBalancerResult"
             }
         },
         "NiftyUpdateInstanceNetworkInterfaces": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u8a2d\u5b9a\u3092\u6307\u5b9a\u3057\u305f\u72b6\u614b\u306b\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u304c\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30b5\u30fc\u30d0\u30fc\u306b\u3064\u3044\u3066</p><p>\u30fb\u30b0\u30ed\u30fc\u30d0\u30eb\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u8a2d\u5b9a\u306e\u5909\u66f4\u306f\u884c\u3046\u3053\u3068\u304c\u3067\u304d\u307e\u305b\u3093</p><p>\u30fb\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u8a2d\u5b9a\u306e\u5909\u66f4\u306f\u884c\u3046\u3053\u3068\u304c\u3067\u304d\u307e\u3059</p><p>\u30b5\u30fc\u30d0\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3092\u4ed6\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306b\u5909\u66f4\u3057\u305f\u3044\u3001\u307e\u305f\u306f\u53d6\u308a\u5916\u3057\u305f\u3044\u5834\u5408\u306fAPI\u300cDisassociateMultiIpAddressGroup\u300d\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateInstanceNetworkInterfacesRequest"
             },
             "name": "NiftyUpdateInstanceNetworkInterfaces",
             "output": {
                 "shape": "NiftyUpdateInstanceNetworkInterfacesResult"
             }
         },
         "NiftyUpdateRouterNetworkInterfaces": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30bf\u30fc\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306e\u5272\u308a\u5f53\u3066\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30bf\u30fc\u30e6\u30cb\u30fc\u30afID\u307e\u305f\u306f\u30eb\u30fc\u30bf\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u3001\u30eb\u30fc\u30bf\u30fc\u306b\u5272\u308a\u5f53\u3066\u308b\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30cd\u30c3\u30c8\u30ef\u30fc\u30afID\u307e\u305f\u306f\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateRouterNetworkInterfacesRequest"
             },
             "name": "NiftyUpdateRouterNetworkInterfaces",
             "output": {
                 "shape": "NiftyUpdateRouterNetworkInterfacesResult"
             }
         },
         "NiftyUpdateSeparateInstanceRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u30bb\u30d1\u30ec\u30fc\u30c8\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateSeparateInstanceRuleRequest"
             },
             "name": "NiftyUpdateSeparateInstanceRule",
             "output": {
                 "shape": "NiftyUpdateSeparateInstanceRuleResult"
             }
         },
         "NiftyUpdateVpnGatewayNetworkInterfaces": {
+            "documentation": "<p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u8a2d\u5b9a\u5909\u66f4\u3092\u3057\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30e6\u30fc\u30b6\u6240\u6709\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306fIP\u30a2\u30c9\u30ec\u30b9\u304c\u6307\u5b9a\u3067\u304d\u307e\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4ID\u307e\u305f\u306f\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u62e0\u70b9\u9593VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cDescribeVpnGateways\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "NiftyUpdateVpnGatewayNetworkInterfacesRequest"
             },
             "name": "NiftyUpdateVpnGatewayNetworkInterfaces",
             "output": {
                 "shape": "NiftyUpdateVpnGatewayNetworkInterfacesResult"
             }
         },
         "RebootInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u518d\u8d77\u52d5\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>NiftyIsBios\u306btrue\u3092\u6307\u5b9a\u3059\u308b\u3068\u3001BIOS\u8d77\u52d5\u753b\u9762\u3067\u505c\u6b62\u3057\u305f\u72b6\u614b\u3068\u306a\u308a\u307e\u3059\u3002\u30b3\u30f3\u30bd\u30fc\u30eb\u304b\u3089BIOS\u8a2d\u5b9a\u64cd\u4f5c\u3092\u884c\u3063\u3066\u304f\u3060\u3055\u3044\u3002</p><p>UserData\u3092\u6307\u5b9a\u3057\u3066\u30ea\u30af\u30a8\u30b9\u30c8\u3059\u308b\u5834\u5408\u306f\u3001POST\u306e\u307f\u306e\u5bfe\u5fdc\u3068\u306a\u308a\u307e\u3059\u306e\u3067\u3001\u3054\u6ce8\u610f\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RebootInstancesRequest"
             },
             "name": "RebootInstances",
             "output": {
                 "shape": "RebootInstancesResult"
             }
         },
         "RebootRemoteAccessVpnGateway": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u518d\u8d77\u52d5\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RebootRemoteAccessVpnGatewayRequest"
             },
             "name": "RebootRemoteAccessVpnGateway",
             "output": {
                 "shape": "RebootRemoteAccessVpnGatewayResult"
             }
         },
         "RefreshInstanceBackupRule": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306b\u5bfe\u3057\u3066\u3001\u521d\u56de\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u518d\u4f5c\u6210\u3057\u307e\u3059\u3002<br> \u5bfe\u8c61\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300cneed_refresh\uff08\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u53d6\u5f97\u4e0d\u53ef\uff09\u300d\u306e\u5834\u5408\u306e\u307f\u5b9f\u884c\u53ef\u80fd\u3068\u306a\u308a\u307e\u3059\u3002</p><p>\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3059\u308b\u5834\u5408\u306f\u3001API\u300c<a href=\"https://docs.nifcloud.com/cp/api/DescribeInstanceBackupRules.htm\">DescribeInstanceBackupRules</a>\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cstatus\uff08\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u30eb\u30fc\u30eb\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\uff09\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RefreshInstanceBackupRuleRequest"
             },
             "name": "RefreshInstanceBackupRule",
             "output": {
                 "shape": "RefreshInstanceBackupRuleResult"
             }
         },
         "RegisterCorporateInfoForCertificate": {
+            "documentation": "<p>SSL\u8a3c\u660e\u66f8\u3092\u7ba1\u7406\u3059\u308b\u7533\u8acb\u6cd5\u4eba\u60c5\u5831\u3092\u767b\u9332\u307e\u305f\u306f\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u4ee5\u4e0b\u306e\u5229\u7528\u898f\u7d04\u3092\u3054\u78ba\u8a8d\u306e\u4e0a\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p><a href=\"https://www.geotrust.co.jp/resources/repository/legal.html\">GeoTrust SSL\u8a3c\u660e\u66f8\u5229\u7528\u898f\u7d04</a></p><p><a href=\"https://www.cybertrust.ne.jp/ssl/repository/index.html\">CyberTrust SureServer\u8a3c\u660e\u66f8\u5229\u7528\u898f\u7d04</a></p><p>\u300cAgreement\u300d\u3092\u6307\u5b9a\u3057\u306a\u3044\u5834\u5408\u3001\u7533\u8acb\u6cd5\u4eba\u60c5\u5831\u767b\u9332\u3001\u66f4\u65b0\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RegisterCorporateInfoForCertificateRequest"
             },
             "name": "RegisterCorporateInfoForCertificate",
             "output": {
                 "shape": "RegisterCorporateInfoForCertificateResult"
             }
         },
         "RegisterInstancesWithLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30b5\u30fc\u30d0\u30fc\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002\u81ea\u5206\u304c\u6240\u6709\u3057\u3066\u3044\u306a\u3044\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u5834\u5408\u306f\u3001\u300c\u30cb\u30d5\u30af\u30e9ID.\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u300d\u306e\u5f62\u5f0f\u3067\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002IP\u30a2\u30c9\u30ec\u30b9\u3092\u56fa\u5b9a\u5316\u3057\u3066\u3044\u308b\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RegisterInstancesWithLoadBalancerRequest"
             },
             "name": "RegisterInstancesWithLoadBalancer",
             "output": {
                 "shape": "RegisterInstancesWithLoadBalancerResultWrapper"
             }
         },
         "RegisterInstancesWithSecurityGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u3001\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3078\u9069\u7528\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3078\u30b5\u30fc\u30d0\u30fc\u3092\u9069\u7528\u3059\u308b\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u9069\u7528\u6e08\u307f\u300d\u306e\u5834\u5408\u3001\u9069\u7528\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u304c\u6b63\u3057\u304f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstancesSet\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RegisterInstancesWithSecurityGroupRequest"
             },
             "name": "RegisterInstancesWithSecurityGroup",
             "output": {
                 "shape": "RegisterInstancesWithSecurityGroupResult"
             }
         },
         "RegisterPortWithLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30dd\u30fc\u30c8\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30dd\u30fc\u30c8\u306e\u8ffd\u52a0\u306b\u6210\u529f\u3057\u305f\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300cRegisterInstancesWithLoadBalancer\u300d\uff08\u30b5\u30fc\u30d0\u30fc\u8a2d\u5b9a\uff09</li> <li>API\u300cConfigureHealthCheck\u300d\uff08\u30d8\u30eb\u30b9\u30c1\u30a7\u30c3\u30af\u8a2d\u5b9a\uff09</li> </ul> <p>\u30d5\u30a3\u30eb\u30bf\u30fc\u306e\u8a2d\u5b9a\u306f\u3001\u300c\u3059\u3079\u3066\u306e\u30a2\u30af\u30bb\u30b9\u3092\u8a31\u53ef\u3059\u308b\u300d\u306b\u306a\u3063\u3066\u3044\u307e\u3059\u3002\u5909\u66f4\u3092\u884c\u3046\u5834\u5408\u306f\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300cSetFilterForLoadBalancer\u300d\uff08\u30d5\u30a3\u30eb\u30bf\u30fc\u8a2d\u5b9a\uff09</li> </ul> <p>Listeners.member.n.Protocol\u3068Listeners.member.n.LoadBalancerPort\u3092\u4e21\u65b9\u6307\u5b9a\u3057\u305f\u5834\u5408\u306f\u3001Listeners.member.n.LoadBalancerPort\u306e\u6307\u5b9a\u304c\u512a\u5148\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RegisterPortWithLoadBalancerRequest"
             },
             "name": "RegisterPortWithLoadBalancer",
             "output": {
                 "shape": "RegisterPortWithLoadBalancerResultWrapper"
             }
         },
         "ReleaseAddress": {
+            "documentation": "<p>\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u306e\u89e3\u653e\u3092\u884c\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReleaseAddressRequest"
             },
             "name": "ReleaseAddress",
             "output": {
                 "shape": "ReleaseAddressResult"
             }
         },
         "ReleaseMultiIpAddresses": {
+            "documentation": "<p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3067\u78ba\u4fdd\u3057\u3066\u3044\u308bIP\u30a2\u30c9\u30ec\u30b9\u3092\u89e3\u653e\u3057\u307e\u3059\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3067\u78ba\u4fdd\u3057\u3066\u3044\u308b\u5168\u3066\u306eIP\u30a2\u30c9\u30ec\u30b9\u3092\u89e3\u653e\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u30de\u30eb\u30c1IP\u30a2\u30c9\u30ec\u30b9\u30b0\u30eb\u30fc\u30d7\u3067\u78ba\u4fdd\u3057\u3066\u3044\u308bIP\u30a2\u30c9\u30ec\u30b9\u3092\u5168\u3066\u89e3\u653e\u3057\u305f\u3044\u5834\u5408\u306f\u3001\u4ee5\u4e0b\u306eAPI\u3092\u5b9f\u884c\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p> <ul> <li>API\u300c<a href=\"https://docs.nifcloud.com/cp/api/DeleteMultiIpAddressGroup.htm\">DeleteMultiIpAddressGroup</a>\u300d</li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReleaseMultiIpAddressesRequest"
             },
             "name": "ReleaseMultiIpAddresses",
             "output": {
                 "shape": "ReleaseMultiIpAddressesResult"
             }
         },
         "ReplaceRemoteAccessVpnGatewayLatestVersion": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u3057\u307e\u3059\u3002<br> \u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u3092\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u3059\u308b\u5834\u5408\u306b\u306f\u3001\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304c\u518d\u8d77\u52d5\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReplaceRemoteAccessVpnGatewayLatestVersionRequest"
             },
             "name": "ReplaceRemoteAccessVpnGatewayLatestVersion",
             "output": {
                 "shape": "ReplaceRemoteAccessVpnGatewayLatestVersionResult"
             }
         },
         "ReplaceRoute": {
+            "documentation": "<p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306b\u767b\u9332\u3055\u308c\u305f\u30eb\u30fc\u30c8\u60c5\u5831\u3092\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30c8\u60c5\u5831\u306b\u5165\u308c\u66ff\u3048\u308b\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReplaceRouteRequest"
             },
             "name": "ReplaceRoute",
             "output": {
                 "shape": "ReplaceRouteResult"
             }
         },
         "ReplaceRouteTableAssociation": {
+            "documentation": "<p>\u30eb\u30fc\u30bf\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u89e3\u9664\u3057\u3001\u6307\u5b9a\u3057\u305f\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u306b\u5165\u308c\u66ff\u3048\u308b\u3002</p><p>\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30eb\u30fc\u30c8\u30c6\u30fc\u30d6\u30ebID\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30eb\u30fc\u30bf\u30fc\u304c\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u306f\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cAgreement\u300d\u306b\u300ctrue\u300d\u3092\u8a2d\u5b9a\u3057\u3001\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u89e3\u9664\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3092\u4fdd\u6301\u3057\u3066\u3044\u308b\u304b\u3069\u3046\u304b\u306fAPI\u300cNiftyDescribeRouters\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cisBackup\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "ReplaceRouteTableAssociationRequest"
             },
             "name": "ReplaceRouteTableAssociation",
             "output": {
                 "shape": "ReplaceRouteTableAssociationResult"
             }
         },
         "RevokeSecurityGroupIngress": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u307e\u305f\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b \u8a31\u53ef\u30d7\u30ed\u30c8\u30b3\u30eb\u540d\u30fb\u8a31\u53ef\u30dd\u30fc\u30c8\u30fb\u8a31\u53ef\u3059\u308b\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u307e\u305f\u306f\u8a31\u53ef\u3059\u308bIP\u30a2\u30c9\u30ec\u30b9 \u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u8a31\u53ef\u30eb\u30fc\u30eb\u306e\u8a31\u53ef\u30d7\u30ed\u30c8\u30b3\u30eb\u304cTCP\u304bUDP\u306e\u5834\u5408\u3001\u8a31\u53ef\u30dd\u30fc\u30c8\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002\u30dd\u30fc\u30c8\u3092\u5358\u4e00\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u307f\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002\u30dd\u30fc\u30c8\u3092\u7bc4\u56f2\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u7d42\u4e86\u30dd\u30fc\u30c8\u306b\u306f\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u5024\u4ee5\u4e0a\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u8a31\u53ef\u30eb\u30fc\u30eb\u306e\u524a\u9664\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u9069\u7528\u6e08\u307f\u300d\u306e\u5834\u5408\u3001\u524a\u9664\u3057\u305f\u8a31\u53ef\u30eb\u30fc\u30eb\u304c\u6b63\u3057\u304f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u540c\u3058\u304fAPI\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cipPermissions\u300d\u307e\u305f\u306f\u300cgroups\u300d\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RevokeSecurityGroupIngressRequest"
             },
             "name": "RevokeSecurityGroupIngress",
             "output": {
                 "shape": "RevokeSecurityGroupIngressResult"
             }
         },
         "RunInstances": {
+            "documentation": "<p>\u30b5\u30fc\u30d0\u30fc\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u4f5c\u6210\u3067\u304d\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u4f5c\u6210\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300cinstanceState\u300d\u3092\u78ba\u8a8d\u3057\u300cpending\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u3001\u307e\u305f\u306f\u30bf\u30a4\u30e0\u30a2\u30a6\u30c8\u3057\u305f\u5834\u5408\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>API\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306b\u300cIpType\u300d\u3001\u300cNetworkInterface.n.NetworkId\u300d\u4e21\u65b9\u3092\u6307\u5b9a\u3057\u306a\u304b\u3063\u305f\u5834\u5408\u3001\u300cIpType\u300d\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306edefault\u5024\u304c\u9069\u7528\u3055\u308c\u307e\u3059\u3002</p><p>UserData\u3092\u6307\u5b9a\u3057\u3066\u30ea\u30af\u30a8\u30b9\u30c8\u3059\u308b\u5834\u5408\u306f\u3001POST\u306e\u307f\u306e\u5bfe\u5fdc\u3068\u306a\u308a\u307e\u3059\u306e\u3067\u3001\u3054\u6ce8\u610f\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "RunInstancesRequest"
             },
             "name": "RunInstances",
             "output": {
                 "shape": "RunInstancesResult"
             }
         },
         "SetFilterForLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u30a2\u30af\u30bb\u30b9\u30d5\u30a3\u30eb\u30bf\u30fc\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "SetFilterForLoadBalancerRequest"
             },
             "name": "SetFilterForLoadBalancer",
             "output": {
                 "shape": "SetFilterForLoadBalancerResultWrapper"
             }
         },
         "SetLoadBalancerListenerSSLCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u5bfe\u3057\u3066SSL\u8a3c\u660e\u66f8\u3092\u53d6\u308a\u4ed8\u3051\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>SSL\u8a3c\u660e\u66f8\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001SSL\u8a3c\u660e\u66f8\u306e\u767a\u884c\u8b58\u5225\u5b50\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u6709\u52b9\u300d\u304b\u3064\u3001\u6570\u91cf\u7121\u5236\u9650\u306e\u8a3c\u660e\u66f8\u306e\u307f\u8a2d\u5b9a\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "SetLoadBalancerListenerSSLCertificateRequest"
             },
             "name": "SetLoadBalancerListenerSSLCertificate",
             "output": {
                 "shape": "SetLoadBalancerListenerSSLCertificateResultWrapper"
             }
         },
         "SetRemoteAccessVpnGatewayCACertificate": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u3001CA\u8a3c\u660e\u66f8\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "SetRemoteAccessVpnGatewayCACertificateRequest"
             },
             "name": "SetRemoteAccessVpnGatewayCACertificate",
             "output": {
                 "shape": "SetRemoteAccessVpnGatewayCACertificateResult"
             }
         },
         "SetRemoteAccessVpnGatewaySSLCertificate": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306b\u3001SSL\u8a3c\u660e\u66f8\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "SetRemoteAccessVpnGatewaySSLCertificateRequest"
             },
             "name": "SetRemoteAccessVpnGatewaySSLCertificate",
             "output": {
                 "shape": "SetRemoteAccessVpnGatewaySSLCertificateResult"
             }
         },
         "StartInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u8d77\u52d5\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u8d77\u52d5\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300ccurrentState.name\u300d\u3092\u78ba\u8a8d\u3057\u3066\u300cpending\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u5834\u5408\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>NiftyIsBios\u3092true\u306b\u6307\u5b9a\u3059\u308b\u3068\u3001BIOS\u8d77\u52d5\u753b\u9762\u3067\u505c\u6b62\u3057\u305f\u72b6\u614b\u3068\u306a\u308a\u307e\u3059\u3002\u30b3\u30f3\u30bd\u30fc\u30eb\u304b\u3089BIOS\u8a2d\u5b9a\u64cd\u4f5c\u3092\u884c\u3063\u3066\u304f\u3060\u3055\u3044\u3002</p><p>UserData\u3092\u6307\u5b9a\u3057\u3066\u30ea\u30af\u30a8\u30b9\u30c8\u3059\u308b\u5834\u5408\u306f\u3001POST\u306e\u307f\u306e\u5bfe\u5fdc\u3068\u306a\u308a\u307e\u3059\u306e\u3067\u3001\u3054\u6ce8\u610f\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "StartInstancesRequest"
             },
             "name": "StartInstances",
             "output": {
                 "shape": "StartInstancesResult"
             }
         },
         "StopInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u505c\u6b62\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u505c\u6b62\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300ccurrentState.name\u300d\u3092\u78ba\u8a8d\u3057\u3066\u300cpending\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u5834\u5408\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u306a\u304a\u3001\u5f37\u5236\u30aa\u30d7\u30b7\u30e7\u30f3\u306b\u300ctrue\u300d\u3092\u6307\u5b9a\u3057\u3066\u5b9f\u884c\u3057\u305f\u969b\u306b\u3001\u30b5\u30fc\u30d0\u30fc\u304c\u505c\u6b62\u3067\u304d\u306a\u3044\u72b6\u614b\u306a\u3069\u306e\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u5f37\u5236\u30aa\u30d7\u30b7\u30e7\u30f3\u306b\u300ctrue\u300d\u3092\u6307\u5b9a\u3057\u3066\u5b9f\u884c\u3057\u305f\u5834\u5408\u306b\u306f\u3001\u30b7\u30b9\u30c6\u30e0\u30c1\u30a7\u30c3\u30af\u3084\u4fee\u5fa9\u3092\u884c\u3046\u3053\u3068\u3092\u304a\u3059\u3059\u3081\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "StopInstancesRequest"
             },
             "name": "StopInstances",
             "output": {
                 "shape": "StopInstancesResult"
             }
         },
         "TerminateInstances": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30b5\u30fc\u30d0\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30b5\u30fc\u30d0\u30fc\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30b5\u30fc\u30d0\u30fc\u306e\u524a\u9664\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u3053\u306eAPI\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u300ccurrentState.name\u300d\u3092\u78ba\u8a8d\u3057\u3066\u300cpending\u300d\u304c\u8fd4\u3063\u3066\u304d\u305f\u5834\u5408\u306f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cinstanceState\u300d\u3067\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002\u307e\u305f\u3001API\u300cDescribeInstances\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u306b\u8a72\u5f53\u60c5\u5831\u304c\u306a\u3044\u5834\u5408\u306f\u3001\u524a\u9664\u51e6\u7406\u306f\u6210\u529f\u3057\u3066\u3044\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u4e2d\u307e\u305f\u306f\u30a4\u30f3\u30dd\u30fc\u30c8\u4e2d\u306e\u30b5\u30fc\u30d0\u30fc\u3092\u3001\u3053\u306eAPI\u3067\u524a\u9664\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002API\u300cCancelUpload\u300d\u3092\u4f7f\u7528\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>\u95a2\u9023\u3059\u308b\u4ed8\u66ffIP\u30a2\u30c9\u30ec\u30b9\u8a2d\u5b9a\u3082\u3042\u308f\u305b\u3066\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "TerminateInstancesRequest"
             },
             "name": "TerminateInstances",
             "output": {
                 "shape": "TerminateInstancesResult"
             }
         },
         "UnsetLoadBalancerListenerSSLCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308bSSL\u8a3c\u660e\u66f8\u3092\u306f\u305a\u3057\u307e\u3059\u3002</p><p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u540d\u30fb\u30dd\u30fc\u30c8\u756a\u53f7\u304c\u5fc5\u8981\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UnsetLoadBalancerListenerSSLCertificateRequest"
             },
             "name": "UnsetLoadBalancerListenerSSLCertificate",
             "output": {
                 "shape": "UnsetLoadBalancerListenerSSLCertificateResultWrapper"
             }
         },
         "UnsetRemoteAccessVpnGatewayCACertificate": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304b\u3089\u3001CA\u8a3c\u660e\u66f8\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UnsetRemoteAccessVpnGatewayCACertificateRequest"
             },
             "name": "UnsetRemoteAccessVpnGatewayCACertificate",
             "output": {
                 "shape": "UnsetRemoteAccessVpnGatewayCACertificateResult"
             }
         },
         "UnsetRemoteAccessVpnGatewaySSLCertificate": {
+            "documentation": "<p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u304b\u3089\u3001SSL\u8a3c\u660e\u66f8\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p><p>\u30ea\u30e2\u30fc\u30c8\u30a2\u30af\u30bb\u30b9VPN\u30b2\u30fc\u30c8\u30a6\u30a7\u30a4\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u304c v2.0.0 \u4ee5\u4e0a\u306e\u5834\u5408\u3001\u5229\u7528\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UnsetRemoteAccessVpnGatewaySSLCertificateRequest"
             },
             "name": "UnsetRemoteAccessVpnGatewaySSLCertificate",
             "output": {
                 "shape": "UnsetRemoteAccessVpnGatewaySSLCertificateResult"
             }
         },
         "UpdateLoadBalancer": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u5b9a\u7fa9\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u30dd\u30fc\u30c8\u5b9a\u7fa9\u3092\u66f4\u65b0\u3059\u308b\u5834\u5408\u306f\u3001\u30dd\u30fc\u30c8\u756a\u53f7\u3082\u3042\u308f\u305b\u3066\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>ListenerUpdate.Listener.Protocol\u306f\u3001\u6307\u5b9a\u3057\u305fListenerUpdate.Listener.LoadBalancerPort\u306e\u5024\u306b\u3088\u3063\u3066\u3001\u8a2d\u5b9a\u5024\u3068\u7570\u306a\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UpdateLoadBalancerRequest"
             },
             "name": "UpdateLoadBalancer",
             "output": {
                 "shape": "UpdateLoadBalancerResult"
             }
         },
         "UpdateLoadBalancerOption": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u30aa\u30d7\u30b7\u30e7\u30f3\u8a2d\u5b9a\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u5404\u30aa\u30d7\u30b7\u30e7\u30f3\u306e\u5229\u7528\u8a2d\u5b9a\u304ctrue\u306e\u5834\u5408\u306f\u6709\u52b9\u3001false\u306e\u5834\u5408\u306f\u7121\u52b9\u3078\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>Sorry\u30da\u30fc\u30b8\u30aa\u30d7\u30b7\u30e7\u30f3\u3092\u6709\u52b9\u306b\u3059\u308b\u305f\u3081\u306b\u306f\u6307\u5b9a\u3059\u308b\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u5f85\u3061\u53d7\u3051\u30dd\u30fc\u30c8\u304c80\u756a\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UpdateLoadBalancerOptionRequest"
             },
             "name": "UpdateLoadBalancerOption",
             "output": {
                 "shape": "UpdateLoadBalancerOptionResult"
             }
         },
         "UpdateSecurityGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u60c5\u5831\u3092\u66f4\u65b0\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u30011\u3064\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u66f4\u65b0\u3067\u304d\u307e\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u6307\u5b9a\u3059\u308b\u305f\u3081\u306b\u306f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u60c5\u5831\u306e\u66f4\u65b0\u306b\u306f\u3001\u6642\u9593\u304c\u304b\u304b\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002API\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u300cgroupStatus\u300d\u3067\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u307e\u305f\u3001\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u300c\u9069\u7528\u6e08\u307f\u300d\u306e\u5834\u5408\u3001\u66f4\u65b0\u3057\u305f\u60c5\u5831\u304c\u6b63\u3057\u304f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u53cd\u6620\u3055\u308c\u3066\u3044\u308b\u304b\u306e\u78ba\u8a8d\u304c\u5fc5\u8981\u3067\u3059\u3002\u540c\u3058\u304fAPI\u300cDescribeSecurityGroups\u300d\u306e\u30ec\u30b9\u30dd\u30f3\u30b9\u5024\u3067\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p><p>\u306a\u304a\u3001\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u300cGroupLogFilterNetBios\u300d\u3068\u300cGroupLogFilterBroadcast\u300d\u306b\u3064\u3044\u3066\u306f\u3001\u6307\u5b9a\u3057\u305f\u5834\u5408\u3067\u3082Default\u306e\u5024\u304c\u9069\u7528\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UpdateSecurityGroupRequest"
             },
             "name": "UpdateSecurityGroup",
             "output": {
                 "shape": "UpdateSecurityGroupResult"
             }
         },
         "UploadIsoImage": {
+            "documentation": "<p>ISO\u30a4\u30e1\u30fc\u30b8\u3092\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3059\u308bISO\u30a4\u30e1\u30fc\u30b8\u306eURL\u306f\u3001\u30cb\u30d5\u30af\u30e9\u304b\u3089\u30a2\u30af\u30bb\u30b9\u53ef\u80fd\u306aURL\u3067\u3042\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UploadIsoImageRequest"
             },
             "name": "UploadIsoImage",
             "output": {
                 "shape": "UploadIsoImageResult"
             }
         },
         "UploadSslCertificate": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fSSL\u8a3c\u660e\u66f8\u3092\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u307e\u3059\u30021\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001SSL\u8a3c\u660e\u66f8\u306e\u30ad\u30fc\u30fbCA\u30fb\u8a3c\u660e\u66f8\u306e1\u30bb\u30c3\u30c8\u3092\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3067\u304d\u307e\u3059\u3002 \u9375\u9577\u304c4096bit\u3092\u8d85\u3048\u308b\u5834\u5408\u3001\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3067\u304d\u307e\u305b\u3093\u3002 </p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/api/"
             },
             "input": {
                 "shape": "UploadSslCertificateRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/computing/3.0/waiters-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/computing/3.0/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'operations'": "{'ChangeResourceRecordSets': {'documentation': "*

 * *                 "'<p>レコードの作成、削除を行います。</p><p>リクエストボディにて作成/削除するレコード情報を入力し、それにもとづいてレコード情報の作成/削除が行われます。</p><p>1つのリクエスト内で複数のレコード作成/削除操作を指定できますが、処理の途中でエラーになった場合部分的な反映になる場合があります。</p><p>同じゾーンに対して同時に作成/削除操作のリクエストを行うと、エラーになる場合があります。</p><p>レコード作成/削除は即時反映ではないため、レスポンスには作成された更新リクエスト情報が含まれ、これの反映ステータスがPENDINGからINSYNCに変わったタイミングが反映完了となります。</p>'}, "*

 * *                 "'CreateHostedZone': {'documentation': "*

 * *                 "'<p>ゾーンの作成を行います。</p><p>リクエストボディにてゾー […]*

```diff
@@ -8,14 +8,15 @@
         "serviceId": "dns",
         "signatureVersion": "v3",
         "uid": "dns-2012-12-12N2013-12-16",
         "xmlNamespace": "https://route53.amazonaws.com/doc/2012-12-12/"
     },
     "operations": {
         "ChangeResourceRecordSets": {
+            "documentation": "<p>\u30ec\u30b3\u30fc\u30c9\u306e\u4f5c\u6210\u3001\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u30dc\u30c7\u30a3\u306b\u3066\u4f5c\u6210/\u524a\u9664\u3059\u308b\u30ec\u30b3\u30fc\u30c9\u60c5\u5831\u3092\u5165\u529b\u3057\u3001\u305d\u308c\u306b\u3082\u3068\u3065\u3044\u3066\u30ec\u30b3\u30fc\u30c9\u60c5\u5831\u306e\u4f5c\u6210/\u524a\u9664\u304c\u884c\u308f\u308c\u307e\u3059\u3002</p><p>1\u3064\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u5185\u3067\u8907\u6570\u306e\u30ec\u30b3\u30fc\u30c9\u4f5c\u6210/\u524a\u9664\u64cd\u4f5c\u3092\u6307\u5b9a\u3067\u304d\u307e\u3059\u304c\u3001\u51e6\u7406\u306e\u9014\u4e2d\u3067\u30a8\u30e9\u30fc\u306b\u306a\u3063\u305f\u5834\u5408\u90e8\u5206\u7684\u306a\u53cd\u6620\u306b\u306a\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u540c\u3058\u30be\u30fc\u30f3\u306b\u5bfe\u3057\u3066\u540c\u6642\u306b\u4f5c\u6210/\u524a\u9664\u64cd\u4f5c\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3092\u884c\u3046\u3068\u3001\u30a8\u30e9\u30fc\u306b\u306a\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30ec\u30b3\u30fc\u30c9\u4f5c\u6210/\u524a\u9664\u306f\u5373\u6642\u53cd\u6620\u3067\u306f\u306a\u3044\u305f\u3081\u3001\u30ec\u30b9\u30dd\u30f3\u30b9\u306b\u306f\u4f5c\u6210\u3055\u308c\u305f\u66f4\u65b0\u30ea\u30af\u30a8\u30b9\u30c8\u60c5\u5831\u304c\u542b\u307e\u308c\u3001\u3053\u308c\u306e\u53cd\u6620\u30b9\u30c6\u30fc\u30bf\u30b9\u304cPENDING\u304b\u3089INSYNC\u306b\u5909\u308f\u3063\u305f\u30bf\u30a4\u30df\u30f3\u30b0\u304c\u53cd\u6620\u5b8c\u4e86\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone/{ZoneID}/rrset"
             },
             "input": {
                 "locationName": "ChangeResourceRecordSetsRequest",
                 "shape": "ChangeResourceRecordSetsRequest",
@@ -25,14 +26,15 @@
             },
             "name": "ChangeResourceRecordSets",
             "output": {
                 "shape": "ChangeResourceRecordSetsResult"
             }
         },
         "CreateHostedZone": {
+            "documentation": "<p>\u30be\u30fc\u30f3\u306e\u4f5c\u6210\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u30dc\u30c7\u30a3\u306b\u3066\u30be\u30fc\u30f3\u306e\u4f5c\u6210\u306b\u5fc5\u8981\u306a\u60c5\u5831\u3092\u5165\u529b\u3057\u3001\u305d\u308c\u306b\u3082\u3068\u3065\u3044\u3066\u30be\u30fc\u30f3\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305f\u30be\u30fc\u30f3\u306e\u30c9\u30e1\u30a4\u30f3\u3092\u30e6\u30fc\u30b6\u30fc\u304c\u6240\u6301\u3057\u3066\u3044\u308b\u5834\u5408\u3001\u8a8d\u8a3c\u306a\u3057\u3067\u30be\u30fc\u30f3\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p><p>\u4f5c\u6210\u3057\u305f\u30be\u30fc\u30f3\u306e\u30c9\u30e1\u30a4\u30f3\u3092\u30e6\u30fc\u30b6\u30fc\u304c\u6240\u6301\u3057\u3066\u3044\u306a\u3044\u5834\u5408\u3001\u30be\u30fc\u30f3\u4f5c\u6210\u524d\u306b\u8a8d\u8a3c\u304c\u884c\u308f\u308c\u308b\u305f\u3081\u3001Unauthorized\u30a8\u30e9\u30fc\u304c\u767a\u751f\u3057\u307e\u3059\u3002 Unauthorized\u767a\u751f\u306e\u5834\u5408\u3001\u30a8\u30e9\u30fc\u30e1\u30c3\u30bb\u30fc\u30b8\u306b\u3042\u308b\u8a8d\u8a3c\u60c5\u5831\u3092\u30ec\u30b8\u30b9\u30c8\u30e9\u307e\u305f\u306fDNS\u306b\u8a2d\u5b9a\u3057\u3001\u518d\u5ea6\u672cAPI\u3092\u5b9f\u884c\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>\u8a8d\u8a3c\u306b\u5931\u6557\u3057\u305f\u5834\u5408\u306f\u3001\u30be\u30fc\u30f3\u306f\u4f5c\u6210\u3055\u308c\u305a\u30a8\u30e9\u30fc\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone"
             },
             "input": {
                 "locationName": "CreateHostedZoneRequest",
                 "shape": "CreateHostedZoneRequest",
@@ -42,66 +44,71 @@
             },
             "name": "CreateHostedZone",
             "output": {
                 "shape": "CreateHostedZoneResult"
             }
         },
         "DeleteHostedZone": {
+            "documentation": "<p>\u30be\u30fc\u30f3\u306e\u524a\u9664\u3092\u884c\u3044\u307e\u3059\u3002</p><p>\u524a\u9664\u3092\u884c\u3046\u30be\u30fc\u30f3\u306f\u3001\u30ea\u30af\u30a8\u30b9\u30c8\u5185\u3067\u30be\u30fc\u30f3ID\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3067\u884c\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone/{ZoneID}"
             },
             "input": {
                 "shape": "DeleteHostedZoneRequest"
             },
             "name": "DeleteHostedZone",
             "output": {
                 "shape": "DeleteHostedZoneResult"
             }
         },
         "GetChange": {
+            "documentation": "<p>\u66f4\u65b0\u30ea\u30af\u30a8\u30b9\u30c8\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u60c5\u5831\u3092\u53d6\u5f97\u3059\u308b\u66f4\u65b0\u30ea\u30af\u30a8\u30b9\u30c8\u60c5\u5831\u306f\u3001\u30ea\u30af\u30a8\u30b9\u30c8\u5185\u3067\u66f4\u65b0\u30ea\u30af\u30a8\u30b9\u30c8ID\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3067\u884c\u3044\u307e\u3059\u3002</p><p>\u672cAPI\u306f\u66f4\u65b0\u7cfbAPI\u6210\u529f\u6642\u306e\u66f4\u65b0\u30ea\u30af\u30a8\u30b9\u30c8ID\u306e\u307f\u5bfe\u5fdc\u3057\u3066\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/2012-12-12N2013-12-16/change/{ChangeID}"
             },
             "input": {
                 "shape": "GetChangeRequest"
             },
             "name": "GetChange",
             "output": {
                 "shape": "GetChangeResult"
             }
         },
         "GetHostedZone": {
+            "documentation": "<p>\u30be\u30fc\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u53d6\u5f97\u3059\u308b\u30be\u30fc\u30f3\u60c5\u5831\u306e\u6307\u5b9a\u306f\u3001\u30ea\u30af\u30a8\u30b9\u30c8URL\u5185\u306b\u542b\u307e\u308c\u308b\u30be\u30fc\u30f3ID\u306b\u3066\u884c\u3044\u307e\u3059\u3002</p><p>\u53d6\u5f97\u3055\u308c\u308b\u60c5\u5831\u306f\u3001\u30be\u30fc\u30f3\u60c5\u5831\u3001\u30cd\u30fc\u30e0\u30b5\u30fc\u30d0\u30fc\u60c5\u5831\u306e\uff12\u3064\u3067\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone/{ZoneID}"
             },
             "input": {
                 "shape": "GetHostedZoneRequest"
             },
             "name": "GetHostedZone",
             "output": {
                 "shape": "GetHostedZoneResult"
             }
         },
         "ListHostedZones": {
+            "documentation": "<p>\u30be\u30fc\u30f3\u306e\u60c5\u5831\u3092\u4e00\u89a7\u3067\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u5185\u306eURL\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306b\u3088\u308a\u3001\u53d6\u5f97\u3059\u308b\u4e00\u89a7\u306e\u5148\u982d\u306e\u30be\u30fc\u30f3ID\u3001\u53d6\u5f97\u3059\u308b\u4e00\u89a7\u306e\u6700\u5927\u4ef6\u6570\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u53d6\u5f97\u3055\u308c\u308b\u60c5\u5831\u306f\u3001\u30be\u30fc\u30f3\u60c5\u5831\u306e\u307f\u3067\u3001\u30cd\u30fc\u30e0\u30b5\u30fc\u30d0\u30fc\u60c5\u5831\u306f\u53d6\u5f97\u3055\u308c\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone"
             },
             "input": {
                 "shape": "ListHostedZonesRequest"
             },
             "name": "ListHostedZones",
             "output": {
                 "shape": "ListHostedZonesResult"
             }
         },
         "ListResourceRecordSets": {
+            "documentation": "<p>\u30ec\u30b3\u30fc\u30c9\u306e\u60c5\u5831\u3092\u4e00\u89a7\u3067\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u5185\u306eURL\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306b\u3088\u308a\u3001\u53d6\u5f97\u3092\u958b\u59cb\u3059\u308b\u30ec\u30b3\u30fc\u30c9\u60c5\u5831\u306e\u540d\u524d\uff08\u30c9\u30e1\u30a4\u30f3\uff09\u3001\u7a2e\u5225\u3001\u8b58\u5225\u60c5\u5831\u3068\u3001\u6700\u5927\u53d6\u5f97\u4ef6\u6570\u3092\u6307\u5b9a\u3067\u304d\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u306eidentifer\u306f\u30e6\u30fc\u30b6\u30fc\u767b\u9332\u3057\u305f\u60c5\u5831\u3067\u306f\u306a\u304f\u3001\u30b7\u30b9\u30c6\u30e0\u304c\u751f\u6210\u3057\u305f\u30e9\u30f3\u30c0\u30e0\u6587\u5b57\u5217\u3067\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u306eidentifer\u3060\u3051\u3067\u30ec\u30b3\u30fc\u30c9\u7279\u5b9a\u3067\u304d\u307e\u3059\u304c\u3001\u7279\u5b9a\u3057\u305f\u30ec\u30b3\u30fc\u30c9\u3068\u6307\u5b9a\u3057\u305fname\u3001type\u4e00\u81f4\u3057\u306a\u3044\u5834\u5408\u3001\u7279\u5b9a\u5931\u6557\u3068\u307f\u306a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/2012-12-12N2013-12-16/hostedzone/{ZoneID}/rrset"
             },
             "input": {
                 "shape": "ListResourceRecordSetsRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/endpoints.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/v1/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/v1/service-2.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874999999999999%*

 * *Differences: {"'operations'": "{'AttachDisk': {'documentation': '<p>ディスクをノードに接続します。</p>'}, "*

 * *                 "'AuthorizeFirewallGroup': {'documentation': "*

 * *                 "'<p>指定したファイアウォールグループへ許可ルールを追加します。</p><p>許可プロトコルがTCPかUDPの場合、許可ポートの指定が必要です。</p><p>ポートを単一指定する際は、許可開始ポートのみを指定します。</p><p>ポートを範囲指定する際は、許可終了ポートには許可開始ポートの値以上を指定します。</p>'}, "*

 * *                 "'CreateCluster': {'documentation': '<p>クラスターを新規作成します。</p>'}, 'CreateDisk': "*

 * *                 "{'documentation': '<p>ディスクを新規作成します。</p>'}, 'CreateFirewallGroup': "*

 * *    […]*

```diff
@@ -7,598 +7,643 @@
         "serviceFullName": "NIFCLOUD Kubernetes Service Hatoba",
         "serviceId": "hatoba",
         "signatureVersion": "v4",
         "uid": "hatoba-2019-03-27"
     },
     "operations": {
         "AttachDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u30ce\u30fc\u30c9\u306b\u63a5\u7d9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/disks/{DiskName}:attach",
                 "responseCode": 201
             },
             "input": {
                 "shape": "AttachDiskRequest"
             },
             "name": "AttachDisk",
             "output": {
                 "shape": "AttachDiskResult"
             }
         },
         "AuthorizeFirewallGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3078\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p><p>\u8a31\u53ef\u30d7\u30ed\u30c8\u30b3\u30eb\u304cTCP\u304bUDP\u306e\u5834\u5408\u3001\u8a31\u53ef\u30dd\u30fc\u30c8\u306e\u6307\u5b9a\u304c\u5fc5\u8981\u3067\u3059\u3002</p><p>\u30dd\u30fc\u30c8\u3092\u5358\u4e00\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u307f\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u30dd\u30fc\u30c8\u3092\u7bc4\u56f2\u6307\u5b9a\u3059\u308b\u969b\u306f\u3001\u8a31\u53ef\u7d42\u4e86\u30dd\u30fc\u30c8\u306b\u306f\u8a31\u53ef\u958b\u59cb\u30dd\u30fc\u30c8\u306e\u5024\u4ee5\u4e0a\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/firewallGroups/{FirewallGroupName}/rules",
                 "responseCode": 201
             },
             "input": {
                 "shape": "AuthorizeFirewallGroupRequest"
             },
             "name": "AuthorizeFirewallGroup",
             "output": {
                 "shape": "AuthorizeFirewallGroupResult"
             }
         },
         "CreateCluster": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/clusters",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateClusterRequest"
             },
             "name": "CreateCluster",
             "output": {
                 "shape": "CreateClusterResult"
             }
         },
         "CreateDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/disks",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateDiskRequest"
             },
             "name": "CreateDisk",
             "output": {
                 "shape": "CreateDiskResult"
             }
         },
         "CreateFirewallGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/firewallGroups",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateFirewallGroupRequest"
             },
             "name": "CreateFirewallGroup",
             "output": {
                 "shape": "CreateFirewallGroupResult"
             }
         },
         "CreateNodePool": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateNodePoolRequest"
             },
             "name": "CreateNodePool",
             "output": {
                 "shape": "CreateNodePoolResult"
             }
         },
         "CreateSnapshot": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/snapshots",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateSnapshotRequest"
             },
             "name": "CreateSnapshot",
             "output": {
                 "shape": "CreateSnapshotResult"
             }
         },
         "CreateTags": {
+            "documentation": "<p>\u30bf\u30b0\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30bf\u30b0\u3092\u4f5c\u6210\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/tags",
                 "responseCode": 201
             },
             "input": {
                 "shape": "CreateTagsRequest"
             },
             "name": "CreateTags",
             "output": {
                 "shape": "CreateTagsResult"
             }
         },
         "DeleteCluster": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/clusters/{ClusterName}"
             },
             "input": {
                 "shape": "DeleteClusterRequest"
             },
             "name": "DeleteCluster",
             "output": {
                 "shape": "DeleteClusterResult"
             }
         },
         "DeleteClusters": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30af\u30e9\u30b9\u30bf\u30fc\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/clusters"
             },
             "input": {
                 "shape": "DeleteClustersRequest"
             },
             "name": "DeleteClusters",
             "output": {
                 "shape": "DeleteClustersResult"
             }
         },
         "DeleteDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/disks/{DiskName}"
             },
             "input": {
                 "shape": "DeleteDiskRequest"
             },
             "name": "DeleteDisk",
             "output": {
                 "shape": "DeleteDiskResult"
             }
         },
         "DeleteDisks": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u524a\u9664\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30c7\u30a3\u30b9\u30af\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/disks"
             },
             "input": {
                 "shape": "DeleteDisksRequest"
             },
             "name": "DeleteDisks",
             "output": {
                 "shape": "DeleteDisksResult"
             }
         },
         "DeleteFirewallGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/firewallGroups/{FirewallGroupName}"
             },
             "input": {
                 "shape": "DeleteFirewallGroupRequest"
             },
             "name": "DeleteFirewallGroup",
             "output": {
                 "shape": "DeleteFirewallGroupResult"
             }
         },
         "DeleteFirewallGroups": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/firewallGroups"
             },
             "input": {
                 "shape": "DeleteFirewallGroupsRequest"
             },
             "name": "DeleteFirewallGroups",
             "output": {
                 "shape": "DeleteFirewallGroupsResult"
             }
         },
         "DeleteNodePool": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools/{NodePoolName}"
             },
             "input": {
                 "shape": "DeleteNodePoolRequest"
             },
             "name": "DeleteNodePool",
             "output": {
                 "shape": "DeleteNodePoolResult"
             }
         },
         "DeleteNodePools": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u3092\u524a\u9664\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools"
             },
             "input": {
                 "shape": "DeleteNodePoolsRequest"
             },
             "name": "DeleteNodePools",
             "output": {
                 "shape": "DeleteNodePoolsResult"
             }
         },
         "DeleteSnapshot": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/snapshots/{SnapshotName}"
             },
             "input": {
                 "shape": "DeleteSnapshotRequest"
             },
             "name": "DeleteSnapshot",
             "output": {
                 "shape": "DeleteSnapshotResult"
             }
         },
         "DeleteSnapshots": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/snapshots"
             },
             "input": {
                 "shape": "DeleteSnapshotsRequest"
             },
             "name": "DeleteSnapshots",
             "output": {
                 "shape": "DeleteSnapshotsResult"
             }
         },
         "DeleteTags": {
+            "documentation": "<p>\u30bf\u30b0\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30bf\u30b0\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/tags"
             },
             "input": {
                 "shape": "DeleteTagsRequest"
             },
             "name": "DeleteTags",
             "output": {
                 "shape": "DeleteTagsResult"
             }
         },
         "DetachDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u3092\u30ce\u30fc\u30c9\u304b\u3089\u5207\u65ad\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/disks/{DiskName}:detach",
                 "responseCode": 201
             },
             "input": {
                 "shape": "DetachDiskRequest"
             },
             "name": "DetachDisk",
             "output": {
                 "shape": "DetachDiskResult"
             }
         },
         "GetCluster": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/clusters/{ClusterName}"
             },
             "input": {
                 "shape": "GetClusterRequest"
             },
             "name": "GetCluster",
             "output": {
                 "shape": "GetClusterResult"
             }
         },
         "GetClusterCredentials": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u306ekubeconfig\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/clusters/{ClusterName}/credentials"
             },
             "input": {
                 "shape": "GetClusterCredentialsRequest"
             },
             "name": "GetClusterCredentials",
             "output": {
                 "shape": "GetClusterCredentialsResult"
             }
         },
         "GetDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/disks/{DiskName}"
             },
             "input": {
                 "shape": "GetDiskRequest"
             },
             "name": "GetDisk",
             "output": {
                 "shape": "GetDiskResult"
             }
         },
         "GetFirewallGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/firewallGroups/{FirewallGroupName}"
             },
             "input": {
                 "shape": "GetFirewallGroupRequest"
             },
             "name": "GetFirewallGroup",
             "output": {
                 "shape": "GetFirewallGroupResult"
             }
         },
         "GetLoadBalancer": {
+            "documentation": "<p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/loadBalancers/{LoadBalancerName}"
             },
             "input": {
                 "shape": "GetLoadBalancerRequest"
             },
             "name": "GetLoadBalancer",
             "output": {
                 "shape": "GetLoadBalancerResult"
             }
         },
         "GetNodePool": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools/{NodePoolName}"
             },
             "input": {
                 "shape": "GetNodePoolRequest"
             },
             "name": "GetNodePool",
             "output": {
                 "shape": "GetNodePoolResult"
             }
         },
         "GetServerConfig": {
+            "documentation": "<p>\u5229\u7528\u53ef\u80fd\u306aKubernetes\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u3092\u8fd4\u5374\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/serverConfig"
             },
             "input": {
                 "shape": "GetServerConfigRequest"
             },
             "name": "GetServerConfig",
             "output": {
                 "shape": "GetServerConfigResult"
             }
         },
         "GetSnapshot": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/snapshots/{SnapshotName}"
             },
             "input": {
                 "shape": "GetSnapshotRequest"
             },
             "name": "GetSnapshot",
             "output": {
                 "shape": "GetSnapshotResult"
             }
         },
         "ListClusters": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u306e\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8907\u6570\u306e\u30af\u30e9\u30b9\u30bf\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/clusters"
             },
             "input": {
                 "shape": "ListClustersRequest"
             },
             "name": "ListClusters",
             "output": {
                 "shape": "ListClustersResult"
             }
         },
         "ListDisks": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u306e\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8907\u6570\u306e\u30c7\u30a3\u30b9\u30af\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/disks"
             },
             "input": {
                 "shape": "ListDisksRequest"
             },
             "name": "ListDisks",
             "output": {
                 "shape": "ListDisksResult"
             }
         },
         "ListFirewallGroups": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/firewallGroups"
             },
             "input": {
                 "shape": "ListFirewallGroupsRequest"
             },
             "name": "ListFirewallGroups",
             "output": {
                 "shape": "ListFirewallGroupsResult"
             }
         },
         "ListLoadBalancers": {
+            "documentation": "<p>\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u306e\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u3001\u8907\u6570\u306e\u30ed\u30fc\u30c9\u30d0\u30e9\u30f3\u30b5\u30fc\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/loadBalancers"
             },
             "input": {
                 "shape": "ListLoadBalancersRequest"
             },
             "name": "ListLoadBalancers",
             "output": {
                 "shape": "ListLoadBalancersResult"
             }
         },
         "ListNodePools": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u306e\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools"
             },
             "input": {
                 "shape": "ListNodePoolsRequest"
             },
             "name": "ListNodePools",
             "output": {
                 "shape": "ListNodePoolsResult"
             }
         },
         "ListSnapshots": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u60c5\u5831\u306e\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/snapshots"
             },
             "input": {
                 "shape": "ListSnapshotsRequest"
             },
             "name": "ListSnapshots",
             "output": {
                 "shape": "ListSnapshotsResult"
             }
         },
         "ListTags": {
+            "documentation": "<p>\u30bf\u30b0\u306e\u60c5\u5831\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u30bf\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/v1/tags"
             },
             "input": {
                 "shape": "ListTagsRequest"
             },
             "name": "ListTags",
             "output": {
                 "shape": "ListTagsResult"
             }
         },
         "RebootNode": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u3092\u518d\u8d77\u52d5\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools/{NodePoolName}/nodes/{NodeName}:reboot",
                 "responseCode": 201
             },
             "input": {
                 "shape": "RebootNodeRequest"
             },
             "name": "RebootNode",
             "output": {
                 "shape": "RebootNodeResult"
             }
         },
         "RestoreClusterFromSnapshot": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u304b\u3089\u65b0\u3057\u3044\u30af\u30e9\u30b9\u30bf\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/snapshots/{SnapshotName}:restore",
                 "responseCode": 201
             },
             "input": {
                 "shape": "RestoreClusterFromSnapshotRequest"
             },
             "name": "RestoreClusterFromSnapshot",
             "output": {
                 "shape": "RestoreClusterFromSnapshotResult"
             }
         },
         "RevokeFirewallGroup": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305f\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u524a\u9664\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u306e\u8a31\u53ef\u30eb\u30fc\u30eb\u3092\u524a\u9664\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/v1/firewallGroups/{FirewallGroupName}/rules"
             },
             "input": {
                 "shape": "RevokeFirewallGroupRequest"
             },
             "name": "RevokeFirewallGroup",
             "output": {
                 "shape": "RevokeFirewallGroupResult"
             }
         },
         "SetNodePoolSize": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u306e\u30ce\u30fc\u30c9\u6570\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools/{NodePoolName}:setSize",
                 "responseCode": 201
             },
             "input": {
                 "shape": "SetNodePoolSizeRequest"
             },
             "name": "SetNodePoolSize",
             "output": {
                 "shape": "SetNodePoolSizeResult"
             }
         },
         "UpdateCluster": {
+            "documentation": "<p>\u30af\u30e9\u30b9\u30bf\u30fc\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/clusters/{ClusterName}"
             },
             "input": {
                 "shape": "UpdateClusterRequest"
             },
             "name": "UpdateCluster",
             "output": {
                 "shape": "UpdateClusterResult"
             }
         },
         "UpdateDisk": {
+            "documentation": "<p>\u30c7\u30a3\u30b9\u30af\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/disks/{DiskName}"
             },
             "input": {
                 "shape": "UpdateDiskRequest"
             },
             "name": "UpdateDisk",
             "output": {
                 "shape": "UpdateDiskResult"
             }
         },
         "UpdateFirewallGroup": {
+            "documentation": "<p>\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/firewallGroups/{FirewallGroupName}"
             },
             "input": {
                 "shape": "UpdateFirewallGroupRequest"
             },
             "name": "UpdateFirewallGroup",
             "output": {
                 "shape": "UpdateFirewallGroupResult"
             }
         },
         "UpdateNodePool": {
+            "documentation": "<p>\u30ce\u30fc\u30c9\u30d7\u30fc\u30eb\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/clusters/{ClusterName}/nodePools/{NodePoolName}"
             },
             "input": {
                 "shape": "UpdateNodePoolRequest"
             },
             "name": "UpdateNodePool",
             "output": {
                 "shape": "UpdateNodePoolResult"
             }
         },
         "UpdateSnapshot": {
+            "documentation": "<p>\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/snapshots/{SnapshotName}"
             },
             "input": {
                 "shape": "UpdateSnapshotRequest"
             },
             "name": "UpdateSnapshot",
             "output": {
                 "shape": "UpdateSnapshotResult"
             }
         },
         "UpdateTags": {
+            "documentation": "<p>\u30bf\u30b0\u306e\u5024\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002 1\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u8907\u6570\u30bf\u30b0\u306e\u5024\u3092\u66f4\u65b0\u53ef\u80fd\u3067\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/v1/tags"
             },
             "input": {
                 "shape": "UpdateTagsRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/hatoba/v1/waiters-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/hatoba/v1/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/nas/N2016-02-24/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/nas/N2016-02-24/service-2.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'operations'": "{'AuthorizeNASSecurityGroupIngress': {'documentation': "*

 * *                 "'<p>下記どちらかの方法でNASファイアウォールグループへの接続を許可します。</p> <ul> "*

 * *                 '<li><p>ニフクラのサーバーからのプライベートネットワーク経由でNASへアクセスしたい場合、ニフクラのファイアウォールグループからの接続を許可できます。</p></li> '*

 * *                 '<li><p>インターネット経由でNASへアクセスしたい場合、特定のIP帯からの接続を許可できます。</p></li> </ul> '*

 * *                 "<p>NASファイアウォールグループに対して、同一ゾーンのニフクラのファイアウォールグループからの接続許可は可能ですが、別ゾーンのニフクラのファイアウォールグループからの接続許可はできません。</p><p>このAPIアクションではCIDRIP（IP範囲）またはSecurityGroupName（ニフクラのファ […]*

```diff
@@ -8,181 +8,194 @@
         "serviceId": "nas",
         "signatureVersion": "v4",
         "uid": "nas-N2016-02-24",
         "xmlNamespace": "https://nas.api.nifcloud.com/"
     },
     "operations": {
         "AuthorizeNASSecurityGroupIngress": {
+            "documentation": "<p>\u4e0b\u8a18\u3069\u3061\u3089\u304b\u306e\u65b9\u6cd5\u3067NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3078\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3057\u307e\u3059\u3002</p> <ul> <li><p>\u30cb\u30d5\u30af\u30e9\u306e\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u7d4c\u7531\u3067NAS\u3078\u30a2\u30af\u30bb\u30b9\u3057\u305f\u3044\u5834\u5408\u3001\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3067\u304d\u307e\u3059\u3002</p></li> <li><p>\u30a4\u30f3\u30bf\u30fc\u30cd\u30c3\u30c8\u7d4c\u7531\u3067NAS\u3078\u30a2\u30af\u30bb\u30b9\u3057\u305f\u3044\u5834\u5408\u3001\u7279\u5b9a\u306eIP\u5e2f\u304b\u3089\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3067\u304d\u307e\u3059\u3002</p></li> </ul> <p>NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u5bfe\u3057\u3066\u3001\u540c\u4e00\u30be\u30fc\u30f3\u306e\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u8a31\u53ef\u306f\u53ef\u80fd\u3067\u3059\u304c\u3001\u5225\u30be\u30fc\u30f3\u306e\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u8a31\u53ef\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u3067\u306fCIDRIP\uff08IP\u7bc4\u56f2\uff09\u307e\u305f\u306fSecurityGroupName\uff08\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\uff09\u3092\u5fc5\u305a\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AuthorizeNASSecurityGroupIngressRequest"
             },
             "name": "AuthorizeNASSecurityGroupIngress",
             "output": {
                 "resultWrapper": "AuthorizeNASSecurityGroupIngressResult",
                 "shape": "AuthorizeNASSecurityGroupIngressResult"
             }
         },
         "ClearNASSession": {
+            "documentation": "<p>NAS\u306e\u30bb\u30c3\u30b7\u30e7\u30f3\u30af\u30ea\u30a2\u3092\u884c\u3044\u307e\u3059\u3002</p><p>NAS\u306e\u30bb\u30c3\u30b7\u30e7\u30f3\u30af\u30ea\u30a2\u3092\u884c\u3046\u3068\u901a\u4fe1\u65ad\uff08\u76ee\u5b89\uff1a5\u5206\u7a0b\u5ea6\uff09\u304c\u767a\u751f\u3057\u3001\u305d\u306e\u9593NAS\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306fclearing-session\uff08\u30bb\u30c3\u30b7\u30e7\u30f3\u30af\u30ea\u30a2\u4e2d\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ClearNASSessionRequest"
             },
             "name": "ClearNASSession",
             "output": {
                 "resultWrapper": "ClearNASSessionResult",
                 "shape": "ClearNASSessionResult"
             }
         },
         "CreateNASInstance": {
+            "documentation": "<p>NAS\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateNASInstanceRequest"
             },
             "name": "CreateNASInstance",
             "output": {
                 "resultWrapper": "CreateNASInstanceResult",
                 "shape": "CreateNASInstanceResult"
             }
         },
         "CreateNASSecurityGroup": {
+            "documentation": "<p>NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateNASSecurityGroupRequest"
             },
             "name": "CreateNASSecurityGroup",
             "output": {
                 "resultWrapper": "CreateNASSecurityGroupResult",
                 "shape": "CreateNASSecurityGroupResult"
             }
         },
         "DeleteNASInstance": {
+            "documentation": "<p>NAS\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u3053\u306e\u64cd\u4f5c\u306e\u9032\u6357\u72b6\u6cc1\u3092\u78ba\u8a8d\u3059\u308b\u306b\u306fDescribeNASInstances\u30a2\u30af\u30b7\u30e7\u30f3\u3092\u5229\u7528\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>\u3053\u306e\u30a2\u30af\u30b7\u30e7\u30f3\u306f\u4e00\u5ea6\u9001\u4fe1\u3059\u308b\u3068\u30ad\u30e3\u30f3\u30bb\u30eb\u30fb\u53d6\u308a\u6d88\u3057\u3092\u884c\u3046\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteNASInstanceRequest"
             },
             "name": "DeleteNASInstance",
             "output": {
                 "resultWrapper": "DeleteNASInstanceResult",
                 "shape": "DeleteNASInstanceResult"
             }
         },
         "DeleteNASSecurityGroup": {
+            "documentation": "<p>NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>NAS\u306b\u9069\u7528\u3055\u308c\u305f\u72b6\u614b\u306eNAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteNASSecurityGroupRequest"
             },
             "name": "DeleteNASSecurityGroup",
             "output": {
                 "shape": "DeleteNASSecurityGroupResult"
             }
         },
         "DescribeNASInstances": {
+            "documentation": "<p>NAS\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeNASInstancesRequest"
             },
             "name": "DescribeNASInstances",
             "output": {
                 "resultWrapper": "DescribeNASInstancesResult",
                 "shape": "DescribeNASInstancesResult"
             }
         },
         "DescribeNASSecurityGroups": {
+            "documentation": "<p>NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>NASSecurityGroupName\uff08NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\uff09\u304c\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u8a72\u5f53\u3059\u308bNAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u306e\u307f\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeNASSecurityGroupsRequest"
             },
             "name": "DescribeNASSecurityGroups",
             "output": {
                 "resultWrapper": "DescribeNASSecurityGroupsResult",
                 "shape": "DescribeNASSecurityGroupsResult"
             }
         },
         "GetMetricStatistics": {
+            "documentation": "<p>NAS\u30b5\u30fc\u30d3\u30b9\u306e\u30e2\u30cb\u30bf\u30ea\u30f3\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30e2\u30cb\u30bf\u30ea\u30f3\u30b0\u8981\u7d20\u306b\u3064\u3044\u3066\u3001\u8a73\u3057\u304f\u306f\u4e0b\u8a18\u30d8\u30eb\u30d7\u30da\u30fc\u30b8\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p><p><a href=\"https://docs.nifcloud.com/nas/help/monitoring.htm\">\u30d8\u30eb\u30d7\uff1aNAS\uff1a\u30e2\u30cb\u30bf\u30ea\u30f3\u30b0</a></p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetMetricStatisticsRequest"
             },
             "name": "GetMetricStatistics",
             "output": {
                 "resultWrapper": "GetMetricStatisticsResult",
                 "shape": "GetMetricStatisticsResult"
             }
         },
         "ModifyNASInstance": {
+            "documentation": "<p>NAS\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u4e00\u5ea6\u306b\u8907\u6570\u306eNAS\u8a2d\u5b9a\u3092\u5909\u66f4\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p><p>NAS\u306b\u63a5\u7d9a\u3057\u305f\u72b6\u614b\u3067\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8IP\u30a2\u30c9\u30ec\u30b9\u3092\u5909\u66f4\u3059\u308b\u3068\u3001NAS\u306b\u30a2\u30af\u30bb\u30b9\u3067\u304d\u306a\u304f\u306a\u308b\u5834\u5408\u304c\u3042\u308a\u307e\u3059\u3002</p><p>NAS\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8IP\u30a2\u30c9\u30ec\u30b9\u3092\u5909\u66f4\u3059\u308b\u5834\u5408\u306f\u3001NAS\u3078\u306e\u63a5\u7d9a\u304c\u306a\u3044\u3053\u3068\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p><p>NAS\u306b\u30a2\u30af\u30bb\u30b9\u3067\u304d\u306a\u304f\u306a\u3063\u305f\u5834\u5408\u306f\u3001\u30af\u30e9\u30a4\u30a2\u30f3\u30c8\u5074\u306eOS\u5f37\u5236\u518d\u8d77\u52d5\u3092\u884c\u3063\u3066\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyNASInstanceRequest"
             },
             "name": "ModifyNASInstance",
             "output": {
                 "resultWrapper": "ModifyNASInstanceResult",
                 "shape": "ModifyNASInstanceResult"
             }
         },
         "ModifyNASSecurityGroup": {
+            "documentation": "<p>NAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u4e00\u5ea6\u306b\u8907\u6570\u306eNAS\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyNASSecurityGroupRequest"
             },
             "name": "ModifyNASSecurityGroup",
             "output": {
                 "resultWrapper": "ModifyNASSecurityGroupResult",
                 "shape": "ModifyNASSecurityGroupResult"
             }
         },
         "RevokeNASSecurityGroupIngress": {
+            "documentation": "<p>\u63a5\u7d9a\u3092\u8a31\u53ef\u3057\u305fIP\u7bc4\u56f2\u307e\u305f\u306f\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u306e\u8a2d\u5b9a\u3092\u53d6\u308a\u6d88\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u3067\u306fCIDRIP\uff08IP\u5e2f\uff09\u307e\u305f\u306fSecurityGroupName\uff08\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\uff09\u3092\u5fc5\u305a\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RevokeNASSecurityGroupIngressRequest"
             },
             "name": "RevokeNASSecurityGroupIngress",
             "output": {
                 "resultWrapper": "RevokeNASSecurityGroupIngressResult",
                 "shape": "RevokeNASSecurityGroupIngressResult"
             }
         },
         "UpgradeNASInstance": {
+            "documentation": "<p>NAS\u306e\u57fa\u76e4\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u3092\u884c\u3044\u307e\u3059\u3002</p><p>NAS\u306e\u57fa\u76e4\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u4e2d\u306fNAS\u306b\u63a5\u7d9a\u3067\u304d\u306a\u3044\u72b6\u614b\u3068\u306a\u308a\u3001\u305d\u306e\u9593\u306eNAS\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306fupgrading\uff08\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u4e2d\uff09\u3068\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "UpgradeNASInstanceRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874999999999999%*

 * *Differences: {"'operations'": "{'AddSourceIdentifierToSubscription': {'documentation': "*

 * *                 "'<p>イベントサブスクリプションにリソースIDを追加します。</p>'}, 'AuthorizeDBSecurityGroupIngress': "*

 * *                 "{'documentation': '<p>下記どちらかの方法でDBファイアウォールグループへの接続を許可します。</p> <ul> "*

 * *                 '<li><p>ニフクラのサーバーからのプライベートネットワーク経由でDBサーバーへアクセスしたい場合、ニフクラのファイアウォールグループからの接続を許可できます。</p></li> '*

 * *                 '<li><p>インターネット経由でDBサーバーへアクセスしたい場合、特定のIP帯からの接続を許可できます。</p></li> </ul> '*

 * *                 "<p>DBファイアウォールグループに対して、同一ゾーンのニフクラのファイア […]*

```diff
@@ -8,614 +8,658 @@
         "serviceId": "rdb",
         "signatureVersion": "v4",
         "uid": "rdb-2013-05-15N2013-12-16",
         "xmlNamespace": "https://rdb.api.nifcloud.com/"
     },
     "operations": {
         "AddSourceIdentifierToSubscription": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u306b\u30ea\u30bd\u30fc\u30b9ID\u3092\u8ffd\u52a0\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AddSourceIdentifierToSubscriptionRequest"
             },
             "name": "AddSourceIdentifierToSubscription",
             "output": {
                 "resultWrapper": "AddSourceIdentifierToSubscriptionResult",
                 "shape": "AddSourceIdentifierToSubscriptionResult"
             }
         },
         "AuthorizeDBSecurityGroupIngress": {
+            "documentation": "<p>\u4e0b\u8a18\u3069\u3061\u3089\u304b\u306e\u65b9\u6cd5\u3067DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3078\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3057\u307e\u3059\u3002</p> <ul> <li><p>\u30cb\u30d5\u30af\u30e9\u306e\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u7d4c\u7531\u3067DB\u30b5\u30fc\u30d0\u30fc\u3078\u30a2\u30af\u30bb\u30b9\u3057\u305f\u3044\u5834\u5408\u3001\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3067\u304d\u307e\u3059\u3002</p></li> <li><p>\u30a4\u30f3\u30bf\u30fc\u30cd\u30c3\u30c8\u7d4c\u7531\u3067DB\u30b5\u30fc\u30d0\u30fc\u3078\u30a2\u30af\u30bb\u30b9\u3057\u305f\u3044\u5834\u5408\u3001\u7279\u5b9a\u306eIP\u5e2f\u304b\u3089\u306e\u63a5\u7d9a\u3092\u8a31\u53ef\u3067\u304d\u307e\u3059\u3002</p></li> </ul> <p>DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306b\u5bfe\u3057\u3066\u3001\u540c\u4e00\u30be\u30fc\u30f3\u306e\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u8a31\u53ef\u306f\u53ef\u80fd\u3067\u3059\u304c\u3001\u5225\u30be\u30fc\u30f3\u306e\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u306e\u63a5\u7d9a\u8a31\u53ef\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u3067\u306fCIDRIP\uff08IP\u7bc4\u56f2\uff09\u307e\u305f\u306fEC2SecurityGroupName\uff08\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\uff09\u3092\u5fc5\u305a\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AuthorizeDBSecurityGroupIngressRequest"
             },
             "name": "AuthorizeDBSecurityGroupIngress",
             "output": {
                 "resultWrapper": "AuthorizeDBSecurityGroupIngressResult",
                 "shape": "AuthorizeDBSecurityGroupIngressResult"
             }
         },
         "CopyDBSnapshot": {
+            "documentation": "<p>DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u30b3\u30d4\u30fc\u3057\u307e\u3059\u3002</p><p>\u30b3\u30d4\u30fc\u5143\u306eDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306f\u30b9\u30c6\u30fc\u30bf\u30b9\u304c\u201davailable\u201d\u3067\u306a\u3051\u308c\u3070\u306a\u308a\u307e\u305b\u3093\u3002</p><p>\u81ea\u52d5\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u6a5f\u80fd\u3067\u4f5c\u6210\u3055\u308c\u305fDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u307f\u30b3\u30d4\u30fc\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CopyDBSnapshotRequest"
             },
             "name": "CopyDBSnapshot",
             "output": {
                 "resultWrapper": "CopyDBSnapshotResult",
                 "shape": "CopyDBSnapshotResult"
             }
         },
         "CreateDBInstance": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateDBInstanceRequest"
             },
             "name": "CreateDBInstance",
             "output": {
                 "resultWrapper": "CreateDBInstanceResult",
                 "shape": "CreateDBInstanceResult"
             }
         },
         "CreateDBInstanceReadReplica": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u30ea\u30fc\u30c9\u30ec\u30d7\u30ea\u30ab\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u3059\u3079\u3066\u306e\u30ea\u30fc\u30c9\u30ec\u30d7\u30ea\u30ab\u306f\u5197\u9577\u5316\u6a5f\u80fd\u7121\u52b9\u30fb\u81ea\u52d5\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u7121\u52b9\u3067\u4f5c\u6210\u3055\u308c\u307e\u3059\u3002</p><p>\u30ea\u30af\u30a8\u30b9\u30c8\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3067\u6307\u5b9a\u3057\u305f\u3082\u306e\u4ee5\u5916\u306e\u5c5e\u6027\u306f\u3001\u4f5c\u6210\u5143\u306eDB\u30b5\u30fc\u30d0\u30fc\u304b\u3089\u7d99\u627f\u3055\u308c\u307e\u3059\u3002</p><p>[\u91cd\u8981]</p><p>\u4f5c\u6210\u5143\u306eDB\u30b5\u30fc\u30d0\u30fc\u306f\u81ea\u52d5\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u304c\u6709\u52b9\u3067\u306a\u3051\u308c\u3070\u306a\u308a\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateDBInstanceReadReplicaRequest"
             },
             "name": "CreateDBInstanceReadReplica",
             "output": {
                 "resultWrapper": "CreateDBInstanceReadReplicaResult",
                 "shape": "CreateDBInstanceReadReplicaResult"
             }
         },
         "CreateDBParameterGroup": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306e\u5024\u3092\u30ab\u30b9\u30bf\u30de\u30a4\u30ba\u3057\u305f\u3044\u5834\u5408\u306b\u306f\u3001ModifyDBParameterGroup\u3092\u4f7f\u3044\u307e\u3059\u3002</p><p>\u8d77\u52d5\u3057\u3066\u3044\u308bDB\u30b5\u30fc\u30d0\u30fc\u3078\u65b0\u3057\u3044DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u9069\u7528\u3057\u305f\u3044\u5834\u5408\u306b\u306f\u3001DB\u30b5\u30fc\u30d0\u30fc\u306e\u518d\u8d77\u52d5\u304c\u5fc5\u8981\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateDBParameterGroupRequest"
             },
             "name": "CreateDBParameterGroup",
             "output": {
                 "resultWrapper": "CreateDBParameterGroupResult",
                 "shape": "CreateDBParameterGroupResult"
             }
         },
         "CreateDBSecurityGroup": {
+            "documentation": "<p>DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateDBSecurityGroupRequest"
             },
             "name": "CreateDBSecurityGroup",
             "output": {
                 "resultWrapper": "CreateDBSecurityGroupResult",
                 "shape": "CreateDBSecurityGroupResult"
             }
         },
         "CreateDBSnapshot": {
+            "documentation": "<p>DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u4f5c\u6210\u5143\u3068\u306a\u308bDB\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u201davailable\u201d\u3067\u306a\u3051\u308c\u3070\u306a\u308a\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateDBSnapshotRequest"
             },
             "name": "CreateDBSnapshot",
             "output": {
                 "resultWrapper": "CreateDBSnapshotResult",
                 "shape": "CreateDBSnapshotResult"
             }
         },
         "CreateEventSubscription": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u3092\u65b0\u898f\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateEventSubscriptionRequest"
             },
             "name": "CreateEventSubscription",
             "output": {
                 "resultWrapper": "CreateEventSubscriptionResult",
                 "shape": "CreateEventSubscriptionResult"
             }
         },
         "DeleteDBInstance": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u6210\u529f\u3057\u305f\u30ec\u30b9\u30dd\u30f3\u30b9\u306f\u30ea\u30af\u30a8\u30b9\u30c8\u304c\u6b63\u3057\u304f\u53d7\u3051\u53d6\u3089\u308c\u305f\u3053\u3068\u3092\u8868\u3057\u307e\u3059\u3002</p><p>DB\u30b5\u30fc\u30d0\u30fc\u3092\u524a\u9664\u3059\u308b\u3068\u3001\u81ea\u52d5\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u6a5f\u80fd\u3067\u4f5c\u6210\u3055\u308c\u305f\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u3082\u524a\u9664\u3055\u308c\u5fa9\u5143\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u306a\u304f\u306a\u308a\u307e\u3059\u3002</p><p>\u624b\u52d5\u3067\u4f5c\u6210\u3057\u305fDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306f\u524a\u9664\u3055\u308c\u307e\u305b\u3093\u3002</p><p>\u524a\u9664\u524d\u306b\u6700\u5f8c\u306eDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u4f5c\u6210\u3059\u308b\u3053\u3068\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u3001DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u304c\u4f5c\u6210\u3055\u308c\u308b\u307e\u3067DB\u30b5\u30fc\u30d0\u30fc\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306fdeleting(\u524a\u9664\u4e2d)\u306b\u306a\u308a\u307e\u3059\u3002</p><p>\u3053\u306e\u64cd\u4f5c\u306e\u9032\u6357\u72b6\u6cc1\u3092\u78ba\u8a8d\u3059\u308b\u306b\u306fDescribeDBInstance\u30a2\u30af\u30b7\u30e7\u30f3\u3092\u5229\u7528\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p><p>\u3053\u306e\u30a2\u30af\u30b7\u30e7\u30f3\u306f\u4e00\u5ea6\u9001\u4fe1\u3059\u308b\u3068\u30ad\u30e3\u30f3\u30bb\u30eb\u30fb\u53d6\u308a\u6d88\u3057\u3092\u884c\u3046\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteDBInstanceRequest"
             },
             "name": "DeleteDBInstance",
             "output": {
                 "resultWrapper": "DeleteDBInstanceResult",
                 "shape": "DeleteDBInstanceResult"
             }
         },
         "DeleteDBParameterGroup": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>DB\u30b5\u30fc\u30d0\u30fc\u306b\u7d10\u3065\u3044\u3066\u3044\u308bDB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteDBParameterGroupRequest"
             },
             "name": "DeleteDBParameterGroup",
             "output": {
                 "shape": "DeleteDBParameterGroupResult"
             }
         },
         "DeleteDBSecurityGroup": {
+            "documentation": "<p>DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>DB\u30b5\u30fc\u30d0\u30fc\u306b\u9069\u7528\u3055\u308c\u305f\u72b6\u614b\u306eDB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u3092\u524a\u9664\u3059\u308b\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteDBSecurityGroupRequest"
             },
             "name": "DeleteDBSecurityGroup",
             "output": {
                 "shape": "DeleteDBSecurityGroupResult"
             }
         },
         "DeleteDBSnapshot": {
+            "documentation": "<p>DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u624b\u52d5\u4f5c\u6210\u3057\u305fDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u307f\u524a\u9664\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u3055\u3089\u306b\u3001DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u30b9\u30c6\u30fc\u30bf\u30b9\u306f\u201davailable\u201d\u307e\u305f\u306f\u201dfailed\u201d\u3067\u306a\u3051\u308c\u3070\u306a\u308a\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteDBSnapshotRequest"
             },
             "name": "DeleteDBSnapshot",
             "output": {
                 "resultWrapper": "DeleteDBSnapshotResult",
                 "shape": "DeleteDBSnapshotResult"
             }
         },
         "DeleteEventSubscription": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteEventSubscriptionRequest"
             },
             "name": "DeleteEventSubscription",
             "output": {
                 "resultWrapper": "DeleteEventSubscriptionResult",
                 "shape": "DeleteEventSubscriptionResult"
             }
         },
         "DescribeCertificates": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u306b\u9069\u7528\u3067\u304d\u308bCA\u8a3c\u660e\u66f8\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u306f\u30da\u30fc\u30b8\u30cd\u30fc\u30c8\u3092\u30b5\u30dd\u30fc\u30c8\u3057\u3066\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeCertificatesRequest"
             },
             "name": "DescribeCertificates",
             "output": {
                 "resultWrapper": "DescribeCertificatesResult",
                 "shape": "DescribeCertificatesResult"
             }
         },
         "DescribeDBEngineVersions": {
+            "documentation": "<p>\u30c7\u30fc\u30bf\u30d9\u30fc\u30b9\u30a8\u30f3\u30b8\u30f3\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBEngineVersionsRequest"
             },
             "name": "DescribeDBEngineVersions",
             "output": {
                 "resultWrapper": "DescribeDBEngineVersionsResult",
                 "shape": "DescribeDBEngineVersionsResult"
             }
         },
         "DescribeDBInstances": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u306f\u30da\u30fc\u30b8\u30cd\u30fc\u30c8\u3092\u30b5\u30dd\u30fc\u30c8\u3057\u3066\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBInstancesRequest"
             },
             "name": "DescribeDBInstances",
             "output": {
                 "resultWrapper": "DescribeDBInstancesResult",
                 "shape": "DescribeDBInstancesResult"
             }
         },
         "DescribeDBLogFiles": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u5185\u306e\u30ed\u30b0\u30d5\u30a1\u30a4\u30eb\u306e\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBLogFilesRequest"
             },
             "name": "DescribeDBLogFiles",
             "output": {
                 "resultWrapper": "DescribeDBLogFilesResult",
                 "shape": "DescribeDBLogFilesResult"
             }
         },
         "DescribeDBParameterGroups": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>DBParameterGroupName(DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u540d)\u3092\u6307\u5b9a\u3057\u305f\u5834\u5408\u306b\u306f\u3001\u8a72\u5f53\u3059\u308bDB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u306e\u307f\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBParameterGroupsRequest"
             },
             "name": "DescribeDBParameterGroups",
             "output": {
                 "resultWrapper": "DescribeDBParameterGroupsResult",
                 "shape": "DescribeDBParameterGroupsResult"
             }
         },
         "DescribeDBParameters": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u304b\u3089\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBParametersRequest"
             },
             "name": "DescribeDBParameters",
             "output": {
                 "resultWrapper": "DescribeDBParametersResult",
                 "shape": "DescribeDBParametersResult"
             }
         },
         "DescribeDBSecurityGroups": {
+            "documentation": "<p>DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>DBSecurityGroupName(DB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d)\u304c\u6307\u5b9a\u3055\u308c\u305f\u5834\u5408\u306f\u8a72\u5f53\u3059\u308bDB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u306e\u60c5\u5831\u306e\u307f\u304c\u8fd4\u5374\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBSecurityGroupsRequest"
             },
             "name": "DescribeDBSecurityGroups",
             "output": {
                 "resultWrapper": "DescribeDBSecurityGroupsResult",
                 "shape": "DescribeDBSecurityGroupsResult"
             }
         },
         "DescribeDBSnapshots": {
+            "documentation": "<p>DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u306f\u30da\u30fc\u30b8\u30cd\u30fc\u30c8\u3092\u30b5\u30dd\u30fc\u30c8\u3057\u3066\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeDBSnapshotsRequest"
             },
             "name": "DescribeDBSnapshots",
             "output": {
                 "resultWrapper": "DescribeDBSnapshotsResult",
                 "shape": "DescribeDBSnapshotsResult"
             }
         },
         "DescribeEngineDefaultParameters": {
+            "documentation": "<p>\u6307\u5b9a\u3057\u305fDB\u30a8\u30f3\u30b8\u30f3\u306e\u30c7\u30d5\u30a9\u30eb\u30c8\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeEngineDefaultParametersRequest"
             },
             "name": "DescribeEngineDefaultParameters",
             "output": {
                 "resultWrapper": "DescribeEngineDefaultParametersResult",
                 "shape": "DescribeEngineDefaultParametersResult"
             }
         },
         "DescribeEventCategories": {
+            "documentation": "<p>\u5404\u30ea\u30bd\u30fc\u30b9\u30bf\u30a4\u30d7\u306b\u5bfe\u3059\u308b\u30a4\u30d9\u30f3\u30c8\u30ab\u30c6\u30b4\u30ea\u306e\u4e00\u89a7\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeEventCategoriesRequest"
             },
             "name": "DescribeEventCategories",
             "output": {
                 "resultWrapper": "DescribeEventCategoriesResult",
                 "shape": "DescribeEventCategoriesResult"
             }
         },
         "DescribeEventSubscriptions": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeEventSubscriptionsRequest"
             },
             "name": "DescribeEventSubscriptions",
             "output": {
                 "resultWrapper": "DescribeEventSubscriptionsResult",
                 "shape": "DescribeEventSubscriptionsResult"
             }
         },
         "DescribeEvents": {
+            "documentation": "<p>\u904e\u53bb14\u65e5\u306eDB\u30b5\u30fc\u30d0\u30fc\u30fbDB\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u30fbDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u30fbDB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306b\u95a2\u3059\u308b\u30a4\u30d9\u30f3\u30c8\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u7279\u5b9a\u306e\u30ea\u30bd\u30fc\u30b9\u306b\u3064\u3044\u3066\u306e\u30a4\u30d9\u30f3\u30c8\u60c5\u5831\u3092\u53d6\u5f97\u3059\u308b\u306b\u306f\u5bfe\u8c61\u306eSourceIdentifier(\u30ea\u30bd\u30fc\u30b9\u540d)\u3068SourceType(\u30ea\u30bd\u30fc\u30b9\u30bf\u30a4\u30d7)\u3092\u6307\u5b9a\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeEventsRequest"
             },
             "name": "DescribeEvents",
             "output": {
                 "resultWrapper": "DescribeEventsResult",
                 "shape": "DescribeEventsResult"
             }
         },
         "DescribeOrderableDBInstanceOptions": {
+            "documentation": "<p>\u7279\u5b9a\u306e\u30a8\u30f3\u30b8\u30f3\u306b\u7d10\u3065\u304fDB\u30b5\u30fc\u30d0\u30fc\u30aa\u30d7\u30b7\u30e7\u30f3\u306e\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeOrderableDBInstanceOptionsRequest"
             },
             "name": "DescribeOrderableDBInstanceOptions",
             "output": {
                 "resultWrapper": "DescribeOrderableDBInstanceOptionsResult",
                 "shape": "DescribeOrderableDBInstanceOptionsResult"
             }
         },
         "DownloadDBLogFilePortion": {
+            "documentation": "<p>\u7279\u5b9a\u306e\u30ed\u30b0\u30d5\u30a1\u30a4\u30eb\u306e\u6700\u65b0\u884c\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DownloadDBLogFilePortionRequest"
             },
             "name": "DownloadDBLogFilePortion",
             "output": {
                 "resultWrapper": "DownloadDBLogFilePortionResult",
                 "shape": "DownloadDBLogFilePortionResult"
             }
         },
         "ModifyDBInstance": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u306e\u8a2d\u5b9a\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p><p>\u4e00\u5ea6\u306b\u8907\u6570\u306eDB\u8a2d\u5b9a\u3092\u5909\u66f4\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u4e00\u90e8\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306f\u3001ApplyImmediately\u3092false\u306b\u6307\u5b9a\u3057\u3066\u3082\u300c\u4eca\u3059\u3050\u300d\u9069\u7528\u3055\u308c\u308b\u3053\u3068\u306b\u3054\u6ce8\u610f\u304f\u3060\u3055\u3044\u3002</p><p>\u307e\u305f\u3001\u8a2d\u5b9a\u5909\u66f4\u5185\u5bb9\u306b\u3088\u3063\u3066\u306fIO\u6027\u80fd\u4f4e\u4e0b\u30fbDB\u30b5\u30fc\u30d0\u30fc\u505c\u6b62\u30fbDB\u30b5\u30fc\u30d3\u30b9\u505c\u6b62\u3092\u4f34\u3046\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u8a73\u3057\u304f\u306f\u30e6\u30fc\u30b6\u30ac\u30a4\u30c9\u3068RDB\u6280\u8853\u4ed5\u69d8/\u5236\u9650\u5024\u3092\u53c2\u7167\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p> <ul> <li><a href=\"https://docs.nifcloud.com/rdb/guide/server_change.htm\">DB\u30b5\u30fc\u30d0\u30fc\u306e\u8a2d\u5b9a\u5909\u66f4</a></li> <li><a href=\"https://docs.nifcloud.com/rdb/spec/server_maintenance.htm\">\u30e1\u30f3\u30c6\u30ca\u30f3\u30b9</a></li> </ul>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyDBInstanceRequest"
             },
             "name": "ModifyDBInstance",
             "output": {
                 "resultWrapper": "ModifyDBInstanceResult",
                 "shape": "ModifyDBInstanceResult"
             }
         },
         "ModifyDBInstanceNetwork": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u306e\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8LAN\u30fb\u30d7\u30e9\u30a4\u30d9\u30fc\u30c8IP\u30a2\u30c9\u30ec\u30b9\u3092\u5909\u66f4\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyDBInstanceNetworkRequest"
             },
             "name": "ModifyDBInstanceNetwork",
             "output": {
                 "resultWrapper": "ModifyDBInstanceNetworkResult",
                 "shape": "ModifyDBInstanceNetworkResult"
             }
         },
         "ModifyDBParameterGroup": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u6700\u592720\u500b\u306eDB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30921\u56de\u306e\u30ea\u30af\u30a8\u30b9\u30c8\u3067\u5909\u66f4\u3067\u304d\u307e\u3059\u3002</p><p>\u9069\u7528\u65b9\u6cd5\u306b\u306fapply-immediate(\u4eca\u3059\u3050)\u3068pending-reboot(\u518d\u8d77\u52d5\u5f85\u3061)\u306e2\u7a2e\u985e\u304c\u3042\u308a\u307e\u3059\u3002</p><p>apply-immediate\u306fdynamic\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306b\u306e\u307f\u5229\u7528\u3067\u304d\u307e\u3059\u3002</p><p>pending-reboot\u306fMySQL\u3001PostgreSQL\u30a8\u30f3\u30b8\u30f3\u306e\u5834\u5408\u306fdynamic\u30fbstatic\u4e21\u65b9\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306b\u5229\u7528\u3067\u304d\u307e\u3059\u3002</p><p>PostgreSQL \u30a8\u30f3\u30b8\u30f3\u306e\u5834\u5408\u3001pending-reboot\u3092\u6307\u5b9a\u3057\u3066\u3082\u3001dynamic\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306f\u5373\u6642\u53cd\u6620\uff08apply-immediate\u3068\u540c\u3058\u52d5\u4f5c\uff09\u306b\u306a\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyDBParameterGroupRequest"
             },
             "name": "ModifyDBParameterGroup",
             "output": {
                 "resultWrapper": "ModifyDBParameterGroupResult",
                 "shape": "ModifyDBParameterGroupResult"
             }
         },
         "ModifyEventSubscription": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u3067\u306f\u3001\u30ea\u30bd\u30fc\u30b9ID\u306e\u5909\u66f4\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u30ea\u30bd\u30fc\u30b9ID\u306e\u5909\u66f4\u3092\u884c\u3046\u306b\u306f AddSourceIdentifierToSubscription\u3001RemoveSourceIdentifierFromSubscription\u3092\u4f7f\u7528\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ModifyEventSubscriptionRequest"
             },
             "name": "ModifyEventSubscription",
             "output": {
                 "resultWrapper": "ModifyEventSubscriptionResult",
                 "shape": "ModifyEventSubscriptionResult"
             }
         },
         "NiftyGetMetricStatistics": {
+            "documentation": "<p>RDB\u30b5\u30fc\u30d3\u30b9\u306e\u30e2\u30cb\u30bf\u30ea\u30f3\u30b0\u60c5\u5831\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p><p>\u30e2\u30cb\u30bf\u30ea\u30f3\u30b0\u8981\u7d20\u306b\u3064\u3044\u3066\u3001\u8a73\u3057\u304f\u306f\u4e0b\u8a18\u30d8\u30eb\u30d7\u30da\u30fc\u30b8\u3092\u3054\u78ba\u8a8d\u304f\u3060\u3055\u3044\u3002</p><p><a href=\"https://docs.nifcloud.com/rdb/help/monitoring.htm\">\u30d8\u30eb\u30d7\uff1aRDB : \u30e2\u30cb\u30bf\u30ea\u30f3\u30b0</a></p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "NiftyGetMetricStatisticsRequest"
             },
             "name": "NiftyGetMetricStatistics",
             "output": {
                 "resultWrapper": "NiftyGetMetricStatisticsResult",
                 "shape": "NiftyGetMetricStatisticsResult"
             }
         },
         "RebootDBInstance": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u3092\u518d\u8d77\u52d5\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u306fDB\u30b5\u30fc\u30d0\u30fc\u306b\u9069\u7528\u3055\u308c\u3066\u3044\u308bDB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306e\u4e2d\u3067\u3001ApplyStatus(\u9069\u7528\u72b6\u6cc1)\u304cpending-reboot(\u518d\u8d77\u52d5\u5f85\u3061)\u3068\u306a\u3063\u3066\u3044\u308b\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u66f4\u65b0\u3057\u307e\u3059\u3002</p><p>DB\u30b5\u30fc\u30d0\u30fc\u3092\u518d\u8d77\u52d5\u3059\u308b\u3068\u5c11\u3057\u306e\u9593DB\u30b5\u30fc\u30d0\u30fc\u306f\u6a5f\u80fd\u505c\u6b62\u3057\u3001\u305d\u306e\u9593\u30b9\u30c6\u30fc\u30bf\u30b9\u306frebooting(\u518d\u8d77\u52d5\u4e2d)\u3068\u306a\u308a\u307e\u3059\u3002</p><p>DB\u30b5\u30fc\u30d0\u30fc\u306e\u5197\u9577\u5316\u6a5f\u80fd\u304c\u6709\u52b9\u306e\u5834\u5408\u306b\u306f\u3001\u5f37\u5236\u7684\u306b\u30d5\u30a7\u30a4\u30eb\u30aa\u30fc\u30d0\u30fc\u3055\u305b\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RebootDBInstanceRequest"
             },
             "name": "RebootDBInstance",
             "output": {
                 "resultWrapper": "RebootDBInstanceResult",
                 "shape": "RebootDBInstanceResult"
             }
         },
         "RemoveSourceIdentifierFromSubscription": {
+            "documentation": "<p>\u30a4\u30d9\u30f3\u30c8\u30b5\u30d6\u30b9\u30af\u30ea\u30d7\u30b7\u30e7\u30f3\u304b\u3089\u30ea\u30bd\u30fc\u30b9ID\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RemoveSourceIdentifierFromSubscriptionRequest"
             },
             "name": "RemoveSourceIdentifierFromSubscription",
             "output": {
                 "resultWrapper": "RemoveSourceIdentifierFromSubscriptionResult",
                 "shape": "RemoveSourceIdentifierFromSubscriptionResult"
             }
         },
         "ResetDBParameterGroup": {
+            "documentation": "<p>DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u30c7\u30d5\u30a9\u30eb\u30c8\u5024\u306b\u30ea\u30bb\u30c3\u30c8\u3057\u307e\u3059\u3002</p><p>\u7279\u5b9a\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u30ea\u30bb\u30c3\u30c8\u3059\u308b\u306b\u306fParameterName(\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u540d)\u3068ApplyMethod(\u9069\u7528\u65b9\u6cd5)\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u3059\u3079\u3066\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u30ea\u30bb\u30c3\u30c8\u3059\u308b\u306b\u306f\u3001DBParameterGroupName(DB\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u30b0\u30eb\u30fc\u30d7\u540d)\u3068ResetAllParameters(\u3059\u3079\u3066\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u3092\u30ea\u30bb\u30c3\u30c8\u3059\u308b\u30d5\u30e9\u30b0)\u3092\u6307\u5b9a\u3057\u307e\u3059\u3002</p><p>\u3059\u3079\u3066\u306e\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u3092\u30ea\u30bb\u30c3\u30c8\u3059\u308b\u5834\u5408\u3001dynamic\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306f\u305f\u3060\u3061\u306b\u9069\u7528\u3055\u308c\u307e\u3059\u304c\u3001static\u30d1\u30e9\u30e1\u30fc\u30bf\u30fc\u306f\u30b9\u30c6\u30fc\u30bf\u30b9\u304cpending-reboot(\u518d\u8d77\u52d5\u5f85\u3061)\u306b\u5909\u308f\u308a\u3001DB\u30b5\u30fc\u30d0\u30fc\u304c\u518d\u8d77\u52d5\u3055\u308c\u308b\u304bRebootInstance\u30a2\u30af\u30b7\u30e7\u30f3\u304c\u547c\u3073\u51fa\u3055\u308c\u305f\u3068\u304d\u306b\u9069\u7528\u304c\u884c\u308f\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ResetDBParameterGroupRequest"
             },
             "name": "ResetDBParameterGroup",
             "output": {
                 "resultWrapper": "ResetDBParameterGroupResult",
                 "shape": "ResetDBParameterGroupResult"
             }
         },
         "ResetExternalMaster": {
+            "documentation": "<p>\u5916\u90e8\u30ec\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u3092\u89e3\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ResetExternalMasterRequest"
             },
             "name": "ResetExternalMaster",
             "output": {
                 "resultWrapper": "ResetExternalMasterResult",
                 "shape": "ResetExternalMasterResult"
             }
         },
         "RestoreDBInstanceFromDBSnapshot": {
+            "documentation": "<p>DB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u304b\u3089\u65b0\u3057\u3044DB\u30b5\u30fc\u30d0\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u5143\u306eDB\u30b5\u30fc\u30d0\u30fc\u3068\u307b\u307c\u540c\u3058\u8a2d\u5b9a\u3067DB\u30b5\u30fc\u30d0\u30fc\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u304c\u3001\u7570\u306a\u308b\u8a2d\u5b9a\u3092\u9069\u7528\u3059\u308b\u3053\u3068\u3082\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RestoreDBInstanceFromDBSnapshotRequest"
             },
             "name": "RestoreDBInstanceFromDBSnapshot",
             "output": {
                 "resultWrapper": "RestoreDBInstanceFromDBSnapshotResult",
                 "shape": "RestoreDBInstanceFromDBSnapshotResult"
             }
         },
         "RestoreDBInstanceToPointInTime": {
+            "documentation": "<p>\u65e2\u5b58\u306eDB\u30b5\u30fc\u30d0\u30fc\u306e\u3042\u308b\u65e5\u6642\u306e\u72b6\u614b\u304b\u3089\u65b0\u3057\u3044DB\u30b5\u30fc\u30d0\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p><p>\u6700\u65b0\u306e\u30ea\u30b9\u30c8\u30a2\u53ef\u80fd\u6642\u9593\u304b\u3089\u30d0\u30c3\u30af\u30a2\u30c3\u30d7\u4fdd\u6301\u671f\u9593\u307e\u3067\u306e\u72b6\u614b\u306b\u30ea\u30b9\u30c8\u30a2\u3059\u308b\u3053\u3068\u304c\u3067\u304d\u307e\u3059\u3002</p><p>\u5143\u306eDB\u30b5\u30fc\u30d0\u30fc\u3068\u307b\u307c\u540c\u3058\u8a2d\u5b9a\u3067DB\u30b5\u30fc\u30d0\u30fc\u304c\u4f5c\u6210\u3055\u308c\u307e\u3059\u304c\u3001\u7570\u306a\u308b\u8a2d\u5b9a\u3092\u9069\u7528\u3059\u308b\u3053\u3068\u3082\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RestoreDBInstanceToPointInTimeRequest"
             },
             "name": "RestoreDBInstanceToPointInTime",
             "output": {
                 "resultWrapper": "RestoreDBInstanceToPointInTimeResult",
                 "shape": "RestoreDBInstanceToPointInTimeResult"
             }
         },
         "RevokeDBSecurityGroupIngress": {
+            "documentation": "<p>\u63a5\u7d9a\u3092\u8a31\u53ef\u3057\u305fIP\u7bc4\u56f2\u307e\u305f\u306f\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\u306e\u8a2d\u5b9a\u3092\u53d6\u308a\u6d88\u3057\u307e\u3059\u3002</p><p>\u3053\u306eAPI\u30a2\u30af\u30b7\u30e7\u30f3\u3067\u306fCIDRIP\uff08IP\u5e2f\uff09\u307e\u305f\u306fEC2SecurityGroupName\uff08\u30cb\u30d5\u30af\u30e9\u306e\u30d5\u30a1\u30a4\u30a2\u30a6\u30a9\u30fc\u30eb\u30b0\u30eb\u30fc\u30d7\u540d\uff09\u3092\u5fc5\u305a\u6307\u5b9a\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RevokeDBSecurityGroupIngressRequest"
             },
             "name": "RevokeDBSecurityGroupIngress",
             "output": {
                 "resultWrapper": "RevokeDBSecurityGroupIngressResult",
                 "shape": "RevokeDBSecurityGroupIngressResult"
             }
         },
         "SetExternalMaster": {
+            "documentation": "<p>\u5916\u90e8\u30ec\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u306e\u8a2d\u5b9a\u3092\u884c\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "SetExternalMasterRequest"
             },
             "name": "SetExternalMaster",
             "output": {
                 "resultWrapper": "SetExternalMasterResult",
                 "shape": "SetExternalMasterResult"
             }
         },
         "StartReplication": {
+            "documentation": "<p>\u5916\u90e8\u30ec\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u3092\u958b\u59cb\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StartReplicationRequest"
             },
             "name": "StartReplication",
             "output": {
                 "resultWrapper": "StartReplicationResult",
                 "shape": "StartReplicationResult"
             }
         },
         "StopReplication": {
+            "documentation": "<p>\u5916\u90e8\u30ec\u30d7\u30ea\u30b1\u30fc\u30b7\u30e7\u30f3\u3092\u505c\u6b62\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopReplicationRequest"
             },
             "name": "StopReplication",
             "output": {
                 "resultWrapper": "StopReplicationResult",
                 "shape": "StopReplicationResult"
             }
         },
         "UpgradeDBEngineVersion": {
+            "documentation": "<p>DB\u30b5\u30fc\u30d0\u30fc\u306e\u30c7\u30fc\u30bf\u30d9\u30fc\u30b9\u30a8\u30f3\u30b8\u30f3\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u3092\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u3057\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u53ef\u80fd\u306a\u30d0\u30fc\u30b8\u30e7\u30f3\u306fDescribeDBEngineVersions API\u304b\u3089\u53d6\u5f97\u3067\u304d\u307e\u3059\u3002</p><p>\u30ea\u30fc\u30c9\u30ec\u30d7\u30ea\u30ab\u304c\u5b58\u5728\u3059\u308b\u5834\u5408\u306f\u3001\u30de\u30b9\u30bf\u30fc\u3088\u308a\u5148\u306b\u5168\u3066\u306e\u30ea\u30fc\u30c9\u30ec\u30d7\u30ea\u30ab\u3092\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u3059\u308b\u5fc5\u8981\u304c\u3042\u308a\u307e\u3059\u3002</p><p>\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u304c\u6210\u529f\u3057\u305f\u5834\u5408\u3001\u5143\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u623b\u3059\u3053\u3068\u306f\u3067\u304d\u307e\u305b\u3093\u3002</p><p>\u5fc5\u8981\u306b\u5fdc\u3058\u3066PreUpgradeDBSnapshotIdentifier\u3092\u6307\u5b9a\u3057\u3001\u30a2\u30c3\u30d7\u30b0\u30ec\u30fc\u30c9\u524d\u306eDB\u30b9\u30ca\u30c3\u30d7\u30b7\u30e7\u30c3\u30c8\u3092\u4f5c\u6210\u3057\u3066\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "UpgradeDBEngineVersionRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/script/2015-09-01/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/script/2015-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/sdk-default-configuration.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/sdk-default-configuration.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'operations'": "{'DescribeEventAttributes': {'documentation': "*

 * *                 "'<p>ニフクラのサービス稼働に関するイベントをリストで取得します。</p>'}, 'DescribeEventCalendar': "*

 * *                 "{'documentation': '<p>ニフクラのサービス稼働に関するイベントをカレンダー形式で取得します。</p>'}, "*

 * *                 "'DescribeServiceStatuses': {'documentation': '<p>ニフクラのサービス稼働状況を取得します。</p>'}}"}*

```diff
@@ -7,40 +7,43 @@
         "serviceFullName": "NIFCLOUD Service Activity",
         "serviceId": "service-activity",
         "signatureVersion": "v4",
         "uid": "service-activity-2020-11-25"
     },
     "operations": {
         "DescribeEventAttributes": {
+            "documentation": "<p>\u30cb\u30d5\u30af\u30e9\u306e\u30b5\u30fc\u30d3\u30b9\u7a3c\u50cd\u306b\u95a2\u3059\u308b\u30a4\u30d9\u30f3\u30c8\u3092\u30ea\u30b9\u30c8\u3067\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/events/attributes/{YearMonth}"
             },
             "input": {
                 "shape": "DescribeEventAttributesRequest"
             },
             "name": "DescribeEventAttributes",
             "output": {
                 "shape": "DescribeEventAttributesResult"
             }
         },
         "DescribeEventCalendar": {
+            "documentation": "<p>\u30cb\u30d5\u30af\u30e9\u306e\u30b5\u30fc\u30d3\u30b9\u7a3c\u50cd\u306b\u95a2\u3059\u308b\u30a4\u30d9\u30f3\u30c8\u3092\u30ab\u30ec\u30f3\u30c0\u30fc\u5f62\u5f0f\u3067\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/events/calendars/{YearMonth}"
             },
             "input": {
                 "shape": "DescribeEventCalendarRequest"
             },
             "name": "DescribeEventCalendar",
             "output": {
                 "shape": "DescribeEventCalendarResult"
             }
         },
         "DescribeServiceStatuses": {
+            "documentation": "<p>\u30cb\u30d5\u30af\u30e9\u306e\u30b5\u30fc\u30d3\u30b9\u7a3c\u50cd\u72b6\u6cc1\u3092\u53d6\u5f97\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/services/statuses"
             },
             "input": {
                 "shape": "DescribeServiceStatusesRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/data/storage/2006-03-01/service-2.json` & `nifcloud-cli-1.9.0/nifcloudcli/data/storage/2006-03-01/service-2.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9865853658536585%*

 * *Differences: {"'operations'": "{'AbortMultipartUpload': {'documentation': '<p>マルチパートアップロードを中止します。</p>'}, "*

 * *                 "'CompleteMultipartUpload': {'documentation': "*

 * *                 "'<p>分割データを結合し、マルチパートアップロードを完了します。</p><p>注意事項: まれにAPIエラーコード400 "*

 * *                 "(InvalidPart)が返却されることがあります。その際は数秒おいてから再実行をお願いします。</p>'}, 'DeleteBucket': "*

 * *                 "{'documentation': '<p>空のバケットを削除します。</p><p>注意事項: "*

 * *                 "バケット内にオブジェクトが存在する場合、本操作は失敗します。</p>'}, 'DeleteBucketCors': {'documentation': "*

 * *               […]*

```diff
@@ -9,24 +9,26 @@
         "signatureVersion": "s3v4",
         "signingName": "s3",
         "uid": "storage-2006-03-01",
         "xmlNamespace": "http://s3.amazonaws.com/doc/2006-03-01/"
     },
     "operations": {
         "AbortMultipartUpload": {
+            "documentation": "<p>\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3092\u4e2d\u6b62\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}/{Object+}?x-id=AbortMultipartUpload"
             },
             "input": {
                 "shape": "AbortMultipartUploadRequest"
             },
             "name": "AbortMultipartUpload"
         },
         "CompleteMultipartUpload": {
+            "documentation": "<p>\u5206\u5272\u30c7\u30fc\u30bf\u3092\u7d50\u5408\u3057\u3001\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3092\u5b8c\u4e86\u3057\u307e\u3059\u3002</p><p>\u6ce8\u610f\u4e8b\u9805: \u307e\u308c\u306bAPI\u30a8\u30e9\u30fc\u30b3\u30fc\u30c9400 (InvalidPart)\u304c\u8fd4\u5374\u3055\u308c\u308b\u3053\u3068\u304c\u3042\u308a\u307e\u3059\u3002\u305d\u306e\u969b\u306f\u6570\u79d2\u304a\u3044\u3066\u304b\u3089\u518d\u5b9f\u884c\u3092\u304a\u9858\u3044\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/{Bucket}/{Object+}?x-id=CompleteMultipartUpload"
             },
             "input": {
                 "locationName": "CompleteMultipartUploadRequest",
                 "shape": "CompleteMultipartUploadRequest",
@@ -36,64 +38,70 @@
             },
             "name": "CompleteMultipartUpload",
             "output": {
                 "shape": "CompleteMultipartUploadResult"
             }
         },
         "DeleteBucket": {
+            "documentation": "<p>\u7a7a\u306e\u30d0\u30b1\u30c3\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p><p>\u6ce8\u610f\u4e8b\u9805: \u30d0\u30b1\u30c3\u30c8\u5185\u306b\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u304c\u5b58\u5728\u3059\u308b\u5834\u5408\u3001\u672c\u64cd\u4f5c\u306f\u5931\u6557\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}?x-id=DeleteBucket"
             },
             "input": {
                 "shape": "DeleteBucketRequest"
             },
             "name": "DeleteBucket"
         },
         "DeleteBucketCors": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308bCors (Cross-Origin Resource Sharing)\u69cb\u6210\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}?cors&x-id=DeleteBucketCors"
             },
             "input": {
                 "shape": "DeleteBucketCorsRequest"
             },
             "name": "DeleteBucketCors"
         },
         "DeleteBucketLifecycle": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30e9\u30a4\u30d5\u30b5\u30a4\u30af\u30eb\u69cb\u6210\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}?lifecycle&x-id=DeleteBucketLifecycle"
             },
             "input": {
                 "shape": "DeleteBucketLifecycleRequest"
             },
             "name": "DeleteBucketLifecycle"
         },
         "DeleteBucketPolicy": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30dd\u30ea\u30b7\u30fc\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}?policy&x-id=DeleteBucketPolicy"
             },
             "input": {
                 "shape": "DeleteBucketPolicyRequest"
             },
             "name": "DeleteBucketPolicy"
         },
         "DeleteBucketTagging": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u30bf\u30b0\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}?tagging&x-id=DeleteBucketTagging"
             },
             "input": {
                 "shape": "DeleteBucketTaggingRequest"
             },
             "name": "DeleteBucketTagging"
         },
         "DeleteMultipleObjects": {
+            "documentation": "<p>\u8907\u6570\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/{Bucket}?delete&x-id=DeleteMultipleObjects"
             },
             "input": {
                 "locationName": "DeleteMultipleObjectsRequest",
                 "shape": "DeleteMultipleObjectsRequest",
@@ -103,245 +111,264 @@
             },
             "name": "DeleteMultipleObjects",
             "output": {
                 "shape": "DeleteMultipleObjectsResult"
             }
         },
         "DeleteObject": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}/{Object+}?x-id=DeleteObject"
             },
             "input": {
                 "shape": "DeleteObjectRequest"
             },
             "name": "DeleteObject",
             "output": {
                 "shape": "DeleteObjectResult"
             }
         },
         "DeleteObjectTagging": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30bf\u30b0\u60c5\u5831\u3092\u524a\u9664\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "DELETE",
                 "requestUri": "/{Bucket}/{Object+}?tagging&x-id=DeleteObjectTagging"
             },
             "input": {
                 "shape": "DeleteObjectTaggingRequest"
             },
             "name": "DeleteObjectTagging",
             "output": {
                 "shape": "DeleteObjectTaggingResult"
             }
         },
         "GetBucket": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u5185\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u4e00\u90e8\u307e\u305f\u306f\u5168\u90e8(\u6700\u59271000)\u3092\u4e00\u89a7\u8868\u793a\u3057\u307e\u3059\u3002</p><p>\u6ce8\u610f\u4e8b\u9805: \u672cAPI\u306f\u65e7\u30d0\u30fc\u30b8\u30e7\u30f3API\u3067\u3059\u3002\u300c<a href=\"https://docs.nifcloud.com/object-storage-service/api/GetBucketVersion2.htm\">GetBucketVersion2</a>\u300d\u3092\u3054\u5229\u7528\u304f\u3060\u3055\u3044\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?x-id=GetBucket"
             },
             "input": {
                 "shape": "GetBucketRequest"
             },
             "name": "GetBucket",
             "output": {
                 "shape": "GetBucketResult"
             }
         },
         "GetBucketACL": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u30a2\u30af\u30bb\u30b9\u5236\u5fa1\u30ea\u30b9\u30c8\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?acl&x-id=GetBucketACL"
             },
             "input": {
                 "shape": "GetBucketACLRequest"
             },
             "name": "GetBucketACL",
             "output": {
                 "shape": "GetBucketACLResult"
             }
         },
         "GetBucketConsistency": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u6574\u5408\u6027\u30ec\u30d9\u30eb\u3092\u554f\u3044\u5408\u308f\u305b\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?x-ntap-sg-consistency&x-id=GetBucketConsistency"
             },
             "input": {
                 "shape": "GetBucketConsistencyRequest"
             },
             "name": "GetBucketConsistency",
             "output": {
                 "shape": "GetBucketConsistencyResult"
             }
         },
         "GetBucketCors": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308bCors(Cross-Origin Resource Sharing)\u69cb\u6210\u60c5\u5831\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?cors&x-id=GetBucketCors"
             },
             "input": {
                 "shape": "GetBucketCorsRequest"
             },
             "name": "GetBucketCors",
             "output": {
                 "shape": "GetBucketCorsResult"
             }
         },
         "GetBucketLifecycleConfiguration": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u3066\u3044\u308b\u30e9\u30a4\u30d5\u30b5\u30a4\u30af\u30eb\u69cb\u6210\u60c5\u5831\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?lifecycle&x-id=GetBucketLifecycleConfiguration"
             },
             "input": {
                 "shape": "GetBucketLifecycleConfigurationRequest"
             },
             "name": "GetBucketLifecycleConfiguration",
             "output": {
                 "shape": "GetBucketLifecycleConfigurationResult"
             }
         },
         "GetBucketObjectVersions": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u5185\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u3059\u3079\u3066\u306e\u30d0\u30fc\u30b8\u30e7\u30f3\u306b\u95a2\u3059\u308b\u30e1\u30bf\u30c7\u30fc\u30bf\u3092\u4e00\u89a7\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?versions&x-id=GetBucketObjectVersions"
             },
             "input": {
                 "shape": "GetBucketObjectVersionsRequest"
             },
             "name": "GetBucketObjectVersions",
             "output": {
                 "shape": "GetBucketObjectVersionsResult"
             }
         },
         "GetBucketPolicy": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u8a2d\u5b9a\u3055\u308c\u305f\u30dd\u30ea\u30b7\u30fc\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?policy&x-id=GetBucketPolicy"
             },
             "input": {
                 "shape": "GetBucketPolicyRequest"
             },
             "name": "GetBucketPolicy",
             "output": {
                 "shape": "GetBucketPolicyResult"
             }
         },
         "GetBucketTagging": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u30bf\u30b0\u60c5\u5831\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?tagging&x-id=GetBucketTagging"
             },
             "input": {
                 "shape": "GetBucketTaggingRequest"
             },
             "name": "GetBucketTagging",
             "output": {
                 "shape": "GetBucketTaggingResult"
             }
         },
         "GetBucketVersion2": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u5185\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u4e00\u90e8\u307e\u305f\u306f\u5168\u90e8(\u6700\u59271000)\u3092\u4e00\u89a7\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?x-id=GetBucketVersion2"
             },
             "input": {
                 "shape": "GetBucketVersion2Request"
             },
             "name": "GetBucketVersion2",
             "output": {
                 "shape": "GetBucketVersion2Result"
             }
         },
         "GetBucketVersioning": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u30d0\u30fc\u30b8\u30e7\u30cb\u30f3\u30b0\u72b6\u614b\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?versioning&x-id=GetBucketVersioning"
             },
             "input": {
                 "shape": "GetBucketVersioningRequest"
             },
             "name": "GetBucketVersioning",
             "output": {
                 "shape": "GetBucketVersioningResult"
             }
         },
         "GetObject": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u5185\u5bb9\u3068\u30e1\u30bf\u30c7\u30fc\u30bf\u3092\u30c0\u30a6\u30f3\u30ed\u30fc\u30c9\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}/{Object+}?x-id=GetObject"
             },
             "input": {
                 "shape": "GetObjectRequest"
             },
             "name": "GetObject",
             "output": {
                 "shape": "GetObjectResult"
             }
         },
         "GetObjectACL": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306eACL\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}/{Object+}?acl&x-id=GetObjectACL"
             },
             "input": {
                 "shape": "GetObjectACLRequest"
             },
             "name": "GetObjectACL",
             "output": {
                 "shape": "GetObjectACLResult"
             }
         },
         "GetObjectTagging": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30bf\u30b0\u60c5\u5831\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}/{Object+}?tagging&x-id=GetObjectTagging"
             },
             "input": {
                 "shape": "GetObjectTaggingRequest"
             },
             "name": "GetObjectTagging",
             "output": {
                 "shape": "GetObjectTaggingResult"
             }
         },
         "GetService": {
+            "documentation": "<p>\u6240\u6709\u3057\u3066\u3044\u308b\u3059\u3079\u3066\u306e\u30d0\u30b1\u30c3\u30c8\u3092\u4e00\u89a7\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/?x-id=GetService"
             },
             "input": {
                 "shape": "GetServiceRequest"
             },
             "name": "GetService",
             "output": {
                 "shape": "GetServiceResult"
             }
         },
         "HeadBucket": {
+            "documentation": "<p>\u6307\u5b9a\u3059\u308b\u30d0\u30b1\u30c3\u30c8\u306b\u30a2\u30af\u30bb\u30b9\u6a29\u304c\u3042\u308b\u304b\u3069\u3046\u304b\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "HEAD",
                 "requestUri": "/{Bucket}?x-id=HeadBucket"
             },
             "input": {
                 "shape": "HeadBucketRequest"
             },
             "name": "HeadBucket"
         },
         "HeadObject": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30e1\u30bf\u30c7\u30fc\u30bf\u3092\u8868\u793a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "HEAD",
                 "requestUri": "/{Bucket}/{Object+}?x-id=HeadObject"
             },
             "input": {
                 "shape": "HeadObjectRequest"
             },
             "name": "HeadObject",
             "output": {
                 "shape": "HeadObjectResult"
             }
         },
         "InitiateMultipartUpload": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u304c\u958b\u59cb\u3055\u308c\u3001\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9ID\u304c\u8fd4\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/{Bucket}/{Object+}?uploads&x-id=InitiateMultipartUpload"
             },
             "input": {
                 "locationName": "InitiateMultipartUploadRequest",
                 "shape": "InitiateMultipartUploadRequest",
@@ -351,168 +378,182 @@
             },
             "name": "InitiateMultipartUpload",
             "output": {
                 "shape": "InitiateMultipartUploadResult"
             }
         },
         "ListMultipartUploads": {
+            "documentation": "<p>\u9032\u884c\u4e2d\u306e\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u304c\u8868\u793a\u3055\u308c\u307e\u3059\u3002</p><p><a href=\"https://docs.nifcloud.com/object-storage-service/api/CompleteMultipartUpload.htm\">CompleteMultipartUpload</a>\u3067\u5b8c\u4e86\u3057\u305f\u30d1\u30fc\u30c8\u306f\u8868\u793a\u3055\u308c\u307e\u305b\u3093\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}?uploads&x-id=ListMultipartUploads"
             },
             "input": {
                 "shape": "ListMultipartUploadsRequest"
             },
             "name": "ListMultipartUploads",
             "output": {
                 "shape": "ListMultipartUploadsResult"
             }
         },
         "ListParts": {
+            "documentation": "<p>\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9ID\u306b\u7d10\u4ed8\u3044\u3066\u3044\u308b\u3001\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u7528\u306b\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3055\u308c\u305f\u30d1\u30fc\u30c8\u3092\u4e00\u89a7\u8868\u793a\u3057\u307e\u3059\u3002</p><p>\u5206\u5272\u30d5\u30a1\u30a4\u30eb\u306e\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u72b6\u6cc1\u3092\u78ba\u8a8d\u3067\u304d\u307e\u3059\u3002</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/{Bucket}/{Object+}?x-id=ListParts"
             },
             "input": {
                 "shape": "ListPartsRequest"
             },
             "name": "ListParts",
             "output": {
                 "shape": "ListPartsResult"
             }
         },
         "PutBucket": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?x-id=PutBucket"
             },
             "input": {
                 "shape": "PutBucketRequest"
             },
             "name": "PutBucket",
             "output": {
                 "shape": "PutBucketResult"
             }
         },
         "PutBucketConsistency": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306e\u6574\u5408\u6027\u30ec\u30d9\u30eb\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?x-id=PutBucketConsistency"
             },
             "input": {
                 "shape": "PutBucketConsistencyRequest"
             },
             "name": "PutBucketConsistency",
             "output": {
                 "shape": "PutBucketConsistencyResult"
             }
         },
         "PutBucketCors": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306bCors(Cross-Origin Resource Sharing)\u69cb\u6210\u60c5\u5831\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?cors&x-id=PutBucketCors"
             },
             "input": {
                 "shape": "PutBucketCorsRequest"
             },
             "name": "PutBucketCors"
         },
         "PutBucketLifecycleConfiguration": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u30e9\u30a4\u30d5\u30b5\u30a4\u30af\u30eb\u69cb\u6210\u60c5\u5831\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?lifecycle&x-id=PutBucketLifecycleConfiguration"
             },
             "input": {
                 "shape": "PutBucketLifecycleConfigurationRequest"
             },
             "name": "PutBucketLifecycleConfiguration"
         },
         "PutBucketPolicy": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u30dd\u30ea\u30b7\u30fc\u3092\u8a2d\u5b9a\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?policy&x-id=PutBucketPolicy"
             },
             "input": {
                 "shape": "PutBucketPolicyRequest"
             },
             "name": "PutBucketPolicy"
         },
         "PutBucketTagging": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u30bf\u30b0\u60c5\u5831\u3092\u4ed8\u4e0e\u3057\u307e\u3059\u3002\u30bf\u30b0\u60c5\u5831\u306f\u4e0a\u66f8\u304d\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?tagging&x-id=PutBucketTagging"
             },
             "input": {
                 "shape": "PutBucketTaggingRequest"
             },
             "name": "PutBucketTagging"
         },
         "PutBucketVersioning": {
+            "documentation": "<p>\u30d0\u30b1\u30c3\u30c8\u306b\u30d0\u30fc\u30b8\u30e7\u30cb\u30f3\u30b0\u8a2d\u5b9a\u3092\u884c\u3044\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}?versioning&x-id=PutBucketVersioning"
             },
             "input": {
                 "shape": "PutBucketVersioningRequest"
             },
             "name": "PutBucketVersioning"
         },
         "PutObject": {
+            "documentation": "<p>\u65b0\u3057\u3044\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002\u307e\u305f\u306f\u3001\u65e2\u5b58\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u3092\u7f6e\u304d\u63db\u3048\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}/{Object+}?x-id=PutObject"
             },
             "input": {
                 "shape": "PutObjectRequest"
             },
             "name": "PutObject",
             "output": {
                 "shape": "PutObjectResult"
             }
         },
         "PutObjectCopy": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30b3\u30d4\u30fc\u3092\u4f5c\u6210\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}/{Object+}?x-id=PutObjectCopy"
             },
             "input": {
                 "shape": "PutObjectCopyRequest"
             },
             "name": "PutObjectCopy",
             "output": {
                 "shape": "PutObjectCopyResult"
             }
         },
         "PutObjectTagging": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306b\u30bf\u30b0\u60c5\u5831\u3092\u4ed8\u4e0e\u3057\u307e\u3059\u3002\u30bf\u30b0\u60c5\u5831\u306f\u4e0a\u66f8\u304d\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}/{Object+}?tagging&x-id=PutObjectTagging"
             },
             "input": {
                 "shape": "PutObjectTaggingRequest"
             },
             "name": "PutObjectTagging",
             "output": {
                 "shape": "PutObjectTaggingResult"
             }
         },
         "UploadPart": {
+            "documentation": "<p>\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30de\u30eb\u30c1\u30d1\u30fc\u30c8\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u5185\u306e\u30d1\u30fc\u30c8\u304c\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3055\u308c\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}/{Object+}?x-id=UploadPart"
             },
             "input": {
                 "shape": "UploadPartRequest"
             },
             "name": "UploadPart",
             "output": {
                 "shape": "UploadPartResult"
             }
         },
         "UploadPartCopy": {
+            "documentation": "<p>\u30d1\u30fc\u30c8(\u5206\u5272\u30c7\u30fc\u30bf)\u306e\u30c7\u30fc\u30bf\u30bd\u30fc\u30b9\u3068\u3057\u3066\u3001\u65e2\u5b58\u306e\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u304b\u3089\u30c7\u30fc\u30bf\u3092\u30b3\u30d4\u30fc\u3059\u308b\u3053\u3068\u3067\u3001\u30aa\u30d6\u30b8\u30a7\u30af\u30c8\u306e\u30d1\u30fc\u30c8\u3092\u30a2\u30c3\u30d7\u30ed\u30fc\u30c9\u3057\u307e\u3059\u3002</p>",
             "http": {
                 "method": "PUT",
                 "requestUri": "/{Bucket}/{Object+}?x-id=UploadPartCopy"
             },
             "input": {
                 "shape": "UploadPartCopyRequest"
             },
```

### Comparing `nifcloud-cli-1.8.0/nifcloudcli/link.py` & `nifcloud-cli-1.9.0/nifcloudcli/link.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.8.0/setup.py` & `nifcloud-cli-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='FUJITSU CLOUD TECHNOLOGIES',
     url='https://github.com/nifcloud/nifcloud-cli',
     packages=find_packages(exclude=['tests*']),
     package_data={'nifcloudcli': ['data/*.json', 'topics/*.json']},
     include_package_data=True,
-    install_requires=['nifcloud==1.8.0', 'awscli==1.29.1', 'pyyaml==5.3.1'],
+    install_requires=['nifcloud==1.9.0', 'awscli==1.29.1', 'pyyaml==5.3.1'],
     license='Apache License 2.0',
     classifiers=(
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
```

