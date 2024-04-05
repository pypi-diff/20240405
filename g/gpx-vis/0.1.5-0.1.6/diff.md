# Comparing `tmp/gpx_vis-0.1.5.tar.gz` & `tmp/gpx_vis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.1.5.tar", last modified: Fri Apr  5 13:51:13 2024, max compression
+gzip compressed data, was "gpx_vis-0.1.6.tar", last modified: Fri Apr  5 15:11:34 2024, max compression
```

## Comparing `gpx_vis-0.1.5.tar` & `gpx_vis-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.872618 gpx_vis-0.1.5/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.5/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:51:13.872385 gpx_vis-0.1.5/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      142 2024-04-05 12:13:11.000000 gpx_vis-0.1.5/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      454 2024-04-05 13:51:08.000000 gpx_vis-0.1.5/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 13:51:13.872686 gpx_vis-0.1.5/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.871075 gpx_vis-0.1.5/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.5/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.872150 gpx_vis-0.1.5/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      203 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    16922 2024-04-05 13:49:16.000000 gpx_vis-0.1.5/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.058030 gpx_vis-0.1.6/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.6/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     1250 2024-04-05 15:11:34.057156 gpx_vis-0.1.6/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      712 2024-04-05 15:10:14.000000 gpx_vis-0.1.6/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      578 2024-04-05 14:42:31.000000 gpx_vis-0.1.6/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 15:11:34.058204 gpx_vis-0.1.6/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.050822 gpx_vis-0.1.6/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.6/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 15:11:34.056182 gpx_vis-0.1.6/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     1250 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       84 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 15:11:32.000000 gpx_vis-0.1.6/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    17187 2024-04-05 15:09:58.000000 gpx_vis-0.1.6/src/gpx_vis.py
```

### Comparing `gpx_vis-0.1.5/LICENSE` & `gpx_vis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.1.5/src/gpx_vis.py` & `gpx_vis-0.1.6/src/gpx_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,28 +193,34 @@
         # list is empty if there is only one track route.
         if len(idx_list) == 0:
             track_list.append([0, len(self.name)])
             return track_list 
         else:
             # record index from previous loop
             previous_idx = 0 
-            for ii, idx in enumerate(idx_list):
-                # start value
-                if ii == 0:
-                    track_list.append([0, idx+1])
-                    previous_idx = idx + 1
-                # end value
-                elif ii == (len(idx_list) - 1):
-                    # account for both cases in the last loop
-                    track_list.append([previous_idx + 1, idx + 1])
-                    track_list.append([idx + 1, len(self.name)])
-                # in-between values
-                else:
-                    track_list.append([previous_idx + 1, idx + 1])
-                    previous_idx = idx + 1
+            # corner case
+            if len(idx_list) == 1:
+                idx = idx_list[0]
+                track_list.append([0, idx+1])
+                track_list.append([idx+1, len(self.name)])
+            else:
+                for ii, idx in enumerate(idx_list):
+                    # start value
+                    if ii == 0:
+                        track_list.append([0, idx+1])
+                        previous_idx = idx + 1
+                    # end value
+                    elif ii == (len(idx_list) - 1):
+                        # account for both cases in the last loop
+                        track_list.append([previous_idx + 1, idx + 1])
+                        track_list.append([idx + 1, len(self.name)])
+                    # in-between values
+                    else:
+                        track_list.append([previous_idx + 1, idx + 1])
+                        previous_idx = idx + 1
             return track_list
 
     # =============================================================================
     # Plotting on graphs    
     # =============================================================================
 
     def plt_tracks(self):
@@ -294,15 +300,14 @@
         map_sw = self.data[['latitude', 'longitude']].min().values.tolist()
         map_ne = self.data[['latitude', 'longitude']].max().values.tolist()
         # create Map.
         main_map = folium.Map(location = map_center)
         # specify border.
         main_map.fit_bounds([map_sw, map_ne])
         
-        
         # create group
         lineGroup = folium.FeatureGroup("Lines")
         
         # plot waypoints for each end and beginning of a track
         idx_split_list = self.idx_trksplit(self)
         # if list is empty, there is no splitting tracks
         for selected_idx in idx_split_list:
```

