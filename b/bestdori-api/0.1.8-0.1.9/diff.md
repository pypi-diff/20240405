# Comparing `tmp/bestdori_api-0.1.8.tar.gz` & `tmp/bestdori_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori_api-0.1.8.tar", last modified: Sun Mar  3 14:14:50 2024, max compression
+gzip compressed data, was "bestdori_api-0.1.9.tar", last modified: Tue Mar  5 15:23:05 2024, max compression
```

## Comparing `bestdori_api-0.1.8.tar` & `bestdori_api-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.299920 bestdori_api-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-03 14:14:50.299920 bestdori_api-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.295920 bestdori_api-0.1.8/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.295920 bestdori_api-0.1.8/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/ayachan/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.295920 bestdori_api-0.1.8/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/missions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.299920 bestdori_api-0.1.8/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/utils/content.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/utils/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:14:50.299920 bestdori_api-0.1.8/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-03 14:14:50.000000 bestdori_api-0.1.8/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-03 14:14:50.000000 bestdori_api-0.1.8/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 14:14:50.000000 bestdori_api-0.1.8/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-03 14:14:50.000000 bestdori_api-0.1.8/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 14:14:50.299920 bestdori_api-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-03 14:14:42.000000 bestdori_api-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/missions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/setup.py
```

### Comparing `bestdori_api-0.1.8/LICENSE` & `bestdori_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/PKG-INFO` & `bestdori_api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori_api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: UNKNOWN
 Description: ![bestdori_api logo](https://github.com/WindowsSov8forUs/bestdori_api/blob/main/logo.png)
         <div align="center">
```

### Comparing `bestdori_api-0.1.8/README.md` & `bestdori_api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/__init__.py` & `bestdori_api-0.1.9/bestdori/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/_settings.py` & `bestdori_api-0.1.9/bestdori/_settings.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/ayachan/__init__.py` & `bestdori_api-0.1.9/bestdori/ayachan/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/ayachan/utils/network.py` & `bestdori_api-0.1.9/bestdori/ayachan/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/cards.py` & `bestdori_api-0.1.9/bestdori/cards.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/characters.py` & `bestdori_api-0.1.9/bestdori/characters.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/charts.py` & `bestdori_api-0.1.9/bestdori/charts.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/comics.py` & `bestdori_api-0.1.9/bestdori/comics.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/costumes.py` & `bestdori_api-0.1.9/bestdori/costumes.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/eventarchives.py` & `bestdori_api-0.1.9/bestdori/eventarchives.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/events.py` & `bestdori_api-0.1.9/bestdori/events.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/exceptions.py` & `bestdori_api-0.1.9/bestdori/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/gacha.py` & `bestdori_api-0.1.9/bestdori/gacha.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/logincampaigns.py` & `bestdori_api-0.1.9/bestdori/logincampaigns.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/miracleticket.py` & `bestdori_api-0.1.9/bestdori/miracleticket.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/missions.py` & `bestdori_api-0.1.9/bestdori/missions.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/post.py` & `bestdori_api-0.1.9/bestdori/post.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/songmeta.py` & `bestdori_api-0.1.9/bestdori/songmeta.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/songs.py` & `bestdori_api-0.1.9/bestdori/songs.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/upload.py` & `bestdori_api-0.1.9/bestdori/upload.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/user.py` & `bestdori_api-0.1.9/bestdori/user.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/utils/__init__.py` & `bestdori_api-0.1.9/bestdori/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/utils/content.py` & `bestdori_api-0.1.9/bestdori/utils/content.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/utils/network.py` & `bestdori_api-0.1.9/bestdori/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/utils/note.py` & `bestdori_api-0.1.9/bestdori/utils/note.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/bestdori/utils/utils.py` & `bestdori_api-0.1.9/bestdori/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     'event': {
         'banner': 'event/{asset_bundle_name}/images_rip/banner.png',
         'logo': 'event/{asset_bundle_name}/images_rip/logo.png',
         'topscreen': 'event/{asset_bundle_name}/topscreen_rip/{type}_eventtop.png',
         'loginbouns': 'event/loginbonus/{asset_bundle_name}_rip/background.png'
     },
     'songs': {
-        'musicjacket': 'musicjacket/musicjacket{index:>03d}_rip/assets-star-forassetbundle-startapp-musicjacket-musicjacket{index:>03d}-{jacket_image}-jacket.png',
+        'musicjacket': 'musicjacket/musicjacket{index:>02d}_rip/assets-star-forassetbundle-startapp-musicjacket-musicjacket{index:>02d}-{jacket_image}-jacket.png',
         'sound': 'sound/bgm{id:>03d}_rip/bgm{id:>03d}.mp3',
         'musicscore': ''
     },
     'thumb': {
         'chara': 'thumb/chara/card{id:>05d}_rip/{resource_set_name}_{type}.png',
         'degree': 'thumb/degree_rip/{degree_name}.png',
         'costume': 'thumb/costume/group{id}_rip/{asset_bundle_name}.png',
```

### Comparing `bestdori_api-0.1.8/bestdori_api.egg-info/PKG-INFO` & `bestdori_api-0.1.9/bestdori_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori_api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: UNKNOWN
 Description: ![bestdori_api logo](https://github.com/WindowsSov8forUs/bestdori_api/blob/main/logo.png)
         <div align="center">
```

### Comparing `bestdori_api-0.1.8/bestdori_api.egg-info/SOURCES.txt` & `bestdori_api-0.1.9/bestdori_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.8/setup.py` & `bestdori_api-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori_api',
-    version='0.1.8',
+    version='0.1.9',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori_api',
     include_package_data=False,
```

