# Comparing `tmp/nr-oaipmh-harvesters-1.0.8.tar.gz` & `tmp/nr-oaipmh-harvesters-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr-oaipmh-harvesters-1.0.8.tar", last modified: Wed Mar 20 19:58:44 2024, max compression
+gzip compressed data, was "nr-oaipmh-harvesters-1.0.9.tar", last modified: Thu Mar 28 18:08:00 2024, max compression
```

## Comparing `nr-oaipmh-harvesters-1.0.8.tar` & `nr-oaipmh-harvesters-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:58:44.937634 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/nusl/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/nusl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42183 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/nusl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-20 19:58:44.000000 nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:58:44.941634 nr-oaipmh-harvesters-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-03-20 19:57:40.000000 nr-oaipmh-harvesters-1.0.8/tests/test_institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:08:00.412157 nr-oaipmh-harvesters-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-28 18:08:00.412157 nr-oaipmh-harvesters-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:08:00.408157 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:08:00.408157 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/nusl/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/nusl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42186 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/nusl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:08:00.412157 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 18:08:00.000000 nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-28 18:08:00.412157 nr-oaipmh-harvesters-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:08:00.412157 nr-oaipmh-harvesters-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-03-28 18:06:50.000000 nr-oaipmh-harvesters-1.0.9/tests/test_institutions.py
```

### Comparing `nr-oaipmh-harvesters-1.0.8/PKG-INFO` & `nr-oaipmh-harvesters-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-oaipmh-harvesters
-Version: 1.0.8
+Version: 1.0.9
 Summary: OAIPMH harvesters for National repository
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-oai-pmh-harvester>=4.0.0
 Requires-Dist: dojson
 Requires-Dist: Levenshtein
 Requires-Dist: nr-metadata
```

### Comparing `nr-oaipmh-harvesters-1.0.8/README.md` & `nr-oaipmh-harvesters-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/ext.py` & `nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/ext.py`

 * *Files identical despite different names*

### Comparing `nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters/nusl/transformer.py` & `nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters/nusl/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
         md.setdefault("contributors", []).append(
             make_dict(
                 # full name
                 "fullName",
                 value[0],
                 # type of the contributor - only person supported by now
                 "nameType",
-                resolve_name_type(value),
+                resolve_name_type(value[0]),
                 # role of the contributor
                 "role",
                 role,
             )
         )
```

### Comparing `nr-oaipmh-harvesters-1.0.8/nr_oaipmh_harvesters.egg-info/PKG-INFO` & `nr-oaipmh-harvesters-1.0.9/nr_oaipmh_harvesters.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-oaipmh-harvesters
-Version: 1.0.8
+Version: 1.0.9
 Summary: OAIPMH harvesters for National repository
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-oai-pmh-harvester>=4.0.0
 Requires-Dist: dojson
 Requires-Dist: Levenshtein
 Requires-Dist: nr-metadata
```

### Comparing `nr-oaipmh-harvesters-1.0.8/setup.cfg` & `nr-oaipmh-harvesters-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nr-oaipmh-harvesters
-version = 1.0.8
+version = 1.0.9
 description = OAIPMH harvesters for National repository
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>", "Miroslav Simek <miroslav.simek@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `nr-oaipmh-harvesters-1.0.8/tests/test_institutions.py` & `nr-oaipmh-harvesters-1.0.9/tests/test_institutions.py`

 * *Files identical despite different names*

