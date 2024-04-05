# Comparing `tmp/botw_flag_util-0.3.6.tar.gz` & `tmp/botw_flag_util-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botw_flag_util-0.3.6.tar", last modified: Thu Apr  4 23:27:39 2024, max compression
+gzip compressed data, was "botw_flag_util-0.3.7.tar", last modified: Fri Apr  5 00:45:22 2024, max compression
```

## Comparing `botw_flag_util-0.3.6.tar` & `botw_flag_util-0.3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.926700 botw_flag_util-0.3.6/
--rw-rw-rw-   0        0        0    35184 2020-08-02 17:59:47.000000 botw_flag_util-0.3.6/LICENSE
--rw-rw-rw-   0        0        0       41 2020-08-03 21:14:27.000000 botw_flag_util-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5139 2024-04-04 23:27:39.923705 botw_flag_util-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     4508 2020-10-21 04:44:09.000000 botw_flag_util-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.865800 botw_flag_util-0.3.6/botw_flag_util/
--rw-rw-rw-   0        0        0     1196 2020-10-21 04:15:32.000000 botw_flag_util-0.3.6/botw_flag_util/__init__.py
--rw-rw-rw-   0        0        0     2374 2020-11-07 06:36:49.000000 botw_flag_util-0.3.6/botw_flag_util/__main__.py
--rw-rw-rw-   0        0        0       79 2024-04-04 23:24:06.000000 botw_flag_util-0.3.6/botw_flag_util/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.919213 botw_flag_util-0.3.6/botw_flag_util/data/
--rw-rw-rw-   0        0        0     5768 2024-03-31 17:44:13.000000 botw_flag_util-0.3.6/botw_flag_util/data/overrides.json
--rw-rw-rw-   0        0        0   298979 2020-11-07 13:28:40.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_actors.json
--rw-rw-rw-   0        0        0    73792 2020-10-19 01:40:13.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_hash.json
--rw-rw-rw-   0        0        0    17070 2020-10-19 22:14:41.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_shrines.json
--rw-rw-rw-   0        0        0     2369 2021-02-13 23:11:54.000000 botw_flag_util-0.3.6/botw_flag_util/finder.py
--rw-rw-rw-   0        0        0    71132 2024-03-31 17:44:40.000000 botw_flag_util-0.3.6/botw_flag_util/flag.py
--rw-rw-rw-   0        0        0    17938 2022-07-04 09:10:09.000000 botw_flag_util-0.3.6/botw_flag_util/generator.py
--rw-rw-rw-   0        0        0     8902 2021-02-13 23:09:43.000000 botw_flag_util-0.3.6/botw_flag_util/store.py
--rw-rw-rw-   0        0        0     8409 2020-10-24 23:49:38.000000 botw_flag_util-0.3.6/botw_flag_util/util.py
-drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.921709 botw_flag_util-0.3.6/botw_flag_util.egg-info/
--rw-rw-rw-   0        0        0     5139 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 23:27:39.927200 botw_flag_util-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1024 2020-11-27 07:20:27.000000 botw_flag_util-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:22.272765 botw_flag_util-0.3.7/
+-rw-rw-rw-   0        0        0    35184 2020-08-02 17:59:47.000000 botw_flag_util-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0       41 2020-08-03 21:14:27.000000 botw_flag_util-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5139 2024-04-05 00:45:22.270792 botw_flag_util-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4508 2020-10-21 04:44:09.000000 botw_flag_util-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:22.220867 botw_flag_util-0.3.7/botw_flag_util/
+-rw-rw-rw-   0        0        0     1196 2020-10-21 04:15:32.000000 botw_flag_util-0.3.7/botw_flag_util/__init__.py
+-rw-rw-rw-   0        0        0     2374 2020-11-07 06:36:49.000000 botw_flag_util-0.3.7/botw_flag_util/__main__.py
+-rw-rw-rw-   0        0        0       79 2024-04-05 00:45:05.000000 botw_flag_util-0.3.7/botw_flag_util/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:22.266291 botw_flag_util-0.3.7/botw_flag_util/data/
+-rw-rw-rw-   0        0        0     5768 2024-03-31 17:44:13.000000 botw_flag_util-0.3.7/botw_flag_util/data/overrides.json
+-rw-rw-rw-   0        0        0   298979 2020-11-07 13:28:40.000000 botw_flag_util-0.3.7/botw_flag_util/data/vanilla_actors.json
+-rw-rw-rw-   0        0        0    73792 2020-10-19 01:40:13.000000 botw_flag_util-0.3.7/botw_flag_util/data/vanilla_hash.json
+-rw-rw-rw-   0        0        0    17070 2020-10-19 22:14:41.000000 botw_flag_util-0.3.7/botw_flag_util/data/vanilla_shrines.json
+-rw-rw-rw-   0        0        0     2369 2021-02-13 23:11:54.000000 botw_flag_util-0.3.7/botw_flag_util/finder.py
+-rw-rw-rw-   0        0        0    71131 2024-04-05 00:44:27.000000 botw_flag_util-0.3.7/botw_flag_util/flag.py
+-rw-rw-rw-   0        0        0    17938 2022-07-04 09:10:09.000000 botw_flag_util-0.3.7/botw_flag_util/generator.py
+-rw-rw-rw-   0        0        0     8902 2021-02-13 23:09:43.000000 botw_flag_util-0.3.7/botw_flag_util/store.py
+-rw-rw-rw-   0        0        0     8409 2020-10-24 23:49:38.000000 botw_flag_util-0.3.7/botw_flag_util/util.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:22.269269 botw_flag_util-0.3.7/botw_flag_util.egg-info/
+-rw-rw-rw-   0        0        0     5139 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 00:45:22.000000 botw_flag_util-0.3.7/botw_flag_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 00:45:22.272765 botw_flag_util-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2020-11-27 07:20:27.000000 botw_flag_util-0.3.7/setup.py
```

### Comparing `botw_flag_util-0.3.6/LICENSE` & `botw_flag_util-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/PKG-INFO` & `botw_flag_util-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botw_flag_util
-Version: 0.3.6
+Version: 0.3.7
 Summary: Game data and save game data flag utilities for LoZ:BotW
 Home-page: https://github.com/GingerAvalanche/botw_flag_util
 Author: Ginger
 Author-email: chodness@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `botw_flag_util-0.3.6/README.md` & `botw_flag_util-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/__init__.py` & `botw_flag_util-0.3.7/botw_flag_util/__init__.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/__main__.py` & `botw_flag_util-0.3.7/botw_flag_util/__main__.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/data/overrides.json` & `botw_flag_util-0.3.7/botw_flag_util/data/overrides.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_actors.json` & `botw_flag_util-0.3.7/botw_flag_util/data/vanilla_actors.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_hash.json` & `botw_flag_util-0.3.7/botw_flag_util/data/vanilla_hash.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_shrines.json` & `botw_flag_util-0.3.7/botw_flag_util/data/vanilla_shrines.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/finder.py` & `botw_flag_util-0.3.7/botw_flag_util/finder.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/flag.py` & `botw_flag_util-0.3.7/botw_flag_util/flag.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,15 +567,15 @@
                 self.max_value = value
         for regex, value in OVERRIDES["OVERRIDE_S32_MIN_VALUE"].items():
             if re.search(regex, self.data_name):
                 self.min_value = value
         for regex, value in OVERRIDES["OVERRIDE_S32_IS_SAVE"].items():
             if re.search(regex, self.data_name):
                 self.min_value = value
-        for regex, value in OVERRIDES["OVERRIDE_S32_RESET_VALUE"].items():
+        for regex, value in OVERRIDES["OVERRIDE_S32_RESET_TYPE"].items():
             if re.search(regex, self.data_name):
                 self.min_value = value
 
 
 class S32ArrayFlag(BFUFlag):
     def __init__(self, flag: Hash = None, **kwargs) -> None:
         super(S32ArrayFlag, self).__init__(flag=flag)
```

### Comparing `botw_flag_util-0.3.6/botw_flag_util/generator.py` & `botw_flag_util-0.3.7/botw_flag_util/generator.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/store.py` & `botw_flag_util-0.3.7/botw_flag_util/store.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util/util.py` & `botw_flag_util-0.3.7/botw_flag_util/util.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/botw_flag_util.egg-info/PKG-INFO` & `botw_flag_util-0.3.7/botw_flag_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botw_flag_util
-Version: 0.3.6
+Version: 0.3.7
 Summary: Game data and save game data flag utilities for LoZ:BotW
 Home-page: https://github.com/GingerAvalanche/botw_flag_util
 Author: Ginger
 Author-email: chodness@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `botw_flag_util-0.3.6/botw_flag_util.egg-info/SOURCES.txt` & `botw_flag_util-0.3.7/botw_flag_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.6/setup.py` & `botw_flag_util-0.3.7/setup.py`

 * *Files identical despite different names*

