# Comparing `tmp/galter-subjects-utils-0.3.5.tar.gz` & `tmp/galter-subjects-utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galter-subjects-utils-0.3.5.tar", last modified: Thu Mar 21 19:46:41 2024, max compression
+gzip compressed data, was "galter-subjects-utils-0.4.0.tar", last modified: Fri Apr  5 12:48:52 2024, max compression
```

## Comparing `galter-subjects-utils-0.3.5.tar` & `galter-subjects-utils-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.936047 galter-subjects-utils-0.3.5/galter_subjects_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.936047 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.936047 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/galter_subjects_utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 19:46:41.000000 galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.932047 galter-subjects-utils-0.3.5/tests/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/tests/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/contrib/mesh/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/contrib/mesh/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/contrib/mesh/test_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:41.940047 galter-subjects-utils-0.3.5/tests/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/downloads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/test_keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/test_lcsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-21 19:46:36.000000 galter-subjects-utils-0.3.5/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.210984 galter-subjects-utils-0.4.0/galter_subjects_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.210984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/lcsh/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/types_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/galter_subjects_utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:48:52.000000 galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.214984 galter-subjects-utils-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.206984 galter-subjects-utils-0.4.0/tests/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/lcsh/test_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/contrib/mesh/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:52.218984 galter-subjects-utils-0.4.0/tests/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/downloads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-05 12:48:42.000000 galter-subjects-utils-0.4.0/tests/test_writer.py
```

### Comparing `galter-subjects-utils-0.3.5/LICENSE` & `galter-subjects-utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/MANIFEST.in` & `galter-subjects-utils-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/PKG-INFO` & `galter-subjects-utils-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.3.5
+Version: 0.4.0
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `galter-subjects-utils-0.3.5/README.md` & `galter-subjects-utils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/adapter.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/adapter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,40 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2024 Northwestern University.
+# Copyright (C) 2021-2024 Northwestern University.
 #
 # galter-subjects-utils is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""Adapters to convert between different outputs and inputs."""
+"""Generic download functionality."""
 
-from .converter import Subject
+from .types_internal import Subject
 
 
-def generate_replacements(replace_iter):
-    """Converts a replace iterable into a replacement dict.
-
-    :param replace_iter: Iterable[ReplaceEntry]
-
-    ReplaceEntry:
-
-    {
-        "MH OLD": "...",
-        "MH NEW": "...",
-        "delete": "...",
-        "status": "...",
-    }
-    """
-    return {
-        e["MH OLD"]: e["MH NEW"] for e in replace_iter if e["delete"]
-    }
-
-
-def converted_to_subjects(rdm_iter):
+def converted_to_subjects(rdm_iter, prefix):
     """Adapts an RDMSubject ("Converted") iterable into a Subject iterable.
 
     :param rdm_iter: Iterable[RDMSubject]
 
     RDMSubject:
 
     {
-        "id": "https://id.nlm.nih.gov/mesh/...",
+        "id": "<prefix>...",
         "scheme": "...",
         "subject": "..."
     }
 
     :return: Iterable[Subject]
 
     Subject:
 
-        id (minus the https://id.nlm.nih.gov/mesh/ part)
+        id (minus the <prefix> part)
         label
     """
-    prefix = "https://id.nlm.nih.gov/mesh/"
     len_prefix = len(prefix)
     return (
         Subject(
             id=e["id"][len_prefix:] if e["id"].startswith(prefix) else e["id"],
             label=e["subject"]
         ) for e in rdm_iter
     )
```

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/cli.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 from datetime import date
 from functools import wraps
 from pathlib import Path
 
 import click
 from flask.cli import with_appcontext
 
+from galter_subjects_utils.adapter import converted_to_subjects
+from galter_subjects_utils.deltor import DeltasGenerator
 from galter_subjects_utils.keeptrace import KeepTrace
 from galter_subjects_utils.reader import get_rdm_subjects, mapping_by
-from galter_subjects_utils.writer import write_csv, write_jsonl
+from galter_subjects_utils.writer import write_csv
 
-from .adapter import converted_to_subjects, generate_replacements
-from .converter import MeSHRDMConverter, MeSHSubjectDeltasConverter
+from .adapter import generate_replacements
+from .converter import MeSHRDMConverter
 from .downloader import MeSHDownloader
 from .reader import MeSHReader, MeSHReplaceReader, topic_filter
+from .scheme import MeSHScheme
 
 defaults = {
     "year": date.today().year,
     "filter": "topic-qualifier",
     "downloads-dir": Path.cwd(),
     "output-file": Path.cwd(),
 }
@@ -160,18 +163,19 @@
 @with_appcontext
 def mesh_deltas(**parameters):
     """Write MeSH subject delta operations to file."""
     print("Generating deltas...")
     downloads_dir = parameters["downloads_dir"].expanduser()
     year = parameters["year"]
     filter_ = parameters["filter"]
+    mesh = MeSHScheme()
 
     # Source subjects
-    subject_rdm_preexisting = get_rdm_subjects(scheme="MeSH")
-    src = converted_to_subjects(subject_rdm_preexisting)
+    subject_rdm_preexisting = get_rdm_subjects(scheme=mesh.name)
+    src = converted_to_subjects(subject_rdm_preexisting, mesh.prefix)
 
     # Destination subjects
     subjects_fp = downloads_dir / f"d{year}.bin"
     topics = MeSHReader(subjects_fp, filter=topic_filter).read()
 
     if filter_ == "topic-qualifier":
         qualifiers_fp = downloads_dir / f"q{year}.bin"
@@ -188,20 +192,21 @@
     # Replacements
     replace_fp = downloads_dir / f"replace{year}.txt"
     replacements = generate_replacements(
         MeSHReplaceReader(replace_fp).read()
     )
 
     ops = (
-        MeSHSubjectDeltasConverter(
+        DeltasGenerator(
             src_subjects=src,
             dst_subjects=dst,
+            scheme=mesh,
             replacements=replacements
         )
-        .convert()
+        .generate()
     )
     # in-place
     KeepTrace.mark(
         ops,
         # only can keep trace of *those* anyway
         yes_logic=lambda op: op["type"] in ["rename", "replace", "remove"]
     )
```

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/converter.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/deltor.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,114 +2,63 @@
 #
 # Copyright (C) 2024 Northwestern University.
 #
 # galter-subjects-utils is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""Convert MeSH data to InvenioRDM/ops."""
+"""Generate delta operations."""
 
 from dataclasses import dataclass
 
 
-def generate_id(identifier):
-    """Generate URI id."""
-    return f"https://id.nlm.nih.gov/mesh/{identifier}"
-
-
-class MeSHRDMConverter:
-    """Convert MeSH term into RDM subject dict."""
-
-    def __init__(self, topics, qualifiers_mapping=None):
-        """Constructor.
-
-        :param topics: MeSH Topics iterable
-        :type topics: iterable[dict]
-        :param qualifiers: MeSH qualifiers iterable, defaults to None
-        :type qualifiers: iterable[dict], optional
-        """
-        self.topics = topics
-        self.qualifiers_mapping = qualifiers_mapping
-
-    def __iter__(self):
-        """Iterate over converted entries.
-
-        DEPRECATED.
-        """
-        yield from self.convert()
-
-    def convert(self):
-        """Iterator over converted entries."""
-        for topic in self.topics:
-            yield {
-                "id": generate_id(topic['UI']),
-                "scheme": "MeSH",
-                "subject": topic['MH']
-            }
-
-            if not self.qualifiers_mapping:
-                continue
-
-            for qid in topic.get("AQ", []):
-                qualifier = self.qualifiers_mapping.get(qid)
-
-                if not qualifier:
-                    continue
-
-                yield {
-                    "id": generate_id(topic['UI'] + qualifier['UI']),
-                    "scheme": "MeSH",
-                    "subject": topic['MH'] + "/" + qualifier['SH']
-                }
-
-
-@dataclass
-class Subject:
-    """Minimalist subject data."""
-
-    id: str
-    label: str
-
-
 @dataclass
 class Analysis:
-    """Holds results of analyzing a src subject."""
+    """
+    Holds results of analyzing a src subject.
+
+    Can't be a namedtuple because it needs to be mutable.
+    """
 
     id: str
     seen: bool = False  # present in dst subjects
     relabelled: str = ""  # new label
     replaced: str = ""  # id of replacing subject
 
 
-class MeSHSubjectDeltasConverter:
-    """Converter between subjects in DB + new subject file to operations."""
+class DeltasGenerator:
+    """Generates deltas between subjects in DB and new subjects."""
 
-    def __init__(self, src_subjects, dst_subjects, replacements):
+    def __init__(
+            self, src_subjects, dst_subjects, scheme, replacements=None):
         """Constructor.
 
         :param src_subjects: MeSH subjects found in the instance
         :type src_subjects: Iterable[Subject]
         :param dst_subjects: new subjects reader
         :type dst_subjects: Iterable[Subject]
         :param replacements: mapping of src labels to dst labels
         :type replacements: dict[str, str]
         """
         self.src_subjects = src_subjects
         self.dst_subjects = dst_subjects
+        self.scheme = scheme
         self.replacements = replacements
 
-        # Will be filled out by _analyze_src(), _analyze_dst() and
+        # The below will be filled out by _analyze_src(), _analyze_dst() and
         # _analyze_replace()
         self._id_to_analysis = {}
         self._label_to_analysis = {}
         self._additions = []
 
-        self.scheme = "MeSH"
+        # Ease of refactoring
+        self.name_of_scheme = scheme.name
+        self.generate_id = scheme.generate_id
 
-    def convert(self):
+    def generate(self):
         """Generate operations."""
         self._analyze_src()
         self._analyze_dst()
         self._analyze_replace()
         return self._generate_ops()
 
     def _analyze_src(self):
@@ -138,15 +87,22 @@
                 analysis.relabelled = dst_subject.label
             # identical ?
             else:
                 analysis = self._id_to_analysis[dst_subject.id]
                 analysis.seen = True
 
     def _analyze_replace(self):
-        """Determine which subjects have been replaced."""
+        """Determine which subjects have been replaced.
+
+        TODO with more subjects examples: revise this implementation. Right
+        now, the implementation stems from the original MeSH
+        case where replacements were given as labels to new label. In LCSH,
+        replacements are not given but extracted/devised by expert. We need
+        more cases before an abstraction can be made.
+        """
 
         def find_replacement_label(label):
             """Return replacement label or None."""
             new_label = self.replacements.get(label)
             if new_label:
                 return new_label
 
@@ -202,53 +158,53 @@
         """Generate delta operations."""
         result = []
 
         # Additions
         result.extend(
             {
                 "type": "add",
-                "scheme": self.scheme,
-                "id": generate_id(a.id),
+                "scheme": self.name_of_scheme,
+                "id": self.generate_id(a.id),
                 "subject": a.label
             }
             for a in self._additions
         )
 
         # Renames
         result.extend(
             {
                 "type": "rename",
-                "scheme": self.scheme,
-                "id": generate_id(analysis.id),
+                "scheme": self.name_of_scheme,
+                "id": self.generate_id(analysis.id),
                 "subject": label,
                 "new_subject": analysis.relabelled
             }
             for label, analysis in self._label_to_analysis.items()
             if analysis.relabelled
         )
 
         # Replaces
         result.extend(
             {
                 "type": "replace",
-                "scheme": self.scheme,
-                "id": generate_id(analysis.id),
+                "scheme": self.name_of_scheme,
+                "id": self.generate_id(analysis.id),
                 "subject": label,
-                "new_id": generate_id(analysis.replaced)
+                "new_id": self.generate_id(analysis.replaced)
             }
             for label, analysis in self._label_to_analysis.items()
             if analysis.replaced
         )
 
         # Removes
         result.extend(
             {
                 "type": "remove",
-                "scheme": self.scheme,
-                "id": generate_id(analysis.id),
+                "scheme": self.name_of_scheme,
+                "id": self.generate_id(analysis.id),
                 "subject": label
             }
             for label, analysis in self._label_to_analysis.items()
             if not analysis.seen and not analysis.replaced
         )
 
         return result
```

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/downloader.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/contrib/mesh/reader.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/contrib/mesh/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/downloader.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/downloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,29 +26,7 @@
 def extract_file(in_filepath, out_filepath):
     """Extract gzipped file."""
     with gzip.open(in_filepath, 'rb') as f_in:
         with open(out_filepath, 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
 
     return out_filepath
-
-
-class LCSHDownloader:
-    """Download LCSH file."""
-
-    def __init__(self, directory, cache=False):
-        """Constructor."""
-        self.base_url = "https://id.loc.gov/download/authorities/subjects.skosrdf.jsonld.gz"  # noqa
-        self.directory = directory
-        self.filepath = self.directory / self.base_url.rsplit("/")[-1]
-        self.cache = cache
-
-    def download(self):
-        """Download LCSH files of interest."""
-        if not self.cache or not self.filepath.exists():
-            download_file(self.base_url, self.filepath)
-            # sneak extraction in caching: bit of a cheat, but ok for now
-            extract_file(self.filepath, self.filepath.with_suffix(""))
-
-        self.downloaded_filepath = self.filepath  # just a marker + future
-        self.extracted_filepath = self.filepath.with_suffix("")
-        return self.extracted_filepath
```

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/keeptrace.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/reader.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/updater.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils/writer.py` & `galter-subjects-utils-0.4.0/galter_subjects_utils/writer.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/PKG-INFO` & `galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.3.5
+Version: 0.4.0
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `galter-subjects-utils-0.3.5/galter_subjects_utils.egg-info/SOURCES.txt` & `galter-subjects-utils-0.4.0/galter_subjects_utils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 galter_subjects_utils/__init__.py
+galter_subjects_utils/adapter.py
 galter_subjects_utils/cli.py
-galter_subjects_utils/converter.py
+galter_subjects_utils/deltor.py
 galter_subjects_utils/downloader.py
 galter_subjects_utils/keeptrace.py
 galter_subjects_utils/reader.py
+galter_subjects_utils/scheme.py
+galter_subjects_utils/types_internal.py
 galter_subjects_utils/updater.py
 galter_subjects_utils/writer.py
 galter_subjects_utils.egg-info/PKG-INFO
 galter_subjects_utils.egg-info/SOURCES.txt
 galter_subjects_utils.egg-info/dependency_links.txt
 galter_subjects_utils.egg-info/entry_points.txt
 galter_subjects_utils.egg-info/requires.txt
 galter_subjects_utils.egg-info/top_level.txt
 galter_subjects_utils/contrib/__init__.py
+galter_subjects_utils/contrib/lcsh/__init__.py
+galter_subjects_utils/contrib/lcsh/adapter.py
+galter_subjects_utils/contrib/lcsh/cli.py
+galter_subjects_utils/contrib/lcsh/converter.py
+galter_subjects_utils/contrib/lcsh/downloader.py
+galter_subjects_utils/contrib/lcsh/scheme.py
 galter_subjects_utils/contrib/mesh/__init__.py
 galter_subjects_utils/contrib/mesh/adapter.py
 galter_subjects_utils/contrib/mesh/cli.py
 galter_subjects_utils/contrib/mesh/converter.py
 galter_subjects_utils/contrib/mesh/downloader.py
 galter_subjects_utils/contrib/mesh/reader.py
+galter_subjects_utils/contrib/mesh/scheme.py
 tests/conftest.py
+tests/test_deltor.py
 tests/test_keeptrace.py
-tests/test_lcsh.py
 tests/test_reader.py
 tests/test_updater.py
 tests/test_writer.py
+tests/contrib/lcsh/test_converter.py
+tests/contrib/lcsh/test_downloader.py
 tests/contrib/mesh/test_converter.py
 tests/contrib/mesh/test_downloader.py
 tests/contrib/mesh/test_reader.py
 tests/downloads/.gitkeep
```

### Comparing `galter-subjects-utils-0.3.5/pyproject.toml` & `galter-subjects-utils-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 keywords = ["invenio", "inveniordm", "subjects", "MeSH"]
 license = {file = "LICENSE"}
 name = "galter-subjects-utils"
 readme = "README.md"
 requires-python = ">=3.8"
 scripts = {galter-subjects-utils = "galter_subjects_utils.cli:main"}
 urls = {Repository = "https://github.com/galterlibrary/galter-subjects-utils"}
-version = "0.3.5"
+version = "0.4.0"
 
 [project.optional-dependencies]
 dev = [
     "check-manifest>=0.49",
     "invenio-search[opensearch2]>=2.1.0,<3.0.0",  # Needs to be specified separately as it's up to instance
     "invoke>=2.2,<3.0",
     "pytest-invenio>=2.1.1,<3.0.0",
```

### Comparing `galter-subjects-utils-0.3.5/tests/conftest.py` & `galter-subjects-utils-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/contrib/mesh/test_downloader.py` & `galter-subjects-utils-0.4.0/tests/contrib/mesh/test_downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/contrib/mesh/test_reader.py` & `galter-subjects-utils-0.4.0/tests/contrib/mesh/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/test_keeptrace.py` & `galter-subjects-utils-0.4.0/tests/test_keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/test_reader.py` & `galter-subjects-utils-0.4.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/test_updater.py` & `galter-subjects-utils-0.4.0/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.3.5/tests/test_writer.py` & `galter-subjects-utils-0.4.0/tests/test_writer.py`

 * *Files identical despite different names*

