# Comparing `tmp/PyLLSM5DTools-1.0.1.tar.gz` & `tmp/PyLLSM5DTools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLLSM5DTools-1.0.1.tar", last modified: Wed Mar 27 22:56:37 2024, max compression
+gzip compressed data, was "PyLLSM5DTools-1.0.2.tar", last modified: Fri Apr  5 06:00:57 2024, max compression
```

## Comparing `PyLLSM5DTools-1.0.1.tar` & `PyLLSM5DTools-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-27 22:56:37.274530 PyLLSM5DTools-1.0.1/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 PyLLSM5DTools-1.0.1/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-03-27 22:56:37.274530 PyLLSM5DTools-1.0.1/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-27 22:56:37.274530 PyLLSM5DTools-1.0.1/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3796 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2794 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7971 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3114 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2782 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2060 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-03-27 20:44:20.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-03-27 21:32:27.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8629 2024-03-20 22:25:41.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-27 22:56:37.274530 PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-03-27 22:56:37.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-03-27 22:56:37.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-03-27 22:56:37.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-03-27 22:56:37.000000 PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 PyLLSM5DTools-1.0.1/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-03-27 22:56:37.274530 PyLLSM5DTools-1.0.1/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-03-27 20:38:05.000000 PyLLSM5DTools-1.0.1/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 PyLLSM5DTools-1.0.2/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2805 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2782 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-05 04:46:15.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-05 06:00:57.000000 PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 PyLLSM5DTools-1.0.2/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-05 06:00:57.205800 PyLLSM5DTools-1.0.2/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-05 04:47:16.000000 PyLLSM5DTools-1.0.2/setup.py
```

### Comparing `PyLLSM5DTools-1.0.1/LICENSE.txt` & `PyLLSM5DTools-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,22 @@
 
 def XR_FSC_analysis_wrapper(dataPaths, **kwargs):
     function_name = "XR_FSC_analysis_wrapper"
     XR_FSC_analysis_wrapper_dict = {
         "outDirstr": [kwargs.get("outDirstr", "FSCs"), "char"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "dz": [kwargs.get("dz", 0.1), "numericScalar"],
-        "angle": [kwargs.get("angle", 32.45), "numericScalar"],
         "dr": [kwargs.get("dr", 1), "numericScalar"],
         "dtheta": [kwargs.get("dtheta", math.pi/12), "numericScalar"],
         "resThreshMethod": [kwargs.get("resThreshMethod", "fixed"), "char"],
         "resThresh": [kwargs.get("resThresh", 0.2), "numericScalar"],
         "N": [kwargs.get("N", [251,251,251]), "numericArr"],
         "bbox": [kwargs.get("bbox", []), "numericScalar"],
         "resAxis": [kwargs.get("resAxis", "xz"), "char"],
         "skipConeRegion": [kwargs.get("skipConeRegion", True), "logical"],
-        "Deskew": [kwargs.get("Deskew", True), "logical"],
-        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "ZstageScan": [kwargs.get("ZstageScan", False), "logical"],
         "ChannelPatterns": [kwargs.get("ChannelPatterns", ['tif']), "cell"],
         "Channels": [kwargs.get("Channels", [488,560]), "numericArr"],
         "multiRegions": [kwargs.get("multiRegions", False), "logical"],
         "regionInterval": [kwargs.get("regionInterval", [50,50,-1]), "numericArr"],
         "regionGrid": [kwargs.get("regionGrid", []), "numericScalar"],
         "clipPer": [kwargs.get("clipPer", []), "numericScalar"],
         "suffix": [kwargs.get("suffix", "decon"), "char"],
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_MIP_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import subprocess
 
 
 def XR_MIP_wrapper(dataPaths, **kwargs):
     function_name = "XR_MIP_wrapper"
     XR_MIP_wrapper_dict = {
         "axis": [kwargs.get("axis", [0,0,1]), "numericArr"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
+        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
         "Save16bit": [kwargs.get("Save16bit", True), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "parseParfor": [kwargs.get("parseParfor", False), "logical"],
-        "jobLogDir": [kwargs.get("jobLogDir", "../job_logs/"), "char"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 3), "numericScalar"],
+        "jobLogDir": [kwargs.get("jobLogDir", "../job_logs/"), "char"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "debug": [kwargs.get("debug", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
         "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_crop_dataset.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_decon_data_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "Interp": [kwargs.get("Interp", "linear"), "char"],
         "maskFns": [kwargs.get("maskFns", []), "cell"],
         "suffix": [kwargs.get("suffix", ""), "char"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "parseParfor": [kwargs.get("parseParfor", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 8), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "debug": [kwargs.get("debug", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
         "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         "axisOrder": [kwargs.get("axisOrder", "x,y,z"), "char"],
         "dataOrder": [kwargs.get("dataOrder", "y,x,z"), "char"],
         "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
         "IOScan": [kwargs.get("IOScan", False), "logical"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
         "poolSize": [kwargs.get("poolSize", []), "numericScalar"],
-        "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
         "batchSize": [kwargs.get("batchSize", [500,500,500]), "numericArr"],
+        "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
         "shardSize": [kwargs.get("shardSize", []), "numericArr"],
         "zarrSubSize": [kwargs.get("zarrSubSize", []), "numericArr"],
         "resampleType": [kwargs.get("resampleType", "xy_isotropic"), "char"],
         "resample": [kwargs.get("resample", []), "numericArr"],
         "InputBbox": [kwargs.get("InputBbox", []), "numericArr"],
         "tileOutBbox": [kwargs.get("tileOutBbox", []), "numericArr"],
         "TileOffset": [kwargs.get("TileOffset", 0), "numericScalar"],
@@ -49,15 +49,15 @@
         "xcorrMode": [kwargs.get("xcorrMode", "primaryFirst"), "char"],
         "shiftMethod": [kwargs.get("shiftMethod", "grid"), "char"],
         "axisWeight": [kwargs.get("axisWeight", [1,0.1,10]), "numericArr"],
         "groupFile": [kwargs.get("groupFile", ""), "char"],
         "primaryCh": [kwargs.get("primaryCh", ""), "char"],
         "usePrimaryCoords": [kwargs.get("usePrimaryCoords", False), "logical"],
         "Save16bit": [kwargs.get("Save16bit", False), "logical"],
-        "EdgeArtifacts": [kwargs.get("EdgeArtifacts", 2), "numericScalar"],
+        "EdgeArtifacts": [kwargs.get("EdgeArtifacts", 0), "numericScalar"],
         "distBboxes": [kwargs.get("distBboxes", []), "numericArr"],
         "saveMIP": [kwargs.get("saveMIP", True), "logical"],
         "stitchMIP": [kwargs.get("stitchMIP", []), "logicalArr"],
         "onlineStitch": [kwargs.get("onlineStitch", False), "logical"],
         "bigStitchData": [kwargs.get("bigStitchData", False), "logical"],
         "pipeline": [kwargs.get("pipeline", "zarr"), "char"],
         "processFunPath": [kwargs.get("processFunPath", ), "cell"],
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 def XR_microscopeAutomaticProcessing(dataPaths, **kwargs):
     function_name = "XR_microscopeAutomaticProcessing"
     XR_microscopeAutomaticProcessing_dict = {
         "Overwrite": [kwargs.get("Overwrite", False), "logical"],
         "Streaming": [kwargs.get("Streaming", True), "logical"],
         "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
+        "Channels": [kwargs.get("Channels", [488,560,642]), "numericArr"],
         "SkewAngle": [kwargs.get("SkewAngle", 32.45), "numericScalar"],
         "dz": [kwargs.get("dz", 0.5), "numericScalar"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "Reverse": [kwargs.get("Reverse", True), "logical"],
         "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
         "ZstageScan": [kwargs.get("ZstageScan", False), "logical"],
         "sCMOSCameraFlip": [kwargs.get("sCMOSCameraFlip", False), "logical"],
@@ -74,15 +75,15 @@
         "fixIter": [kwargs.get("fixIter", False), "logical"],
         "errThresh": [kwargs.get("errThresh", []), "numericScalar"],
         "debug": [kwargs.get("debug", False), "logical"],
         "GPUJob": [kwargs.get("GPUJob", False), "logical"],
         "largeFile": [kwargs.get("largeFile", False), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
         "unitWaitTime": [kwargs.get("unitWaitTime", 1), "numericScalar"],
         "minModifyTime": [kwargs.get("minModifyTime", 1), "numericScalar"],
         "maxModifyTime": [kwargs.get("maxModifyTime", 10), "numericScalar"],
         "maxWaitLoopNum": [kwargs.get("maxWaitLoopNum", 10), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         "distThresh": [kwargs.get("distThresh", [256,128,201]), "numericArr"],
         "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
         "Channels": [kwargs.get("Channels", [488,560]), "numericArr"],
         "RWFn": [kwargs.get("RWFn", ['/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_515em_128_128_101_100nmSteps.tif','/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_605em_128_128_101_100nmSteps.tif']), "cell"],
         "sourceStr": [kwargs.get("sourceStr", "test"), "char"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", False), "logical"],
-        "prefix": [kwargs.get("prefix", "test_"), "char"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
         "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_resample_dataset.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     XR_visualize_OTF_mask_segmentation_dict = {
 
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     OTFCumThreshString = "[" + ",".join(str(item) for item in OTFCumThresh) + "]"
-    skewedString = "[" + ",".join(str(item) for item in skewed) + "]"
+    skewedString = "{" + ",".join(f"'{item}'" for item in skewed) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{psfFn}\" \"{OTFCumThreshString}\" \"{skewedString}\" "
     
     for key, value in XR_visualize_OTF_mask_segmentation_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/__init__.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/generatePythonWrapper.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,31 +20,34 @@
         raise ValueError(f"Invalid MATLAB function format for file: {matlab_file_path}")
 
     function_name = match.group(1)
 
     # Extract inputParser parameters
     input_parser_params_addRequired = re.findall(r"ip\.addRequired\((.*?)(?:\s*,(.*))?\);", matlab_function)
     input_parser_params_addParameter = re.findall(r"ip\.addParameter\((.*)\s*,(.*)\s*,(.*)\);", matlab_function)
+    input_parser_params_addOptional = re.findall(r"ip\.addOptional\((.*)\s*,(.*)\s*,(.*)\);", matlab_function)
+    num_optional = len(input_parser_params_addOptional)
 
     # Concatenate the capture groups and remove spaces
     input_parser_params = [",".join(param).replace(" ", "") for param in input_parser_params_addRequired]
     input_parser_params += [",".join(param).replace(" ", "") for param in input_parser_params_addParameter]
+    input_parser_params += [",".join(param).replace(" ", "") for param in input_parser_params_addOptional]
 
-    return function_name, input_parser_params
+    return function_name, input_parser_params, num_optional
 
 
 def generate_function(matlab_file_path):
-    function_name, input_parser_params = parse_matlab_file(matlab_file_path)
+    function_name, input_parser_params, num_optional = parse_matlab_file(matlab_file_path)
 
     if "_parser" in function_name:
         function_name = function_name.replace("_parser", "")
     functionString = "import os\nimport subprocess\n\n\ndef " + function_name + "("
 
     # Count the number of strings with only one comma
-    numRequired = sum(param.count(',') == 1 for param in input_parser_params)
+    numRequired = sum(param.count(',') == 1 for param in input_parser_params)+num_optional
     addRequired = True
     first_strings = [re.search(r"'([^']*)'", param).group(1) for param in input_parser_params]
     for i in range(numRequired):
         functionString = functionString + first_strings[i] + ", "
     functionString = functionString + f"**kwargs):\n    function_name = \"{function_name}\"\n    {function_name}_dict = {{\n        "
     varTypes = [""] * len(input_parser_params)
     # Have to hard code some variables that are ambiguous at the moment
```

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools/generate_config_file.py` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/PyLLSM5DTools.egg-info/SOURCES.txt` & `PyLLSM5DTools-1.0.2/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/README.md` & `PyLLSM5DTools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.1/setup.py` & `PyLLSM5DTools-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.0.1'
+version = '1.0.2'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

