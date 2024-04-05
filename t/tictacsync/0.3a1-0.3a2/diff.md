# Comparing `tmp/tictacsync-0.3a1.tar.gz` & `tmp/tictacsync-0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacsync-0.3a1.tar", last modified: Thu Apr  4 15:36:35 2024, max compression
+gzip compressed data, was "tictacsync-0.3a2.tar", last modified: Thu Apr  4 16:36:38 2024, max compression
```

## Comparing `tictacsync-0.3a1.tar` & `tictacsync-0.3a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.126706 tictacsync-0.3a1/
--rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a1/LICENSE
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 15:36:35.126213 tictacsync-0.3a1/PKG-INFO
--rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a1/README.md
--rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-04 15:36:35.126843 tictacsync-0.3a1/setup.cfg
--rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-04 15:36:22.000000 tictacsync-0.3a1/setup.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.121611 tictacsync-0.3a1/tictacsync/
--rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a1/tictacsync/__init__.py
--rw-r--r--   0 lutzray    (501) staff       (20)    27558 2024-04-02 15:17:03.000000 tictacsync-0.3a1/tictacsync/device_scanner.py
--rw-r--r--   0 lutzray    (501) staff       (20)    11391 2024-04-04 14:48:23.000000 tictacsync-0.3a1/tictacsync/entry.py
--rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a1/tictacsync/multi2polywav.py
--rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a1/tictacsync/remergemix.py
--rw-r--r--   0 lutzray    (501) staff       (20)    45946 2024-04-04 14:45:33.000000 tictacsync-0.3a1/tictacsync/timeline.py
--rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a1/tictacsync/yaltc.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 15:36:35.125494 tictacsync-0.3a1/tictacsync.egg-info/
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/PKG-INFO
--rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/SOURCES.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/dependency_links.txt
--rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/entry_points.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a1/tictacsync.egg-info/not-zip-safe
--rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/requires.txt
--rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-04 15:36:35.000000 tictacsync-0.3a1/tictacsync.egg-info/top_level.txt
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 16:36:38.959350 tictacsync-0.3a2/
+-rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a2/LICENSE
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 16:36:38.958864 tictacsync-0.3a2/PKG-INFO
+-rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a2/README.md
+-rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-04 16:36:38.959510 tictacsync-0.3a2/setup.cfg
+-rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-04 16:33:19.000000 tictacsync-0.3a2/setup.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 16:36:38.954252 tictacsync-0.3a2/tictacsync/
+-rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a2/tictacsync/__init__.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    27558 2024-04-02 15:17:03.000000 tictacsync-0.3a2/tictacsync/device_scanner.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    11391 2024-04-04 16:34:29.000000 tictacsync-0.3a2/tictacsync/entry.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a2/tictacsync/multi2polywav.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a2/tictacsync/remergemix.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    45977 2024-04-04 16:31:31.000000 tictacsync-0.3a2/tictacsync/timeline.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a2/tictacsync/yaltc.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-04 16:36:38.958145 tictacsync-0.3a2/tictacsync.egg-info/
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/PKG-INFO
+-rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/entry_points.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a2/tictacsync.egg-info/not-zip-safe
+-rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/requires.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-04 16:36:38.000000 tictacsync-0.3a2/tictacsync.egg-info/top_level.txt
```

### Comparing `tictacsync-0.3a1/LICENSE` & `tictacsync-0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/PKG-INFO` & `tictacsync-0.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a1
+Version: 0.3a2
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tictacsync-0.3a1/README.md` & `tictacsync-0.3a2/README.md`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/setup.py` & `tictacsync-0.3a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     entry_points = {
         "console_scripts": [
         'tictacsync = tictacsync.entry:main',
         'remergemix = tictacsync.remergemix:main',
         'multi2polywav = tictacsync.multi2polywav:main',
         ]
         },
-    version = '0.3a1',
+    version = '0.3a2',
     description = "command for syncing audio video recordings",
     long_description_content_type='text/markdown',
     long_description = long_descr,
     include_package_data=True,
     zip_safe=False,
     author = "Raymond Lutz",
     author_email = "lutzrayblog@mac.com",
```

### Comparing `tictacsync-0.3a1/tictacsync/device_scanner.py` & `tictacsync-0.3a2/tictacsync/device_scanner.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/tictacsync/entry.py` & `tictacsync-0.3a2/tictacsync/entry.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/tictacsync/multi2polywav.py` & `tictacsync-0.3a2/tictacsync/multi2polywav.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/tictacsync/remergemix.py` & `tictacsync-0.3a2/tictacsync/remergemix.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/tictacsync/timeline.py` & `tictacsync-0.3a2/tictacsync/timeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,16 +603,16 @@
                     shift += 1
                 for unused_tr in device.tracks.unused:
                     if mix_tracks[0] > unused_tr:
                         shift += 1
                 mix_tracks = [t-shift for t in mix_tracks]
                 logger.debug('new mix_tracks: %s'%mix_tracks)
                 return _sox_keep(multichan_tmpfl, mix_tracks)
-            else: # no tracks declaration, mix programmatically
-                return _sox_mix(_split_channels(multichan_tmpfl))
+        else: # no tracks declaration, mix programmatically
+            return _sox_mix(_split_channels(multichan_tmpfl))
 
     def build_audio_and_write_video(self, top_dir, output_dir,
                                     write_multicam_structure,
                                     asked_ISOs):
         """
         top_dir: Path, directory where media were looked for
 
@@ -683,15 +683,16 @@
         #
         multiple_recorders = len(merged_audio_files_by_device) > 1
         logger.debug('multiple_recorder: %s'%multiple_recorders)
         # dev_mixes_mix contains all audio recorders if many
         mixes = [self._get_mix(device, multi_chan_audio)
                 for device, multi_chan_audio
                 in merged_audio_files_by_device]
-        logger.debug('thera are %i dev mixes'%len(mixes))
+        logger.debug('there are %i dev mixes'%len(mixes))
+        logger.debug('mixes %s'%mixes)
         dev_mixes_mix = _sox_mix(mixes)
         # dev_mixes_mix = _sox_combine([audio for _, audio
         #         in merged_audio_files_by_device]) # all devices
         logger.debug('will merge with %s'%(_pathname(dev_mixes_mix)))
         self.ref_recording.synced_audio = dev_mixes_mix
         logger.debug('dev_mixes_mix n chan: %i'%
             sox.file_info.channels(_pathname(dev_mixes_mix)))
```

### Comparing `tictacsync-0.3a1/tictacsync/yaltc.py` & `tictacsync-0.3a2/tictacsync/yaltc.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a1/tictacsync.egg-info/PKG-INFO` & `tictacsync-0.3a2/tictacsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a1
+Version: 0.3a2
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

