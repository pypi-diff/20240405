# Comparing `tmp/napari-segment-everything-0.1.1.tar.gz` & `tmp/napari-segment-everything-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-everything-0.1.1.tar", last modified: Tue Apr  2 13:51:52 2024, max compression
+gzip compressed data, was "napari-segment-everything-0.1.2.tar", last modified: Thu Apr  4 15:28:58 2024, max compression
```

## Comparing `napari-segment-everything-0.1.1.tar` & `napari-segment-everything-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.050761 napari-segment-everything-0.1.1/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1488 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/LICENSE
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       96 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/MANIFEST.in
--rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/PKG-INFO
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     2776 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/README.md
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1185 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/pyproject.toml
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1549 2024-04-02 13:51:52.050761 napari-segment-everything-0.1.1/setup.cfg
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/__init__.py
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/__init__.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       67 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/test_widget.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      214 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/interactive_launch.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      411 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/napari.yaml
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     6570 2024-04-02 12:43:49.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/sam_helper.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)    16181 2024-04-02 13:38:14.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/segment_everything.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     7539 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/widgets.py
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/
--rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/PKG-INFO
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      748 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/SOURCES.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        1 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/dependency_links.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       84 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/entry_points.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      131 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/requires.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       26 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/top_level.txt
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1488 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/LICENSE
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       96 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/MANIFEST.in
+-rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/PKG-INFO
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     2776 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/README.md
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1185 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/pyproject.toml
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1549 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/setup.cfg
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/src/
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/src/napari_segment_everything/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/__init__.py
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/src/napari_segment_everything/_tests/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/_tests/__init__.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       67 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/_tests/test_widget.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      214 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/interactive_launch.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      411 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/napari.yaml
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     6792 2024-04-03 10:17:05.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/sam_helper.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)    18266 2024-04-04 15:28:22.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/segment_everything.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     7539 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.2/src/napari_segment_everything/widgets.py
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-04 15:28:58.264173 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/
+-rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/PKG-INFO
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      748 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/SOURCES.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        1 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/dependency_links.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       84 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/entry_points.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      131 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/requires.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       26 2024-04-04 15:28:58.000000 napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/top_level.txt
```

### Comparing `napari-segment-everything-0.1.1/LICENSE` & `napari-segment-everything-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.1/PKG-INFO` & `napari-segment-everything-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-everything
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Napari SAM plugin to segment everything in your image (not just some things)
 Home-page: https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 Author: Brian Northan
 Author-email: bnorthan@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-segment-everything-0.1.1/README.md` & `napari-segment-everything-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.1/pyproject.toml` & `napari-segment-everything-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.1/setup.cfg` & `napari-segment-everything-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-segment-everything
-version = 0.1.1
+version = 0.1.2
 description = A Napari SAM plugin to segment everything in your image (not just some things)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 author = Brian Northan
 author_email = bnorthan@gmail.com
 license = BSD-3-Clause
```

### Comparing `napari-segment-everything-0.1.1/src/napari_segment_everything/sam_helper.py` & `napari-segment-everything-0.1.2/src/napari_segment_everything/sam_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,30 @@
     return sam
 
 def get_sam_predictor(model_type: str):
     sam = sam_model_registry[model_type](get_weights_path(model_type))
     #sam.to(self._device)
     return SamPredictor(sam)
 
-def get_sam_automatic_mask_generator(model_type: str, points_per_side=32, pred_iou_thresh=0.1, stability_score_thresh=0.1, box_nms_thresh=0.5):
+def get_sam_automatic_mask_generator(model_type: str, 
+                                     points_per_side=32, 
+                                     pred_iou_thresh=0.1, 
+                                     stability_score_thresh=0.1, 
+                                     box_nms_thresh=0.5,
+                                     crop_n_layers=1):
+    
     sam = sam_model_registry[model_type](get_weights_path(model_type))
     sam_anything_predictor = SamAutomaticMaskGenerator(sam,
         points_per_side=int(points_per_side),
         #points_per_batch=64,
         pred_iou_thresh=pred_iou_thresh,
         stability_score_thresh=stability_score_thresh,
         #stability_score_offset=1.0
         box_nms_thresh=box_nms_thresh,
-        #crop_n_layers=1,
+        crop_n_layers=crop_n_layers,
         #crop_nms_thresh=0.7,
         #crop_overlap_ratio: float = 512 / 1500,
         #crop_n_points_downscale_factor=1,
         #in_mask_region_area=0,
         #point_grids: Optional[List[np.ndarray]] = None,
         )
     #sam.to(self._device)
```

### Comparing `napari-segment-everything-0.1.1/src/napari_segment_everything/segment_everything.py` & `napari-segment-everything-0.1.2/src/napari_segment_everything/segment_everything.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import matplotlib.pyplot as plt
 from magicgui.widgets import create_widget
 from napari.layers import Image
 import numpy as np
 from skimage import color, util
 from typing import Optional
 
-from sympy import im
 from napari_segment_everything.widgets import LabeledSpinner, LabeledMinMaxSlider
 from napari_segment_everything.sam_helper import get_sam_automatic_mask_generator, make_label_image_3d, add_properties_to_label_image, filter_labels_3d_multi
 import pickle
 
 # qypt improts
 from qtpy.QtWidgets import (
     QVBoxLayout,
@@ -17,15 +15,16 @@
     QPushButton,
     QComboBox,
     QLabel,
     QHBoxLayout,
     QFileDialog,
     QStackedWidget,
     QGroupBox,
-    QSizePolicy
+    QSizePolicy,
+    QMessageBox
 )
 
 class NapariSegmentEverything(QWidget):
 
     def __init__(self, napari_viewer, parent=None):
 
         QWidget.__init__(self, parent=parent)
@@ -37,30 +36,57 @@
         self.initUI()
 
         self._3D_labels_layer = self.viewer.add_labels(
             data=np.zeros((256, 256, 256), dtype=int),
             name="SAM 3D labels",
         )
 
+        self._3D_labels_layer.mouse_double_click_callbacks.append(self.test_double_click)
         self.load_image(self.im_layer_widget.value)
 
+        self.msg = QMessageBox()
+
+    def test_double_click(self, layer, event):
+        index = int(layer._value)-1  
+
+        result = self.results[index]
+        stats = [
+            f"Area: {result['area']}",
+            f"Circularity: {result['circularity']:.2f}",
+            f"Solidity: {result['solidity']:.2f}",
+            f"Mean intensity: {result['mean_intensity']:.2f}",
+            f"10th percentile intensity: {result['10th_percentile_intensity']:.2f}",
+            f"Mean hue: {result['mean_hue']:.2f}",
+            f"Mean saturation: {result['mean_saturation']:.2f}",
+            f"Predicted IOU: {result['predicted_iou']:.2f}",
+            f"Stability score: {result['stability_score']:.2f}",
+        ]
+        stats_text = "\n".join(stats)
+
+        self.msg.setIcon(QMessageBox.Information)
+        self.msg.setText("Result Stats")
+        self.msg.setInformativeText(stats_text)
+        self.msg.setWindowTitle("Result Stats")
+        self.msg.setModal(True)
+        self.msg.show()
+
     def initUI(self):
         
         self.setWindowTitle('Segment Everything')
         layout = QVBoxLayout()
-        layout.setSpacing(2)
+        layout.setSpacing(30)
 
-        ##### 1.  SAM Parameters #####
+        ##### 1.  SAM Parameters ####
 
-        self.sam_parameters_group = QGroupBox("SAM Parameters")
+        self.sam_parameters_group = QGroupBox("1. Generate 3D labels")
         self.sam_layout = QVBoxLayout()
         self.sam_parameters_group.setLayout(self.sam_layout)
 
         # add open results button
-        self.open_project_button = QPushButton("Open SAM project")
+        self.open_project_button = QPushButton("Open previous...")
         self.open_project_button.clicked.connect(self.open_project)
         self.sam_layout.addWidget(self.open_project_button)
 
         # Dropdown for selecting the model
         model_label = QLabel("Select Model")# Dropdown for selecting the model
         self.model_dropdown = QComboBox()
         self.model_dropdown.addItems(["vit_b"])
@@ -82,30 +108,32 @@
         self.viewer.layers.events.inserted.connect(self.im_layer_widget.reset_choices)
         self.viewer.layers.events.removed.connect(self.im_layer_widget.reset_choices)
 
         self.points_per_side_spinner = LabeledSpinner("Points per side", 4, 100, 32, None)
         self.pred_iou_thresh_spinner = LabeledSpinner("Pred IOU Threshold", 0, 1, 0.1, None, is_double=True)
         self.stability_score_thresh_spinner = LabeledSpinner("Stability Score Threshold", 0, 1, 0.1, None, is_double=True)
         self.box_nms_thresh_spinner = LabeledSpinner("Box NMS Threshold", 0, 1, 0.7, None, is_double=True)
+        self.crop_n_layers_spinner = LabeledSpinner("Crop N Layers", 0, 10, 0, None)
 
         self.sam_layout.addWidget(self.points_per_side_spinner)
         self.sam_layout.addWidget(self.pred_iou_thresh_spinner)
         self.sam_layout.addWidget(self.stability_score_thresh_spinner)
         self.sam_layout.addWidget(self.box_nms_thresh_spinner)
+        self.sam_layout.addWidget(self.crop_n_layers_spinner)
 
         # add process button
-        self.process_button = QPushButton("Process")
+        self.process_button = QPushButton("Generate 3D labels")
         self.process_button.clicked.connect(self.process)
         self.sam_layout.addWidget(self.process_button)
 
         layout.addWidget(self.sam_parameters_group)
 
         ##### 2.  Filter Results #####
 
-        self.filter_results_group = QGroupBox("Filter 3D Results")
+        self.filter_results_group = QGroupBox("2. Filter 3D Labels")
         self.filter_layout = QVBoxLayout()
         self.filter_results_group.setLayout(self.filter_layout)
 
         sizePolicy = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         self.filter_results_group.setSizePolicy(sizePolicy)
 
         self.min_max_area_slider = LabeledMinMaxSlider("Area", 0, 1000000, 0, 1000000, 1000, 'area', self.change_stat)
@@ -135,15 +163,15 @@
         self.filter_layout.addLayout(select_slider_layout)
         self.stacked_widget.setFixedHeight(100)
         self.filter_results_group.setFixedHeight(160)
         self.filter_layout.addWidget(self.stacked_widget)        
         
         layout.addWidget(self.filter_results_group)
 
-        self.make_2d_labels_groups = QGroupBox("Make 2D Labels")
+        self.make_2d_labels_groups = QGroupBox("3. Generate 2D Labels")
         self.make_2d_labels_layout = QVBoxLayout()
         self.make_2d_labels_groups.setLayout(self.make_2d_labels_layout)
         
         # add 2d labels options
         self.labels_options_layout = QHBoxLayout()
         self.labels_options_label = QLabel("2D Labels Options")
         self.labels_options_combo = QComboBox()
@@ -177,17 +205,20 @@
         if file_name:
             with open(file_name, 'rb') as f:
                 project = pickle.load(f)
                 self.results = project['results']
                 image = project['image']
                 self.viewer.add_image(image)
                 self.image = image
+        
         self._3D_labels_layer.data = make_label_image_3d(self.results)
+        self.viewer.dims.ndisplay = 3
 
         add_properties_to_label_image(self.image, self.results)
+        self.update_slider_min_max() 
 
     def save_project(self):
         options = QFileDialog.Options()
         file_name, _ = QFileDialog.getSaveFileName(self, "QFileDialog.getSaveFileName()", "", "Pickle Files (*.pkl)", options=options)
         if file_name:
             project = {'results': self.results, 'image': self.image}
             with open(file_name, 'wb') as f:
@@ -197,50 +228,64 @@
         if self.image is None:
             return
         
         points_per_side = self.points_per_side_spinner.spinner.value()
         pred_iou_thresh = self.pred_iou_thresh_spinner.spinner.value()
         stability_score_thresh = self.stability_score_thresh_spinner.spinner.value()
         box_nms_thresh = self.box_nms_thresh_spinner.spinner.value()
+        crop_n_layers = self.crop_n_layers_spinner.spinner.value()
         
-        self._predictor = get_sam_automatic_mask_generator("vit_b", points_per_side=points_per_side, pred_iou_thresh=pred_iou_thresh, stability_score_thresh=stability_score_thresh, box_nms_thresh=box_nms_thresh)
+        self._predictor = get_sam_automatic_mask_generator("vit_b", points_per_side=points_per_side, 
+                                                           pred_iou_thresh=pred_iou_thresh, 
+                                                           stability_score_thresh=stability_score_thresh, 
+                                                           box_nms_thresh=box_nms_thresh,
+                                                           crop_n_layers=crop_n_layers
+                                                           )
         
         self.results = self._predictor.generate(self.image)
+        
         self.results = sorted(self.results, key=lambda x: x['area'], reverse=False)
 
         print(len(self.results), 'objects found')
-        label_num=1
+        
+        label_num = 1
         for result in self.results:
             result['keep'] = True
             result['label_num'] = label_num
             label_num += 1
 
         add_properties_to_label_image(self.image, self.results)
 
         label_image = make_label_image_3d(self.results)
 
         print(label_image.shape)
-        
-        self._3D_labels_layer.data = label_image
-        
-        self.block_stats = True
-        self.min_max_label_num_slider.max_spinbox.setRange(0, label_num)
-        self.min_max_label_num_slider.max_slider.setRange(0, label_num)
-        self.block_stats = False
 
+        self.update_slider_min_max() 
+        self._3D_labels_layer.data = label_image
         self.viewer.dims.ndisplay = 3
 
     def update_slider_min_max(self):
 
         stats = ['area', 'label_num', 'solidity', 'circularity', 'mean_intensity', '10th_percentile_intensity', 'mean_hue', 'mean_saturation', 'predicted_iou', 'stability_score']
         for stat in stats:
             min_ = min([result[stat] for result in self.results])
             max_ = max([result[stat] for result in self.results])
 
             print(stat, min_, max_)
+
+        num_labels = len(self.results)
+
+        self.block_stats = True
+        self.min_max_label_num_slider.min_spinbox.setRange(0, num_labels)
+        self.min_max_label_num_slider.max_spinbox.setRange(0, num_labels)
+        self.min_max_label_num_slider.min_slider.setRange(0, num_labels)
+        self.min_max_label_num_slider.max_slider.setRange(0, num_labels)
+        #self.min_max_label_num_slider.min_slider.setValue(0)
+        self.min_max_label_num_slider.max_slider.setValue(num_labels)
+        self.block_stats = False
         
     def change_stat(self, stat, min_value, max_value):
         if (self.block_stats == True):
             return
         
         if (self.viewer.dims.ndisplay != 3):
             return
@@ -346,7 +391,9 @@
         self.min_max_area_slider.max_slider.setRange(0, max_area)
 
         for i in range(len(self.viewer.layers)):
             if self.viewer.layers[i].name == "SAM 3D labels":
                 self.viewer.layers.move(i, -1)
                 break
 
+        
+
```

### Comparing `napari-segment-everything-0.1.1/src/napari_segment_everything/widgets.py` & `napari-segment-everything-0.1.2/src/napari_segment_everything/widgets.py`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/PKG-INFO` & `napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-everything
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Napari SAM plugin to segment everything in your image (not just some things)
 Home-page: https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 Author: Brian Northan
 Author-email: bnorthan@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/SOURCES.txt` & `napari-segment-everything-0.1.2/src/napari_segment_everything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

