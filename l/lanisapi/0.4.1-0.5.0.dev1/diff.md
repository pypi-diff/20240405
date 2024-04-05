# Comparing `tmp/lanisapi-0.4.1.tar.gz` & `tmp/lanisapi-0.5.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanisapi-0.4.1.tar", last modified: Sun Nov 26 00:46:09 2023, max compression
+gzip compressed data, was "lanisapi-0.5.0.dev1.tar", last modified: Fri Apr  5 17:35:30 2024, max compression
```

## Comparing `lanisapi-0.4.1.tar` & `lanisapi-0.5.0.dev1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-26 00:45:57.000000 lanisapi-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-11-26 00:46:09.130667 lanisapi-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2023-11-26 00:45:57.000000 lanisapi-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-11-26 00:45:57.000000 lanisapi-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 00:46:09.130667 lanisapi-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.126667 lanisapi-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.126667 lanisapi-0.4.1/src/lanisapi/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/authentication_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/conversations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/schools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/cryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/html_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.422249 lanisapi-0.5.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.422249 lanisapi-0.5.0.dev1/src/lanisapi/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/core/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/core/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/helper/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/helper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/helper/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/core/initialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/initialization/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/core/initialization/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/module/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/module/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/custom/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/module/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi/module/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/standard/substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 17:35:26.000000 lanisapi-0.5.0.dev1/src/lanisapi/module/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:35:30.426249 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-05 17:35:30.000000 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 17:35:30.000000 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:35:30.000000 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 17:35:30.000000 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 17:35:30.000000 lanisapi-0.5.0.dev1/src/lanisapi.egg-info/top_level.txt
```

