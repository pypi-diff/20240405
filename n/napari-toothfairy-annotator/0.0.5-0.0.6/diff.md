# Comparing `tmp/napari-toothfairy-annotator-0.0.5.tar.gz` & `tmp/napari-toothfairy-annotator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-toothfairy-annotator-0.0.5.tar", last modified: Wed Apr  3 15:24:51 2024, max compression
+gzip compressed data, was "napari-toothfairy-annotator-0.0.6.tar", last modified: Fri Apr  5 14:32:39 2024, max compression
```

## Comparing `napari-toothfairy-annotator-0.0.5.tar` & `napari-toothfairy-annotator-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.303018 napari-toothfairy-annotator-0.0.5/
--rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2024-04-03 15:24:51.302018 napari-toothfairy-annotator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/README.md
--rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2024-04-03 15:24:51.305019 napari-toothfairy-annotator-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.194557 napari-toothfairy-annotator-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.237901 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/
--rw-rw-rw-   0        0        0     9570 2024-03-28 15:26:39.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/FDI_Annotator.py
--rw-rw-rw-   0        0        0      335 2024-04-03 15:24:23.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/__init__.py
--rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.299017 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_reader.py
--rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_widget.py
--rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_writer.py
--rw-rw-rw-   0        0        0    13283 2024-04-03 15:21:58.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_widget.py
--rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_writer.py
--rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.301018 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/
--rw-rw-rw-   0        0        0     4716 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.822719 napari-toothfairy-annotator-0.0.6/
+-rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2024-04-05 14:32:39.822719 napari-toothfairy-annotator-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2024-04-05 14:32:39.824719 napari-toothfairy-annotator-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.794387 napari-toothfairy-annotator-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.805518 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/
+-rw-rw-rw-   0        0        0     9832 2024-04-05 14:25:52.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/FDI_Annotator.py
+-rw-rw-rw-   0        0        0      335 2024-04-05 14:30:15.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.819721 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_writer.py
+-rw-rw-rw-   0        0        0    13283 2024-04-03 15:21:58.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_widget.py
+-rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_writer.py
+-rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-05 14:32:39.820722 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/
+-rw-rw-rw-   0        0        0     4716 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-05 14:32:39.000000 napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/top_level.txt
```

### Comparing `napari-toothfairy-annotator-0.0.5/LICENSE` & `napari-toothfairy-annotator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/PKG-INFO` & `napari-toothfairy-annotator-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.5
+Version: 0.0.6
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.5/README.md` & `napari-toothfairy-annotator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/pyproject.toml` & `napari-toothfairy-annotator-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/setup.cfg` & `napari-toothfairy-annotator-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/FDI_Annotator.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/FDI_Annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
             "Lower Jawbone": {"quadrant": 0, "ID": "01", "type": "Lower Jawbone", "name": "Lower Jawbone"},
             "Upper Jawbone": {"quadrant": 0, "ID": "02", "type": "Upper Jawbone", "name": "Upper Jawbone"},
             "Left Inferior Alveolar Canal": {"quadrant": 0, "ID": "03", "type": "Left Inferior Alveolar Canal", "name": "Left Inferior Alveolar Canal"},
             "Right Inferior Alveolar Canal": {"quadrant": 0, "ID": "04", "type": "Right Inferior Alveolar Canal", "name": "Right Inferior Alveolar Canal"},
             "Left Maxillary Sinus": {"quadrant": 0, "ID": "05", "type": "Left Maxillary Sinus", "name": "Left Maxillary Sinus"},
             "Right Maxillary Sinus": {"quadrant": 0, "ID": "06", "type": "Right Maxillary Sinus", "name": "Right Maxillary Sinus"},
             "Pharynx": {"quadrant": 0, "ID": "07", "type": "Pharynx", "name": "Pharynx"},
-
+            "Bridge": {"quadrant": 0, "ID": "08", "type": "Bridge", "name": "Bridge"},
+            "Crown": {"quadrant": 0, "ID": "09", "type": "Crown", "name": "Crown"},
+            "Implant": {"quadrant": 0, "ID": "10", "type": "Implant", "name": "Implant"},
             "Upper Right Central Incisor": {"quadrant": 1, "ID": "11", "type": "Incisor", "name": "Upper Right Central Incisor"},
             "Upper Right Lateral Incisor": {"quadrant": 1, "ID": "12", "type": "Incisor", "name": "Upper Right Lateral Incisor"},
             "Upper Right Canine": {"quadrant": 1, "ID": "13", "type": "Canine", "name": "Upper Right Canine"},
             "Upper Right First Premolar": {"quadrant": 1, "ID": "14", "type": "Premolar", "name": "Upper Right First Premolar"},
             "Upper Right Second Premolar": {"quadrant": 1, "ID": "15", "type": "Premolar", "name": "Upper Right Second Premolar"},
             "Upper Right First Molar": {"quadrant": 1, "ID": "16", "type": "Molar", "name": "Upper Right First Molar"},
             "Upper Right Second Molar": {"quadrant": 1, "ID": "17", "type": "Molar", "name": "Upper Right Second Molar"},
```

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_reader.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_reader.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_widget.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_widget.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_writer.py` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/napari.yaml` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/PKG-INFO` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.5
+Version: 0.0.6
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/SOURCES.txt` & `napari-toothfairy-annotator-0.0.6/src/napari_toothfairy_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

