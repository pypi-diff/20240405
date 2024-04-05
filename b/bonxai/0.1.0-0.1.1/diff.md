# Comparing `tmp/bonxai-0.1.0.tar.gz` & `tmp/bonxai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/grace/git/bonXAI/bonxai/dist/.tmp-0lg_tus7/bonxai-0.1.0.tar", last modified: Tue Apr  2 16:42:27 2024, max compression
+gzip compressed data, was "bonxai-0.1.1.tar", last modified: Fri Apr  5 15:44:09 2024, max compression
```

## Comparing `bonxai-0.1.0.tar` & `bonxai-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.617713 bonxai-0.1.0/
--rw-r--r--   0 grace      (501) staff       (20)      389 2024-02-19 01:05:14.000000 bonxai-0.1.0/MANIFEST.in
--rw-r--r--   0 grace      (501) staff       (20)     1829 2024-04-02 16:42:27.617566 bonxai-0.1.0/PKG-INFO
--rw-r--r--   0 grace      (501) staff       (20)      758 2024-02-19 01:05:14.000000 bonxai-0.1.0/README.md
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.588516 bonxai-0.1.0/bonxai/
--rw-r--r--   0 grace      (501) staff       (20)     1655 2024-02-19 01:20:17.000000 bonxai-0.1.0/bonxai/__init__.py
--rw-r--r--   0 grace      (501) staff       (20)       67 2024-04-02 16:39:54.000000 bonxai-0.1.0/bonxai/_version.py
--rw-r--r--   0 grace      (501) staff       (20)     1283 2024-02-19 01:05:14.000000 bonxai-0.1.0/bonxai/example.py
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.593270 bonxai-0.1.0/bonxai/labextension/
--rw-r--r--   0 grace      (501) staff       (20)     1742 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/package.json
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.602710 bonxai-0.1.0/bonxai/labextension/static/
--rw-r--r--   0 grace      (501) staff       (20)     3825 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/108.23ad6e269281ac8fcc48.js
--rw-r--r--   0 grace      (501) staff       (20)    24617 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/132.94d3969a67cfb47cbbdb.js
--rw-r--r--   0 grace      (501) staff       (20)      344 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/285.8217fca0e09a88793c35.js
--rw-r--r--   0 grace      (501) staff       (20)     4094 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/344.812f20d8164116c2af7c.js
--rw-r--r--   0 grace      (501) staff       (20)     9717 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/384.1f5603aca89b72e166df.js
--rw-r--r--   0 grace      (501) staff       (20)      583 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/493.34aef21d5d25d4977fa3.js
--rw-r--r--   0 grace      (501) staff       (20)   186252 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js
--rw-r--r--   0 grace      (501) staff       (20)      667 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js.LICENSE.txt
--rw-r--r--   0 grace      (501) staff       (20)   282224 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/693.a16a48e43b121674a96e.js
--rw-r--r--   0 grace      (501) staff       (20)     3825 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/727.7c9b1efcbca8326e44e9.js
--rw-r--r--   0 grace      (501) staff       (20)    11034 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/868.8c5d3421dde8e45893be.js
--rw-r--r--   0 grace      (501) staff       (20)     7448 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/871.0685090689ea8f246831.js
--rw-r--r--   0 grace      (501) staff       (20)      246 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/871.0685090689ea8f246831.js.LICENSE.txt
--rw-r--r--   0 grace      (501) staff       (20)     8488 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/remoteEntry.4306fab7b58084a21b84.js
--rw-r--r--   0 grace      (501) staff       (20)      118 2024-04-02 16:42:17.000000 bonxai-0.1.0/bonxai/labextension/static/style.js
--rw-r--r--   0 grace      (501) staff       (20)    66084 2024-04-02 16:42:25.000000 bonxai-0.1.0/bonxai/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.605704 bonxai-0.1.0/bonxai/nbextension/
--rw-r--r--   0 grace      (501) staff       (20)      521 2024-04-02 16:41:24.000000 bonxai-0.1.0/bonxai/nbextension/extension.js
--rw-r--r--   0 grace      (501) staff       (20)   659357 2024-04-02 16:41:39.000000 bonxai-0.1.0/bonxai/nbextension/index.js
--rw-r--r--   0 grace      (501) staff       (20)     1636 2024-04-02 16:41:39.000000 bonxai-0.1.0/bonxai/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 grace      (501) staff       (20)    10283 2024-04-02 14:58:30.000000 bonxai-0.1.0/bonxai/widget.py
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.617088 bonxai-0.1.0/bonxai.egg-info/
--rw-r--r--   0 grace      (501) staff       (20)     1829 2024-04-02 16:42:26.000000 bonxai-0.1.0/bonxai.egg-info/PKG-INFO
--rw-r--r--   0 grace      (501) staff       (20)     1784 2024-04-02 16:42:27.000000 bonxai-0.1.0/bonxai.egg-info/SOURCES.txt
--rw-r--r--   0 grace      (501) staff       (20)        1 2024-04-02 16:42:26.000000 bonxai-0.1.0/bonxai.egg-info/dependency_links.txt
--rw-r--r--   0 grace      (501) staff       (20)        1 2024-02-19 01:31:04.000000 bonxai-0.1.0/bonxai.egg-info/not-zip-safe
--rw-r--r--   0 grace      (501) staff       (20)       21 2024-04-02 16:42:26.000000 bonxai-0.1.0/bonxai.egg-info/requires.txt
--rw-r--r--   0 grace      (501) staff       (20)        7 2024-04-02 16:42:26.000000 bonxai-0.1.0/bonxai.egg-info/top_level.txt
--rw-r--r--   0 grace      (501) staff       (20)       60 2024-02-19 01:05:14.000000 bonxai-0.1.0/bonxai.json
--rw-r--r--   0 grace      (501) staff       (20)      172 2024-02-19 01:05:14.000000 bonxai-0.1.0/install.json
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.608456 bonxai-0.1.0/js/
--rw-r--r--   0 grace      (501) staff       (20)      152 2024-02-19 01:05:14.000000 bonxai-0.1.0/js/README.md
--rw-r--r--   0 grace      (501) staff       (20)      647 2024-02-19 01:05:14.000000 bonxai-0.1.0/js/amd-public-path.js
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.611484 bonxai-0.1.0/js/dist/
--rw-r--r--   0 grace      (501) staff       (20)   659357 2024-04-02 16:41:38.000000 bonxai-0.1.0/js/dist/index.js
--rw-r--r--   0 grace      (501) staff       (20)     1636 2024-04-02 16:41:38.000000 bonxai-0.1.0/js/dist/index.js.LICENSE.txt
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.614186 bonxai-0.1.0/js/lib/
--rw-r--r--   0 grace      (501) staff       (20)     1257 2024-02-19 01:05:14.000000 bonxai-0.1.0/js/lib/example.js
--rw-r--r--   0 grace      (501) staff       (20)      449 2024-02-19 01:05:14.000000 bonxai-0.1.0/js/lib/extension.js
--rw-r--r--   0 grace      (501) staff       (20)      258 2024-02-20 02:10:45.000000 bonxai-0.1.0/js/lib/index.js
--rw-r--r--   0 grace      (501) staff       (20)      649 2024-02-20 02:10:17.000000 bonxai-0.1.0/js/lib/labplugin.js
-drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-02 16:42:27.616704 bonxai-0.1.0/js/lib/lib/
--rw-r--r--   0 grace      (501) staff       (20)     5918 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/DataExplorer.js
--rw-r--r--   0 grace      (501) staff       (20)     6363 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/DataSelector.js
--rw-r--r--   0 grace      (501) staff       (20)     8659 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/DataTable.js
--rw-r--r--   0 grace      (501) staff       (20)    10236 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/HistogramVis.js
--rw-r--r--   0 grace      (501) staff       (20)     1845 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/InferenceExplorer.js
--rw-r--r--   0 grace      (501) staff       (20)     2465 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/Search.js
--rw-r--r--   0 grace      (501) staff       (20)     3537 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/SelectedTable.js
--rw-r--r--   0 grace      (501) staff       (20)     7212 2024-04-02 14:58:42.000000 bonxai-0.1.0/js/lib/lib/UMAPVis.js
--rw-r--r--   0 grace      (501) staff       (20)     5012 2024-04-02 16:32:04.000000 bonxai-0.1.0/js/lib/react.js
--rw-r--r--   0 grace      (501) staff       (20)     1626 2024-04-02 16:31:02.000000 bonxai-0.1.0/js/package.json
--rw-r--r--   0 grace      (501) staff       (20)     2813 2024-02-19 01:05:14.000000 bonxai-0.1.0/js/webpack.config.js
--rw-r--r--   0 grace      (501) staff       (20)   134927 2024-04-02 16:37:20.000000 bonxai-0.1.0/js/yarn.lock
--rw-r--r--   0 grace      (501) staff       (20)      145 2024-02-19 01:05:14.000000 bonxai-0.1.0/pyproject.toml
--rw-r--r--   0 grace      (501) staff       (20)     1107 2024-04-02 16:42:27.619125 bonxai-0.1.0/setup.cfg
--rw-r--r--   0 grace      (501) staff       (20)      891 2024-02-19 01:05:14.000000 bonxai-0.1.0/setup.py
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.139449 bonxai-0.1.1/
+-rw-r--r--   0 grace      (501) staff       (20)      389 2024-02-19 01:05:14.000000 bonxai-0.1.1/MANIFEST.in
+-rw-r--r--   0 grace      (501) staff       (20)     1829 2024-04-05 15:44:09.139216 bonxai-0.1.1/PKG-INFO
+-rw-r--r--   0 grace      (501) staff       (20)      758 2024-02-19 01:05:14.000000 bonxai-0.1.1/README.md
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.104578 bonxai-0.1.1/bonxai/
+-rw-r--r--   0 grace      (501) staff       (20)     1655 2024-02-19 01:20:17.000000 bonxai-0.1.1/bonxai/__init__.py
+-rw-r--r--   0 grace      (501) staff       (20)       67 2024-04-02 21:32:50.000000 bonxai-0.1.1/bonxai/_version.py
+-rw-r--r--   0 grace      (501) staff       (20)     1283 2024-02-19 01:05:14.000000 bonxai-0.1.1/bonxai/example.py
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.109391 bonxai-0.1.1/bonxai/labextension/
+-rw-r--r--   0 grace      (501) staff       (20)     1742 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/package.json
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.119085 bonxai-0.1.1/bonxai/labextension/static/
+-rw-r--r--   0 grace      (501) staff       (20)     3825 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/108.23ad6e269281ac8fcc48.js
+-rw-r--r--   0 grace      (501) staff       (20)    24617 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/132.94d3969a67cfb47cbbdb.js
+-rw-r--r--   0 grace      (501) staff       (20)      344 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/285.8217fca0e09a88793c35.js
+-rw-r--r--   0 grace      (501) staff       (20)     4094 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/344.812f20d8164116c2af7c.js
+-rw-r--r--   0 grace      (501) staff       (20)     9717 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/384.1f5603aca89b72e166df.js
+-rw-r--r--   0 grace      (501) staff       (20)      583 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/493.34aef21d5d25d4977fa3.js
+-rw-r--r--   0 grace      (501) staff       (20)   186252 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js
+-rw-r--r--   0 grace      (501) staff       (20)      667 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js.LICENSE.txt
+-rw-r--r--   0 grace      (501) staff       (20)   282224 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/693.a16a48e43b121674a96e.js
+-rw-r--r--   0 grace      (501) staff       (20)     3825 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/727.7c9b1efcbca8326e44e9.js
+-rw-r--r--   0 grace      (501) staff       (20)    11034 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/868.8c5d3421dde8e45893be.js
+-rw-r--r--   0 grace      (501) staff       (20)     7448 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/871.0685090689ea8f246831.js
+-rw-r--r--   0 grace      (501) staff       (20)      246 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/871.0685090689ea8f246831.js.LICENSE.txt
+-rw-r--r--   0 grace      (501) staff       (20)     8488 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/remoteEntry.4306fab7b58084a21b84.js
+-rw-r--r--   0 grace      (501) staff       (20)      118 2024-04-05 15:44:00.000000 bonxai-0.1.1/bonxai/labextension/static/style.js
+-rw-r--r--   0 grace      (501) staff       (20)    66084 2024-04-05 15:44:07.000000 bonxai-0.1.1/bonxai/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.122381 bonxai-0.1.1/bonxai/nbextension/
+-rw-r--r--   0 grace      (501) staff       (20)      521 2024-04-05 15:43:20.000000 bonxai-0.1.1/bonxai/nbextension/extension.js
+-rw-r--r--   0 grace      (501) staff       (20)   659357 2024-04-05 15:43:31.000000 bonxai-0.1.1/bonxai/nbextension/index.js
+-rw-r--r--   0 grace      (501) staff       (20)     1636 2024-04-05 15:43:31.000000 bonxai-0.1.1/bonxai/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 grace      (501) staff       (20)    10229 2024-04-02 21:32:30.000000 bonxai-0.1.1/bonxai/widget.py
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.138711 bonxai-0.1.1/bonxai.egg-info/
+-rw-r--r--   0 grace      (501) staff       (20)     1829 2024-04-05 15:44:08.000000 bonxai-0.1.1/bonxai.egg-info/PKG-INFO
+-rw-r--r--   0 grace      (501) staff       (20)     1797 2024-04-05 15:44:09.000000 bonxai-0.1.1/bonxai.egg-info/SOURCES.txt
+-rw-r--r--   0 grace      (501) staff       (20)        1 2024-04-05 15:44:08.000000 bonxai-0.1.1/bonxai.egg-info/dependency_links.txt
+-rw-r--r--   0 grace      (501) staff       (20)        1 2024-02-19 01:31:04.000000 bonxai-0.1.1/bonxai.egg-info/not-zip-safe
+-rw-r--r--   0 grace      (501) staff       (20)       21 2024-04-05 15:44:08.000000 bonxai-0.1.1/bonxai.egg-info/requires.txt
+-rw-r--r--   0 grace      (501) staff       (20)        7 2024-04-05 15:44:08.000000 bonxai-0.1.1/bonxai.egg-info/top_level.txt
+-rw-r--r--   0 grace      (501) staff       (20)       60 2024-02-19 01:05:14.000000 bonxai-0.1.1/bonxai.json
+-rw-r--r--   0 grace      (501) staff       (20)      172 2024-02-19 01:05:14.000000 bonxai-0.1.1/install.json
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.127431 bonxai-0.1.1/js/
+-rw-r--r--   0 grace      (501) staff       (20)     6148 2024-04-04 14:32:42.000000 bonxai-0.1.1/js/.DS_Store
+-rw-r--r--   0 grace      (501) staff       (20)      152 2024-02-19 01:05:14.000000 bonxai-0.1.1/js/README.md
+-rw-r--r--   0 grace      (501) staff       (20)      647 2024-02-19 01:05:14.000000 bonxai-0.1.1/js/amd-public-path.js
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.131637 bonxai-0.1.1/js/dist/
+-rw-r--r--   0 grace      (501) staff       (20)   659357 2024-04-05 15:43:32.000000 bonxai-0.1.1/js/dist/index.js
+-rw-r--r--   0 grace      (501) staff       (20)     1636 2024-04-05 15:43:32.000000 bonxai-0.1.1/js/dist/index.js.LICENSE.txt
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.135071 bonxai-0.1.1/js/lib/
+-rw-r--r--   0 grace      (501) staff       (20)     1257 2024-02-19 01:05:14.000000 bonxai-0.1.1/js/lib/example.js
+-rw-r--r--   0 grace      (501) staff       (20)      449 2024-02-19 01:05:14.000000 bonxai-0.1.1/js/lib/extension.js
+-rw-r--r--   0 grace      (501) staff       (20)      258 2024-02-20 02:10:45.000000 bonxai-0.1.1/js/lib/index.js
+-rw-r--r--   0 grace      (501) staff       (20)      649 2024-02-20 02:10:17.000000 bonxai-0.1.1/js/lib/labplugin.js
+drwxr-xr-x   0 grace      (501) staff       (20)        0 2024-04-05 15:44:09.138266 bonxai-0.1.1/js/lib/lib/
+-rw-r--r--   0 grace      (501) staff       (20)     5918 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/DataExplorer.js
+-rw-r--r--   0 grace      (501) staff       (20)     6363 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/DataSelector.js
+-rw-r--r--   0 grace      (501) staff       (20)     8659 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/DataTable.js
+-rw-r--r--   0 grace      (501) staff       (20)    10236 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/HistogramVis.js
+-rw-r--r--   0 grace      (501) staff       (20)     1845 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/InferenceExplorer.js
+-rw-r--r--   0 grace      (501) staff       (20)     2465 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/Search.js
+-rw-r--r--   0 grace      (501) staff       (20)     3537 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/SelectedTable.js
+-rw-r--r--   0 grace      (501) staff       (20)     7212 2024-04-02 14:58:42.000000 bonxai-0.1.1/js/lib/lib/UMAPVis.js
+-rw-r--r--   0 grace      (501) staff       (20)     5012 2024-04-02 16:32:04.000000 bonxai-0.1.1/js/lib/react.js
+-rw-r--r--   0 grace      (501) staff       (20)     1626 2024-04-02 16:31:02.000000 bonxai-0.1.1/js/package.json
+-rw-r--r--   0 grace      (501) staff       (20)     2813 2024-02-19 01:05:14.000000 bonxai-0.1.1/js/webpack.config.js
+-rw-r--r--   0 grace      (501) staff       (20)   134927 2024-04-02 16:37:20.000000 bonxai-0.1.1/js/yarn.lock
+-rw-r--r--   0 grace      (501) staff       (20)      145 2024-02-19 01:05:14.000000 bonxai-0.1.1/pyproject.toml
+-rw-r--r--   0 grace      (501) staff       (20)     1107 2024-04-05 15:44:09.140246 bonxai-0.1.1/setup.cfg
+-rw-r--r--   0 grace      (501) staff       (20)      891 2024-02-19 01:05:14.000000 bonxai-0.1.1/setup.py
```

### Comparing `bonxai-0.1.0/PKG-INFO` & `bonxai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonxai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com//bonxai
 Author: 
 Author-email: 
 License: BSD 3-Clause License
 Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bonxai-0.1.0/README.md` & `bonxai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/__init__.py` & `bonxai-0.1.1/bonxai/__init__.py`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/example.py` & `bonxai-0.1.1/bonxai/example.py`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/package.json` & `bonxai-0.1.1/bonxai/labextension/package.json`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/108.23ad6e269281ac8fcc48.js` & `bonxai-0.1.1/bonxai/labextension/static/108.23ad6e269281ac8fcc48.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/132.94d3969a67cfb47cbbdb.js` & `bonxai-0.1.1/bonxai/labextension/static/132.94d3969a67cfb47cbbdb.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/344.812f20d8164116c2af7c.js` & `bonxai-0.1.1/bonxai/labextension/static/344.812f20d8164116c2af7c.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/384.1f5603aca89b72e166df.js` & `bonxai-0.1.1/bonxai/labextension/static/384.1f5603aca89b72e166df.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/493.34aef21d5d25d4977fa3.js` & `bonxai-0.1.1/bonxai/labextension/static/493.34aef21d5d25d4977fa3.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js` & `bonxai-0.1.1/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js.LICENSE.txt` & `bonxai-0.1.1/bonxai/labextension/static/600.15ca81d21dc08dd850d4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/693.a16a48e43b121674a96e.js` & `bonxai-0.1.1/bonxai/labextension/static/693.a16a48e43b121674a96e.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/727.7c9b1efcbca8326e44e9.js` & `bonxai-0.1.1/bonxai/labextension/static/727.7c9b1efcbca8326e44e9.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/868.8c5d3421dde8e45893be.js` & `bonxai-0.1.1/bonxai/labextension/static/868.8c5d3421dde8e45893be.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/871.0685090689ea8f246831.js` & `bonxai-0.1.1/bonxai/labextension/static/871.0685090689ea8f246831.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/remoteEntry.4306fab7b58084a21b84.js` & `bonxai-0.1.1/bonxai/labextension/static/remoteEntry.4306fab7b58084a21b84.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/labextension/static/third-party-licenses.json` & `bonxai-0.1.1/bonxai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/nbextension/extension.js` & `bonxai-0.1.1/bonxai/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/nbextension/index.js` & `bonxai-0.1.1/bonxai/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/nbextension/index.js.LICENSE.txt` & `bonxai-0.1.1/bonxai/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/bonxai/widget.py` & `bonxai-0.1.1/bonxai/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import pandas as pd
 from datasets import Dataset, Features
-from sentence_transformers import SentenceTransformer
 from transformers import pipeline
 import umap
 import torch
 
 import ipywidgets as widgets
 from traitlets import Unicode, Dict, List, TraitError
```

### Comparing `bonxai-0.1.0/bonxai.egg-info/PKG-INFO` & `bonxai-0.1.1/bonxai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonxai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com//bonxai
 Author: 
 Author-email: 
 License: BSD 3-Clause License
 Keywords: ipython,widgets,Jupyter,JupyterLab,JupyterLab3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bonxai-0.1.0/bonxai.egg-info/SOURCES.txt` & `bonxai-0.1.1/bonxai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 bonxai/labextension/static/871.0685090689ea8f246831.js.LICENSE.txt
 bonxai/labextension/static/remoteEntry.4306fab7b58084a21b84.js
 bonxai/labextension/static/style.js
 bonxai/labextension/static/third-party-licenses.json
 bonxai/nbextension/extension.js
 bonxai/nbextension/index.js
 bonxai/nbextension/index.js.LICENSE.txt
+js/.DS_Store
 js/README.md
 js/amd-public-path.js
 js/package.json
 js/webpack.config.js
 js/yarn.lock
 js/dist/index.js
 js/dist/index.js.LICENSE.txt
```

### Comparing `bonxai-0.1.0/js/amd-public-path.js` & `bonxai-0.1.1/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/dist/index.js` & `bonxai-0.1.1/js/dist/index.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/dist/index.js.LICENSE.txt` & `bonxai-0.1.1/js/dist/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/example.js` & `bonxai-0.1.1/js/lib/example.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/labplugin.js` & `bonxai-0.1.1/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/DataExplorer.js` & `bonxai-0.1.1/js/lib/lib/DataExplorer.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/DataSelector.js` & `bonxai-0.1.1/js/lib/lib/DataSelector.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/DataTable.js` & `bonxai-0.1.1/js/lib/lib/DataTable.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/HistogramVis.js` & `bonxai-0.1.1/js/lib/lib/HistogramVis.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/InferenceExplorer.js` & `bonxai-0.1.1/js/lib/lib/InferenceExplorer.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/Search.js` & `bonxai-0.1.1/js/lib/lib/Search.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/SelectedTable.js` & `bonxai-0.1.1/js/lib/lib/SelectedTable.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/lib/UMAPVis.js` & `bonxai-0.1.1/js/lib/lib/UMAPVis.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/lib/react.js` & `bonxai-0.1.1/js/lib/react.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/package.json` & `bonxai-0.1.1/js/package.json`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/webpack.config.js` & `bonxai-0.1.1/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/js/yarn.lock` & `bonxai-0.1.1/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/setup.cfg` & `bonxai-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bonxai-0.1.0/setup.py` & `bonxai-0.1.1/setup.py`

 * *Files identical despite different names*

