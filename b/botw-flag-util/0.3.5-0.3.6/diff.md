# Comparing `tmp/botw_flag_util-0.3.5.tar.gz` & `tmp/botw_flag_util-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\botw_flag_util-0.3.5.tar", last modified: Mon Jan 31 00:52:01 2022, max compression
+gzip compressed data, was "botw_flag_util-0.3.6.tar", last modified: Thu Apr  4 23:27:39 2024, max compression
```

## Comparing `botw_flag_util-0.3.5.tar` & `botw_flag_util-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/
--rw-rw-rw-   0        0        0       41 2020-08-03 21:14:27.000000 botw_flag_util-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5506 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     4508 2020-10-21 04:44:09.000000 botw_flag_util-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/botw_flag_util/
--rw-rw-rw-   0        0        0     1196 2020-10-21 04:15:32.000000 botw_flag_util-0.3.5/botw_flag_util/__init__.py
--rw-rw-rw-   0        0        0     2374 2020-11-07 06:36:49.000000 botw_flag_util-0.3.5/botw_flag_util/__main__.py
--rw-rw-rw-   0        0        0       79 2022-01-31 00:50:18.000000 botw_flag_util-0.3.5/botw_flag_util/__version__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/botw_flag_util/data/
--rw-rw-rw-   0        0        0     5622 2020-12-06 00:49:40.000000 botw_flag_util-0.3.5/botw_flag_util/data/overrides.json
--rw-rw-rw-   0        0        0   298979 2020-11-07 13:28:40.000000 botw_flag_util-0.3.5/botw_flag_util/data/vanilla_actors.json
--rw-rw-rw-   0        0        0    73792 2020-10-19 01:40:13.000000 botw_flag_util-0.3.5/botw_flag_util/data/vanilla_hash.json
--rw-rw-rw-   0        0        0    17070 2020-10-19 22:14:41.000000 botw_flag_util-0.3.5/botw_flag_util/data/vanilla_shrines.json
--rw-rw-rw-   0        0        0     2369 2021-02-13 23:11:54.000000 botw_flag_util-0.3.5/botw_flag_util/finder.py
--rw-rw-rw-   0        0        0    70804 2021-09-03 05:32:43.000000 botw_flag_util-0.3.5/botw_flag_util/flag.py
--rw-rw-rw-   0        0        0    17938 2022-01-31 00:47:32.000000 botw_flag_util-0.3.5/botw_flag_util/generator.py
--rw-rw-rw-   0        0        0     8902 2021-02-13 23:09:43.000000 botw_flag_util-0.3.5/botw_flag_util/store.py
--rw-rw-rw-   0        0        0     8409 2020-10-24 23:49:38.000000 botw_flag_util-0.3.5/botw_flag_util/util.py
-drwxrwxrwx   0        0        0        0 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/
--rw-rw-rw-   0        0        0     5506 2022-01-31 00:52:00.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-31 00:52:00.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2022-01-31 00:52:00.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2022-01-31 00:52:00.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-01-31 00:52:00.000000 botw_flag_util-0.3.5/botw_flag_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-31 00:52:01.000000 botw_flag_util-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1024 2020-11-27 07:20:27.000000 botw_flag_util-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.926700 botw_flag_util-0.3.6/
+-rw-rw-rw-   0        0        0    35184 2020-08-02 17:59:47.000000 botw_flag_util-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0       41 2020-08-03 21:14:27.000000 botw_flag_util-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5139 2024-04-04 23:27:39.923705 botw_flag_util-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4508 2020-10-21 04:44:09.000000 botw_flag_util-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.865800 botw_flag_util-0.3.6/botw_flag_util/
+-rw-rw-rw-   0        0        0     1196 2020-10-21 04:15:32.000000 botw_flag_util-0.3.6/botw_flag_util/__init__.py
+-rw-rw-rw-   0        0        0     2374 2020-11-07 06:36:49.000000 botw_flag_util-0.3.6/botw_flag_util/__main__.py
+-rw-rw-rw-   0        0        0       79 2024-04-04 23:24:06.000000 botw_flag_util-0.3.6/botw_flag_util/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.919213 botw_flag_util-0.3.6/botw_flag_util/data/
+-rw-rw-rw-   0        0        0     5768 2024-03-31 17:44:13.000000 botw_flag_util-0.3.6/botw_flag_util/data/overrides.json
+-rw-rw-rw-   0        0        0   298979 2020-11-07 13:28:40.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_actors.json
+-rw-rw-rw-   0        0        0    73792 2020-10-19 01:40:13.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_hash.json
+-rw-rw-rw-   0        0        0    17070 2020-10-19 22:14:41.000000 botw_flag_util-0.3.6/botw_flag_util/data/vanilla_shrines.json
+-rw-rw-rw-   0        0        0     2369 2021-02-13 23:11:54.000000 botw_flag_util-0.3.6/botw_flag_util/finder.py
+-rw-rw-rw-   0        0        0    71132 2024-03-31 17:44:40.000000 botw_flag_util-0.3.6/botw_flag_util/flag.py
+-rw-rw-rw-   0        0        0    17938 2022-07-04 09:10:09.000000 botw_flag_util-0.3.6/botw_flag_util/generator.py
+-rw-rw-rw-   0        0        0     8902 2021-02-13 23:09:43.000000 botw_flag_util-0.3.6/botw_flag_util/store.py
+-rw-rw-rw-   0        0        0     8409 2020-10-24 23:49:38.000000 botw_flag_util-0.3.6/botw_flag_util/util.py
+drwxrwxrwx   0        0        0        0 2024-04-04 23:27:39.921709 botw_flag_util-0.3.6/botw_flag_util.egg-info/
+-rw-rw-rw-   0        0        0     5139 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 23:27:39.000000 botw_flag_util-0.3.6/botw_flag_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 23:27:39.927200 botw_flag_util-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2020-11-27 07:20:27.000000 botw_flag_util-0.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `botw_flag_util-0.3.5/PKG-INFO` & `botw_flag_util-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 Metadata-Version: 2.1
 Name: botw_flag_util
-Version: 0.3.5
+Version: 0.3.6
 Summary: Game data and save game data flag utilities for LoZ:BotW
 Home-page: https://github.com/GingerAvalanche/botw_flag_util
 Author: Ginger
 Author-email: chodness@gmail.com
-License: UNKNOWN
-Description: # Breath of the Wild Flag Utilities
-        Game data and save game data flag utilities for LoZ:BotW
-        
-        ## Dependencies
-        * A dumped copy of Legend of Zelda: Breath of the Wild (for Wii U or Switch)
-        * Python 3.7+ (64-bit, added to system PATH)
-        
-        The following `pip` packages, which will be automatically installed:
-        * bcml
-        * oead
-        
-        ## Setup
-        1. Download and install Python 3.7+, 64-bit. You must choose the "Add to System PATH" option during installation.
-        2. Open a command line and run `pip install botw_flag_util`
-        
-        ### How to Use
-        
-        #### Generate flags:
-        `botw_flag_util generate [path_to_mod_root] [-a] [-r # #] [-b] [-v]`
-        * `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
-        * `-a` - Generate actor flags.
-        * `-r # #` - Generate revival flags. The first number is the ResetType for MainField actors. The second is the ResetType for CDungeon (shrine) actors. If one of them is set to -1, it will skip flag generation for that field type.
-        * `-b` - Use big-endian mode. For generating flags for Wii U.
-        * `-v` - Use verbose mode. Will give more verbose after-action report.
-        
-        #### Find flags:
-        `botw_flag_util find [path_to_mod_root] [search_name] [-b] [-v]`
-        * `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
-        * `search_name` - The name of the flag to search for. Will find all flags whose DataName contains `search_name`. For example, `MainField_Npc_HiddenKorok` will find all Korok NPC flags.
-        * `-b` - Use big-endian mode. For deleting flags for Wii U.
-        * `-v` - Use verbose mode. Will give more verbose after-action report.
-        
-        Once the search has been completed, you will be told how many game data and save data flags were found that matched `search_name`. You will then be given three choices:
-        * `v` - View more detailed information on the flags found: their full names and their types, and then prompt for another choice.
-        * `d` - Delete all the flags that were found by this search, and then return to the command line.
-        * `x` - Return to the command line.
-        
-        ##### Quirks
-        * `botw_flag_util` does not need a Bootup.pack present in your mod to do its thing. If one is not present, it will copy it from your game dump into your mod files and then edit that copy.
-        * A new copy of gamedata.ssarc and savedataformat.ssarc will always be written to Bootup.pack, even if no changes were made. This is done so that any invalid flags (e.g. duplicate flags) will be deleted from them. Invalid flags will cause BOTW to perform abnormally. This feature was included by request, and should never harm anything, but if you notice that your Bootup.pack's modified date has changed after no changes were made, this is why.
-        * Knowing which flags to give what properties is a very complicated affair. Rather than try to retrieve all that information from the data files, a stopgap has been developed: inside the `data` folder, where `botw_flag_util` is installed, is a file called `overrides.json`. In this file is a comprehensive set of override conditions. If you have come across any flags that you notice are receiving incorrect values, you may place the flag name inside the dictionary for the correspond flag type/property and give it a value. Any flags with that name as part of their name will receive that value for that property, overriding whatever standard logic applies to that flag during the generation process. For example, inside OVERRIDE_IS_ONE_SAVE is the name/value `"IsGet_": true`. This means that all flags with `IsGet_` in the name will have their `IsSave` property set to `true`. You can modify this file whenever you want, and as long as it is valid JSON and the values are valid for the properties they're being inserted into, the values will be properly overridden. `If you use this feature to create a more comprehensive ruleset for flag generation, please consider opening a PR on GitHub so that others may benefit from it as well.`
-        
-        ## Contributing
-        * Issues: https://github.com/GingerAvalanche/botw_flag_util/issues
-        * Source: https://github.com/GingerAvalanche/botw_flag_util
-        
-        This software is in early, but usable, beta. There are several variable types that are not yet handled, and several cases that are not handled for the variable types that are handled. Feel free to contribute in any way.
-        
-        ## License
-        This software is licensed under the terms of the GNU Affero General Public License, version 3+. The source is publicly available on Github.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: bcml>=3.0.0b25
+Requires-Dist: oead>=0.11.2
+
+# Breath of the Wild Flag Utilities
+Game data and save game data flag utilities for LoZ:BotW
+
+## Dependencies
+* A dumped copy of Legend of Zelda: Breath of the Wild (for Wii U or Switch)
+* Python 3.7+ (64-bit, added to system PATH)
+
+The following `pip` packages, which will be automatically installed:
+* bcml
+* oead
+
+## Setup
+1. Download and install Python 3.7+, 64-bit. You must choose the "Add to System PATH" option during installation.
+2. Open a command line and run `pip install botw_flag_util`
+
+### How to Use
+
+#### Generate flags:
+`botw_flag_util generate [path_to_mod_root] [-a] [-r # #] [-b] [-v]`
+* `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
+* `-a` - Generate actor flags.
+* `-r # #` - Generate revival flags. The first number is the ResetType for MainField actors. The second is the ResetType for CDungeon (shrine) actors. If one of them is set to -1, it will skip flag generation for that field type.
+* `-b` - Use big-endian mode. For generating flags for Wii U.
+* `-v` - Use verbose mode. Will give more verbose after-action report.
+
+#### Find flags:
+`botw_flag_util find [path_to_mod_root] [search_name] [-b] [-v]`
+* `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
+* `search_name` - The name of the flag to search for. Will find all flags whose DataName contains `search_name`. For example, `MainField_Npc_HiddenKorok` will find all Korok NPC flags.
+* `-b` - Use big-endian mode. For deleting flags for Wii U.
+* `-v` - Use verbose mode. Will give more verbose after-action report.
+
+Once the search has been completed, you will be told how many game data and save data flags were found that matched `search_name`. You will then be given three choices:
+* `v` - View more detailed information on the flags found: their full names and their types, and then prompt for another choice.
+* `d` - Delete all the flags that were found by this search, and then return to the command line.
+* `x` - Return to the command line.
+
+##### Quirks
+* `botw_flag_util` does not need a Bootup.pack present in your mod to do its thing. If one is not present, it will copy it from your game dump into your mod files and then edit that copy.
+* A new copy of gamedata.ssarc and savedataformat.ssarc will always be written to Bootup.pack, even if no changes were made. This is done so that any invalid flags (e.g. duplicate flags) will be deleted from them. Invalid flags will cause BOTW to perform abnormally. This feature was included by request, and should never harm anything, but if you notice that your Bootup.pack's modified date has changed after no changes were made, this is why.
+* Knowing which flags to give what properties is a very complicated affair. Rather than try to retrieve all that information from the data files, a stopgap has been developed: inside the `data` folder, where `botw_flag_util` is installed, is a file called `overrides.json`. In this file is a comprehensive set of override conditions. If you have come across any flags that you notice are receiving incorrect values, you may place the flag name inside the dictionary for the correspond flag type/property and give it a value. Any flags with that name as part of their name will receive that value for that property, overriding whatever standard logic applies to that flag during the generation process. For example, inside OVERRIDE_IS_ONE_SAVE is the name/value `"IsGet_": true`. This means that all flags with `IsGet_` in the name will have their `IsSave` property set to `true`. You can modify this file whenever you want, and as long as it is valid JSON and the values are valid for the properties they're being inserted into, the values will be properly overridden. `If you use this feature to create a more comprehensive ruleset for flag generation, please consider opening a PR on GitHub so that others may benefit from it as well.`
+
+## Contributing
+* Issues: https://github.com/GingerAvalanche/botw_flag_util/issues
+* Source: https://github.com/GingerAvalanche/botw_flag_util
+
+This software is in early, but usable, beta. There are several variable types that are not yet handled, and several cases that are not handled for the variable types that are handled. Feel free to contribute in any way.
+
+## License
+This software is licensed under the terms of the GNU Affero General Public License, version 3+. The source is publicly available on Github.
```

### Comparing `botw_flag_util-0.3.5/README.md` & `botw_flag_util-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/__init__.py` & `botw_flag_util-0.3.6/botw_flag_util/__init__.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/__main__.py` & `botw_flag_util-0.3.6/botw_flag_util/__main__.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/data/overrides.json` & `botw_flag_util-0.3.6/botw_flag_util/data/overrides.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'S32_OVERRIDES'": "{'OVERRIDE_S32_IS_SAVE': OrderedDict([('Npc_', True)]), "*

 * *                    "'OVERRIDE_S32_RESET_TYPE': OrderedDict([('Npc_', 3)])}"}*

```diff
@@ -58,27 +58,33 @@
             "EquipTime_": 0,
             "Location_": 0,
             "Location_StartPoint": 1,
             "Npc_": 0,
             "PictureBookSize_": -1,
             "PorchTime_": 0
         },
+        "OVERRIDE_S32_IS_SAVE": {
+            "Npc_": true
+        },
         "OVERRIDE_S32_MAX_VALUE": {
             "EquipTime_": 2147483647,
             "Location_": 2147483647,
             "Npc_": 65535,
             "PictureBookSize_": 65536,
             "PorchTime_": 2147483647
         },
         "OVERRIDE_S32_MIN_VALUE": {
             "EquipTime_": 0,
             "Location_": -2147483648,
             "Npc_": 0,
             "PictureBookSize_": -1,
             "PorchTime_": 0
+        },
+        "OVERRIDE_S32_RESET_TYPE": {
+            "Npc_": 3
         }
     },
     "STANDARD_OVERRIDES": {
         "OVERRIDE_IS_EVENT_ASSOCIATED": {
             "IsInside_Dungeon": true,
             "MapTower_07_Demo": false
         },
```

### Comparing `botw_flag_util-0.3.5/botw_flag_util/data/vanilla_actors.json` & `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_actors.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/data/vanilla_hash.json` & `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_hash.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/data/vanilla_shrines.json` & `botw_flag_util-0.3.6/botw_flag_util/data/vanilla_shrines.json`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/finder.py` & `botw_flag_util-0.3.6/botw_flag_util/finder.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/flag.py` & `botw_flag_util-0.3.6/botw_flag_util/flag.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,14 +564,20 @@
                 self.init_value = value
         for regex, value in OVERRIDES["OVERRIDE_S32_MAX_VALUE"].items():
             if re.search(regex, self.data_name):
                 self.max_value = value
         for regex, value in OVERRIDES["OVERRIDE_S32_MIN_VALUE"].items():
             if re.search(regex, self.data_name):
                 self.min_value = value
+        for regex, value in OVERRIDES["OVERRIDE_S32_IS_SAVE"].items():
+            if re.search(regex, self.data_name):
+                self.min_value = value
+        for regex, value in OVERRIDES["OVERRIDE_S32_RESET_VALUE"].items():
+            if re.search(regex, self.data_name):
+                self.min_value = value
 
 
 class S32ArrayFlag(BFUFlag):
     def __init__(self, flag: Hash = None, **kwargs) -> None:
         super(S32ArrayFlag, self).__init__(flag=flag)
         self.init_value = [0]
         self.max_value = 6553500
```

### Comparing `botw_flag_util-0.3.5/botw_flag_util/generator.py` & `botw_flag_util-0.3.6/botw_flag_util/generator.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/store.py` & `botw_flag_util-0.3.6/botw_flag_util/store.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util/util.py` & `botw_flag_util-0.3.6/botw_flag_util/util.py`

 * *Files identical despite different names*

### Comparing `botw_flag_util-0.3.5/botw_flag_util.egg-info/PKG-INFO` & `botw_flag_util-0.3.6/botw_flag_util.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 Metadata-Version: 2.1
-Name: botw-flag-util
-Version: 0.3.5
+Name: botw_flag_util
+Version: 0.3.6
 Summary: Game data and save game data flag utilities for LoZ:BotW
 Home-page: https://github.com/GingerAvalanche/botw_flag_util
 Author: Ginger
 Author-email: chodness@gmail.com
-License: UNKNOWN
-Description: # Breath of the Wild Flag Utilities
-        Game data and save game data flag utilities for LoZ:BotW
-        
-        ## Dependencies
-        * A dumped copy of Legend of Zelda: Breath of the Wild (for Wii U or Switch)
-        * Python 3.7+ (64-bit, added to system PATH)
-        
-        The following `pip` packages, which will be automatically installed:
-        * bcml
-        * oead
-        
-        ## Setup
-        1. Download and install Python 3.7+, 64-bit. You must choose the "Add to System PATH" option during installation.
-        2. Open a command line and run `pip install botw_flag_util`
-        
-        ### How to Use
-        
-        #### Generate flags:
-        `botw_flag_util generate [path_to_mod_root] [-a] [-r # #] [-b] [-v]`
-        * `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
-        * `-a` - Generate actor flags.
-        * `-r # #` - Generate revival flags. The first number is the ResetType for MainField actors. The second is the ResetType for CDungeon (shrine) actors. If one of them is set to -1, it will skip flag generation for that field type.
-        * `-b` - Use big-endian mode. For generating flags for Wii U.
-        * `-v` - Use verbose mode. Will give more verbose after-action report.
-        
-        #### Find flags:
-        `botw_flag_util find [path_to_mod_root] [search_name] [-b] [-v]`
-        * `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
-        * `search_name` - The name of the flag to search for. Will find all flags whose DataName contains `search_name`. For example, `MainField_Npc_HiddenKorok` will find all Korok NPC flags.
-        * `-b` - Use big-endian mode. For deleting flags for Wii U.
-        * `-v` - Use verbose mode. Will give more verbose after-action report.
-        
-        Once the search has been completed, you will be told how many game data and save data flags were found that matched `search_name`. You will then be given three choices:
-        * `v` - View more detailed information on the flags found: their full names and their types, and then prompt for another choice.
-        * `d` - Delete all the flags that were found by this search, and then return to the command line.
-        * `x` - Return to the command line.
-        
-        ##### Quirks
-        * `botw_flag_util` does not need a Bootup.pack present in your mod to do its thing. If one is not present, it will copy it from your game dump into your mod files and then edit that copy.
-        * A new copy of gamedata.ssarc and savedataformat.ssarc will always be written to Bootup.pack, even if no changes were made. This is done so that any invalid flags (e.g. duplicate flags) will be deleted from them. Invalid flags will cause BOTW to perform abnormally. This feature was included by request, and should never harm anything, but if you notice that your Bootup.pack's modified date has changed after no changes were made, this is why.
-        * Knowing which flags to give what properties is a very complicated affair. Rather than try to retrieve all that information from the data files, a stopgap has been developed: inside the `data` folder, where `botw_flag_util` is installed, is a file called `overrides.json`. In this file is a comprehensive set of override conditions. If you have come across any flags that you notice are receiving incorrect values, you may place the flag name inside the dictionary for the correspond flag type/property and give it a value. Any flags with that name as part of their name will receive that value for that property, overriding whatever standard logic applies to that flag during the generation process. For example, inside OVERRIDE_IS_ONE_SAVE is the name/value `"IsGet_": true`. This means that all flags with `IsGet_` in the name will have their `IsSave` property set to `true`. You can modify this file whenever you want, and as long as it is valid JSON and the values are valid for the properties they're being inserted into, the values will be properly overridden. `If you use this feature to create a more comprehensive ruleset for flag generation, please consider opening a PR on GitHub so that others may benefit from it as well.`
-        
-        ## Contributing
-        * Issues: https://github.com/GingerAvalanche/botw_flag_util/issues
-        * Source: https://github.com/GingerAvalanche/botw_flag_util
-        
-        This software is in early, but usable, beta. There are several variable types that are not yet handled, and several cases that are not handled for the variable types that are handled. Feel free to contribute in any way.
-        
-        ## License
-        This software is licensed under the terms of the GNU Affero General Public License, version 3+. The source is publicly available on Github.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: bcml>=3.0.0b25
+Requires-Dist: oead>=0.11.2
+
+# Breath of the Wild Flag Utilities
+Game data and save game data flag utilities for LoZ:BotW
+
+## Dependencies
+* A dumped copy of Legend of Zelda: Breath of the Wild (for Wii U or Switch)
+* Python 3.7+ (64-bit, added to system PATH)
+
+The following `pip` packages, which will be automatically installed:
+* bcml
+* oead
+
+## Setup
+1. Download and install Python 3.7+, 64-bit. You must choose the "Add to System PATH" option during installation.
+2. Open a command line and run `pip install botw_flag_util`
+
+### How to Use
+
+#### Generate flags:
+`botw_flag_util generate [path_to_mod_root] [-a] [-r # #] [-b] [-v]`
+* `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
+* `-a` - Generate actor flags.
+* `-r # #` - Generate revival flags. The first number is the ResetType for MainField actors. The second is the ResetType for CDungeon (shrine) actors. If one of them is set to -1, it will skip flag generation for that field type.
+* `-b` - Use big-endian mode. For generating flags for Wii U.
+* `-v` - Use verbose mode. Will give more verbose after-action report.
+
+#### Find flags:
+`botw_flag_util find [path_to_mod_root] [search_name] [-b] [-v]`
+* `path_to_mod_root` - The path to the root folder of your mod, which contains the `content` folder. Required.
+* `search_name` - The name of the flag to search for. Will find all flags whose DataName contains `search_name`. For example, `MainField_Npc_HiddenKorok` will find all Korok NPC flags.
+* `-b` - Use big-endian mode. For deleting flags for Wii U.
+* `-v` - Use verbose mode. Will give more verbose after-action report.
+
+Once the search has been completed, you will be told how many game data and save data flags were found that matched `search_name`. You will then be given three choices:
+* `v` - View more detailed information on the flags found: their full names and their types, and then prompt for another choice.
+* `d` - Delete all the flags that were found by this search, and then return to the command line.
+* `x` - Return to the command line.
+
+##### Quirks
+* `botw_flag_util` does not need a Bootup.pack present in your mod to do its thing. If one is not present, it will copy it from your game dump into your mod files and then edit that copy.
+* A new copy of gamedata.ssarc and savedataformat.ssarc will always be written to Bootup.pack, even if no changes were made. This is done so that any invalid flags (e.g. duplicate flags) will be deleted from them. Invalid flags will cause BOTW to perform abnormally. This feature was included by request, and should never harm anything, but if you notice that your Bootup.pack's modified date has changed after no changes were made, this is why.
+* Knowing which flags to give what properties is a very complicated affair. Rather than try to retrieve all that information from the data files, a stopgap has been developed: inside the `data` folder, where `botw_flag_util` is installed, is a file called `overrides.json`. In this file is a comprehensive set of override conditions. If you have come across any flags that you notice are receiving incorrect values, you may place the flag name inside the dictionary for the correspond flag type/property and give it a value. Any flags with that name as part of their name will receive that value for that property, overriding whatever standard logic applies to that flag during the generation process. For example, inside OVERRIDE_IS_ONE_SAVE is the name/value `"IsGet_": true`. This means that all flags with `IsGet_` in the name will have their `IsSave` property set to `true`. You can modify this file whenever you want, and as long as it is valid JSON and the values are valid for the properties they're being inserted into, the values will be properly overridden. `If you use this feature to create a more comprehensive ruleset for flag generation, please consider opening a PR on GitHub so that others may benefit from it as well.`
+
+## Contributing
+* Issues: https://github.com/GingerAvalanche/botw_flag_util/issues
+* Source: https://github.com/GingerAvalanche/botw_flag_util
+
+This software is in early, but usable, beta. There are several variable types that are not yet handled, and several cases that are not handled for the variable types that are handled. Feel free to contribute in any way.
+
+## License
+This software is licensed under the terms of the GNU Affero General Public License, version 3+. The source is publicly available on Github.
```

### Comparing `botw_flag_util-0.3.5/botw_flag_util.egg-info/SOURCES.txt` & `botw_flag_util-0.3.6/botw_flag_util.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 botw_flag_util/__init__.py
 botw_flag_util/__main__.py
 botw_flag_util/__version__.py
 botw_flag_util/finder.py
```

### Comparing `botw_flag_util-0.3.5/setup.py` & `botw_flag_util-0.3.6/setup.py`

 * *Files identical despite different names*

