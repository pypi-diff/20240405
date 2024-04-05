# Comparing `tmp/timelength-1.1.7.tar.gz` & `tmp/timelength-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelength-1.1.7.tar", last modified: Mon Mar  6 03:38:47 2023, max compression
+gzip compressed data, was "timelength-2.0.1.tar", max compression
```

## Comparing `timelength-1.1.7.tar` & `timelength-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 03:38:47.543505 timelength-1.1.7/
--rw-rw-rw-   0        0        0     1082 2022-12-30 05:39:31.000000 timelength-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     3233 2023-03-06 03:38:47.541506 timelength-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2764 2023-03-02 03:24:45.000000 timelength-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-03-06 03:38:47.543505 timelength-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-03-06 03:38:13.000000 timelength-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 03:38:47.516518 timelength-1.1.7/timelength/
--rw-rw-rw-   0        0        0      138 2023-03-02 03:24:37.000000 timelength-1.1.7/timelength/__init__.py
--rw-rw-rw-   0        0        0       79 2023-03-02 03:24:39.000000 timelength-1.1.7/timelength/constants.py
--rw-rw-rw-   0        0        0      414 2022-12-31 16:58:57.000000 timelength-1.1.7/timelength/exceptions.py
--rw-rw-rw-   0        0        0      274 2023-03-02 03:24:40.000000 timelength-1.1.7/timelength/helper.py
--rw-rw-rw-   0        0        0     5509 2023-03-02 03:24:42.000000 timelength-1.1.7/timelength/scales.py
--rw-rw-rw-   0        0        0    10275 2023-03-06 03:37:49.000000 timelength-1.1.7/timelength/timelength.py
-drwxrwxrwx   0        0        0        0 2023-03-06 03:38:47.535508 timelength-1.1.7/timelength.egg-info/
--rw-rw-rw-   0        0        0     3233 2023-03-06 03:38:44.000000 timelength-1.1.7/timelength.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-03-06 03:38:45.000000 timelength-1.1.7/timelength.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 03:38:44.000000 timelength-1.1.7/timelength.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-06 03:38:44.000000 timelength-1.1.7/timelength.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1082 2024-01-19 07:44:29.030225 timelength-2.0.1/LICENSE
+-rw-r--r--   0        0        0      983 2024-04-05 00:58:04.282919 timelength-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5485 2024-04-04 23:50:53.149033 timelength-2.0.1/README.md
+-rw-r--r--   0        0        0      176 2024-04-04 23:50:53.152033 timelength-2.0.1/timelength/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-04 23:50:53.153032 timelength-2.0.1/timelength/dataclasses.py
+-rw-r--r--   0        0        0      919 2024-04-04 23:50:53.154032 timelength-2.0.1/timelength/enums.py
+-rw-r--r--   0        0        0      406 2024-04-04 23:50:53.155032 timelength-2.0.1/timelength/errors.py
+-rw-r--r--   0        0        0     9721 2024-04-04 23:50:53.156033 timelength-2.0.1/timelength/locales/english.json
+-rw-r--r--   0        0        0    12417 2024-04-05 02:05:38.194008 timelength-2.0.1/timelength/locales/spanish.json
+-rw-r--r--   0        0        0     8406 2024-04-04 23:50:53.155032 timelength-2.0.1/timelength/locales.py
+-rw-r--r--   0        0        0    17248 2024-04-05 02:05:48.024835 timelength-2.0.1/timelength/parsers/parser_one.py
+-rw-r--r--   0        0        0     8749 2024-04-05 00:57:48.478450 timelength-2.0.1/timelength/timelength.py
+-rw-r--r--   0        0        0     1296 2024-04-04 23:50:53.159032 timelength-2.0.1/timelength/utils.py
+-rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 timelength-2.0.1/PKG-INFO
```

### Comparing `timelength-1.1.7/LICENSE` & `timelength-2.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Etorix
+Copyright (c) 2024 Etorix
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

