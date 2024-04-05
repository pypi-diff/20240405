# Comparing `tmp/labgym-2.3.5.tar.gz` & `tmp/labgym-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgym-2.3.5.tar", last modified: Thu Mar  7 00:49:27 2024, max compression
+gzip compressed data, was "labgym-2.4.0.tar", last modified: Mon Mar 25 19:09:57 2024, max compression
```

## Comparing `labgym-2.3.5.tar` & `labgym-2.4.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    31919 2024-03-07 00:49:22.487931 labgym-2.3.5/LICENSE.txt
--rw-r--r--   0        0        0      417 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/NOTICE.txt
--rw-r--r--   0        0        0      882 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/__init__.py
--rw-r--r--   0        0        0     1321 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/__main__.py
--rw-r--r--   0        0        0    96963 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/analyzebehaviors.py
--rw-r--r--   0        0        0   208490 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/analyzebehaviorsdetector.py
--rw-r--r--   0        0        0    70637 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/categorizers.py
--rw-r--r--   0        0        0      860 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/detectors/__init__.py
--rw-r--r--   0        0        0      890 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/__init__.py
--rw-r--r--   0        0        0      905 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/analysis/__init__.py
--rw-r--r--   0        0        0     1810 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/analysis/analysis_module.py
--rw-r--r--   0        0        0    72012 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/analysis/analyze_behaviors.py
--rw-r--r--   0        0        0     9857 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/analysis/mine_results.py
--rw-r--r--   0        0        0     4879 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/main_window.py
--rw-r--r--   0        0        0    22010 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/preprocessing.py
--rw-r--r--   0        0        0      905 2024-03-07 00:49:22.487931 labgym-2.3.5/LabGym/gui/training/__init__.py
--rw-r--r--   0        0        0    52807 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/gui/training/behavior_examples.py
--rw-r--r--   0        0        0    34221 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/gui/training/categorizers.py
--rw-r--r--   0        0        0    22496 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/gui/training/detectors.py
--rw-r--r--   0        0        0     5218 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/gui/training/training_module.py
--rw-r--r--   0        0        0     4480 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/gui/utils.py
--rw-r--r--   0        0        0     8518 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/minedata.py
--rw-r--r--   0        0        0      860 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/models/__init__.py
--rw-r--r--   0        0        0    45710 2024-03-07 00:49:22.491931 labgym-2.3.5/LabGym/tools.py
--rw-r--r--   0        0        0      131 2024-03-07 00:49:22.491931 labgym-2.3.5/NOTICE.txt
--rw-r--r--   0        0        0    13320 2024-03-07 00:49:22.491931 labgym-2.3.5/README.md
--rw-r--r--   0        0        0     2208 2024-03-07 00:49:27.075904 labgym-2.3.5/pyproject.toml
--rw-r--r--   0        0        0      859 2024-03-07 00:49:22.495931 labgym-2.3.5/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-07 00:49:22.495931 labgym-2.3.5/tests/test_main.py
--rw-r--r--   0        0        0     1093 2024-03-07 00:49:22.495931 labgym-2.3.5/tests/test_tools.py
--rw-r--r--   0        0        0    14931 1970-01-01 00:00:00.000000 labgym-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0    31919 2024-03-25 19:09:50.314254 labgym-2.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      417 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/NOTICE.txt
+-rw-r--r--   0        0        0      882 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/__init__.py
+-rw-r--r--   0        0        0     1210 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/__main__.py
+-rw-r--r--   0        0        0    87666 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/analyzebehaviors.py
+-rw-r--r--   0        0        0   173802 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/analyzebehaviorsdetector.py
+-rw-r--r--   0        0        0    67359 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/categorizers.py
+-rw-r--r--   0        0        0    12995 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/detector.py
+-rw-r--r--   0        0        0      859 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/detectors/__init__.py
+-rw-r--r--   0        0        0      889 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/__init__.py
+-rw-r--r--   0        0        0      904 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/__init__.py
+-rw-r--r--   0        0        0     1808 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/analysis_module.py
+-rw-r--r--   0        0        0    67750 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/analyze_behaviors.py
+-rw-r--r--   0        0        0     9322 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/mine_results.py
+-rw-r--r--   0        0        0     4833 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/main_window.py
+-rw-r--r--   0        0        0    21798 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/preprocessing.py
+-rw-r--r--   0        0        0      904 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/__init__.py
+-rw-r--r--   0        0        0    51881 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/behavior_examples.py
+-rw-r--r--   0        0        0    33339 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/categorizers.py
+-rw-r--r--   0        0        0    22307 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/detectors.py
+-rw-r--r--   0        0        0     5203 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/training_module.py
+-rw-r--r--   0        0        0     4473 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/utils.py
+-rw-r--r--   0        0        0     8091 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/minedata.py
+-rw-r--r--   0        0        0      859 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/models/__init__.py
+-rw-r--r--   0        0        0    44182 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/tools.py
+-rw-r--r--   0        0        0      131 2024-03-25 19:09:50.318254 labgym-2.4.0/NOTICE.txt
+-rw-r--r--   0        0        0    13320 2024-03-25 19:09:50.318254 labgym-2.4.0/README.md
+-rw-r--r--   0        0        0     2239 2024-03-25 19:09:57.506314 labgym-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      859 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     1093 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/test_tools.py
+-rw-r--r--   0        0        0    14931 1970-01-01 00:00:00.000000 labgym-2.4.0/PKG-INFO
```

### Comparing `labgym-2.3.5/LICENSE.txt` & `labgym-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labgym-2.3.5/LabGym/__init__.py` & `labgym-2.4.0/LabGym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-__version__ = "2.3.5"
+__version__ = "2.4.0"
```

### Comparing `labgym-2.3.5/LabGym/__main__.py` & `labgym-2.4.0/LabGym/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,36 +9,29 @@
 
 
 def main() -> None:
     """Check version and run LabGym."""
 
     try:
         current_version = version.parse(__version__)
-        pypi_json = json.loads(
-            request.urlopen("https://pypi.python.org/pypi/LabGym/json").read()
-        )
+        pypi_json = json.loads(request.urlopen("https://pypi.python.org/pypi/LabGym/json").read())
         latest_version = version.parse(pypi_json["info"]["version"])
 
         if latest_version > current_version:
             if "pipx" in str(Path(__file__)):
                 upgrade_command = "pipx upgrade LabGym"
             else:
                 upgrade_command = "python3 -m pip install --upgrade LabGym"
 
-            print(
-                f"You are using LabGym {current_version}, but version {latest_version} is available."
-            )
-            print(
-                f"Consider upgrading LabGym by using the command '{upgrade_command}'."
-            )
-            print(
-                "For the details of new changes, check https://github.com/umyelab/LabGym.\n"
-            )
+            print(f"You are using LabGym {current_version}, but version {latest_version} is available.")
+            print(f"Consider upgrading LabGym by using the command '{upgrade_command}'.")
+            print("For the details of new changes, check https://github.com/umyelab/LabGym.\n")
     except URLError:
         print("Unable to check for new versions of LabGym!")
         print("Please check https://github.com/umyelab/LabGym for updates.\n")
 
+
     gui.gui()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `labgym-2.3.5/LabGym/analyzebehaviors.py` & `labgym-2.4.0/LabGym/analyzebehaviors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import datetime
 import functools
 import gc
 import math
 import operator
 import os
 from collections import deque
@@ -29,15 +28,15 @@
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 from scipy.spatial import distance
 from tensorflow.keras.models import load_model
 from tensorflow.keras.preprocessing.image import img_to_array
 
-from .tools import *
+from LabGym.tools import *
 
 
 class AnalyzeAnimal:
     def __init__(self):
         self.path_to_video = None
         self.basename = None
         self.fps = None
@@ -107,17 +106,15 @@
     ):
         print("Preparation started...")
         print(datetime.datetime.now())
 
         self.path_to_video = path_to_video
         self.basename = os.path.basename(self.path_to_video)
         self.framewidth = framewidth
-        self.results_path = os.path.join(
-            results_path, os.path.splitext(self.basename)[0]
-        )
+        self.results_path = os.path.join(results_path, os.path.splitext(self.basename)[0])
         self.animal_number = animal_number
         self.dim_tconv = dim_tconv
         self.dim_conv = dim_conv
         self.channel = channel
         self.include_bodyparts = include_bodyparts
         self.std = std
         self.categorize_behavior = categorize_behavior
@@ -128,44 +125,30 @@
         self.length = length
         os.makedirs(self.results_path, exist_ok=True)
         capture = cv2.VideoCapture(self.path_to_video)
         self.fps = round(capture.get(cv2.CAP_PROP_FPS))
         self.count_to_deregister = self.fps * 2
 
         if self.duration <= 0:
-            self.total_analysis_framecount = (
-                int(capture.get(cv2.CAP_PROP_FRAME_COUNT)) + 1
-            )
+            self.total_analysis_framecount = int(capture.get(cv2.CAP_PROP_FRAME_COUNT)) + 1
         else:
             self.total_analysis_framecount = int(self.fps * self.duration) + 1
 
         while True:
             retval, frame = capture.read()
             break
         capture.release()
 
         print("Video fps: " + str(self.fps))
-        print(
-            "The original video framesize: "
-            + str(int(frame.shape[0]))
-            + " X "
-            + str(int(frame.shape[1]))
-        )
+        print("The original video framesize: " + str(int(frame.shape[0])) + " X " + str(int(frame.shape[1])))
 
         if self.framewidth is not None:
             self.frameheight = int(frame.shape[0] * self.framewidth / frame.shape[1])
-            self.background = cv2.resize(
-                frame, (self.framewidth, self.frameheight), interpolation=cv2.INTER_AREA
-            )
-            print(
-                "The resized video framesize: "
-                + str(self.frameheight)
-                + " X "
-                + str(self.framewidth)
-            )
+            self.background = cv2.resize(frame, (self.framewidth, self.frameheight), interpolation=cv2.INTER_AREA)
+            print("The resized video framesize: " + str(self.frameheight) + " X " + str(self.framewidth))
         else:
             self.background = frame
 
         smallest_dimension = min(self.background.shape[0], self.background.shape[1])
         if smallest_dimension / self.animal_number < 250:
             self.kernel = 3
         elif smallest_dimension / self.animal_number < 500:
@@ -204,20 +187,16 @@
         else:
             backgrounds = load_backgrounds_from_folder(path_background, frame_size)
 
         self.background = backgrounds[0]
         self.background_low = backgrounds[1]
         self.background_high = backgrounds[2]
         cv2.imwrite(os.path.join(self.results_path, "background.jpg"), self.background)
-        cv2.imwrite(
-            os.path.join(self.results_path, "background_low.jpg"), self.background_low
-        )
-        cv2.imwrite(
-            os.path.join(self.results_path, "background_high.jpg"), self.background_high
-        )
+        cv2.imwrite(os.path.join(self.results_path, "background_low.jpg"), self.background_low)
+        cv2.imwrite(os.path.join(self.results_path, "background_high.jpg"), self.background_high)
 
         if self.autofind_t:
             self.t = get_stimulation_time(self.path_to_video, self.delta)
 
         self.animal_area = estimate_animal_area(
             self.path_to_video,
             self.delta,
@@ -232,17 +211,15 @@
             self.animal_vs_bg,
             self.kernel,
         )
 
         if self.categorize_behavior is True:
             for behavior_name in names_and_colors:
                 self.all_behavior_parameters[behavior_name] = {}
-                self.all_behavior_parameters[behavior_name]["color"] = names_and_colors[
-                    behavior_name
-                ]
+                self.all_behavior_parameters[behavior_name]["color"] = names_and_colors[behavior_name]
                 for parameter_name in [
                     "acceleration",
                     "count",
                     "distance",
                     "duration",
                     "intensity_area",
                     "intensity_length",
@@ -303,17 +280,15 @@
                 ] * self.total_analysis_framecount
             self.pattern_images[i] = [
                 np.zeros((self.dim_conv, self.dim_conv, 3), dtype="uint8")
             ] * self.total_analysis_framecount
 
         print("Preparation completed!")
 
-    def track_animal(
-        self, frame_count_analyze, contours, centers, heights, inners=None, blobs=None
-    ):
+    def track_animal(self, frame_count_analyze, contours, centers, heights, inners=None, blobs=None):
         unused_existing_indices = list(self.animal_existingcenters)
         existing_centers = list(self.animal_existingcenters.values())
         unused_new_indices = list(range(len(centers)))
         dt_flattened = distance.cdist(existing_centers, centers).flatten()
         dt_sort_index = dt_flattened.argsort()
         length = len(centers)
 
@@ -323,69 +298,57 @@
             if index_in_existing in unused_existing_indices:
                 if index_in_new in unused_new_indices:
                     unused_existing_indices.remove(index_in_existing)
                     unused_new_indices.remove(index_in_new)
                     if self.register_counts[index_in_existing] is None:
                         self.register_counts[index_in_existing] = frame_count_analyze
                     self.to_deregister[index_in_existing] = 0
-                    self.animal_contours[index_in_existing][
-                        frame_count_analyze
-                    ] = contours[index_in_new]
+                    self.animal_contours[index_in_existing][frame_count_analyze] = contours[index_in_new]
                     center = centers[index_in_new]
                     self.animal_centers[index_in_existing][frame_count_analyze] = center
                     self.animal_existingcenters[index_in_existing] = center
-                    self.animal_heights[index_in_existing][
-                        frame_count_analyze
-                    ] = heights[index_in_new]
+                    self.animal_heights[index_in_existing][frame_count_analyze] = heights[index_in_new]
                     if self.animation_analyzer is True:
                         blob = blobs[index_in_new]
                         blob = img_to_array(
                             cv2.resize(
                                 blob,
                                 (self.dim_tconv, self.dim_tconv),
                                 interpolation=cv2.INTER_AREA,
                             )
                         )
                         self.animal_blobs[index_in_existing].append(blob)
-                        self.animations[index_in_existing][
-                            frame_count_analyze
-                        ] = np.array(self.animal_blobs[index_in_existing])
-                    if self.include_bodyparts is True:
-                        self.animal_inners[index_in_existing].append(
-                            inners[index_in_new]
+                        self.animations[index_in_existing][frame_count_analyze] = np.array(
+                            self.animal_blobs[index_in_existing]
                         )
+                    if self.include_bodyparts is True:
+                        self.animal_inners[index_in_existing].append(inners[index_in_new])
                         pattern_image = generate_patternimage(
                             self.background,
                             self.animal_contours[index_in_existing][
-                                max(
-                                    0, (frame_count_analyze - self.length + 1)
-                                ) : frame_count_analyze + 1
+                                max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                             ],
                             inners=self.animal_inners[index_in_existing],
                             std=self.std,
                         )
                     else:
                         pattern_image = generate_patternimage(
                             self.background,
                             self.animal_contours[index_in_existing][
-                                max(
-                                    0, (frame_count_analyze - self.length + 1)
-                                ) : frame_count_analyze + 1
+                                max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                             ],
                             inners=None,
                             std=0,
                         )
                     pattern_image = cv2.resize(
                         pattern_image,
                         (self.dim_conv, self.dim_conv),
                         interpolation=cv2.INTER_AREA,
                     )
-                    self.pattern_images[index_in_existing][
-                        frame_count_analyze
-                    ] = np.array(pattern_image)
+                    self.pattern_images[index_in_existing][frame_count_analyze] = np.array(pattern_image)
 
         if len(unused_existing_indices) > 0:
             for i in unused_existing_indices:
                 if self.to_deregister[i] <= self.count_to_deregister:
                     self.to_deregister[i] += 1
                 else:
                     self.animal_existingcenters[i] = (-10000, -10000)
@@ -523,34 +486,28 @@
                                         )
                                     else:
                                         blob = extract_blob_background(
                                             f,
                                             self.animal_contours[i][
                                                 max(
                                                     0,
-                                                    (
-                                                        frame_count_analyze
-                                                        - self.length
-                                                        + 1
-                                                    ),
+                                                    (frame_count_analyze - self.length + 1),
                                                 ) : frame_count_analyze + 1
                                             ],
                                             contour=None,
                                             channel=self.channel,
                                             background_free=False,
                                         )
                                         blob = cv2.resize(
                                             blob,
                                             (self.dim_tconv, self.dim_tconv),
                                             interpolation=cv2.INTER_AREA,
                                         )
                                     animation.append(img_to_array(blob))
-                                self.animations[i][frame_count_analyze] = np.array(
-                                    animation
-                                )
+                                self.animations[i][frame_count_analyze] = np.array(animation)
 
                 frame_count_analyze += 1
 
             frame_count += 1
 
         capture.release()
 
@@ -584,19 +541,15 @@
         capture = cv2.VideoCapture(self.path_to_video)
         frame_count = frame_count_analyze = 0
         temp_frames = deque(maxlen=self.length)
         temp_contours = deque(maxlen=self.length)
         temp_inners = deque(maxlen=self.length)
         animation = (
             deque(
-                [
-                    np.zeros(
-                        (self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8"
-                    )
-                ],
+                [np.zeros((self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8")],
                 maxlen=self.length,
             )
             * self.length
         )
 
         start_t = round((self.t - self.length / self.fps), 2)
         if start_t < 0:
@@ -660,17 +613,15 @@
                     temp_contours.append(contours)
                     temp_inners.append(inners)
                     length = len(temp_frames)
                     if length == 1:
                         self.register_counts[0] = frame_count_analyze
                     self.animal_contours[0][frame_count_analyze] = contours
 
-                    (y_bt, y_tp, x_lf, x_rt) = crop_frame(
-                        frame, functools.reduce(operator.iconcat, temp_contours, [])
-                    )
+                    (y_bt, y_tp, x_lf, x_rt) = crop_frame(frame, functools.reduce(operator.iconcat, temp_contours, []))
                     self.animal_centers[0][frame_count_analyze] = (x_lf + 5, y_bt + 10)
 
                     pattern_image = generate_patternimage_all(
                         frame,
                         y_bt,
                         y_tp,
                         x_lf,
@@ -687,17 +638,15 @@
                         )
                     )
 
                     if self.animation_analyzer is True:
                         for i, f in enumerate(temp_frames):
                             if (
                                 self.animal_contours[0][
-                                    max(
-                                        0, (frame_count_analyze - self.length + 1)
-                                    ) : frame_count_analyze + 1
+                                    max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                                 ][n]
                                 is None
                             ):
                                 blob = np.zeros(
                                     (self.dim_tconv, self.dim_tconv, self.channel),
                                     dtype="uint8",
                                 )
@@ -714,17 +663,15 @@
                                 )
                             blob = cv2.resize(
                                 blob,
                                 (self.dim_tconv, self.dim_tconv),
                                 interpolation=cv2.INTER_AREA,
                             )
                             animation.append(img_to_array(blob))
-                            self.animations[0][frame_count_analyze] = np.array(
-                                animation
-                            )
+                            self.animations[0][frame_count_analyze] = np.array(animation)
 
                 frame_count_analyze += 1
 
             frame_count += 1
 
         capture.release()
 
@@ -799,34 +746,28 @@
 
         del self.animations
         del self.pattern_images
         gc.collect()
 
         with tf.device("CPU"):
             if self.animation_analyzer is True:
-                animations = tf.convert_to_tensor(
-                    np.array(animations, dtype="float32") / 255.0
-                )
-            pattern_images = tf.convert_to_tensor(
-                np.array(pattern_images, dtype="float32") / 255.0
-            )
+                animations = tf.convert_to_tensor(np.array(animations, dtype="float32") / 255.0)
+            pattern_images = tf.convert_to_tensor(np.array(pattern_images, dtype="float32") / 255.0)
 
         if self.animation_analyzer is True:
             inputs = [animations, pattern_images]
         else:
             inputs = pattern_images
 
         categorizer = load_model(path_to_categorizer)
         predictions = categorizer.predict(inputs, batch_size=32)
 
         for behavior_name in self.all_behavior_parameters:
             for i in IDs:
-                self.all_behavior_parameters[behavior_name]["probability"][i] = [
-                    np.nan
-                ] * len(self.all_time)
+                self.all_behavior_parameters[behavior_name]["probability"][i] = [np.nan] * len(self.all_time)
                 self.event_probability[i] = [["NA", -1]] * len(self.all_time)
 
         idx = 0
         for n in IDs:
             i = self.length + self.register_counts[n]
             idx += i
             while i < len(self.animal_contours[n]):
@@ -841,38 +782,31 @@
                         for behavior_name in behavior_names:
                             if len(behavior_names) == 2:
                                 if behavior_names.index(behavior_name) == 0:
                                     probability = 1 - prediction[0]
                                 else:
                                     probability = prediction[0]
                             else:
-                                probability = prediction[
-                                    behavior_names.index(behavior_name)
-                                ]
-                            self.all_behavior_parameters[behavior_name]["probability"][
-                                n
-                            ][i] = probability
+                                probability = prediction[behavior_names.index(behavior_name)]
+                            self.all_behavior_parameters[behavior_name]["probability"][n][i] = probability
                         if len(behavior_names) == 2:
                             if prediction[0] > 0.5:
                                 if prediction[0] - (1 - prediction[0]) > uncertain:
                                     self.event_probability[n][i] = [
                                         behavior_names[1],
                                         prediction[0],
                                     ]
                             if prediction[0] < 0.5:
                                 if (1 - prediction[0]) - prediction[0] > uncertain:
                                     self.event_probability[n][i] = [
                                         behavior_names[0],
                                         1 - prediction[0],
                                     ]
                         else:
-                            if (
-                                sorted(prediction)[-1] - sorted(prediction)[-2]
-                                > uncertain
-                            ):
+                            if sorted(prediction)[-1] - sorted(prediction)[-2] > uncertain:
                                 self.event_probability[n][i] = [
                                     behavior_names[np.argmax(prediction)],
                                     max(prediction),
                                 ]
 
                 idx += 1
                 i += 1
@@ -882,30 +816,24 @@
 
         print("Behavioral categorization completed!")
 
     def annotate_video(self, behavior_to_include, show_legend=True, interact_all=False):
         print("Annotating video...")
         print(datetime.datetime.now())
 
-        text_scl = max(
-            min(self.background.shape[0], self.background.shape[1]) / 960, 0.5
-        )
-        text_tk = max(
-            1, int(min(self.background.shape[0], self.background.shape[1]) / 960)
-        )
+        text_scl = 1
+        text_tk = 2
 
         if self.categorize_behavior is True:
             colors = {}
             for behavior_name in self.all_behavior_parameters:
                 if self.all_behavior_parameters[behavior_name]["color"][1][0] != "#":
                     colors[behavior_name] = (255, 255, 255)
                 else:
-                    hex_color = self.all_behavior_parameters[behavior_name]["color"][
-                        1
-                    ].lstrip("#")
+                    hex_color = self.all_behavior_parameters[behavior_name]["color"][1].lstrip("#")
                     color = tuple(int(hex_color[i : i + 2], 16) for i in (0, 2, 4))
                     colors[behavior_name] = color[::-1]
 
             if len(behavior_to_include) != len(self.all_behavior_parameters):
                 for behavior_name in self.all_behavior_parameters:
                     if behavior_name not in behavior_to_include:
                         del colors[behavior_name]
@@ -981,90 +909,59 @@
                                         (cx, cy),
                                         int(text_tk * 3),
                                         (255, 0, 0),
                                         -1,
                                     )
 
                                 if self.categorize_behavior is True:
-                                    if (
-                                        self.event_probability[i][frame_count_analyze][
-                                            0
-                                        ]
-                                        == "NA"
-                                    ):
+                                    if self.event_probability[i][frame_count_analyze][0] == "NA":
                                         if interact_all is True:
                                             cv2.drawContours(
                                                 frame,
-                                                self.animal_contours[i][
-                                                    frame_count_analyze
-                                                ],
+                                                self.animal_contours[i][frame_count_analyze],
                                                 -1,
                                                 (255, 255, 255),
                                                 1,
                                             )
                                         else:
                                             cv2.drawContours(
                                                 frame,
-                                                [
-                                                    self.animal_contours[i][
-                                                        frame_count_analyze
-                                                    ]
-                                                ],
+                                                [self.animal_contours[i][frame_count_analyze]],
                                                 0,
                                                 (255, 255, 255),
                                                 1,
                                             )
                                         cv2.putText(
                                             frame,
                                             "NA",
                                             (cx + 10, cy - 10),
                                             cv2.FONT_HERSHEY_SIMPLEX,
                                             text_scl,
                                             (255, 255, 255),
                                             text_tk,
                                         )
                                     else:
-                                        name = self.event_probability[i][
-                                            frame_count_analyze
-                                        ][0]
+                                        name = self.event_probability[i][frame_count_analyze][0]
                                         probability = (
-                                            str(
-                                                round(
-                                                    self.event_probability[i][
-                                                        frame_count_analyze
-                                                    ][1]
-                                                    * 100
-                                                )
-                                            )
-                                            + "%"
+                                            str(round(self.event_probability[i][frame_count_analyze][1] * 100)) + "%"
                                         )
                                         if name in colors:
-                                            color = colors[
-                                                self.event_probability[i][
-                                                    frame_count_analyze
-                                                ][0]
-                                            ]
+                                            color = colors[self.event_probability[i][frame_count_analyze][0]]
                                             if interact_all is True:
                                                 cv2.drawContours(
                                                     frame,
-                                                    self.animal_contours[i][
-                                                        frame_count_analyze
-                                                    ],
+                                                    self.animal_contours[i][frame_count_analyze],
                                                     -1,
                                                     color,
                                                     1,
                                                 )
                                             else:
                                                 cv2.drawContours(
                                                     frame,
-                                                    [
-                                                        self.animal_contours[i][
-                                                            frame_count_analyze
-                                                        ]
-                                                    ],
+                                                    [self.animal_contours[i][frame_count_analyze]],
                                                     0,
                                                     color,
                                                     1,
                                                 )
                                             cv2.putText(
                                                 frame,
                                                 name + " " + probability,
@@ -1074,29 +971,23 @@
                                                 color,
                                                 text_tk,
                                             )
                                         else:
                                             if interact_all is True:
                                                 cv2.drawContours(
                                                     frame,
-                                                    self.animal_contours[i][
-                                                        frame_count_analyze
-                                                    ],
+                                                    self.animal_contours[i][frame_count_analyze],
                                                     -1,
                                                     (255, 255, 255),
                                                     1,
                                                 )
                                             else:
                                                 cv2.drawContours(
                                                     frame,
-                                                    [
-                                                        self.animal_contours[i][
-                                                            frame_count_analyze
-                                                        ]
-                                                    ],
+                                                    [self.animal_contours[i][frame_count_analyze]],
                                                     0,
                                                     (255, 255, 255),
                                                     1,
                                                 )
                                             cv2.putText(
                                                 frame,
                                                 "NA",
@@ -1157,89 +1048,64 @@
                     if "4 locomotion parameters" in parameter_to_analyze:
                         self.all_behavior_parameters[behavior_name]["distance"][i] = 0.0
                     if "latency" in parameter_to_analyze:
                         self.all_behavior_parameters[behavior_name]["latency"][i] = "NA"
 
                 for parameter_name in all_parameters:
                     for i in self.event_probability:
-                        self.all_behavior_parameters[behavior_name][parameter_name][
-                            i
-                        ] = [np.nan] * len(self.all_time)
+                        self.all_behavior_parameters[behavior_name][parameter_name][i] = [np.nan] * len(self.all_time)
 
         else:
             for i in self.animal_contours:
                 if "4 locomotion parameters" in parameter_to_analyze:
                     self.all_behavior_parameters["distance"][i] = 0.0
                 for parameter_name in all_parameters:
-                    self.all_behavior_parameters[parameter_name][i] = [np.nan] * len(
-                        self.all_time
-                    )
+                    self.all_behavior_parameters[parameter_name][i] = [np.nan] * len(self.all_time)
 
         if len(parameter_to_analyze) > 0:
             for i in self.animal_contours:
                 n = self.length + self.register_counts[i]
 
                 while n < len(self.animal_contours[i]):
                     if self.categorize_behavior is True:
                         behavior_name = self.event_probability[i][n][0]
 
                         if behavior_name != "NA":
                             if "count" in parameter_to_analyze:
                                 if behavior_name != self.event_probability[i][n - 1][0]:
-                                    self.all_behavior_parameters[behavior_name][
-                                        "count"
-                                    ][i] += 1
+                                    self.all_behavior_parameters[behavior_name]["count"][i] += 1
 
                             if "duration" in parameter_to_analyze:
-                                self.all_behavior_parameters[behavior_name]["duration"][
-                                    i
-                                ] += round(1 / self.fps, 2)
+                                self.all_behavior_parameters[behavior_name]["duration"][i] += round(1 / self.fps, 2)
 
                             if "latency" in parameter_to_analyze:
-                                if (
-                                    self.all_behavior_parameters[behavior_name][
-                                        "latency"
-                                    ][i]
-                                    == "NA"
-                                ):
-                                    self.all_behavior_parameters[behavior_name][
-                                        "latency"
-                                    ][i] = self.all_time[n]
+                                if self.all_behavior_parameters[behavior_name]["latency"][i] == "NA":
+                                    self.all_behavior_parameters[behavior_name]["latency"][i] = self.all_time[n]
 
                             if "3 length parameters" in parameter_to_analyze:
                                 heights_diffs = []
-                                for h in self.animal_heights[i][
-                                    n - self.length + 1 : n + 1
-                                ]:
+                                for h in self.animal_heights[i][n - self.length + 1 : n + 1]:
                                     if h is None or self.animal_heights[i][n] is None:
                                         height_diff = 0.0
                                     else:
-                                        height_diff = (
-                                            abs(h - self.animal_heights[i][n]) / h
-                                        )
+                                        height_diff = abs(h - self.animal_heights[i][n]) / h
                                     heights_diffs.append(height_diff)
                                 magnitude_length = max(heights_diffs)
-                                vigor_length = magnitude_length / (
-                                    (self.length - np.argmax(heights_diffs)) / self.fps
-                                )
-                                intensity_length = sum(heights_diffs) / (
-                                    self.length / self.fps
-                                )
+                                vigor_length = magnitude_length / ((self.length - np.argmax(heights_diffs)) / self.fps)
+                                intensity_length = sum(heights_diffs) / (self.length / self.fps)
                                 if magnitude_length > 0:
-                                    self.all_behavior_parameters[behavior_name][
-                                        "magnitude_length"
-                                    ][i][n] = magnitude_length
+                                    self.all_behavior_parameters[behavior_name]["magnitude_length"][i][n] = (
+                                        magnitude_length
+                                    )
                                 if vigor_length > 0:
-                                    self.all_behavior_parameters[behavior_name][
-                                        "vigor_length"
-                                    ][i][n] = vigor_length
+                                    self.all_behavior_parameters[behavior_name]["vigor_length"][i][n] = vigor_length
                                 if intensity_length > 0:
-                                    self.all_behavior_parameters[behavior_name][
-                                        "intensity_length"
-                                    ][i][n] = intensity_length
+                                    self.all_behavior_parameters[behavior_name]["intensity_length"][i][n] = (
+                                        intensity_length
+                                    )
 
                             if "4 locomotion parameters" in parameter_to_analyze:
                                 distance_traveled = 0.0
                                 d = n - self.length
                                 while d < n - 1:
                                     start_center = self.animal_centers[i][d]
                                     end_center = self.animal_centers[i][d + 1]
@@ -1252,157 +1118,107 @@
                                 if normalize_distance is True:
                                     calibrator = math.sqrt(self.animal_area)
                                     distance_traveled = distance_traveled / calibrator
                                 speed = distance_traveled / (self.length / self.fps)
                                 end_center = self.animal_centers[i][n]
                                 if end_center is not None:
                                     displacements = []
-                                    for ct in self.animal_centers[i][
-                                        n - self.length + 1 : n + 1
-                                    ]:
+                                    for ct in self.animal_centers[i][n - self.length + 1 : n + 1]:
                                         if ct is None:
                                             displacements.append(0)
                                         else:
-                                            displacements.append(
-                                                math.dist(end_center, ct)
-                                            )
+                                            displacements.append(math.dist(end_center, ct))
                                     displacement = max(displacements)
                                     if normalize_distance is True:
                                         displacement = displacement / calibrator
-                                    velocity = displacement / (
-                                        (self.length - np.argmax(displacements))
-                                        / self.fps
-                                    )
-                                    self.all_behavior_parameters[behavior_name][
-                                        "velocity"
-                                    ][i][n] = velocity
+                                    velocity = displacement / ((self.length - np.argmax(displacements)) / self.fps)
+                                    self.all_behavior_parameters[behavior_name]["velocity"][i][n] = velocity
                                 velocities_max = []
                                 velocities_min = []
-                                for v in self.all_behavior_parameters[behavior_name][
-                                    "velocity"
-                                ][i][n - self.length + 1 : n + 1]:
+                                for v in self.all_behavior_parameters[behavior_name]["velocity"][i][
+                                    n - self.length + 1 : n + 1
+                                ]:
                                     if v != np.nan:
                                         velocities_max.append(v)
                                         velocities_min.append(v)
                                     else:
                                         velocities_max.append(-float("inf"))
                                         velocities_min.append(float("inf"))
                                 vmax = max(velocities_max)
                                 vmin = min(velocities_min)
                                 if vmax != -float("inf") and vmin != float("inf"):
-                                    if np.argmax(velocities_max) != np.argmin(
-                                        velocities_min
-                                    ):
-                                        t = (
-                                            abs(
-                                                np.argmax(velocities_max)
-                                                - np.argmin(velocities_min)
-                                            )
-                                            / self.fps
-                                        )
-                                        self.all_behavior_parameters[behavior_name][
-                                            "acceleration"
-                                        ][i][n] = (vmax - vmin) / t
-                                self.all_behavior_parameters[behavior_name]["distance"][
-                                    i
-                                ] += distance_traveled
-                                self.all_behavior_parameters[behavior_name]["speed"][i][
-                                    n
-                                ] = speed
+                                    if np.argmax(velocities_max) != np.argmin(velocities_min):
+                                        t = abs(np.argmax(velocities_max) - np.argmin(velocities_min)) / self.fps
+                                        self.all_behavior_parameters[behavior_name]["acceleration"][i][n] = (
+                                            vmax - vmin
+                                        ) / t
+                                self.all_behavior_parameters[behavior_name]["distance"][i] += distance_traveled
+                                self.all_behavior_parameters[behavior_name]["speed"][i][n] = speed
 
                             if "3 areal parameters" in parameter_to_analyze:
                                 mask = np.zeros_like(self.background)
                                 contour = self.animal_contours[i][n]
                                 if contour is not None:
-                                    cv2.drawContours(
-                                        mask, [contour], 0, (255, 255, 255), -1
-                                    )
+                                    cv2.drawContours(mask, [contour], 0, (255, 255, 255), -1)
                                     mask = cv2.cvtColor(mask, cv2.COLOR_BGR2GRAY)
                                     area_diffs = []
-                                    for ct in self.animal_contours[i][
-                                        n - self.length + 1 : n + 1
-                                    ]:
+                                    for ct in self.animal_contours[i][n - self.length + 1 : n + 1]:
                                         if ct is not None:
                                             prev_mask = np.zeros_like(self.background)
-                                            cv2.drawContours(
-                                                prev_mask, [ct], 0, (255, 255, 255), -1
-                                            )
-                                            prev_mask = cv2.cvtColor(
-                                                prev_mask, cv2.COLOR_BGR2GRAY
-                                            )
+                                            cv2.drawContours(prev_mask, [ct], 0, (255, 255, 255), -1)
+                                            prev_mask = cv2.cvtColor(prev_mask, cv2.COLOR_BGR2GRAY)
                                             xlf1, ybt1, w, h = cv2.boundingRect(contour)
                                             xrt1 = xlf1 + w
                                             ytp1 = ybt1 + h
                                             xlf2, ybt2, w, h = cv2.boundingRect(ct)
                                             xrt2 = xlf2 + w
                                             ytp2 = ybt2 + h
                                             xlf = min(xlf1, xlf2)
                                             xrt = max(xrt1, xrt2)
                                             ybt = min(ybt1, ybt2)
                                             ytp = max(ytp1, ytp2)
                                             curr_mask = mask[ybt:ytp, xlf:xrt]
                                             prev_mask = prev_mask[ybt:ytp, xlf:xrt]
                                             diff = cv2.bitwise_xor(prev_mask, curr_mask)
                                             # diff[diff!=0]=255
-                                            area_diff = (np.sum(diff) / 255) / (
-                                                np.sum(prev_mask) / 255
-                                            )
+                                            area_diff = (np.sum(diff) / 255) / (np.sum(prev_mask) / 255)
                                             area_diffs.append(area_diff)
                                     if len(area_diffs) > 0:
                                         magnitude_area = max(area_diffs)
-                                        vigor_area = magnitude_area / (
-                                            (self.length - np.argmax(area_diffs))
-                                            / self.fps
-                                        )
-                                        intensity_area = sum(area_diffs) / (
-                                            self.length / self.fps
-                                        )
+                                        vigor_area = magnitude_area / ((self.length - np.argmax(area_diffs)) / self.fps)
+                                        intensity_area = sum(area_diffs) / (self.length / self.fps)
                                         if magnitude_area > 0:
-                                            self.all_behavior_parameters[behavior_name][
-                                                "magnitude_area"
-                                            ][i][n] = magnitude_area
+                                            self.all_behavior_parameters[behavior_name]["magnitude_area"][i][n] = (
+                                                magnitude_area
+                                            )
                                         if vigor_area > 0:
-                                            self.all_behavior_parameters[behavior_name][
-                                                "vigor_area"
-                                            ][i][n] = vigor_area
+                                            self.all_behavior_parameters[behavior_name]["vigor_area"][i][n] = vigor_area
                                         if intensity_area > 0:
-                                            self.all_behavior_parameters[behavior_name][
-                                                "intensity_area"
-                                            ][i][n] = intensity_area
+                                            self.all_behavior_parameters[behavior_name]["intensity_area"][i][n] = (
+                                                intensity_area
+                                            )
 
                     else:
                         if "3 length parameters" in parameter_to_analyze:
                             heights_diffs = []
-                            for h in self.animal_heights[i][
-                                n - self.length + 1 : n + 1
-                            ]:
+                            for h in self.animal_heights[i][n - self.length + 1 : n + 1]:
                                 if h is None or self.animal_heights[i][n] is None:
                                     height_diff = 0.0
                                 else:
                                     height_diff = abs(h - self.animal_heights[i][n]) / h
                                 heights_diffs.append(height_diff)
                             magnitude_length = max(heights_diffs)
-                            vigor_length = magnitude_length / (
-                                (self.length - np.argmax(heights_diffs)) / self.fps
-                            )
-                            intensity_length = sum(heights_diffs) / (
-                                self.length / self.fps
-                            )
+                            vigor_length = magnitude_length / ((self.length - np.argmax(heights_diffs)) / self.fps)
+                            intensity_length = sum(heights_diffs) / (self.length / self.fps)
                             if magnitude_length > 0:
-                                self.all_behavior_parameters["magnitude_length"][i][
-                                    n
-                                ] = magnitude_length
+                                self.all_behavior_parameters["magnitude_length"][i][n] = magnitude_length
                             if vigor_length > 0:
-                                self.all_behavior_parameters["vigor_length"][i][
-                                    n
-                                ] = vigor_length
+                                self.all_behavior_parameters["vigor_length"][i][n] = vigor_length
                             if intensity_length > 0:
-                                self.all_behavior_parameters["intensity_length"][i][
-                                    n
-                                ] = intensity_length
+                                self.all_behavior_parameters["intensity_length"][i][n] = intensity_length
 
                         if "4 locomotion parameters" in parameter_to_analyze:
                             distance_traveled = 0.0
                             d = n - self.length
                             while d < n - 1:
                                 start_center = self.animal_centers[i][d]
                                 end_center = self.animal_centers[i][d + 1]
@@ -1415,151 +1231,97 @@
                             if normalize_distance is True:
                                 calibrator = math.sqrt(self.animal_area)
                                 distance_traveled = distance_traveled / calibrator
                             speed = distance_traveled / (self.length / self.fps)
                             end_center = self.animal_centers[i][n]
                             if end_center is not None:
                                 displacements = []
-                                for ct in self.animal_centers[i][
-                                    n - self.length + 1 : n + 1
-                                ]:
+                                for ct in self.animal_centers[i][n - self.length + 1 : n + 1]:
                                     if ct is None:
                                         displacements.append(0)
                                     else:
                                         displacements.append(math.dist(end_center, ct))
                                 displacement = max(displacements)
                                 if normalize_distance is True:
                                     displacement = displacement / calibrator
-                                velocity = displacement / (
-                                    (self.length - np.argmax(displacements)) / self.fps
-                                )
-                                self.all_behavior_parameters["velocity"][i][
-                                    n
-                                ] = velocity
+                                velocity = displacement / ((self.length - np.argmax(displacements)) / self.fps)
+                                self.all_behavior_parameters["velocity"][i][n] = velocity
                             velocities_max = []
                             velocities_min = []
-                            for v in self.all_behavior_parameters["velocity"][i][
-                                n - self.length + 1 : n + 1
-                            ]:
+                            for v in self.all_behavior_parameters["velocity"][i][n - self.length + 1 : n + 1]:
                                 if v != np.nan:
                                     velocities_max.append(v)
                                     velocities_min.append(v)
                                 else:
                                     velocities_max.append(-float("inf"))
                                     velocities_min.append(float("inf"))
                             vmax = max(velocities_max)
                             vmin = min(velocities_min)
                             if vmax != -float("inf") and vmin != float("inf"):
-                                if np.argmax(velocities_max) != np.argmin(
-                                    velocities_min
-                                ):
-                                    t = (
-                                        abs(
-                                            np.argmax(velocities_max)
-                                            - np.argmin(velocities_min)
-                                        )
-                                        / self.fps
-                                    )
-                                    self.all_behavior_parameters["acceleration"][i][
-                                        n
-                                    ] = (vmax - vmin) / t
-                            self.all_behavior_parameters["distance"][
-                                i
-                            ] += distance_traveled
+                                if np.argmax(velocities_max) != np.argmin(velocities_min):
+                                    t = abs(np.argmax(velocities_max) - np.argmin(velocities_min)) / self.fps
+                                    self.all_behavior_parameters["acceleration"][i][n] = (vmax - vmin) / t
+                            self.all_behavior_parameters["distance"][i] += distance_traveled
                             self.all_behavior_parameters["speed"][i][n] = speed
 
                         if "3 areal parameters" in parameter_to_analyze:
                             mask = np.zeros_like(self.background)
                             contour = self.animal_contours[i][n]
                             if contour is not None:
-                                cv2.drawContours(
-                                    mask, [contour], 0, (255, 255, 255), -1
-                                )
+                                cv2.drawContours(mask, [contour], 0, (255, 255, 255), -1)
                                 mask = cv2.cvtColor(mask, cv2.COLOR_BGR2GRAY)
                                 area_diffs = []
-                                for ct in self.animal_contours[i][
-                                    n - self.length + 1 : n + 1
-                                ]:
+                                for ct in self.animal_contours[i][n - self.length + 1 : n + 1]:
                                     if ct is not None:
                                         prev_mask = np.zeros_like(self.background)
-                                        cv2.drawContours(
-                                            prev_mask, [ct], 0, (255, 255, 255), -1
-                                        )
-                                        prev_mask = cv2.cvtColor(
-                                            prev_mask, cv2.COLOR_BGR2GRAY
-                                        )
+                                        cv2.drawContours(prev_mask, [ct], 0, (255, 255, 255), -1)
+                                        prev_mask = cv2.cvtColor(prev_mask, cv2.COLOR_BGR2GRAY)
                                         xlf1, ybt1, w, h = cv2.boundingRect(contour)
                                         xrt1 = xlf1 + w
                                         ytp1 = ybt1 + h
                                         xlf2, ybt2, w, h = cv2.boundingRect(ct)
                                         xrt2 = xlf2 + w
                                         ytp2 = ybt2 + h
                                         xlf = min(xlf1, xlf2)
                                         xrt = max(xrt1, xrt2)
                                         ybt = min(ybt1, ybt2)
                                         ytp = max(ytp1, ytp2)
                                         curr_mask = mask[ybt:ytp, xlf:xrt]
                                         prev_mask = prev_mask[ybt:ytp, xlf:xrt]
                                         diff = cv2.bitwise_xor(prev_mask, curr_mask)
                                         # diff[diff!=0]=255
-                                        area_diff = (np.sum(diff) / 255) / (
-                                            np.sum(prev_mask) / 255
-                                        )
+                                        area_diff = (np.sum(diff) / 255) / (np.sum(prev_mask) / 255)
                                         area_diffs.append(area_diff)
                                 if len(area_diffs) > 0:
                                     magnitude_area = max(area_diffs)
-                                    vigor_area = magnitude_area / (
-                                        (self.length - np.argmax(area_diffs)) / self.fps
-                                    )
-                                    intensity_area = sum(area_diffs) / (
-                                        self.length / self.fps
-                                    )
+                                    vigor_area = magnitude_area / ((self.length - np.argmax(area_diffs)) / self.fps)
+                                    intensity_area = sum(area_diffs) / (self.length / self.fps)
                                     if magnitude_area > 0:
-                                        self.all_behavior_parameters["magnitude_area"][
-                                            i
-                                        ][n] = magnitude_area
+                                        self.all_behavior_parameters["magnitude_area"][i][n] = magnitude_area
                                     if vigor_area > 0:
-                                        self.all_behavior_parameters["vigor_area"][i][
-                                            n
-                                        ] = vigor_area
+                                        self.all_behavior_parameters["vigor_area"][i][n] = vigor_area
                                     if intensity_area > 0:
-                                        self.all_behavior_parameters["intensity_area"][
-                                            i
-                                        ][n] = intensity_area
+                                        self.all_behavior_parameters["intensity_area"][i][n] = intensity_area
 
                     n += 1
 
                 if self.categorize_behavior is True:
                     if "duration" in parameter_to_analyze:
                         for behavior_name in self.all_behavior_parameters:
-                            if (
-                                self.all_behavior_parameters[behavior_name]["duration"][
-                                    i
-                                ]
-                                != 0.0
-                            ):
-                                self.all_behavior_parameters[behavior_name]["duration"][
-                                    i
-                                ] += round(self.length / self.fps, 2)
+                            if self.all_behavior_parameters[behavior_name]["duration"][i] != 0.0:
+                                self.all_behavior_parameters[behavior_name]["duration"][i] += round(
+                                    self.length / self.fps, 2
+                                )
                             else:
-                                self.all_behavior_parameters[behavior_name]["duration"][
-                                    i
-                                ] = "NA"
+                                self.all_behavior_parameters[behavior_name]["duration"][i] = "NA"
 
                     if "4 locomotion parameters" in parameter_to_analyze:
                         for behavior_name in self.all_behavior_parameters:
-                            if (
-                                self.all_behavior_parameters[behavior_name]["distance"][
-                                    i
-                                ]
-                                == 0.0
-                            ):
-                                self.all_behavior_parameters[behavior_name]["distance"][
-                                    i
-                                ] = "NA"
+                            if self.all_behavior_parameters[behavior_name]["distance"][i] == 0.0:
+                                self.all_behavior_parameters[behavior_name]["distance"][i] = "NA"
 
     def export_results(self, normalize_distance=True, parameter_to_analyze=[]):
         print("Quantifying behaviors...")
         print(datetime.datetime.now())
 
         self.analyze_parameters(
             normalize_distance=normalize_distance,
@@ -1567,14 +1329,25 @@
         )
 
         print("Behavioral quantification completed!")
 
         print("Exporting results...")
         print(datetime.datetime.now())
 
+        # Export centers data every time
+        pd.DataFrame.from_dict(
+            self.animal_centers,
+            orient="index",
+            columns=self.all_time,
+        ).reset_index(drop=True).transpose().to_excel(
+            os.path.join(self.results_path, "centers.xlsx"),
+            float_format="%.2f",
+            index_label="time/ID",
+        )
+
         if self.categorize_behavior is True:
             events_df = pd.DataFrame(self.event_probability, index=self.all_time)
             events_df.to_excel(
                 os.path.join(self.results_path, "all_event_probability.xlsx"),
                 float_format="%.2f",
                 index_label="time/ID",
             )
@@ -1595,27 +1368,23 @@
         if "3 areal parameters" in parameter_to_analyze:
             all_parameters += ["intensity_area", "magnitude_area", "vigor_area"]
         if "4 locomotion parameters" in parameter_to_analyze:
             all_parameters += ["acceleration", "distance", "speed", "velocity"]
 
         if self.categorize_behavior is True:
             for behavior_name in self.all_behavior_parameters:
-                os.makedirs(
-                    os.path.join(self.results_path, behavior_name), exist_ok=True
-                )
+                os.makedirs(os.path.join(self.results_path, behavior_name), exist_ok=True)
 
                 summary = []
 
                 for parameter_name in all_parameters:
                     if parameter_name in ["count", "duration", "distance", "latency"]:
                         summary.append(
                             pd.DataFrame.from_dict(
-                                self.all_behavior_parameters[behavior_name][
-                                    parameter_name
-                                ],
+                                self.all_behavior_parameters[behavior_name][parameter_name],
                                 orient="index",
                                 columns=[parameter_name],
                             ).reset_index(drop=True)
                         )
                     else:
                         individual_df = pd.DataFrame.from_dict(
                             self.all_behavior_parameters[behavior_name][parameter_name],
@@ -1653,17 +1422,15 @@
                             ),
                             float_format="%.2f",
                             index_label="time/ID",
                         )
 
                 if len(summary) >= 1:
                     pd.concat(summary, axis=1).to_excel(
-                        os.path.join(
-                            self.results_path, behavior_name, "all_summary.xlsx"
-                        ),
+                        os.path.join(self.results_path, behavior_name, "all_summary.xlsx"),
                         float_format="%.2f",
                         index_label="ID/parameter",
                     )
 
         else:
             summary = []
 
@@ -1732,17 +1499,15 @@
             background_high = np.uint8(255 - background_high)
 
         capture = cv2.VideoCapture(self.path_to_video)
         frame_count = frame_count_analyze = 0
         temp_frames = deque(maxlen=self.length)
 
         for i in range(self.animal_number):
-            os.makedirs(
-                os.path.join(self.results_path, "examples", str(i)), exist_ok=True
-            )
+            os.makedirs(os.path.join(self.results_path, "examples", str(i)), exist_ok=True)
 
         if self.t is not None and self.length is not None:
             start_t = round((self.t - self.length / self.fps), 2)
         else:
             start_t = 0.0
 
         if self.duration == 0:
@@ -1787,36 +1552,29 @@
                         contours,
                         centers,
                         heights,
                         inners=inners,
                         blobs=None,
                     )
 
-                    if (
-                        frame_count_analyze >= self.length
-                        and frame_count_analyze % skip_redundant == 0
-                    ):
+                    if frame_count_analyze >= self.length and frame_count_analyze % skip_redundant == 0:
                         for n in self.animal_centers:
                             h = w = 0
                             animation = []
                             for i, f in enumerate(temp_frames):
                                 contour = self.animal_contours[n][
-                                    frame_count_analyze
-                                    - self.length
-                                    + 1 : frame_count_analyze + 1
+                                    frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                 ][i]
                                 if contour is None:
                                     blob = np.zeros_like(f)
                                 else:
                                     blob = extract_blob_background(
                                         f,
                                         self.animal_contours[n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         contour=contour,
                                         channel=3,
                                         background_free=background_free,
                                     )
                                     h, w = blob.shape[:2]
                                 animation.append(blob)
@@ -1846,17 +1604,15 @@
                                         + "_std"
                                         + str(self.std)
                                         + ".jpg"
                                     )
                                     pattern_image = generate_patternimage(
                                         self.background,
                                         self.animal_contours[n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         inners=self.animal_inners[n],
                                         std=self.std,
                                     )
                                 else:
                                     animation_name = (
                                         os.path.splitext(self.basename)[0]
@@ -1877,17 +1633,15 @@
                                         + "_len"
                                         + str(self.length)
                                         + ".jpg"
                                     )
                                     pattern_image = generate_patternimage(
                                         self.background,
                                         self.animal_contours[n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         inners=None,
                                         std=0,
                                     )
 
                                 path_animation = os.path.join(
                                     self.results_path,
@@ -1906,19 +1660,15 @@
                                     path_animation,
                                     cv2.VideoWriter_fourcc(*"MJPG"),
                                     self.fps / 5,
                                     (w, h),
                                     True,
                                 )
                                 for blob in animation:
-                                    writer.write(
-                                        cv2.resize(
-                                            blob, (w, h), interpolation=cv2.INTER_AREA
-                                        )
-                                    )
+                                    writer.write(cv2.resize(blob, (w, h), interpolation=cv2.INTER_AREA))
                                 writer.release()
 
                                 cv2.imwrite(path_pattern_image, pattern_image)
 
                 frame_count_analyze += 1
 
             frame_count += 1
@@ -1991,18 +1741,15 @@
                     temp_inners.append(None)
                     animation.append(np.zeros_like(self.background))
 
                 else:
                     temp_contours.append(contours)
                     temp_inners.append(inners)
 
-                    if (
-                        frame_count_analyze >= self.length
-                        and frame_count_analyze % skip_redundant == 0
-                    ):
+                    if frame_count_analyze >= self.length and frame_count_analyze % skip_redundant == 0:
                         (y_bt, y_tp, x_lf, x_rt) = crop_frame(
                             frame, functools.reduce(operator.iconcat, temp_contours, [])
                         )
 
                         h = w = 0
                         for i, f in enumerate(temp_frames):
                             if temp_contours[i] is None:
@@ -2077,34 +1824,26 @@
                                     x_lf,
                                     x_rt,
                                     temp_contours,
                                     temp_inners,
                                     std=0,
                                 )
 
-                            path_animation = os.path.join(
-                                self.results_path, "examples", "0", animation_name
-                            )
-                            path_pattern_image = os.path.join(
-                                self.results_path, "examples", "0", pattern_image_name
-                            )
+                            path_animation = os.path.join(self.results_path, "examples", "0", animation_name)
+                            path_pattern_image = os.path.join(self.results_path, "examples", "0", pattern_image_name)
 
                             writer = cv2.VideoWriter(
                                 path_animation,
                                 cv2.VideoWriter_fourcc(*"MJPG"),
                                 self.fps / 5,
                                 (w, h),
                                 True,
                             )
                             for blob in animation:
-                                writer.write(
-                                    cv2.resize(
-                                        blob, (w, h), interpolation=cv2.INTER_AREA
-                                    )
-                                )
+                                writer.write(cv2.resize(blob, (w, h), interpolation=cv2.INTER_AREA))
                             writer.release()
 
                             cv2.imwrite(path_pattern_image, pattern_image)
 
                 frame_count_analyze += 1
 
             frame_count += 1
```

### Comparing `labgym-2.3.5/LabGym/analyzebehaviorsdetector.py` & `labgym-2.4.0/LabGym/analyzebehaviorsdetector.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,250 +15,31 @@
 
 Email: bingye@umich.edu
 """
 
 import datetime
 import functools
 import gc
-import json
 import math
 import operator
 import os
-import shutil
 from collections import deque
-from pathlib import Path
 
 import cv2
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 import torch
 from scipy.spatial import distance
 from skimage import exposure
 from tensorflow.keras.models import load_model
 from tensorflow.keras.preprocessing.image import img_to_array
 
-from .tools import *
-
-try:
-    from detectron2 import model_zoo
-    from detectron2.checkpoint import DetectionCheckpointer
-    from detectron2.config import get_cfg
-    from detectron2.data import (
-        DatasetCatalog,
-        MetadataCatalog,
-        build_detection_test_loader,
-    )
-    from detectron2.data.datasets import register_coco_instances
-    from detectron2.engine import DefaultPredictor, DefaultTrainer
-    from detectron2.evaluation import COCOEvaluator, inference_on_dataset
-    from detectron2.modeling import build_model
-    from detectron2.utils.visualizer import Visualizer
-except:
-    print("You need to install Detectron2 to use the Detector module in LabGym:")
-    print("https://detectron2.readthedocs.io/en/latest/tutorials/install.html")
-
-
-DETECTOR_FOLDER = Path(__file__).resolve().parent / "detectors"
-
-
-def get_detector_names() -> list[str]:
-    """Return the names of all saved detectors."""
-    ignore = ["__pycache__", "__init__", "__init.py__"]
-    return [
-        path.name
-        for path in DETECTOR_FOLDER.glob("*")
-        if path.is_dir() and path.name not in ignore
-    ]
-
-
-def get_animal_names(detector_name: str) -> list[str]:
-    """Return a list of animal names associated with the given Detector.
-
-    Args:
-        detector_name: The name of the Detector.
-
-    Raises:
-        FileNotFoundError: The Detector doesn't exist (this should be taken
-            care of by the detector selection).
-    """
-    animalmapping = DETECTOR_FOLDER / detector_name / "model_parameters.txt"
-    with open(animalmapping) as f:
-        model_parameters = f.read()
-    return json.loads(model_parameters)["animal_names"]
-
-
-def get_annotation_class_names(annotation_path: str) -> list[str]:
-    """Return a list of class names associated with the annotation file.
-
-    Args:
-        annotation_path: The absolute path to the COCO annotation file.
-
-    Raises:
-        FileNotFoundError: The annotation file doesn't exist (this should
-            be taken care of by the file selection GUI).
-    """
-    with open(annotation_path) as f:
-        info = json.load(f)
-    classnames = []
-    for category in info["categories"]:
-        if category["id"] > 0:
-            classnames.append(category["name"])
-    return classnames
-
-
-def delete_detector(detector_name: str):
-    """Permanently delete the given detector."""
-    shutil.rmtree(str(DETECTOR_FOLDER / detector_name))
-
-
-def train_detector(
-    path_to_annotation: str,
-    path_to_trainingimages: str,
-    detector_name: str,
-    iteration_num: int,
-    inference_size: int,
-):
-    path_to_detector = str(DETECTOR_FOLDER / detector_name)
-    if torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    if str("LabGym_detector_train") in DatasetCatalog.list():
-        DatasetCatalog.remove("LabGym_detector_train")
-        MetadataCatalog.remove("LabGym_detector_train")
-    register_coco_instances(
-        "LabGym_detector_train", {}, path_to_annotation, path_to_trainingimages
-    )
-    datasetcat = DatasetCatalog.get("LabGym_detector_train")
-    metadatacat = MetadataCatalog.get("LabGym_detector_train")
-    classnames = metadatacat.thing_classes
-
-    model_parameters_dict = {}
-    model_parameters_dict["animal_names"] = []
-    annotation_data = json.load(open(path_to_annotation))
-    for i in annotation_data["categories"]:
-        if i["id"] > 0:
-            model_parameters_dict["animal_names"].append(i["name"])
-    print(
-        "Animal names in annotation file: " + str(model_parameters_dict["animal_names"])
-    )
-
-    cfg = get_cfg()
-    cfg.merge_from_file(
-        model_zoo.get_config_file(
-            "COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml"
-        )
-    )
-    cfg.OUTPUT_DIR = path_to_detector
-    cfg.DATASETS.TRAIN = ("LabGym_detector_train",)
-    cfg.DATASETS.TEST = ()
-    cfg.DATALOADER.NUM_WORKERS = 4
-    cfg.MODEL.WEIGHTS = model_zoo.get_checkpoint_url(
-        "COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml"
-    )
-    cfg.MODEL.ROI_HEADS.BATCH_SIZE_PER_IMAGE = 128
-    cfg.MODEL.ROI_HEADS.NUM_CLASSES = int(len(classnames))
-    cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = 0.5
-    cfg.SOLVER.MAX_ITER = int(iteration_num)
-    cfg.SOLVER.BASE_LR = 0.001
-    cfg.SOLVER.WARMUP_ITERS = int(iteration_num * 0.1)
-    cfg.SOLVER.STEPS = (int(iteration_num * 0.4), int(iteration_num * 0.8))
-    cfg.SOLVER.GAMMA = 0.5
-    cfg.SOLVER.IMS_PER_BATCH = 4
-    cfg.MODEL.DEVICE = device
-    cfg.INPUT.MIN_SIZE_TEST = int(inference_size)
-    cfg.INPUT.MAX_SIZE_TEST = int(inference_size)
-    cfg.INPUT.MIN_SIZE_TRAIN = (int(inference_size),)
-    cfg.INPUT.MAX_SIZE_TRAIN = int(inference_size)
-    os.makedirs(cfg.OUTPUT_DIR)
-    trainer = DefaultTrainer(cfg)
-    trainer.resume_or_load(False)
-    trainer.train()
-
-    model_parameters = os.path.join(cfg.OUTPUT_DIR, "model_parameters.txt")
-
-    model_parameters_dict["animal_mapping"] = {}
-    model_parameters_dict["inferencing_framesize"] = int(inference_size)
-
-    for i in range(len(classnames)):
-        model_parameters_dict["animal_mapping"][i] = classnames[i]
-
-    with open(model_parameters, "w") as f:
-        f.write(json.dumps(model_parameters_dict))
-
-    predictor = DefaultPredictor(cfg)
-    model = predictor.model
-    DetectionCheckpointer(model).resume_or_load(
-        os.path.join(cfg.OUTPUT_DIR, "model_final.pth")
-    )
-    model.eval()
-
-    config = os.path.join(cfg.OUTPUT_DIR, "config.yaml")
-    with open(config, "w") as f:
-        f.write(cfg.dump())
-
-    print("Detector training completed!")
-
-
-def test_detector(
-    path_to_annotation: str,
-    path_to_testingimages: str,
-    detector_name: str,
-    output_path: str,
-):
-    path_to_detector = str(DETECTOR_FOLDER / detector_name)
-    if str("LabGym_detector_test") in DatasetCatalog.list():
-        DatasetCatalog.remove("LabGym_detector_test")
-        MetadataCatalog.remove("LabGym_detector_test")
-    register_coco_instances(
-        "LabGym_detector_test", {}, path_to_annotation, path_to_testingimages
-    )
-    datasetcat = DatasetCatalog.get("LabGym_detector_test")
-    metadatacat = MetadataCatalog.get("LabGym_detector_test")
-
-    animalmapping = os.path.join(path_to_detector, "model_parameters.txt")
-    with open(animalmapping) as f:
-        model_parameters = f.read()
-    animal_names = json.loads(model_parameters)["animal_names"]
-    dt_infersize = int(json.loads(model_parameters)["inferencing_framesize"])
-    print(
-        "The total categories of animals / objects in this Detector: "
-        + str(animal_names)
-    )
-    print("The inferencing framesize of this Detector: " + str(dt_infersize))
-    cfg = get_cfg()
-    cfg.merge_from_file(os.path.join(path_to_detector, "config.yaml"))
-    cfg.MODEL.WEIGHTS = os.path.join(path_to_detector, "model_final.pth")
-    cfg.MODEL.DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
-
-    predictor = DefaultPredictor(cfg)
-
-    for d in datasetcat:
-        im = cv2.imread(d["file_name"])
-        outputs = predictor(im)
-        v = Visualizer(
-            im[:, :, ::-1], MetadataCatalog.get("LabGym_detector_test"), scale=1.2
-        )
-        out = v.draw_instance_predictions(outputs["instances"].to("cpu"))
-        cv2.imwrite(
-            os.path.join(output_path, os.path.basename(d["file_name"])),
-            out.get_image()[:, :, ::-1],
-        )
-
-    evaluator = COCOEvaluator(
-        "LabGym_detector_test", cfg, False, output_dir=output_path
-    )
-    val_loader = build_detection_test_loader(cfg, "LabGym_detector_test")
-    inference_on_dataset(predictor.model, val_loader, evaluator)
-    mAP = evaluator._results["bbox"]["AP"]
-    print(f"The mean average precision (mAP) of the Detector is: {mAP:.4f}" + "%.")
-
-    print("Detector testing completed!")
+from LabGym.detector import Detector
+from LabGym.tools import *
 
 
 class AnalyzeAnimalDetector:
     def __init__(self):
         self.behavior_mode = 0
         self.detector = None
         self.animal_mapping = None
@@ -326,43 +107,24 @@
         duration=5,  # the duration for example generation / analysis
         length=15,  # the duration (number of frames) of a behavior example (a behavior episode)
         social_distance=0,  # the distance to determine which two animals / objects form a interactive pair / group
     ):
         print("Preparation started...")
         print(datetime.datetime.now())
 
-        config = os.path.join(path_to_detector, "config.yaml")
-        detector = os.path.join(path_to_detector, "model_final.pth")
-        animalmapping = os.path.join(path_to_detector, "model_parameters.txt")
-        with open(animalmapping) as f:
-            model_parameters = f.read()
-        self.animal_mapping = json.loads(model_parameters)["animal_mapping"]
-        animal_names = json.loads(model_parameters)["animal_names"]
-        dt_infersize = int(json.loads(model_parameters)["inferencing_framesize"])
-        print(
-            "The total categories of animals / objects in this Detector: "
-            + str(animal_names)
-        )
-        print(
-            "The animals / objects of interest in this Detector: " + str(animal_kinds)
-        )
-        print("The inferencing framesize of this Detector: " + str(dt_infersize))
-        cfg = get_cfg()
-        cfg.merge_from_file(config)
-        cfg.MODEL.DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
-        self.detector = build_model(cfg)
-        DetectionCheckpointer(self.detector).load(detector)
-        self.detector.eval()
+        self.detector = Detector(path=path_to_detector)
+        print(f"The total categories of animals / objects in this Detector: {self.detector.animal_names}")
+        print(f"The animals / objects of interest in this Detector: {animal_kinds}")
+        print(f"The inferencing framesize of this Detector: {self.detector.inferencing_framesize}")
+        self.animal_mapping = self.detector.animal_mapping
 
         self.path_to_video = path_to_video
         self.basename = os.path.basename(self.path_to_video)
         self.framewidth = framewidth
-        self.results_path = os.path.join(
-            results_path, os.path.splitext(self.basename)[0]
-        )
+        self.results_path = os.path.join(results_path, os.path.splitext(self.basename)[0])
         self.animal_number = animal_number
         self.animal_kinds = animal_kinds
         self.behavior_mode = behavior_mode
         self.dim_tconv = dim_tconv
         self.dim_conv = dim_conv
         self.channel = channel
         self.include_bodyparts = include_bodyparts
@@ -377,60 +139,44 @@
             self.social_distance = float("inf")
         os.makedirs(self.results_path, exist_ok=True)
         capture = cv2.VideoCapture(self.path_to_video)
         self.fps = round(capture.get(cv2.CAP_PROP_FPS))
         self.count_to_deregister = self.fps * 2
 
         if self.duration <= 0:
-            self.total_analysis_framecount = (
-                int(capture.get(cv2.CAP_PROP_FRAME_COUNT)) + 1
-            )
+            self.total_analysis_framecount = int(capture.get(cv2.CAP_PROP_FRAME_COUNT)) + 1
         else:
             self.total_analysis_framecount = int(self.fps * self.duration) + 1
 
         while True:
             retval, frame = capture.read()
             break
         capture.release()
 
         print("Video fps: " + str(self.fps))
-        print(
-            "The original video framesize: "
-            + str(int(frame.shape[0]))
-            + " X "
-            + str(int(frame.shape[1]))
-        )
+        print("The original video framesize: " + str(int(frame.shape[0])) + " X " + str(int(frame.shape[1])))
 
         if self.framewidth is not None:
             self.frameheight = int(frame.shape[0] * self.framewidth / frame.shape[1])
-            self.background = cv2.resize(
-                frame, (self.framewidth, self.frameheight), interpolation=cv2.INTER_AREA
-            )
-            print(
-                "The resized video framesize: "
-                + str(self.frameheight)
-                + " X "
-                + str(self.framewidth)
-            )
+            self.background = cv2.resize(frame, (self.framewidth, self.frameheight), interpolation=cv2.INTER_AREA)
+            print("The resized video framesize: " + str(self.frameheight) + " X " + str(self.framewidth))
         else:
             self.background = frame
         self.temp_frames = deque(maxlen=self.length)
         framesize = min(self.background.shape[0], self.background.shape[1])
 
         total_number = 0
         for animal_name in self.animal_kinds:
             total_number += self.animal_number[animal_name]
             if self.categorize_behavior is True:
                 self.event_probability[animal_name] = {}
                 self.all_behavior_parameters[animal_name] = {}
                 for behavior_name in names_and_colors:
                     self.all_behavior_parameters[animal_name][behavior_name] = {}
-                    self.all_behavior_parameters[animal_name][behavior_name][
-                        "color"
-                    ] = names_and_colors[behavior_name]
+                    self.all_behavior_parameters[animal_name][behavior_name]["color"] = names_and_colors[behavior_name]
                     for parameter_name in [
                         "acceleration",
                         "count",
                         "distance",
                         "duration",
                         "intensity_area",
                         "intensity_length",
@@ -439,17 +185,15 @@
                         "magnitude_length",
                         "probability",
                         "speed",
                         "velocity",
                         "vigor_area",
                         "vigor_length",
                     ]:
-                        self.all_behavior_parameters[animal_name][behavior_name][
-                            parameter_name
-                        ] = {}
+                        self.all_behavior_parameters[animal_name][behavior_name][parameter_name] = {}
             else:
                 self.dim_conv = 8
                 self.animation_analyzer = False
                 self.all_behavior_parameters[animal_name] = {}
                 for parameter_name in [
                     "acceleration",
                     "distance",
@@ -479,34 +223,24 @@
                     self.animal_other_inners[animal_name] = {}
             if self.animation_analyzer is True:
                 self.animal_blobs[animal_name] = {}
                 self.animations[animal_name] = {}
             for i in range(self.animal_number[animal_name]):
                 self.to_deregister[animal_name][i] = 0
                 self.register_counts[animal_name][i] = None
-                self.animal_contours[animal_name][i] = [
-                    None
-                ] * self.total_analysis_framecount
+                self.animal_contours[animal_name][i] = [None] * self.total_analysis_framecount
                 if self.behavior_mode == 2:
-                    self.animal_other_contours[animal_name][i] = deque(
-                        maxlen=self.length
-                    )
-                self.animal_centers[animal_name][i] = [
-                    None
-                ] * self.total_analysis_framecount
+                    self.animal_other_contours[animal_name][i] = deque(maxlen=self.length)
+                self.animal_centers[animal_name][i] = [None] * self.total_analysis_framecount
                 self.animal_existingcenters[animal_name][i] = (-10000, -10000)
-                self.animal_heights[animal_name][i] = [
-                    None
-                ] * self.total_analysis_framecount
+                self.animal_heights[animal_name][i] = [None] * self.total_analysis_framecount
                 if self.include_bodyparts is True:
                     self.animal_inners[animal_name][i] = deque(maxlen=self.length)
                     if self.behavior_mode == 2:
-                        self.animal_other_inners[animal_name][i] = deque(
-                            maxlen=self.length
-                        )
+                        self.animal_other_inners[animal_name][i] = deque(maxlen=self.length)
                 if self.animation_analyzer is True:
                     self.animal_blobs[animal_name][i] = (
                         deque(
                             [
                                 np.zeros(
                                     (self.dim_tconv, self.dim_tconv, self.channel),
                                     dtype="uint8",
@@ -561,74 +295,58 @@
             index_in_existing = int(idx / length)
             index_in_new = int(idx % length)
             if index_in_existing in unused_existing_indices:
                 if index_in_new in unused_new_indices:
                     unused_existing_indices.remove(index_in_existing)
                     unused_new_indices.remove(index_in_new)
                     if self.register_counts[animal_name][index_in_existing] is None:
-                        self.register_counts[animal_name][index_in_existing] = (
-                            frame_count_analyze
-                        )
+                        self.register_counts[animal_name][index_in_existing] = frame_count_analyze
                     self.to_deregister[animal_name][index_in_existing] = 0
-                    self.animal_contours[animal_name][index_in_existing][
-                        frame_count_analyze
-                    ] = contours[index_in_new]
+                    self.animal_contours[animal_name][index_in_existing][frame_count_analyze] = contours[index_in_new]
                     center = centers[index_in_new]
-                    self.animal_centers[animal_name][index_in_existing][
-                        frame_count_analyze
-                    ] = center
+                    self.animal_centers[animal_name][index_in_existing][frame_count_analyze] = center
                     self.animal_existingcenters[animal_name][index_in_existing] = center
-                    self.animal_heights[animal_name][index_in_existing][
-                        frame_count_analyze
-                    ] = heights[index_in_new]
+                    self.animal_heights[animal_name][index_in_existing][frame_count_analyze] = heights[index_in_new]
                     if self.animation_analyzer is True:
                         blob = img_to_array(
                             cv2.resize(
                                 blobs[index_in_new],
                                 (self.dim_tconv, self.dim_tconv),
                                 interpolation=cv2.INTER_AREA,
                             )
                         )
                         self.animal_blobs[animal_name][index_in_existing].append(blob)
-                        self.animations[animal_name][index_in_existing][
-                            frame_count_analyze
-                        ] = np.array(self.animal_blobs[animal_name][index_in_existing])
-                    if self.include_bodyparts is True:
-                        self.animal_inners[animal_name][index_in_existing].append(
-                            inners[index_in_new]
+                        self.animations[animal_name][index_in_existing][frame_count_analyze] = np.array(
+                            self.animal_blobs[animal_name][index_in_existing]
                         )
+                    if self.include_bodyparts is True:
+                        self.animal_inners[animal_name][index_in_existing].append(inners[index_in_new])
                         pattern_image = generate_patternimage(
                             self.background,
                             self.animal_contours[animal_name][index_in_existing][
-                                max(
-                                    0, (frame_count_analyze - self.length + 1)
-                                ) : frame_count_analyze + 1
+                                max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                             ],
                             inners=self.animal_inners[animal_name][index_in_existing],
                             std=self.std,
                         )
                     else:
                         pattern_image = generate_patternimage(
                             self.background,
                             self.animal_contours[animal_name][index_in_existing][
-                                max(
-                                    0, (frame_count_analyze - self.length + 1)
-                                ) : frame_count_analyze + 1
+                                max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                             ],
                             inners=None,
                             std=0,
                         )
                     pattern_image = cv2.resize(
                         pattern_image,
                         (self.dim_conv, self.dim_conv),
                         interpolation=cv2.INTER_AREA,
                     )
-                    self.pattern_images[animal_name][index_in_existing][
-                        frame_count_analyze
-                    ] = np.array(pattern_image)
+                    self.pattern_images[animal_name][index_in_existing][frame_count_analyze] = np.array(pattern_image)
 
         if len(unused_existing_indices) > 0:
             for i in unused_existing_indices:
                 if self.to_deregister[animal_name][i] <= self.count_to_deregister:
                     self.to_deregister[animal_name][i] += 1
                 else:
                     self.animal_existingcenters[animal_name][i] = (-10000, -10000)
@@ -665,131 +383,91 @@
                 if self.include_bodyparts is True:
                     animal_inners = inners[n:animal_length]
                     animal_other_inners = other_inners[n:animal_length]
                 if self.animation_analyzer is True:
                     animal_blobs = blobs[n:animal_length]
 
                 unused_existing_indices = list(self.animal_existingcenters[animal_name])
-                existing_centers = list(
-                    self.animal_existingcenters[animal_name].values()
-                )
+                existing_centers = list(self.animal_existingcenters[animal_name].values())
                 unused_new_indices = list(range(len(animal_centers)))
-                dt_flattened = distance.cdist(
-                    existing_centers, animal_centers
-                ).flatten()
+                dt_flattened = distance.cdist(existing_centers, animal_centers).flatten()
                 dt_sort_index = dt_flattened.argsort()
                 length = len(animal_centers)
 
                 for idx in dt_sort_index:
                     index_in_existing = int(idx / length)
                     index_in_new = int(idx % length)
                     if index_in_existing in unused_existing_indices:
                         if index_in_new in unused_new_indices:
                             unused_existing_indices.remove(index_in_existing)
                             unused_new_indices.remove(index_in_new)
-                            if (
-                                self.register_counts[animal_name][index_in_existing]
-                                is None
-                            ):
-                                self.register_counts[animal_name][index_in_existing] = (
-                                    frame_count_analyze
-                                )
+                            if self.register_counts[animal_name][index_in_existing] is None:
+                                self.register_counts[animal_name][index_in_existing] = frame_count_analyze
                             self.to_deregister[animal_name][index_in_existing] = 0
                             contour = animal_contours[index_in_new]
-                            self.animal_contours[animal_name][index_in_existing][
-                                frame_count_analyze
-                            ] = contour
+                            self.animal_contours[animal_name][index_in_existing][frame_count_analyze] = contour
                             center = animal_centers[index_in_new]
-                            self.animal_centers[animal_name][index_in_existing][
-                                frame_count_analyze
-                            ] = center
-                            self.animal_existingcenters[animal_name][
-                                index_in_existing
-                            ] = center
-                            self.animal_heights[animal_name][index_in_existing][
-                                frame_count_analyze
-                            ] = animal_heights[index_in_new]
-                            self.animal_other_contours[animal_name][
-                                index_in_existing
-                            ].append(animal_other_contours[index_in_new])
+                            self.animal_centers[animal_name][index_in_existing][frame_count_analyze] = center
+                            self.animal_existingcenters[animal_name][index_in_existing] = center
+                            self.animal_heights[animal_name][index_in_existing][frame_count_analyze] = animal_heights[
+                                index_in_new
+                            ]
+                            self.animal_other_contours[animal_name][index_in_existing].append(
+                                animal_other_contours[index_in_new]
+                            )
                             if self.animation_analyzer is True:
                                 blob = img_to_array(
                                     cv2.resize(
                                         animal_blobs[index_in_new],
                                         (self.dim_tconv, self.dim_tconv),
                                         interpolation=cv2.INTER_AREA,
                                     )
                                 )
-                                self.animal_blobs[animal_name][
-                                    index_in_existing
-                                ].append(blob)
-                                self.animations[animal_name][index_in_existing][
-                                    frame_count_analyze
-                                ] = np.array(
+                                self.animal_blobs[animal_name][index_in_existing].append(blob)
+                                self.animations[animal_name][index_in_existing][frame_count_analyze] = np.array(
                                     self.animal_blobs[animal_name][index_in_existing]
                                 )
                             if self.include_bodyparts is True:
-                                self.animal_inners[animal_name][
-                                    index_in_existing
-                                ].append(animal_inners[index_in_new])
-                                self.animal_other_inners[animal_name][
-                                    index_in_existing
-                                ].append(animal_other_inners[index_in_new])
+                                self.animal_inners[animal_name][index_in_existing].append(animal_inners[index_in_new])
+                                self.animal_other_inners[animal_name][index_in_existing].append(
+                                    animal_other_inners[index_in_new]
+                                )
                                 pattern_image = generate_patternimage_interact(
                                     self.background,
-                                    self.animal_contours[animal_name][
-                                        index_in_existing
-                                    ][
-                                        max(
-                                            0, (frame_count_analyze - self.length + 1)
-                                        ) : frame_count_analyze + 1
-                                    ],
-                                    self.animal_other_contours[animal_name][
-                                        index_in_existing
-                                    ],
-                                    inners=self.animal_inners[animal_name][
-                                        index_in_existing
-                                    ],
-                                    other_inners=self.animal_other_inners[animal_name][
-                                        index_in_existing
+                                    self.animal_contours[animal_name][index_in_existing][
+                                        max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                                     ],
+                                    self.animal_other_contours[animal_name][index_in_existing],
+                                    inners=self.animal_inners[animal_name][index_in_existing],
+                                    other_inners=self.animal_other_inners[animal_name][index_in_existing],
                                     std=self.std,
                                 )
                             else:
                                 pattern_image = generate_patternimage_interact(
                                     self.background,
-                                    self.animal_contours[animal_name][
-                                        index_in_existing
-                                    ][
-                                        max(
-                                            0, (frame_count_analyze - self.length + 1)
-                                        ) : frame_count_analyze + 1
-                                    ],
-                                    self.animal_other_contours[animal_name][
-                                        index_in_existing
+                                    self.animal_contours[animal_name][index_in_existing][
+                                        max(0, (frame_count_analyze - self.length + 1)) : frame_count_analyze + 1
                                     ],
+                                    self.animal_other_contours[animal_name][index_in_existing],
                                     inners=None,
                                     other_inners=None,
                                     std=0,
                                 )
                             pattern_image = cv2.resize(
                                 pattern_image,
                                 (self.dim_conv, self.dim_conv),
                                 interpolation=cv2.INTER_AREA,
                             )
-                            self.pattern_images[animal_name][index_in_existing][
-                                frame_count_analyze
-                            ] = np.array(pattern_image)
+                            self.pattern_images[animal_name][index_in_existing][frame_count_analyze] = np.array(
+                                pattern_image
+                            )
 
                 if len(unused_existing_indices) > 0:
                     for i in unused_existing_indices:
-                        if (
-                            self.to_deregister[animal_name][i]
-                            <= self.count_to_deregister
-                        ):
+                        if self.to_deregister[animal_name][i] <= self.count_to_deregister:
                             self.to_deregister[animal_name][i] += 1
                         else:
                             self.animal_existingcenters[animal_name][i] = (
                                 -10000,
                                 -10000,
                             )
                         self.animal_other_contours[animal_name][i].append([None])
@@ -810,35 +488,29 @@
         self,
         frames,
         batch_size,
         frame_count_analyze,
         background_free=True,
         animation=None,
     ):
-        tensor_frames = [
-            torch.as_tensor(frame.astype("float32").transpose(2, 0, 1))
-            for frame in frames
-        ]
+        tensor_frames = [torch.as_tensor(frame.astype("float32").transpose(2, 0, 1)) for frame in frames]
         inputs = [{"image": tensor_frame} for tensor_frame in tensor_frames]
 
-        with torch.no_grad():
-            outputs = self.detector(inputs)
+        outputs = self.detector(inputs)
 
         for batch_count, output in enumerate(outputs):
             frame = frames[batch_count]
             self.temp_frames.append(frame)
             instances = outputs[batch_count]["instances"].to("cpu")
             masks = instances.pred_masks.numpy().astype(np.uint8)
             classes = instances.pred_classes.numpy()
             scores = instances.scores.numpy()
 
             if len(masks) == 0:
-                self.skipped_frames.append(
-                    frame_count_analyze + 1 - batch_size + batch_count
-                )
+                self.skipped_frames.append(frame_count_analyze + 1 - batch_size + batch_count)
 
                 for animal_name in self.animal_kinds:
                     for i in self.animal_centers[animal_name]:
                         if self.animation_analyzer is True:
                             self.animal_blobs[animal_name][i].append(
                                 np.zeros(
                                     (self.dim_tconv, self.dim_tconv, self.channel),
@@ -849,51 +521,35 @@
                             self.animal_inners[animal_name][i].append(None)
 
             else:
                 mask_area = np.sum(np.array(masks), axis=(1, 2))
                 exclusion_mask = np.zeros(len(masks), dtype=bool)
                 exclusion_mask[
                     np.where(
-                        (
-                            np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3))
-                            / mask_area[:, None]
-                            > 0.8
-                        )
+                        (np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3)) / mask_area[:, None] > 0.8)
                         & (mask_area[:, None] < mask_area[None, :])
                     )[0]
                 ] = True
                 masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
-                classes = [
-                    c for c, exclude in zip(classes, exclusion_mask) if not exclude
-                ]
+                classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                 classes = [self.animal_mapping[str(x)] for x in classes]
-                scores = [
-                    s for s, exclude in zip(scores, exclusion_mask) if not exclude
-                ]
+                scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                 for animal_name in self.animal_kinds:
                     contours = []
                     centers = []
                     goodcontours = []
                     goodmasks = []
                     heights = []
                     inners = []
                     blobs = []
 
                     animal_number = int(self.animal_number[animal_name])
-                    animal_masks = [
-                        masks[a]
-                        for a, name in enumerate(classes)
-                        if name == animal_name
-                    ]
-                    animal_scores = [
-                        scores[a]
-                        for a, name in enumerate(classes)
-                        if name == animal_name
-                    ]
+                    animal_masks = [masks[a] for a, name in enumerate(classes) if name == animal_name]
+                    animal_scores = [scores[a] for a, name in enumerate(classes) if name == animal_name]
 
                     if len(animal_masks) == 0:
                         for i in self.animal_centers[animal_name]:
                             if self.animation_analyzer is True:
                                 self.animal_blobs[animal_name][i].append(
                                     np.zeros(
                                         (self.dim_tconv, self.dim_tconv, self.channel),
@@ -901,94 +557,68 @@
                                     )
                                 )
                             if self.include_bodyparts is True:
                                 self.animal_inners[animal_name][i].append(None)
 
                     else:
                         if len(animal_scores) > animal_number * 2:
-                            sorted_scores_indices = np.argsort(animal_scores)[
-                                -int(animal_number * 2) :
-                            ]
-                            animal_masks = [
-                                animal_masks[x] for x in sorted_scores_indices
-                            ]
+                            sorted_scores_indices = np.argsort(animal_scores)[-int(animal_number * 2) :]
+                            animal_masks = [animal_masks[x] for x in sorted_scores_indices]
                         for mask in animal_masks:
                             mask = cv2.morphologyEx(
                                 mask,
                                 cv2.MORPH_CLOSE,
                                 np.ones((self.kernel, self.kernel), np.uint8),
                             )
                             goodmasks.append(mask)
                             cnts, _ = cv2.findContours(
                                 (mask * 255).astype(np.uint8),
                                 cv2.RETR_EXTERNAL,
                                 cv2.CHAIN_APPROX_NONE,
                             )
-                            goodcontours.append(
-                                sorted(cnts, key=cv2.contourArea, reverse=True)[0]
-                            )
+                            goodcontours.append(sorted(cnts, key=cv2.contourArea, reverse=True)[0])
                         areas = [cv2.contourArea(ct) for ct in goodcontours]
-                        sorted_area_indices = np.argsort(np.array(areas))[
-                            -animal_number:
-                        ]
+                        sorted_area_indices = np.argsort(np.array(areas))[-animal_number:]
                         areas_sorted = sorted(areas)[-animal_number:]
                         area = sum(areas_sorted) / len(areas_sorted)
                         if self.animal_area[animal_name] is None:
                             self.animal_area[animal_name] = area
                         else:
-                            self.animal_area[animal_name] = (
-                                self.animal_area[animal_name] + area
-                            ) / 2
+                            self.animal_area[animal_name] = (self.animal_area[animal_name] + area) / 2
                         for x in sorted_area_indices:
                             mask = goodmasks[x]
                             cnt = goodcontours[x]
                             contours.append(cnt)
                             centers.append(
                                 (
-                                    int(
-                                        cv2.moments(cnt)["m10"]
-                                        / cv2.moments(cnt)["m00"]
-                                    ),
-                                    int(
-                                        cv2.moments(cnt)["m01"]
-                                        / cv2.moments(cnt)["m00"]
-                                    ),
+                                    int(cv2.moments(cnt)["m10"] / cv2.moments(cnt)["m00"]),
+                                    int(cv2.moments(cnt)["m01"] / cv2.moments(cnt)["m00"]),
                                 )
                             )
                             (_, _), (w, h), _ = cv2.minAreaRect(cnt)
                             heights.append(max(w, h))
                             if self.include_bodyparts is True:
-                                masked_frame = (
-                                    cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
-                                )
+                                masked_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
                                 inners.append(get_inner(masked_frame, cnt))
                             if self.animation_analyzer is True:
-                                masked_frame = frame * cv2.cvtColor(
-                                    mask, cv2.COLOR_GRAY2BGR
-                                )
+                                masked_frame = frame * cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
                                 x, y, w, h = cv2.boundingRect(cnt)
                                 difference = int(abs(w - h) / 2) + 1
                                 if w > h:
                                     y_bt = max(y - difference - 1, 0)
-                                    y_tp = min(
-                                        y + h + difference + 1, self.background.shape[0]
-                                    )
+                                    y_tp = min(y + h + difference + 1, self.background.shape[0])
                                     x_lf = max(x - 1, 0)
                                     x_rt = min(x + w + 1, self.background.shape[1])
                                 else:
                                     y_bt = max(y - 1, 0)
                                     y_tp = min(y + h + 1, self.background.shape[0])
                                     x_lf = max(x - difference - 1, 0)
-                                    x_rt = min(
-                                        x + w + difference + 1, self.background.shape[1]
-                                    )
+                                    x_rt = min(x + w + difference + 1, self.background.shape[1])
                                 blob = masked_frame[y_bt:y_tp, x_lf:x_rt]
-                                blob = np.uint8(
-                                    exposure.rescale_intensity(blob, out_range=(0, 255))
-                                )
+                                blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                                 if self.channel == 1:
                                     blob = cv2.cvtColor(blob, cv2.COLOR_BGR2GRAY)
                                     blob = img_to_array(blob)
                                 blobs.append(blob)
 
                         self.track_animal(
                             frame_count_analyze + 1 - batch_size + batch_count,
@@ -1010,19 +640,15 @@
                                                     0,
                                                     frame_count_analyze
                                                     + 1
                                                     - batch_size
                                                     + batch_count
                                                     - self.length
                                                     + 1,
-                                                ) : frame_count_analyze
-                                                + 1
-                                                - batch_size
-                                                + batch_count
-                                                + 1
+                                                ) : frame_count_analyze + 1 - batch_size + batch_count + 1
                                             ][n]
                                             is None
                                         ):
                                             blob = np.zeros(
                                                 (
                                                     self.dim_tconv,
                                                     self.dim_tconv,
@@ -1038,60 +664,45 @@
                                                         0,
                                                         frame_count_analyze
                                                         + 1
                                                         - batch_size
                                                         + batch_count
                                                         - self.length
                                                         + 1,
-                                                    ) : frame_count_analyze
-                                                    + 1
-                                                    - batch_size
-                                                    + batch_count
-                                                    + 1
+                                                    ) : frame_count_analyze + 1 - batch_size + batch_count + 1
                                                 ],
                                                 contour=None,
                                                 channel=self.channel,
                                                 background_free=False,
                                             )
                                             blob = cv2.resize(
                                                 blob,
                                                 (self.dim_tconv, self.dim_tconv),
                                                 interpolation=cv2.INTER_AREA,
                                             )
                                         animation.append(img_to_array(blob))
                                     self.animations[animal_name][i][
-                                        frame_count_analyze
-                                        + 1
-                                        - batch_size
-                                        + batch_count
+                                        frame_count_analyze + 1 - batch_size + batch_count
                                     ] = np.array(animation)
 
-    def detect_track_interact(
-        self, frames, batch_size, frame_count_analyze, background_free=True
-    ):
-        tensor_frames = [
-            torch.as_tensor(frame.astype("float32").transpose(2, 0, 1))
-            for frame in frames
-        ]
+    def detect_track_interact(self, frames, batch_size, frame_count_analyze, background_free=True):
+        tensor_frames = [torch.as_tensor(frame.astype("float32").transpose(2, 0, 1)) for frame in frames]
         inputs = [{"image": tensor_frame} for tensor_frame in tensor_frames]
 
-        with torch.no_grad():
-            outputs = self.detector(inputs)
+        outputs = self.detector(inputs)
 
         for batch_count, output in enumerate(outputs):
             frame = frames[batch_count]
             instances = outputs[batch_count]["instances"].to("cpu")
             masks = instances.pred_masks.numpy().astype(np.uint8)
             classes = instances.pred_classes.numpy()
             scores = instances.scores.numpy()
 
             if len(masks) == 0:
-                self.skipped_frames.append(
-                    frame_count_analyze + 1 - batch_size + batch_count
-                )
+                self.skipped_frames.append(frame_count_analyze + 1 - batch_size + batch_count)
 
                 for animal_name in self.animal_kinds:
                     self.animal_present[animal_name] = 0
                     for i in self.animal_centers[animal_name]:
                         self.animal_other_contours[animal_name][i].append([None])
                         if self.animation_analyzer is True:
                             self.animal_blobs[animal_name][i].append(
@@ -1105,53 +716,37 @@
                             self.animal_other_inners[animal_name][i].append([None])
 
             else:
                 mask_area = np.sum(np.array(masks), axis=(1, 2))
                 exclusion_mask = np.zeros(len(masks), dtype=bool)
                 exclusion_mask[
                     np.where(
-                        (
-                            np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3))
-                            / mask_area[:, None]
-                            > 0.8
-                        )
+                        (np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3)) / mask_area[:, None] > 0.8)
                         & (mask_area[:, None] < mask_area[None, :])
                     )[0]
                 ] = True
                 masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
-                classes = [
-                    c for c, exclude in zip(classes, exclusion_mask) if not exclude
-                ]
+                classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                 classes = [self.animal_mapping[str(x)] for x in classes]
-                scores = [
-                    s for s, exclude in zip(scores, exclusion_mask) if not exclude
-                ]
+                scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                 all_centers = []
                 all_masks = []
                 all_contours = []
                 all_inners = []
                 all_heights = []
                 all_blobs = []
                 average_area = []
 
                 for animal_name in self.animal_kinds:
                     goodmasks = []
                     goodcontours = []
                     animal_number = int(self.animal_number[animal_name])
-                    animal_masks = [
-                        masks[a]
-                        for a, name in enumerate(classes)
-                        if name == animal_name
-                    ]
-                    animal_scores = [
-                        scores[a]
-                        for a, name in enumerate(classes)
-                        if name == animal_name
-                    ]
+                    animal_masks = [masks[a] for a, name in enumerate(classes) if name == animal_name]
+                    animal_scores = [scores[a] for a, name in enumerate(classes) if name == animal_name]
 
                     if len(animal_masks) == 0:
                         self.animal_present[animal_name] = 0
                         for i in self.animal_centers[animal_name]:
                             self.animal_other_contours[animal_name][i].append([None])
                             if self.animation_analyzer is True:
                                 self.animal_blobs[animal_name][i].append(
@@ -1161,145 +756,96 @@
                                     )
                                 )
                             if self.include_bodyparts is True:
                                 self.animal_inners[animal_name][i].append(None)
                                 self.animal_other_inners[animal_name][i].append([None])
                     else:
                         if len(animal_scores) > animal_number * 2:
-                            sorted_scores_indices = np.argsort(animal_scores)[
-                                -int(animal_number * 2) :
-                            ]
-                            animal_masks = [
-                                animal_masks[x] for x in sorted_scores_indices
-                            ]
+                            sorted_scores_indices = np.argsort(animal_scores)[-int(animal_number * 2) :]
+                            animal_masks = [animal_masks[x] for x in sorted_scores_indices]
                         for mask in animal_masks:
                             mask = cv2.morphologyEx(
                                 mask,
                                 cv2.MORPH_CLOSE,
                                 np.ones((self.kernel, self.kernel), np.uint8),
                             )
                             goodmasks.append(mask)
                             cnts, _ = cv2.findContours(
                                 (mask * 255).astype(np.uint8),
                                 cv2.RETR_EXTERNAL,
                                 cv2.CHAIN_APPROX_NONE,
                             )
-                            goodcontours.append(
-                                sorted(cnts, key=cv2.contourArea, reverse=True)[0]
-                            )
+                            goodcontours.append(sorted(cnts, key=cv2.contourArea, reverse=True)[0])
                         areas = [cv2.contourArea(ct) for ct in goodcontours]
-                        sorted_area_indices = np.argsort(np.array(areas))[
-                            -animal_number:
-                        ]
+                        sorted_area_indices = np.argsort(np.array(areas))[-animal_number:]
                         self.animal_present[animal_name] = len(sorted_area_indices)
                         areas_sorted = sorted(areas)[-animal_number:]
                         area = sum(areas_sorted) / len(areas_sorted)
                         if self.animal_area[animal_name] is None:
                             self.animal_area[animal_name] = area
                         else:
-                            self.animal_area[animal_name] = (
-                                self.animal_area[animal_name] + area
-                            ) / 2
+                            self.animal_area[animal_name] = (self.animal_area[animal_name] + area) / 2
                         average_area.append(self.animal_area[animal_name])
                         for x in sorted_area_indices:
                             mask = goodmasks[x]
                             all_masks.append(mask)
                             cnt = goodcontours[x]
                             all_contours.append(cnt)
                             all_centers.append(
                                 (
-                                    int(
-                                        cv2.moments(cnt)["m10"]
-                                        / cv2.moments(cnt)["m00"]
-                                    ),
-                                    int(
-                                        cv2.moments(cnt)["m01"]
-                                        / cv2.moments(cnt)["m00"]
-                                    ),
+                                    int(cv2.moments(cnt)["m10"] / cv2.moments(cnt)["m00"]),
+                                    int(cv2.moments(cnt)["m01"] / cv2.moments(cnt)["m00"]),
                                 )
                             )
                             (_, _), (w, h), _ = cv2.minAreaRect(cnt)
                             all_heights.append(max(w, h))
                             if self.include_bodyparts is True:
-                                masked_frame = (
-                                    cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
-                                )
+                                masked_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
                                 all_inners.append(get_inner(masked_frame, cnt))
 
                 if len(all_centers) > 1:
                     centers_array = np.array(all_centers)
-                    distances_squared = np.sum(
-                        (centers_array[:, None] - centers_array) ** 2, axis=2
-                    )
+                    distances_squared = np.sum((centers_array[:, None] - centers_array) ** 2, axis=2)
                     determine = np.logical_and(
                         distances_squared > 0,
                         distances_squared
-                        < (
-                            math.sqrt(sum(average_area) / len(average_area))
-                            * self.social_distance
-                        )
-                        ** 2,
+                        < (math.sqrt(sum(average_area) / len(average_area)) * self.social_distance) ** 2,
                     )
                     other_contours = [
-                        [
-                            all_contours[x]
-                            for x, determ in enumerate(determine[y])
-                            if determ
-                        ]
+                        [all_contours[x] for x, determ in enumerate(determine[y]) if determ]
                         for y, c in enumerate(all_centers)
                     ]
                     if self.include_bodyparts is True:
                         other_inners = [
-                            [
-                                all_inners[x]
-                                for x, determ in enumerate(determine[y])
-                                if determ
-                            ]
+                            [all_inners[x] for x, determ in enumerate(determine[y]) if determ]
                             for y, c in enumerate(all_centers)
                         ]
                     else:
                         other_inners = None
                     if self.animation_analyzer is True:
                         other_masks = [
-                            np.bitwise_or.reduce(
-                                np.stack(np.array(all_masks)[determine[x]])
-                            )
-                            if len(c) > 0
-                            else None
+                            np.bitwise_or.reduce(np.stack(np.array(all_masks)[determine[x]])) if len(c) > 0 else None
                             for x, c in enumerate(other_contours)
                         ]
                         for i, other_mask in enumerate(other_masks):
                             contour = all_contours[i]
                             total_contours = other_contours[i]
                             total_contours.append(contour)
-                            (y_bt, y_tp, x_lf, x_rt) = crop_frame(
-                                self.background, total_contours
-                            )
+                            (y_bt, y_tp, x_lf, x_rt) = crop_frame(self.background, total_contours)
                             if background_free is True:
-                                blob = frame * cv2.cvtColor(
-                                    all_masks[i], cv2.COLOR_GRAY2BGR
-                                )
+                                blob = frame * cv2.cvtColor(all_masks[i], cv2.COLOR_GRAY2BGR)
                                 if other_mask is not None:
                                     other_blob = cv2.cvtColor(
-                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-                                        * other_mask,
+                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * other_mask,
                                         cv2.COLOR_GRAY2BGR,
                                     )
                                     blob = cv2.add(blob, other_blob)
-                                    blob = np.uint8(
-                                        exposure.rescale_intensity(
-                                            blob, out_range=(0, 255)
-                                        )
-                                    )
+                                    blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                             else:
-                                blob = np.uint8(
-                                    exposure.rescale_intensity(
-                                        frame, out_range=(0, 255)
-                                    )
-                                )
+                                blob = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
                             cv2.drawContours(blob, [contour], 0, (255, 0, 255), 2)
                             all_blobs.append(blob[y_bt:y_tp, x_lf:x_rt])
 
                     self.track_animal_interact(
                         frame_count_analyze + 1 - batch_size + batch_count,
                         all_contours,
                         other_contours,
@@ -1314,24 +860,18 @@
                     if len(all_centers) > 0:
                         other_contours = [[None]]
                         if self.include_bodyparts is True:
                             other_inners = [[None]]
                         else:
                             other_inners = None
                         if background_free is True:
-                            blob = frame * cv2.cvtColor(
-                                all_masks[0], cv2.COLOR_GRAY2BGR
-                            )
-                            blob = np.uint8(
-                                exposure.rescale_intensity(blob, out_range=(0, 255))
-                            )
+                            blob = frame * cv2.cvtColor(all_masks[0], cv2.COLOR_GRAY2BGR)
+                            blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                         else:
-                            blob = np.uint8(
-                                exposure.rescale_intensity(frame, out_range=(0, 255))
-                            )
+                            blob = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
                         contour = all_contours[0]
                         cv2.drawContours(blob, [contour], 0, (255, 0, 255), 2)
                         x, y, w, h = cv2.boundingRect(contour)
                         difference = int(abs(w - h) / 2) + 1
                         if w > h:
                             y_bt = max(y - difference - 1, 0)
                             y_tp = min(y + h + difference + 1, self.background.shape[0])
@@ -1361,19 +901,15 @@
         print(datetime.datetime.now())
 
         capture = cv2.VideoCapture(self.path_to_video)
         batch = []
         batch_count = frame_count = frame_count_analyze = 0
         animation = (
             deque(
-                [
-                    np.zeros(
-                        (self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8"
-                    )
-                ],
+                [np.zeros((self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8")],
                 maxlen=self.length,
             )
             * self.length
         )
 
         start_t = round((self.t - self.length / self.fps), 2)
         if start_t < 0:
@@ -1429,21 +965,15 @@
                 frame_count_analyze += 1
 
             frame_count += 1
 
         capture.release()
 
         for animal_name in self.animal_kinds:
-            print(
-                "The area of "
-                + str(animal_name)
-                + " is: "
-                + str(self.animal_area[animal_name])
-                + "."
-            )
+            print("The area of " + str(animal_name) + " is: " + str(self.animal_area[animal_name]) + ".")
 
         print("Information acquisition completed!")
 
     def acquire_information_interact_basic(self, batch_size=1, background_free=True):
         print("Acquiring information in each frame...")
         print(datetime.datetime.now())
 
@@ -1473,19 +1003,15 @@
         capture = cv2.VideoCapture(self.path_to_video)
         batch = []
         batch_count = frame_count = frame_count_analyze = 0
         temp_contours = deque(maxlen=self.length)
         temp_inners = deque(maxlen=self.length)
         animation = (
             deque(
-                [
-                    np.zeros(
-                        (self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8"
-                    )
-                ],
+                [np.zeros((self.dim_tconv, self.dim_tconv, self.channel), dtype="uint8")],
                 maxlen=self.length,
             )
             * self.length
         )
 
         start_t = round((self.t - self.length / self.fps), 2)
         if start_t < 0:
@@ -1518,49 +1044,41 @@
 
                 batch.append(frame)
                 batch_count += 1
 
                 if batch_count == batch_size:
                     batch_count = 0
 
-                    tensor_frames = [
-                        torch.as_tensor(frame.astype("float32").transpose(2, 0, 1))
-                        for frame in batch
-                    ]
+                    tensor_frames = [torch.as_tensor(frame.astype("float32").transpose(2, 0, 1)) for frame in batch]
                     inputs = [{"image": tensor_frame} for tensor_frame in tensor_frames]
 
-                    with torch.no_grad():
-                        outputs = self.detector(inputs)
+                    outputs = self.detector(inputs)
 
                     for batch_count, output in enumerate(outputs):
                         frame = batch[batch_count]
                         self.temp_frames.append(frame)
                         instances = outputs[batch_count]["instances"].to("cpu")
                         masks = instances.pred_masks.numpy().astype(np.uint8)
                         classes = instances.pred_classes.numpy()
                         scores = instances.scores.numpy()
 
                         if len(masks) == 0:
-                            self.skipped_frames.append(
-                                frame_count_analyze + 1 - batch_size + batch_count
-                            )
+                            self.skipped_frames.append(frame_count_analyze + 1 - batch_size + batch_count)
 
                             temp_contours.append(None)
                             temp_inners.append(None)
                             animation.append(
                                 np.zeros(
                                     (self.dim_tconv, self.dim_tconv, self.channel),
                                     dtype="uint8",
                                 )
                             )
 
                         else:
-                            self.register_counts[name][0] = (
-                                frame_count_analyze + 1 - batch_size + batch_count
-                            )
+                            self.register_counts[name][0] = frame_count_analyze + 1 - batch_size + batch_count
 
                             mask_area = np.sum(np.array(masks), axis=(1, 2))
                             exclusion_mask = np.zeros(len(masks), dtype=bool)
                             exclusion_mask[
                                 np.where(
                                     (
                                         np.sum(
@@ -1569,142 +1087,94 @@
                                         )
                                         / mask_area[:, None]
                                         > 0.8
                                     )
                                     & (mask_area[:, None] < mask_area[None, :])
                                 )[0]
                             ] = True
-                            masks = [
-                                m
-                                for m, exclude in zip(masks, exclusion_mask)
-                                if not exclude
-                            ]
-                            classes = [
-                                c
-                                for c, exclude in zip(classes, exclusion_mask)
-                                if not exclude
-                            ]
+                            masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
+                            classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                             classes = [self.animal_mapping[str(x)] for x in classes]
-                            scores = [
-                                s
-                                for s, exclude in zip(scores, exclusion_mask)
-                                if not exclude
-                            ]
+                            scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                             contours = []
                             inners = []
 
                             for animal_name in self.animal_kinds:
                                 goodcontours = []
                                 goodmasks = []
                                 animal_number = int(self.animal_number[animal_name])
-                                animal_masks = [
-                                    masks[a]
-                                    for a, n in enumerate(classes)
-                                    if n == animal_name
-                                ]
-                                animal_scores = [
-                                    scores[a]
-                                    for a, n in enumerate(classes)
-                                    if n == animal_name
-                                ]
+                                animal_masks = [masks[a] for a, n in enumerate(classes) if n == animal_name]
+                                animal_scores = [scores[a] for a, n in enumerate(classes) if n == animal_name]
                                 if len(animal_masks) > 0:
                                     if len(animal_scores) > animal_number * 2:
-                                        sorted_scores_indices = np.argsort(
-                                            animal_scores
-                                        )[-int(animal_number * 2) :]
-                                        animal_masks = [
-                                            animal_masks[x]
-                                            for x in sorted_scores_indices
-                                        ]
+                                        sorted_scores_indices = np.argsort(animal_scores)[-int(animal_number * 2) :]
+                                        animal_masks = [animal_masks[x] for x in sorted_scores_indices]
                                     for mask in animal_masks:
                                         mask = cv2.morphologyEx(
                                             mask,
                                             cv2.MORPH_CLOSE,
-                                            np.ones(
-                                                (self.kernel, self.kernel), np.uint8
-                                            ),
+                                            np.ones((self.kernel, self.kernel), np.uint8),
                                         )
                                         cnts, _ = cv2.findContours(
                                             (mask * 255).astype(np.uint8),
                                             cv2.RETR_EXTERNAL,
                                             cv2.CHAIN_APPROX_NONE,
                                         )
-                                        goodcontours.append(
-                                            sorted(
-                                                cnts, key=cv2.contourArea, reverse=True
-                                            )[0]
-                                        )
+                                        goodcontours.append(sorted(cnts, key=cv2.contourArea, reverse=True)[0])
                                         goodmasks.append(mask)
                                     areas = [cv2.contourArea(ct) for ct in goodcontours]
-                                    sorted_area_indices = np.argsort(np.array(areas))[
-                                        -animal_number:
-                                    ]
+                                    sorted_area_indices = np.argsort(np.array(areas))[-animal_number:]
                                     for x in sorted_area_indices:
                                         cnt = goodcontours[x]
                                         mask = goodmasks[x]
                                         contours.append(cnt)
                                         if self.include_bodyparts is True:
-                                            masked_frame = (
-                                                cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-                                                * mask
-                                            )
+                                            masked_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
                                             inners.append(get_inner(masked_frame, cnt))
 
-                            self.animal_contours[name][0][
-                                frame_count_analyze + 1 - batch_size + batch_count
-                            ] = contours
+                            self.animal_contours[name][0][frame_count_analyze + 1 - batch_size + batch_count] = contours
 
                             temp_contours.append(contours)
                             temp_inners.append(inners)
                             (y_bt, y_tp, x_lf, x_rt) = crop_frame(
                                 frame,
                                 functools.reduce(operator.iconcat, temp_contours, []),
                             )
 
-                            self.animal_centers[name][0][
-                                frame_count_analyze + 1 - batch_size + batch_count
-                            ] = (x_lf + 20, y_bt + 10)
+                            self.animal_centers[name][0][frame_count_analyze + 1 - batch_size + batch_count] = (
+                                x_lf + 20,
+                                y_bt + 10,
+                            )
 
                             pattern_image = generate_patternimage_all(
                                 frame,
                                 y_bt,
                                 y_tp,
                                 x_lf,
                                 x_rt,
                                 temp_contours,
                                 temp_inners,
                                 std=self.std,
                             )
-                            self.pattern_images[name][0][
-                                frame_count_analyze + 1 - batch_size + batch_count
-                            ] = np.array(
+                            self.pattern_images[name][0][frame_count_analyze + 1 - batch_size + batch_count] = np.array(
                                 cv2.resize(
                                     pattern_image,
                                     (self.dim_conv, self.dim_conv),
                                     interpolation=cv2.INTER_AREA,
                                 )
                             )
                             if self.animation_analyzer is True:
                                 for i, f in enumerate(self.temp_frames):
                                     if (
                                         self.animal_contours[name][0][
                                             max(
                                                 0,
-                                                frame_count_analyze
-                                                + 1
-                                                - batch_size
-                                                + batch_count
-                                                - self.length
-                                                + 1,
-                                            ) : frame_count_analyze
-                                            + 1
-                                            - batch_size
-                                            + batch_count
-                                            + 1
+                                                frame_count_analyze + 1 - batch_size + batch_count - self.length + 1,
+                                            ) : frame_count_analyze + 1 - batch_size + batch_count + 1
                                         ][i]
                                         is None
                                     ):
                                         blob = np.zeros(
                                             (
                                                 self.dim_tconv,
                                                 self.dim_tconv,
@@ -1725,20 +1195,17 @@
                                         )
                                         blob = cv2.resize(
                                             blob,
                                             (self.dim_tconv, self.dim_tconv),
                                             interpolation=cv2.INTER_AREA,
                                         )
                                     animation.append(img_to_array(blob))
-                                    self.animations[name][0][
-                                        frame_count_analyze
-                                        + 1
-                                        - batch_size
-                                        + batch_count
-                                    ] = np.array(animation)
+                                    self.animations[name][0][frame_count_analyze + 1 - batch_size + batch_count] = (
+                                        np.array(animation)
+                                    )
 
                     batch = []
 
                 frame_count_analyze += 1
 
             frame_count += 1
 
@@ -1790,30 +1257,20 @@
                             del self.animal_other_inners[animal_name][i]
                     if self.animation_analyzer is True:
                         del self.animal_blobs[animal_name][i]
                         del self.animations[animal_name][i]
                     del self.pattern_images[animal_name][i]
 
             for i in self.animal_centers[animal_name]:
-                self.animal_centers[animal_name][i] = self.animal_centers[animal_name][
-                    i
-                ][:length]
-                self.animal_contours[animal_name][i] = self.animal_contours[
-                    animal_name
-                ][i][:length]
-                self.animal_heights[animal_name][i] = self.animal_heights[animal_name][
-                    i
-                ][:length]
+                self.animal_centers[animal_name][i] = self.animal_centers[animal_name][i][:length]
+                self.animal_contours[animal_name][i] = self.animal_contours[animal_name][i][:length]
+                self.animal_heights[animal_name][i] = self.animal_heights[animal_name][i][:length]
                 if self.animation_analyzer is True:
-                    self.animations[animal_name][i] = self.animations[animal_name][i][
-                        :length
-                    ]
-                self.pattern_images[animal_name][i] = self.pattern_images[animal_name][
-                    i
-                ][:length]
+                    self.animations[animal_name][i] = self.animations[animal_name][i][:length]
+                self.pattern_images[animal_name][i] = self.pattern_images[animal_name][i][:length]
 
         print("Data crafting completed!")
 
     def categorize_behaviors(self, path_to_categorizer, uncertain=0):
         print("Categorizing behaviors...")
         print(datetime.datetime.now())
 
@@ -1838,83 +1295,70 @@
             if self.animation_analyzer is True:
                 del self.animations[animal_name]
             del self.pattern_images[animal_name]
             gc.collect()
 
             with tf.device("CPU"):
                 if self.animation_analyzer is True:
-                    animations = tf.convert_to_tensor(
-                        np.array(animations, dtype="float32") / 255.0
-                    )
-                pattern_images = tf.convert_to_tensor(
-                    np.array(pattern_images, dtype="float32") / 255.0
-                )
+                    animations = tf.convert_to_tensor(np.array(animations, dtype="float32") / 255.0)
+                pattern_images = tf.convert_to_tensor(np.array(pattern_images, dtype="float32") / 255.0)
 
             if self.animation_analyzer is True:
                 inputs = [animations, pattern_images]
             else:
                 inputs = pattern_images
 
             predictions = categorizer.predict(inputs, batch_size=32)
 
             for behavior_name in self.all_behavior_parameters[animal_name]:
                 for i in IDs:
-                    self.all_behavior_parameters[animal_name][behavior_name][
-                        "probability"
-                    ][i] = [np.nan] * len(self.all_time)
-                    self.event_probability[animal_name][i] = [["NA", -1]] * len(
+                    self.all_behavior_parameters[animal_name][behavior_name]["probability"][i] = [np.nan] * len(
                         self.all_time
                     )
+                    self.event_probability[animal_name][i] = [["NA", -1]] * len(self.all_time)
 
             idx = 0
             for n in IDs:
                 i = self.length + self.register_counts[animal_name][n]
                 idx += i
                 while i < len(self.animal_contours[animal_name][n]):
                     if self.animal_contours[animal_name][n][i] is not None:
                         check = 0
-                        for c in self.animal_contours[animal_name][n][
-                            i - self.length + 1 : i + 1
-                        ]:
+                        for c in self.animal_contours[animal_name][n][i - self.length + 1 : i + 1]:
                             if c is None:
                                 check += 1
                         if check <= self.length / 2:
                             prediction = predictions[idx]
-                            behavior_names = list(
-                                self.all_behavior_parameters[animal_name].keys()
-                            )
+                            behavior_names = list(self.all_behavior_parameters[animal_name].keys())
                             for name_index, behavior_name in enumerate(behavior_names):
                                 if len(behavior_names) == 2:
                                     if name_index == 0:
                                         probability = 1 - prediction[0]
                                     else:
                                         probability = prediction[0]
                                 else:
                                     probability = prediction[name_index]
-                                self.all_behavior_parameters[animal_name][
-                                    behavior_name
-                                ]["probability"][n][i] = probability
+                                self.all_behavior_parameters[animal_name][behavior_name]["probability"][n][i] = (
+                                    probability
+                                )
                             if len(behavior_names) == 2:
                                 if prediction[0] > 0.5:
                                     if prediction[0] - (1 - prediction[0]) > uncertain:
                                         self.event_probability[animal_name][n][i] = [
                                             behavior_names[1],
                                             prediction[0],
                                         ]
                                 if prediction[0] < 0.5:
                                     if (1 - prediction[0]) - prediction[0] > uncertain:
                                         self.event_probability[animal_name][n][i] = [
                                             behavior_names[0],
                                             1 - prediction[0],
                                         ]
                             else:
-                                if (
-                                    sorted(prediction)[-1] - sorted(prediction)[-2]
-                                    > uncertain
-                                ):
+                                if sorted(prediction)[-1] - sorted(prediction)[-2] > uncertain:
                                     self.event_probability[animal_name][n][i] = [
                                         behavior_names[np.argmax(prediction)],
                                         max(prediction),
                                     ]
 
                     idx += 1
                     i += 1
@@ -1936,85 +1380,64 @@
                         if behavior_name in specific_behaviors[animal_name]:
                             if specific_behaviors[animal_name][behavior_name] is None:
                                 specific_behaviors[animal_name][behavior_name] = i
                             else:
                                 ID = specific_behaviors[animal_name][behavior_name]
                                 if ID != i:
                                     temp = self.register_counts[animal_name][ID]
-                                    self.register_counts[animal_name][ID] = (
-                                        self.register_counts[animal_name][i]
-                                    )
+                                    self.register_counts[animal_name][ID] = self.register_counts[animal_name][i]
                                     self.register_counts[animal_name][i] = temp
                                     temp = self.animal_centers[animal_name][ID][idx]
-                                    self.animal_centers[animal_name][ID][idx] = (
-                                        self.animal_centers[animal_name][i][idx]
-                                    )
+                                    self.animal_centers[animal_name][ID][idx] = self.animal_centers[animal_name][i][idx]
                                     self.animal_centers[animal_name][i][idx] = temp
                                     temp = self.animal_contours[animal_name][ID][idx]
-                                    self.animal_contours[animal_name][ID][idx] = (
-                                        self.animal_contours[animal_name][i][idx]
-                                    )
+                                    self.animal_contours[animal_name][ID][idx] = self.animal_contours[animal_name][i][
+                                        idx
+                                    ]
                                     self.animal_contours[animal_name][i][idx] = temp
                                     temp = self.animal_heights[animal_name][ID][idx]
-                                    self.animal_heights[animal_name][ID][idx] = (
-                                        self.animal_heights[animal_name][i][idx]
-                                    )
+                                    self.animal_heights[animal_name][ID][idx] = self.animal_heights[animal_name][i][idx]
                                     self.animal_heights[animal_name][i][idx] = temp
                                     temp = self.event_probability[animal_name][ID][idx]
-                                    self.event_probability[animal_name][ID][idx] = (
-                                        self.event_probability[animal_name][i][idx]
-                                    )
+                                    self.event_probability[animal_name][ID][idx] = self.event_probability[animal_name][
+                                        i
+                                    ][idx]
                                     self.event_probability[animal_name][i][idx] = temp
-                                    temp = self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["probability"][ID][idx]
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["probability"][ID][
+                                    temp = self.all_behavior_parameters[animal_name][behavior_name]["probability"][ID][
                                         idx
-                                    ] = self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["probability"][i][idx]
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["probability"][i][idx] = temp
+                                    ]
+                                    self.all_behavior_parameters[animal_name][behavior_name]["probability"][ID][idx] = (
+                                        self.all_behavior_parameters[animal_name][behavior_name]["probability"][i][idx]
+                                    )
+                                    self.all_behavior_parameters[animal_name][behavior_name]["probability"][i][idx] = (
+                                        temp
+                                    )
 
         print("Identity correction completed!")
 
     def annotate_video(self, animal_to_include, behavior_to_include, show_legend=True):
         print("Annotating video...")
         print(datetime.datetime.now())
 
-        text_scl = max(
-            min(self.background.shape[0], self.background.shape[1]) / 960, 0.5
-        )
-        text_tk = max(
-            1, int(min(self.background.shape[0], self.background.shape[1]) / 960)
-        )
+        text_scl = 1
+        text_tk = 2
 
         if self.categorize_behavior is True:
             colors = {}
             for behavior_name in self.all_behavior_parameters[self.animal_kinds[0]]:
-                if (
-                    self.all_behavior_parameters[self.animal_kinds[0]][behavior_name][
-                        "color"
-                    ][1][0]
-                    != "#"
-                ):
+                if self.all_behavior_parameters[self.animal_kinds[0]][behavior_name]["color"][1][0] != "#":
                     colors[behavior_name] = (255, 255, 255)
                 else:
-                    hex_color = self.all_behavior_parameters[self.animal_kinds[0]][
-                        behavior_name
-                    ]["color"][1].lstrip("#")
+                    hex_color = self.all_behavior_parameters[self.animal_kinds[0]][behavior_name]["color"][1].lstrip(
+                        "#"
+                    )
                     color = tuple(int(hex_color[i : i + 2], 16) for i in (0, 2, 4))
                     colors[behavior_name] = color[::-1]
 
-            if len(behavior_to_include) != len(
-                self.all_behavior_parameters[self.animal_kinds[0]]
-            ):
+            if len(behavior_to_include) != len(self.all_behavior_parameters[self.animal_kinds[0]]):
                 for behavior_name in self.all_behavior_parameters[self.animal_kinds[0]]:
                     if behavior_name not in behavior_to_include:
                         del colors[behavior_name]
 
             if show_legend is True:
                 scl = self.background.shape[0] / 1024
                 if 25 * (len(colors) + 1) < self.background.shape[0]:
@@ -2063,29 +1486,18 @@
                                 text_tk,
                             )
                             n += 1
 
                 if frame_count_analyze not in self.skipped_frames:
                     for animal_name in animal_to_include:
                         for i in self.animal_contours[animal_name]:
-                            if frame_count_analyze < len(
-                                self.animal_contours[animal_name][i]
-                            ):
-                                if (
-                                    self.animal_contours[animal_name][i][
-                                        frame_count_analyze
-                                    ]
-                                    is not None
-                                ):
-                                    cx = self.animal_centers[animal_name][i][
-                                        frame_count_analyze
-                                    ][0]
-                                    cy = self.animal_centers[animal_name][i][
-                                        frame_count_analyze
-                                    ][1]
+                            if frame_count_analyze < len(self.animal_contours[animal_name][i]):
+                                if self.animal_contours[animal_name][i][frame_count_analyze] is not None:
+                                    cx = self.animal_centers[animal_name][i][frame_count_analyze][0]
+                                    cy = self.animal_centers[animal_name][i][frame_count_analyze][1]
 
                                     if self.behavior_mode != 1:
                                         cv2.circle(
                                             frame,
                                             (cx, cy),
                                             int(text_tk * 3),
                                             (255, 0, 0),
@@ -2099,90 +1511,67 @@
                                                 animal_name + " " + str(i),
                                                 (cx - 10, cy - 25),
                                                 cv2.FONT_HERSHEY_SIMPLEX,
                                                 text_scl,
                                                 (255, 255, 255),
                                                 text_tk,
                                             )
-                                        if (
-                                            self.event_probability[animal_name][i][
-                                                frame_count_analyze
-                                            ][0]
-                                            == "NA"
-                                        ):
+                                        if self.event_probability[animal_name][i][frame_count_analyze][0] == "NA":
                                             if self.behavior_mode == 1:
                                                 cv2.drawContours(
                                                     frame,
-                                                    self.animal_contours[animal_name][
-                                                        i
-                                                    ][frame_count_analyze],
+                                                    self.animal_contours[animal_name][i][frame_count_analyze],
                                                     -1,
                                                     (255, 255, 255),
                                                     1,
                                                 )
                                             else:
                                                 cv2.drawContours(
                                                     frame,
-                                                    [
-                                                        self.animal_contours[
-                                                            animal_name
-                                                        ][i][frame_count_analyze]
-                                                    ],
+                                                    [self.animal_contours[animal_name][i][frame_count_analyze]],
                                                     0,
                                                     (255, 255, 255),
                                                     1,
                                                 )
                                             cv2.putText(
                                                 frame,
                                                 "NA",
                                                 (cx - 10, cy - 10),
                                                 cv2.FONT_HERSHEY_SIMPLEX,
                                                 text_scl,
                                                 (255, 255, 255),
                                                 text_tk,
                                             )
                                         else:
-                                            name = self.event_probability[animal_name][
-                                                i
-                                            ][frame_count_analyze][0]
+                                            name = self.event_probability[animal_name][i][frame_count_analyze][0]
                                             probability = (
                                                 str(
                                                     round(
-                                                        self.event_probability[
-                                                            animal_name
-                                                        ][i][frame_count_analyze][1]
+                                                        self.event_probability[animal_name][i][frame_count_analyze][1]
                                                         * 100
                                                     )
                                                 )
                                                 + "%"
                                             )
                                             if name in colors:
                                                 color = colors[
-                                                    self.event_probability[animal_name][
-                                                        i
-                                                    ][frame_count_analyze][0]
+                                                    self.event_probability[animal_name][i][frame_count_analyze][0]
                                                 ]
                                                 if self.behavior_mode == 1:
                                                     cv2.drawContours(
                                                         frame,
-                                                        self.animal_contours[
-                                                            animal_name
-                                                        ][i][frame_count_analyze],
+                                                        self.animal_contours[animal_name][i][frame_count_analyze],
                                                         -1,
                                                         color,
                                                         1,
                                                     )
                                                 else:
                                                     cv2.drawContours(
                                                         frame,
-                                                        [
-                                                            self.animal_contours[
-                                                                animal_name
-                                                            ][i][frame_count_analyze]
-                                                        ],
+                                                        [self.animal_contours[animal_name][i][frame_count_analyze]],
                                                         0,
                                                         color,
                                                         1,
                                                     )
                                                 cv2.putText(
                                                     frame,
                                                     name + " " + probability,
@@ -2192,29 +1581,23 @@
                                                     color,
                                                     text_tk,
                                                 )
                                             else:
                                                 if self.behavior_mode == 1:
                                                     cv2.drawContours(
                                                         frame,
-                                                        self.animal_contours[
-                                                            animal_name
-                                                        ][i][frame_count_analyze],
+                                                        self.animal_contours[animal_name][i][frame_count_analyze],
                                                         -1,
                                                         (255, 255, 255),
                                                         1,
                                                     )
                                                 else:
                                                     cv2.drawContours(
                                                         frame,
-                                                        [
-                                                            self.animal_contours[
-                                                                animal_name
-                                                            ][i][frame_count_analyze]
-                                                        ],
+                                                        [self.animal_contours[animal_name][i][frame_count_analyze]],
                                                         0,
                                                         (255, 255, 255),
                                                         1,
                                                     )
                                                 cv2.putText(
                                                     frame,
                                                     "NA",
@@ -2232,19 +1615,15 @@
                                             cv2.FONT_HERSHEY_SIMPLEX,
                                             text_scl,
                                             (255, 255, 255),
                                             text_tk,
                                         )
                                         cv2.drawContours(
                                             frame,
-                                            [
-                                                self.animal_contours[animal_name][i][
-                                                    frame_count_analyze
-                                                ]
-                                            ],
+                                            [self.animal_contours[animal_name][i][frame_count_analyze]],
                                             0,
                                             (255, 255, 255),
                                             1,
                                         )
 
                 if writer is None:
                     (h, w) = frame.shape[:2]
@@ -2277,493 +1656,326 @@
             all_parameters += ["acceleration", "speed", "velocity"]
 
         if self.categorize_behavior is True:
             for animal_name in self.animal_kinds:
                 for behavior_name in self.all_behavior_parameters[animal_name]:
                     for i in self.event_probability[animal_name]:
                         if "count" in parameter_to_analyze:
-                            self.all_behavior_parameters[animal_name][behavior_name][
-                                "count"
-                            ][i] = 0
+                            self.all_behavior_parameters[animal_name][behavior_name]["count"][i] = 0
                         if "duration" in parameter_to_analyze:
-                            self.all_behavior_parameters[animal_name][behavior_name][
-                                "duration"
-                            ][i] = 0.0
+                            self.all_behavior_parameters[animal_name][behavior_name]["duration"][i] = 0.0
                         if "4 locomotion parameters" in parameter_to_analyze:
-                            self.all_behavior_parameters[animal_name][behavior_name][
-                                "distance"
-                            ][i] = 0.0
+                            self.all_behavior_parameters[animal_name][behavior_name]["distance"][i] = 0.0
                         if "latency" in parameter_to_analyze:
-                            self.all_behavior_parameters[animal_name][behavior_name][
-                                "latency"
-                            ][i] = "NA"
+                            self.all_behavior_parameters[animal_name][behavior_name]["latency"][i] = "NA"
                     for parameter_name in all_parameters:
                         for i in self.event_probability[animal_name]:
-                            self.all_behavior_parameters[animal_name][behavior_name][
-                                parameter_name
-                            ][i] = [np.nan] * len(self.all_time)
+                            self.all_behavior_parameters[animal_name][behavior_name][parameter_name][i] = [
+                                np.nan
+                            ] * len(self.all_time)
         else:
             for animal_name in self.animal_kinds:
                 for i in self.animal_contours[animal_name]:
                     if "4 locomotion parameters" in parameter_to_analyze:
                         self.all_behavior_parameters[animal_name]["distance"][i] = 0.0
                     for parameter_name in all_parameters:
-                        self.all_behavior_parameters[animal_name][parameter_name][i] = [
-                            np.nan
-                        ] * len(self.all_time)
+                        self.all_behavior_parameters[animal_name][parameter_name][i] = [np.nan] * len(self.all_time)
 
         if len(parameter_to_analyze) > 0:
             for animal_name in self.animal_kinds:
                 for i in self.animal_contours[animal_name]:
                     n = self.length + self.register_counts[animal_name][i]
 
                     while n < len(self.animal_contours[animal_name][i]):
                         if self.categorize_behavior is True:
                             behavior_name = self.event_probability[animal_name][i][n][0]
 
                             if behavior_name != "NA":
                                 if "count" in parameter_to_analyze:
-                                    if (
-                                        behavior_name
-                                        != self.event_probability[animal_name][i][
-                                            n - 1
-                                        ][0]
-                                    ):
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["count"][i] += 1
+                                    if behavior_name != self.event_probability[animal_name][i][n - 1][0]:
+                                        self.all_behavior_parameters[animal_name][behavior_name]["count"][i] += 1
 
                                 if "duration" in parameter_to_analyze:
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["duration"][i] += round(1 / self.fps, 2)
+                                    self.all_behavior_parameters[animal_name][behavior_name]["duration"][i] += round(
+                                        1 / self.fps, 2
+                                    )
 
                                 if "latency" in parameter_to_analyze:
-                                    if (
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["latency"][i]
-                                        == "NA"
-                                    ):
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["latency"][i] = self.all_time[n]
+                                    if self.all_behavior_parameters[animal_name][behavior_name]["latency"][i] == "NA":
+                                        self.all_behavior_parameters[animal_name][behavior_name]["latency"][i] = (
+                                            self.all_time[n]
+                                        )
 
                                 if "3 length parameters" in parameter_to_analyze:
                                     heights_diffs = []
-                                    for h in self.animal_heights[animal_name][i][
-                                        n - self.length + 1 : n + 1
-                                    ]:
-                                        if (
-                                            h is None
-                                            or self.animal_heights[animal_name][i][n]
-                                            is None
-                                        ):
+                                    for h in self.animal_heights[animal_name][i][n - self.length + 1 : n + 1]:
+                                        if h is None or self.animal_heights[animal_name][i][n] is None:
                                             height_diff = 0.0
                                         else:
-                                            height_diff = (
-                                                abs(
-                                                    h
-                                                    - self.animal_heights[animal_name][
-                                                        i
-                                                    ][n]
-                                                )
-                                                / h
-                                            )
+                                            height_diff = abs(h - self.animal_heights[animal_name][i][n]) / h
                                         heights_diffs.append(height_diff)
                                     magnitude_length = max(heights_diffs)
                                     vigor_length = magnitude_length / (
-                                        (self.length - np.argmax(heights_diffs))
-                                        / self.fps
-                                    )
-                                    intensity_length = sum(heights_diffs) / (
-                                        self.length / self.fps
+                                        (self.length - np.argmax(heights_diffs)) / self.fps
                                     )
+                                    intensity_length = sum(heights_diffs) / (self.length / self.fps)
                                     if magnitude_length > 0:
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["magnitude_length"][i][n] = magnitude_length
+                                        self.all_behavior_parameters[animal_name][behavior_name]["magnitude_length"][i][
+                                            n
+                                        ] = magnitude_length
                                     if vigor_length > 0:
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["vigor_length"][i][n] = vigor_length
+                                        self.all_behavior_parameters[animal_name][behavior_name]["vigor_length"][i][
+                                            n
+                                        ] = vigor_length
                                     if intensity_length > 0:
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["intensity_length"][i][n] = intensity_length
+                                        self.all_behavior_parameters[animal_name][behavior_name]["intensity_length"][i][
+                                            n
+                                        ] = intensity_length
 
                                 if "4 locomotion parameters" in parameter_to_analyze:
                                     distance_traveled = 0.0
                                     d = n - self.length
                                     while d < n - 1:
-                                        start_center = self.animal_centers[animal_name][
-                                            i
-                                        ][d]
-                                        end_center = self.animal_centers[animal_name][
-                                            i
-                                        ][d + 1]
+                                        start_center = self.animal_centers[animal_name][i][d]
+                                        end_center = self.animal_centers[animal_name][i][d + 1]
                                         if start_center is None or end_center is None:
                                             dt = 0.0
                                         else:
                                             dt = math.dist(end_center, start_center)
                                         distance_traveled += dt
                                         d += 1
                                     if normalize_distance is True:
-                                        calibrator = math.sqrt(
-                                            self.animal_area[animal_name]
-                                        )
-                                        distance_traveled = (
-                                            distance_traveled / calibrator
-                                        )
+                                        calibrator = math.sqrt(self.animal_area[animal_name])
+                                        distance_traveled = distance_traveled / calibrator
                                     speed = distance_traveled / (self.length / self.fps)
                                     end_center = self.animal_centers[animal_name][i][n]
                                     if end_center is not None:
                                         displacements = []
-                                        for ct in self.animal_centers[animal_name][i][
-                                            n - self.length + 1 : n + 1
-                                        ]:
+                                        for ct in self.animal_centers[animal_name][i][n - self.length + 1 : n + 1]:
                                             if ct is None:
                                                 displacements.append(0)
                                             else:
-                                                displacements.append(
-                                                    math.dist(end_center, ct)
-                                                )
+                                                displacements.append(math.dist(end_center, ct))
                                         displacement = max(displacements)
                                         if normalize_distance is True:
                                             displacement = displacement / calibrator
-                                        velocity = displacement / (
-                                            (self.length - np.argmax(displacements))
-                                            / self.fps
+                                        velocity = displacement / ((self.length - np.argmax(displacements)) / self.fps)
+                                        self.all_behavior_parameters[animal_name][behavior_name]["velocity"][i][n] = (
+                                            velocity
                                         )
-                                        self.all_behavior_parameters[animal_name][
-                                            behavior_name
-                                        ]["velocity"][i][n] = velocity
                                     velocities_max = []
                                     velocities_min = []
-                                    for v in self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["velocity"][i][n - self.length + 1 : n + 1]:
+                                    for v in self.all_behavior_parameters[animal_name][behavior_name]["velocity"][i][
+                                        n - self.length + 1 : n + 1
+                                    ]:
                                         if v != np.nan:
                                             velocities_max.append(v)
                                             velocities_min.append(v)
                                         else:
                                             velocities_max.append(-float("inf"))
                                             velocities_min.append(float("inf"))
                                     vmax = max(velocities_max)
                                     vmin = min(velocities_min)
                                     if vmax != -float("inf") and vmin != float("inf"):
-                                        if np.argmax(velocities_max) != np.argmin(
-                                            velocities_min
-                                        ):
-                                            t = (
-                                                abs(
-                                                    np.argmax(velocities_max)
-                                                    - np.argmin(velocities_min)
-                                                )
-                                                / self.fps
-                                            )
-                                            self.all_behavior_parameters[animal_name][
-                                                behavior_name
-                                            ]["acceleration"][i][n] = (vmax - vmin) / t
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["distance"][i] += distance_traveled
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["speed"][i][n] = speed
+                                        if np.argmax(velocities_max) != np.argmin(velocities_min):
+                                            t = abs(np.argmax(velocities_max) - np.argmin(velocities_min)) / self.fps
+                                            self.all_behavior_parameters[animal_name][behavior_name]["acceleration"][i][
+                                                n
+                                            ] = (vmax - vmin) / t
+                                    self.all_behavior_parameters[animal_name][behavior_name]["distance"][i] += (
+                                        distance_traveled
+                                    )
+                                    self.all_behavior_parameters[animal_name][behavior_name]["speed"][i][n] = speed
 
                                 if "3 areal parameters" in parameter_to_analyze:
                                     mask = np.zeros_like(self.background)
                                     contour = self.animal_contours[animal_name][i][n]
                                     if contour is not None:
-                                        cv2.drawContours(
-                                            mask, [contour], 0, (255, 255, 255), -1
-                                        )
+                                        cv2.drawContours(mask, [contour], 0, (255, 255, 255), -1)
                                         mask = cv2.cvtColor(mask, cv2.COLOR_BGR2GRAY)
                                         area_diffs = []
-                                        for ct in self.animal_contours[animal_name][i][
-                                            n - self.length + 1 : n + 1
-                                        ]:
+                                        for ct in self.animal_contours[animal_name][i][n - self.length + 1 : n + 1]:
                                             if ct is not None:
-                                                prev_mask = np.zeros_like(
-                                                    self.background
-                                                )
+                                                prev_mask = np.zeros_like(self.background)
                                                 cv2.drawContours(
                                                     prev_mask,
                                                     [ct],
                                                     0,
                                                     (255, 255, 255),
                                                     -1,
                                                 )
-                                                prev_mask = cv2.cvtColor(
-                                                    prev_mask, cv2.COLOR_BGR2GRAY
-                                                )
-                                                xlf1, ybt1, w, h = cv2.boundingRect(
-                                                    contour
-                                                )
+                                                prev_mask = cv2.cvtColor(prev_mask, cv2.COLOR_BGR2GRAY)
+                                                xlf1, ybt1, w, h = cv2.boundingRect(contour)
                                                 xrt1 = xlf1 + w
                                                 ytp1 = ybt1 + h
                                                 xlf2, ybt2, w, h = cv2.boundingRect(ct)
                                                 xrt2 = xlf2 + w
                                                 ytp2 = ybt2 + h
                                                 xlf = min(xlf1, xlf2)
                                                 xrt = max(xrt1, xrt2)
                                                 ybt = min(ybt1, ybt2)
                                                 ytp = max(ytp1, ytp2)
                                                 curr_mask = mask[ybt:ytp, xlf:xrt]
                                                 prev_mask = prev_mask[ybt:ytp, xlf:xrt]
-                                                diff = cv2.bitwise_xor(
-                                                    prev_mask, curr_mask
-                                                )
+                                                diff = cv2.bitwise_xor(prev_mask, curr_mask)
                                                 # diff[diff!=0]=255
-                                                area_diff = (np.sum(diff) / 255) / (
-                                                    np.sum(prev_mask) / 255
-                                                )
+                                                area_diff = (np.sum(diff) / 255) / (np.sum(prev_mask) / 255)
                                                 area_diffs.append(area_diff)
                                         if len(area_diffs) > 0:
                                             magnitude_area = max(area_diffs)
                                             vigor_area = magnitude_area / (
-                                                (self.length - np.argmax(area_diffs))
-                                                / self.fps
-                                            )
-                                            intensity_area = sum(area_diffs) / (
-                                                self.length / self.fps
+                                                (self.length - np.argmax(area_diffs)) / self.fps
                                             )
+                                            intensity_area = sum(area_diffs) / (self.length / self.fps)
                                             if magnitude_area > 0:
-                                                self.all_behavior_parameters[
-                                                    animal_name
-                                                ][behavior_name]["magnitude_area"][i][
-                                                    n
-                                                ] = magnitude_area
+                                                self.all_behavior_parameters[animal_name][behavior_name][
+                                                    "magnitude_area"
+                                                ][i][n] = magnitude_area
                                             if vigor_area > 0:
-                                                self.all_behavior_parameters[
-                                                    animal_name
-                                                ][behavior_name]["vigor_area"][i][
-                                                    n
-                                                ] = vigor_area
+                                                self.all_behavior_parameters[animal_name][behavior_name]["vigor_area"][
+                                                    i
+                                                ][n] = vigor_area
                                             if intensity_area > 0:
-                                                self.all_behavior_parameters[
-                                                    animal_name
-                                                ][behavior_name]["intensity_area"][i][
-                                                    n
-                                                ] = intensity_area
+                                                self.all_behavior_parameters[animal_name][behavior_name][
+                                                    "intensity_area"
+                                                ][i][n] = intensity_area
 
                         else:
                             if "3 length parameters" in parameter_to_analyze:
                                 heights_diffs = []
-                                for h in self.animal_heights[animal_name][i][
-                                    n - self.length + 1 : n + 1
-                                ]:
-                                    if (
-                                        h is None
-                                        or self.animal_heights[animal_name][i][n]
-                                        is None
-                                    ):
+                                for h in self.animal_heights[animal_name][i][n - self.length + 1 : n + 1]:
+                                    if h is None or self.animal_heights[animal_name][i][n] is None:
                                         height_diff = 0.0
                                     else:
-                                        height_diff = (
-                                            abs(
-                                                h
-                                                - self.animal_heights[animal_name][i][n]
-                                            )
-                                            / h
-                                        )
+                                        height_diff = abs(h - self.animal_heights[animal_name][i][n]) / h
                                     heights_diffs.append(height_diff)
                                 magnitude_length = max(heights_diffs)
-                                vigor_length = magnitude_length / (
-                                    (self.length - np.argmax(heights_diffs)) / self.fps
-                                )
-                                intensity_length = sum(heights_diffs) / (
-                                    self.length / self.fps
-                                )
+                                vigor_length = magnitude_length / ((self.length - np.argmax(heights_diffs)) / self.fps)
+                                intensity_length = sum(heights_diffs) / (self.length / self.fps)
                                 if magnitude_length > 0:
-                                    self.all_behavior_parameters[animal_name][
-                                        "magnitude_length"
-                                    ][i][n] = magnitude_length
+                                    self.all_behavior_parameters[animal_name]["magnitude_length"][i][n] = (
+                                        magnitude_length
+                                    )
                                 if vigor_length > 0:
-                                    self.all_behavior_parameters[animal_name][
-                                        "vigor_length"
-                                    ][i][n] = vigor_length
+                                    self.all_behavior_parameters[animal_name]["vigor_length"][i][n] = vigor_length
                                 if intensity_length > 0:
-                                    self.all_behavior_parameters[animal_name][
-                                        "intensity_length"
-                                    ][i][n] = intensity_length
+                                    self.all_behavior_parameters[animal_name]["intensity_length"][i][n] = (
+                                        intensity_length
+                                    )
 
                             if "4 locomotion parameters" in parameter_to_analyze:
                                 distance_traveled = 0.0
                                 d = n - self.length
                                 while d < n - 1:
-                                    start_center = self.animal_centers[animal_name][i][
-                                        d
-                                    ]
-                                    end_center = self.animal_centers[animal_name][i][
-                                        d + 1
-                                    ]
+                                    start_center = self.animal_centers[animal_name][i][d]
+                                    end_center = self.animal_centers[animal_name][i][d + 1]
                                     if start_center is None or end_center is None:
                                         dt = 0.0
                                     else:
                                         dt = math.dist(end_center, start_center)
                                     distance_traveled += dt
                                     d += 1
                                 if normalize_distance is True:
-                                    calibrator = math.sqrt(
-                                        self.animal_area[animal_name]
-                                    )
+                                    calibrator = math.sqrt(self.animal_area[animal_name])
                                     distance_traveled = distance_traveled / calibrator
                                 speed = distance_traveled / (self.length / self.fps)
                                 end_center = self.animal_centers[animal_name][i][n]
                                 if end_center is not None:
                                     displacements = []
-                                    for ct in self.animal_centers[animal_name][i][
-                                        n - self.length + 1 : n + 1
-                                    ]:
+                                    for ct in self.animal_centers[animal_name][i][n - self.length + 1 : n + 1]:
                                         if ct is None:
                                             displacements.append(0)
                                         else:
-                                            displacements.append(
-                                                math.dist(end_center, ct)
-                                            )
+                                            displacements.append(math.dist(end_center, ct))
                                     displacement = max(displacements)
                                     if normalize_distance is True:
                                         displacement = displacement / calibrator
-                                    velocity = displacement / (
-                                        (self.length - np.argmax(displacements))
-                                        / self.fps
-                                    )
-                                    self.all_behavior_parameters[animal_name][
-                                        "velocity"
-                                    ][i][n] = velocity
+                                    velocity = displacement / ((self.length - np.argmax(displacements)) / self.fps)
+                                    self.all_behavior_parameters[animal_name]["velocity"][i][n] = velocity
                                 velocities_max = []
                                 velocities_min = []
-                                for v in self.all_behavior_parameters[animal_name][
-                                    "velocity"
-                                ][i][n - self.length + 1 : n + 1]:
+                                for v in self.all_behavior_parameters[animal_name]["velocity"][i][
+                                    n - self.length + 1 : n + 1
+                                ]:
                                     if v != np.nan:
                                         velocities_max.append(v)
                                         velocities_min.append(v)
                                     else:
                                         velocities_max.append(-float("inf"))
                                         velocities_min.append(float("inf"))
                                 vmax = max(velocities_max)
                                 vmin = min(velocities_min)
                                 if vmax != -float("inf") and vmin != float("inf"):
-                                    if np.argmax(velocities_max) != np.argmin(
-                                        velocities_min
-                                    ):
-                                        t = (
-                                            abs(
-                                                np.argmax(velocities_max)
-                                                - np.argmin(velocities_min)
-                                            )
-                                            / self.fps
-                                        )
-                                        self.all_behavior_parameters[animal_name][
-                                            "acceleration"
-                                        ][i][n] = (vmax - vmin) / t
-                                self.all_behavior_parameters[animal_name]["distance"][
-                                    i
-                                ] += distance_traveled
-                                self.all_behavior_parameters[animal_name]["speed"][i][
-                                    n
-                                ] = speed
+                                    if np.argmax(velocities_max) != np.argmin(velocities_min):
+                                        t = abs(np.argmax(velocities_max) - np.argmin(velocities_min)) / self.fps
+                                        self.all_behavior_parameters[animal_name]["acceleration"][i][n] = (
+                                            vmax - vmin
+                                        ) / t
+                                self.all_behavior_parameters[animal_name]["distance"][i] += distance_traveled
+                                self.all_behavior_parameters[animal_name]["speed"][i][n] = speed
 
                             if "3 areal parameters" in parameter_to_analyze:
                                 mask = np.zeros_like(self.background)
                                 contour = self.animal_contours[animal_name][i][n]
                                 if contour is not None:
-                                    cv2.drawContours(
-                                        mask, [contour], 0, (255, 255, 255), -1
-                                    )
+                                    cv2.drawContours(mask, [contour], 0, (255, 255, 255), -1)
                                     mask = cv2.cvtColor(mask, cv2.COLOR_BGR2GRAY)
                                     area_diffs = []
-                                    for ct in self.animal_contours[animal_name][i][
-                                        n - self.length + 1 : n + 1
-                                    ]:
+                                    for ct in self.animal_contours[animal_name][i][n - self.length + 1 : n + 1]:
                                         if ct is not None:
                                             prev_mask = np.zeros_like(self.background)
-                                            cv2.drawContours(
-                                                prev_mask, [ct], 0, (255, 255, 255), -1
-                                            )
-                                            prev_mask = cv2.cvtColor(
-                                                prev_mask, cv2.COLOR_BGR2GRAY
-                                            )
+                                            cv2.drawContours(prev_mask, [ct], 0, (255, 255, 255), -1)
+                                            prev_mask = cv2.cvtColor(prev_mask, cv2.COLOR_BGR2GRAY)
                                             xlf1, ybt1, w, h = cv2.boundingRect(contour)
                                             xrt1 = xlf1 + w
                                             ytp1 = ybt1 + h
                                             xlf2, ybt2, w, h = cv2.boundingRect(ct)
                                             xrt2 = xlf2 + w
                                             ytp2 = ybt2 + h
                                             xlf = min(xlf1, xlf2)
                                             xrt = max(xrt1, xrt2)
                                             ybt = min(ybt1, ybt2)
                                             ytp = max(ytp1, ytp2)
                                             curr_mask = mask[ybt:ytp, xlf:xrt]
                                             prev_mask = prev_mask[ybt:ytp, xlf:xrt]
                                             diff = cv2.bitwise_xor(prev_mask, curr_mask)
                                             # diff[diff!=0]=255
-                                            area_diff = (np.sum(diff) / 255) / (
-                                                np.sum(prev_mask) / 255
-                                            )
+                                            area_diff = (np.sum(diff) / 255) / (np.sum(prev_mask) / 255)
                                             area_diffs.append(area_diff)
                                     if len(area_diffs) > 0:
                                         magnitude_area = max(area_diffs)
-                                        vigor_area = magnitude_area / (
-                                            (self.length - np.argmax(area_diffs))
-                                            / self.fps
-                                        )
-                                        intensity_area = sum(area_diffs) / (
-                                            self.length / self.fps
-                                        )
+                                        vigor_area = magnitude_area / ((self.length - np.argmax(area_diffs)) / self.fps)
+                                        intensity_area = sum(area_diffs) / (self.length / self.fps)
                                         if magnitude_area > 0:
-                                            self.all_behavior_parameters[animal_name][
-                                                "magnitude_area"
-                                            ][i][n] = magnitude_area
+                                            self.all_behavior_parameters[animal_name]["magnitude_area"][i][n] = (
+                                                magnitude_area
+                                            )
                                         if vigor_area > 0:
-                                            self.all_behavior_parameters[animal_name][
-                                                "vigor_area"
-                                            ][i][n] = vigor_area
+                                            self.all_behavior_parameters[animal_name]["vigor_area"][i][n] = vigor_area
                                         if intensity_area > 0:
-                                            self.all_behavior_parameters[animal_name][
-                                                "intensity_area"
-                                            ][i][n] = intensity_area
+                                            self.all_behavior_parameters[animal_name]["intensity_area"][i][n] = (
+                                                intensity_area
+                                            )
 
                         n += 1
 
                     if self.categorize_behavior is True:
                         if "duration" in parameter_to_analyze:
-                            for behavior_name in self.all_behavior_parameters[
-                                animal_name
-                            ]:
-                                if (
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["duration"][i]
-                                    != 0.0
-                                ):
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["duration"][i] += round(self.length / self.fps, 2)
+                            for behavior_name in self.all_behavior_parameters[animal_name]:
+                                if self.all_behavior_parameters[animal_name][behavior_name]["duration"][i] != 0.0:
+                                    self.all_behavior_parameters[animal_name][behavior_name]["duration"][i] += round(
+                                        self.length / self.fps, 2
+                                    )
                                 else:
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["duration"][i] = "NA"
+                                    self.all_behavior_parameters[animal_name][behavior_name]["duration"][i] = "NA"
 
                         if "4 locomotion parameters" in parameter_to_analyze:
-                            for behavior_name in self.all_behavior_parameters[
-                                animal_name
-                            ]:
-                                if (
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["distance"][i]
-                                    == 0.0
-                                ):
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ]["distance"][i] = "NA"
+                            for behavior_name in self.all_behavior_parameters[animal_name]:
+                                if self.all_behavior_parameters[animal_name][behavior_name]["distance"][i] == 0.0:
+                                    self.all_behavior_parameters[animal_name][behavior_name]["distance"][i] = "NA"
 
     def export_results(self, normalize_distance=True, parameter_to_analyze=[]):
         print("Quantifying behaviors...")
         print(datetime.datetime.now())
 
         self.analyze_parameters(
             normalize_distance=normalize_distance,
@@ -2771,23 +1983,35 @@
         )
 
         print("Behavioral quantification Completed!")
 
         print("Exporting results...")
         print(datetime.datetime.now())
 
+        # Export centers data every time
+        # centers = {}
+        # for animal_name, animal_centers_dict in self.animal_centers.items():
+        #     for i, centers_arr in animal_centers_dict.items():
+        #         centers[f"{animal_name}_{i}"] = centers_arr
+        for animal_name, centers_dict in self.animal_centers.items():
+            pd.DataFrame.from_dict(
+                centers_dict,
+                orient="index",
+                columns=self.all_time,
+            ).transpose().to_excel(
+                os.path.join(self.results_path, f"{animal_name}_centers.xlsx"),
+                float_format="%.2f",
+                index_label="time/ID",
+            )
+
         for animal_name in self.animal_kinds:
             if self.categorize_behavior is True:
-                events_df = pd.DataFrame(
-                    self.event_probability[animal_name], index=self.all_time
-                )
+                events_df = pd.DataFrame(self.event_probability[animal_name], index=self.all_time)
                 events_df.to_excel(
-                    os.path.join(
-                        self.results_path, animal_name + "_all_event_probability.xlsx"
-                    ),
+                    os.path.join(self.results_path, animal_name + "_all_event_probability.xlsx"),
                     float_format="%.2f",
                     index_label="time/ID",
                 )
 
             all_parameters = []
 
             if self.categorize_behavior is True:
@@ -2808,41 +2032,35 @@
             if "3 areal parameters" in parameter_to_analyze:
                 all_parameters += ["intensity_area", "magnitude_area", "vigor_area"]
             if "4 locomotion parameters" in parameter_to_analyze:
                 all_parameters += ["acceleration", "distance", "speed", "velocity"]
 
             if self.categorize_behavior is True:
                 for behavior_name in self.all_behavior_parameters[animal_name]:
-                    os.makedirs(
-                        os.path.join(self.results_path, behavior_name), exist_ok=True
-                    )
+                    os.makedirs(os.path.join(self.results_path, behavior_name), exist_ok=True)
 
                     summary = []
 
                     for parameter_name in all_parameters:
                         if parameter_name in [
                             "count",
                             "duration",
                             "distance",
                             "latency",
                         ]:
                             summary.append(
                                 pd.DataFrame.from_dict(
-                                    self.all_behavior_parameters[animal_name][
-                                        behavior_name
-                                    ][parameter_name],
+                                    self.all_behavior_parameters[animal_name][behavior_name][parameter_name],
                                     orient="index",
                                     columns=[parameter_name],
                                 ).reset_index(drop=True)
                             )
                         else:
                             individual_df = pd.DataFrame.from_dict(
-                                self.all_behavior_parameters[animal_name][
-                                    behavior_name
-                                ][parameter_name],
+                                self.all_behavior_parameters[animal_name][behavior_name][parameter_name],
                                 orient="index",
                                 columns=self.all_time,
                             )
                             if parameter_name != "probability":
                                 summary.append(
                                     individual_df.mean(axis=1, skipna=True)
                                     .to_frame()
@@ -2858,17 +2076,15 @@
                                 summary.append(
                                     individual_df.min(axis=1, skipna=True)
                                     .to_frame()
                                     .reset_index(drop=True)
                                     .rename(columns={0: parameter_name + "_min"})
                                 )
                             individual_df = pd.DataFrame(
-                                self.all_behavior_parameters[animal_name][
-                                    behavior_name
-                                ][parameter_name],
+                                self.all_behavior_parameters[animal_name][behavior_name][parameter_name],
                                 index=self.all_time,
                             )
                             individual_df.to_excel(
                                 os.path.join(
                                     self.results_path,
                                     behavior_name,
                                     animal_name + "_" + parameter_name + ".xlsx",
@@ -2891,17 +2107,15 @@
             else:
                 summary = []
 
                 for parameter_name in all_parameters:
                     if parameter_name == "distance":
                         summary.append(
                             pd.DataFrame.from_dict(
-                                self.all_behavior_parameters[animal_name][
-                                    parameter_name
-                                ],
+                                self.all_behavior_parameters[animal_name][parameter_name],
                                 orient="index",
                                 columns=["distance"],
                             ).reset_index(drop=True)
                         )
                     else:
                         individual_df = pd.DataFrame.from_dict(
                             self.all_behavior_parameters[animal_name][parameter_name],
@@ -2937,17 +2151,15 @@
                             ),
                             float_format="%.2f",
                             index_label="time/ID",
                         )
 
                 if len(summary) >= 1:
                     pd.concat(summary, axis=1).to_excel(
-                        os.path.join(
-                            self.results_path, animal_name + "_all_summary.xlsx"
-                        ),
+                        os.path.join(self.results_path, animal_name + "_all_summary.xlsx"),
                         float_format="%.2f",
                         index_label="ID/parameter",
                     )
 
         print("All results exported in: " + str(self.results_path))
 
     def generate_data(self, background_free=True, skip_redundant=1):
@@ -2992,36 +2204,29 @@
                     1,
                     frame_count_analyze,
                     background_free=background_free,
                     animation=animation,
                 )
 
                 for animal_name in self.animal_kinds:
-                    if (
-                        frame_count_analyze >= self.length
-                        and frame_count_analyze % skip_redundant == 0
-                    ):
+                    if frame_count_analyze >= self.length and frame_count_analyze % skip_redundant == 0:
                         for n in self.animal_centers[animal_name]:
                             h = w = 0
 
                             for i, f in enumerate(self.temp_frames):
                                 contour = self.animal_contours[animal_name][n][
-                                    frame_count_analyze
-                                    - self.length
-                                    + 1 : frame_count_analyze + 1
+                                    frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                 ][i]
                                 if contour is None:
                                     blob = np.zeros_like(self.background)
                                 else:
                                     blob = extract_blob_background(
                                         f,
                                         self.animal_contours[animal_name][n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         contour=contour,
                                         channel=3,
                                         background_free=background_free,
                                     )
                                     h, w = blob.shape[:2]
                                 animation.append(blob)
@@ -3055,17 +2260,15 @@
                                         + "_std"
                                         + str(self.std)
                                         + ".jpg"
                                     )
                                     pattern_image = generate_patternimage(
                                         self.background,
                                         self.animal_contours[animal_name][n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         inners=self.animal_inners[animal_name][n],
                                         std=self.std,
                                     )
                                 else:
                                     animation_name = (
                                         os.path.splitext(self.basename)[0]
@@ -3090,17 +2293,15 @@
                                         + "_len"
                                         + str(self.length)
                                         + ".jpg"
                                     )
                                     pattern_image = generate_patternimage(
                                         self.background,
                                         self.animal_contours[animal_name][n][
-                                            frame_count_analyze
-                                            - self.length
-                                            + 1 : frame_count_analyze + 1
+                                            frame_count_analyze - self.length + 1 : frame_count_analyze + 1
                                         ],
                                         inners=None,
                                         std=0,
                                     )
 
                                 path_animation = os.path.join(
                                     self.results_path,
@@ -3117,19 +2318,15 @@
                                     path_animation,
                                     cv2.VideoWriter_fourcc(*"MJPG"),
                                     self.fps / 5,
                                     (w, h),
                                     True,
                                 )
                                 for blob in animation:
-                                    writer.write(
-                                        cv2.resize(
-                                            blob, (w, h), interpolation=cv2.INTER_AREA
-                                        )
-                                    )
+                                    writer.write(cv2.resize(blob, (w, h), interpolation=cv2.INTER_AREA))
                                 writer.release()
 
                                 cv2.imwrite(path_pattern_image, pattern_image)
 
                 frame_count_analyze += 1
 
             frame_count += 1
@@ -3169,19 +2366,16 @@
                     frame = cv2.resize(
                         frame,
                         (self.framewidth, self.frameheight),
                         interpolation=cv2.INTER_AREA,
                     )
 
                 self.temp_frames.append(frame)
-                tensor_frame = torch.as_tensor(
-                    frame.astype("float32").transpose(2, 0, 1)
-                )
-                with torch.no_grad():
-                    output = self.detector([{"image": tensor_frame}])
+                tensor_frame = torch.as_tensor(frame.astype("float32").transpose(2, 0, 1))
+                output = self.detector([{"image": tensor_frame}])
                 instances = output[0]["instances"].to("cpu")
                 masks = instances.pred_masks.numpy().astype(np.uint8)
                 classes = instances.pred_classes.numpy()
                 scores = instances.scores.numpy()
 
                 if len(masks) == 0:
                     temp_contours.append(None)
@@ -3189,96 +2383,63 @@
                     animation.append(np.zeros_like(self.background))
 
                 else:
                     mask_area = np.sum(np.array(masks), axis=(1, 2))
                     exclusion_mask = np.zeros(len(masks), dtype=bool)
                     exclusion_mask[
                         np.where(
-                            (
-                                np.sum(
-                                    np.logical_and(masks[:, None], masks), axis=(2, 3)
-                                )
-                                / mask_area[:, None]
-                                > 0.8
-                            )
+                            (np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3)) / mask_area[:, None] > 0.8)
                             & (mask_area[:, None] < mask_area[None, :])
                         )[0]
                     ] = True
-                    masks = [
-                        m for m, exclude in zip(masks, exclusion_mask) if not exclude
-                    ]
-                    classes = [
-                        c for c, exclude in zip(classes, exclusion_mask) if not exclude
-                    ]
+                    masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
+                    classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                     classes = [self.animal_mapping[str(x)] for x in classes]
-                    scores = [
-                        s for s, exclude in zip(scores, exclusion_mask) if not exclude
-                    ]
+                    scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                     contours = []
                     inners = []
 
                     for animal_name in self.animal_kinds:
                         goodcontours = []
                         goodmasks = []
                         animal_number = int(self.animal_number[animal_name])
-                        animal_masks = [
-                            masks[a]
-                            for a, name in enumerate(classes)
-                            if name == animal_name
-                        ]
-                        animal_scores = [
-                            scores[a]
-                            for a, name in enumerate(classes)
-                            if name == animal_name
-                        ]
+                        animal_masks = [masks[a] for a, name in enumerate(classes) if name == animal_name]
+                        animal_scores = [scores[a] for a, name in enumerate(classes) if name == animal_name]
                         if len(animal_masks) > 0:
                             if len(animal_scores) > animal_number * 2:
-                                sorted_scores_indices = np.argsort(animal_scores)[
-                                    -int(animal_number * 2) :
-                                ]
-                                animal_masks = [
-                                    animal_masks[x] for x in sorted_scores_indices
-                                ]
+                                sorted_scores_indices = np.argsort(animal_scores)[-int(animal_number * 2) :]
+                                animal_masks = [animal_masks[x] for x in sorted_scores_indices]
                             for mask in animal_masks:
                                 mask = cv2.morphologyEx(
                                     mask,
                                     cv2.MORPH_CLOSE,
                                     np.ones((self.kernel, self.kernel), np.uint8),
                                 )
                                 cnts, _ = cv2.findContours(
                                     (mask * 255).astype(np.uint8),
                                     cv2.RETR_EXTERNAL,
                                     cv2.CHAIN_APPROX_NONE,
                                 )
-                                goodcontours.append(
-                                    sorted(cnts, key=cv2.contourArea, reverse=True)[0]
-                                )
+                                goodcontours.append(sorted(cnts, key=cv2.contourArea, reverse=True)[0])
                                 goodmasks.append(mask)
                             areas = [cv2.contourArea(ct) for ct in goodcontours]
-                            sorted_area_indices = np.argsort(np.array(areas))[
-                                -animal_number:
-                            ]
+                            sorted_area_indices = np.argsort(np.array(areas))[-animal_number:]
                             for x in sorted_area_indices:
                                 cnt = goodcontours[x]
                                 mask = goodmasks[x]
                                 contours.append(cnt)
                                 if self.include_bodyparts is True:
-                                    masked_frame = (
-                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
-                                    )
+                                    masked_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
                                     inners.append(get_inner(masked_frame, cnt))
 
                     temp_contours.append(contours)
                     temp_inners.append(inners)
 
-                    if (
-                        frame_count_analyze >= self.length
-                        and frame_count_analyze % skip_redundant == 0
-                    ):
+                    if frame_count_analyze >= self.length and frame_count_analyze % skip_redundant == 0:
                         (y_bt, y_tp, x_lf, x_rt) = crop_frame(
                             self.background,
                             functools.reduce(operator.iconcat, temp_contours, []),
                         )
 
                         h = w = 0
 
@@ -3355,34 +2516,26 @@
                                     x_lf,
                                     x_rt,
                                     temp_contours,
                                     temp_inners,
                                     std=0,
                                 )
 
-                            path_animation = os.path.join(
-                                self.results_path, "0", animation_name
-                            )
-                            path_pattern_image = os.path.join(
-                                self.results_path, "0", pattern_image_name
-                            )
+                            path_animation = os.path.join(self.results_path, "0", animation_name)
+                            path_pattern_image = os.path.join(self.results_path, "0", pattern_image_name)
 
                             writer = cv2.VideoWriter(
                                 path_animation,
                                 cv2.VideoWriter_fourcc(*"MJPG"),
                                 self.fps / 5,
                                 (w, h),
                                 True,
                             )
                             for blob in animation:
-                                writer.write(
-                                    cv2.resize(
-                                        blob, (w, h), interpolation=cv2.INTER_AREA
-                                    )
-                                )
+                                writer.write(cv2.resize(blob, (w, h), interpolation=cv2.INTER_AREA))
                             writer.release()
 
                             cv2.imwrite(path_pattern_image, pattern_image)
 
                 frame_count_analyze += 1
 
             frame_count += 1
@@ -3434,19 +2587,16 @@
                 if self.framewidth is not None:
                     frame = cv2.resize(
                         frame,
                         (self.framewidth, self.frameheight),
                         interpolation=cv2.INTER_AREA,
                     )
 
-                tensor_frame = torch.as_tensor(
-                    frame.astype("float32").transpose(2, 0, 1)
-                )
-                with torch.no_grad():
-                    output = self.detector([{"image": tensor_frame}])
+                tensor_frame = torch.as_tensor(frame.astype("float32").transpose(2, 0, 1))
+                output = self.detector([{"image": tensor_frame}])
                 instances = output[0]["instances"].to("cpu")
                 masks = instances.pred_masks.numpy().astype(np.uint8)
                 classes = instances.pred_classes.numpy()
                 scores = instances.scores.numpy()
 
                 if len(masks) == 0:
                     for animal_name in self.animal_kinds:
@@ -3461,219 +2611,136 @@
                                 self.animal_other_inners[animal_name][i].append([None])
 
                 else:
                     mask_area = np.sum(np.array(masks), axis=(1, 2))
                     exclusion_mask = np.zeros(len(masks), dtype=bool)
                     exclusion_mask[
                         np.where(
-                            (
-                                np.sum(
-                                    np.logical_and(masks[:, None], masks), axis=(2, 3)
-                                )
-                                / mask_area[:, None]
-                                > 0.8
-                            )
+                            (np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3)) / mask_area[:, None] > 0.8)
                             & (mask_area[:, None] < mask_area[None, :])
                         )[0]
                     ] = True
-                    masks = [
-                        m for m, exclude in zip(masks, exclusion_mask) if not exclude
-                    ]
-                    classes = [
-                        c for c, exclude in zip(classes, exclusion_mask) if not exclude
-                    ]
+                    masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
+                    classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                     classes = [self.animal_mapping[str(x)] for x in classes]
-                    scores = [
-                        s for s, exclude in zip(scores, exclusion_mask) if not exclude
-                    ]
+                    scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                     all_centers = []
                     all_masks = []
                     all_contours = []
                     all_inners = []
                     all_blobs = []
                     average_area = []
 
                     for animal_name in self.animal_kinds:
                         goodmasks = []
                         goodcontours = []
                         animal_number = int(self.animal_number[animal_name])
-                        animal_masks = [
-                            masks[a]
-                            for a, name in enumerate(classes)
-                            if name == animal_name
-                        ]
-                        animal_scores = [
-                            scores[a]
-                            for a, name in enumerate(classes)
-                            if name == animal_name
-                        ]
+                        animal_masks = [masks[a] for a, name in enumerate(classes) if name == animal_name]
+                        animal_scores = [scores[a] for a, name in enumerate(classes) if name == animal_name]
 
                         if len(animal_masks) == 0:
                             self.animal_present[animal_name] = 0
                             for i in self.animal_centers[animal_name]:
                                 self.animal_contours[animal_name][i].append(None)
-                                self.animal_other_contours[animal_name][i].append(
-                                    [None]
-                                )
+                                self.animal_other_contours[animal_name][i].append([None])
                                 self.animal_centers[animal_name][i].append(None)
                                 self.animal_blobs[animal_name][i].append(None)
                                 if self.include_bodyparts is True:
                                     self.animal_inners[animal_name][i].append(None)
-                                    self.animal_other_inners[animal_name][i].append(
-                                        [None]
-                                    )
+                                    self.animal_other_inners[animal_name][i].append([None])
                         else:
                             if len(animal_scores) > animal_number * 2:
-                                sorted_scores_indices = np.argsort(animal_scores)[
-                                    -int(animal_number * 2) :
-                                ]
-                                animal_masks = [
-                                    animal_masks[x] for x in sorted_scores_indices
-                                ]
+                                sorted_scores_indices = np.argsort(animal_scores)[-int(animal_number * 2) :]
+                                animal_masks = [animal_masks[x] for x in sorted_scores_indices]
                             for mask in animal_masks:
                                 mask = cv2.morphologyEx(
                                     mask,
                                     cv2.MORPH_CLOSE,
                                     np.ones((self.kernel, self.kernel), np.uint8),
                                 )
                                 goodmasks.append(mask)
                                 cnts, _ = cv2.findContours(
                                     (mask * 255).astype(np.uint8),
                                     cv2.RETR_EXTERNAL,
                                     cv2.CHAIN_APPROX_NONE,
                                 )
-                                goodcontours.append(
-                                    sorted(cnts, key=cv2.contourArea, reverse=True)[0]
-                                )
+                                goodcontours.append(sorted(cnts, key=cv2.contourArea, reverse=True)[0])
                             areas = [cv2.contourArea(ct) for ct in goodcontours]
-                            sorted_area_indices = np.argsort(np.array(areas))[
-                                -animal_number:
-                            ]
+                            sorted_area_indices = np.argsort(np.array(areas))[-animal_number:]
                             self.animal_present[animal_name] = len(sorted_area_indices)
                             areas_sorted = sorted(areas)[-animal_number:]
                             area = sum(areas_sorted) / len(areas_sorted)
                             if self.animal_area[animal_name] is None:
                                 self.animal_area[animal_name] = area
                             else:
-                                self.animal_area[animal_name] = (
-                                    self.animal_area[animal_name] + area
-                                ) / 2
+                                self.animal_area[animal_name] = (self.animal_area[animal_name] + area) / 2
                             average_area.append(self.animal_area[animal_name])
                             for x in sorted_area_indices:
                                 mask = goodmasks[x]
                                 all_masks.append(mask)
                                 cnt = goodcontours[x]
                                 all_contours.append(cnt)
                                 all_centers.append(
                                     (
-                                        int(
-                                            cv2.moments(cnt)["m10"]
-                                            / cv2.moments(cnt)["m00"]
-                                        ),
-                                        int(
-                                            cv2.moments(cnt)["m01"]
-                                            / cv2.moments(cnt)["m00"]
-                                        ),
+                                        int(cv2.moments(cnt)["m10"] / cv2.moments(cnt)["m00"]),
+                                        int(cv2.moments(cnt)["m01"] / cv2.moments(cnt)["m00"]),
                                     )
                                 )
                                 if self.include_bodyparts is True:
-                                    masked_frame = (
-                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
-                                    )
+                                    masked_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * mask
                                     all_inners.append(get_inner(masked_frame, cnt))
 
                     if len(all_centers) > 1:
                         centers_array = np.array(all_centers)
-                        distances_squared = np.sum(
-                            (centers_array[:, None] - centers_array) ** 2, axis=2
-                        )
+                        distances_squared = np.sum((centers_array[:, None] - centers_array) ** 2, axis=2)
                         determine = np.logical_and(
                             distances_squared > 0,
                             distances_squared
-                            < (
-                                math.sqrt(sum(average_area) / len(average_area))
-                                * self.social_distance
-                            )
-                            ** 2,
+                            < (math.sqrt(sum(average_area) / len(average_area)) * self.social_distance) ** 2,
                         )
                         other_contours = [
-                            [
-                                all_contours[x]
-                                for x, determ in enumerate(determine[y])
-                                if determ
-                            ]
+                            [all_contours[x] for x, determ in enumerate(determine[y]) if determ]
                             for y, c in enumerate(all_centers)
                         ]
                         if self.include_bodyparts is True:
                             other_inners = [
-                                [
-                                    all_inners[x]
-                                    for x, determ in enumerate(determine[y])
-                                    if determ
-                                ]
+                                [all_inners[x] for x, determ in enumerate(determine[y]) if determ]
                                 for y, c in enumerate(all_centers)
                             ]
                         other_masks = [
-                            np.bitwise_or.reduce(
-                                np.stack(np.array(all_masks)[determine[x]])
-                            )
-                            if len(c) > 0
-                            else None
+                            np.bitwise_or.reduce(np.stack(np.array(all_masks)[determine[x]])) if len(c) > 0 else None
                             for x, c in enumerate(other_contours)
                         ]
                         for i, other_mask in enumerate(other_masks):
                             if background_free is True:
-                                blob = frame * cv2.cvtColor(
-                                    all_masks[i], cv2.COLOR_GRAY2BGR
-                                )
+                                blob = frame * cv2.cvtColor(all_masks[i], cv2.COLOR_GRAY2BGR)
                                 if other_mask is not None:
                                     other_blob = cv2.cvtColor(
-                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-                                        * other_mask,
+                                        cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY) * other_mask,
                                         cv2.COLOR_GRAY2BGR,
                                     )
                                     blob = cv2.add(blob, other_blob)
-                                    blob = np.uint8(
-                                        exposure.rescale_intensity(
-                                            blob, out_range=(0, 255)
-                                        )
-                                    )
+                                    blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                             else:
-                                blob = np.uint8(
-                                    exposure.rescale_intensity(
-                                        frame, out_range=(0, 255)
-                                    )
-                                )
-                            cv2.drawContours(
-                                blob, [all_contours[i]], 0, (255, 0, 255), 2
-                            )
+                                blob = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
+                            cv2.drawContours(blob, [all_contours[i]], 0, (255, 0, 255), 2)
                             all_blobs.append(blob)
 
                     else:
                         if len(all_centers) > 0:
                             other_contours = [[None]]
                             if self.include_bodyparts is True:
                                 other_inners = [[None]]
                             if background_free is True:
-                                blob = frame * cv2.cvtColor(
-                                    all_masks[0], cv2.COLOR_GRAY2BGR
-                                )
-                                blob = np.uint8(
-                                    exposure.rescale_intensity(blob, out_range=(0, 255))
-                                )
+                                blob = frame * cv2.cvtColor(all_masks[0], cv2.COLOR_GRAY2BGR)
+                                blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                             else:
-                                blob = np.uint8(
-                                    exposure.rescale_intensity(
-                                        frame, out_range=(0, 255)
-                                    )
-                                )
-                            cv2.drawContours(
-                                blob, [all_contours[0]], 0, (255, 0, 255), 2
-                            )
+                                blob = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
+                            cv2.drawContours(blob, [all_contours[0]], 0, (255, 0, 255), 2)
                             all_blobs.append(blob)
 
                     n = 0
 
                     for animal_name in self.animal_number:
                         if self.animal_present[animal_name] > 0:
                             animal_length = n + self.animal_present[animal_name]
@@ -3682,118 +2749,86 @@
                             animal_contours = all_contours[n:animal_length]
                             animal_other_contours = other_contours[n:animal_length]
                             animal_blobs = all_blobs[n:animal_length]
                             if self.include_bodyparts is True:
                                 animal_inners = all_inners[n:animal_length]
                                 animal_other_inners = other_inners[n:animal_length]
 
-                            unused_existing_indices = list(
-                                self.animal_existingcenters[animal_name]
-                            )
-                            existing_centers = list(
-                                self.animal_existingcenters[animal_name].values()
-                            )
+                            unused_existing_indices = list(self.animal_existingcenters[animal_name])
+                            existing_centers = list(self.animal_existingcenters[animal_name].values())
                             unused_new_indices = list(range(len(animal_centers)))
-                            dt_flattened = distance.cdist(
-                                existing_centers, animal_centers
-                            ).flatten()
+                            dt_flattened = distance.cdist(existing_centers, animal_centers).flatten()
                             dt_sort_index = dt_flattened.argsort()
                             length = len(animal_centers)
 
                             for idx in dt_sort_index:
                                 index_in_existing = int(idx / length)
                                 index_in_new = int(idx % length)
                                 if index_in_existing in unused_existing_indices:
                                     if index_in_new in unused_new_indices:
-                                        unused_existing_indices.remove(
-                                            index_in_existing
-                                        )
+                                        unused_existing_indices.remove(index_in_existing)
                                         unused_new_indices.remove(index_in_new)
-                                        self.to_deregister[animal_name][
-                                            index_in_existing
-                                        ] = 0
+                                        self.to_deregister[animal_name][index_in_existing] = 0
                                         contour = animal_contours[index_in_new]
-                                        self.animal_contours[animal_name][
-                                            index_in_existing
-                                        ].append(contour)
+                                        self.animal_contours[animal_name][index_in_existing].append(contour)
                                         center = animal_centers[index_in_new]
-                                        self.animal_centers[animal_name][
-                                            index_in_existing
-                                        ].append(center)
-                                        self.animal_existingcenters[animal_name][
-                                            index_in_existing
-                                        ] = center
-                                        self.animal_other_contours[animal_name][
-                                            index_in_existing
-                                        ].append(animal_other_contours[index_in_new])
-
-                                        self.animal_blobs[animal_name][
-                                            index_in_existing
-                                        ].append(animal_blobs[index_in_new])
+                                        self.animal_centers[animal_name][index_in_existing].append(center)
+                                        self.animal_existingcenters[animal_name][index_in_existing] = center
+                                        self.animal_other_contours[animal_name][index_in_existing].append(
+                                            animal_other_contours[index_in_new]
+                                        )
+
+                                        self.animal_blobs[animal_name][index_in_existing].append(
+                                            animal_blobs[index_in_new]
+                                        )
                                         if self.include_bodyparts is True:
-                                            self.animal_inners[animal_name][
-                                                index_in_existing
-                                            ].append(animal_inners[index_in_new])
-                                            self.animal_other_inners[animal_name][
-                                                index_in_existing
-                                            ].append(animal_other_inners[index_in_new])
+                                            self.animal_inners[animal_name][index_in_existing].append(
+                                                animal_inners[index_in_new]
+                                            )
+                                            self.animal_other_inners[animal_name][index_in_existing].append(
+                                                animal_other_inners[index_in_new]
+                                            )
 
                             if len(unused_existing_indices) > 0:
                                 for i in unused_existing_indices:
-                                    if (
-                                        self.to_deregister[animal_name][i]
-                                        <= self.count_to_deregister
-                                    ):
+                                    if self.to_deregister[animal_name][i] <= self.count_to_deregister:
                                         self.to_deregister[animal_name][i] += 1
                                     else:
                                         self.animal_existingcenters[animal_name][i] = (
                                             -10000,
                                             -10000,
                                         )
                                     self.animal_contours[animal_name][i].append(None)
-                                    self.animal_other_contours[animal_name][i].append(
-                                        [None]
-                                    )
+                                    self.animal_other_contours[animal_name][i].append([None])
                                     self.animal_centers[animal_name][i].append(None)
                                     self.animal_blobs[animal_name][i].append(None)
                                     if self.include_bodyparts is True:
                                         self.animal_inners[animal_name][i].append(None)
-                                        self.animal_other_inners[animal_name][i].append(
-                                            [None]
-                                        )
+                                        self.animal_other_inners[animal_name][i].append([None])
 
                             n += self.animal_present[animal_name]
 
-                if (
-                    frame_count_analyze >= self.length
-                    and frame_count_analyze % skip_redundant == 0
-                ):
+                if frame_count_analyze >= self.length and frame_count_analyze % skip_redundant == 0:
                     for animal_name in self.animal_kinds:
                         if self.animal_present[animal_name] > 0:
                             for n in self.animal_centers[animal_name]:
                                 total_contours = functools.reduce(
                                     operator.iconcat,
                                     self.animal_other_contours[animal_name][n],
                                     [],
                                 )
                                 total_contours += self.animal_contours[animal_name][n]
-                                total_contours = [
-                                    i for i in total_contours if i is not None
-                                ]
+                                total_contours = [i for i in total_contours if i is not None]
 
                                 if len(total_contours) > 0:
-                                    (y_bt, y_tp, x_lf, x_rt) = crop_frame(
-                                        self.background, total_contours
-                                    )
+                                    (y_bt, y_tp, x_lf, x_rt) = crop_frame(self.background, total_contours)
 
                                     h = w = 0
 
-                                    for i, b in enumerate(
-                                        self.animal_blobs[animal_name][n]
-                                    ):
+                                    for i, b in enumerate(self.animal_blobs[animal_name][n]):
                                         if b is None:
                                             blob = np.zeros_like(self.background)
                                         else:
                                             blob = b[y_bt:y_tp, x_lf:x_rt]
                                             h, w = blob.shape[:2]
                                         animation.append(blob)
 
@@ -3835,23 +2870,17 @@
                                                 + "_std"
                                                 + str(self.std)
                                                 + "_itadv.jpg"
                                             )
                                             pattern_image = generate_patternimage_interact(
                                                 self.background,
                                                 self.animal_contours[animal_name][n],
-                                                self.animal_other_contours[animal_name][
-                                                    n
-                                                ],
-                                                inners=self.animal_inners[animal_name][
-                                                    n
-                                                ],
-                                                other_inners=self.animal_other_inners[
-                                                    animal_name
-                                                ][n],
+                                                self.animal_other_contours[animal_name][n],
+                                                inners=self.animal_inners[animal_name][n],
+                                                other_inners=self.animal_other_inners[animal_name][n],
                                                 std=self.std,
                                             )
                                         else:
                                             animation_name = (
                                                 os.path.splitext(self.basename)[0]
                                                 + "_"
                                                 + animal_name
@@ -3875,27 +2904,21 @@
                                                 + str(frame_count_analyze)
                                                 + "_len"
                                                 + str(self.length)
                                                 + "_scdt"
                                                 + scdt
                                                 + "_itadv.jpg"
                                             )
-                                            pattern_image = (
-                                                generate_patternimage_interact(
-                                                    self.background,
-                                                    self.animal_contours[animal_name][
-                                                        n
-                                                    ],
-                                                    self.animal_other_contours[
-                                                        animal_name
-                                                    ][n],
-                                                    inners=None,
-                                                    other_inners=None,
-                                                    std=0,
-                                                )
+                                            pattern_image = generate_patternimage_interact(
+                                                self.background,
+                                                self.animal_contours[animal_name][n],
+                                                self.animal_other_contours[animal_name][n],
+                                                inners=None,
+                                                other_inners=None,
+                                                std=0,
                                             )
 
                                         path_animation = os.path.join(
                                             self.results_path,
                                             str(animal_name) + "_" + str(n),
                                             animation_name,
                                         )
@@ -3950,37 +2973,19 @@
         uncertain=0,
         background_free=True,
         social_distance=0,
     ):
         print("Preparation started...")
         print(datetime.datetime.now())
 
-        config = os.path.join(path_to_detector, "config.yaml")
-        animalmapping = os.path.join(path_to_detector, "model_parameters.txt")
-        with open(animalmapping) as f:
-            model_parameters = f.read()
-        animal_mapping = json.loads(model_parameters)["animal_mapping"]
-        animal_names = json.loads(model_parameters)["animal_names"]
-        dt_infersize = int(json.loads(model_parameters)["inferencing_framesize"])
-        print(
-            "The total categories of animals / objects in this Detector: "
-            + str(animal_names)
-        )
-        print(
-            "The animals / objects of interest in this Detector: " + str(animal_kinds)
-        )
-        print("The inferencing framesize of this Detector: " + str(dt_infersize))
-        cfg = get_cfg()
-        cfg.merge_from_file(config)
-        cfg.MODEL.DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
-        detector = build_model(cfg)
-        DetectionCheckpointer(detector).load(
-            os.path.join(path_to_detector, "model_final.pth")
-        )
-        detector.eval()
+        detector = Detector(path=path_to_detector)
+        print(f"The total categories of animals / objects in this Detector: {detector.animal_names}")
+        print(f"The animals / objects of interest in this Detector: {animal_kinds}")
+        print(f"The inferencing framesize of this Detector: {detector.inferencing_framesize}")
+        animal_mapping = detector.animal_mapping
 
         if social_distance == 0:
             social_distance = float("inf")
 
         print("Preparation completed!")
 
         if generate is True:
@@ -3999,42 +3004,43 @@
                     else:
                         hex_color = names_and_colors[behavior_name][1].lstrip("#")
                         color = tuple(int(hex_color[i : i + 2], 16) for i in (0, 2, 4))
                         colors[behavior_name] = color[::-1]
                     for animal_name in animal_kinds:
                         if animal_name in animal_to_include:
                             animal_information[behavior_name][animal_name] = {}
-                            animal_information[behavior_name][animal_name][
-                                "probability"
-                            ] = {}
+                            animal_information[behavior_name][animal_name]["probability"] = {}
+                            animal_information[behavior_name][animal_name]["probability"] = {}
                             animal_information[behavior_name][animal_name]["count"] = {}
+                            animal_information[behavior_name][animal_name]["date"] = {}
+                            animal_information[behavior_name][animal_name]["time"] = {}
             print("Analyzing images...")
         print(datetime.datetime.now())
 
         for path_to_image in list(path_to_images):
             blobs = []
             image = cv2.imread(path_to_image)
             image_name = os.path.splitext(os.path.basename(path_to_image))[0]
 
             if generate is False:
                 for behavior_name in names_and_colors:
                     for animal_name in animal_kinds:
                         if animal_name in animal_to_include:
-                            animal_information[behavior_name][animal_name][
-                                "probability"
-                            ][image_name] = [[]]
-                            animal_information[behavior_name][animal_name]["count"][
-                                image_name
-                            ] = 0
+                            animal_information[behavior_name][animal_name]["probability"][image_name] = [[]]
+                            animal_information[behavior_name][animal_name]["count"][image_name] = 0
+                            animal_information[behavior_name][animal_name]["time"][image_name] = (
+                                pd.to_datetime(int(os.path.getmtime(path_to_image)), utc=True, unit="s")
+                            ).strftime("%H:%M:%S")
+                            animal_information[behavior_name][animal_name]["date"][image_name] = (
+                                pd.to_datetime(int(os.path.getmtime(path_to_image)), utc=True, unit="s")
+                            ).strftime("%Y-%m-%d")
 
             if imagewidth is not None:
                 imageheight = int(image.shape[0] * imagewidth / image.shape[1])
-                image = cv2.resize(
-                    image, (imagewidth, imageheight), interpolation=cv2.INTER_AREA
-                )
+                image = cv2.resize(image, (imagewidth, imageheight), interpolation=cv2.INTER_AREA)
                 kernel = min(imagewidth, imageheight)
             else:
                 kernel = min(image.shape[0], image.shape[1])
 
             if generate is False:
                 text_scl = max(kernel / 960, 0.5)
                 text_tk = max(1, int(kernel / 960))
@@ -4050,65 +3056,52 @@
                 kernel = 5
             elif kernel < 1500:
                 kernel = 7
             else:
                 kernel = 9
 
             tensor_image = torch.as_tensor(image.astype("float32").transpose(2, 0, 1))
-            with torch.no_grad():
-                output = detector([{"image": tensor_image}])
+            output = detector([{"image": tensor_image}])
             instances = output[0]["instances"].to("cpu")
             masks = instances.pred_masks.numpy().astype(np.uint8)
             classes = instances.pred_classes.numpy()
             scores = instances.scores.numpy()
 
             if len(masks) > 0:
                 mask_area = np.sum(np.array(masks), axis=(1, 2))
                 exclusion_mask = np.zeros(len(masks), dtype=bool)
                 exclusion_mask[
                     np.where(
-                        (
-                            np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3))
-                            / mask_area[:, None]
-                            > 0.8
-                        )
+                        (np.sum(np.logical_and(masks[:, None], masks), axis=(2, 3)) / mask_area[:, None] > 0.8)
                         & (mask_area[:, None] < mask_area[None, :])
                     )[0]
                 ] = True
                 masks = [m for m, exclude in zip(masks, exclusion_mask) if not exclude]
-                classes = [
-                    c for c, exclude in zip(classes, exclusion_mask) if not exclude
-                ]
+                classes = [c for c, exclude in zip(classes, exclusion_mask) if not exclude]
                 classes = [animal_mapping[str(x)] for x in classes]
-                scores = [
-                    s for s, exclude in zip(scores, exclusion_mask) if not exclude
-                ]
+                scores = [s for s, exclude in zip(scores, exclusion_mask) if not exclude]
 
                 contours = []
                 blobs = []
                 blobclasses = []
                 blobscores = []
 
                 for n, mask in enumerate(masks):
                     score = scores[n]
                     if score > detection_threshold:
-                        mask = cv2.morphologyEx(
-                            mask, cv2.MORPH_CLOSE, np.ones((kernel, kernel), np.uint8)
-                        )
+                        mask = cv2.morphologyEx(mask, cv2.MORPH_CLOSE, np.ones((kernel, kernel), np.uint8))
                         cnts, _ = cv2.findContours(
                             (mask * 255).astype(np.uint8),
                             cv2.RETR_EXTERNAL,
                             cv2.CHAIN_APPROX_NONE,
                         )
                         cnt = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
                         contours.append(cnt)
                         if background_free is True:
-                            masked_image = image * cv2.cvtColor(
-                                mask, cv2.COLOR_GRAY2BGR
-                            )
+                            masked_image = image * cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
                         else:
                             masked_image = image
                         x, y, w, h = cv2.boundingRect(cnt)
                         difference = int(abs(w - h) / 2) + 1
                         if w > h:
                             y_bt = max(y - difference - 1, 0)
                             y_tp = min(y + h + difference + 1, image.shape[0])
@@ -4116,93 +3109,76 @@
                             x_rt = min(x + w + 1, image.shape[1])
                         else:
                             y_bt = max(y - 1, 0)
                             y_tp = min(y + h + 1, image.shape[0])
                             x_lf = max(x - difference - 1, 0)
                             x_rt = min(x + w + difference + 1, image.shape[1])
                         blob = masked_image[y_bt:y_tp, x_lf:x_rt]
-                        blob = np.uint8(
-                            exposure.rescale_intensity(blob, out_range=(0, 255))
-                        )
+                        blob = np.uint8(exposure.rescale_intensity(blob, out_range=(0, 255)))
                         if generate is True:
                             cv2.imwrite(
-                                os.path.join(
-                                    results_path, image_name + "_" + str(n) + ".jpg"
-                                ),
+                                os.path.join(results_path, image_name + "_" + str(n) + ".jpg"),
                                 blob,
                             )
                         else:
-                            blob = cv2.resize(
-                                blob, (dim_conv, dim_conv), interpolation=cv2.INTER_AREA
-                            )
+                            blob = cv2.resize(blob, (dim_conv, dim_conv), interpolation=cv2.INTER_AREA)
                             if channel == 1:
                                 blob = cv2.cvtColor(blob, cv2.COLOR_BGR2GRAY)
                             blobs.append(img_to_array(blob))
                             blobclasses.append(classes[n])
                             blobscores.append(score)
 
                 if generate is False:
                     with tf.device("CPU"):
-                        blobs = tf.convert_to_tensor(
-                            np.array(blobs, dtype="float32") / 255.0
-                        )
+                        blobs = tf.convert_to_tensor(np.array(blobs, dtype="float32") / 255.0)
                     predictions = categorizer.predict(blobs, batch_size=32)
 
                     for idx, animal_name in enumerate(blobclasses):
                         if animal_name in animal_to_include:
                             prediction = predictions[idx]
-                            for name_index, behavior_name in enumerate(
-                                names_and_colors
-                            ):
+                            for name_index, behavior_name in enumerate(names_and_colors):
                                 if len(names_and_colors) == 2:
                                     if name_index == 0:
                                         probability = 1 - prediction[0]
                                     else:
                                         probability = prediction[0]
                                 else:
                                     probability = prediction[name_index]
-                                animal_information[behavior_name][animal_name][
-                                    "probability"
-                                ][image_name][0].append(probability)
+                                animal_information[behavior_name][animal_name]["probability"][image_name][0].append(
+                                    probability
+                                )
                             behavior_names = list(names_and_colors.keys())
                             if len(behavior_names) == 2:
                                 if prediction[0] > 0.5:
                                     if prediction[0] - (1 - prediction[0]) > uncertain:
-                                        animal_information[behavior_names[1]][
-                                            animal_name
-                                        ]["count"][image_name] += 1
+                                        animal_information[behavior_names[1]][animal_name]["count"][image_name] += 1
                                         if behavior_names[1] in colors:
                                             cv2.drawContours(
                                                 image,
                                                 [contours[idx]],
                                                 0,
                                                 colors[behavior_names[1]],
                                                 1,
                                             )
                                 if prediction[0] < 0.5:
                                     if (1 - prediction[0]) - prediction[0] > uncertain:
-                                        animal_information[behavior_names[0]][
-                                            animal_name
-                                        ]["count"][image_name] += 1
+                                        animal_information[behavior_names[0]][animal_name]["count"][image_name] += 1
                                         if behavior_names[0] in colors:
                                             cv2.drawContours(
                                                 image,
                                                 [contours[idx]],
                                                 0,
                                                 colors[behavior_names[0]],
                                                 1,
                                             )
                             else:
-                                if (
-                                    sorted(prediction)[-1] - sorted(prediction)[-2]
-                                    > uncertain
-                                ):
-                                    animal_information[
-                                        behavior_names[np.argmax(prediction)]
-                                    ][animal_name]["count"][image_name] += 1
+                                if sorted(prediction)[-1] - sorted(prediction)[-2] > uncertain:
+                                    animal_information[behavior_names[np.argmax(prediction)]][animal_name]["count"][
+                                        image_name
+                                    ] += 1
                                     cv2.drawContours(
                                         image,
                                         [contours[idx]],
                                         0,
                                         colors[behavior_names[np.argmax(prediction)]],
                                         1,
                                     )
@@ -4233,37 +3209,46 @@
 
         if generate is True:
             print("Behavior example generation completed!")
 
         else:
             for behavior_name in names_and_colors:
                 for animal_name in animal_to_include:
-                    names = np.array(
-                        list(
-                            animal_information[behavior_name][animal_name][
-                                "count"
-                            ].keys()
-                        )
+                    names = np.array(list(animal_information[behavior_name][animal_name]["count"].keys()))
+
+                    results_df1 = pd.DataFrame.from_dict(
+                        animal_information[behavior_name][animal_name]["count"], orient="index", columns=["count"]
                     )
-                    results_df = pd.DataFrame.from_dict(
-                        animal_information[behavior_name][animal_name]["count"],
-                        orient="index",
-                        columns=["count"],
-                    ).reset_index(drop=True)
-                    results_df.set_index(names).join(
+                    results_df2 = pd.DataFrame.from_dict(
+                        animal_information[behavior_name][animal_name]["date"], orient="index", columns=["date"]
+                    )
+
+                    results_df3 = pd.DataFrame.from_dict(
+                        animal_information[behavior_name][animal_name]["time"], orient="index", columns=["time"]
+                    )
+
+                    # Very weird solution, had to create new dataframe from count and date/time merge
+                    firstCombination = pd.merge(
+                        results_df1, results_df2, left_index=True, right_index=True, how="outer"
+                    )
+
+                    results_df = pd.merge(firstCombination, results_df3, left_index=True, right_index=True, how="outer")
+
+                    # Sets the index to names, if future dataframes/data need to be join do it here
+                    results_df = results_df.set_index(names)
+                    results_df = results_df.join(
                         pd.DataFrame.from_dict(
-                            animal_information[behavior_name][animal_name][
-                                "probability"
-                            ],
+                            animal_information[behavior_name][animal_name]["probability"],
                             orient="index",
                             columns=["probability"],
                         )
                         .reset_index(drop=True)
                         .set_index(names)
-                    ).to_excel(
-                        os.path.join(
-                            results_path, behavior_name + "_" + animal_name + ".xlsx"
-                        ),
+                    )
+
+                    # Exports the data to an excel file: format is 'behaviorName_animalName.xlsx'
+                    results_df.to_excel(
+                        os.path.join(results_path, behavior_name + "_" + animal_name + ".xlsx"),
                         index_label="imagename/parameter",
                     )
 
             print("All results exported in: " + str(results_path))
```

### Comparing `labgym-2.3.5/LabGym/categorizers.py` & `labgym-2.4.0/LabGym/categorizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import matplotlib
 
-from .tools import *
-
 matplotlib.use("Agg")
 import datetime
 import os
 import random
 import shutil
 from collections import deque
 from pathlib import Path
@@ -57,25 +54,23 @@
     ZeroPadding2D,
     concatenate,
 )
 from tensorflow.keras.models import Model, load_model
 from tensorflow.keras.optimizers import SGD
 from tensorflow.keras.preprocessing.image import img_to_array
 
+from LabGym.tools import *
+
 CATEGORIZER_FOLDER = Path(__file__).resolve().parent / "models"
 
 
 def get_categorizer_names() -> list[str]:
     """Return the names of all saved categorizers."""
     ignore = ["__pycache__", "__init__", "__init.py__"]
-    return [
-        path.name
-        for path in CATEGORIZER_FOLDER.glob("*")
-        if path.is_dir() and path.name not in ignore
-    ]
+    return [path.name for path in CATEGORIZER_FOLDER.glob("*") if path.is_dir() and path.name not in ignore]
 
 
 def delete_categorizer(categorizer_name: str):
     """Permanently delete the given categorizer."""
     shutil.rmtree(str(CATEGORIZER_FOLDER / categorizer_name))
 
 
@@ -93,76 +88,52 @@
             ".bmp",
             ".BMP",
         )
         self.extension_video = (".avi", ".mpg", ".wmv", ".mp4", ".mkv", ".m4v", ".mov")
         self.classnames = None
 
     def rename_label(self, file_path, new_path, resize=None):
-        folder_list = [
-            i
-            for i in os.listdir(file_path)
-            if os.path.isdir(os.path.join(file_path, i))
-        ]
+        folder_list = [i for i in os.listdir(file_path) if os.path.isdir(os.path.join(file_path, i))]
         print("Behavior names are: " + str(folder_list))
         previous_lenth = None
         imagedata = False
 
         for folder in folder_list:
-            name_list = [
-                i
-                for i in os.listdir(os.path.join(file_path, folder))
-                if i.endswith(".avi")
-            ]
+            name_list = [i for i in os.listdir(os.path.join(file_path, folder)) if i.endswith(".avi")]
 
             if len(name_list) == 0:
-                name_list = [
-                    i
-                    for i in os.listdir(os.path.join(file_path, folder))
-                    if i.endswith(".jpg")
-                ]
+                name_list = [i for i in os.listdir(os.path.join(file_path, folder)) if i.endswith(".jpg")]
                 imagedata = True
 
             for i in name_list:
                 if imagedata is True:
                     image = os.path.join(file_path, folder, i)
-                    new_image = os.path.join(
-                        new_path, str(name_list.index(i)) + "_" + folder + ".jpg"
-                    )
+                    new_image = os.path.join(new_path, str(name_list.index(i)) + "_" + folder + ".jpg")
                     image = cv2.imread(image)
                     if resize is not None:
-                        image = cv2.resize(
-                            image, (resize, resize), interpolation=cv2.INTER_AREA
-                        )
+                        image = cv2.resize(image, (resize, resize), interpolation=cv2.INTER_AREA)
                     cv2.imwrite(new_image, image)
 
                 else:
                     animation = os.path.join(file_path, folder, i)
-                    pattern_image = os.path.join(
-                        file_path, folder, os.path.splitext(i)[0] + ".jpg"
-                    )
+                    pattern_image = os.path.join(file_path, folder, os.path.splitext(i)[0] + ".jpg")
                     current_length = 0
 
-                    new_animation = os.path.join(
-                        new_path, str(name_list.index(i)) + "_" + folder + ".avi"
-                    )
-                    new_pattern_image = os.path.join(
-                        new_path, str(name_list.index(i)) + "_" + folder + ".jpg"
-                    )
+                    new_animation = os.path.join(new_path, str(name_list.index(i)) + "_" + folder + ".avi")
+                    new_pattern_image = os.path.join(new_path, str(name_list.index(i)) + "_" + folder + ".jpg")
                     writer = None
                     capture = cv2.VideoCapture(animation)
                     fps = round(capture.get(cv2.CAP_PROP_FPS))
                     while True:
                         retval, frame = capture.read()
                         current_length += 1
                         if frame is None:
                             break
                         if resize is not None:
-                            frame = cv2.resize(
-                                frame, (resize, resize), interpolation=cv2.INTER_AREA
-                            )
+                            frame = cv2.resize(frame, (resize, resize), interpolation=cv2.INTER_AREA)
                         if writer is None:
                             (h, w) = frame.shape[:2]
                             writer = cv2.VideoWriter(
                                 new_animation,
                                 cv2.VideoWriter_fourcc(*"MJPG"),
                                 fps,
                                 (w, h),
@@ -350,17 +321,15 @@
                     scale = np.random.uniform(0.6, 0.9)
                 else:
                     scale = None
 
                 if "del1" in m:
                     if time_step >= 30:
                         idx1 = random.randint(0, round(time_step / 3))
-                        idx2 = random.randint(
-                            round(time_step / 3) + 1, round(time_step * 2 / 3)
-                        )
+                        idx2 = random.randint(round(time_step / 3) + 1, round(time_step * 2 / 3))
                         to_delete = [idx1, idx2]
                     else:
                         to_delete = [random.randint(0, round(time_step / 3))]
                 elif "del2" in m:
                     to_delete = [random.randint(0, round(time_step / 2) + 1)]
                 else:
                     to_delete = None
@@ -380,57 +349,41 @@
                             break
                         frames.append(frame)
 
                     frames_length = len(frames)
                     if frames_length < time_step:
                         for diff in range(time_step - frames_length):
                             frames.append(np.zeros_like(original_frame))
-                        print(
-                            "Inconsistent duration of animation detected at: "
-                            + str(i)
-                            + "."
-                        )
-                        print(
-                            "Zero padding has been used, which may decrease the training accuracy."
-                        )
+                        print("Inconsistent duration of animation detected at: " + str(i) + ".")
+                        print("Zero padding has been used, which may decrease the training accuracy.")
 
                     for frame in frames:
                         if to_delete is not None and n in to_delete:
                             blob = np.zeros_like(original_frame)
 
                         else:
-                            frame_contrast = np.uint8(
-                                exposure.rescale_intensity(frame, out_range=(0, 255))
-                            )
+                            frame_contrast = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
 
                             if background_free is True:
-                                frame_gray = cv2.cvtColor(
-                                    frame_contrast, cv2.COLOR_BGR2GRAY
-                                )
+                                frame_gray = cv2.cvtColor(frame_contrast, cv2.COLOR_BGR2GRAY)
                                 thred = cv2.threshold(
                                     frame_gray,
                                     0,
                                     255,
                                     cv2.THRESH_BINARY + cv2.THRESH_OTSU,
                                 )[1]
-                                cnts, _ = cv2.findContours(
-                                    thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE
-                                )
+                                cnts, _ = cv2.findContours(thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE)
                                 if len(cnts) == 0:
                                     blob = np.zeros_like(frame)
                                 else:
                                     if behavior_mode == 0:
-                                        contour = sorted(
-                                            cnts, key=cv2.contourArea, reverse=True
-                                        )[0]
+                                        contour = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
                                         blob = extract_blob(frame, contour, channel=3)
                                     else:
-                                        (y_bt, y_tp, x_lf, x_rt) = crop_frame(
-                                            frame, cnts
-                                        )
+                                        (y_bt, y_tp, x_lf, x_rt) = crop_frame(frame, cnts)
                                         blob = frame_contrast[y_bt:y_tp, x_lf:x_rt]
                             else:
                                 blob = frame_contrast
 
                             if code is not None:
                                 blob = cv2.flip(blob, code)
 
@@ -439,17 +392,15 @@
                                 if background_free is True:
                                     blob[blob > 30] += beta
                                 else:
                                     blob += beta
                                 blob = np.uint8(np.clip(blob, 0, 255))
 
                             if angle is not None:
-                                blob = ndimage.rotate(
-                                    blob, angle, reshape=False, prefilter=False
-                                )
+                                blob = ndimage.rotate(blob, angle, reshape=False, prefilter=False)
 
                             if shear is not None:
                                 tf = AffineTransform(shear=shear)
                                 blob = transform.warp(
                                     blob,
                                     tf,
                                     order=1,
@@ -470,25 +421,21 @@
                                         blob,
                                         (int(blob.shape[1] * scale), blob.shape[0]),
                                         interpolation=cv2.INTER_AREA,
                                     )
                                 blob_scl = img_to_array(blob_scl)
                                 x = (blob_black.shape[1] - blob_scl.shape[1]) // 2
                                 y = (blob_black.shape[0] - blob_scl.shape[0]) // 2
-                                blob_black[
-                                    y : y + blob_scl.shape[0], x : x + blob_scl.shape[1]
-                                ] = blob_scl
+                                blob_black[y : y + blob_scl.shape[0], x : x + blob_scl.shape[1]] = blob_scl
                                 blob = blob_black
 
                         if channel == 1:
                             blob = cv2.cvtColor(np.uint8(blob), cv2.COLOR_BGR2GRAY)
 
-                        blob = cv2.resize(
-                            blob, (dim_tconv, dim_tconv), interpolation=cv2.INTER_AREA
-                        )
+                        blob = cv2.resize(blob, (dim_tconv, dim_tconv), interpolation=cv2.INTER_AREA)
                         blob = img_to_array(blob)
                         animation.append(blob)
 
                         n += 1
 
                     capture.release()
 
@@ -498,51 +445,39 @@
 
                 if code is not None:
                     pattern_image = cv2.flip(pattern_image, code)
 
                 if behavior_mode >= 3:
                     if beta is not None:
                         if background_free is True:
-                            pattern_image_gray = cv2.cvtColor(
-                                pattern_image, cv2.COLOR_BGR2GRAY
-                            )
+                            pattern_image_gray = cv2.cvtColor(pattern_image, cv2.COLOR_BGR2GRAY)
                             thred = cv2.threshold(
                                 pattern_image_gray,
                                 0,
                                 255,
                                 cv2.THRESH_BINARY + cv2.THRESH_OTSU,
                             )[1]
-                            cnts, _ = cv2.findContours(
-                                thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE
-                            )
+                            cnts, _ = cv2.findContours(thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE)
                             if len(cnts) == 0:
                                 pattern_image = np.zeros_like(pattern_image)
                             else:
-                                contour = sorted(
-                                    cnts, key=cv2.contourArea, reverse=True
-                                )[0]
-                                pattern_image = extract_blob(
-                                    pattern_image, contour, channel=3
-                                )
+                                contour = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
+                                pattern_image = extract_blob(pattern_image, contour, channel=3)
                             pattern_image = pattern_image.astype("float")
                             pattern_image[pattern_image > 30] += beta
                         else:
                             pattern_image += beta
                         pattern_image = np.uint8(np.clip(pattern_image, 0, 255))
 
                 if angle is not None:
-                    pattern_image = ndimage.rotate(
-                        pattern_image, angle, reshape=False, prefilter=False
-                    )
+                    pattern_image = ndimage.rotate(pattern_image, angle, reshape=False, prefilter=False)
 
                 if shear is not None:
                     tf = AffineTransform(shear=shear)
-                    pattern_image = transform.warp(
-                        pattern_image, tf, order=1, preserve_range=True, mode="constant"
-                    )
+                    pattern_image = transform.warp(pattern_image, tf, order=1, preserve_range=True, mode="constant")
 
                 if scale is not None:
                     pattern_image_black = np.zeros_like(pattern_image)
                     if width == 0:
                         pattern_image_scl = cv2.resize(
                             pattern_image,
                             (
@@ -567,21 +502,17 @@
                         x : x + pattern_image_scl.shape[1],
                         :,
                     ] = pattern_image_scl
                     pattern_image = pattern_image_black
 
                 if behavior_mode >= 3:
                     if channel == 1:
-                        pattern_image = cv2.cvtColor(
-                            np.uint8(pattern_image), cv2.COLOR_BGR2GRAY
-                        )
+                        pattern_image = cv2.cvtColor(np.uint8(pattern_image), cv2.COLOR_BGR2GRAY)
 
-                pattern_image = cv2.resize(
-                    pattern_image, (dim_conv, dim_conv), interpolation=cv2.INTER_AREA
-                )
+                pattern_image = cv2.resize(pattern_image, (dim_conv, dim_conv), interpolation=cv2.INTER_AREA)
                 pattern_images.append(img_to_array(pattern_image))
 
                 labels.append(label)
 
                 amount += 1
                 if amount % 10000 == 0:
                     print("The augmented example amount: " + str(amount))
@@ -620,17 +551,15 @@
                             filters,
                             kernel_size=(3, 3),
                             padding="same",
                             activation="relu",
                         )(x)
                         x = BatchNormalization()(x)
                 else:
-                    x = Conv2D(
-                        filters, kernel_size=(3, 3), padding="same", activation="relu"
-                    )(x)
+                    x = Conv2D(filters, kernel_size=(3, 3), padding="same", activation="relu")(x)
                     x = BatchNormalization()(x)
             x = MaxPooling2D(pool_size=(2, 2))(x)
             filters = int(filters * 2)
 
         x = Flatten()(x)
 
         if with_classifier is False:
@@ -741,17 +670,15 @@
         else:
             x = Activation("relu")(x)
 
             x = Conv2D(int(filters * 4), (1, 1), strides=(1, 1))(x)
             x = BatchNormalization()(x)
 
             if block is False:
-                shortcut = Conv2D(filters * 4, (1, 1), strides=(strides, strides))(
-                    shortcut
-                )
+                shortcut = Conv2D(filters * 4, (1, 1), strides=(strides, strides))(shortcut)
                 shortcut = BatchNormalization()(shortcut)
 
         x = Add()([x, shortcut])
         x = Activation("relu")(x)
 
         return x
 
@@ -770,29 +697,25 @@
 
         x = TimeDistributed(ZeroPadding2D((1, 1)))(x)
         x = TimeDistributed(Conv2D(filters, (3, 3), strides=(1, 1)))(x)
         x = TimeDistributed(BatchNormalization())(x)
 
         if basic is True:
             if block is False:
-                shortcut = TimeDistributed(
-                    Conv2D(filters, (1, 1), strides=(strides, strides))
-                )(shortcut)
+                shortcut = TimeDistributed(Conv2D(filters, (1, 1), strides=(strides, strides)))(shortcut)
                 shortcut = TimeDistributed(BatchNormalization())(shortcut)
 
         else:
             x = TimeDistributed(Activation("relu"))(x)
 
             x = TimeDistributed(Conv2D(int(filters * 4), (1, 1), strides=(1, 1)))(x)
             x = TimeDistributed(BatchNormalization())(x)
 
             if block is False:
-                shortcut = TimeDistributed(
-                    Conv2D(int(filters * 4), (1, 1), strides=(strides, strides))
-                )(shortcut)
+                shortcut = TimeDistributed(Conv2D(int(filters * 4), (1, 1), strides=(strides, strides)))(shortcut)
                 shortcut = TimeDistributed(BatchNormalization())(shortcut)
 
         x = Add()([x, shortcut])
         x = TimeDistributed(Activation("relu"))(x)
 
         return x
 
@@ -813,21 +736,17 @@
             layers = [3, 4, 6, 3]
             basic = False
 
         for i in layers:
             for n in range(i):
                 if n == 0:
                     if layers.index(i) == 0:
-                        x = self.res_block(
-                            x, filters, strides=1, block=False, basic=basic
-                        )
+                        x = self.res_block(x, filters, strides=1, block=False, basic=basic)
                     else:
-                        x = self.res_block(
-                            x, filters, strides=2, block=False, basic=basic
-                        )
+                        x = self.res_block(x, filters, strides=2, block=False, basic=basic)
                 else:
                     x = self.res_block(x, filters, strides=1, block=True, basic=basic)
             filters = int(filters * 2)
 
         x = AveragePooling2D((2, 2))(x)
         x = Flatten()(x)
 
@@ -841,17 +760,15 @@
             else:
                 x = Dense(classes, activation="softmax")(x)
 
             model = Model(inputs=inputs, outputs=x)
 
             return model
 
-    def simple_tresnet(
-        self, inputs, filters, classes=3, level=5, with_classifier=False
-    ):
+    def simple_tresnet(self, inputs, filters, classes=3, level=5, with_classifier=False):
         x = TimeDistributed(ZeroPadding2D((3, 3)))(inputs)
         x = TimeDistributed(Conv2D(filters, (5, 5), strides=(2, 2)))(x)
         x = TimeDistributed(BatchNormalization())(x)
         x = TimeDistributed(Activation("relu"))(x)
         x = TimeDistributed(MaxPooling2D((3, 3), strides=(2, 2)))(x)
 
         if level < 6:
@@ -864,21 +781,17 @@
             layers = [3, 4, 6, 3]
             basic = False
 
         for i in layers:
             for n in range(i):
                 if n == 0:
                     if layers.index(i) == 0:
-                        x = self.tres_block(
-                            x, filters, strides=1, block=False, basic=basic
-                        )
+                        x = self.tres_block(x, filters, strides=1, block=False, basic=basic)
                     else:
-                        x = self.tres_block(
-                            x, filters, strides=2, block=False, basic=basic
-                        )
+                        x = self.tres_block(x, filters, strides=2, block=False, basic=basic)
                 else:
                     x = self.tres_block(x, filters, strides=1, block=True, basic=basic)
             filters = int(filters * 2)
 
         x = TimeDistributed(AveragePooling2D((2, 2)))(x)
         x = TimeDistributed(Flatten())(x)
 
@@ -971,17 +884,15 @@
         outputs = BatchNormalization()(outputs)
         outputs = Dropout(0.5)(outputs)
         if classes == 2:
             predictions = Dense(1, activation="sigmoid")(outputs)
         else:
             predictions = Dense(classes, activation="softmax")(outputs)
 
-        model = Model(
-            inputs=[animation_inputs, pattern_image_inputs], outputs=predictions
-        )
+        model = Model(inputs=[animation_inputs, pattern_image_inputs], outputs=predictions)
 
         return model
 
     def train_pattern_recognizer(
         self,
         data_path,
         model_path,
@@ -1001,18 +912,15 @@
         filters = 8
 
         for i in range(round(dim / 60)):
             filters = min(int(filters * 2), 64)
 
         inputs = Input(shape=(dim, dim, channel))
 
-        print(
-            "Training the Categorizer w/ only Pattern Recognizer using the behavior examples in: "
-            + str(data_path)
-        )
+        print("Training the Categorizer w/ only Pattern Recognizer using the behavior examples in: " + str(data_path))
 
         files = [i for i in os.listdir(data_path) if i.endswith(self.extension_image)]
 
         path_files = []
         labels = []
 
         for i in files:
@@ -1051,26 +959,20 @@
             "inner_code": int(inner_code),
             "std": int(std),
             "background_free": int(background_code),
             "behavior_kind": int(behavior_mode),
             "social_distance": int(social_distance),
         }
         pd_parameters = pd.DataFrame.from_dict(parameters)
-        pd_parameters.to_csv(
-            os.path.join(model_path, "model_parameters.txt"), index=False
-        )
+        pd_parameters.to_csv(os.path.join(model_path, "model_parameters.txt"), index=False)
 
-        (train_files, test_files, y1, y2) = train_test_split(
-            path_files, labels, test_size=0.2, stratify=labels
-        )
+        (train_files, test_files, y1, y2) = train_test_split(path_files, labels, test_size=0.2, stratify=labels)
 
         print("Perform augmentation for the behavior examples...")
-        print(
-            "This might take hours or days, depending on the capacity of your computer."
-        )
+        print("This might take hours or days, depending on the capacity of your computer.")
         print(datetime.datetime.now())
 
         print("Start to augment training examples...")
         _, trainX, trainY = self.build_data(
             train_files,
             dim_tconv=0,
             dim_conv=dim,
@@ -1272,18 +1174,15 @@
         filters = 8
 
         for i in range(round(dim / 60)):
             filters = min(int(filters * 2), 64)
 
         inputs = Input(shape=(time_step, dim, dim, channel))
 
-        print(
-            "Training the Categorizer w/o Pattern Recognizer using the behavior examples in: "
-            + str(data_path)
-        )
+        print("Training the Categorizer w/o Pattern Recognizer using the behavior examples in: " + str(data_path))
 
         files = [i for i in os.listdir(data_path) if i.endswith(self.extension_video)]
 
         path_files = []
         labels = []
 
         for i in files:
@@ -1318,26 +1217,20 @@
             "inner_code": int(inner_code),
             "std": int(std),
             "background_free": int(background_code),
             "behavior_kind": int(behavior_mode),
             "social_distance": int(social_distance),
         }
         pd_parameters = pd.DataFrame.from_dict(parameters)
-        pd_parameters.to_csv(
-            os.path.join(model_path, "model_parameters.txt"), index=False
-        )
+        pd_parameters.to_csv(os.path.join(model_path, "model_parameters.txt"), index=False)
 
-        (train_files, test_files, y1, y2) = train_test_split(
-            path_files, labels, test_size=0.2, stratify=labels
-        )
+        (train_files, test_files, y1, y2) = train_test_split(path_files, labels, test_size=0.2, stratify=labels)
 
         print("Perform augmentation for the behavior examples...")
-        print(
-            "This might take hours or days, depending on the capacity of your computer."
-        )
+        print("This might take hours or days, depending on the capacity of your computer.")
         print(datetime.datetime.now())
 
         print("Start to augment training examples...")
         trainX, _, trainY = self.build_data(
             train_files,
             dim_tconv=dim,
             dim_conv=dim,
@@ -1583,26 +1476,20 @@
             "inner_code": int(inner_code),
             "std": int(std),
             "background_free": int(background_code),
             "behavior_kind": int(behavior_mode),
             "social_distance": int(social_distance),
         }
         pd_parameters = pd.DataFrame.from_dict(parameters)
-        pd_parameters.to_csv(
-            os.path.join(model_path, "model_parameters.txt"), index=False
-        )
+        pd_parameters.to_csv(os.path.join(model_path, "model_parameters.txt"), index=False)
 
-        (train_files, test_files, y1, y2) = train_test_split(
-            path_files, labels, test_size=0.2, stratify=labels
-        )
+        (train_files, test_files, y1, y2) = train_test_split(path_files, labels, test_size=0.2, stratify=labels)
 
         print("Perform augmentation for the behavior examples...")
-        print(
-            "This might take hours or days, depending on the capacity of your computer."
-        )
+        print("This might take hours or days, depending on the capacity of your computer.")
         print(datetime.datetime.now())
 
         print("Start to augment training examples...")
         train_animations, train_pattern_images, trainY = self.build_data(
             train_files,
             dim_tconv=dim_tconv,
             dim_conv=dim_conv,
@@ -1642,27 +1529,17 @@
             train_animations = tf.convert_to_tensor(train_animations)
             train_pattern_images = tf.convert_to_tensor(train_pattern_images)
             trainY = tf.convert_to_tensor(trainY)
             test_animations_tensor = tf.convert_to_tensor(test_animations)
             test_pattern_images_tensor = tf.convert_to_tensor(test_pattern_images)
             testY_tensor = tf.convert_to_tensor(testY)
 
-        print(
-            "Training example shape : "
-            + str(train_animations.shape)
-            + ", "
-            + str(train_pattern_images.shape)
-        )
+        print("Training example shape : " + str(train_animations.shape) + ", " + str(train_pattern_images.shape))
         print("Training label shape : " + str(trainY.shape))
-        print(
-            "Validation example shape : "
-            + str(test_animations.shape)
-            + ", "
-            + str(test_pattern_images.shape)
-        )
+        print("Validation example shape : " + str(test_animations.shape) + ", " + str(test_pattern_images.shape))
         print("Validation label shape : " + str(testY.shape))
         print(datetime.datetime.now())
 
         if train_animations.shape[0] < 5000:
             batch_size = 8
         elif train_animations.shape[0] < 50000:
             batch_size = 16
@@ -1730,17 +1607,15 @@
             callbacks=[cp, es, rl],
         )
 
         model.save(model_path)
         print("Trained Categorizer saved in: " + str(model_path))
 
         try:
-            predictions = model.predict(
-                [test_animations, test_pattern_images], batch_size=batch_size
-            )
+            predictions = model.predict([test_animations, test_pattern_images], batch_size=batch_size)
 
             if len(self.classnames) == 2:
                 print(
                     classification_report(
                         testY.argmax(axis=1),
                         predictions.argmax(axis=1),
                         target_names=[self.classnames[0]],
@@ -1853,66 +1728,41 @@
         elif behavior_mode == 2:
             print(
                 "The behavior mode of the Categorizer: Interactive advanced (Social distance "
                 + str(parameters["social_distance"][0])
                 + ")."
             )
         else:
-            print(
-                "The behavior mode of the Categorizer: Static images (non-interactive)."
-            )
+            print("The behavior mode of the Categorizer: Static images (non-interactive).")
         length = int(parameters["time_step"][0])
-        print(
-            "The length of a behavior example in the Categorizer: "
-            + str(length)
-            + " frames."
-        )
+        print("The length of a behavior example in the Categorizer: " + str(length) + " frames.")
         if int(parameters["inner_code"][0]) == 0:
-            print(
-                "The Categorizer includes body parts in analysis with STD = "
-                + str(parameters["std"][0])
-                + "."
-            )
+            print("The Categorizer includes body parts in analysis with STD = " + str(parameters["std"][0]) + ".")
         else:
             print("The Categorizer does not include body parts in analysis.")
         if int(parameters["background_free"][0]) == 0:
             print("The Categorizer does not include background in analysis.")
         else:
             print("The Categorizer includes background in analysis.")
         classnames = list(parameters["classnames"])
         print("Behavior names in the Categorizer: " + str(classnames))
-        behaviornames = [
-            i
-            for i in os.listdir(groundtruth_path)
-            if os.path.isdir(os.path.join(groundtruth_path, i))
-        ]
+        behaviornames = [i for i in os.listdir(groundtruth_path) if os.path.isdir(os.path.join(groundtruth_path, i))]
         incorrect_behaviors = list(set(behaviornames) - set(classnames))
         incorrect_classes = list(set(classnames) - set(behaviornames))
         if len(incorrect_behaviors) > 0:
-            print(
-                "Mismatched behavior names in testing examples: "
-                + str(incorrect_behaviors)
-            )
+            print("Mismatched behavior names in testing examples: " + str(incorrect_behaviors))
         if len(incorrect_classes) > 0:
             print("Unused behavior names in the Categorizer: " + str(incorrect_classes))
 
         if len(incorrect_behaviors) == 0 and len(incorrect_classes) == 0:
             for behavior in behaviornames:
                 if network != 0:
-                    filenames = [
-                        i
-                        for i in os.listdir(os.path.join(groundtruth_path, behavior))
-                        if i.endswith(".avi")
-                    ]
+                    filenames = [i for i in os.listdir(os.path.join(groundtruth_path, behavior)) if i.endswith(".avi")]
                 else:
-                    filenames = [
-                        i
-                        for i in os.listdir(os.path.join(groundtruth_path, behavior))
-                        if i.endswith(".jpg")
-                    ]
+                    filenames = [i for i in os.listdir(os.path.join(groundtruth_path, behavior)) if i.endswith(".jpg")]
 
                 for i in filenames:
                     if network != 0:
                         path_to_animation = os.path.join(groundtruth_path, behavior, i)
 
                         capture = cv2.VideoCapture(path_to_animation)
                         animation = deque()
@@ -1923,37 +1773,30 @@
                             if frame is None:
                                 break
                             frames.append(frame)
 
                         capture.release()
 
                         for frame in frames:
-                            frame = np.uint8(
-                                exposure.rescale_intensity(frame, out_range=(0, 255))
-                            )
+                            frame = np.uint8(exposure.rescale_intensity(frame, out_range=(0, 255)))
                             if channel == 1:
-                                frame = cv2.cvtColor(
-                                    np.uint8(frame), cv2.COLOR_BGR2GRAY
-                                )
+                                frame = cv2.cvtColor(np.uint8(frame), cv2.COLOR_BGR2GRAY)
                             frame = cv2.resize(
                                 frame,
                                 (dim_tconv, dim_tconv),
                                 interpolation=cv2.INTER_AREA,
                             )
                             frame = img_to_array(frame)
                             animation.append(frame)
 
                         animations.append(np.array(animation))
 
                     if network != 1:
                         path_to_pattern_image = (
-                            os.path.splitext(
-                                os.path.join(groundtruth_path, behavior, i)
-                            )[0]
-                            + ".jpg"
+                            os.path.splitext(os.path.join(groundtruth_path, behavior, i))[0] + ".jpg"
                         )
                         pattern_image = cv2.imread(path_to_pattern_image)
                         pattern_image = cv2.resize(
                             pattern_image,
                             (dim_conv, dim_conv),
                             interpolation=cv2.INTER_AREA,
                         )
@@ -1972,19 +1815,15 @@
             if network == 0:
                 predictions = model.predict(pattern_images, batch_size=32)
             elif network == 1:
                 predictions = model.predict(animations, batch_size=32)
             else:
                 predictions = model.predict([animations, pattern_images], batch_size=32)
 
-            print(
-                classification_report(
-                    labels, predictions.argmax(axis=1), target_names=classnames
-                )
-            )
+            print(classification_report(labels, predictions.argmax(axis=1), target_names=classnames))
             report = classification_report(
                 labels,
                 predictions.argmax(axis=1),
                 target_names=classnames,
                 output_dict=True,
             )
```

### Comparing `labgym-2.3.5/LabGym/detectors/__init__.py` & `labgym-2.4.0/LabGym/detectors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
```

### Comparing `labgym-2.3.5/LabGym/gui/__init__.py` & `labgym-2.4.0/LabGym/gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
```

### Comparing `labgym-2.3.5/LabGym/gui/analysis/__init__.py` & `labgym-2.4.0/LabGym/gui/analysis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
```

### Comparing `labgym-2.3.5/LabGym/gui/analysis/analysis_module.py` & `labgym-2.4.0/LabGym/gui/analysis/analysis_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 from ..utils import LabGymWindow
 from .analyze_behaviors import AnalyzeBehaviors
 from .mine_results import MineResults
 
 
 class AnalysisModule(LabGymWindow):
     def __init__(self):
```

### Comparing `labgym-2.3.5/LabGym/gui/analysis/analyze_behaviors.py` & `labgym-2.4.0/LabGym/gui/analysis/analyze_behaviors.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 USA
 
 Email: bingye@umich.edu
 """
 
 import json
 import os
-from pathlib import Path
 
 import matplotlib as mpl
 import pandas as pd
 import torch
 import wx
 
 from LabGym.analyzebehaviors import AnalyzeAnimal
 from LabGym.analyzebehaviorsdetector import AnalyzeAnimalDetector
+from LabGym.categorizers import CATEGORIZER_FOLDER, get_categorizer_names
+from LabGym.detector import Detector, get_detector_names
 from LabGym.gui.utils import WX_IMAGE_WILDCARD, WX_VIDEO_WILDCARD, LabGymWindow
 from LabGym.tools import plot_evnets
 
-the_absolute_current_path = str(Path(__file__).resolve().parent.parent.parent)
-
 
 class ColorPicker(wx.Dialog):
     def __init__(self, parent, title, name_and_color):
         super(ColorPicker, self).__init__(parent=None, title=title, size=(200, 200))
 
         self.name_and_color = name_and_color
         name = self.name_and_color[0]
@@ -57,23 +56,19 @@
 
 
 class AnalyzeBehaviors(LabGymWindow):
     def __init__(self):
         super().__init__(title="Analyze Behaviors", size=(1000, 600))
         self.behavior_mode = 0
         self.use_detector = False
-        self.detector_path = None
         self.path_to_detector = None
         self.detector_batch = 1
         self.detection_threshold = 0
         self.animal_kinds = []
-        self.background_path = (
-            None  # if not None, will load background images from path
-        )
-        self.model_path = None  # the parent path of the Categorizers
+        self.background_path = None  # if not None, will load background images from path
         self.path_to_categorizer = None
         self.path_to_videos = None
         self.result_path = None
         self.framewidth = None
         self.delta = 10000
         self.decode_animalnumber = False
         self.animal_number = None
@@ -85,15 +80,17 @@
         self.ex_start = 0
         self.ex_end = None
         self.behaviornames_and_colors = {}
         self.dim_tconv = 8
         self.dim_conv = 8
         self.channel = 1
         self.length = 15
-        self.animal_vs_bg = 0  # 0: animals birghter than the background; 1: animals darker than the background; 2: hard to tell
+        self.animal_vs_bg = (
+            0  # 0: animals birghter than the background; 1: animals darker than the background; 2: hard to tell
+        )
         self.stable_illumination = True
         self.animation_analyzer = True
         self.animal_to_include = []
         self.behavior_to_include = ["all"]  # behaviors for annotation and analyze
         self.parameter_to_analyze = []
         self.include_bodyparts = False
         self.std = 0
@@ -130,37 +127,31 @@
         self.add_module(
             button_label="Select a folder to store\nthe analysis results",
             button_handler=self.select_outpath,
             tool_tip='If analyzing videos, will create a subfolder for each video in the selected folder. Each subfolder is named after the file name of the video and stores the detailed analysis results for this video. For "Static images" mode, all results will be in this folder. See Extended Guide for details.',
             text=self.text_outputfolder,
         )
 
-        self.text_detection = self.module_text(
-            "Default: Background subtraction-based method."
-        )
+        self.text_detection = self.module_text("Default: Background subtraction-based method.")
         self.add_module(
             button_label="Specify the method to\ndetect animals or objects",
             button_handler=self.select_method,
             tool_tip="Background subtraction-based method is accurate and fast but requires static background and stable illumination in videos; Detectors-based method is accurate and versatile in any recording settings but is slow. See Extended Guide for details.",
             text=self.text_detection,
         )
 
-        self.text_startanalyze = self.module_text(
-            "Default: at the beginning of the video(s)."
-        )
+        self.text_startanalyze = self.module_text("Default: at the beginning of the video(s).")
         self.add_module(
             button_label="Specify when the analysis\nshould begin (unit: second)",
             button_handler=self.specify_timing,
             tool_tip='Enter a beginning time point for all videos in one analysis batch or use "Decode from filenames" to let LabGym decode the different beginning time for different videos. See Extended Guide for details.',
             text=self.text_startanalyze,
         )
 
-        self.text_duration = self.module_text(
-            "Default: from the specified start time to the end of a video"
-        )
+        self.text_duration = self.module_text("Default: from the specified start time to the end of a video")
         self.add_module(
             button_label="Specify the analysis duration\n(unit: second)",
             button_handler=self.input_duration,
             tool_tip="The duration is the same for all the videos in a same analysis batch.",
             text=self.text_duration,
         )
 
@@ -168,17 +159,15 @@
         self.add_module(
             button_label="Specify the number of animals\nin a video",
             button_handler=self.specify_animalnumber,
             tool_tip='Enter a number for all videos in one analysis batch or use "Decode from filenames" to let LabGym decode the different animal number for different videos. See Extended Guide for details.',
             text=self.text_animalnumber,
         )
 
-        self.text_selectbehaviors = self.module_text(
-            "Default: No Categorizer selected, no behavior selected."
-        )
+        self.text_selectbehaviors = self.module_text("Default: No Categorizer selected, no behavior selected.")
         self.add_module(
             button_label="Select the behaviors for\nannotations and plots",
             button_handler=self.select_behaviors,
             tool_tip="The behavior categories are determined by the selected Categorizer. Select which behaviors to show in the annotated videos / images and the raster plot (only for videos). See Extended Guide for details.",
             text=self.text_selectbehaviors,
         )
 
@@ -195,79 +184,56 @@
             handler=self.analyze_behaviors,
             tool_tip='If analyzing videos, will output a raster plot for all behavior events in all videos, an annotated video copy for each video, various spreadsheets storing quantification results for each selected behavior parameter. For "Static images" mode, will output annotated image copies and spreadsheet storing behavior count and probability.',
         )
 
         self.display_window()
 
     def select_categorizer(self, event):
-        if self.model_path is None:
-            self.model_path = os.path.join(the_absolute_current_path, "models")
-
-        categorizers = [
-            i
-            for i in os.listdir(self.model_path)
-            if os.path.isdir(os.path.join(self.model_path, i))
-        ]
-        if "__pycache__" in categorizers:
-            categorizers.remove("__pycache__")
-        if "__init__" in categorizers:
-            categorizers.remove("__init__")
-        if "__init__.py" in categorizers:
-            categorizers.remove("__init__.py")
+        categorizers = get_categorizer_names()
         categorizers.sort()
-        if (
-            "No behavior classification, just track animals and quantify motion kinematics"
-            not in categorizers
-        ):
-            categorizers.append(
-                "No behavior classification, just track animals and quantify motion kinematics"
-            )
+        if "No behavior classification, just track animals and quantify motion kinematics" not in categorizers:
+            categorizers.append("No behavior classification, just track animals and quantify motion kinematics")
         if "Choose a new directory of the Categorizer" not in categorizers:
             categorizers.append("Choose a new directory of the Categorizer")
 
         dialog = wx.SingleChoiceDialog(
             self,
             message="Select a Categorizer for behavior classification",
             caption="Select a Categorizer",
             choices=categorizers,
         )
 
         if dialog.ShowModal() == wx.ID_OK:
             categorizer = dialog.GetStringSelection()
             if categorizer == "Choose a new directory of the Categorizer":
-                dialog1 = wx.DirDialog(
-                    self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-                )
+                dialog1 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
                 if dialog1.ShowModal() == wx.ID_OK:
                     self.path_to_categorizer = dialog1.GetPaths()
                 dialog1.Destroy()
                 dialog1 = wx.NumberEntryDialog(
                     self,
                     "Enter the Categorizer's uncertainty level (0~100%)",
                     "If probability difference between\n1st- and 2nd-likely behaviors\nis less than uncertainty,\nclassfication outputs an 'NA'. Enter 0 if don't know how to set.",
                     "Uncertainty level",
                     0,
                     0,
                     100,
                 )
-                if dialog1.ShowModal() == wx.ID_OK:
+                if dialog1.ShowModal() != wx.ID_OK:
+                    dialog1.Destroy()
+                    return
+                else:
                     uncertain = dialog1.GetValue()
                     self.uncertain = uncertain / 100
-                dialog1.Destroy()
+                    dialog1.Destroy()
+
                 self.text_selectcategorizer.SetLabel(
-                    "The path to the Categorizer is: "
-                    + self.path_to_categorizer
-                    + " with uncertainty of "
-                    + str(uncertain)
-                    + "%."
+                    f"The path to the Categorizer is {self.path_to_categorizer} with uncertainty of {uncertain} %."
                 )
-            elif (
-                categorizer
-                == "No behavior classification, just track animals and quantify motion kinematics"
-            ):
+            elif categorizer == "No behavior classification, just track animals and quantify motion kinematics":
                 self.path_to_categorizer = None
                 dialog1 = wx.NumberEntryDialog(
                     self,
                     "Specify a time window used for measuring\nmotion kinematics of the tracked animals",
                     "Enter the number of\nframes (minimum=3):",
                     "Time window for calculating kinematics",
                     15,
@@ -284,42 +250,34 @@
                     + str(self.length)
                     + " frames."
                 )
                 self.text_selectbehaviors.SetLabel(
                     "No behavior classification. Just track animals and quantify motion kinematics."
                 )
             else:
-                self.path_to_categorizer = os.path.join(self.model_path, categorizer)
+                self.path_to_categorizer = os.path.join(str(CATEGORIZER_FOLDER), categorizer)
                 dialog1 = wx.NumberEntryDialog(
                     self,
                     "Enter the Categorizer's uncertainty level (0~100%)",
                     "If probability difference between\n1st- and 2nd-likely behaviors\nis less than uncertainty,\nclassfication outputs an 'NA'.",
                     "Uncertainty level",
                     0,
                     0,
                     100,
                 )
                 if dialog1.ShowModal() == wx.ID_OK:
                     uncertain = dialog1.GetValue()
                     self.uncertain = uncertain / 100
                     self.text_selectcategorizer.SetLabel(
-                        "Categorizer: "
-                        + categorizer
-                        + " with uncertainty of "
-                        + str(uncertain)
-                        + "%."
+                        "Categorizer: " + categorizer + " with uncertainty of " + str(uncertain) + "%."
                     )
-            self.text_selectbehaviors.SetLabel(
-                "All the behaviors in the selected Categorizer with default colors."
-            )
+            self.text_selectbehaviors.SetLabel("All the behaviors in the selected Categorizer with default colors.")
 
             if self.path_to_categorizer is not None:
-                parameters = pd.read_csv(
-                    os.path.join(self.path_to_categorizer, "model_parameters.txt")
-                )
+                parameters = pd.read_csv(os.path.join(self.path_to_categorizer, "model_parameters.txt"))
                 complete_colors = list(mpl.colors.cnames.values())
                 colors = []
                 for c in complete_colors:
                     colors.append(["#ffffff", c])
                 self.behaviornames_and_colors = {}
 
                 for behavior_name in list(parameters["classnames"]):
@@ -386,17 +344,15 @@
 
     def select_videos(self, event):
         if self.behavior_mode == 3:
             wildcard = WX_IMAGE_WILDCARD
         else:
             wildcard = WX_VIDEO_WILDCARD
 
-        dialog = wx.FileDialog(
-            self, "Select video(s) / image(s)", "", "", wildcard, style=wx.FD_MULTIPLE
-        )
+        dialog = wx.FileDialog(self, "Select video(s) / image(s)", "", "", wildcard, style=wx.FD_MULTIPLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.path_to_videos = dialog.GetPaths()
             self.path_to_videos.sort()
             path = os.path.dirname(self.path_to_videos[0])
             dialog1 = wx.MessageDialog(
                 self,
                 'Proportional resize the video frames / images? Reducing frame / image size\nis highly recommended. But select "No" if dont know what it is.',
@@ -448,17 +404,15 @@
             dialog1.Destroy()
         dialog.Destroy()
 
     def select_outpath(self, event):
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = dialog.GetPath()
-            self.text_outputfolder.SetLabel(
-                "Results will be in: " + self.result_path + "."
-            )
+            self.text_outputfolder.SetLabel("Results will be in: " + self.result_path + ".")
         dialog.Destroy()
 
     def select_method(self, event):
         if self.behavior_mode <= 1:
             methods = [
                 "Subtract background (fast but requires static background & stable illumination)",
                 "Use trained Detectors (versatile but slow)",
@@ -472,18 +426,15 @@
             caption="Detection methods",
             choices=methods,
         )
 
         if dialog.ShowModal() == wx.ID_OK:
             method = dialog.GetStringSelection()
 
-            if (
-                method
-                == "Subtract background (fast but requires static background & stable illumination)"
-            ):
+            if method == "Subtract background (fast but requires static background & stable illumination)":
                 self.use_detector = False
 
                 contrasts = [
                     "Animal brighter than background",
                     "Animal darker than background",
                     "Hard to tell",
                 ]
@@ -505,17 +456,15 @@
                     dialog2 = wx.MessageDialog(
                         self,
                         'Load an existing background from a folder?\nSelect "No" if dont know what it is.',
                         "(Optional) load existing background?",
                         wx.YES_NO | wx.ICON_QUESTION,
                     )
                     if dialog2.ShowModal() == wx.ID_YES:
-                        dialog3 = wx.DirDialog(
-                            self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-                        )
+                        dialog3 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
                         if dialog3.ShowModal() == wx.ID_OK:
                             self.background_path = dialog3.GetPath()
                         dialog3.Destroy()
                     else:
                         self.background_path = None
                         if self.animal_vs_bg != 2:
                             dialog3 = wx.MessageDialog(
@@ -541,35 +490,29 @@
                             self,
                             message="Specify the time window for background extraction",
                             caption="Time window for background extraction",
                             choices=ex_methods,
                         )
                         if dialog2.ShowModal() == wx.ID_OK:
                             ex_method = dialog2.GetStringSelection()
-                            if (
-                                ex_method
-                                == "Use the entire duration (default but NOT recommended)"
-                            ):
+                            if ex_method == "Use the entire duration (default but NOT recommended)":
                                 self.decode_extraction = False
                                 if self.animal_vs_bg == 0:
                                     self.text_detection.SetLabel(
                                         "Background subtraction: animal brighter, using the entire duration."
                                     )
                                 elif self.animal_vs_bg == 1:
                                     self.text_detection.SetLabel(
                                         "Background subtraction: animal darker, using the entire duration."
                                     )
                                 else:
                                     self.text_detection.SetLabel(
                                         "Background subtraction: animal partially brighter/darker, using the entire duration."
                                     )
-                            elif (
-                                ex_method
-                                == 'Decode from filenames: "_xst_" and "_xet_"'
-                            ):
+                            elif ex_method == 'Decode from filenames: "_xst_" and "_xet_"':
                                 self.decode_extraction = True
                                 if self.animal_vs_bg == 0:
                                     self.text_detection.SetLabel(
                                         'Background subtraction: animal brighter, using time window decoded from filenames "_xst_" and "_xet_".'
                                     )
                                 elif self.animal_vs_bg == 1:
                                     self.text_detection.SetLabel(
@@ -655,68 +598,47 @@
                         dialog2.Destroy()
 
                 dialog1.Destroy()
 
             else:
                 self.use_detector = True
                 self.animal_number = {}
-                self.detector_path = os.path.join(
-                    the_absolute_current_path, "detectors"
-                )
 
-                detectors = [
-                    i
-                    for i in os.listdir(self.detector_path)
-                    if os.path.isdir(os.path.join(self.detector_path, i))
-                ]
-                if "__pycache__" in detectors:
-                    detectors.remove("__pycache__")
-                if "__init__" in detectors:
-                    detectors.remove("__init__")
-                if "__init__.py" in detectors:
-                    detectors.remove("__init__.py")
+                detectors = get_detector_names()
                 detectors.sort()
                 if "Choose a new directory of the Detector" not in detectors:
                     detectors.append("Choose a new directory of the Detector")
 
                 dialog1 = wx.SingleChoiceDialog(
                     self,
                     message="Select a Detector for animal detection",
                     caption="Select a Detector",
                     choices=detectors,
                 )
                 if dialog1.ShowModal() == wx.ID_OK:
-                    detector = dialog1.GetStringSelection()
-                    if detector == "Choose a new directory of the Detector":
-                        dialog2 = wx.DirDialog(
-                            self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-                        )
+                    detector_name = dialog1.GetStringSelection()
+                    if detector_name == "Choose a new directory of the Detector":
+                        dialog2 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
                         if dialog2.ShowModal() == wx.ID_OK:
-                            self.path_to_detector = dialog2.GetPaths()
+                            self.detector = Detector(path=dialog2.GetPath())
                         dialog2.Destroy()
                     else:
-                        self.path_to_detector = os.path.join(
-                            self.detector_path, detector
-                        )
-                    with open(
-                        os.path.join(self.path_to_detector, "model_parameters.txt")
-                    ) as f:
+                        self.detector = Detector(name=detector_name)
+                    with open(self.detector.path / "model_parameters.txt") as f:
                         model_parameters = f.read()
                     animal_names = json.loads(model_parameters)["animal_names"]
                     if len(animal_names) > 1:
                         dialog2 = wx.MultiChoiceDialog(
                             self,
                             message="Specify which animals/objects involved in analysis",
                             caption="Animal/Object kind",
                             choices=animal_names,
                         )
                         if dialog2.ShowModal() == wx.ID_OK:
-                            self.animal_kinds = [
-                                animal_names[i] for i in dialog2.GetSelections()
-                            ]
+                            self.animal_kinds = [animal_names[i] for i in dialog2.GetSelections()]
                         else:
                             self.animal_kinds = animal_names
                         dialog2.Destroy()
                     else:
                         self.animal_kinds = animal_names
                     if self.behavior_mode >= 3:
                         dialog2 = wx.NumberEntryDialog(
@@ -729,15 +651,15 @@
                             100,
                         )
                         if dialog2.ShowModal() == wx.ID_OK:
                             detection_threshold = dialog2.GetValue()
                             self.detection_threshold = detection_threshold / 100
                         self.text_detection.SetLabel(
                             "Detector: "
-                            + detector
+                            + detector_name
                             + " (detection threshold: "
                             + str(detection_threshold)
                             + "%); The animals/objects: "
                             + str(self.animal_kinds)
                             + "."
                         )
                         dialog2.Destroy()
@@ -748,20 +670,15 @@
                             "The number of "
                             + str(self.animal_kinds)
                             + " is: "
                             + str(list(self.animal_number.values()))
                             + "."
                         )
                         self.text_detection.SetLabel(
-                            "Detector: "
-                            + detector
-                            + "; "
-                            + "The animals/objects: "
-                            + str(self.animal_kinds)
-                            + "."
+                            "Detector: " + detector_name + "; " + "The animals/objects: " + str(self.animal_kinds) + "."
                         )
                 dialog1.Destroy()
 
                 if self.behavior_mode < 3:
                     if torch.cuda.is_available():
                         dialog1 = wx.NumberEntryDialog(
                             self,
@@ -855,17 +772,15 @@
                         0,
                         100000000000000,
                     )
                     if dialog2.ShowModal() == wx.ID_OK:
                         self.t = float(dialog2.GetValue())
                         if self.t < 0:
                             self.t = 0
-                        self.text_startanalyze.SetLabel(
-                            "Analysis will begin at the: " + str(self.t) + " second."
-                        )
+                        self.text_startanalyze.SetLabel("Analysis will begin at the: " + str(self.t) + " second.")
                     dialog2.Destroy()
             dialog.Destroy()
 
     def input_duration(self, event):
         if self.behavior_mode >= 3:
             wx.MessageBox(
                 'No need to specify this since the selected behavior mode is "Static images".',
@@ -882,17 +797,15 @@
                 0,
                 0,
                 100000000000000,
             )
             if dialog.ShowModal() == wx.ID_OK:
                 self.duration = int(dialog.GetValue())
                 if self.duration != 0:
-                    self.text_duration.SetLabel(
-                        "The analysis duration is " + str(self.duration) + " seconds."
-                    )
+                    self.text_duration.SetLabel("The analysis duration is " + str(self.duration) + " seconds.")
                 else:
                     self.text_duration.SetLabel(
                         "The analysis duration is from the specified beginning time to the end of a video."
                     )
             dialog.Destroy()
 
     def specify_animalnumber(self, event):
@@ -925,17 +838,15 @@
                                 "The number of " + str(animal_name) + ": ",
                                 str(animal_name) + " number",
                                 1,
                                 1,
                                 100,
                             )
                             if dialog1.ShowModal() == wx.ID_OK:
-                                self.animal_number[animal_name] = int(
-                                    dialog1.GetValue()
-                                )
+                                self.animal_number[animal_name] = int(dialog1.GetValue())
                             else:
                                 self.animal_number[animal_name] = 1
                             dialog1.Destroy()
                         self.text_animalnumber.SetLabel(
                             "The number of "
                             + str(self.animal_kinds)
                             + " is: "
@@ -953,17 +864,15 @@
                             100,
                         )
                         if dialog1.ShowModal() == wx.ID_OK:
                             self.animal_number = int(dialog1.GetValue())
                         else:
                             self.animal_number = 1
                         self.text_animalnumber.SetLabel(
-                            "The total number of animals in a video is "
-                            + str(self.animal_number)
-                            + "."
+                            "The total number of animals in a video is " + str(self.animal_number) + "."
                         )
                         dialog1.Destroy()
                 else:
                     self.decode_animalnumber = True
                     self.text_animalnumber.SetLabel(
                         'Decode from the filenames: the "n" immediately after the letter "n" in _"nn"_.'
                     )
@@ -982,33 +891,30 @@
                 dialog = wx.MultiChoiceDialog(
                     self,
                     message="Specify which animals/objects to annotate",
                     caption="Animal/Object to annotate",
                     choices=self.animal_kinds,
                 )
                 if dialog.ShowModal() == wx.ID_OK:
-                    self.animal_to_include = [
-                        self.animal_kinds[i] for i in dialog.GetSelections()
-                    ]
+                    self.animal_to_include = [self.animal_kinds[i] for i in dialog.GetSelections()]
                 else:
                     self.animal_to_include = self.animal_kinds
                 dialog.Destroy()
             else:
                 self.animal_to_include = self.animal_kinds
 
             dialog = wx.MultiChoiceDialog(
                 self,
                 message="Select behaviors",
                 caption="Behaviors to annotate",
                 choices=list(self.behaviornames_and_colors.keys()),
             )
             if dialog.ShowModal() == wx.ID_OK:
                 self.behavior_to_include = [
-                    list(self.behaviornames_and_colors.keys())[i]
-                    for i in dialog.GetSelections()
+                    list(self.behaviornames_and_colors.keys())[i] for i in dialog.GetSelections()
                 ]
             else:
                 self.behavior_to_include = list(self.behaviornames_and_colors.keys())
             dialog.Destroy()
 
             if len(self.behavior_to_include) == 0:
                 self.behavior_to_include = list(self.behaviornames_and_colors.keys())
@@ -1022,31 +928,24 @@
                     "Individual-specific behaviors?",
                     wx.YES_NO | wx.ICON_QUESTION,
                 )
                 if dialog.ShowModal() == wx.ID_YES:
                     for animal_name in self.animal_kinds:
                         dialog1 = wx.MultiChoiceDialog(
                             self,
-                            message="Select individual-specific behaviors for "
-                            + str(animal_name),
-                            caption="Individual-specific behaviors for "
-                            + str(animal_name),
+                            message="Select individual-specific behaviors for " + str(animal_name),
+                            caption="Individual-specific behaviors for " + str(animal_name),
                             choices=self.behavior_to_include,
                         )
                         if dialog1.ShowModal() == wx.ID_OK:
                             self.specific_behaviors[animal_name] = {}
                             self.correct_ID = True
-                            specific_behaviors = [
-                                self.behavior_to_include[i]
-                                for i in dialog1.GetSelections()
-                            ]
+                            specific_behaviors = [self.behavior_to_include[i] for i in dialog1.GetSelections()]
                             for specific_behavior in specific_behaviors:
-                                self.specific_behaviors[animal_name][
-                                    specific_behavior
-                                ] = None
+                                self.specific_behaviors[animal_name][specific_behavior] = None
                         dialog1.Destroy()
                 else:
                     self.correct_ID = False
                 dialog.Destroy()
 
             complete_colors = list(mpl.colors.cnames.values())
             colors = []
@@ -1075,52 +974,44 @@
                             "#ffffff",
                             new_color,
                         ]
                         names_colors[self.behavior_to_include[n]] = new_color
                     else:
                         if n < len(colors):
                             names_colors[self.behavior_to_include[n]] = colors[n][1]
-                            self.behaviornames_and_colors[
-                                self.behavior_to_include[n]
-                            ] = colors[n]
+                            self.behaviornames_and_colors[self.behavior_to_include[n]] = colors[n]
                     dialog2.Destroy()
                     n += 1
                 if self.correct_ID is True:
                     self.text_selectbehaviors.SetLabel(
                         "Selected: "
                         + str(list(names_colors.keys()))
                         + ". Specific behaviors: "
                         + str(self.specific_behaviors)
                         + "."
                     )
                 else:
-                    self.text_selectbehaviors.SetLabel(
-                        "Selected: " + str(list(names_colors.keys())) + "."
-                    )
+                    self.text_selectbehaviors.SetLabel("Selected: " + str(list(names_colors.keys())) + ".")
             else:
                 for color in colors:
                     index = colors.index(color)
                     if index < len(self.behavior_to_include):
-                        behavior_name = list(self.behaviornames_and_colors.keys())[
-                            index
-                        ]
+                        behavior_name = list(self.behaviornames_and_colors.keys())[index]
                         self.behaviornames_and_colors[behavior_name] = color
                 if self.correct_ID is True:
                     self.text_selectbehaviors.SetLabel(
                         "Selected: "
                         + str(self.behavior_to_include)
                         + " with default colors. Specific behaviors:"
                         + str(self.specific_behaviors)
                         + "."
                     )
                 else:
                     self.text_selectbehaviors.SetLabel(
-                        "Selected: "
-                        + str(self.behavior_to_include)
-                        + " with default colors."
+                        "Selected: " + str(self.behavior_to_include) + " with default colors."
                     )
             dialog.Destroy()
 
             if self.behavior_mode != 3:
                 dialog = wx.MessageDialog(
                     self,
                     "Show legend of behavior names in the annotated video?",
@@ -1164,17 +1055,15 @@
             dialog = wx.MultiChoiceDialog(
                 self,
                 message="Select quantitative measurements",
                 caption="Quantitative measurements",
                 choices=parameters,
             )
             if dialog.ShowModal() == wx.ID_OK:
-                self.parameter_to_analyze = [
-                    parameters[i] for i in dialog.GetSelections()
-                ]
+                self.parameter_to_analyze = [parameters[i] for i in dialog.GetSelections()]
             else:
                 self.parameter_to_analyze = []
             dialog.Destroy()
 
             if len(self.parameter_to_analyze) <= 0:
                 self.parameter_to_analyze = []
                 self.normalize_distance = False
@@ -1186,50 +1075,42 @@
                         "Normalize the distances by the size of an animal? If no, all distances will be output in pixels.",
                         "Normalize the distances?",
                         wx.YES_NO | wx.ICON_QUESTION,
                     )
                     if dialog.ShowModal() == wx.ID_YES:
                         self.normalize_distance = True
                         self.text_selectparameters.SetLabel(
-                            "Selected: "
-                            + str(self.parameter_to_analyze)
-                            + "; with normalization of distance."
+                            "Selected: " + str(self.parameter_to_analyze) + "; with normalization of distance."
                         )
                     else:
                         self.normalize_distance = False
                         self.text_selectparameters.SetLabel(
-                            "Selected: "
-                            + str(self.parameter_to_analyze)
-                            + "; NO normalization of distance."
+                            "Selected: " + str(self.parameter_to_analyze) + "; NO normalization of distance."
                         )
                     dialog.Destroy()
                 else:
                     self.normalize_distance = False
-                    self.text_selectparameters.SetLabel(
-                        "Selected: " + str(self.parameter_to_analyze) + "."
-                    )
+                    self.text_selectparameters.SetLabel("Selected: " + str(self.parameter_to_analyze) + ".")
 
     def analyze_behaviors(self, event):
         if self.path_to_videos is None or self.result_path is None:
-            wx.MessageBox(
-                "No input video(s) / result folder.", "Error", wx.OK | wx.ICON_ERROR
-            )
+            wx.MessageBox("No input video(s) / result folder.", "Error", wx.OK | wx.ICON_ERROR)
 
         else:
             if self.behavior_mode >= 3:
                 if self.path_to_categorizer is None or self.path_to_detector is None:
                     wx.MessageBox(
                         "You need to select a Categorizer / Detector.",
                         "Error",
                         wx.OK | wx.ICON_ERROR,
                     )
                 else:
                     AAD = AnalyzeAnimalDetector()
                     AAD.analyze_images_individuals(
-                        self.path_to_detector,
+                        str(self.detector.path),
                         self.path_to_videos,
                         self.result_path,
                         self.animal_kinds,
                         path_to_categorizer=self.path_to_categorizer,
                         generate=False,
                         animal_to_include=self.animal_to_include,
                         behavior_to_include=self.behavior_to_include,
@@ -1254,26 +1135,22 @@
                     if len(self.animal_to_include) == 0:
                         self.animal_to_include = self.animal_kinds
 
                 if self.path_to_categorizer is None:
                     self.behavior_to_include = []
                 else:
                     if self.behavior_to_include[0] == "all":
-                        self.behavior_to_include = list(
-                            self.behaviornames_and_colors.keys()
-                        )
+                        self.behavior_to_include = list(self.behaviornames_and_colors.keys())
 
                 for i in self.path_to_videos:
                     filename = os.path.splitext(os.path.basename(i))[0].split("_")
                     if self.decode_animalnumber is True:
                         if self.use_detector is True:
                             self.animal_number = {}
-                            number = [
-                                x[1:] for x in filename if len(x) > 1 and x[0] == "n"
-                            ]
+                            number = [x[1:] for x in filename if len(x) > 1 and x[0] == "n"]
                             for a, animal_name in enumerate(self.animal_kinds):
                                 self.animal_number[animal_name] = int(number[a])
                         else:
                             for x in filename:
                                 if len(x) > 1:
                                     if x[0] == "n":
                                         self.animal_number = int(x[1:])
@@ -1331,22 +1208,18 @@
                             animal_vs_bg=self.animal_vs_bg,
                         )
                         if self.behavior_mode == 0:
                             AA.acquire_information(background_free=self.background_free)
                             AA.craft_data()
                             interact_all = False
                         else:
-                            AA.acquire_information_interact_basic(
-                                background_free=self.background_free
-                            )
+                            AA.acquire_information_interact_basic(background_free=self.background_free)
                             interact_all = True
                         if self.path_to_categorizer is not None:
-                            AA.categorize_behaviors(
-                                self.path_to_categorizer, uncertain=self.uncertain
-                            )
+                            AA.categorize_behaviors(self.path_to_categorizer, uncertain=self.uncertain)
                         AA.annotate_video(
                             self.behavior_to_include,
                             show_legend=self.show_legend,
                             interact_all=interact_all,
                         )
                         AA.export_results(
                             normalize_distance=self.normalize_distance,
@@ -1357,15 +1230,15 @@
                             for n in AA.event_probability:
                                 all_events[len(all_events)] = AA.event_probability[n]
                                 all_lengths.append(len(AA.event_probability[n]))
 
                     else:
                         AAD = AnalyzeAnimalDetector()
                         AAD.prepare_analysis(
-                            self.path_to_detector,
+                            str(self.detector.path),
                             i,
                             self.result_path,
                             self.animal_number,
                             self.animal_kinds,
                             self.behavior_mode,
                             names_and_colors=self.behaviornames_and_colors,
                             framewidth=self.framewidth,
@@ -1384,17 +1257,15 @@
                         AAD.acquire_information(
                             batch_size=self.detector_batch,
                             background_free=self.background_free,
                         )
                         if self.behavior_mode != 1:
                             AAD.craft_data()
                         if self.path_to_categorizer is not None:
-                            AAD.categorize_behaviors(
-                                self.path_to_categorizer, uncertain=self.uncertain
-                            )
+                            AAD.categorize_behaviors(self.path_to_categorizer, uncertain=self.uncertain)
                         if self.correct_ID is True:
                             AAD.correct_identity(self.specific_behaviors)
                         AAD.annotate_video(
                             self.animal_to_include,
                             self.behavior_to_include,
                             show_legend=self.show_legend,
                         )
@@ -1402,27 +1273,23 @@
                             normalize_distance=self.normalize_distance,
                             parameter_to_analyze=self.parameter_to_analyze,
                         )
 
                         if self.path_to_categorizer is not None:
                             for animal_name in self.animal_kinds:
                                 for n in AAD.event_probability[animal_name]:
-                                    all_events[animal_name][
-                                        len(all_events[animal_name])
-                                    ] = AAD.event_probability[animal_name][n]
-                                    all_lengths.append(
-                                        len(AAD.event_probability[animal_name][n])
-                                    )
+                                    all_events[animal_name][len(all_events[animal_name])] = AAD.event_probability[
+                                        animal_name
+                                    ][n]
+                                    all_lengths.append(len(AAD.event_probability[animal_name][n]))
 
                 if self.path_to_categorizer is not None:
                     if self.use_detector is False:
                         for n in all_events:
-                            event_data[len(event_data)] = all_events[n][
-                                : min(all_lengths)
-                            ]
+                            event_data[len(event_data)] = all_events[n][: min(all_lengths)]
                         time_points = AA.all_time[: min(all_lengths)]
                         all_events_df = pd.DataFrame(event_data, index=time_points)
                         all_events_df.to_excel(
                             os.path.join(self.result_path, "all_events.xlsx"),
                             float_format="%.2f",
                             index_label="time/ID",
                         )
@@ -1432,52 +1299,44 @@
                             time_points,
                             self.behaviornames_and_colors,
                             self.behavior_to_include,
                             width=0,
                             height=0,
                         )
                         folders = [
-                            i
-                            for i in os.listdir(self.result_path)
-                            if os.path.isdir(os.path.join(self.result_path, i))
+                            i for i in os.listdir(self.result_path) if os.path.isdir(os.path.join(self.result_path, i))
                         ]
                         folders.sort()
                         for behavior_name in self.behaviornames_and_colors:
                             all_summary = []
                             for folder in folders:
                                 individual_summary = os.path.join(
                                     self.result_path,
                                     folder,
                                     behavior_name,
                                     "all_summary.xlsx",
                                 )
                                 if os.path.exists(individual_summary) is True:
-                                    all_summary.append(
-                                        pd.read_excel(individual_summary)
-                                    )
+                                    all_summary.append(pd.read_excel(individual_summary))
                             if len(all_summary) >= 1:
                                 all_summary = pd.concat(all_summary, ignore_index=True)
                                 all_summary.to_excel(
                                     os.path.join(
                                         self.result_path,
                                         behavior_name + "_summary.xlsx",
                                     ),
                                     float_format="%.2f",
                                     index_label="ID/parameter",
                                 )
 
                     else:
                         for animal_name in self.animal_to_include:
                             for n in all_events[animal_name]:
-                                event_data[len(event_data)] = all_events[animal_name][
-                                    n
-                                ][: min(all_lengths)]
-                            event_data[len(event_data)] = [["NA", -1]] * min(
-                                all_lengths
-                            )
+                                event_data[len(event_data)] = all_events[animal_name][n][: min(all_lengths)]
+                            event_data[len(event_data)] = [["NA", -1]] * min(all_lengths)
                         del event_data[len(event_data) - 1]
                         time_points = AAD.all_time[: min(all_lengths)]
                         all_events_df = pd.DataFrame(event_data, index=time_points)
                         all_events_df.to_excel(
                             os.path.join(self.result_path, "all_events.xlsx"),
                             float_format="%.2f",
                             index_label="time/ID",
@@ -1488,41 +1347,32 @@
                             time_points,
                             self.behaviornames_and_colors,
                             self.behavior_to_include,
                             width=0,
                             height=0,
                         )
                         folders = [
-                            i
-                            for i in os.listdir(self.result_path)
-                            if os.path.isdir(os.path.join(self.result_path, i))
+                            i for i in os.listdir(self.result_path) if os.path.isdir(os.path.join(self.result_path, i))
                         ]
                         folders.sort()
                         for animal_name in self.animal_kinds:
                             for behavior_name in self.behaviornames_and_colors:
                                 all_summary = []
                                 for folder in folders:
                                     individual_summary = os.path.join(
                                         self.result_path,
                                         folder,
                                         behavior_name,
                                         animal_name + "_all_summary.xlsx",
                                     )
                                     if os.path.exists(individual_summary) is True:
-                                        all_summary.append(
-                                            pd.read_excel(individual_summary)
-                                        )
+                                        all_summary.append(pd.read_excel(individual_summary))
                                 if len(all_summary) >= 1:
-                                    all_summary = pd.concat(
-                                        all_summary, ignore_index=True
-                                    )
+                                    all_summary = pd.concat(all_summary, ignore_index=True)
                                     all_summary.to_excel(
                                         os.path.join(
                                             self.result_path,
-                                            animal_name
-                                            + "_"
-                                            + behavior_name
-                                            + "_summary.xlsx",
+                                            animal_name + "_" + behavior_name + "_summary.xlsx",
                                         ),
                                         float_format="%.2f",
                                         index_label="ID/parameter",
                                     )
```

### Comparing `labgym-2.3.5/LabGym/gui/analysis/mine_results.py` & `labgym-2.4.0/LabGym/gui/analysis/mine_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
@@ -39,78 +39,58 @@
         self.display_window()
 
     def display_window(self):
         panel = wx.Panel(self)
         boxsizer = wx.BoxSizer(wx.VERTICAL)
 
         module_inputfolder = wx.BoxSizer(wx.HORIZONTAL)
-        button_inputfolder = wx.Button(
-            panel, label="Select the folder that stores\nthe data files", size=(300, 40)
-        )
+        button_inputfolder = wx.Button(panel, label="Select the folder that stores\nthe data files", size=(300, 40))
         button_inputfolder.Bind(wx.EVT_BUTTON, self.select_filepath)
         wx.Button.SetToolTip(
             button_inputfolder,
             "Put all folders that store analysis results (each folder contains one raster plot) for control / experimental groups into this folder.",
         )
-        self.text_inputfolder = wx.StaticText(
-            panel, label="None.", style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END
-        )
-        module_inputfolder.Add(
-            button_inputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
-        module_inputfolder.Add(
-            self.text_inputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
+        self.text_inputfolder = wx.StaticText(panel, label="None.", style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END)
+        module_inputfolder.Add(button_inputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
+        module_inputfolder.Add(self.text_inputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(0, 10, 0)
         boxsizer.Add(module_inputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(0, 5, 0)
 
         module_selectcontrol = wx.BoxSizer(wx.HORIZONTAL)
-        button_selectcontrol = wx.Button(
-            panel, label="Select the\ncontrol group", size=(300, 40)
-        )
+        button_selectcontrol = wx.Button(panel, label="Select the\ncontrol group", size=(300, 40))
         button_selectcontrol.Bind(wx.EVT_BUTTON, self.select_control)
         wx.Button.SetToolTip(
             button_selectcontrol,
             "For multiple-group comparison, you can select one group as control for post-hoc comparison. If no control is selected, post-hoc comparison will be performed between each pair of the two groups.",
         )
         self.text_selectcontrol = wx.StaticText(
             panel,
             label="Default: no control group.",
             style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END,
         )
-        module_selectcontrol.Add(
-            button_selectcontrol, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
-        module_selectcontrol.Add(
-            self.text_selectcontrol, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
+        module_selectcontrol.Add(button_selectcontrol, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
+        module_selectcontrol.Add(self.text_selectcontrol, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(module_selectcontrol, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(0, 5, 0)
 
         module_outputfolder = wx.BoxSizer(wx.HORIZONTAL)
         button_outputfolder = wx.Button(
             panel,
             label="Select the folder to store\nthe data mining results",
             size=(300, 40),
         )
         button_outputfolder.Bind(wx.EVT_BUTTON, self.select_result_path)
         wx.Button.SetToolTip(
             button_outputfolder,
             "A spreadsheet containing all data mining results will be stored in this folder.",
         )
-        self.text_outputfolder = wx.StaticText(
-            panel, label="None.", style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END
-        )
-        module_outputfolder.Add(
-            button_outputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
-        module_outputfolder.Add(
-            self.text_outputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10
-        )
+        self.text_outputfolder = wx.StaticText(panel, label="None.", style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END)
+        module_outputfolder.Add(button_outputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
+        module_outputfolder.Add(self.text_outputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(module_outputfolder, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(0, 5, 0)
 
         button_minedata = wx.Button(panel, label="Start to mine data", size=(300, 40))
         button_minedata.Bind(wx.EVT_BUTTON, self.mine_data)
         wx.Button.SetToolTip(
             button_minedata,
@@ -122,79 +102,61 @@
 
         panel.SetSizer(boxsizer)
 
         self.Centre()
         self.Show(True)
 
     def select_filepath(self, event):
-        dialog = wx.MessageDialog(
-            self, "Is the data paired?", "Paired data?", wx.YES_NO | wx.ICON_QUESTION
-        )
+        dialog = wx.MessageDialog(self, "Is the data paired?", "Paired data?", wx.YES_NO | wx.ICON_QUESTION)
         if dialog.ShowModal() == wx.ID_YES:
             self.paired = True
         else:
             self.paired = False
         dialog.Destroy()
 
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.file_path = dialog.GetPath()
             if self.paired is True:
-                self.text_inputfolder.SetLabel(
-                    "Paired input data is in: " + self.file_path + "."
-                )
+                self.text_inputfolder.SetLabel("Paired input data is in: " + self.file_path + ".")
             else:
-                self.text_inputfolder.SetLabel(
-                    "Unpaired input data is in: " + self.file_path + "."
-                )
+                self.text_inputfolder.SetLabel("Unpaired input data is in: " + self.file_path + ".")
         dialog.Destroy()
 
     def select_control(self, event):
         dialog = wx.SingleChoiceDialog(
             self,
             "Select the folder for the control group.",
             "Ignore if you wish to compare all groups",
-            choices=[
-                i
-                for i in os.listdir(self.file_path)
-                if os.path.isdir(os.path.join(self.file_path, i))
-            ],
+            choices=[i for i in os.listdir(self.file_path) if os.path.isdir(os.path.join(self.file_path, i))],
             style=wx.DD_DEFAULT_STYLE,
         )
         if dialog.ShowModal() == wx.ID_OK:
             control_path = dialog.GetStringSelection()
-            self.text_selectcontrol.SetLabel(
-                "The control group is: " + control_path + "."
-            )
+            self.text_selectcontrol.SetLabel("The control group is: " + control_path + ".")
             self.control = self.read_folder(os.path.join(self.file_path, control_path))
             self.control_file_name = os.path.split(control_path)[1]
         else:
             self.control = None
             self.text_selectcontrol.SetLabel("No control group.")
         dialog.Destroy()
 
     def select_result_path(self, event):
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = dialog.GetPath()
-            self.text_outputfolder.SetLabel(
-                "Mining results are in: " + self.result_path + "."
-            )
+            self.text_outputfolder.SetLabel("Mining results are in: " + self.result_path + ".")
         dialog.Destroy()
 
     def read_folder(self, folder):
         folder = folder.replace("\\", "/")
         filelist = {}
         df = {}
         for i in os.listdir(folder):
-            if (
-                i.endswith("_summary.xlsx")
-                or i.endswith("_summary.xls")
-                or i.endswith("_summary.XLS")
-            ):
+            if i.endswith("_summary.xlsx") or i.endswith("_summary.xls") or i.endswith("_summary.XLS"):
                 behavior_name = i.split("_")[-2]
                 filelist[behavior_name] = os.path.join(folder, i)
         if len(filelist) == 0:
             print('No "_summary.xlsx" excel file found!')
         else:
             for behavior_name in filelist:
                 dataset = pd.read_excel(r"" + filelist[behavior_name])
@@ -222,17 +184,15 @@
             return
         del_idx = self.file_names.index(self.control_file_name)
         self.dataset.pop(del_idx)
         self.file_names.insert(0, self.file_names.pop(del_idx))
 
     def mine_data(self, event):
         if self.file_path is None or self.result_path is None:
-            wx.MessageBox(
-                "No input / output folder selected.", "Error", wx.OK | wx.ICON_ERROR
-            )
+            wx.MessageBox("No input / output folder selected.", "Error", wx.OK | wx.ICON_ERROR)
 
         else:
             dialog = wx.TextEntryDialog(
                 self,
                 "Enter a p-value to determine statistical significance",
                 "Default p-value is 0.05",
                 "0.05",
```

### Comparing `labgym-2.3.5/LabGym/gui/main_window.py` & `labgym-2.4.0/LabGym/gui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import wx
 import wx.lib.agw.hyperlink
 
 from LabGym import __version__
 
 from .analysis import AnalysisModule
 from .preprocessing import PreprocessingModule
@@ -52,33 +51,29 @@
             style=wx.ALIGN_CENTER | wx.ST_ELLIPSIZE_END,
         )
         boxsizer.Add(self.developers_text, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 5)
         boxsizer.Add(0, 60, 0)
 
         # Links to GitHub and extended user guide
         links = wx.BoxSizer(wx.HORIZONTAL)
-        homepage = wx.lib.agw.hyperlink.HyperLinkCtrl(
-            panel, 0, "Home Page", URL="https://github.com/umyelab/LabGym"
-        )
+        homepage = wx.lib.agw.hyperlink.HyperLinkCtrl(panel, 0, "Home Page", URL="https://github.com/umyelab/LabGym")
         userguide = wx.lib.agw.hyperlink.HyperLinkCtrl(
             panel,
             0,
             "Extended Guide",
             URL="https://github.com/yujiahu415/LabGym/blob/master/LabGym%20user%20guide_v2.2.pdf",
         )
         links.Add(homepage, 0, wx.LEFT | wx.EXPAND, 10)
         links.Add(userguide, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         boxsizer.Add(links, 0, wx.ALIGN_CENTER, 50)
         boxsizer.Add(0, 50, 0)
 
         # Main modules
         modules = wx.BoxSizer(wx.HORIZONTAL)
-        preprocessing_button = wx.Button(
-            panel, label="Preprocessing Module", size=(200, 40)
-        )
+        preprocessing_button = wx.Button(panel, label="Preprocessing Module", size=(200, 40))
         preprocessing_button.Bind(wx.EVT_BUTTON, self.open_preprocessing_module)
         wx.Button.SetToolTip(
             preprocessing_button,
             "Enhance video contrast / crop frames to exclude unnecessary region / trim videos to only keep necessary time windows.",
         )
         training_button = wx.Button(panel, label="Training Module", size=(200, 40))
         training_button.Bind(wx.EVT_BUTTON, self.open_training_module)
```

### Comparing `labgym-2.3.5/LabGym/gui/preprocessing.py` & `labgym-2.4.0/LabGym/gui/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import os
 from pathlib import Path
 from typing import Tuple
 
 import cv2
 import numpy as np
 import wx
@@ -84,17 +83,15 @@
             button_handler=self.crop_frames,
             tool_tip="Cropping frames to exclude unnecessary areas can increase the analysis efficiency. You need to specify the 4 corner points of the cropping window. This cropping window will be applied for all videos selected.",
             text=self.text_cropframe,
         )
 
         # Contrast module
         # TODO: This feature increases brightness, not contrast (see tools.preprocess_video())
-        self.text_enhancecontrast = self.module_text(
-            "Default: not to enhance contrast."
-        )
+        self.text_enhancecontrast = self.module_text("Default: not to enhance contrast.")
         self.add_module(
             button_label="Specify whether to enhance\nthe contrast in videos",
             button_handler=self.enhance_contrasts,
             tool_tip="Enhancing video contrast will increase the detection accuracy especially when the detection method is background subtraction based. Enter a contrast value to see whether it is good to apply or re-enter it.",
             text=self.text_enhancecontrast,
         )
 
@@ -171,22 +168,18 @@
 
         frame_width_dialog.Destroy()
         resize_dialog.Destroy()
         self.text_inputvideos.SetLabel(label_text)
 
     def select_outpath(self, event):
         """Opens folder selection dialog for storing processed video."""
-        dialog = wx.DirDialog(
-            parent=self, message="Select a directory", style=wx.DD_DEFAULT_STYLE
-        )
+        dialog = wx.DirDialog(parent=self, message="Select a directory", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = dialog.GetPath()
-            self.text_outputfolder.SetLabel(
-                f"Processed videos will be in: {self.result_path}."
-            )
+            self.text_outputfolder.SetLabel(f"Processed videos will be in: {self.result_path}.")
         dialog.Destroy()
 
     def input_duration(self, event):
         """Opens dialogs to configure input time windows."""
 
         # Ask whether or not to trim a video
         trim_dialog = wx.MessageDialog(
@@ -238,17 +231,15 @@
             windows_dialog.Destroy()
             method_dialog.Destroy()
             return
 
         try:
             window_input: str = windows_dialog.GetValue()
             self.time_windows = self.parse_time_window_str(window_input)
-            self.text_duration.SetLabel(
-                f"The time windows to form the new, trimmed video: {self.time_windows}."
-            )
+            self.text_duration.SetLabel(f"The time windows to form the new, trimmed video: {self.time_windows}.")
         except ValueError as err:
             self.trim_video = False
             self.text_duration.SetLabel("Not to trim the videos.")
             wx.MessageBox(
                 f"{str(err)} Please enter the time windows in correct format!",
                 "Error",
                 wx.OK | wx.ICON_ERROR,
@@ -453,17 +444,15 @@
                 self.enhance_contrast = False
                 self.text_enhancecontrast.SetLabel("Not to enhance contrast.")
                 confirm.Destroy()
                 dialog.Destroy()
                 continue
 
             self.enhance_contrast = True
-            self.text_enhancecontrast.SetLabel(
-                f"The contrast enhancement fold change is: {self.contrast}."
-            )
+            self.text_enhancecontrast.SetLabel(f"The contrast enhancement fold change is: {self.contrast}.")
             confirm.Destroy()
             dialog.Destroy()
             cv2.destroyAllWindows()
             break
 
     @property
     def fps_reduction_factor(self):
@@ -534,19 +523,15 @@
             A list of tuples (start, end) where start and end are floats that
             represent the start and end times in seconds of each time window.
 
         Raises:
             ValueError: There was an error parsing the file path.
         """
         video = Path(video_path)
-        parts = [
-            part
-            for part in video.stem.split("_")
-            if part.startswith("st") or part.startswith("ed")
-        ]
+        parts = [part for part in video.stem.split("_") if part.startswith("st") or part.startswith("ed")]
 
         windows = []
         for i in range(0, len(parts), 2):
             if i >= len(parts):
                 raise ValueError(f"Missing ed tag in file {video.name}.")
             try:
                 assert parts[i].startswith("st")
@@ -562,17 +547,15 @@
 
         return windows
 
     def preprocess_videos(self, event):
         """Process videos given the current configuration."""
 
         if self.video_paths is None or self.result_path is None:
-            wx.MessageBox(
-                "No input video(s) / output folder.", "Error", wx.OK | wx.ICON_ERROR
-            )
+            wx.MessageBox("No input video(s) / output folder.", "Error", wx.OK | wx.ICON_ERROR)
             return
 
         print("Start to preprocess video(s)...")
         for video_path in self.video_paths:
             if self.decode_t is True:
                 self.time_windows = self.parse_time_window_filename(video_path)
```

### Comparing `labgym-2.3.5/LabGym/gui/training/__init__.py` & `labgym-2.4.0/LabGym/gui/training/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
```

### Comparing `labgym-2.3.5/LabGym/gui/training/behavior_examples.py` & `labgym-2.4.0/LabGym/gui/training/behavior_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,39 +25,33 @@
 
 import cv2
 import numpy as np
 import wx
 from cv2.typing import MatLike
 
 from LabGym.analyzebehaviors import AnalyzeAnimal
-from LabGym.analyzebehaviorsdetector import (
-    AnalyzeAnimalDetector,
-    get_animal_names,
-    get_detector_names,
-)
+from LabGym.analyzebehaviorsdetector import AnalyzeAnimalDetector
+from LabGym.detector import Detector, get_detector_names
 from LabGym.gui.utils import (
     WX_IMAGE_WILDCARD,
     WX_VIDEO_WILDCARD,
     BehaviorMode,
     LabGymWindow,
 )
 from LabGym.tools import AnimalVsBg
 
-THE_ABSOLUTE_CURRENT_PATH = str(Path(__file__).resolve().parent.parent.parent)
-
 
 class GenerateBehaviorExamples(LabGymWindow):
     """Generate behavior examples for the user to sort."""
 
     def __init__(self):
         super().__init__(title="Generate Behavior Examples", size=(1000, 530))
         self.behavior_mode = BehaviorMode.NON_INTERACTIVE
         self.use_detector = False
-        self.detector_path = None
-        self.path_to_detector = None
+        self.detector = None
         self.detection_threshold = 0
         self.animal_kinds = []
         self.background_path = None
         self.path_to_videos = None
         self.result_path = None
         self.framewidth = None
         self.delta = 10000
@@ -101,37 +95,31 @@
         self.add_module(
             "Select a folder to store the\ngenerated behavior examples",
             self.select_outpath,
             'Will create a subfolder for each video in the selected folder. Each subfolder is named after the file name of the video and stores the generated behavior examples. For "Static images" mode, all generated behavior examples will be in this folder.',
             self.text_outputfolder,
         )
 
-        self.text_detection = self.module_text(
-            "Default: Background subtraction-based method."
-        )
+        self.text_detection = self.module_text("Default: Background subtraction-based method.")
         self.add_module(
             "Specify the method to\ndetect animals or objects",
             self.select_method,
             "Background subtraction-based method is accurate and fast but needs static background and stable illumination in videos; Detectors-based method is accurate and versatile in any recording settings but is slow. See Extended Guide for details.",
             self.text_detection,
         )
 
-        self.text_startgenerate = self.module_text(
-            "Default: at the beginning of the video(s)."
-        )
+        self.text_startgenerate = self.module_text("Default: at the beginning of the video(s).")
         self.add_module(
             "Specify when generating behavior examples\nshould begin (unit: second)",
             self.specify_timing,
             'Enter a beginning time point for all videos or use "Decode from filenames" to let LabGym decode the different beginning time for different videos. See Extended Guide for details.',
             self.text_startgenerate,
         )
 
-        self.text_duration = self.module_text(
-            "Default: from the specified beginning time to the end of a video."
-        )
+        self.text_duration = self.module_text("Default: from the specified beginning time to the end of a video.")
         self.add_module(
             "Specify how long generating examples\nshould last (unit: second)",
             self.input_duration,
             "The duration is the same for all the videos in one batch.",
             self.text_duration,
         )
 
@@ -184,17 +172,15 @@
             self,
             message="Specify the mode of behavior examples to generate",
             caption="Behavior-example mode",
             choices=behavior_modes,
         )
         if dialog.ShowModal() != wx.ID_OK:
             self.behavior_mode = BehaviorMode.NON_INTERACTIVE
-            self.text_specifymode.SetLabel(
-                f"Behavior mode: {behavior_modes[self.behavior_mode]}."
-            )
+            self.text_specifymode.SetLabel(f"Behavior mode: {behavior_modes[self.behavior_mode]}.")
             dialog.Destroy()
             return
 
         self.behavior_mode = dialog.GetSelection()
         dialog.Destroy()
 
         if self.behavior_mode == BehaviorMode.INTERACT_ADVANCED:
@@ -221,23 +207,19 @@
         elif self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             self.text_detection.SetLabel(
                 "Only Detector-based detection method is available for the selected behavior mode."
             )
             self.text_startgenerate.SetLabel(
                 'No need to specify this since the selected behavior mode is "Static images".'
             )
-            self.text_duration.SetLabel(
-                'No need to specify this since the selected behavior mode is "Static images".'
-            )
+            self.text_duration.SetLabel('No need to specify this since the selected behavior mode is "Static images".')
             self.text_animalnumber.SetLabel(
                 'No need to specify this since the selected behavior mode is "Static images".'
             )
-            self.text_length.SetLabel(
-                'No need to specify this since the selected behavior mode is "Static images".'
-            )
+            self.text_length.SetLabel('No need to specify this since the selected behavior mode is "Static images".')
             self.text_skipredundant.SetLabel(
                 'No need to specify this since the selected behavior mode is "Static images".'
             )
 
         label_text = f"Behavior mode: {behavior_modes[self.behavior_mode]}"
         if self.behavior_mode == BehaviorMode.INTERACT_ADVANCED:
             label_text += f" with social distance {self.social_distance}"
@@ -247,17 +229,15 @@
     def select_videos(self, event):
         """Select videos/images to generate behavior examples from."""
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             wildcard = WX_IMAGE_WILDCARD
         else:
             wildcard = WX_VIDEO_WILDCARD
 
-        dialog = wx.FileDialog(
-            self, "Select video(s) / image(s)", "", "", wildcard, style=wx.FD_MULTIPLE
-        )
+        dialog = wx.FileDialog(self, "Select video(s) / image(s)", "", "", wildcard, style=wx.FD_MULTIPLE)
         if dialog.ShowModal() != wx.ID_OK:
             dialog.Destroy()
             return
 
         self.path_to_videos = dialog.GetPaths()
         self.path_to_videos.sort()
         dialog.Destroy()
@@ -301,17 +281,15 @@
         )
 
     def select_outpath(self, event):
         """Select folder to store behavior examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = dialog.GetPath()
-            self.text_outputfolder.SetLabel(
-                f"Generate behavior examples in: {self.result_path}."
-            )
+            self.text_outputfolder.SetLabel(f"Generate behavior examples in: {self.result_path}.")
         dialog.Destroy()
 
     def _configure_background_subtraction(self):
         """Configure background subtraction-based example generation."""
         self.use_detector = False
 
         # The indices of these options are mapped to the same values as the
@@ -343,17 +321,15 @@
         dialog2 = wx.MessageDialog(
             self,
             'Load an existing background from a folder?\nSelect "No" if dont know what it is.',
             "(Optional) load existing background?",
             wx.YES_NO | wx.ICON_QUESTION,
         )
         if dialog2.ShowModal() == wx.ID_YES:
-            start_time_dialog = wx.DirDialog(
-                self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-            )
+            start_time_dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
             if start_time_dialog.ShowModal() == wx.ID_OK:
                 self.background_path = start_time_dialog.GetPath()
             start_time_dialog.Destroy()
         else:
             self.background_path = None
             if self.animal_vs_bg != AnimalVsBg.HARD_TO_TELL:
                 start_time_dialog = wx.MessageDialog(
@@ -390,17 +366,15 @@
 
         self.decode_extraction = False
         if extraction_method == extraction_methods[0]:
             self.text_detection.SetLabel(f"{label_text}, using the entire duration.")
             return
         elif extraction_method == extraction_methods[1]:
             self.decode_extraction = True
-            self.text_detection.SetLabel(
-                f"{label_text}, using time window decoded from filenames '_xst_' and '_xet_'."
-            )
+            self.text_detection.SetLabel(f"{label_text}, using time window decoded from filenames '_xst_' and '_xet_'.")
             return
 
         # Prompt for extraction time window
         label_text += ", using time window (in seconds) from "
         start_time_dialog = wx.NumberEntryDialog(
             self,
             "Enter the start time",
@@ -435,43 +409,40 @@
 
         self.text_detection.SetLabel(label_text)
 
     def _configure_detector(self):
         """Configure Detector-based example generation."""
         self.use_detector = True
         self.animal_number = {}
-        self.detector_path = os.path.join(THE_ABSOLUTE_CURRENT_PATH, "detectors")
 
         detectors = get_detector_names()
         detectors.append("Choose a new directory of the Detector")
 
         select_detector_dialog = wx.SingleChoiceDialog(
             self,
             message="Select a Detector for animal detection",
             caption="Select a Detector",
             choices=detectors,
         )
         if select_detector_dialog.ShowModal() != wx.ID_OK:
             select_detector_dialog.Destroy()
             return
         else:
-            detector = select_detector_dialog.GetStringSelection()
+            detector_name = select_detector_dialog.GetStringSelection()
             select_detector_dialog.Destroy()
 
-        if detector == "Choose a new directory of the Detector":
-            dialog2 = wx.DirDialog(
-                self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-            )
+        if detector_name == "Choose a new directory of the Detector":
+            dialog2 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
             if dialog2.ShowModal() == wx.ID_OK:
-                self.path_to_detector = dialog2.GetPaths()
+                self.detector = Detector(path=dialog2.GetPath())
             dialog2.Destroy()
         else:
-            self.path_to_detector = os.path.join(self.detector_path, detector)
+            self.detector = Detector(name=detector_name)
 
-        animal_names = get_animal_names(detector)
+        animal_names = self.detector.animal_names
         if len(animal_names) > 1:
             dialog2 = wx.MultiChoiceDialog(
                 self,
                 message="Specify which animals/objects involved in behavior examples",
                 caption="Animal/Object kind",
                 choices=animal_names,
             )
@@ -493,26 +464,24 @@
                 0,
                 100,
             )
             if dialog2.ShowModal() == wx.ID_OK:
                 detection_threshold = dialog2.GetValue()
                 self.detection_threshold = detection_threshold / 100
                 self.text_detection.SetLabel(
-                    f"Detector: {detector} (detection threshold: {detection_threshold}%); The animals/objects: {self.animal_kinds}."
+                    f"Detector: {detector_name} (detection threshold: {detection_threshold}%); The animals/objects: {self.animal_kinds}."
                 )
             dialog2.Destroy()
         else:
             for animal_name in self.animal_kinds:
                 self.animal_number[animal_name] = 1
             self.text_animalnumber.SetLabel(
                 f"The number of {self.animal_kinds} is: {list(self.animal_number.values())}."
             )
-            self.text_detection.SetLabel(
-                f"Detector: {detector}; The animals/objects: {self.animal_kinds}."
-            )
+            self.text_detection.SetLabel(f"Detector: {detector_name}; The animals/objects: {self.animal_kinds}.")
 
     def select_method(self, event):
         """Select method to generate contours for behavior examples."""
         DETECTOR = "Use trained Detectors (versatile but slow)"
         BACKGROUND_SUBTRACTION = "Subtract background (fast but requires static background & stable illumination)"
         methods = [DETECTOR]
         if self.behavior_mode in [
@@ -602,17 +571,15 @@
                 "Beginning time to generate examples",
                 0,
                 0,
                 100000000000000,
             )
             if dialog2.ShowModal() == wx.ID_OK:
                 self.t = max(float(dialog2.GetValue()), 0)
-                self.text_startgenerate.SetLabel(
-                    f"Start to generate behavior examples at the: {self.t} second."
-                )
+                self.text_startgenerate.SetLabel(f"Start to generate behavior examples at the: {self.t} second.")
             dialog2.Destroy()
 
     def input_duration(self, event):
         """Select duration for generating behavior examples."""
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             wx.MessageBox(
                 "No need to specify this since the selected behavior mode is 'Static images'.",
@@ -629,17 +596,15 @@
             0,
             0,
             100000000000000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.duration = int(dialog.GetValue())
             if self.duration != 0:
-                self.text_duration.SetLabel(
-                    f"The generation of behavior examples lasts for {self.duration} seconds."
-                )
+                self.text_duration.SetLabel(f"The generation of behavior examples lasts for {self.duration} seconds.")
             else:
                 self.text_duration.SetLabel(
                     "The generation of behavior examples lasts for the entire duration of a video."
                 )
         dialog.Destroy()
 
     def specify_animalnumber(self, event):
@@ -707,17 +672,15 @@
                 1,
                 100,
             )
             if dialog1.ShowModal() == wx.ID_OK:
                 self.animal_number = int(dialog1.GetValue())
             else:
                 self.animal_number = 1
-            self.text_animalnumber.SetLabel(
-                f"The total number of animals in a video is {self.animal_number}."
-            )
+            self.text_animalnumber.SetLabel(f"The total number of animals in a video is {self.animal_number}.")
             dialog1.Destroy()
 
     def input_length(self, event):
         """Enter the number of frames corresponding to a behavior."""
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             wx.MessageBox(
                 'No need to specify this since the selected behavior mode is "Static images".',
@@ -733,17 +696,15 @@
             "Behavior episode duration",
             15,
             1,
             1000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.length = max(int(dialog.GetValue()), 3)
-            self.text_length.SetLabel(
-                f"The duration of a behavior example is: {self.length} frames."
-            )
+            self.text_length.SetLabel(f"The duration of a behavior example is: {self.length} frames.")
         dialog.Destroy()
 
     def specify_redundant(self, event):
         """Select the number of frames to skip when generating examples."""
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             wx.MessageBox(
                 'No need to specify this since the selected behavior mode is "Static images".',
@@ -759,22 +720,18 @@
             "Interval for generating examples",
             15,
             0,
             100000000000000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.skip_redundant = int(dialog.GetValue())
-            self.text_skipredundant.SetLabel(
-                f"Generate a pair of example every {self.skip_redundant} frames."
-            )
+            self.text_skipredundant.SetLabel(f"Generate a pair of example every {self.skip_redundant} frames.")
         else:
             self.skip_redundant = 1
-            self.text_skipredundant.SetLabel(
-                "Generate a pair of example at every frame."
-            )
+            self.text_skipredundant.SetLabel("Generate a pair of example at every frame.")
         dialog.Destroy()
 
     def generate_data(self, event):
         """Generate behavior examples with the given configuration."""
         if self.path_to_videos is None or self.result_path is None:
             wx.MessageBox(
                 "No input video(s) / output folder selected.",
@@ -789,23 +746,21 @@
             "Including background?",
             wx.YES_NO | wx.ICON_QUESTION,
         )
         self.background_free = dialog.ShowModal() != wx.ID_YES
         dialog.Destroy()
 
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
-            if self.path_to_detector is None:
-                wx.MessageBox(
-                    "You need to select a Detector.", "Error", wx.OK | wx.ICON_ERROR
-                )
+            if self.detector is None:
+                wx.MessageBox("You need to select a Detector.", "Error", wx.OK | wx.ICON_ERROR)
                 return
             else:
                 AAD = AnalyzeAnimalDetector()
                 AAD.analyze_images_individuals(
-                    self.path_to_detector,
+                    str(self.detector.path),
                     self.path_to_videos,
                     self.result_path,
                     self.animal_kinds,
                     generate=True,
                     imagewidth=self.framewidth,
                     detection_threshold=self.detection_threshold,
                     background_free=self.background_free,
@@ -913,17 +868,21 @@
                     )
                 else:
                     AA.generate_data_interact_basic(
                         background_free=self.background_free,
                         skip_redundant=self.skip_redundant,
                     )
             else:
+                if self.detector is None:
+                    wx.MessageBox("You need to select a Detector.", "Error", wx.OK | wx.ICON_ERROR)
+                    return
+
                 AAD = AnalyzeAnimalDetector()
                 AAD.prepare_analysis(
-                    self.path_to_detector,
+                    str(self.detector.path),
                     video,
                     self.result_path,
                     self.animal_number,
                     self.animal_kinds,
                     self.behavior_mode,
                     framewidth=self.framewidth,
                     channel=3,
@@ -995,27 +954,23 @@
         self.display_window()
 
     def input_folder(self, event):
         """Select folder with unsorted behavior examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.input_path = Path(dialog.GetPath())
-            self.text_inputfolder.SetLabel(
-                f"Unsorted behavior examples are in: f{self.input_path}."
-            )
+            self.text_inputfolder.SetLabel(f"Unsorted behavior examples are in: f{self.input_path}.")
         dialog.Destroy()
 
     def output_folder(self, event):
         """Select folder to store sorted behavior examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = Path(dialog.GetPath())
-            self.text_outputfolder.SetLabel(
-                f"Sorted behavior examples will be in: {self.result_path}."
-            )
+            self.text_outputfolder.SetLabel(f"Sorted behavior examples will be in: {self.result_path}.")
         dialog.Destroy()
 
     def parse_key_behavior_pairs(self, key_behavior_pairs: str):
         """Parse a keyboard shortcut behavior string into a dictionary.
 
         Each key should be associated with a behavior name in the format
 
@@ -1044,22 +999,18 @@
             if len(pair.split("-")) != 2:
                 raise ValueError(f"Invalid key-behavior pair '{pair}'.")
 
             key = pair.split("-")[0]
             behavior_name = pair.split("-")[1]
 
             if len(key) != 1:
-                raise ValueError(
-                    f"Invalid key '{key}'. Key must be a single character."
-                )
+                raise ValueError(f"Invalid key '{key}'. Key must be a single character.")
 
             if key.lower() in RESERVED_KEYS:
-                raise ValueError(
-                    f"Key '{key}' is reserved. Please use a different key."
-                )
+                raise ValueError(f"Key '{key}' is reserved. Please use a different key.")
 
             self.keys_behaviors[key] = behavior_name
 
     def input_keys(self, event):
         """Enter keyboard shortcuts to automate sorting."""
         while True:
             dialog = wx.TextEntryDialog(
@@ -1081,22 +1032,18 @@
                 wx.MessageBox(
                     str(err),
                     "Error",
                     wx.OK | wx.ICON_ERROR,
                 )
                 continue
 
-            self.text_keynames.SetLabel(
-                f"The key-behaviorname pairs: {key_behavior_pairs}."
-            )
+            self.text_keynames.SetLabel(f"The key-behaviorname pairs: {key_behavior_pairs}.")
             break
 
-    def _generate_behavior_preview(
-        self, pattern_image: MatLike, animation: cv2.VideoCapture | None = None
-    ) -> MatLike:
+    def _generate_behavior_preview(self, pattern_image: MatLike, animation: cv2.VideoCapture | None = None) -> MatLike:
         """Generate the behavior example display to show to the user."""
 
         def put_example_text(img: MatLike, text: str, pos: Tuple[int, int]):
             """Put the given text on the image at the given position."""
             cv2.putText(
                 img,
                 text,
@@ -1134,19 +1081,15 @@
         for key, behavior in self.keys_behaviors.items():
             put_example_text(combined, f"{key}: {behavior}", (x_begin, 15 * n))
             n += 1
         return combined
 
     def sort_behaviors(self, event):
         """Sort behavior examples."""
-        if (
-            self.input_path is None
-            or self.result_path is None
-            or not self.keys_behaviors
-        ):
+        if self.input_path is None or self.result_path is None or not self.keys_behaviors:
             wx.MessageBox(
                 "No input / output folder or shortcut key - behavior name pair specified.",
                 "Error",
                 wx.OK | wx.ICON_ERROR,
             )
             return
 
@@ -1318,40 +1261,32 @@
             ValueError: Invalid behavior name or example name.
         """
         if example not in self._remaining_examples:
             raise ValueError(f"Invalid behavior example {example}.")
         if behavior not in self._behaviors:
             raise ValueError(f"Invalid behavior name {behavior}.")
 
-        (self.source / (example + ".jpg")).rename(
-            self.destination / behavior / (example + ".jpg")
-        )
+        (self.source / (example + ".jpg")).rename(self.destination / behavior / (example + ".jpg"))
         if not self.IMAGES_ONLY:
-            (self.source / (example + ".avi")).rename(
-                self.destination / behavior / (example + ".avi")
-            )
+            (self.source / (example + ".avi")).rename(self.destination / behavior / (example + ".avi"))
         self._action_stack.append((behavior, example))
 
     def undo(self):
         """Undo the most recent sorting operation.
 
         Raises:
             IndexError: No operations left to undo.
         """
         if len(self._action_stack) == 0:
             raise IndexError("Nothing to undo.")
 
         behavior, example = self._action_stack.pop()
-        (self.destination / behavior / (example + ".jpg")).rename(
-            self.source / (example + ".jpg")
-        )
+        (self.destination / behavior / (example + ".jpg")).rename(self.source / (example + ".jpg"))
         if not self.IMAGES_ONLY:
-            (self.destination / behavior / example + ".avi").rename(
-                self.source / (example + ".avi")
-            )
+            (self.destination / behavior / example + ".avi").rename(self.source / (example + ".avi"))
 
     def next(self):
         """Skip to the next behavior example."""
         self._index = (self._index + 1) % self.num_remaining_examples
 
     def prev(self):
         """Go to the previous behavior example."""
```

### Comparing `labgym-2.3.5/LabGym/gui/training/categorizers.py` & `labgym-2.4.0/LabGym/gui/training/categorizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import os
-from pathlib import Path
 
 import wx
 
-from LabGym.categorizers import Categorizers, delete_categorizer, get_categorizer_names
+from LabGym.categorizers import (
+    CATEGORIZER_FOLDER,
+    Categorizers,
+    delete_categorizer,
+    get_categorizer_names,
+)
 from LabGym.gui.utils import BehaviorMode, LabGymWindow
 
-the_absolute_current_path = str(Path(__file__).resolve().parent.parent.parent)
-
 
 class TrainCategorizers(LabGymWindow):
     """Train a Categorizer model using sorted behavior examples.
 
     Attributes:
         behavior_example_folder: The location of the sorted behavior examples.
         renamed_example_folder: The location of the renamed, labeled examples.
@@ -43,15 +44,14 @@
         dim_conv: The width of the Pattern Recognizer.
         channel: The number of channels in ???
         behavior_length: The number of frames corresponding to a single
             behavior.
         aug_methods: A list of augmentation methods to use while training.
         augvalid: Whether or not to use augmentation for validation data.
         data_path: The path to all prepared training examples.
-        model_path: The location of the available categorizers.
         path_to_categorizer: The path to the newly created categorizer.
         training_report_path: The folder in which to store training reports.
         include_bodyparts: Whether or not to include body parts.
         std: ???
         example_width: The behavior example width after resizing, if required.
         background_free: Whether or not the animations contain backgrounds.
         social_distance: The social distance when detecting interactive
@@ -69,18 +69,15 @@
         self.dim_tconv = 32
         self.dim_conv = 32
         self.channel = 1
         self.behavior_length = 15
         self.aug_methods = []
         self.augvalid = True
         self.data_path = None
-        self.model_path = os.path.join(the_absolute_current_path, "models")
-        self.path_to_categorizer = os.path.join(
-            the_absolute_current_path, "models", "New_model"
-        )
+        self.path_to_categorizer = os.path.join(str(CATEGORIZER_FOLDER), "New_model")
         self.training_report_path = None
         self.include_bodyparts = False
         self.std = 0
         self.example_width = None
         self.background_free = True
         self.social_distance = 0
 
@@ -112,17 +109,15 @@
         self.add_module(
             "Specify the type / complexity of\nthe Categorizer to train",
             self.configure_categorizer,
             "Categorizer with both Animation Analyzer and Pattern Recognizer is slower but a little more accurate than that with Pattern Recognizer only. Higher complexity level means deeper and more complex network architecture. See Extended Guide for details.",
             self.text_categorizertype,
         )
 
-        self.text_categorizershape = self.module_text(
-            "Default: (width,height,channel) is (32,32,1) / (32,32,3)."
-        )
+        self.text_categorizershape = self.module_text("Default: (width,height,channel) is (32,32,1) / (32,32,3).")
         self.add_module(
             "Specify the input shape for\nAnimation Analyzer / Pattern Recognizer",
             self.set_categorizer_shape,
             "The input frame / image size should be an even integer and larger than 8. The larger size, the wider of network architecture. Use large size only when there are detailed features in frames / images that are important for identifying behaviors. See Extended Guide for details.",
             self.text_categorizershape,
         )
 
@@ -167,29 +162,23 @@
         self.display_window()
 
     def select_behavior_example_folder(self, event):
         """Select the folder containing sorted behavior examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.behavior_example_folder = dialog.GetPath()
-            self.text_inputexamples.SetLabel(
-                f"Path to sorted behavior examples: {self.behavior_example_folder}."
-            )
+            self.text_inputexamples.SetLabel(f"Path to sorted behavior examples: {self.behavior_example_folder}.")
         dialog.Destroy()
 
     def select_renamed_example_folder(self, event):
         """Select directory to store renamed behavior examples."""
-        dialog = wx.DirDialog(
-            self, "Select a new directory", "", style=wx.DD_DEFAULT_STYLE
-        )
+        dialog = wx.DirDialog(self, "Select a new directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.renamed_example_folder = dialog.GetPath()
-            self.text_renameexample.SetLabel(
-                f"Will copy and rename the examples to: {self.renamed_example_folder}."
-            )
+            self.text_renameexample.SetLabel(f"Will copy and rename the examples to: {self.renamed_example_folder}.")
         dialog.Destroy()
 
         dialog = wx.MessageDialog(
             self,
             'Reducing frame / image size can speed up training\nSelect "No" if dont know what it is.',
             "Resize the frames / images?",
             wx.YES_NO | wx.ICON_QUESTION,
@@ -275,21 +264,17 @@
                 return
             else:
                 self.social_distance = float(distance_dialog.GetValue())
                 if self.social_distance == 0:
                     self.social_distance = float("inf")
                 distance_dialog.Destroy()
         elif self.behavior_mode == BehaviorMode.STATIC_IMAGES:
-            self.text_length.SetLabel(
-                'No need to specify this since the selected behavior mode is "Static images".'
-            )
+            self.text_length.SetLabel('No need to specify this since the selected behavior mode is "Static images".')
 
-        PATTERN_RECOGNIZER_ONLY = (
-            "Categorizer (Pattern Recognizer only) (faster / a little less accurate)"
-        )
+        PATTERN_RECOGNIZER_ONLY = "Categorizer (Pattern Recognizer only) (faster / a little less accurate)"
         BOTH = "Categorizer (Animation Analyzer + Pattern Recognizer)"
         categorizer_types = [PATTERN_RECOGNIZER_ONLY]
         if self.behavior_mode != BehaviorMode.STATIC_IMAGES:
             categorizer_types.append(BOTH)
 
         dialog = wx.SingleChoiceDialog(
             self,
@@ -343,20 +328,16 @@
             label_text += f" and Animation Analyzer (Level {self.level_tconv})"
 
         if self.behavior_mode == BehaviorMode.NON_INTERACTIVE:
             label_text += " to identify non-interactive behaviors of each individual."
         elif self.behavior_mode == BehaviorMode.INTERACT_BASIC:
             label_text += " to identify interactive behaviors of the group."
         elif self.behavior_mode == BehaviorMode.INTERACT_ADVANCED:
-            label_text += (
-                " to identify interactive behaviors of the individual and groups."
-            )
-            label_text += (
-                f" Social Distance: {self.social_distance} folds of animal diameter."
-            )
+            label_text += " to identify interactive behaviors of the individual and groups."
+            label_text += f" Social Distance: {self.social_distance} folds of animal diameter."
         else:
             label_text += " to identify non-interactive behaviors of each individual in static images."
 
         self.text_categorizertype.SetLabel(label_text)
 
     def set_categorizer_shape(self, event):
         """Set the network shape of the categorizer."""
@@ -444,17 +425,15 @@
             "Behavior episode duration",
             15,
             1,
             1000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.behavior_length = max(int(dialog.GetValue()), 3)
-            self.text_length.SetLabel(
-                f"The duration of a behavior example is: {self.behavior_length}."
-            )
+            self.text_length.SetLabel(f"The duration of a behavior example is: {self.behavior_length}.")
         dialog.Destroy()
 
     def select_training_examples(self, event):
         """Select the directory with the training examples."""
         dialog = wx.MessageDialog(
             self,
             "Are the animations (in any) in\ntraining examples background free?",
@@ -570,32 +549,26 @@
         dialog = wx.MessageDialog(
             self,
             "Export the training reports?",
             "Export training reports?",
             wx.YES_NO | wx.ICON_QUESTION,
         )
         if dialog.ShowModal() == wx.ID_YES:
-            dialog2 = wx.DirDialog(
-                self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-            )
+            dialog2 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
             if dialog2.ShowModal() == wx.ID_OK:
                 self.training_report_path = dialog2.GetPath()
-                self.text_report.SetLabel(
-                    f"Training reports will be in: {self.training_report_path}."
-                )
+                self.text_report.SetLabel(f"Training reports will be in: {self.training_report_path}.")
             dialog2.Destroy()
         else:
             self.training_report_path = None
         dialog.Destroy()
 
     def train_categorizer(self, event):
         if self.data_path is None:
-            wx.MessageBox(
-                "No path to training examples.", "Error", wx.OK | wx.ICON_ERROR
-            )
+            wx.MessageBox("No path to training examples.", "Error", wx.OK | wx.ICON_ERROR)
             return
 
         while True:
             dialog = wx.TextEntryDialog(
                 self,
                 "Enter a name for the Categorizer to train",
                 "Categorizer name",
@@ -616,15 +589,15 @@
                 wx.MessageBox(
                     f"The Categorizer {categorizer_name} already exists!",
                     "Error",
                     wx.OK | wx.ICON_ERROR,
                 )
                 continue
 
-            self.path_to_categorizer = os.path.join(self.model_path, dialog.GetValue())
+            self.path_to_categorizer = os.path.join(str(CATEGORIZER_FOLDER), dialog.GetValue())
             os.makedirs(self.path_to_categorizer)
 
             if self.using_animation_analyzer is False:
                 CA = Categorizers()
                 if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
                     self.behavior_length = self.std = 0
                     self.include_bodyparts = False
@@ -673,15 +646,14 @@
 
 class TestCategorizers(LabGymWindow):
     """Test a categorizer."""
 
     def __init__(self):
         super().__init__(title="Test Categorizers", size=(1000, 240))
         self.file_path = None
-        self.model_path = os.path.join(the_absolute_current_path, "models")
         self.path_to_categorizer = None
         self.out_path = None
 
         self.text_selectcategorizer = self.module_text("None.")
         self.add_module(
             "Select a Categorizer\nto test",
             self.select_categorizer,
@@ -702,26 +674,22 @@
             "Select a folder to\nexport testing reports",
             self.select_reportpath,
             "This is the folder to store the reports of testing results and metrics. It is optional.",
             self.text_report,
         )
 
         test_and_delete = wx.BoxSizer(wx.HORIZONTAL)
-        button_test = wx.Button(
-            self.panel, label="Test the Categorizer", size=(300, 40)
-        )
+        button_test = wx.Button(self.panel, label="Test the Categorizer", size=(300, 40))
         button_test.Bind(wx.EVT_BUTTON, self.test_categorizer)
         wx.Button.SetToolTip(
             button_test,
             "Test the selected Categorizer on the ground-truth behavior examples",
         )
 
-        button_delete = wx.Button(
-            self.panel, label="Delete a Categorizer", size=(300, 40)
-        )
+        button_delete = wx.Button(self.panel, label="Delete a Categorizer", size=(300, 40))
         button_delete.Bind(wx.EVT_BUTTON, self.remove_categorizer)
         wx.Button.SetToolTip(
             button_delete,
             "Permanently delete a Categorizer. The deletion CANNOT be restored.",
         )
         test_and_delete.Add(button_test, 0, wx.RIGHT, 50)
         test_and_delete.Add(button_delete, 0, wx.LEFT, 50)
@@ -748,58 +716,48 @@
             dialog.Destroy()
             return
         else:
             categorizer = dialog.GetStringSelection()
             dialog.Destroy()
 
         if categorizer == LOAD_NEW_CATEGORIZER:
-            dialog1 = wx.DirDialog(
-                self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-            )
+            dialog1 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
             if dialog1.ShowModal() != wx.ID_OK:
                 dialog1.Destroy()
                 return
             else:
                 self.path_to_categorizer = dialog1.GetPaths()
                 dialog1.Destroy()
 
-            self.text_selectcategorizer.SetLabel(
-                f"The path to the Categorizer to test is: {self.path_to_categorizer}."
-            )
+            self.text_selectcategorizer.SetLabel(f"The path to the Categorizer to test is: {self.path_to_categorizer}.")
         else:
-            self.path_to_categorizer = os.path.join(self.model_path, categorizer)
+            self.path_to_categorizer = os.path.join(str(CATEGORIZER_FOLDER), categorizer)
             self.text_selectcategorizer.SetLabel(f"Categorizer to test: {categorizer}.")
 
     def select_filepath(self, event):
         """Select the directory with ground-truth behavior examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.file_path = dialog.GetPath()
-            self.text_inputexamples.SetLabel(
-                f"Path to ground-truth behavior examples: {self.file_path}."
-            )
+            self.text_inputexamples.SetLabel(f"Path to ground-truth behavior examples: {self.file_path}.")
         dialog.Destroy()
 
     def select_reportpath(self, event):
         """Select the path to store testing reports."""
         dialog = wx.MessageDialog(
             self,
             "Export the testing reports?",
             "Export testing reports?",
             wx.YES_NO | wx.ICON_QUESTION,
         )
         if dialog.ShowModal() == wx.ID_YES:
-            dialog1 = wx.DirDialog(
-                self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE
-            )
+            dialog1 = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
             if dialog1.ShowModal() == wx.ID_OK:
                 self.out_path = dialog1.GetPath()
-                self.text_report.SetLabel(
-                    f"Testing reports will be in: {self.out_path}."
-                )
+                self.text_report.SetLabel(f"Testing reports will be in: {self.out_path}.")
             dialog1.Destroy()
         else:
             self.out_path = None
         dialog.Destroy()
 
     def test_categorizer(self, event):
         """Test a categorizer."""
@@ -807,17 +765,15 @@
             wx.MessageBox(
                 "No Categorizer selected / path to ground-truth behavior examples.",
                 "Error",
                 wx.OK | wx.ICON_ERROR,
             )
         else:
             CA = Categorizers()
-            CA.test_categorizer(
-                self.file_path, self.path_to_categorizer, result_path=self.out_path
-            )
+            CA.test_categorizer(self.file_path, self.path_to_categorizer, result_path=self.out_path)
 
     def remove_categorizer(self, event):
         """Delete the a categorizer."""
         categorizers = get_categorizer_names()
 
         dialog = wx.SingleChoiceDialog(
             self,
```

### Comparing `labgym-2.3.5/LabGym/gui/training/detectors.py` & `labgym-2.4.0/LabGym/gui/training/detectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-
 import os
 
 import wx
 
-from LabGym.analyzebehaviorsdetector import (
-    delete_detector,
-    get_animal_names,
-    get_annotation_class_names,
-    get_detector_names,
-    test_detector,
-    train_detector,
-)
+from LabGym.detector import Detector, get_annotation_class_names, get_detector_names
 from LabGym.gui.utils import WX_VIDEO_WILDCARD, LabGymWindow
 from LabGym.tools import extract_frames
 
 
 class GenerateImageExamples(LabGymWindow):
     """Generate image examples to use to train a Detector."""
 
@@ -58,37 +50,31 @@
         self.add_module(
             "Select a folder to store the\ngenerated image examples",
             self.select_outpath,
             "The generated image examples (extracted frames) will be stored in this folder.",
             self.text_outputfolder,
         )
 
-        self.text_startgenerate = self.module_text(
-            "Default: at the beginning of the video(s)."
-        )
+        self.text_startgenerate = self.module_text("Default: at the beginning of the video(s).")
         self.add_module(
             "Specify when generating image examples\nshould begin (unit: second)",
             self.specify_timing,
             "Enter a beginning time point for all videos",
             self.text_startgenerate,
         )
 
-        self.text_duration = self.module_text(
-            "Default: from the specified beginning time to the end of a video."
-        )
+        self.text_duration = self.module_text("Default: from the specified beginning time to the end of a video.")
         self.add_module(
             "Specify how long generating examples\nshould last (unit: second)",
             self.input_duration,
             "This duration will be used for all the videos.",
             self.text_duration,
         )
 
-        self.text_skipredundant = self.module_text(
-            "Default: generate an image example every 1000 frames."
-        )
+        self.text_skipredundant = self.module_text("Default: generate an image example every 1000 frames.")
         self.add_module(
             "Specify how many frames to skip when\ngenerating two consecutive images",
             self.specify_redundant,
             "To increase the efficiency of training a Detector, you need to make the training images as diverse (look different) as possible. You can do this by setting an interval between the two consecutively extracted images.",
             self.text_skipredundant,
         )
 
@@ -98,17 +84,15 @@
             tool_tip="Press the button to start generating image examples.",
         )
 
         self.display_window()
 
     def select_videos(self, event):
         """Open dialogs to select videos to generate images from."""
-        video_select_dialog = wx.FileDialog(
-            self, "Select video(s)", "", "", WX_VIDEO_WILDCARD, style=wx.FD_MULTIPLE
-        )
+        video_select_dialog = wx.FileDialog(self, "Select video(s)", "", "", WX_VIDEO_WILDCARD, style=wx.FD_MULTIPLE)
         if video_select_dialog.ShowModal() != wx.ID_OK:
             video_select_dialog.Destroy()
             return
 
         self.path_to_videos = video_select_dialog.GetPaths()
         video_select_dialog.Destroy()
 
@@ -155,17 +139,15 @@
         frame_width_dialog.Destroy()
 
     def select_outpath(self, event):
         """Select directory to store image examples."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.result_path = dialog.GetPath()
-            self.text_outputfolder.SetLabel(
-                f"Generate image examples in: {self.result_path}."
-            )
+            self.text_outputfolder.SetLabel(f"Generate image examples in: {self.result_path}.")
         dialog.Destroy()
 
     def specify_timing(self, event):
         """Choose time point to start generating image examples."""
         dialog = wx.NumberEntryDialog(
             parent=self,
             message="Enter beginning time to generate examples",
@@ -173,17 +155,15 @@
             caption="Beginning time to generate examples",
             value=0,
             min=0,
             max=100000000000000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.t = max(float(dialog.GetValue()), 0)
-            self.text_startgenerate.SetLabel(
-                f"Start to generate image examples at the: {str(self.t)} second."
-            )
+            self.text_startgenerate.SetLabel(f"Start to generate image examples at the: {str(self.t)} second.")
         dialog.Destroy()
 
     def input_duration(self, event):
         """Choose duration to generate video examples."""
         dialog = wx.NumberEntryDialog(
             parent=self,
             message="Enter the duration for generating examples",
@@ -191,36 +171,30 @@
             caption="Duration for generating examples",
             value=0,
             min=0,
             max=100000000000000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.duration = int(dialog.GetValue())
-            self.text_duration.SetLabel(
-                f"The generation of image examples lasts for {self.duration} seconds."
-            )
+            self.text_duration.SetLabel(f"The generation of image examples lasts for {self.duration} seconds.")
         dialog.Destroy()
 
     def specify_redundant(self, event):
         """Select number of frames to skip per example."""
         dialog = wx.NumberEntryDialog(
             self,
             "How many frames to skip?",
             "Enter a number:",
             "Interval for generating examples",
             15,
             0,
             100000000000000,
         )
-        self.skip_redundant = (
-            int(dialog.GetValue()) if dialog.ShowModal() == wx.ID_OK else 1000
-        )
-        self.text_skipredundant.SetLabel(
-            f"Generate an image example every {self.skip_redundant} frames."
-        )
+        self.skip_redundant = int(dialog.GetValue()) if dialog.ShowModal() == wx.ID_OK else 1000
+        self.text_skipredundant.SetLabel(f"Generate an image example every {self.skip_redundant} frames.")
         dialog.Destroy()
 
     def generate_images(self, event):
         """Confirm image example generation."""
         if self.path_to_videos is None or self.result_path is None:
             wx.MessageBox(
                 "No input video(s) / output folder selected.",
@@ -302,34 +276,34 @@
         self.display_window()
 
     def select_images(self, event):
         """Select labeled images."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.path_to_trainingimages = dialog.GetPath()
-            self.text_selectimages.SetLabel(
-                f"Path to training images: {self.path_to_trainingimages}."
-            )
+            self.text_selectimages.SetLabel(f"Path to training images: {self.path_to_trainingimages}.")
         dialog.Destroy()
 
     def select_annotation(self, event):
         """Select COCO annotation file for images."""
         dialog = wx.FileDialog(
             self,
             "Select the annotation file (.json)",
             "",
             wildcard="Annotation File (*.json)|*.json",
             style=wx.FD_OPEN,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.path_to_annotation = dialog.GetPath()
-            class_names = get_annotation_class_names(self.path_to_annotation)
-            self.text_selectannotation.SetLabel(
-                f"Animal/object categories in annotation file: {class_names}."
-            )
+            try:
+                class_names = get_annotation_class_names(self.path_to_annotation)
+            except ValueError as err:
+                wx.MessageBox(str(err), "Error", wx.OK | wx.ICON_ERROR)
+                return
+            self.text_selectannotation.SetLabel(f"Animal/object categories in annotation file: {class_names}.")
         dialog.Destroy()
 
     @property
     def inference_size(self) -> int:
         """The inferencing frame size for the Detector."""
         return self._inference_size
 
@@ -360,17 +334,15 @@
         )
         if dialog.ShowModal() != wx.ID_OK:
             dialog.Destroy()
             return
 
         try:
             self.inference_size = int(dialog.GetValue())
-            self.text_inferencingsize.SetLabel(
-                "Inferencing frame size: " + str(self.inference_size) + "."
-            )
+            self.text_inferencingsize.SetLabel("Inferencing frame size: " + str(self.inference_size) + ".")
         except ValueError as err:
             wx.MessageBox(
                 str(err),
                 "Error",
                 wx.OK | wx.ICON_ERROR,
             )
         dialog.Destroy()
@@ -384,33 +356,29 @@
             "Iterations",
             value=self.iteration_num,
             min=1,
             max=10000,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.iteration_num = int(dialog.GetValue())
-            self.text_iterations.SetLabel(
-                f"Training iteration number: {self.iteration_num}."
-            )
+            self.text_iterations.SetLabel(f"Training iteration number: {self.iteration_num}.")
         dialog.Destroy()
 
     def train_detector(self, event):
         """Train a Detector with the given parameters."""
         if self.path_to_trainingimages is None or self.path_to_annotation is None:
             wx.MessageBox(
                 "No training images / annotation file selected.",
                 "Error",
                 wx.OK | wx.ICON_ERROR,
             )
             return
 
         while True:
-            dialog = wx.TextEntryDialog(
-                self, "Enter a name for the Detector to train", "Detector name"
-            )
+            dialog = wx.TextEntryDialog(self, "Enter a name for the Detector to train", "Detector name")
             if dialog.ShowModal() != wx.ID_OK:
                 break
 
             if dialog.GetValue().strip() == "":
                 wx.MessageBox(
                     "Please enter a name.",
                     "Error",
@@ -423,32 +391,31 @@
                 wx.MessageBox(
                     f"The Detector {dialog.GetValue()} already exists!",
                     "Error",
                     wx.OK | wx.ICON_ERROR,
                 )
                 continue
 
-            train_detector(
+            Detector(name=detector_name).train(
                 self.path_to_annotation,
                 self.path_to_trainingimages,
-                detector_name,
                 self.iteration_num,
                 self.inference_size,
             )
             break
 
 
 class TestDetectors(LabGymWindow):
     """Test Detectors using labeled image examples."""
 
     def __init__(self):
         super().__init__(title="Test Detectors", size=(1000, 280))
         self.path_to_testingimages = None
         self.path_to_annotation = None
-        self.detector_name = None
+        self.detector = None
         self.results_folder = None
 
         self.text_selectdetector = self.module_text("None.")
         self.add_module(
             "Select a Detector\nto test",
             self.select_detector,
             "The object / animal names in the ground-truth testing image dataset should match those in the selected Detector.",
@@ -491,110 +458,107 @@
         wx.Button.SetToolTip(
             button_delete,
             "Permanently delete a Detector. The deletion CANNOT be restored.",
         )
         testanddelete.Add(button_test, 0, wx.RIGHT, 5)
         testanddelete.Add(button_delete, 0, wx.LEFT, 5)
         self.boxsizer.Add(0, self.MODULE_TOP_MARGIN, 0)
-        self.boxsizer.Add(
-            testanddelete, 0, wx.RIGHT | wx.ALIGN_RIGHT, self.BOTTOM_MARGIN * 2
-        )
+        self.boxsizer.Add(testanddelete, 0, wx.RIGHT | wx.ALIGN_RIGHT, self.BOTTOM_MARGIN * 2)
         self.boxsizer.Add(0, self.BOTTOM_MARGIN, 0)
 
         self.display_window()
 
     def select_detector(self, event):
         """Select a detector to test."""
         dialog = wx.SingleChoiceDialog(
             self,
             message="Select a Detector to test",
             caption="Test a Detector",
             choices=get_detector_names(),
         )
 
         if dialog.ShowModal() == wx.ID_OK:
-            self.detector_name = dialog.GetStringSelection()
+            self.detector = Detector(name=dialog.GetStringSelection())
             self.text_selectdetector.SetLabel(
-                f"Selected: {self.detector_name} (animals/objects: {get_animal_names(self.detector_name)})."
+                f"Selected: {self.detector} (animals/objects: {self.detector.animal_names})."
             )
         dialog.Destroy()
 
     def select_images(self, event):
         """Select annotated testing images."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.path_to_testingimages = dialog.GetPath()
-            self.text_selectimages.SetLabel(
-                f"Path to testing images: {self.path_to_testingimages}."
-            )
+            self.text_selectimages.SetLabel(f"Path to testing images: {self.path_to_testingimages}.")
         dialog.Destroy()
 
     def select_annotation(self, event):
         """Select COCO annotation file."""
         dialog = wx.FileDialog(
             self,
             "Select the annotation file (.json)",
             "",
             wildcard="Annotation File (*.json)|*.json",
             style=wx.FD_OPEN,
         )
         if dialog.ShowModal() == wx.ID_OK:
             self.path_to_annotation = dialog.GetPath()
-            class_names = get_annotation_class_names(self.path_to_annotation)
-            self.text_selectannotation.SetLabel(
-                f"Animal/object categories in annotation file: {class_names}."
-            )
+            try:
+                class_names = get_annotation_class_names(self.path_to_annotation)
+            except ValueError as err:
+                wx.MessageBox(str(err), "Error", wx.OK | wx.ICON_ERROR)
+                return
+            self.text_selectannotation.SetLabel(f"Animal/object categories in annotation file: {class_names}.")
         dialog.Destroy()
 
     def select_results_folder(self, event):
         """Select folder to store testing results."""
         dialog = wx.DirDialog(self, "Select a directory", "", style=wx.DD_DEFAULT_STYLE)
         if dialog.ShowModal() == wx.ID_OK:
             self.results_folder = dialog.GetPath()
-            self.text_select_results_folder.SetLabel(
-                f"Testing results stored in: {self.results_folder}."
-            )
+            self.text_select_results_folder.SetLabel(f"Testing results stored in: {self.results_folder}.")
         dialog.Destroy()
 
     def test_detector(self, event):
         """Test the selected detector."""
         if (
-            self.detector_name is None
+            self.detector is None
             or self.path_to_testingimages is None
             or self.path_to_annotation is None
             or self.results_folder is None
         ):
             wx.MessageBox(
                 "No Detector / training images / annotation file / output path selected.",
                 "Error",
                 wx.OK | wx.ICON_ERROR,
             )
         else:
-            test_detector(
+            mAP = self.detector.test(
                 self.path_to_annotation,
                 self.path_to_testingimages,
-                self.detector_name,
                 self.results_folder,
             )
+            print(f"The mean average precision (mAP) of the Detector is: {mAP:.4f}%.")
+            print("Detector testing completed!")
 
     def delete_detector(self, event):
         """Delete a Detector."""
         dialog = wx.SingleChoiceDialog(
             self,
             message="Select a Detector to delete",
             caption="Delete a Detector",
             choices=get_detector_names().sort(),
         )
         if dialog.ShowModal() != wx.ID_OK:
             dialog.Destroy()
             return
 
-        detector = dialog.GetStringSelection()
+        detector = Detector(name=dialog.GetStringSelection())
         confirm = wx.MessageDialog(
             self,
             f"Delete {detector}?",
             "CANNOT be restored!",
             wx.YES_NO | wx.ICON_QUESTION,
         )
         if confirm.ShowModal() == wx.ID_YES:
-            delete_detector(detector)
+            detector.delete()
         confirm.Destroy()
```

### Comparing `labgym-2.3.5/LabGym/gui/training/training_module.py` & `labgym-2.4.0/LabGym/gui/training/training_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
@@ -96,17 +96,15 @@
         )
 
         self.boxsizer.Add(0, 45, 0)
         self.panel.SetSizer(self.boxsizer)
         self.Centre()
         self.Show(True)
 
-    def add_button(
-        self, button_label: str, button_handler: Callable, button_tool_tip: str
-    ):
+    def add_button(self, button_label: str, button_handler: Callable, button_tool_tip: str):
         """
         Adds a button to the main sizer.
 
         Args:
             button_label: The button label.
             button_handler: The function to handle the button press.
             button_tool_tip: The text displayed when the user hovers over the button.
```

### Comparing `labgym-2.3.5/LabGym/gui/utils.py` & `labgym-2.4.0/LabGym/gui/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
@@ -16,16 +16,20 @@
 Email: bingye@umich.edu
 """
 
 from typing import Callable, Tuple
 
 import wx
 
-WX_VIDEO_WILDCARD = "Video files(*.avi;*.mpg;*.mpeg;*.wmv;*.mp4;*.mkv;*.m4v;*.mov)|*.avi;*.mpg;*.mpeg;*.wmv;*.mp4;*.mkv;*.m4v;*.mov"
-WX_IMAGE_WILDCARD = "Image files(*.jpg;*.jpeg;*.png;*.tiff;*.bmp)|*.jpg;*.JPG;*.jpeg;*.JPEG;*.png;*.PNG;*.tiff;*.TIFF;*.bmp;*.BMP"
+WX_VIDEO_WILDCARD = (
+    "Video files(*.avi;*.mpg;*.mpeg;*.wmv;*.mp4;*.mkv;*.m4v;*.mov)|*.avi;*.mpg;*.mpeg;*.wmv;*.mp4;*.mkv;*.m4v;*.mov"
+)
+WX_IMAGE_WILDCARD = (
+    "Image files(*.jpg;*.jpeg;*.png;*.tiff;*.bmp)|*.jpg;*.JPG;*.jpeg;*.JPEG;*.png;*.PNG;*.tiff;*.TIFF;*.bmp;*.BMP"
+)
 
 
 class LabGymWindow(wx.Frame):
     """A base class for LabGym windows.
 
     LabGym windows currently contain a list of buttons with StaticText to their
     right, indicating the current configuration state, as well as a submit
@@ -74,17 +78,15 @@
         module.Add(button, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         module.Add(text, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
         self.boxsizer.Add(0, self.MODULE_TOP_MARGIN, 0)
         self.boxsizer.Add(module, 0, wx.LEFT | wx.RIGHT | wx.EXPAND, 10)
 
     def module_text(self, label: str) -> wx.StaticText:
         """Return a wx.StaticText instance with the given label."""
-        return wx.StaticText(
-            self.panel, label=label, style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END
-        )
+        return wx.StaticText(self.panel, label=label, style=wx.ALIGN_LEFT | wx.ST_ELLIPSIZE_END)
 
     def add_submit_button(self, label: str, handler: Callable, tool_tip: str):
         """Add a submit button.
 
         Args:
             label: The button label.
             handler: The function to handle the button press.
```

### Comparing `labgym-2.3.5/LabGym/minedata.py` & `labgym-2.4.0/LabGym/minedata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 For license issues, please contact:
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 Email: bingye@umich.edu
 """
 
-
 import os
 
 import pandas as pd
 import scikit_posthocs as sp
 from scipy import stats
 
 
@@ -31,17 +30,15 @@
         pval_in=0.05,
         file_names_in=None,
     ):
         self.data = data_in
         self.control = control_in
         self.paired = paired_in
         self.pval = pval_in
-        self.writer = pd.ExcelWriter(
-            os.path.join(result_path_in, "data_mining_results.xlsx")
-        )
+        self.writer = pd.ExcelWriter(os.path.join(result_path_in, "data_mining_results.xlsx"))
         self.file_names = file_names_in
 
     def normal(self, dataset):
         normal = True
         for i in dataset:
             if len(dataset) >= 3:
                 if stats.shapiro(i).pvalue < self.pval:
@@ -77,28 +74,22 @@
                 if result.pvalue <= self.pval:
                     print("\t", parameter)
                     print("\t", "performing", test)
                     print("\t" * 2, "p-value: ", result.pvalue)
                     parameters.append(parameter)
                     pvalues.append(result.pvalue)
 
-                    stat_info = pd.DataFrame(
-                        {"p-value": pvalues}, index=parameters
-                    )  # parameter and associated p-value
-                    stat_info.to_excel(
-                        self.writer, sheet_name=behavior, startrow=startrow
-                    )
+                    stat_info = pd.DataFrame({"p-value": pvalues}, index=parameters)  # parameter and associated p-value
+                    stat_info.to_excel(self.writer, sheet_name=behavior, startrow=startrow)
 
                     significant_data = pd.DataFrame(
                         (setA, setB)
                     ).transpose()  # print out the datasets with significant findings
                     significant_data.columns = self.file_names
-                    significant_data.to_excel(
-                        self.writer, sheet_name=behavior, startrow=startrow, startcol=3
-                    )
+                    significant_data.to_excel(self.writer, sheet_name=behavior, startrow=startrow, startcol=3)
 
                     sheet = self.writer.sheets[behavior]
                     sheet.write_string(startrow, 0, test)
                     startrow += significant_data.shape[0] + 2
 
     def multiple_groups(self):
         for behavior in self.data[0]:
@@ -132,61 +123,51 @@
                     print("\t", parameter)
                     print("\t", "performing", test)
                     print("\t" * 2, "p-value: ", result.pvalue)
 
                     pvalues.append(result.pvalue)
                     parameters.append(parameter)
 
-                    stat_info = pd.DataFrame(
-                        {"p-value": pvalues}, index=parameters
-                    )  # parameter and associated p-value
-                    stat_info.to_excel(
-                        self.writer, sheet_name=behavior, startrow=startrow
-                    )
+                    stat_info = pd.DataFrame({"p-value": pvalues}, index=parameters)  # parameter and associated p-value
+                    stat_info.to_excel(self.writer, sheet_name=behavior, startrow=startrow)
 
                     significant_data = pd.DataFrame(
                         dataset
                     ).transpose()  # print out the datasets with significant findings
                     significant_data.columns = self.file_names
-                    significant_data.to_excel(
-                        self.writer, sheet_name=behavior, startrow=startrow, startcol=8
-                    )
+                    significant_data.to_excel(self.writer, sheet_name=behavior, startrow=startrow, startcol=8)
 
                     if test == "ANOVA":
                         if self.control == None:
                             tukey = stats.tukey_hsd(*dataset)
                             print(tukey)
 
                             posthoc_name = "Tukey"
                             posthoc = pd.DataFrame(tukey)
                         else:
                             dataset_exp = dataset[1:]
                             dunnett = stats.dunnett(*dataset_exp, control=self.control)
                             dunnett.columns = self.file_names[1:]
                             dunnett.index = self.file_names[1:]
                             print("\t" * 2, "Dunnett's post-hoc results:")
-                            print(
-                                "\t" * 2 + dunnett.to_string().replace("\n", "\n\t\t")
-                            )
+                            print("\t" * 2 + dunnett.to_string().replace("\n", "\n\t\t"))
 
                             posthoc_name = "Dunnett"
                             posthoc = pd.DataFrame(dunnett)
                     else:
                         dunn = sp.posthoc_dunn(dataset)
                         dunn.columns = self.file_names
                         dunn.index = self.file_names
                         print("\t" * 2, "Dunn's post-hoc results:")
                         print("\t" * 2 + dunn.to_string().replace("\n", "\n\t\t"))
 
                         posthoc_name = "Dunn"
                         posthoc = pd.DataFrame(dunn)
 
-                    posthoc.to_excel(
-                        self.writer, sheet_name=behavior, startrow=startrow, startcol=3
-                    )
+                    posthoc.to_excel(self.writer, sheet_name=behavior, startrow=startrow, startcol=3)
                     sheet = self.writer.sheets[behavior]
                     sheet.write_string(startrow, 0, test)
                     sheet.write_string(startrow, 3, posthoc_name + "'s post-hoc")
                     startrow += significant_data.shape[0] + 2
 
     def statistical_analysis(self):
         if (len(self.data) == 2 and self.control == None) or (
```

### Comparing `labgym-2.3.5/LabGym/models/__init__.py` & `labgym-2.4.0/LabGym/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
```

### Comparing `labgym-2.3.5/LabGym/tools.py` & `labgym-2.4.0/LabGym/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Copyright (C)
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext. 
+You should have received a copy of the GNU General Public License along with this program. If not, see https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)#fulltext.
 
 For license issues, please contact:
 
 Dr. Bing Ye
 Life Sciences Institute
 University of Michigan
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
+
 from __future__ import annotations
 
 import datetime
 import functools
 import gc
 import operator
 import os
@@ -91,29 +92,23 @@
         for n in range(0, len_frames - 101, 30):
             frames_temp = frames_arr[n : n + 100]
             mean = frames_temp.mean(0)
             frames_mean.append(frames_temp.mean(0))
             check_frames.append(abs(mean - mean_overall) + frames_temp.std(0))
         frames_mean = np.array(frames_mean, dtype="float32")
         check_frames = np.array(check_frames, dtype="float32")
-        background = np.uint8(
-            np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0]
-        )
+        background = np.uint8(np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0])
         del frames_mean
         del check_frames
         del frames_temp
         gc.collect()
         return background  # type: ignore
 
     if stable_illumination is True:
-        return (
-            np.uint8(frames_arr.max(0))
-            if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER
-            else np.uint8(frames_arr.min(0))
-        )  # type:ignore
+        return np.uint8(frames_arr.max(0)) if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else np.uint8(frames_arr.min(0))  # type:ignore
 
     if len_frames > 101:
         frames_mean = []
         check_frames = []
         for n in range(0, len_frames - 101, 30):
             frames_temp = frames_arr[n : n + 100]
             mean = frames_temp.mean(0)
@@ -121,28 +116,22 @@
             if animal_vs_bg == 1:
                 frames_temp_inv = 255 - frames_temp
                 check_frames.append(frames_temp_inv.mean(0) + frames_temp_inv.std(0))
             else:
                 check_frames.append(mean + frames_temp.std(0))
         frames_mean = np.array(frames_mean, dtype="float32")
         check_frames = np.array(check_frames, dtype="float32")
-        background = np.uint8(
-            np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0]
-        )
+        background = np.uint8(np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0])
         del frames_mean
         del check_frames
         del frames_temp
         gc.collect()
         return background  # type: ignore
 
-    return (
-        np.uint8(frames_arr.max(0))
-        if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER
-        else np.uint8(frames_arr.min(0))
-    )  # type: ignore
+    return np.uint8(frames_arr.max(0)) if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else np.uint8(frames_arr.min(0))  # type: ignore
 
 
 def extract_backgrounds_from_video(
     path_to_video: str,
     delta: float,
     frame_size: tuple[int, int] | None = None,
     stable_illumination: bool = True,
@@ -184,20 +173,16 @@
     frame_count = int(capture.get(cv2.CAP_PROP_FRAME_COUNT))
     duration = frame_count / fps
     initial_frame = None
     lower_threshold = None
     upper_threshold = None
 
     if start_time >= duration:
-        print(
-            "The beginning time for background extraction is later than the end of the video!"
-        )
-        print(
-            "Will use the 1st second of the video as the beginning time for background extraction!"
-        )
+        print("The beginning time for background extraction is later than the end of the video!")
+        print("Will use the 1st second of the video as the beginning time for background extraction!")
         start_time = 0
     if start_time == end_time:
         end_time = start_time + 1
 
     # Initialize data storage
     frames = {}
     counts = {}
@@ -209,17 +194,15 @@
         background_options[bg_type] = deque(maxlen=1000)
         backgrounds[bg_type] = None
 
     for frame_number in range(1, frame_count + 1):
         _, frame = capture.read()
 
         reached_start = frame_number >= start_time * fps
-        reached_end = (
-            end_time is not None and frame_number >= end_time * fps or frame is None
-        )
+        reached_end = end_time is not None and frame_number >= end_time * fps or frame is None
 
         if reached_end:
             break
 
         if not reached_start:
             continue
 
@@ -243,29 +226,25 @@
             frames["default"].append(frame)
             counts["default"] += 1
 
         # Extract background if frame buffer has reached 1000 frames
         for bg_type in BG_TYPES:
             if counts[bg_type] == 1001:
                 counts[bg_type] = 1
-                background = _extract_background(
-                    frames[bg_type], stable_illumination, animal_vs_bg
-                )
+                background = _extract_background(frames[bg_type], stable_illumination, animal_vs_bg)
                 if background is not None:
                     background_options[bg_type].append(background)
 
     capture.release()
 
     for bg_type in BG_TYPES:
         if len(background_options[bg_type]) > 0:
             # Process any remaining frames
             if counts[bg_type] > 600:
-                background = _extract_background(
-                    frames[bg_type], stable_illumination, animal_vs_bg
-                )
+                background = _extract_background(frames[bg_type], stable_illumination, animal_vs_bg)
                 if background is not None:
                     background_options[bg_type].append(background)
 
             # Pick the best background option
             if len(background_options[bg_type]) == 1:
                 backgrounds[bg_type] = background_options[bg_type][0]
             else:
@@ -275,33 +254,29 @@
                 elif animal_vs_bg == AnimalVsBg.ANIMAL_DARKER:
                     backgrounds[bg_type] = options.max(axis=0)
                 elif animal_vs_bg == AnimalVsBg.HARD_TO_TELL:
                     backgrounds[bg_type] = np.median(options, axis=0)
                 del options
                 gc.collect()
         else:
-            backgrounds[bg_type] = _extract_background(
-                frames[bg_type], stable_illumination, animal_vs_bg
-            )
+            backgrounds[bg_type] = _extract_background(frames[bg_type], stable_illumination, animal_vs_bg)
 
     if backgrounds["default"] is None:
         background = initial_frame
     if backgrounds["low"] is None:
         backgrounds["low"] = backgrounds["default"]
     if backgrounds["high"] is None:
         backgrounds["high"] = backgrounds["default"]
 
     print("Background extraction completed!")
 
     return (backgrounds["default"], backgrounds["low"], backgrounds["high"])  # type: ignore
 
 
-def load_backgrounds_from_folder(
-    folder: str, frame_size: tuple[int, int] | None = None
-) -> tuple[Frame, Frame, Frame]:
+def load_backgrounds_from_folder(folder: str, frame_size: tuple[int, int] | None = None) -> tuple[Frame, Frame, Frame]:
     """
     Loads background images from given folder, resizing them if required.
 
     Args:
         folder: The path to the folder containing the background images.
         frame_size: The dimensions (width, height) by which to resize the frame
 
@@ -456,17 +431,15 @@
     lower_threshold = None
     upper_threshold = None
     total_contour_areas = []
     for frame_number in range(1, frame_count + 1):
         _, frame = capture.read()
 
         reached_start = frame_number >= start_time * fps
-        reached_end = (
-            end_time is not None and frame_number >= end_time * fps or frame is None
-        )
+        reached_end = end_time is not None and frame_number >= end_time * fps or frame is None
         if reached_end:
             break
         if not reached_start:
             continue
 
         # Preprocess frame
         if frame_size is not None:
@@ -493,17 +466,15 @@
         if animal_vs_bg == AnimalVsBg.HARD_TO_TELL:
             foreground = cv2.absdiff(frame, background)
         else:
             foreground = cv2.subtract(frame, background)
         foreground = cv2.cvtColor(foreground, cv2.COLOR_BGR2GRAY)
 
         # Extract contours from frame
-        _, thred = cv2.threshold(
-            foreground, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
-        )
+        _, thred = cv2.threshold(foreground, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
         kernel = np.ones((kernel_size, kernel_size), np.uint8)
         thred = cv2.morphologyEx(thred, cv2.MORPH_CLOSE, kernel)
         if animal_vs_bg == AnimalVsBg.HARD_TO_TELL:
             kernel_erode_size = max(kernel_size - 4, 1)
             kernel_erode = np.ones((kernel_erode_size, kernel_erode_size), np.uint8)
             thred = cv2.erode(thred, kernel_erode)
         contours, _ = cv2.findContours(thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE)
@@ -525,22 +496,18 @@
 
     animal_area = sum(total_contour_areas) / len(total_contour_areas) / animal_number
     print(f"Single animal size: {animal_area}")
     return animal_area
 
 
 def crop_frame(frame, contours):
-    lfbt = np.array(
-        [contours[i].min(0) for i in range(len(contours)) if contours[i] is not None]
-    ).min(0)[0]
+    lfbt = np.array([contours[i].min(0) for i in range(len(contours)) if contours[i] is not None]).min(0)[0]
     x_lf = lfbt[0]
     y_bt = lfbt[1]
-    rttp = np.array(
-        [contours[i].max(0) for i in range(len(contours)) if contours[i] is not None]
-    ).max(0)[0]
+    rttp = np.array([contours[i].max(0) for i in range(len(contours)) if contours[i] is not None]).max(0)[0]
     x_rt = rttp[0]
     y_tp = rttp[1]
 
     w = x_rt - x_lf + 1
     h = y_tp - y_bt + 1
 
     difference = int(abs(w - h) / 2) + 1
@@ -586,17 +553,15 @@
     if channel == 1:
         blob = cv2.cvtColor(blob, cv2.COLOR_BGR2GRAY)
         blob = img_to_array(blob)
 
     return blob
 
 
-def extract_blob_background(
-    frame, contours, contour=None, channel=1, background_free=False
-):
+def extract_blob_background(frame, contours, contour=None, channel=1, background_free=False):
     (y_bt, y_tp, x_lf, x_rt) = crop_frame(frame, contours)
     if background_free is True:
         mask = np.zeros_like(frame)
         cv2.drawContours(mask, [contour], 0, (255, 255, 255), -1)
         masked_frame = frame * (mask / 255.0)
     else:
         masked_frame = frame
@@ -606,17 +571,15 @@
     if channel == 1:
         blob = cv2.cvtColor(blob, cv2.COLOR_BGR2GRAY)
         blob = img_to_array(blob)
 
     return blob
 
 
-def extract_blob_all(
-    frame, y_bt, y_tp, x_lf, x_rt, contours=None, channel=1, background_free=False
-):
+def extract_blob_all(frame, y_bt, y_tp, x_lf, x_rt, contours=None, channel=1, background_free=False):
     if background_free is True:
         mask = np.zeros_like(frame)
         cv2.drawContours(mask, contours, -1, (255, 255, 255), -1)
         masked_frame = frame * (mask / 255.0)
     else:
         masked_frame = frame
     blob = masked_frame[y_bt:y_tp, x_lf:x_rt]
@@ -673,17 +636,15 @@
         if animal_vs_bg == 2:
             foreground = cv2.absdiff(frame, background)
         else:
             foreground = cv2.subtract(frame, background)
 
     foreground = cv2.cvtColor(foreground, cv2.COLOR_BGR2GRAY)
     thred = cv2.threshold(foreground, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
-    thred = cv2.morphologyEx(
-        thred, cv2.MORPH_CLOSE, np.ones((kernel, kernel), np.uint8)
-    )
+    thred = cv2.morphologyEx(thred, cv2.MORPH_CLOSE, np.ones((kernel, kernel), np.uint8))
     if animal_vs_bg == 2:
         kernel_erode = max(kernel - 4, 1)
         thred = cv2.erode(thred, np.ones((kernel_erode, kernel_erode), np.uint8))
     cnts, _ = cv2.findContours(thred, cv2.RETR_LIST, cv2.CHAIN_APPROX_NONE)
 
     contours = []
     centers = []
@@ -745,49 +706,33 @@
                     cv2.drawContours(background_std, inners[n], -1, (255, 255, 255), -1)
                     backgrounds_std.append(background_std)
 
             if n < length / 4:
                 d = n * int((255 * 4 / length))
                 cv2.drawContours(background_outlines, [outline], 0, (255, d, 0), p_size)
                 if inners is not None:
-                    cv2.drawContours(
-                        background_inners, inners[n], -1, (255, d, 0), p_size
-                    )
+                    cv2.drawContours(background_inners, inners[n], -1, (255, d, 0), p_size)
             elif n < length / 2:
                 d = int((n - length / 4) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255, 255, d), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255, 255, d), p_size)
                 if inners is not None:
-                    cv2.drawContours(
-                        background_inners, inners[n], -1, (255, 255, d), p_size
-                    )
+                    cv2.drawContours(background_inners, inners[n], -1, (255, 255, d), p_size)
             elif n < 3 * length / 4:
                 d = int((n - length / 2) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255, 255 - d, 255), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255, 255 - d, 255), p_size)
                 if inners is not None:
-                    cv2.drawContours(
-                        background_inners, inners[n], -1, (255, 255 - d, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inners[n], -1, (255, 255 - d, 255), p_size)
             else:
                 d = int((n - 3 * length / 4) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255 - d, 0, 255), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255 - d, 0, 255), p_size)
                 if inners is not None:
-                    cv2.drawContours(
-                        background_inners, inners[n], -1, (255 - d, 0, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inners[n], -1, (255 - d, 0, 255), p_size)
 
             if inners is not None:
-                cv2.drawContours(
-                    background_outers, [outline], 0, (255, 255, 255), int(2 * p_size)
-                )
+                cv2.drawContours(background_outers, [outline], 0, (255, 255, 255), int(2 * p_size))
 
     outlines_image = background_outlines[y_bt:y_tp, x_lf:x_rt]
 
     if inners is not None:
         inners_image = background_inners[y_bt:y_tp, x_lf:x_rt]
         outers_image = background_outers[y_bt:y_tp, x_lf:x_rt]
         inners_image = cv2.subtract(inners_image, outers_image)
@@ -803,17 +748,15 @@
         pattern_image = cv2.add(inners_image, outlines_image)
     else:
         pattern_image = outlines_image
 
     return pattern_image
 
 
-def generate_patternimage_all(
-    frame, y_bt, y_tp, x_lf, x_rt, outlines_list, inners_list, std=0
-):
+def generate_patternimage_all(frame, y_bt, y_tp, x_lf, x_rt, outlines_list, inners_list, std=0):
     inners_length = len(inners_list[0])
 
     if inners_length > 0:
         background_inners = np.zeros_like(frame)
         background_outers = np.zeros_like(frame)
 
     background_outlines = np.zeros_like(frame)
@@ -839,42 +782,30 @@
                 for inners in inners_list[n]:
                     cv2.drawContours(background_inners, inners, -1, (255, d, 0), p_size)
         elif n < length / 2:
             d = int((n - length / 4) * (255 * 4 / length))
             cv2.drawContours(background_outlines, outlines, -1, (255, 255, d), p_size)
             if inners_length > 0:
                 for inners in inners_list[n]:
-                    cv2.drawContours(
-                        background_inners, inners, -1, (255, 255, d), p_size
-                    )
+                    cv2.drawContours(background_inners, inners, -1, (255, 255, d), p_size)
         elif n < 3 * length / 4:
             d = int((n - length / 2) * (255 * 4 / length))
-            cv2.drawContours(
-                background_outlines, outlines, -1, (255, 255 - d, 255), p_size
-            )
+            cv2.drawContours(background_outlines, outlines, -1, (255, 255 - d, 255), p_size)
             if inners_length > 0:
                 for inners in inners_list[n]:
-                    cv2.drawContours(
-                        background_inners, inners, -1, (255, 255 - d, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inners, -1, (255, 255 - d, 255), p_size)
         else:
             d = int((n - 3 * length / 4) * (255 * 4 / length))
-            cv2.drawContours(
-                background_outlines, outlines, -1, (255 - d, 0, 255), p_size
-            )
+            cv2.drawContours(background_outlines, outlines, -1, (255 - d, 0, 255), p_size)
             if inners_length > 0:
                 for inners in inners_list[n]:
-                    cv2.drawContours(
-                        background_inners, inners, -1, (255 - d, 0, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inners, -1, (255 - d, 0, 255), p_size)
 
         if inners_length > 0:
-            cv2.drawContours(
-                background_outers, outlines, -1, (255, 255, 255), int(2 * p_size)
-            )
+            cv2.drawContours(background_outers, outlines, -1, (255, 255, 255), int(2 * p_size))
 
     outlines_image = background_outlines[y_bt:y_tp, x_lf:x_rt]
 
     if inners_length > 0:
         inners_image = background_inners[y_bt:y_tp, x_lf:x_rt]
         outers_image = background_outers[y_bt:y_tp, x_lf:x_rt]
         inners_image = cv2.subtract(inners_image, outers_image)
@@ -890,17 +821,15 @@
         pattern_image = cv2.add(inners_image, outlines_image)
     else:
         pattern_image = outlines_image
 
     return pattern_image
 
 
-def generate_patternimage_interact(
-    frame, outlines, other_outlines, inners=None, other_inners=None, std=0
-):
+def generate_patternimage_interact(frame, outlines, other_outlines, inners=None, other_inners=None, std=0):
     total_outlines = functools.reduce(operator.iconcat, other_outlines, [])
     total_outlines += outlines
     (y_bt, y_tp, x_lf, x_rt) = crop_frame(frame, total_outlines)
 
     if inners is not None:
         background_inners = np.zeros_like(frame)
         background_outers = np.zeros_like(frame)
@@ -913,75 +842,55 @@
     length = len(outlines)
     p_size = int(max(abs(y_bt - y_tp), abs(x_lf - x_rt)) / 150 + 1)
 
     for n, outline in enumerate(outlines):
         other_outline = other_outlines[n]
         if len(other_outline) > 0:
             if other_outline[0] is not None:
-                cv2.drawContours(
-                    background_outlines, other_outline, -1, (150, 150, 150), p_size
-                )
+                cv2.drawContours(background_outlines, other_outline, -1, (150, 150, 150), p_size)
 
         if outline is not None:
             if inners is not None:
                 inner = inners[n]
                 other_inner = functools.reduce(operator.iconcat, other_inners[n], [])
                 if other_inner is not None:
-                    cv2.drawContours(
-                        background_inners, other_inner, -1, (150, 150, 150), p_size
-                    )
+                    cv2.drawContours(background_inners, other_inner, -1, (150, 150, 150), p_size)
                 if std > 0:
                     background_std = np.zeros_like(frame)
                     if inner is not None:
                         cv2.drawContours(background_std, inner, -1, (255, 255, 255), -1)
                     if other_inner is not None:
-                        cv2.drawContours(
-                            background_std, other_inner, -1, (255, 255, 255), -1
-                        )
+                        cv2.drawContours(background_std, other_inner, -1, (255, 255, 255), -1)
                     backgrounds_std.append(background_std)
             else:
                 inner = None
 
             if n < length / 4:
                 d = n * int((255 * 4 / length))
                 cv2.drawContours(background_outlines, [outline], 0, (255, d, 0), p_size)
                 if inner is not None:
                     cv2.drawContours(background_inners, inner, -1, (255, d, 0), p_size)
             elif n < length / 2:
                 d = int((n - length / 4) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255, 255, d), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255, 255, d), p_size)
                 if inner is not None:
-                    cv2.drawContours(
-                        background_inners, inner, -1, (255, 255, d), p_size
-                    )
+                    cv2.drawContours(background_inners, inner, -1, (255, 255, d), p_size)
             elif n < 3 * length / 4:
                 d = int((n - length / 2) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255, 255 - d, 255), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255, 255 - d, 255), p_size)
                 if inner is not None:
-                    cv2.drawContours(
-                        background_inners, inner, -1, (255, 255 - d, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inner, -1, (255, 255 - d, 255), p_size)
             else:
                 d = int((n - 3 * length / 4) * (255 * 4 / length))
-                cv2.drawContours(
-                    background_outlines, [outline], 0, (255 - d, 0, 255), p_size
-                )
+                cv2.drawContours(background_outlines, [outline], 0, (255 - d, 0, 255), p_size)
                 if inner is not None:
-                    cv2.drawContours(
-                        background_inners, inner, -1, (255 - d, 0, 255), p_size
-                    )
+                    cv2.drawContours(background_inners, inner, -1, (255 - d, 0, 255), p_size)
 
             if inners is not None:
-                cv2.drawContours(
-                    background_outers, [outline], 0, (255, 255, 255), int(2 * p_size)
-                )
+                cv2.drawContours(background_outers, [outline], 0, (255, 255, 255), int(2 * p_size))
                 if len(other_outline) > 0:
                     if other_outline[0] is not None:
                         cv2.drawContours(
                             background_outers,
                             other_outline,
                             -1,
                             (150, 150, 150),
@@ -1055,17 +964,15 @@
                     data.append(-1)
                     mask.append(True)
             all_data.append(data)
             masks.append(mask)
 
         all_data = np.array(all_data)
         masks = np.array(masks)
-        dataframe = pd.DataFrame(
-            all_data, columns=[float("{:.1f}".format(i)) for i in time_points]
-        )
+        dataframe = pd.DataFrame(all_data, columns=[float("{:.1f}".format(i)) for i in time_points])
 
         heatmap = sb.heatmap(
             dataframe,
             mask=masks,
             xticklabels=x_intvl,
             cmap=LinearSegmentedColormap.from_list("", names_and_colors[behavior_name]),
             cbar=False,
@@ -1097,17 +1004,15 @@
         plt.close()
 
     plt.close("all")
 
     print("The raster plot stored in: " + str(result_path))
 
 
-def extract_frames(
-    path_to_video, out_path, framewidth=None, start_t=0, duration=0, skip_redundant=1000
-):
+def extract_frames(path_to_video, out_path, framewidth=None, start_t=0, duration=0, skip_redundant=1000):
     capture = cv2.VideoCapture(path_to_video)
     fps = round(capture.get(cv2.CAP_PROP_FPS))
     full_duration = capture.get(cv2.CAP_PROP_FRAME_COUNT) / fps
     video_name = os.path.splitext(os.path.basename(path_to_video))[0]
 
     if start_t >= full_duration:
         print("The beginning time is later than the end of the video!")
@@ -1128,22 +1033,18 @@
         if t >= end_t:
             break
 
         if t >= start_t:
             if frame_count_generate % skip_redundant == 0:
                 if framewidth is not None:
                     frameheight = int(frame.shape[0] * framewidth / frame.shape[1])
-                    frame = cv2.resize(
-                        frame, (framewidth, frameheight), interpolation=cv2.INTER_AREA
-                    )
+                    frame = cv2.resize(frame, (framewidth, frameheight), interpolation=cv2.INTER_AREA)
 
                 cv2.imwrite(
-                    os.path.join(
-                        out_path, video_name + "_" + str(frame_count_generate) + ".jpg"
-                    ),
+                    os.path.join(out_path, video_name + "_" + str(frame_count_generate) + ".jpg"),
                     frame,
                 )
 
             frame_count_generate += 1
 
         frame_count += 1
```

### Comparing `labgym-2.3.5/README.md` & `labgym-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `labgym-2.3.5/pyproject.toml` & `labgym-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "2.3.5"
+version = "2.4.0"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
 Homepage = "http://github.com/umyelab/LabGym"
 Documentation = "https://labgym.readthedocs.io/en/latest/"
@@ -74,14 +74,17 @@
     "sphinx-autobuild>=2021.3.14",
     "sphinx-copybutton>=0.5.2",
     "myst-parser>=2.0.0",
     "furo>=2023.9.10",
     "sphinx-inline-tabs>=2023.4.21",
 ]
 
+[tool.ruff]
+line-length = 120
+
 [tool.ruff.lint]
 select = [
     "E4",
     "E7",
     "E9",
     "F",
     "I001",
```

### Comparing `labgym-2.3.5/tests/__init__.py` & `labgym-2.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.3.5/tests/test_main.py` & `labgym-2.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `labgym-2.3.5/tests/test_tools.py` & `labgym-2.4.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.3.5/PKG-INFO` & `labgym-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabGym
-Version: 2.3.5
+Version: 2.4.0
 Summary: Quantify user-defined behaviors.
 Keywords: behavior analysis behavioral analysis user defined behaviors
 Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, M. Victor Struman <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

