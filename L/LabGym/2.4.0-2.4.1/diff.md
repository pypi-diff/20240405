# Comparing `tmp/labgym-2.4.0.tar.gz` & `tmp/labgym-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgym-2.4.0.tar", last modified: Mon Mar 25 19:09:57 2024, max compression
+gzip compressed data, was "labgym-2.4.1.tar", last modified: Fri Apr  5 15:29:19 2024, max compression
```

## Comparing `labgym-2.4.0.tar` & `labgym-2.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    31919 2024-03-25 19:09:50.314254 labgym-2.4.0/LICENSE.txt
--rw-r--r--   0        0        0      417 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/NOTICE.txt
--rw-r--r--   0        0        0      882 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/__init__.py
--rw-r--r--   0        0        0     1210 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/__main__.py
--rw-r--r--   0        0        0    87666 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/analyzebehaviors.py
--rw-r--r--   0        0        0   173802 2024-03-25 19:09:50.314254 labgym-2.4.0/LabGym/analyzebehaviorsdetector.py
--rw-r--r--   0        0        0    67359 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/categorizers.py
--rw-r--r--   0        0        0    12995 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/detector.py
--rw-r--r--   0        0        0      859 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/detectors/__init__.py
--rw-r--r--   0        0        0      889 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/__init__.py
--rw-r--r--   0        0        0      904 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/__init__.py
--rw-r--r--   0        0        0     1808 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/analysis_module.py
--rw-r--r--   0        0        0    67750 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/analyze_behaviors.py
--rw-r--r--   0        0        0     9322 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/analysis/mine_results.py
--rw-r--r--   0        0        0     4833 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/main_window.py
--rw-r--r--   0        0        0    21798 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/preprocessing.py
--rw-r--r--   0        0        0      904 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/__init__.py
--rw-r--r--   0        0        0    51881 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/behavior_examples.py
--rw-r--r--   0        0        0    33339 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/categorizers.py
--rw-r--r--   0        0        0    22307 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/detectors.py
--rw-r--r--   0        0        0     5203 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/training/training_module.py
--rw-r--r--   0        0        0     4473 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/gui/utils.py
--rw-r--r--   0        0        0     8091 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/minedata.py
--rw-r--r--   0        0        0      859 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/models/__init__.py
--rw-r--r--   0        0        0    44182 2024-03-25 19:09:50.318254 labgym-2.4.0/LabGym/tools.py
--rw-r--r--   0        0        0      131 2024-03-25 19:09:50.318254 labgym-2.4.0/NOTICE.txt
--rw-r--r--   0        0        0    13320 2024-03-25 19:09:50.318254 labgym-2.4.0/README.md
--rw-r--r--   0        0        0     2239 2024-03-25 19:09:57.506314 labgym-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      859 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/test_main.py
--rw-r--r--   0        0        0     1093 2024-03-25 19:09:50.326254 labgym-2.4.0/tests/test_tools.py
--rw-r--r--   0        0        0    14931 1970-01-01 00:00:00.000000 labgym-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    31919 2024-04-05 15:29:14.834631 labgym-2.4.1/LICENSE.txt
+-rw-r--r--   0        0        0      417 2024-04-05 15:29:14.834631 labgym-2.4.1/LabGym/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-04-05 15:29:14.834631 labgym-2.4.1/LabGym/NOTICE.txt
+-rw-r--r--   0        0        0      882 2024-04-05 15:29:14.834631 labgym-2.4.1/LabGym/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-05 15:29:14.834631 labgym-2.4.1/LabGym/__main__.py
+-rw-r--r--   0        0        0    87666 2024-04-05 15:29:14.834631 labgym-2.4.1/LabGym/analyzebehaviors.py
+-rw-r--r--   0        0        0   173802 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/analyzebehaviorsdetector.py
+-rw-r--r--   0        0        0    67359 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/categorizers.py
+-rw-r--r--   0        0        0    12995 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/detector.py
+-rw-r--r--   0        0        0      859 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/detectors/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/analysis/__init__.py
+-rw-r--r--   0        0        0     1808 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/analysis/analysis_module.py
+-rw-r--r--   0        0        0    67751 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/analysis/analyze_behaviors.py
+-rw-r--r--   0        0        0     9322 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/analysis/mine_results.py
+-rw-r--r--   0        0        0     4833 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/main_window.py
+-rw-r--r--   0        0        0    21918 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/preprocessing.py
+-rw-r--r--   0        0        0      904 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/training/__init__.py
+-rw-r--r--   0        0        0    51881 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/training/behavior_examples.py
+-rw-r--r--   0        0        0    33348 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/training/categorizers.py
+-rw-r--r--   0        0        0    22307 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/training/detectors.py
+-rw-r--r--   0        0        0     5203 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/training/training_module.py
+-rw-r--r--   0        0        0     4473 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/gui/utils.py
+-rw-r--r--   0        0        0     8091 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/minedata.py
+-rw-r--r--   0        0        0      859 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/models/__init__.py
+-rw-r--r--   0        0        0    44963 2024-04-05 15:29:14.838631 labgym-2.4.1/LabGym/tools.py
+-rw-r--r--   0        0        0      131 2024-04-05 15:29:14.838631 labgym-2.4.1/NOTICE.txt
+-rw-r--r--   0        0        0    13320 2024-04-05 15:29:14.838631 labgym-2.4.1/README.md
+-rw-r--r--   0        0        0     2164 2024-04-05 15:29:19.602731 labgym-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      859 2024-04-05 15:29:14.846631 labgym-2.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-05 15:29:14.846631 labgym-2.4.1/tests/test_main.py
+-rw-r--r--   0        0        0     1093 2024-04-05 15:29:14.846631 labgym-2.4.1/tests/test_tools.py
+-rw-r--r--   0        0        0    14864 1970-01-01 00:00:00.000000 labgym-2.4.1/PKG-INFO
```

### Comparing `labgym-2.4.0/LICENSE.txt` & `labgym-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/__init__.py` & `labgym-2.4.1/LabGym/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
```

### Comparing `labgym-2.4.0/LabGym/analyzebehaviors.py` & `labgym-2.4.1/LabGym/analyzebehaviors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/analyzebehaviorsdetector.py` & `labgym-2.4.1/LabGym/analyzebehaviorsdetector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/categorizers.py` & `labgym-2.4.1/LabGym/categorizers.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/detector.py` & `labgym-2.4.1/LabGym/detector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/detectors/__init__.py` & `labgym-2.4.1/LabGym/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/__init__.py` & `labgym-2.4.1/LabGym/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/analysis/__init__.py` & `labgym-2.4.1/LabGym/gui/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/analysis/analysis_module.py` & `labgym-2.4.1/LabGym/gui/analysis/analysis_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/analysis/analyze_behaviors.py` & `labgym-2.4.1/LabGym/gui/analysis/analyze_behaviors.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,16 +410,16 @@
             self.result_path = dialog.GetPath()
             self.text_outputfolder.SetLabel("Results will be in: " + self.result_path + ".")
         dialog.Destroy()
 
     def select_method(self, event):
         if self.behavior_mode <= 1:
             methods = [
-                "Subtract background (fast but requires static background & stable illumination)",
                 "Use trained Detectors (versatile but slow)",
+                "Subtract background (fast but requires static background & stable illumination)", 
             ]
         else:
             methods = ["Use trained Detectors (versatile but slow)"]
 
         dialog = wx.SingleChoiceDialog(
             self,
             message="How to detect the animals?",
```

### Comparing `labgym-2.4.0/LabGym/gui/analysis/mine_results.py` & `labgym-2.4.1/LabGym/gui/analysis/mine_results.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/main_window.py` & `labgym-2.4.1/LabGym/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/preprocessing.py` & `labgym-2.4.1/LabGym/gui/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,28 +407,30 @@
                 "Enter the fold changes for contrast enhancement",
                 "A number between 1.0~5.0",
             )
             if dialog.ShowModal() != wx.ID_OK:
                 self.enhance_contrast = False
                 self.text_enhancecontrast.SetLabel("Not to enhance contrast.")
                 dialog.Destroy()
+                cv2.destroyAllWindows()
                 break
 
             contrast = dialog.GetValue()
             try:
                 self.contrast = float(contrast)
             except ValueError:
                 self.enhance_contrast = False
                 wx.MessageBox(
                     "Please enter a float number between 1.0~5.0.",
                     "Error",
                     wx.OK | wx.ICON_ERROR,
                 )
                 self.text_enhancecontrast.SetLabel("Not to enhance contrast.")
                 dialog.Destroy()
+                cv2.destroyAllWindows()
                 continue
 
             show_frame = frame * self.contrast  # type: ignore
             show_frame[show_frame > 255] = 255
             show_frame = np.uint8(show_frame)
             cv2.destroyAllWindows()
             cv2.namedWindow("The first frame in coordinates", cv2.WINDOW_NORMAL)
@@ -441,14 +443,15 @@
                 wx.YES_NO | wx.ICON_QUESTION,
             )
             if confirm.ShowModal() != wx.ID_YES:
                 self.enhance_contrast = False
                 self.text_enhancecontrast.SetLabel("Not to enhance contrast.")
                 confirm.Destroy()
                 dialog.Destroy()
+                cv2.destroyAllWindows()
                 continue
 
             self.enhance_contrast = True
             self.text_enhancecontrast.SetLabel(f"The contrast enhancement fold change is: {self.contrast}.")
             confirm.Destroy()
             dialog.Destroy()
             cv2.destroyAllWindows()
```

### Comparing `labgym-2.4.0/LabGym/gui/training/__init__.py` & `labgym-2.4.1/LabGym/gui/training/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/training/behavior_examples.py` & `labgym-2.4.1/LabGym/gui/training/behavior_examples.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/training/categorizers.py` & `labgym-2.4.1/LabGym/gui/training/categorizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,19 +266,19 @@
                 self.social_distance = float(distance_dialog.GetValue())
                 if self.social_distance == 0:
                     self.social_distance = float("inf")
                 distance_dialog.Destroy()
         elif self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             self.text_length.SetLabel('No need to specify this since the selected behavior mode is "Static images".')
 
-        PATTERN_RECOGNIZER_ONLY = "Categorizer (Pattern Recognizer only) (faster / a little less accurate)"
         BOTH = "Categorizer (Animation Analyzer + Pattern Recognizer)"
+        PATTERN_RECOGNIZER_ONLY = "Categorizer (Pattern Recognizer only) (faster / a little less accurate)"
         categorizer_types = [PATTERN_RECOGNIZER_ONLY]
         if self.behavior_mode != BehaviorMode.STATIC_IMAGES:
-            categorizer_types.append(BOTH)
+            categorizer_types.insert(0, BOTH)
 
         dialog = wx.SingleChoiceDialog(
             self,
             message="Select the Categorizer type",
             caption="Categorizer types",
             choices=categorizer_types,
         )
@@ -286,30 +286,14 @@
             dialog.Destroy()
             return
         else:
             categorizer_tp = dialog.GetStringSelection()
             self.using_animation_analyzer = categorizer_tp != PATTERN_RECOGNIZER_ONLY
             dialog.Destroy()
 
-        dialog1 = wx.NumberEntryDialog(
-            self,
-            "Complexity level from 1 to 7\nhigher level = deeper network",
-            "Enter a number (1~7)",
-            "Pattern Recognizer level",
-            2,
-            1,
-            7,
-        )
-        if dialog1.ShowModal() != wx.ID_OK:
-            dialog1.Destroy()
-            return
-        else:
-            self.level_conv = int(dialog1.GetValue())
-            dialog1.Destroy()
-
         if self.using_animation_analyzer:
             dialog1 = wx.NumberEntryDialog(
                 self,
                 "Complexity level from 1 to 7\nhigher level = deeper network",
                 "Enter a number (1~7)",
                 "Animation Analyzer level",
                 2,
@@ -319,17 +303,34 @@
             if dialog1.ShowModal() != wx.ID_OK:
                 dialog1.Destroy()
                 return
             else:
                 self.level_tconv = int(dialog1.GetValue())
                 dialog1.Destroy()
 
-        label_text = f"Using Pattern Recognizer (Level {self.level_conv})"
+        dialog1 = wx.NumberEntryDialog(
+            self,
+            "Complexity level from 1 to 7\nhigher level = deeper network",
+            "Enter a number (1~7)",
+            "Pattern Recognizer level",
+            2,
+            1,
+            7,
+        )
+        if dialog1.ShowModal() != wx.ID_OK:
+            dialog1.Destroy()
+            return
+        else:
+            self.level_conv = int(dialog1.GetValue())
+            dialog1.Destroy()
+
+        label_text = "Using "
         if self.using_animation_analyzer:
-            label_text += f" and Animation Analyzer (Level {self.level_tconv})"
+            label_text = f"Animation Analyzer (Level {self.level_tconv}) and "
+        label_text += f"Pattern Recognizer (Level {self.level_conv})"
 
         if self.behavior_mode == BehaviorMode.NON_INTERACTIVE:
             label_text += " to identify non-interactive behaviors of each individual."
         elif self.behavior_mode == BehaviorMode.INTERACT_BASIC:
             label_text += " to identify interactive behaviors of the group."
         elif self.behavior_mode == BehaviorMode.INTERACT_ADVANCED:
             label_text += " to identify interactive behaviors of the individual and groups."
@@ -397,19 +398,19 @@
             if dialog1.ShowModal() == wx.ID_YES:
                 self.channel = 1
             dialog1.Destroy()
 
         shape_tconv = f"({self.dim_tconv}, {self.dim_tconv}, {self.channel})"
         shape_conv = f"({self.dim_conv}, {self.dim_conv}, {self.channel})"
 
-        label_text = f"Input shapes: Pattern Recognizer {shape_conv}"
+        label_text = "Input shapes: "
         if self.using_animation_analyzer:
-            label_text += f", Animation Analyzer {shape_tconv}."
-        else:
-            label_text += "."
+            label_text += f"Animation Analyzer {shape_tconv}, "
+        label_text += f"Pattern Recognizer {shape_conv}."
+
         self.text_categorizershape.SetLabel(label_text)
 
     def input_behavior_length(self, event):
         """Set the number of frames corresponding to a behavior."""
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             wx.MessageBox(
                 'No need to specify this since the selected behavior mode is "Static images".',
```

### Comparing `labgym-2.4.0/LabGym/gui/training/detectors.py` & `labgym-2.4.1/LabGym/gui/training/detectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 class TrainDetectors(LabGymWindow):
     """Train Detectors using labeled image examples."""
 
     def __init__(self):
         super().__init__(title="Train Detectors", size=(1000, 280))
         self.path_to_trainingimages = None
         self.path_to_annotation = None
-        self.inference_size = 320
+        self.inference_size = 480
         self.iteration_num = 200
 
         self.text_selectimages = self.module_text("None.")
         self.add_module(
             button_label="Select the folder containing\nall the training images",
             button_handler=self.select_images,
             tool_tip="The folder that stores all the training images.",
```

### Comparing `labgym-2.4.0/LabGym/gui/training/training_module.py` & `labgym-2.4.1/LabGym/gui/training/training_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/gui/utils.py` & `labgym-2.4.1/LabGym/gui/utils.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/minedata.py` & `labgym-2.4.1/LabGym/minedata.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/models/__init__.py` & `labgym-2.4.1/LabGym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/LabGym/tools.py` & `labgym-2.4.1/LabGym/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import datetime
 import functools
 import gc
 import operator
 import os
 from collections import deque
-from typing import Sequence, Tuple, Union
+from typing import Sequence, Tuple
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from cv2.typing import MatLike
@@ -43,15 +43,15 @@
 class AnimalVsBg:
     ANIMAL_LIGHTER = 0
     ANIMAL_DARKER = 1
     HARD_TO_TELL = 2
 
 
 # Use Frame to refer to different representations of a frame
-Frame = Union[NDArray[np.uint8], MatLike]
+Frame = NDArray[np.uint8]
 
 
 def _extract_background(
     frames: Sequence[MatLike],
     stable_illumination: bool = True,
     animal_vs_bg: int = AnimalVsBg.ANIMAL_LIGHTER,
 ) -> Frame | None:
@@ -63,75 +63,93 @@
         stable_illumination: False if background lighting changes for
             optogenetic experiments, else True.
         animal_vs_bg: Whether the animal is lighter or darker than the
             background or whether it's hard to tell; use constants at top of
             tools.py for specific values.
 
     Returns:
-        An NDArray containing the extracted background.
+        An NDArray containing the extracted background. Returns None if less
+        than 4 frames are provided.
 
     Raises:
         None
     """
 
     len_frames = len(frames)
 
     # Need at least 4 frames to extract background
     if len_frames <= 3:
         return None
 
     # Convert to ndarray
-    frames_arr = np.array(frames, dtype="float32")
+    frames_arr = np.array(frames, dtype=np.uint8)
 
     if animal_vs_bg == AnimalVsBg.HARD_TO_TELL:
         if len_frames <= 101:
-            return np.uint8(np.median(frames_arr, axis=0))  # type: ignore
+            background = np.median(frames_arr, axis=0).astype(np.uint8)
+            print(f"Returning background of type {background.dtype}")
+            return
 
         frames_mean = []
         check_frames = []
         mean_overall = frames_arr.mean(0)
         for n in range(0, len_frames - 101, 30):
             frames_temp = frames_arr[n : n + 100]
             mean = frames_temp.mean(0)
             frames_mean.append(frames_temp.mean(0))
             check_frames.append(abs(mean - mean_overall) + frames_temp.std(0))
+
         frames_mean = np.array(frames_mean, dtype="float32")
         check_frames = np.array(check_frames, dtype="float32")
-        background = np.uint8(np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0])
+        background = np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0].astype(np.uint8)
+
         del frames_mean
         del check_frames
         del frames_temp
         gc.collect()
-        return background  # type: ignore
 
-    if stable_illumination is True:
-        return np.uint8(frames_arr.max(0)) if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else np.uint8(frames_arr.min(0))  # type:ignore
+        print(f"Returning background of type {background.dtype}")
+        return background
+
+    if stable_illumination:
+        max_background = frames_arr.max(0).astype(np.uint8)
+        min_background = frames_arr.min(0).astype(np.uint8)
+        background = max_background if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else min_background
+        print(f"Returning background of type {background.dtype}")
+        return background
 
     if len_frames > 101:
         frames_mean = []
         check_frames = []
         for n in range(0, len_frames - 101, 30):
             frames_temp = frames_arr[n : n + 100]
             mean = frames_temp.mean(0)
             frames_mean.append(mean)
-            if animal_vs_bg == 1:
+            if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER:
                 frames_temp_inv = 255 - frames_temp
                 check_frames.append(frames_temp_inv.mean(0) + frames_temp_inv.std(0))
             else:
                 check_frames.append(mean + frames_temp.std(0))
         frames_mean = np.array(frames_mean, dtype="float32")
         check_frames = np.array(check_frames, dtype="float32")
-        background = np.uint8(np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0])
+        background = np.take_along_axis(frames_mean, np.argsort(check_frames, axis=0), axis=0)[0].astype(np.uint8)
+
         del frames_mean
         del check_frames
         del frames_temp
         gc.collect()
-        return background  # type: ignore
 
-    return np.uint8(frames_arr.max(0)) if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else np.uint8(frames_arr.min(0))  # type: ignore
+        print(f"Returning background of type {background.dtype}")
+        return background
+
+    max_background = frames_arr.max(0).astype(np.uint8)
+    min_background = frames_arr.min(0).astype(np.uint8)
+    background = max_background if animal_vs_bg == AnimalVsBg.ANIMAL_DARKER else min_background
+    print(f"Returning background of type {background.dtype}")
+    return background
 
 
 def extract_backgrounds_from_video(
     path_to_video: str,
     delta: float,
     frame_size: tuple[int, int] | None = None,
     stable_illumination: bool = True,
@@ -263,17 +281,20 @@
     if backgrounds["default"] is None:
         background = initial_frame
     if backgrounds["low"] is None:
         backgrounds["low"] = backgrounds["default"]
     if backgrounds["high"] is None:
         backgrounds["high"] = backgrounds["default"]
 
+    # Convert backgrounds to correct dtype
+    backgrounds = {bg_type: bg.astype(np.uint8) for bg_type, bg in backgrounds.items()}
+
     print("Background extraction completed!")
 
-    return (backgrounds["default"], backgrounds["low"], backgrounds["high"])  # type: ignore
+    return (backgrounds["default"], backgrounds["low"], backgrounds["high"])
 
 
 def load_backgrounds_from_folder(folder: str, frame_size: tuple[int, int] | None = None) -> tuple[Frame, Frame, Frame]:
     """
     Loads background images from given folder, resizing them if required.
 
     Args:
@@ -460,14 +481,15 @@
         elif np.mean(frame) > upper_threshold:
             background = background_high_estimation
         else:
             background = background_estimation
 
         # Subtract background and convert to grayscale
         if animal_vs_bg == AnimalVsBg.HARD_TO_TELL:
+            print(f"Frame: {frame.dtype}; Background: {background.dtype}")
             foreground = cv2.absdiff(frame, background)
         else:
             foreground = cv2.subtract(frame, background)
         foreground = cv2.cvtColor(foreground, cv2.COLOR_BGR2GRAY)
 
         # Extract contours from frame
         _, thred = cv2.threshold(foreground, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
```

### Comparing `labgym-2.4.0/README.md` & `labgym-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/pyproject.toml` & `labgym-2.4.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,28 +13,29 @@
     { name = "M. Victor Struman", email = "strmark@umich.edu" },
     { name = "Kelly Goss", email = "khgoss@umich.edu" },
     { name = "Isabelle Baker", email = "ibaker@umich.edu" },
 ]
 dependencies = [
     "tensorflow>=2.10.1; platform_system != 'Windows'",
     "tensorflow<2.11; platform_system == 'Windows'",
-    "matplotlib>=3.8.2",
-    "opencv-python>=4.9.0.80",
-    "opencv-contrib-python>=4.9.0.80",
-    "openpyxl>=3.1.2",
-    "xlsxwriter>=3.1.9",
-    "pandas>=2.1.4",
-    "scikit-learn>=1.3.2",
-    "scikit-image>=0.22.0",
-    "seaborn>=0.13.1",
-    "wxPython>=4.2.1",
-    "scikit-posthocs>=0.8.1",
+    "matplotlib",
+    "opencv-python",
+    "opencv-contrib-python",
+    "openpyxl",
+    "xlsxwriter",
+    "pandas",
+    "scikit-learn",
+    "scikit-image",
+    "seaborn",
+    "wxPython",
+    "scikit-posthocs",
     "torch==2.0.1 ; platform_system == 'Darwin'",
     "torchvision==0.15.2 ; platform_system == 'Darwin'",
-    "packaging>=23.2",
+    "packaging",
+    "requests",
 ]
 requires-python = ">=3.9,<3.11"
 readme = "README.md"
 keywords = [
     "behavior analysis",
     "behavioral analysis",
     "user defined behaviors",
@@ -44,15 +45,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "2.4.0"
+version = "2.4.1"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
 Homepage = "http://github.com/umyelab/LabGym"
 Documentation = "https://labgym.readthedocs.io/en/latest/"
```

### Comparing `labgym-2.4.0/tests/__init__.py` & `labgym-2.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/tests/test_main.py` & `labgym-2.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/tests/test_tools.py` & `labgym-2.4.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.0/PKG-INFO` & `labgym-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabGym
-Version: 2.4.0
+Version: 2.4.1
 Summary: Quantify user-defined behaviors.
 Keywords: behavior analysis behavioral analysis user defined behaviors
 Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, M. Victor Struman <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,28 +13,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Project-URL: Homepage, http://github.com/umyelab/LabGym
 Project-URL: Documentation, https://labgym.readthedocs.io/en/latest/
 Project-URL: Issues, http://github.com/umyelab/LabGym/issues
 Requires-Python: <3.11,>=3.9
 Requires-Dist: tensorflow>=2.10.1; platform_system != "Windows"
 Requires-Dist: tensorflow<2.11; platform_system == "Windows"
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: opencv-python>=4.9.0.80
-Requires-Dist: opencv-contrib-python>=4.9.0.80
-Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: xlsxwriter>=3.1.9
-Requires-Dist: pandas>=2.1.4
-Requires-Dist: scikit-learn>=1.3.2
-Requires-Dist: scikit-image>=0.22.0
-Requires-Dist: seaborn>=0.13.1
-Requires-Dist: wxPython>=4.2.1
-Requires-Dist: scikit-posthocs>=0.8.1
+Requires-Dist: matplotlib
+Requires-Dist: opencv-python
+Requires-Dist: opencv-contrib-python
+Requires-Dist: openpyxl
+Requires-Dist: xlsxwriter
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: scikit-image
+Requires-Dist: seaborn
+Requires-Dist: wxPython
+Requires-Dist: scikit-posthocs
 Requires-Dist: torch==2.0.1; platform_system == "Darwin"
 Requires-Dist: torchvision==0.15.2; platform_system == "Darwin"
-Requires-Dist: packaging>=23.2
+Requires-Dist: packaging
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # LabGym: quantifying user-defined behaviors
 
 [![PyPI - Version](https://img.shields.io/pypi/v/LabGym)](https://pypi.org/project/LabGym/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/LabGym)](https://pypi.org/project/LabGym/)
 [![Downloads](https://static.pepy.tech/badge/LabGym)](https://pepy.tech/project/LabGym)
```

