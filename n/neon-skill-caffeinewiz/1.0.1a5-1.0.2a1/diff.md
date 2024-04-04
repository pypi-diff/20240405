# Comparing `tmp/neon-skill-caffeinewiz-1.0.1a5.tar.gz` & `tmp/neon-skill-caffeinewiz-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-caffeinewiz-1.0.1a5.tar", last modified: Fri Mar  1 23:49:40 2024, max compression
+gzip compressed data, was "neon-skill-caffeinewiz-1.0.2a1.tar", last modified: Thu Apr  4 22:23:26 2024, max compression
```

## Comparing `neon-skill-caffeinewiz-1.0.1a5.tar` & `neon-skill-caffeinewiz-1.0.2a1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24730 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/data/
--rw-r--r--   0 runner    (1001) docker     (127)    31954 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/data/caffeine_wiz_data.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/dialog/drink_caffeine.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/regex/drink.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/goodbye.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/de-de/vocab/query_caffeine.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.750771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/drink_caffeine.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/how_about_more.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/more_drinks.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/multiple_drinks.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/no_drink_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/not_found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/provided_by_caffeinewiz.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/stay_caffeinated.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/update_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/update_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/updating.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_liter.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_milligrams.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_milliliters.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/dialog/word_ounces.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/regex/drink.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/caffeine.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/goodbye.voc
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/query_caffeine.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/locale/en-us/vocab/update_caffeine.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-01 23:49:40.000000 neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 23:49:40.758771 neon-skill-caffeinewiz-1.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:49:40.754771 neon-skill-caffeinewiz-1.0.1a5/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-01 23:49:34.000000 neon-skill-caffeinewiz-1.0.1a5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    31954 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/data/caffeine_wiz_data.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/dialog/drink_caffeine.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/regex/drink.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/vocab/goodbye.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/de-de/vocab/query_caffeine.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.203739 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/drink_caffeine.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/how_about_more.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/more_drinks.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/multiple_drinks.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/no_drink_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/not_found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/provided_by_caffeinewiz.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/stay_caffeinated.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/update_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/update_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/word_liter.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/word_milligrams.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/word_milliliters.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/dialog/word_ounces.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/regex/drink.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/vocab/caffeine.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/vocab/goodbye.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/vocab/query_caffeine.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/locale/en-us/vocab/update_caffeine.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 22:23:26.000000 neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:23:26.207738 neon-skill-caffeinewiz-1.0.2a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-04 22:23:21.000000 neon-skill-caffeinewiz-1.0.2a1/version.py
```

### Comparing `neon-skill-caffeinewiz-1.0.1a5/LICENSE.md` & `neon-skill-caffeinewiz-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/PKG-INFO` & `neon-skill-caffeinewiz-1.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-caffeinewiz
-Version: 1.0.1a5
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-caffeinewiz
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-caffeinewiz-1.0.1a5/README.md` & `neon-skill-caffeinewiz-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/__init__.py` & `neon-skill-caffeinewiz-1.0.2a1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,14 @@
             }
 
         self.default_intent_timeout = 60
         self.from_caffeine_wiz = list()
         self.from_caffeine_informer = list()
         self._update_event = Event()
         CommonQuerySkill.__init__(self, **kwargs)
-        from neon_utils.signal_utils import init_signal_bus
-        init_signal_bus(self.bus)
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
@@ -267,17 +265,14 @@
         results = data.get("results")
         message = Message.deserialize(data.get("message")) if \
             data.get("message") else None
         if results:
             if len(results) == 1:
                 self.speak_dialog("stay_caffeinated")
             else:
-                # TODO: This is patching poor handling in get_response
-                from neon_utils.signal_utils import wait_for_signal_clear
-                wait_for_signal_clear("isSpeaking", 30)
                 if self.ask_yesno("more_drinks") == "yes":
                     LOG.info("YES")
                     self._speak_alternate_results(message, results)
                     self.speak_dialog("provided_by_caffeinewiz")
                 else:
                     LOG.info("NO")
                     self.speak_dialog("stay_caffeinated")
@@ -357,18 +352,19 @@
                     caff_mg = str(caffeine)
                     caff_vol = str(oz)
                     unit_dialog = 'word_ounces'
 
                 self.speak_dialog('multiple_drinks',
                                   {'drink': drink,
                                    'caffeine_content': caff_mg,
-                                   'caffeine_units': self.translate(
+                                   'caffeine_units': self.resources.render_dialog(
                                        'word_milligrams'),
                                    'drink_size': caff_vol,
-                                   'drink_units': self.translate(unit_dialog)})
+                                   'drink_units': self.resources.render_dialog(
+                                       unit_dialog)})
                 spoken.append(caff_list[i][0])
                 sleep(0.5)  # Prevent simultaneous speak inserts
             cnt = cnt + 1
 
     def _add_more_caffeine_data(self):
         """
         Add in some arbitrary additional data.
@@ -557,11 +553,11 @@
             caff_vol = str(caff_oz)
             unit_dialog = 'word_ounces'
 
         LOG.info(f"{drink} | {caff_mg} | {caff_vol} | {unit_dialog}")
         to_speak = self.dialog_renderer.render('drink_caffeine', {
             'drink': drink,
             'caffeine_content': caff_mg,
-            'caffeine_units': self.translate('word_milligrams'),
+            'caffeine_units': self.resources.render_dialog('word_milligrams'),
             'drink_size': caff_vol,
-            'drink_units': self.translate(unit_dialog)})
+            'drink_units': self.resources.render_dialog(unit_dialog)})
         return to_speak, results
```

### Comparing `neon-skill-caffeinewiz-1.0.1a5/data/caffeine_wiz_data.pickle` & `neon-skill-caffeinewiz-1.0.2a1/data/caffeine_wiz_data.pickle`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/PKG-INFO` & `neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-caffeinewiz
-Version: 1.0.1a5
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-caffeinewiz
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-caffeinewiz-1.0.1a5/neon_skill_caffeinewiz.egg-info/SOURCES.txt` & `neon-skill-caffeinewiz-1.0.2a1/neon_skill_caffeinewiz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/setup.py` & `neon-skill-caffeinewiz-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/skill.json` & `neon-skill-caffeinewiz-1.0.2a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/test/test_skill.py` & `neon-skill-caffeinewiz-1.0.2a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-caffeinewiz-1.0.1a5/version.py` & `neon-skill-caffeinewiz-1.0.2a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a5"
+__version__ = "1.0.2a1"
```

