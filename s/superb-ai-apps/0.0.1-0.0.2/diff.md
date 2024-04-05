# Comparing `tmp/superb-ai-apps-0.0.1.tar.gz` & `tmp/superb-ai-apps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.1.tar", last modified: Thu Apr  4 09:25:55 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.2.tar", last modified: Fri Apr  5 04:05:51 2024, max compression
```

## Comparing `superb-ai-apps-0.0.1.tar` & `superb-ai-apps-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/curate/superb_curate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/label/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-04 09:25:42.000000 superb-ai-apps-0.0.1/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:25:55.924298 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 09:25:55.000000 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 09:25:55.000000 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:25:55.000000 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 09:25:55.000000 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:25:55.000000 superb-ai-apps-0.0.1/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.768951 superb-ai-apps-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 04:05:51.768951 superb-ai-apps-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:05:51.768951 superb-ai-apps-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.764951 superb-ai-apps-0.0.2/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.764951 superb-ai-apps-0.0.2/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/curate/superb_curate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.764951 superb-ai-apps-0.0.2/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/label/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.764951 superb-ai-apps-0.0.2/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-05 04:05:40.000000 superb-ai-apps-0.0.2/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:05:51.768951 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 04:05:51.000000 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 04:05:51.000000 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:05:51.000000 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 04:05:51.000000 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 04:05:51.000000 superb-ai-apps-0.0.2/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.1/spb_apps/apps.py` & `superb-ai-apps-0.0.2/spb_apps/apps.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.1/spb_apps/curate/superb_curate.py` & `superb-ai-apps-0.0.2/spb_apps/curate/superb_curate.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.1/spb_apps/label/superb_label.py` & `superb-ai-apps-0.0.2/spb_apps/label/superb_label.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.1/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.2/spb_apps/utils/converter.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.1/spb_apps/utils/utils.py` & `superb-ai-apps-0.0.2/spb_apps/utils/utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.1/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.2/superb_ai_apps.egg-info/requires.txt`

 * *Files identical despite different names*

