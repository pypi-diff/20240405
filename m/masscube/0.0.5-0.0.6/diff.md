# Comparing `tmp/masscube-0.0.5.tar.gz` & `tmp/masscube-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masscube-0.0.5.tar", last modified: Thu Mar 21 20:36:38 2024, max compression
+gzip compressed data, was "masscube-0.0.6.tar", last modified: Fri Apr  5 03:19:58 2024, max compression
```

## Comparing `masscube-0.0.5.tar` & `masscube-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-03-21 20:36:38.798902 masscube-0.0.5/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.5/LICENSE
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2631 2024-03-21 20:36:38.798713 masscube-0.0.5/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.5/README.md
--rw-r--r--   0 jiemoniu   (501) staff       (20)      985 2024-03-21 20:36:34.000000 masscube-0.0.5/pyproject.toml
--rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-03-21 20:36:38.798943 masscube-0.0.5/setup.cfg
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-03-21 20:36:38.794926 masscube-0.0.5/src/
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-03-21 20:36:38.797578 masscube-0.0.5/src/masscube/
--rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.5/src/masscube/__init__.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    33295 2024-03-12 08:18:03.000000 masscube-0.0.5/src/masscube/alignment.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    15196 2024-03-11 20:20:29.000000 masscube-0.0.5/src/masscube/annotation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     3360 2024-03-04 07:41:12.000000 masscube-0.0.5/src/masscube/feature_evaluation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     8648 2024-03-05 07:37:45.000000 masscube-0.0.5/src/masscube/feature_grouping.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.5/src/masscube/feature_table_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.5/src/masscube/network.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     3383 2024-03-08 01:14:01.000000 masscube-0.0.5/src/masscube/normalization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10140 2024-03-12 22:27:15.000000 masscube-0.0.5/src/masscube/params.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    16386 2024-03-19 00:37:25.000000 masscube-0.0.5/src/masscube/peak_detect.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    32528 2024-03-19 00:24:14.000000 masscube-0.0.5/src/masscube/raw_data_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5078 2024-03-08 02:19:48.000000 masscube-0.0.5/src/masscube/stats.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.5/src/masscube/utils_functions.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    12353 2024-03-12 01:16:11.000000 masscube-0.0.5/src/masscube/visualization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5493 2024-03-18 22:35:52.000000 masscube-0.0.5/src/masscube/workflows.py
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-03-21 20:36:38.798476 masscube-0.0.5/src/masscube.egg-info/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2631 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/SOURCES.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/dependency_links.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      138 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/entry_points.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      148 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/requires.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-03-21 20:36:38.000000 masscube-0.0.5/src/masscube.egg-info/top_level.txt
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.356791 masscube-0.0.6/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.6/LICENSE
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-05 03:19:58.356612 masscube-0.0.6/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.6/README.md
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      959 2024-04-05 00:44:14.000000 masscube-0.0.6/pyproject.toml
+-rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-05 03:19:58.356829 masscube-0.0.6/setup.cfg
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.349487 masscube-0.0.6/src/
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.355561 masscube-0.0.6/src/masscube/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.6/src/masscube/__init__.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    19558 2024-04-03 22:03:37.000000 masscube-0.0.6/src/masscube/alignment.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.6/src/masscube/annotation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2062 2024-04-03 22:01:18.000000 masscube-0.0.6/src/masscube/feature_evaluation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.6/src/masscube/feature_grouping.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.6/src/masscube/feature_table_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.6/src/masscube/network.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     3477 2024-03-22 03:35:49.000000 masscube-0.0.6/src/masscube/normalization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10243 2024-04-03 00:15:40.000000 masscube-0.0.6/src/masscube/params.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10680 2024-04-03 22:03:45.000000 masscube-0.0.6/src/masscube/peak_detect.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    29428 2024-04-05 02:13:47.000000 masscube-0.0.6/src/masscube/raw_data_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     5504 2024-03-22 22:35:24.000000 masscube-0.0.6/src/masscube/stats.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.6/src/masscube/utils_functions.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12618 2024-04-03 23:13:18.000000 masscube-0.0.6/src/masscube/visualization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     5717 2024-04-03 23:10:04.000000 masscube-0.0.6/src/masscube/workflows.py
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.356409 masscube-0.0.6/src/masscube.egg-info/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/SOURCES.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/dependency_links.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      138 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/entry_points.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/requires.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/top_level.txt
```

### Comparing `masscube-0.0.5/LICENSE` & `masscube-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `masscube-0.0.5/PKG-INFO` & `masscube-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.5
+Version: 0.0.6
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.0
 Requires-Dist: pyteomics>=4.6
 Requires-Dist: scipy>=1.10.1
-Requires-Dist: tensorflow>=2.12.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: matplotlib
 Requires-Dist: ms_entropy>=1.1.1
 Requires-Dist: networkx
 Requires-Dist: scikit-learn
```

### Comparing `masscube-0.0.5/README.md` & `masscube-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `masscube-0.0.5/pyproject.toml` & `masscube-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masscube"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Accurate and fast data processing for metabolomics"
@@ -20,15 +20,14 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy>=1.24",
     "pandas>=2.0",
     "pyteomics>=4.6",
     "scipy>=1.10.1",
-    "tensorflow>=2.12.0",
     "tqdm>=4.65.0",
     "lxml>=4.9.2",
     "matplotlib",
     "ms_entropy>=1.1.1",
     "networkx",
     "scikit-learn"
 ]
```

### Comparing `masscube-0.0.5/src/masscube/alignment.py` & `masscube-0.0.6/src/masscube/alignment.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import numpy as np
 import pandas as pd
 import os
 from tqdm import tqdm
 from .visualization import mirror_ms2_db
 from .raw_data_utils import read_raw_file_to_obj
 
-from time import time
-
 
 def feature_alignment(path, parameters):
     """
     A function to align the features from individual files.
 
     Parameters
     ----------------------------------------------------------
@@ -49,16 +47,15 @@
 
         # check if the file exists
         if not os.path.exists(csv_file_names[i]):
             problematic_files.append(file_name)
             continue
         
         # read feature table
-        current_table = pd.read_csv(csv_file_names[i])
-        # current_table = current_table[current_table["MS2"].notna()|(current_table["length"] > parameters.min_ion_num)|(current_table["peak_height"] > parameters.int_tol*3)]
+        current_table = pd.read_csv(csv_file_names[i], low_memory=False)
         current_table = current_table[current_table["MS2"].notna()|(current_table["peak_height"] > parameters.int_tol*3)]
         # sort current table by peak height from high to low
         current_table = current_table.sort_values(by="peak_height", ascending=False)
         current_table.index = range(len(current_table))
         new_feature_idx = []
 
         mz_seq = np.array(feature_table["m/z"], dtype=float)
@@ -84,16 +81,16 @@
                 feature_table.loc[idx, file_name] = current_table.loc[j, "peak_height"]
                 # update the m/z and RT of the feature by averaging the values
                 feature_table.loc[idx, "m/z"] = (feature_table.loc[idx, "m/z"]*i + current_table.loc[j, "m/z"])/(i+1)
                 feature_table.loc[idx, "RT"] = (feature_table.loc[idx, "RT"]*i + current_table.loc[j, "RT"])/(i+1)
                 # if the intensity is the largest, update the reference file
                 if current_table.loc[j, "peak_height"] > int_seq[idx]:
                     feature_table.iloc[idx, 3:10] = [current_table.loc[j, "adduct"], current_table.loc[j, "is_isotope"], 
-                                                     current_table.loc[j, "is_in_source_fragment"], current_table.loc[j, "peak_shape"], 
-                                                     current_table.loc[j, "Gaussian_similarity"], current_table.loc[j, "charge"], 
+                                                     current_table.loc[j, "is_in_source_fragment"], current_table.loc[j, "Gaussian_similarity"], 
+                                                     current_table.loc[j, "noise_level"], current_table.loc[j, "charge"], 
                                                      current_table.loc[j, "isotopes"]]
                     # only overwrite the MS2 if the current MS2 is not nan
                     if current_table.loc[j, "MS2"] == current_table.loc[j, "MS2"]:
                         feature_table.loc[idx,"MS2"] = current_table.loc[j, "MS2"]
                     feature_table.loc[idx, "alignment_reference"] = file_name
                     int_seq[idx] = current_table.loc[j, "peak_height"]
 
@@ -110,15 +107,15 @@
         
         new_feature_table = current_table.loc[new_feature_idx]
         new_feature_table.index = range(last_file_feature_idx, last_file_feature_idx+len(new_feature_table))
         a = last_file_feature_idx+len(new_feature_table)-1
         feature_table.loc[last_file_feature_idx:a, "m/z"] = new_feature_table["m/z"]
         feature_table.loc[last_file_feature_idx:a, "RT"] = new_feature_table["RT"]
         feature_table.loc[last_file_feature_idx:a, "adduct"] = new_feature_table["adduct"]
-        feature_table.loc[last_file_feature_idx:a, "peak_shape"] = new_feature_table["peak_shape"]
+        feature_table.loc[last_file_feature_idx:a, "noise_level"] = new_feature_table["noise_level"]
         feature_table.loc[last_file_feature_idx:a, "Gaussian_similarity"] = new_feature_table["Gaussian_similarity"]
         feature_table.loc[last_file_feature_idx:a, "charge"] = new_feature_table["charge"]
         feature_table.loc[last_file_feature_idx:a, "isotopes"] = new_feature_table["isotopes"]
         feature_table.loc[last_file_feature_idx:a, "MS2"] = new_feature_table["MS2"]
         feature_table.loc[last_file_feature_idx:a, "alignment_reference"] = file_name
         feature_table.loc[last_file_feature_idx:a, "is_isotope"] = new_feature_table["is_isotope"]
         feature_table.loc[last_file_feature_idx:a, "is_in_source_fragment"] = new_feature_table["is_in_source_fragment"]
@@ -181,153 +178,19 @@
                 print("No raw file found for ", file_name)
                 continue
             else:
                 matched_raw_file_name = matched_raw_file_name[0]
                 d = read_raw_file_to_obj(matched_raw_file_name, int_tol=parameters.int_tol)
                 for i in range(len(feature_table)):
                     if pd.isna(feature_table.loc[i, file_name]):
-                        _, eic_int, _, _ = d.get_eic_data(feature_table.loc[i, "m/z"], feature_table.loc[i, "RT"], parameters.align_mz_tol, parameters.align_rt_tol)
+                        _, eic_int, _, _ = d.get_eic_data(feature_table.loc[i, "m/z"], feature_table.loc[i, "RT"], parameters.align_mz_tol, 0.05)
                         feature_table.loc[i, file_name] = np.max(eic_int)
     return feature_table
 
 
-def feature_alignment_object(path, parameters):
-    """
-    A function to align the features from individual files.
-
-    Parameters
-    ----------------------------------------------------------
-    d_list: list
-        A list of MS data to be aligned.
-    parameters: Params object
-        The parameters for alignment.
-
-    Returns
-    ----------------------------------------------------------
-    feature_table: DataFrame
-        The aligned feature table.
-    """
-
-    # STEP 1: get names of individual files (.csv)
-    csv_file_names = parameters.sample_names
-    csv_file_names = [f + ".csv" for f in csv_file_names]
-    csv_file_names = [os.path.join(path, name) for name in csv_file_names]
-
-    # STEP 2: initiate aligned features
-    feature_list = []
-
-    df = pd.read_csv(csv_file_names[0])
-    for i in range(len(df)):
-        feature = AlignedFeature()
-        feature.extend_feat_from_a_row(df.iloc[i])
-        feature_list.append(feature)
-
-    mz_tol = parameters.align_mz_tol
-    rt_tol = parameters.align_rt_tol
-
-    # STEP 3: read individual feature tables and align features
-    for i in tqdm(range(1, len(csv_file_names))):
-        # read feature table
-        df = pd.read_csv(csv_file_names[i])
-        # sort current table by peak height from high to low
-        df = df.sort_values(by="peak_height", ascending=False)
-
-        mz_seq = np.array([feat.mz for feat in feature_list])
-        rt_seq = np.array([feat.rt for feat in feature_list])
-        int_seq = np.array([feat.highest_roi_intensity for feat in feature_list])
-
-        unmatched_feat = np.ones(len(feature_list), dtype=bool)
-        # compare the m/z and RT of the features
-        for j in range(len(df)):
-            v = np.logical_and(np.abs(mz_seq - df.loc[j, "m/z"]) < mz_tol, np.abs(rt_seq - df.loc[j, "RT"]) < rt_tol)
-            # check if the feature is already in the aligned feature table using tolerance
-            # including parameters.align_mz_tol and parameters.align_rt_tol
-            v = np.where(np.logical_and(v, unmatched_feat))[0]
-            # if the feature is already in the aligned feature table, update the feature
-            if len(v) == 0:
-                feature = AlignedFeature()
-                feature.extend_feat_from_a_row(row=df.iloc[j], front_zeros=[0.0] * i)
-                feature_list.append(feature)
-                continue
-            
-            if len(v) > 1:
-                idx = v[np.argmax(int_seq[v])]
-            else:
-                idx = v[0]
-            
-            feature_list[idx].extend_feat_from_a_row(row=df.iloc[j])
-
-    feature_list.sort(key=lambda x: x.highest_roi_intensity, reverse=True)
-
-    return feature_list
-
-    # STEP 4: output the aligned feature table
-    output_aligned_features(feature_list, parameters.sample_names, parameters.project_dir, int_values="peak_height")
-    
-
-
-
-def feature_alignment_old(feature_list, d):
-    """
-    A function to correct the retention time (RT) of the MS data to be aligned.
-
-    Parameters
-    ----------------------------------------------------------
-    feature_list: list
-        A list of features to be aligned.
-    d: MSData
-        The MS data to be aligned.
-    """
-
-    # Initiate the aligned features using the first MS data if feature_list is empty
-    if len(feature_list) == 0:
-        for roi in d.rois:
-            aligned_feature = AlignedFeature()
-            aligned_feature.extend_feat(roi)
-            feature_list.append(aligned_feature)
-
-        # sort features in feature list by peak height from high to low
-        feature_list.sort(key=lambda x: x.highest_roi_intensity, reverse=True)
-        
-    else:
-        # get the number of features in the feature list
-        existed_file_num = len(feature_list[0].mz_seq)
-
-        mz_seq = np.array([roi.mz for roi in d.rois])
-        rt_seq = np.array([roi.rt for roi in d.rois])
-        int_seq = np.array([roi.peak_height for roi in d.rois])
-        labeled_roi = np.ones(len(d.rois), dtype=bool)
-
-        for feat in feature_list:
-            v = np.logical_and(np.abs(mz_seq - feat.mz) < d.params.align_mz_tol, np.abs(rt_seq - feat.rt) < d.params.align_rt_tol)
-            v = np.where(np.logical_and(v, labeled_roi))[0]
-
-            if len(v) == 0:
-                feat.extend_feat(roi=None)
-                continue
-
-            if len(v) > 1:
-                # select the one with the highest intensity
-                v = v[np.argmax(int_seq[v])]
-            else:
-                v = v[0]
-
-            feat.extend_feat(roi=d.rois[v])
-            labeled_roi[v] = False
-        
-        # For newly detected features, add them to the feature list
-        for i in range(len(labeled_roi)):
-            if labeled_roi[i]:
-                aligned_feature = AlignedFeature()
-                aligned_feature.extend_feat(roi=d.rois[i], front_zeros=[0.0] * existed_file_num)
-                feature_list.append(aligned_feature)
-        
-        feature_list.sort(key=lambda x: x.highest_roi_intensity, reverse=True)
-
-
 class AlignedFeature:
     """
     A class to model an aligned feature from different files.
     """
 
     def __init__(self):
         """
@@ -342,15 +205,14 @@
         self.peak_height_seq = []           # peak height from different files
         self.peak_area_seq = []             # peak area from different files 
         self.top_average_seq = []           # top average from different files
         self.ms2_seq = []                   # MS2 from different files
         self.best_ms2 = None                # the best MS2
         self.reference_file = None          # the reference file
         self.highest_roi_intensity = 0.0    # the highest peak height
-        self.quality = "good"               # quality of the feature
 
         # annotation by MS2 matching
         self.annotation = None              # annotated compound name
         self.annotation_mode = None         # 'identity search' or 'hybrid search'
         self.similarity = None              # similarity score (0-1)
         self.matched_peak_number = None     # number of matched peaks
         self.smiles = None                  # SMILES
@@ -483,266 +345,98 @@
 
     def sum_feature(self, id=None):
         self.id = id
         self.mz_seq = np.array(self.mz_seq)
         self.rt_seq = np.array(self.rt_seq)
         self.mz = np.mean(self.mz_seq[self.mz_seq > 0])
         self.rt = np.mean(self.rt_seq[self.rt_seq > 0])
-        self.quality = self.highest_roi.quality
 
         self.choose_best_ms2()
 
         self.charge_state = self.highest_roi.charge_state
         self.is_isotope = self.highest_roi.is_isotope
         self.isotope_mz_seq = self.highest_roi.isotope_mz_seq
         self.isotope_int_seq = self.highest_roi.isotope_int_seq
         self.is_in_source_fragment = self.highest_roi.is_in_source_fragment
         self.adduct_type = self.highest_roi.adduct_type
 
 
-def summarize_aligned_features(feature_list):
-    """
-    A function to summarize the aligned features.
+# def summarize_aligned_features(feature_list):
+#     """
+#     A function to summarize the aligned features.
 
-    Parameters
-    ----------------------------------------------------------
-    feature_list: list
-        A list of aligned features.   
-    """
+#     Parameters
+#     ----------------------------------------------------------
+#     feature_list: list
+#         A list of aligned features.   
+#     """
 
-    for i, f in enumerate(feature_list):
-        f.sum_feature(i)
+#     for i, f in enumerate(feature_list):
+#         f.sum_feature(i)
 
 
-def output_aligned_features(feature_list, file_names, path, int_values="peak_height"):
-    """
-    A function to output the aligned features.
+# def output_aligned_features(feature_list, file_names, path, int_values="peak_height"):
+#     """
+#     A function to output the aligned features.
 
-    Parameters
-    ----------------------------------------------------------
-    feature_list: list
-        A list of aligned features.
-    output_path: str
-        The path to the output file.
-    """
+#     Parameters
+#     ----------------------------------------------------------
+#     feature_list: list
+#         A list of aligned features.
+#     output_path: str
+#         The path to the output file.
+#     """
 
-    result = []
+#     result = []
 
-    for idx, f in enumerate(feature_list):
+#     for idx, f in enumerate(feature_list):
         
-        iso_dist = ""
-        for i in range(len(f.isotope_mz_seq)):
-            iso_dist += str(np.round(f.isotope_mz_seq[i], decimals=4)) + ";" + str(np.round(f.isotope_int_seq[i], decimals=0)) + "|"
-        iso_dist = iso_dist[:-1]
-
-        ms2 = ""
-        if f.best_ms2 is not None:
-            for i in range(len(f.best_ms2.peaks)):
-                ms2 += str(np.round(f.best_ms2.peaks[i, 0], decimals=4)) + ";" + str(np.round(f.best_ms2.peaks[i, 1], decimals=0)) + "|"
-            ms2 = ms2[:-1]
-
-        if int_values.lower()=="peak_area":
-            int_seq = f.peak_area_seq
-        elif int_values.lower()=="peak_height":
-            int_seq = f.peak_height_seq
-        elif int_values.lower()=="top_average":
-            int_seq = f.top_average_seq
-
-        temp = [idx+1, f.mz, f.rt, ms2, f.charge_state, f.is_isotope, iso_dist,
-                f.is_in_source_fragment, f.adduct_type, f.annotation, f.annotation_mode,
-                f.similarity, f.matched_peak_number, f.smiles, f.inchikey, f.quality]
+#         iso_dist = ""
+#         for i in range(len(f.isotope_mz_seq)):
+#             iso_dist += str(np.round(f.isotope_mz_seq[i], decimals=4)) + ";" + str(np.round(f.isotope_int_seq[i], decimals=0)) + "|"
+#         iso_dist = iso_dist[:-1]
+
+#         ms2 = ""
+#         if f.best_ms2 is not None:
+#             for i in range(len(f.best_ms2.peaks)):
+#                 ms2 += str(np.round(f.best_ms2.peaks[i, 0], decimals=4)) + ";" + str(np.round(f.best_ms2.peaks[i, 1], decimals=0)) + "|"
+#             ms2 = ms2[:-1]
+
+#         if int_values.lower()=="peak_area":
+#             int_seq = f.peak_area_seq
+#         elif int_values.lower()=="peak_height":
+#             int_seq = f.peak_height_seq
+#         elif int_values.lower()=="top_average":
+#             int_seq = f.top_average_seq
+
+#         temp = [idx+1, f.mz, f.rt, ms2, f.charge_state, f.is_isotope, iso_dist,
+#                 f.is_in_source_fragment, f.adduct_type, f.annotation, f.annotation_mode,
+#                 f.similarity, f.matched_peak_number, f.smiles, f.inchikey]
                 
-        temp.extend(int_seq)
+#         temp.extend(int_seq)
 
-        result.append(temp)
+#         result.append(temp)
 
-    # convert result to a pandas dataframe
-    columns = ["id", "mz", "rt", "ms2", "charge_state", "is_isotope", "isotope_dist",
-                "in_source_fragment", "adduct_type", "annotation", "annotation mode", 
-                "similarity_score", "matched_peak_number", "smiles", "inchikey", "quality"]
+#     # convert result to a pandas dataframe
+#     columns = ["id", "mz", "rt", "ms2", "charge_state", "is_isotope", "isotope_dist",
+#                 "in_source_fragment", "adduct_type", "annotation", "annotation mode", 
+#                 "similarity_score", "matched_peak_number", "smiles", "inchikey"]
 
-    file_names_output = [name.split("/")[-1].split(".")[0] for name in file_names]
+#     file_names_output = [name.split("/")[-1].split(".")[0] for name in file_names]
 
-    columns.extend(file_names_output)
-    df = pd.DataFrame(result, columns=columns)
+#     columns.extend(file_names_output)
+#     df = pd.DataFrame(result, columns=columns)
     
-    # save the dataframe to csv file
-    path = path + "aligned_feature_table.csv"
-    df.to_csv(path, index=False)
+#     # save the dataframe to csv file
+#     path = path + "aligned_feature_table.csv"
+#     df.to_csv(path, index=False)
 
 
 # generate an empty feature table with 100000 rows
 def _init_feature_table(rows=5000, sample_names=[]):
     tmp = pd.DataFrame(
-        columns=["ID", "m/z", "RT", "adduct", "is_isotope", "is_in_source_fragment", "peak_shape", "Gaussian_similarity", "charge", "isotopes", "MS2", 
+        columns=["ID", "m/z", "RT", "adduct", "is_isotope", "is_in_source_fragment", "Gaussian_similarity", "noise_level", "charge", "isotopes", "MS2", 
                 "matched_MS2", "search_mode", "annotation", "formula", "similarity", "matched_peak_number", "SMILES", "InChIKey", 
                 "fill_percentage", "alignment_reference"] + sample_names,
         index=range(rows)
     )
-    return tmp
-
-
-
-
-# def feature_alignment(path, parameters):
-#     """
-#     A function to align the features from individual files.
-
-#     Parameters
-#     ----------------------------------------------------------
-#     d_list: list
-#         A list of MS data to be aligned.
-#     parameters: Params object
-#         The parameters for alignment.
-
-#     Returns
-#     ----------------------------------------------------------
-#     feature_table: DataFrame
-#         The aligned feature table.
-#     """
-
-#     # STEP 1: get names of individual files (.csv)
-#     csv_file_names = parameters.sample_names
-#     csv_file_names = [f + ".csv" for f in csv_file_names]
-#     csv_file_names = [os.path.join(path, name) for name in csv_file_names]
-
-#     # STEP 2: initiate aligned features
-#     feature_table = _init_feature_table(sample_names=parameters.sample_names)
-
-#     mz_tol = parameters.align_mz_tol
-#     rt_tol = parameters.align_rt_tol
-
-#     # STEP 3: read individual feature tables and align features
-#     last_file_feature_idx = 0
-#     int_seq = np.zeros(len(feature_table))
-#     for i, file_name in enumerate(tqdm(parameters.sample_names[:2])):
-#         # read feature table
-#         current_table = pd.read_csv(csv_file_names[i])
-#         # sort current table by peak height from high to low
-#         current_table = current_table.sort_values(by="peak_height", ascending=False)
-#         current_table.index = range(len(current_table))
-#         new_feature_idx = []
-
-#         mz_seq = np.array(feature_table["m/z"], dtype=float)
-#         rt_seq = np.array(feature_table["RT"], dtype=float)
-#         mz_to_be_matched = np.array(current_table["m/z"], dtype=float)
-#         rt_to_be_matched = np.array(current_table["RT"], dtype=float)
-#         labeled_v = feature_table[file_name].isna()
-#         # compare the m/z and RT of the features
-#         for j in range(len(current_table)):
-#             v = np.logical_and(np.abs(mz_seq - mz_to_be_matched[j]) < mz_tol, np.abs(rt_seq - rt_to_be_matched[j]) < rt_tol)
-#             # check if the feature is already in the aligned feature table using tolerance
-#             # including parameters.align_mz_tol and parameters.align_rt_tol
-#             v = np.logical_and(v, labeled_v)
-#             v = np.where(v)[0]
-#             # if the feature is already in the aligned feature table, update the feature
-#             if len(v) > 0:
-#                 if len(v) > 1:
-#                     idx = v[np.argmax(int_seq[v])]
-#                 else:
-#                     idx = v[0]
-#                 feature_table.loc[idx, file_name] = current_table.loc[j, "peak_height"]
-#                 # update the m/z and RT of the feature by averaging the values
-#                 feature_table.loc[idx, "m/z"] = (feature_table.loc[idx, "m/z"]*i + current_table.loc[j, "m/z"])/(i+1)
-#                 feature_table.loc[idx, "RT"] = (feature_table.loc[idx, "RT"]*i + current_table.loc[j, "RT"])/(i+1)
-#                 # if the intensity is the largest, update the reference file
-#                 if current_table.loc[j, "peak_height"] == np.max(feature_table.iloc[idx, -len(parameters.sample_names):]):
-#                     feature_table.iloc[idx, 3:12] = [current_table.loc[j, "adduct"], current_table.loc[j, "is_isotope"], 
-#                                                      current_table.loc[j, "is_in_source_fragment"], current_table.loc[j, "peak_shape"], 
-#                                                      current_table.loc[j, "Gaussian_similarity"], current_table.loc[j, "charge"], 
-#                                                      current_table.loc[j, "isotopes"], file_name, current_table.loc[j, "MS2"]]
-#                     feature_table.loc[idx, "alignment_reference"] = file_name
-#                 int_seq[idx] = current_table.loc[j, "peak_height"]
-
-#             # if the feature is not in the aligned feature table, add the feature to the table
-#             elif len(v) == 0:
-#                 new_feature_idx.append(j)
-
-#         # add new features to the aligned feature table
-#         # check if the aligned feature table is full
-#         if last_file_feature_idx + len(new_feature_idx) > len(feature_table):
-#             empty_row = pd.DataFrame(np.nan, index=range(len(new_feature_idx)), columns=feature_table.columns)
-#             feature_table = pd.concat([feature_table, empty_row], ignore_index=True)
-#             int_seq = np.append(int_seq, np.zeros(len(new_feature_idx)))
-        
-#         new_feature_table = current_table.loc[new_feature_idx]
-#         new_feature_table.index = range(last_file_feature_idx, last_file_feature_idx+len(new_feature_table))
-#         a = last_file_feature_idx+len(new_feature_table)-1
-#         feature_table.loc[last_file_feature_idx:a, "m/z"] = new_feature_table["m/z"]
-#         feature_table.loc[last_file_feature_idx:a, "RT"] = new_feature_table["RT"]
-#         feature_table.loc[last_file_feature_idx:a, "adduct"] = new_feature_table["adduct"]
-#         feature_table.loc[last_file_feature_idx:a, "peak_shape"] = new_feature_table["peak_shape"]
-#         feature_table.loc[last_file_feature_idx:a, "Gaussian_similarity"] = new_feature_table["Gaussian_similarity"]
-#         feature_table.loc[last_file_feature_idx:a, "charge"] = new_feature_table["charge"]
-#         feature_table.loc[last_file_feature_idx:a, "isotopes"] = new_feature_table["isotopes"]
-#         feature_table.loc[last_file_feature_idx:a, "MS2"] = new_feature_table["MS2"]
-#         feature_table.loc[last_file_feature_idx:a, "alignment_reference"] = file_name
-#         feature_table.loc[last_file_feature_idx:a, "is_isotope"] = new_feature_table["is_isotope"]
-#         feature_table.loc[last_file_feature_idx:a, "is_in_source_fragment"] = new_feature_table["is_in_source_fragment"]
-#         feature_table.loc[last_file_feature_idx:a, file_name] = new_feature_table["peak_height"]
-#         int_seq[last_file_feature_idx:last_file_feature_idx+len(new_feature_table)] = new_feature_table["peak_height"]
-#         last_file_feature_idx += len(new_feature_table)
-
-
-#     # STEP 4: drop the empty rows and index the feature table
-#     feature_table.dropna(subset=["m/z"], inplace=True)
-#     feature_table['ID'] = range(1, len(feature_table)+1)
-
-#     return feature_table
-
-
-# def _alignement_old(feature_list, d):
-#     """
-#     A function to correct the retention time (RT) of the MS data to be aligned.
-
-#     Parameters
-#     ----------------------------------------------------------
-#     feature_list: list
-#         A list of features to be aligned.
-#     d: MSData
-#         The MS data to be aligned.
-#     """
-
-#     # Initiate the aligned features using the first MS data if feature_list is empty
-#     if len(feature_list) == 0:
-#         for roi in d.rois:
-#             aligned_feature = AlignedFeature()
-#             aligned_feature.extend_feat(roi)
-#             feature_list.append(aligned_feature)
-
-#         # sort features in feature list by peak height from high to low
-#         feature_list.sort(key=lambda x: x.highest_roi_intensity, reverse=True)
-        
-#     else:
-#         # get the number of features in the feature list
-#         existed_file_num = len(feature_list[0].mz_seq)
-
-#         mz_seq = np.array([roi.mz for roi in d.rois])
-#         rt_seq = np.array([roi.rt for roi in d.rois])
-#         int_seq = np.array([roi.peak_height for roi in d.rois])
-#         labeled_roi = np.ones(len(d.rois), dtype=bool)
-
-#         for feat in feature_list:
-#             v = np.logical_and(np.abs(mz_seq - feat.mz) < d.params.align_mz_tol, np.abs(rt_seq - feat.rt) < d.params.align_rt_tol)
-#             v = np.where(np.logical_and(v, labeled_roi))[0]
-
-#             if len(v) == 0:
-#                 feat.extend_feat(roi=None)
-#                 continue
-
-#             if len(v) > 1:
-#                 # select the one with the highest intensity
-#                 v = v[np.argmax(int_seq[v])]
-#             else:
-#                 v = v[0]
-
-#             feat.extend_feat(roi=d.rois[v])
-#             labeled_roi[v] = False
-        
-#         # For newly detected features, add them to the feature list
-#         for i in range(len(labeled_roi)):
-#             if labeled_roi[i]:
-#                 aligned_feature = AlignedFeature()
-#                 aligned_feature.extend_feat(roi=d.rois[i], front_zeros=[0.0] * existed_file_num)
-#                 feature_list.append(aligned_feature)
-        
-#         feature_list.sort(key=lambda x: x.highest_roi_intensity, reverse=True)
+    return tmp
```

### Comparing `masscube-0.0.5/src/masscube/annotation.py` & `masscube-0.0.6/src/masscube/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
             feature_table.loc[i, 'search_mode'] = 'identity_search'
             feature_table.loc[i, 'similarity'] = entropy_similarity[idx]
             feature_table.loc[i, 'matched_peak_number'] = matched_peaks_number[idx]
             feature_table.loc[i, 'SMILES'] = matched['smiles'] if 'smiles' in matched else None
             feature_table.loc[i, 'InChIKey'] = matched['inchikey'] if 'inchikey' in matched else None
             feature_table.loc[i, 'matched_MS2'] = _convert_peaks_to_string(matched['peaks'])
             feature_table.loc[i, 'formula'] = matched['formula'] if 'formula' in matched else None
+            feature_table.loc[i, 'adduct'] = matched['precursor_type']
         else:
             entropy_similarity = entropy_search.hybrid_search(precursor_mz=precursor_mz, peaks=peaks, ms1_tolerance_in_da=parameters.mz_tol_ms1, 
                                                               ms2_tolerance_in_da=parameters.mz_tol_ms2)
             idx = np.argmax(entropy_similarity)
             if entropy_similarity[idx] > parameters.ms2_sim_tol:
                 matched = entropy_search[np.argmax(entropy_similarity)]
                 matched = {k.lower():v for k,v in matched.items()}
@@ -381,8 +382,8 @@
     """
     
     ms2 = ""
     for i in range(len(peaks)):
         ms2 += str(np.round(peaks[i, 0], decimals=4)) + ";" + str(np.round(peaks[i, 1], decimals=4)) + "|"
     ms2 = ms2[:-1]
     
-    return ms2
+    return ms2
```

### Comparing `masscube-0.0.5/src/masscube/feature_grouping.py` & `masscube-0.0.6/src/masscube/feature_grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
         # find roi using isotope list
         for iso in isotopes:
             
             # if isotpoe is not found in two daltons, stop searching
             if iso - last_mz > 2.2:
                 break
 
-            v = np.where(np.logical_and(np.abs(d.roi_mz_seq - iso) < 0.01, np.abs(d.roi_rt_seq - r.rt) < 0.2))[0]
+            v = np.where(np.logical_and(np.abs(d.roi_mz_seq - iso) < 0.01, np.abs(d.roi_rt_seq - r.rt) < 0.05))[0]
 
             if len(v) == 0:
                 continue
 
             # an isotope can't have intensity 3 fold or higher than M0 or 1% lower than the M0
-            v = [v[i] for i in range(len(v)) if d.rois[v[i]].peak_height < 3*r.peak_height]
+            v = [v[i] for i in range(len(v)) if d.rois[v[i]].peak_height < 1.2*r.peak_height]
             v = [v[i] for i in range(len(v)) if d.rois[v[i]].peak_height > 0.01*r.peak_height]
 
             if len(v) == 0:
                 continue
             
             # for high-resolution data, C and N isotopes can be separated and need to be summed
             total_int = np.sum([d.rois[vi].peak_height for vi in v])
@@ -223,16 +223,19 @@
         return 1.0
 
     # find the intensities of the common scans in the two rois
     int1 = roi1.int_seq[np.isin(roi1.scan_idx_seq, common_scans)]
     int2 = roi2.int_seq[np.isin(roi2.scan_idx_seq, common_scans)]
 
     # calculate the correlation
+    # if all values are same, return 1
+    if np.all(int1 == int1[0]) or np.all(int2 == int2[0]):
+        return 1.0
+    
     pp_cor = np.corrcoef(int1, int2)[0, 1]
-
     return pp_cor
 
 
 def get_charge_state(mz_seq):
     
     if len(mz_seq) < 2:
         return 1
```

### Comparing `masscube-0.0.5/src/masscube/feature_table_utils.py` & `masscube-0.0.6/src/masscube/feature_table_utils.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.5/src/masscube/network.py` & `masscube-0.0.6/src/masscube/network.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.5/src/masscube/normalization.py` & `masscube-0.0.6/src/masscube/normalization.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,10 +109,13 @@
     else:
         array = np.array(feature_table.iloc[:, -total_number:-blank_number])
 
     v = find_normalization_factors(array, method=method)
 
     array = sample_normalization_by_factors(array, v)
 
-    feature_table.iloc[:, -total_number:-total_number+array.shape[1]] = array
+    if blank_number == 0:
+        feature_table.iloc[:, -total_number:] = array
+    else:
+        feature_table.iloc[:, -total_number:-total_number+array.shape[1]] = array
 
     return feature_table
```

### Comparing `masscube-0.0.5/src/masscube/params.py` & `masscube-0.0.6/src/masscube/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.rt_range = [0.0, 1000.0]       # RT range in minutes, list of two floats
         self.ion_mode = "positive"          # Ionization mode, "positive" or "negative", character string
 
         # Feature detection
         self.mz_tol_ms1 = 0.01              # m/z tolerance for MS1, default is 0.01
         self.mz_tol_ms2 = 0.015             # m/z tolerance for MS2, default is 0.015
         self.int_tol = 1000                 # Intensity tolerance, default is 30000 for Orbitrap and 1000 for other instruments, integer
-        self.roi_gap = 2                    # Gap within a feature, default is 2 (i.e. 2 consecutive scans without signal), integer
+        self.roi_gap = 50                   # Gap within a feature, default is 2 (i.e. 2 consecutive scans without signal), integer
         self.min_ion_num = 10               # Minimum scan number a feature, default is 10, integer
 
         # Parameters for feature alignment
         self.align_mz_tol = 0.01            # m/z tolerance for MS1, default is 0.01
         self.align_rt_tol = 0.2             # RT tolerance, default is 0.2
 
         # Parameters for feature annotation
@@ -133,25 +133,28 @@
             os.makedirs(self.network_dir)
         if not os.path.exists(self.statistics_dir):
             os.makedirs(self.statistics_dir)
 
         # STEP 4: read the sample table and allocate the sample groups
         #         reorder the samples by qc, sample, and blank
         sample_table = pd.read_csv(os.path.join(self.project_dir, "sample_table.csv"))
-        sample_table.iloc[:, 1] = sample_table.iloc[:, 1].str.lower()
+        try:
+            sample_table.iloc[:, 1] = sample_table.iloc[:, 1].str.lower()
+        except:
+            raise ValueError("The second column of the sample table is not correct.")
         sample_groups_pre = list(set(sample_table.iloc[:, 1]))
         sample_groups = [i for i in sample_groups_pre if i not in ["qc", "blank"]]
         self.sample_group_num = len(sample_groups)
         if "qc" in sample_groups_pre:
             sample_groups = ["qc"] + sample_groups
         if "blank" in sample_groups_pre:
             sample_groups = sample_groups + ["blank"]
 
-        sample_table_new = sample_table[sample_table.iloc[:, 1].str.contains("qc")]
-        for i in range(1,len(sample_groups)):
+        sample_table_new = pd.DataFrame(columns=sample_table.columns)
+        for i in range(len(sample_groups)):
             sample_table_new = pd.concat([sample_table_new, sample_table[sample_table.iloc[:, 1].str.contains(sample_groups[i])]])
         self.sample_names = list(sample_table_new.iloc[:, 0])
         self.sample_groups = sample_groups
         self.individual_sample_groups = []
         for name in self.sample_names:
             self.individual_sample_groups.append(sample_table_new[sample_table_new.iloc[:, 0] == name].iloc[0, 1])
```

### Comparing `masscube-0.0.5/src/masscube/peak_detect.py` & `masscube-0.0.6/src/masscube/peak_detect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,138 @@
 # Author: Hauxu Yu
 
 # A module for feature/peak detection
 
 # Import modules
 import numpy as np
-from tqdm import tqdm
-from scipy.signal import argrelextrema
-from ms_entropy import calculate_entropy_similarity
-import copy
 from scipy.signal import find_peaks
-from scipy.ndimage import uniform_filter1d
+from scipy.ndimage import gaussian_filter1d
+from copy import deepcopy
+from .feature_evaluation import calculate_noise_level
 
+from .feature_evaluation import calculate_gaussian_similarity
 
-def roi_finder(d):
+def find_rois(d):
     """
     A function to find the region of interest (ROI) in the MS data.
 
     Parameters
     ----------------------------------------------------------
     d: MSData object
         An MSData object that contains the MS data.
     """
 
     # A list to store the rois in progress
     rois = []
-    # A list for finally selected ROIs
+    # A list for the finally detected ROIs
     final_rois = []
 
     # Initiate a set of rois using the first MS1 scan
     fs = d.scans[d.ms1_idx[0]]    # The first scan
 
-    # Find the MS2 for this scan
-    allocate_vec = loc_ms2_for_ms1_scan(d, d.ms1_idx[0])
-
     for i in range(len(fs.int_seq)):
         roi = Roi(scan_idx=d.ms1_idx[0], rt=fs.rt, mz=fs.mz_seq[i], intensity=fs.int_seq[i])
-        if allocate_vec[i] > 0:
-            roi.ms2_seq.append(d.scans[allocate_vec[i]])
         rois.append(roi)
     
     last_ms1_idx = d.ms1_idx[0]
     last_rt = fs.rt
 
     # Loop over all MS1 scans
-    for ms1_idx in tqdm(d.ms1_idx[1:]):
+    for ms1_idx in d.ms1_idx[1:]:
 
         s = d.scans[ms1_idx]    # The current MS1 scan
 
-        # Find the MS2 for this scan
-        allocate_vec = loc_ms2_for_ms1_scan(d, ms1_idx)
-
-        visited_idx = []    # A list to store the visited indices of ions in the current MS1 scan
+        visited_idx = []        # A list to store the visited indices of ions in the current MS1 scan
         visited_rois_idx = []   # A list to store the visited indices of rois
 
         # Loop over all current rois
         for i, roi in enumerate(rois):
             
             mz_diff = np.abs(roi.mz_seq[-1] - s.mz_seq)
-
             min_idx = np.argmin(mz_diff)
 
             if mz_diff[min_idx] < d.params.mz_tol_ms1:
                 if min_idx not in visited_idx:
                     roi.extend_roi(scan_idx=ms1_idx, rt=s.rt, mz=s.mz_seq[min_idx], intensity=s.int_seq[min_idx])
-                    
                     roi.gap_counter = 0
-
-                    if allocate_vec[min_idx] > 0:
-                        roi.ms2_seq.append(d.scans[allocate_vec[min_idx]])
                     visited_idx.append(min_idx)
                     visited_rois_idx.append(i)
             
         to_be_moved = []
 
         # Plus one to the gap counter of the rois that are not visited
         for i in range(len(rois)):
             if i not in visited_rois_idx:
-                rois[i].extend_roi(scan_idx=ms1_idx, rt=s.rt, mz=np.nan, intensity=0)
-
+                rois[i].extend_roi(scan_idx=ms1_idx, rt=s.rt, mz=rois[i].mz_seq[-1], intensity=0)
                 rois[i].gap_counter = rois[i].gap_counter + 1
                 if rois[i].gap_counter > d.params.roi_gap:
                     to_be_moved.append(i)
         
         # Move the rois that have not been visited for a long time to final_rois
         for i in to_be_moved[::-1]:
             final_rois.append(rois.pop(i))
         
         # Create new rois for the rest
         for i in range(len(s.int_seq)):
             if i not in visited_idx:
                 # Add a zero before the new roi
                 roi = Roi(scan_idx=last_ms1_idx, rt=last_rt, mz=s.mz_seq[i], intensity=0)
                 roi.extend_roi(scan_idx=ms1_idx, rt=s.rt, mz=s.mz_seq[i], intensity=s.int_seq[i])
-                if allocate_vec[i] > 0:
-                    roi.ms2_seq.append(d.scans[allocate_vec[i]])
                 rois.append(roi)
         last_ms1_idx = ms1_idx
         last_rt = s.rt
            
     # Move all rois to final_rois
     for roi in rois:
         final_rois.append(roi)
 
     return final_rois
 
 
-def find_roi_cut(roi, params):
+def cut_roi(r, int_tol=1000):
     """
-    A function to find place to cut an roi based on ion identity.
-    An roi will be cut only if it has
-    - params.min_ion_num or more non-zero intensities
-    - two or more MS/MS spectra
-
-    Parameters
-    ----------------------------------------------------------
-    roi: Roi object
-        An Roi object that contains the roi.
-    params: Params object
-        A Params object that contains the parameters.
+    Function to cut an ROI by providing the start and end positions.
     """
 
-    # counter the number of non-zero intensities in the roi
-    non_zero_int = np.count_nonzero(roi.int_seq)
+    r.int_seq = np.array(r.int_seq)
+    r.noise_level = calculate_noise_level(r.int_seq)
 
-    if non_zero_int >= params.min_ion_num and len(roi.ms2_seq) >= 2:
+    if r.noise_level > 0.4 or len(r.int_seq) < 10 or r.peak_height < 3*int_tol:
+        return [r]
 
-        cut_positions = argrelextrema(np.array(roi.int_seq), np.less)[0]
+    ss = gaussian_filter1d(r.int_seq, sigma=1)
+    peaks, _ = find_peaks(ss, prominence=np.max(ss)*0.01, distance=5)
 
-        if len(cut_positions) != 0:
-            final_cut_positions = []
-            
-            scan_for_cut = [roi.scan_idx_seq[i] for i in cut_positions]
-            ms2_scan_number = [ms2.scan for ms2 in roi.ms2_seq]
-            indices = np.searchsorted(np.array(ms2_scan_number), np.array(scan_for_cut))
-            ms2_groups = [len(group) for group in np.split(ms2_scan_number, indices)]
-
-            best_ms2s = []
-            a = 0
-            for i in ms2_groups:
-                b = a + i
-                best_ms2s.append(find_best_ms2(roi.ms2_seq[a:b]))
-                a = b            
-
-            ms2_ref = None
-            for i in range(len(best_ms2s)):
-                if best_ms2s[i] is None or best_ms2s[i].peaks.shape[0] == 0:
-                    continue
-                
-                if ms2_ref is None:
-                    ms2_ref = best_ms2s[i]
-                else:
-                    score = calculate_entropy_similarity(ms2_ref.peaks, best_ms2s[i].peaks)
-                    if score < params.ms2_sim_tol:
-                        final_cut_positions.append(cut_positions[i-1])
-                        ms2_ref = best_ms2s[i]
-                    else:
-                        ms2_ref = find_best_ms2([ms2_ref, best_ms2s[i]])
-
-            # cut the roi
-            if len(final_cut_positions) != 0 and len(final_cut_positions) <= 5:
-                return final_cut_positions
-            else:
-                return None
-    else:
-        return None
-
-
-def roi_cutter(roi, positions):
-    """
-    A function to cut a long roi by given positions.
-
-    Parameters
-    ----------------------------------------------------------
-    roi: Roi object
-        An Roi object that contains the roi.
-    positions: list
-        A list of positions to cut the roi.
-    """
+    peaks = peaks[r.int_seq[peaks] > 2*int_tol]
 
-    for i in positions:
-        roi.int_seq[i] = roi.int_seq[i] / 2
+    if len(peaks) < 2:
+        return [r]
 
-    # add a zero and len(int_seq) to positions
-    positions = np.insert(np.array([0, len(roi.int_seq)-1]), 1, positions)
-
-    rois = []
-
-    for i in range(len(positions)-1):
-        fst = positions[i]
-        snd = positions[i+1]+1
-        temp = copy.deepcopy(roi)
-        temp.subset_roi(fst, snd)
-        rois.append(temp)
-
-    return rois
+    if len(peaks) > 4:
+        r.int_seq = np.array(r.int_seq)
+        peaks = np.sort(peaks[np.argsort(r.int_seq[peaks])[-4:]])
     
+    positions = [0]
+    for i in range(len(peaks)-1):
+        lowest_int = 1e10
+        for j in range(peaks[i], peaks[i+1]):
+            if r.int_seq[j] < lowest_int:
+                lowest_int = r.int_seq[j]
+                lowest_int_idx = j
+        positions.append(lowest_int_idx)
+    positions.append(len(r.int_seq)-1)
+    
+    cut_rois = []
+    for i in range(len(positions)-1):
+        tmp = deepcopy(r)
+        tmp.subset_roi(start=positions[i], end=positions[i+1]+1)
+        tmp.cut = True
+        cut_rois.append(tmp)
 
-def loc_ms2_for_ms1_scan(d, ms1_idx):
-    """
-    A function to allocate MS2 scans for the ions in a given MS1 scan.
-
-    Parameters
-    ----------------------------------------------------------
-    d: MSData object
-        An MSData object that contains the MS data.
-    ms1_idx: int
-        The index of the MS1 scan.
-    """
-
-    allocate_vec = [0] * len(d.scans[ms1_idx].mz_seq)
-    mz_vec = d.scans[ms1_idx].mz_seq
-
-    for i in range(ms1_idx+1, len(d.scans)):
-        if d.scans[i].level == 1:
-            break
-        if d.scans[i].level == 2:
-            mz_diff = np.abs(mz_vec - d.scans[i].precursor_mz)
-            if np.min(mz_diff) < 0.01:
-                allocate_vec[np.argmin(mz_diff)] = i
-
-    return allocate_vec
+    return cut_rois
 
 
 class Roi:
     """
     A class to store a region of interest (ROI).
     """
 
@@ -254,26 +163,23 @@
 
         # Count the gaps in the ROI's tail
         self.gap_counter = 0
 
         # Create attributes for the summarized values of the ROI
         self.mz = mz
         self.rt = np.nan
-        self.scan_number = -1
+        self.scan_number = 0
         self.peak_area = np.nan
         self.peak_height = np.nan
-        self.top_average = np.nan
         self.best_ms2 = None
         self.length = 0
-        self.apexes = []
         self.merged = False
         self.gaussian_similarity = 0.0
-
-        # Ceature attributes for roi evaluation
-        self.quality = None
+        self.noise_level = 0.0
+        self.cut = False
         
         # Isotopes
         self.charge_state = 1
         self.is_isotope = False
         self.isotope_mz_seq = []
         self.isotope_int_seq = []
         self.isotope_id_seq = []
@@ -292,14 +198,15 @@
         self.annotation = None
         self.formula = None
         self.similarity = None
         self.matched_peak_number = None
         self.smiles = None
         self.inchikey = None
 
+
     def extend_roi(self, scan_idx, rt, mz, intensity):
         """
         Function to extend an ROI by providing the scan indices, 
         retention time, m/z and intensity.
 
         Parameters
         ----------------------------------------------------------
@@ -314,15 +221,15 @@
         """
 
         # Extend the ROI
         self.scan_idx_seq.append(scan_idx)
         self.rt_seq.append(rt)
         self.mz_seq.append(mz)
         self.int_seq.append(intensity)
-    
+
 
     def show_roi_info(self, show_annotation=False):
         """
         Function to print the information of the ROI.
         """
 
         print(f"ROI: {self.mz:.4f} m/z, {self.rt:.2f} min, {self.peak_area:.2f} area, {self.peak_height:.2f} height")
@@ -342,89 +249,73 @@
             print(f"Isf parent roi id: {self.isf_parent_roi_id}")
 
             print("Adduct information:")
             print(f"Adduct type: {self.adduct_type}")
             print(f"Adduct parent roi id: {self.adduct_parent_roi_id}")
             print(f"Adduct child roi id: {self.adduct_child_roi_id}")
     
-    def roi_mz_error(self):
-        """
-        Function to calculate the m/z error (standard deviation of m/z) of the ROI.
-        """
 
-        return np.nanstd(self.mz_seq)
-
-
-    def find_apex(self):
+    def get_mz_error(self):
         """
-        Function to find the retention time of the ROI.
+        Function to calculate the m/z error (maximum - minimum) of the ROI.
         """
-        
-        tmp = max(range(len(self.int_seq)), key=self.int_seq.__getitem__)
 
-        self.rt = self.rt_seq[tmp]
-        self.scan_number = self.scan_idx_seq[tmp]
-        self.peak_height = int(self.int_seq[tmp])
-        self.mz = self.mz_seq[tmp]
+        return np.max(self.mz_seq) - np.min(self.mz_seq)
 
 
-    def find_roi_area(self):
+    def find_rt_ph_pa(self):
         """
         Function to find the peak area of the ROI using trapzoidal rule.
 
         """
         
-        self.peak_area = int(np.trapz(y=self.int_seq, x=self.rt_seq) * 60) # use seconds to calculate area
+        idx = np.argmax(self.int_seq)
+        self.mz = self.mz_seq[idx]
+        self.rt = self.rt_seq[idx]
+        self.peak_height = self.int_seq[idx]
+        self.peak_area = int(np.trapz(y=self.int_seq, x=self.rt_seq) * 60)
     
 
-    def find_roi_top_average(self, num=3):
+    def find_top_average(self, num=3):
         """
         Function to find the peak height of the ROI by averaging
         the heighest three intensities.
         """
 
         d = np.sort(self.int_seq)[-num:]
         # calculate mean of non-zero values
         d = d[d != 0]
         self.top_average = np.mean(d, dtype=np.int64)
     
 
-    def sum_roi(self):
+    def sum_roi(self, cal_gss=True):
         """
         Function to summarize the ROI to generate attributes.
         """
-
+        self.int_seq = np.array(self.int_seq)
         end_idx = len(self.int_seq)-1
 
         while self.int_seq[end_idx] == 0 and self.int_seq[end_idx-1] == 0:
             end_idx -= 1
 
         end_idx += 1
 
         # keep one zero in the end of ROI
         self.mz_seq = self.mz_seq[:end_idx]
         self.int_seq = self.int_seq[:end_idx]
         self.rt_seq = self.rt_seq[:end_idx]
         self.scan_idx_seq = self.scan_idx_seq[:end_idx]
         
-        self.find_apex()
-        self.find_roi_area()
-        self.find_roi_top_average()
-        self.find_best_ms2()
-
-        tmp = 0
-        if self.int_seq[0] == 0:
-            tmp += 1
-        if self.int_seq[-1] == 0:
-            tmp += 1
-        
-        if self.int_seq[0] == 0:
-            self.mz_seq[0] = np.nan
+        self.find_rt_ph_pa()
+
+        self.noise_level = calculate_noise_level(self.int_seq)
 
-        self.length = len(self.int_seq) - tmp
+        if cal_gss:
+            self.gaussian_similarity = calculate_gaussian_similarity(self.rt_seq, self.int_seq)
+        self.length = np.sum(self.int_seq > 0)
     
 
     def subset_roi(self, start, end):
         """
         Function to subset the ROI by providing the positions.
 
         Parameters
@@ -442,89 +333,8 @@
 
         ms2_seq = []
 
         for ms2 in self.ms2_seq:
             if ms2.scan > self.scan_idx_seq[0] and ms2.scan < self.scan_idx_seq[-1]:
                 ms2_seq.append(ms2)
         
-        self.ms2_seq = ms2_seq
-
-
-    def find_best_ms2(self):
-        """
-        Function to find the best MS2 spectrum of the ROI.
-        """
-
-        self.best_ms2 = find_best_ms2(self.ms2_seq)
-
-
-def find_best_ms2(ms2_seq):
-    """
-    Function to find the best MS2 spectrum for a list of MS2 spectra.
-    """
-
-    if len(ms2_seq) > 0:
-        total_ints = [np.sum(ms2.peaks[:,1]) for ms2 in ms2_seq]
-        if np.max(total_ints) == 0:
-            return None
-        else:
-            return ms2_seq[max(range(len(total_ints)), key=total_ints.__getitem__)]
-    else:
-        return None
-
-
-def apex_detection(retention_times, intensities, merge_peak_rt_tol=0.02, retuen_idx=False, size=30, fold=1.5, find_peak_threh=0.2):
-    """
-    Detection of the apexes within a Region of Interest (ROI).s
-
-    Parameters
-    ----------
-    retention_times : numpy.ndarray
-        Retention times of the data points.
-    intensities : numpy.ndarray
-        Intensities of the data points.
-    """
-
-    # Apply a minimum filter to estimate the baseline
-    baseline = uniform_filter1d(intensities, size=size)*fold
-    substracted = intensities - baseline
-    substracted[substracted < 0] = 0
-    top = np.max(substracted)
-
-    # Detect peaks
-    peaks, _ = find_peaks(substracted, height=top*find_peak_threh)
-
-    if len(peaks)==0:
-        return []
-
-    peak_rts = [retention_times[i] for i in peaks]
-    peak_ints = [intensities[i] for i in peaks]
-
-    # merge peaks that are too close and keep the higher one
-    if merge_peak_rt_tol is not None:
-        merged_rts = []
-        merged_ints = []
-        merged_idx = []
-
-        merged_rts.append(peak_rts[0])
-        merged_ints.append(peak_ints[0])
-        merged_idx.append(peaks[0])
-
-        for i in range(1, len(peak_rts)):
-            if peak_rts[i] - merged_rts[-1] > merge_peak_rt_tol:
-                merged_rts.append(peak_rts[i])
-                merged_ints.append(peak_ints[i])
-                merged_idx.append(peaks[i])
-            else:
-                if peak_ints[i] > merged_ints[-1]:
-                    merged_ints[-1] = peak_ints[i]
-                    merged_rts[-1] = peak_rts[i]
-                    merged_idx[-1] = peaks[i]
-
-        peak_rts = merged_rts
-        peak_ints = merged_ints
-        peaks = merged_idx
-
-    if retuen_idx:
-        return peaks
-    else:
-        return [[retention_times[i], intensities[i]] for i in peaks]
+        self.ms2_seq = ms2_seq
```

### Comparing `masscube-0.0.5/src/masscube/raw_data_utils.py` & `masscube-0.0.6/src/masscube/raw_data_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # A module to read and process the raw MS data
 # Classes are defined in order to handle the data
 
 # Import modules
 from pyteomics import mzml, mzxml
 import numpy as np
 import os
-from . import peak_detect
 import matplotlib.pyplot as plt
 import pandas as pd
+from datetime import datetime
 
-from .feature_evaluation import calculate_gaussian_similarity
 from .params import Params
+from .peak_detect import find_rois, cut_roi
 
 
 class MSData:
     """
     A class that models a single file (mzML or mzXML) and
     processes the raw data.
 
@@ -41,17 +41,18 @@
         self.ms1_rt_seq = []        # Retention times of all MS1 scans
         self.bpc_int = []           # Intensity of the BPC
         self.rois = []              # A list of ROIs
         self.params = None          # A Params object
         self.file_name = None       # File name of the raw data without extension
         self.roi_mz_seq = None      # m/z of all ROIs
         self.roi_rt_seq = None      # Retention time of all ROIs
+        self.start_time = None      # Start acquisition time of the raw data
 
 
-    def read_raw_data(self, file_name, params):
+    def read_raw_data(self, file_name, params, centroid=True):
         """
         Function to read raw data to MS1 and MS2 (if available)
         (supported by pyteomics package).
 
         Parameters
         ----------------------------------------------------------
         file_name: str
@@ -62,29 +63,32 @@
 
         self.params = params
 
         if os.path.isfile(file_name):
             # get extension from file name
             ext = os.path.splitext(file_name)[1]
 
+            if ext.lower() != ".mzml" and ext.lower() != ".mzxml":
+                raise ValueError("Unsupported raw data format. Raw data must be in mzML or mzXML.")
+
             self.file_name = os.path.splitext(os.path.basename(file_name))[0]
 
+            self.start_time = get_start_time(file_name)
+
             if ext.lower() == ".mzml":
                 with mzml.MzML(file_name) as reader:
-                    self.extract_scan_mzml(reader)
+                    self.extract_scan_mzml(reader, centroid)
             elif ext.lower() == ".mzxml":
                 with mzxml.MzXML(file_name) as reader:
-                    self.extract_scan_mzxml(reader)
-            else:
-                print("Unsupported raw data format. Raw data must be in mzML or mzXML.")
+                    self.extract_scan_mzxml(reader, centroid)
         else:
             print("File does not exist.")
 
 
-    def extract_scan_mzml(self, spectra):
+    def extract_scan_mzml(self, spectra, centroid=True):
         """
         Function to extract all scans and convert them to Scan objects.
 
         Parameters
         ----------------------------------------------------------
         spectra: pyteomics object
             An iteratable object that contains all MS1 and MS2 scans.
@@ -109,15 +113,16 @@
 
             # Check if the retention time is within the range
             if self.params.rt_range[0] < rt < self.params.rt_range[1]:
                 if spec['ms level'] == 1:
                     temp_scan = Scan(level=1, scan=idx, rt=rt)
                     mz_array = spec['m/z array']
                     int_array = spec['intensity array']
-                    mz_array, int_array = _centroid(mz_array, int_array)
+                    if centroid:
+                        mz_array, int_array = _centroid(mz_array, int_array)
 
                     temp_scan.add_info_by_level(mz_seq=mz_array, int_seq=int_array)
                     self.ms1_idx.append(idx)
 
                     # update base peak chromatogram
                     self.bpc_int.append(np.max(spec['intensity array']))
                     self.ms1_rt_seq.append(rt)
@@ -130,15 +135,15 @@
                     _clean_ms2(temp_scan)
                     self.ms2_idx.append(idx)
                 
                 self.scans.append(temp_scan)
                 idx += 1
 
 
-    def extract_scan_mzxml(self, spectra):
+    def extract_scan_mzxml(self, spectra, centroid=True):
         """
         Function to extract all scans and convert them to Scan objects.
 
         Parameters
         ----------------------------------------------------------
         spectra: pyteomics object
             An iteratable object that contains all MS1 and MS2 scans.
@@ -160,15 +165,16 @@
 
             # Check if the retention time is within the range
             if self.params.rt_range[0] < rt < self.params.rt_range[1]:
                 if spec['msLevel'] == 1:
                     temp_scan = Scan(level=1, scan=idx, rt=rt)
                     mz_array = spec['m/z array']
                     int_array = spec['intensity array']
-                    mz_array, int_array = _centroid(mz_array, int_array)
+                    if centroid:
+                        mz_array, int_array = _centroid(mz_array, int_array)
 
                     temp_scan.add_info_by_level(mz_seq=mz_array, int_seq=int_array)
                     self.ms1_idx.append(idx)
 
                     # update base peak chromatogram
                     self.bpc_int.append(np.max(spec['intensity array']))
                     self.ms1_rt_seq.append(rt)
@@ -206,109 +212,67 @@
 
         Parameters
         ----------------------------------------------------------
         params: Params object
             A Params object that contains the parameters.
         """
 
-        self.rois = peak_detect.roi_finder(self)
+        self.rois = find_rois(self)
     
 
-    def cut_rois(self, return_cut_rois=False):
+    def cut_rois(self):
         """
         Function to cut ROI into smaller pieces.
         """
 
-        small_rois = []
-        to_be_removed = []
-
-        pairs = []
-        for i, roi in enumerate(self.rois):
-            
-            positions = peak_detect.find_roi_cut(roi, self.params)
-            
-            if positions is not None:
-
-                # append each item in a list to small_rois
-                small_rois_tmp = peak_detect.roi_cutter(roi, positions)
-                small_rois.extend(small_rois_tmp)
-                to_be_removed.append(i)
-
-                pairs.append([roi, small_rois_tmp])
-        
-        # remove the original rois
-        for i in sorted(to_be_removed, reverse=True):
-            del self.rois[i]
-
-        # append the small rois to the original rois
-        self.rois.extend(small_rois)
-
-        if return_cut_rois:
-            return pairs
-    
-
-    def merge_rois(self):
-        """
-        Function to merge ROIs.
-        """
-
+        self.rois = [cut_roi(r, int_tol=self.params.int_tol) for r in self.rois]
+        tmp = []
         for roi in self.rois:
-            roi.sum_roi()
-        # sort rois by m/z
-        self.rois = sorted(self.rois, key=lambda x: x.mz)
+            tmp.extend(roi)
 
-        mz_arr = np.array([roi.mz for roi in self.rois])
-        grouped_arr = _group_by_threshold(mz_arr, 0.003)
-
-        merged_rois = []
-        for g in grouped_arr:
-            if len(g) == 1:
-                merged_rois.append(self.rois[g[0]])
-            else:
-                _merge_roi(self, g, merged_rois)
-
-        self.rois = merged_rois
+        self.rois = tmp
 
 
-    def summarize_roi(self):
+    def summarize_roi(self, cal_gss=True):
         """
         Function to process ROIs.
 
         Parameters
         ----------------------------------------------------------
         params: Params object
             A Params object that contains the parameters.
         """      
 
         for roi in self.rois:
-            roi.sum_roi()
-            roi.int_seq = np.array(roi.int_seq)
-            
-            # For long ROIs: further detect the local maxima
-            if roi.length < self.params.min_ion_num:
-                roi.quality = 'short'
-            else:
-                roi.quality = 'good'
-                roi.apexes = peak_detect.apex_detection(roi.rt_seq, roi.int_seq)
-            
-            roi.gaussian_similarity = calculate_gaussian_similarity(roi.rt_seq, roi.int_seq)
-
-            # find the best MS2
-            roi.find_best_ms2()
+            roi.sum_roi(cal_gss=cal_gss)
 
         # sort rois by m/z
         self.rois.sort(key=lambda x: x.mz)
 
         # index the rois
         for idx in range(len(self.rois)):
             self.rois[idx].id = idx
-        
+
         # extract mz and rt of all rois for further use (feature grouping)
         self.roi_mz_seq = np.array([roi.mz for roi in self.rois])
         self.roi_rt_seq = np.array([roi.rt for roi in self.rois])
+
+        # allocate ms2 to rois
+        for i in self.ms2_idx:
+            idx = np.where(np.abs(self.roi_mz_seq - self.scans[i].precursor_mz) < self.params.mz_tol_ms2)[0]
+            for j in idx:
+                if self.rois[j].rt_seq[0] < self.scans[i].rt < self.rois[j].rt_seq[-1]:
+                    self.rois[j].ms2_seq.append(self.scans[i])
+                    break
+
+        # find best ms2 for each roi
+        for roi in self.rois:
+            if len(roi.ms2_seq) > 0:
+                roi.best_ms2 = find_best_ms2(roi.ms2_seq)
+        
     
     def drop_rois_without_ms2(self):
         """
         Function to drop ROIs without MS2.
         """
 
         self.rois = [roi for roi in self.rois if len(roi.ms2_seq) > 0]
@@ -380,41 +344,31 @@
             iso_dist = iso_dist[:-1]
 
             ms2 = ""
             if roi.best_ms2 is not None:
                 for i in range(len(roi.best_ms2.peaks)):
                     ms2 += str(np.round(roi.best_ms2.peaks[i, 0], decimals=4)) + ";" + str(np.round(roi.best_ms2.peaks[i, 1], decimals=0)) + "|"
                 ms2 = ms2[:-1]
-            
-            apexes = ""
-            if len(roi.apexes) > 1 and len(roi.apexes) < 5:
-                for i in range(len(roi.apexes)):
-                    apexes += str(np.round(roi.apexes[i][0] , decimals=3)) + ";" + str(np.round(roi.apexes[i][1], decimals=4)) + "|"
-                apexes = apexes[:-1]
 
             temp = [roi.id, roi.mz.__round__(4), roi.rt.__round__(3), roi.length, roi.rt_seq[0],
-                    roi.rt_seq[-1], roi.peak_area, roi.peak_height,
-                    roi.top_average, apexes, roi.gaussian_similarity, roi.quality,
-                    roi.charge_state, roi.is_isotope, str(roi.isotope_id_seq)[1:-1], iso_dist,
+                    roi.rt_seq[-1], roi.peak_area, roi.peak_height, roi.gaussian_similarity.__round__(2), 
+                    roi.noise_level.__round__(2), roi.charge_state, roi.is_isotope, str(roi.isotope_id_seq)[1:-1], iso_dist,
                     roi.is_in_source_fragment, roi.isf_parent_roi_id, str(roi.isf_child_roi_id)[1:-1],
                     roi.adduct_type, roi.adduct_parent_roi_id, str(roi.adduct_child_roi_id)[1:-1],
                     ]
             
             temp.extend([ms2, roi.annotation, roi.formula, roi.similarity, roi.matched_peak_number, roi.smiles, roi.inchikey])
 
             result.append(temp)
 
         # convert result to a pandas dataframe
-        columns = [ "ID", "m/z", "RT", "length", "RT_start",
-                    "RT_end", "peak_area", "peak_height",
-                    "top_average", "apexes", "Gaussian_similarity",
-                    "peak_shape", "charge", "is_isotope", "isotope_IDs",
-                    "isotopes", "is_in_source_fragment",
-                    "ISF_parent_ID", "ISF_child_ID", "adduct",
-                    "adduct_base_ID", "adduct_other_ID"]
+        columns = [ "ID", "m/z", "RT", "length", "RT_start", "RT_end", "peak_area", "peak_height",
+                    "Gaussian_similarity", "noise_level", "charge", "is_isotope", "isotope_IDs", "isotopes", "is_in_source_fragment",
+                    "ISF_parent_ID", "ISF_child_ID", "adduct", "adduct_base_ID", "adduct_other_ID"]
+                    
         
         columns.extend(["MS2", "annotation", "formula", "similarity", "matched_peak_number", "SMILES", "InChIKey"])
 
         df = pd.DataFrame(result, columns=columns)
         
         # save the dataframe to csv file
         if user_defined_output_path:
@@ -423,15 +377,15 @@
             path = os.path.join(self.params.single_file_dir)
             if not os.path.exists(path):
                 os.makedirs(path)
             path = os.path.join(self.params.single_file_dir, self.file_name + ".csv")
         df.to_csv(path, index=False)
     
 
-    def get_eic_data(self, target_mz, target_rt=None, mz_tol=0.005, rt_tol=0.3):
+    def get_eic_data(self, target_mz, target_rt=None, mz_tol=0.005, rt_tol=0.3, rt_range=None):
         """
         To get the EIC data of a target m/z.
 
         Parameters
         ----------
         target_mz: float
             Target m/z.
@@ -455,18 +409,18 @@
         """
 
         eic_rt = []
         eic_int = []
         eic_mz = []
         eic_scan_idx = []
 
-        if target_rt is None:
-            rt_range = [0, np.inf]
-        else:
+        if target_rt is not None:
             rt_range = [target_rt - rt_tol, target_rt + rt_tol]
+        elif rt_range is None:
+            rt_range = [0, np.inf]
 
         for i in self.ms1_idx:
             if self.scans[i].rt > rt_range[0] and self.scans[i].rt < rt_range[1]:
                 mz_diff = np.abs(self.scans[i].mz_seq - target_mz)
                 if len(mz_diff)>0 and np.min(mz_diff) < mz_tol:
                     eic_rt.append(self.scans[i].rt)
                     eic_int.append(self.scans[i].int_seq[np.argmin(mz_diff)])
@@ -632,27 +586,24 @@
             plt.close()
             return None
         else:
             plt.show()
             return eic_rt[np.argmax(eic_int)], np.max(eic_int), eic_scan_idx[np.argmax(eic_int)]
 
 
-    def plot_all_rois(self, output_path, mz_tol=0.01, rt_range=[0, np.inf], rt_window=None, quality=None):
+    def plot_all_rois(self, output_path, mz_tol=0.01, rt_range=[0, np.inf], rt_window=None):
         """
         Function to plot EIC of all ROIs.
         """
 
         if output_path[-1] != "/":
             output_path += "/"
 
         for idx, roi in enumerate(self.rois):
 
-            if quality and roi.quality != quality:
-                continue
-
             if rt_window is not None:
                 rt_range = [roi.rt_seq[0] - rt_window, roi.rt_seq[-1] + rt_window]
 
             # get the eic data
             eic_rt, eic_int, _, eic_scan_idx = self.get_eic_data(roi.mz, mz_tol=mz_tol, rt_range=rt_range)
             idx_start = np.where(eic_scan_idx == roi.scan_idx_seq[0])[0][0]
             idx_end = np.where(eic_scan_idx == roi.scan_idx_seq[-1])[0][0] + 1
@@ -664,43 +615,20 @@
             plt.fill_between(eic_rt[idx_start:idx_end], eic_int[idx_start:idx_end], color="black", alpha=0.2)
             plt.axvline(x = roi.rt, color = 'b', linestyle = '--', linewidth=1)
             plt.xlabel("Retention Time (min)", fontsize=18, fontname='Arial')
             plt.ylabel("Intensity", fontsize=18, fontname='Arial')
             plt.xticks(fontsize=14, fontname='Arial')
             plt.yticks(fontsize=14, fontname='Arial')
             plt.text(eic_rt[0], np.max(eic_int)*0.95, "m/z = {:.4f}".format(roi.mz), fontsize=12, fontname='Arial')
-            plt.text(eic_rt[0] + (eic_rt[-1]-eic_rt[0])*0.2, np.max(eic_int)*0.95, "Quality = {}".format(roi.quality), fontsize=12, fontname='Arial', color="blue")
             plt.text(eic_rt[0] + (eic_rt[-1]-eic_rt[0])*0.6, np.max(eic_int)*0.95, self.file_name, fontsize=10, fontname='Arial', color="gray")
 
             file_name = output_path + "roi{}_".format(idx) + str(roi.mz.__round__(4)) + ".png"
 
             plt.savefig(file_name, dpi=300, bbox_inches="tight")
             plt.close()
-    
-
-    def sum_roi_quality(self):
-        """
-        Function to calculate the sum of all ROI qualities.
-        """
-
-        counter1 = 0
-        counter2 = 0
-        counter3 = 0
-
-        for r in self.rois:
-            if r.quality == "good":
-                counter1 += 1
-            elif r.quality == "short":
-                counter2 += 1
-            elif r.quality == "bad peak shape":
-                counter3 += 1
-        
-        print("Number of good ROIs: " + str(counter1))
-        print("Number of short ROIs: " + str(counter2))
-        print("Number of bad peak shape ROIs: " + str(counter3))
 
 
 class Scan:
     """
     A class that represents a MS scan.
     A MS1 spectrum has properties including:
         scan number, retention time, 
@@ -771,15 +699,15 @@
 
         elif self.level == 2:
             # keep 4 decimal places for m/z and 0 decimal place for intensity
             print("Precursor m/z: " + str(np.round(self.precursor_mz, decimals=4)))
             print(self.peaks)
     
 
-    def plot_scan(self, mz_range=None):
+    def plot_scan(self, mz_range=None, return_data=False):
         """
         Function to plot a scan.
         
         Parameters
         ----------------------------------------------------------
         """
 
@@ -804,94 +732,31 @@
         plt.hlines(y = 0, xmin = mz_range[0], xmax = mz_range[1], color="black", linewidth=1.5)
         plt.xlabel("m/z, Dalton", fontsize=18, fontname='Arial')
         plt.ylabel("Intensity", fontsize=18, fontname='Arial')
         plt.xticks(fontsize=14, fontname='Arial')
         plt.yticks(fontsize=14, fontname='Arial')
         plt.show()
 
+        if return_data:
+            return x, y
 
-def _clean_ms2(ms2, offset=0):
+
+def _clean_ms2(ms2, offset=2):
     """
     A function to clean MS/MS by
     1. Drop ions with m/z > (precursor_mz - offset)   
     2. Drop ions with intensity < 1% of the base peak intensity
     """
     
     if ms2.peaks.shape[0] > 0:
         ms2.peaks = ms2.peaks[ms2.peaks[:, 0] < ms2.precursor_mz - offset]
     if ms2.peaks.shape[0] > 0:
         ms2.peaks = ms2.peaks[ms2.peaks[:, 1] > 0.01 * np.max(ms2.peaks[:, 1])]
 
 
-def _group_by_threshold(arr, threshold):
-    groups = []
-    current_group = [0]  # Start with the first element
-
-    for i in range(1, len(arr)):
-        if arr[i] - arr[i-1] < threshold:
-            current_group.append(i)
-        else:
-            groups.append(current_group)
-            current_group = [i]
-    groups.append(current_group)  # Add the last group
-    return groups
-
-
-def _merge_roi(d, g, merged_rois):
-
-    current_roi_group = [d.rois[g[i]] for i in range(len(g))]
-    # reorder currect roi group by retention time
-    current_roi_group = sorted(current_roi_group, key=lambda x: x.rt)
-    current_merged = [0]
-    check = False
-    if current_roi_group[0].peak_height > 3*d.params.int_tol:
-        check = True
-    for i in range(1, len(current_roi_group)):
-        if (current_roi_group[i].peak_height > 3*d.params.int_tol and check) or (current_roi_group[i].rt_seq[0] - current_roi_group[i-1].rt_seq[-1] > 0.5):
-            merged_rois.append(_connect_rois([current_roi_group[j] for j in current_merged]))
-            current_merged = [i]
-            if current_roi_group[i].peak_height > 3*d.params.int_tol:
-                check = True
-            else:
-                check = False
-            continue
-        current_merged.append(i)
-        if current_roi_group[i].peak_height > 3*d.params.int_tol:
-            check = True
-    merged_rois.append(_connect_rois([current_roi_group[j] for j in current_merged]))
-
-
-def _connect_rois(rois):
-    output = rois[0]
-    for i in range(1, len(rois)):
-        output.rt_seq.extend(rois[i].rt_seq)
-        output.int_seq.extend(rois[i].int_seq)
-        output.mz_seq.extend(rois[i].mz_seq)
-        output.ms2_seq.extend(rois[i].ms2_seq)
-        output.scan_idx_seq.extend(rois[i].scan_idx_seq)
-    
-    order = np.argsort(output.scan_idx_seq)
-    output.rt_seq = [output.rt_seq[i] for i in order]
-    output.int_seq = [output.int_seq[i] for i in order]
-    output.mz_seq = [output.mz_seq[i] for i in order]
-    output.scan_idx_seq = [output.scan_idx_seq[i] for i in order]
-        
-    i = len(output.scan_idx_seq) - 1
-
-    while i > 0:
-        if output.scan_idx_seq[i] == output.scan_idx_seq[i-1]:
-            output.scan_idx_seq.pop(i)
-            output.rt_seq.pop(i)
-            output.int_seq[i-1] += output.int_seq.pop(i)
-            output.mz_seq.pop(i)
-        i -= 1
-    output.merged = True
-    return output
-
-
 def _centroid(mz_seq, int_seq, centroiding_mz_tol=0.005):
     """
     Function to centroid the m/z and intensity sequences.
 
     Parameters
     ----------
     mz_seq: numpy array or list
@@ -907,42 +772,90 @@
 
     if len(tmp) == 0:
         return mz_seq, int_seq
     
     mz_seq = list(mz_seq)
     int_seq = list(int_seq)
     for i in tmp[::-1]:
-        int_seq[i] += int_seq[i+1]
         mz_seq[i] = (mz_seq[i]*int_seq[i] + mz_seq[i+1]*int_seq[i+1]) / (int_seq[i] + int_seq[i+1])
+        int_seq[i] += int_seq[i+1]
         mz_seq.pop(i+1)
         int_seq.pop(i+1)
 
-    return mz_seq, int_seq
+    return np.array(mz_seq), int_seq
 
 
-def read_raw_file_to_obj(file_name, params=None, int_tol=0.0, print_summary=False):
+def read_raw_file_to_obj(file_name, params=None, int_tol=0.0, centroid=True, print_summary=False):
     """
     Read a raw file to a MSData object.
     It's a useful function for data visualization or brief data analysis.
 
     Parameters
     ----------
     file_name : str
         The file name of the raw file.
+    params : Params object
+        A Params object that contains the parameters.
+    int_tol : float
+        Intensity tolerance for dropping ions.
+    centroid : bool
+        True: centroid the raw data.
+        False: do not centroid the raw data.
+    print_summary : bool
+        True: print the summary of the raw data.
+        False: do not print the summary of the raw data.
+
+    Returns
+    -------
+    d : MSData object
+        A MSData object.
     """
 
     # create a MSData object
     d = MSData()
 
     # read raw data
     if params is None:
         params = Params()
-    d.read_raw_data(file_name, params)
+    d.read_raw_data(file_name, params, centroid)
 
     if int_tol > 0:
         d.params.int_tol = int_tol
         d.drop_ion_by_int()
     
     if print_summary:
         print("Number of MS1 scans: " + str(len(d.ms1_idx)), "Number of MS2 scans: " + str(len(d.ms2_idx)))
     
-    return d
+    return d
+
+
+def find_best_ms2(ms2_seq):
+    """
+    Function to find the best MS2 spectrum for a list of MS2 spectra.
+    """
+
+    if len(ms2_seq) > 0:
+        total_ints = [np.sum(ms2.peaks[:,1]) for ms2 in ms2_seq]
+        if np.max(total_ints) == 0:
+            return None
+        else:
+            return ms2_seq[max(range(len(total_ints)), key=total_ints.__getitem__)]
+    else:
+        return None
+
+
+def get_start_time(file_name):
+    """
+    Function to get the start time of the raw data.
+
+    Parameters
+    ----------
+    file_name : str
+        Absolute path of the raw data.
+    """
+
+    with open(file_name, "rb") as f:
+        for l in f:
+            l = str(l)
+            if "startTimeStamp" in str(l):
+                t = l.split("startTimeStamp")[1].split('"')[1]
+                return datetime.strptime(t, "%Y-%m-%dT%H:%M:%SZ")
```

### Comparing `masscube-0.0.5/src/masscube/stats.py` & `masscube-0.0.6/src/masscube/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # A module for statistical analysis
 
 # imports
 from scipy.stats import ttest_ind, false_discovery_control, f_oneway
 import numpy as np
 import os
 
-def statistical_analysis(feature_table, params):
+def statistical_analysis(feature_table, params, before_norm=False):
     """
     1. Univariate analysis (t-test and p-value adjustment for two groups; ANOVA and p-value adjustment for multiple groups)
     2. Multivariate analysis (PCA)
 
     Parameters
     ----------
     feature_table : pandas DataFrame
@@ -26,28 +26,26 @@
     data_array = np.array(feature_table[v], dtype=int)
 
     s = len(params.sample_groups) - 2
     v = np.array([i for i in params.individual_sample_groups if i not in ['qc', 'blank']])
 
     if s == 2:
         p_values = t_test(data_array, v)
-        # feature_table['t_test_p_adjusted'] = adjusted_p_values
     elif s > 2:
         p_values = anova(data_array, v)
-        # feature_table['ANOVA_p_adjusted'] = adjusted_p_values
 
-    else:
+    elif s == 1 and before_norm==False:
         print("No statistical analysis is performed since only one group is found.")
 
     # for PCA analysis, the QC samples should also be included
     v = [params.sample_names[i] for i in range(len(params.individual_sample_groups)) if params.individual_sample_groups[i] not in ['blank']]
     data_array = feature_table[v].values
     v = np.array([i for i in params.individual_sample_groups if i not in ['blank']])
 
-    pca_analysis(data_array, v, output_dir=params.statistics_dir)
+    pca_analysis(data_array, v, output_dir=params.statistics_dir, before_norm=before_norm)
 
     if s == 2:
         feature_table['t_test_p'] = p_values
     elif s > 2:
         feature_table['ANOVA_p'] = p_values
     
     return feature_table
@@ -76,15 +74,19 @@
         print("The number of sample groups is not equal to 2.")
         return None
     
     v1 = individual_sample_groups == sample_groups[0]
     v2 = individual_sample_groups == sample_groups[1]
 
     for i in range(len(data_array)):
-        p_values.append(ttest_ind(data_array[i, v1], data_array[i, v2]).pvalue)
+        # if all values are equal, the p-value will be 1
+        if np.all(data_array[i] == data_array[i, 0]):
+            p_values.append(1)
+        else:
+            p_values.append(ttest_ind(data_array[i, v1], data_array[i, v2]).pvalue)
     
     # adjusted_p_values = false_discovery_control(p_values)
 
     return p_values
 
 
 def anova(data_array, individual_sample_groups):
@@ -107,29 +109,32 @@
     sample_groups = list(set(individual_sample_groups))
 
     if len(sample_groups) < 2:
         print("The number of sample groups is less than 2.")
         return None
     
     for i in range(len(data_array)):
-        p_values.append(f_oneway(*[data_array[i, individual_sample_groups == g] for g in sample_groups]).pvalue)
+        if np.all(data_array[i] == data_array[i, 0]):
+            p_values.append(1)
+        else:
+            p_values.append(f_oneway(*[data_array[i, individual_sample_groups == g] for g in sample_groups]).pvalue)
     
     # adjusted_p_values = false_discovery_control(p_values)
 
     return p_values
 
 
 import numpy as np
 from sklearn.decomposition import PCA
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 from .visualization import plot_pca
 
 
-def pca_analysis(data_array, individual_sample_groups, scaling=True, transformation=True, gapFillingRatio=0.2, output_dir=None):
+def pca_analysis(data_array, individual_sample_groups, scaling=True, transformation=True, gapFillingRatio=0.2, output_dir=None, before_norm=False):
     """
     Principal component analysis (PCA) analysis.
 
     Parameters
     ----------
     data_array : numpy array
         The feature intensities.
@@ -157,21 +162,26 @@
 
     # transformation by log10
     if transformation:
         X = np.log10(X)
 
     # scaling
     if scaling:
-        X = (X - np.mean(X, axis=0)) / np.std(X, axis=0)
+        X = (X - np.mean(X, axis=1).reshape(-1, 1)) / np.std(X, axis=1).reshape(-1, 1)
     
     # PCA analysis
     X = X.transpose()
     pca = PCA(n_components=2)
     pca.fit(X)
     var_PC1, var_PC2 = pca.explained_variance_ratio_
     vecPC1 = pca.transform(X)[:,0]
     vecPC2 = pca.transform(X)[:,1]
 
     if output_dir is not None:
-        output_dir = os.path.join(output_dir, "PCA.png")
+        if before_norm:
+            output_dir = os.path.join(output_dir, "PCA_before_normalization.png")
+        else:
+            output_dir = os.path.join(output_dir, "PCA.png")
 
     plot_pca(vecPC1, vecPC2, var_PC1, var_PC2, individual_sample_groups, output_dir)
+
+    return vecPC1, vecPC2, var_PC1, var_PC2
```

### Comparing `masscube-0.0.5/src/masscube/utils_functions.py` & `masscube-0.0.6/src/masscube/utils_functions.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.5/src/masscube/visualization.py` & `masscube-0.0.6/src/masscube/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # A module for data visualization.
 
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import random
 import numpy as np
 import os
+import re
 
 from .annotation import _extract_peaks_from_string
 
 def plot_bpcs(data_list=None, output=None, autocolor=False):
     """
     A function to plot the base peak chromatograms (overlapped) of a list of data.
     
@@ -50,50 +51,52 @@
     color = random.choice(list(mcolors.CSS4_COLORS.keys()))
     return color
 
 
 _color_list = ["red", "blue", "green", "orange", "purple", "brown", "pink", "gray", "olive", "cyan"]
 
 
-def plot_roi(d, roi, mz_tol=0.005, rt_tol=1.0, output=False, break_scan=None, label_quality=True):
+def plot_roi(d, roi, mz_tol=0.005, rt_tol=1.0, output=False, break_scan=None):
     """
     Function to plot EIC of a target m/z.
     """
-    if rt_tol < roi.rt_seq[-1] - roi.rt or rt_tol < roi.rt - roi.rt_seq[0]:
-        rt_tol = max(roi.rt_seq[-1] - roi.rt, roi.rt - roi.rt_seq[0]) + 1.0
+    rt_range = [roi.rt_seq[0]-rt_tol, roi.rt_seq[-1]+rt_tol]
     # get the eic data
-    eic_rt, eic_int, _, eic_scan_idx = d.get_eic_data(target_mz=roi.mz, target_rt=roi.rt, mz_tol=mz_tol, rt_tol=rt_tol)
+    eic_rt, eic_int, _, eic_scan_idx = d.get_eic_data(target_mz=roi.mz, rt_range=rt_range, mz_tol=mz_tol)
     idx_start = np.where(eic_scan_idx == roi.scan_idx_seq[0])[0][0]
     idx_end = np.where(eic_scan_idx == roi.scan_idx_seq[-1])[0][0] + 1
 
     if break_scan is not None:
         idx_middle = np.where(eic_scan_idx == break_scan)[0][0]
 
+    max_int = np.max(eic_int)
+
     plt.figure(figsize=(9, 3))
     plt.rcParams['font.size'] = 14
     plt.rcParams['font.family'] = 'Arial'
     plt.plot(eic_rt, eic_int, linewidth=0.5, color="black")
+    plt.ylim(0, max_int*1.2)
 
     if break_scan is not None:
         plt.fill_between(eic_rt[idx_start:(idx_middle+1)], eic_int[idx_start:(idx_middle+1)], color="blue", alpha=0.2)
         plt.fill_between(eic_rt[idx_middle:idx_end], eic_int[idx_middle:idx_end], color="red", alpha=0.2)
     else:
         plt.fill_between(eic_rt[idx_start:idx_end], eic_int[idx_start:idx_end], color="black", alpha=0.2)
-    plt.axvline(x = roi.rt, color = 'b', linestyle = '--', linewidth=1)
+    plt.axvline(x = roi.rt, color = 'b', linestyle = '--', linewidth=1, ymax=0.8)
     # label the left and right of the ROI
-    plt.axvline(x = roi.rt_seq[0], color = 'grey', linestyle = '--', linewidth=0.5)
-    plt.axvline(x = roi.rt_seq[-1], color = 'grey', linestyle = '--', linewidth=0.5)
+    plt.axvline(x = roi.rt_seq[0], color = 'black', linestyle = '--', linewidth=0.5, ymax=0.8)
+    plt.axvline(x = roi.rt_seq[-1], color = 'black', linestyle = '--', linewidth=0.5, ymax=0.8)
     plt.xlabel("Retention Time (min)", fontsize=18, fontname='Arial')
     plt.ylabel("Intensity", fontsize=18, fontname='Arial')
     plt.xticks(fontsize=14, fontname='Arial')
     plt.yticks(fontsize=14, fontname='Arial')
-    plt.text(eic_rt[0], np.max(eic_int)*0.95, "m/z = {:.4f}".format(roi.mz), fontsize=12, fontname='Arial')
-    if label_quality:
-        plt.text(eic_rt[0] + (eic_rt[-1]-eic_rt[0])*0.2, np.max(eic_int)*0.95, "Quality = {}".format(roi.quality), fontsize=12, fontname='Arial', color="blue")
-    plt.text(eic_rt[0] + (eic_rt[-1]-eic_rt[0])*0.6, np.max(eic_int)*0.95, d.file_name, fontsize=10, fontname='Arial', color="gray")
+    plt.text(eic_rt[0], max_int*1.1, "m/z = {:.4f}".format(roi.mz), fontsize=11, fontname='Arial')
+    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.2, max_int*1.1, "G-score = {:.2f}".format(roi.gaussian_similarity), fontsize=11, fontname='Arial', color="blue")
+    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.4, max_int*1.1, "N-score = {:.2f}".format(roi.noise_level), fontsize=11, fontname='Arial', color="red")
+    plt.text(eic_rt[0]+(eic_rt[-1]-eic_rt[0])*0.6,max_int*1.1, d.file_name, fontsize=11, fontname='Arial', color="gray")
 
     if output:
         plt.savefig(output, dpi=600, bbox_inches="tight")
         plt.close()
     else:
         plt.show()
 
@@ -210,51 +213,56 @@
 
     sub_feature_table = feature_table[feature_table["search_mode"] == "identity_search"]
     ms2 = list(sub_feature_table["MS2"])
     matched_ms2 = list(sub_feature_table["matched_MS2"])
     score = list(sub_feature_table["similarity"])
     mz = list(sub_feature_table["m/z"])
     annotations = list(sub_feature_table["annotation"])
+    id = list(sub_feature_table["ID"])
 
     if output_dir is None and params is not None:
         output_dir = params.ms2_matching_dir
     elif output_dir is None and params is None:
         print("Please provide the output directory for MS2 matching plots.")
         return None
 
     for i in range(len(ms2)):
         peaks1 = _extract_peaks_from_string(ms2[i])
         peaks2 = _extract_peaks_from_string(matched_ms2[i])
 
-        output = os.path.join(output_dir, "{}.png".format(annotations[i]))
+        # replace all the special characters to "_"
+        a = re.sub(r"[^a-zA-Z0-9]", "_", annotations[i])
+        a = re.sub(r"[^a-zA-Z0-9]+", "_", a)
+        a = "ID" + "_" + str(id[i]) + "_" + a
+        output = os.path.join(output_dir, "{}.png".format(a))
         mirror_ms2(mz[i], mz[i], peaks1, peaks2, annotations[i], score[i], output)
 
 
 def plot_pca(vecPC1, vecPC2, var_PC1, var_PC2, group_names, output_dir=None):
     
     fig, ax = plt.subplots(figsize=(10,10))
     groups = np.unique(np.array(group_names))
     colors = COLORS[:len(groups)]
     for group, color in zip(groups, colors):
         idxs = np.where(np.array(group_names) == group)
         # No legend will be generated if we don't pass label=species
         confidence_ellipse(vecPC1[idxs], vecPC2[idxs], ax, edgecolor='black', facecolor=color, alpha=0.1, zorder=1, linewidth=1)
         ax.scatter(
             vecPC1[idxs], vecPC2[idxs], label=group,
-            s=300, color=color, alpha=0.8
+            s=300, color=color, alpha=0.3
         )
     for axis in ['top','bottom','left','right']:
         ax.spines[axis].set_linewidth(2)
     ax.tick_params(width=2, length=8) 
 
-    plt.xticks(np.arange(-40, 60, 20), fontname='Arial', fontsize=20)
-    plt.yticks(np.arange(-40, 60, 20), fontname='Arial', fontsize=20)
-    plt.grid(linestyle=':')
     plt.xlabel("PC 1 ({:.1f} %)".format(var_PC1*100), fontname='Arial', fontsize=30, labelpad=25)
     plt.ylabel("PC 2 ({:.1f} %)".format(var_PC2*100), fontname='Arial', fontsize=30, labelpad=25)
+    plt.xticks(fontname='Arial', fontsize=24)
+    plt.yticks(fontname='Arial', fontsize=24)
+    plt.grid(linestyle=':')
     plt.legend(fontsize=20, loc='upper right', frameon=False)
     plt.rcParams.update({'font.size': 24})
 
     if output_dir is not None:
         plt.savefig(output_dir, dpi=600, bbox_inches="tight")
         plt.close()
     else:
```

### Comparing `masscube-0.0.5/src/masscube/workflows.py` & `masscube-0.0.6/src/masscube/workflows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # Author: Hauxu Yu
 
 # A module to summarize the premade data processing workflows.
 
 # Import modules
 import os
-from keras.models import load_model
-import pandas as pd
 import multiprocessing
 import pickle
+from copy import deepcopy
 
 from .raw_data_utils import MSData
 from .params import Params, find_ms_info
-from .feature_evaluation import predict_quality, load_ann_model
 from .feature_grouping import annotate_isotope, annotate_adduct, annotate_in_source_fragment
 from .alignment import feature_alignment, gap_filling
 from .annotation import feature_annotation, annotate_rois
 from .normalization import sample_normalization
 from .visualization import plot_ms2_matching_from_feature_table
 from .network import network_analysis
 from .stats import statistical_analysis
 from .feature_table_utils import calculate_fill_percentage
 
 
 # Untargeted feature detection for a single file
-def feature_detection(file_name, params=None, ann_model=None, annotation=False, cut_roi=True):
+def feature_detection(file_name, params=None, cal_gss=True, annotation=False):
     """
     Untargeted feature detection from a single file (.mzML or .mzXML).
 
     Parameters
     ----------
     file_name : str
         Path to the raw file.
@@ -54,36 +52,26 @@
         params.set_default(ms_type, ion_mode)
 
     # read raw data
     d.read_raw_data(file_name, params)
 
     # drop ions by intensity (defined in params.int_tol)
     d.drop_ion_by_int()
-
     # detect region of interests (ROIs)
     d.find_rois()
 
     # cut ROIs
-    if cut_roi:
-        d.cut_rois()
-
-    # merge ROIs to group noise peaks
-    d.merge_rois()
+    d.cut_rois()
 
     # label short ROIs, find the best MS2, and sort ROIs by m/z
-    d.summarize_roi()
-
-    # predict feature quality
-    if ann_model is None:
-        ann_model = load_ann_model()
-    predict_quality(d, ann_model)
+    d.summarize_roi(cal_gss=cal_gss)
 
-    print("Number of extracted ROIs: " + str(len(d.rois)))
+    print("Number of detected features: " + str(len(d.rois)))
 
-    # annotate isotopes, adducts, and in-source fragments
+    # # annotate isotopes, adducts, and in-source fragments
     annotate_isotope(d)
     annotate_in_source_fragment(d)
     annotate_adduct(d)
 
     # annotate MS2 spectra
     if annotation and d.params.msms_library is not None:
         annotate_rois(d)
@@ -114,21 +102,26 @@
     with open(os.path.join(params.project_dir, "project.mc"), "wb") as f:
         pickle.dump(params, f)
     
     raw_file_names = os.listdir(params.sample_dir)
     raw_file_names = [f for f in raw_file_names if f.lower().endswith(".mzml") or f.lower().endswith(".mzxml")]
     raw_file_names = [os.path.join(params.sample_dir, f) for f in raw_file_names]
 
-    # process files by multiprocessing
+    # process files by multiprocessing, each batch contains 300 files
     print("Processing files by multiprocessing...")
     workers = int(multiprocessing.cpu_count() * 0.8)
-    p = multiprocessing.Pool(workers)
-    p.starmap(feature_detection, [(f, params) for f in raw_file_names]) 
-    p.close()
-    p.join()
+    for i in range(0, len(raw_file_names), 300):
+        if len(raw_file_names) - i < 300:
+            print("Processing files from " + str(i) + " to " + str(len(raw_file_names)))
+        else:
+            print("Processing files from " + str(i) + " to " + str(i+300))
+        p = multiprocessing.Pool(workers)
+        p.starmap(feature_detection, [(f, params) for f in raw_file_names[i:i+300]])
+        p.close()
+        p.join()
 
     # feature alignment
     print("Aligning features...")
     feature_table = feature_alignment(params.single_file_dir, params)
 
     # gap filling
     print("Filling gaps...")
@@ -143,20 +136,22 @@
         feature_annotation(feature_table, params)
     else:
         print("No MS2 library is found. Skipping annotation...")
 
     # normalization
     if params.run_normalization:
         feature_table.to_csv(os.path.join(params.project_dir, "aligned_feature_table_before_normalization.csv"), index=False)
+        feature_table_before_normalization = deepcopy(feature_table)
         print("Running normalization...")
         feature_table = sample_normalization(feature_table, params.individual_sample_groups, params.normalization_method)
 
     # statistical analysis
     if params.run_statistics:
         print("Running statistical analysis...")
+        feature_table_before_normalization = statistical_analysis(feature_table_before_normalization, params, before_norm=True)
         feature_table = statistical_analysis(feature_table, params)
 
     # network analysis
     if params.run_network:
         print("Running network analysis...This may take several minutes...")
         network_analysis(feature_table)
```

### Comparing `masscube-0.0.5/src/masscube.egg-info/PKG-INFO` & `masscube-0.0.6/src/masscube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.5
+Version: 0.0.6
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.0
 Requires-Dist: pyteomics>=4.6
 Requires-Dist: scipy>=1.10.1
-Requires-Dist: tensorflow>=2.12.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: matplotlib
 Requires-Dist: ms_entropy>=1.1.1
 Requires-Dist: networkx
 Requires-Dist: scikit-learn
```

### Comparing `masscube-0.0.5/src/masscube.egg-info/SOURCES.txt` & `masscube-0.0.6/src/masscube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

