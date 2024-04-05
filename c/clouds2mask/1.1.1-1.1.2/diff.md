# Comparing `tmp/clouds2mask-1.1.1.tar.gz` & `tmp/clouds2mask-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouds2mask-1.1.1.tar", last modified: Fri Dec 15 04:57:18 2023, max compression
+gzip compressed data, was "clouds2mask-1.1.2.tar", last modified: Fri Apr  5 00:31:55 2024, max compression
```

## Comparing `clouds2mask-1.1.1.tar` & `clouds2mask-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-12-15 04:57:18.248565 clouds2mask-1.1.1/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1066 2023-12-14 00:58:36.000000 clouds2mask-1.1.1/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)     3989 2023-12-15 04:57:18.244565 clouds2mask-1.1.1/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     3412 2023-12-14 04:15:36.000000 clouds2mask-1.1.1/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-12-15 04:57:18.244565 clouds2mask-1.1.1/clouds2mask/
--rw-rw-r--   0 nick      (1000) nick      (1000)      146 2023-12-15 04:52:53.000000 clouds2mask-1.1.1/clouds2mask/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6608 2023-12-15 04:50:11.000000 clouds2mask-1.1.1/clouds2mask/build_vrt.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7159 2023-12-15 04:50:09.000000 clouds2mask-1.1.1/clouds2mask/cloud_mask.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4780 2023-12-15 04:50:10.000000 clouds2mask-1.1.1/clouds2mask/cloud_mask_linear.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4051 2023-12-15 04:50:08.000000 clouds2mask-1.1.1/clouds2mask/download_model_weights.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     9020 2023-12-15 04:50:07.000000 clouds2mask-1.1.1/clouds2mask/inference.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5788 2023-12-15 04:50:06.000000 clouds2mask-1.1.1/clouds2mask/make_qml_files.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      306 2023-12-14 02:06:56.000000 clouds2mask-1.1.1/clouds2mask/model_download_links.csv
--rw-rw-r--   0 nick      (1000) nick      (1000)     4257 2023-12-15 04:50:05.000000 clouds2mask-1.1.1/clouds2mask/model_helpers.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5715 2023-12-15 04:50:04.000000 clouds2mask-1.1.1/clouds2mask/model_settings.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    10999 2023-12-15 04:50:03.000000 clouds2mask-1.1.1/clouds2mask/patch_generator.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6012 2023-12-15 04:50:02.000000 clouds2mask-1.1.1/clouds2mask/pred_joiner.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14346 2023-12-15 04:50:01.000000 clouds2mask-1.1.1/clouds2mask/processing_settings.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5448 2023-12-15 04:49:59.000000 clouds2mask-1.1.1/clouds2mask/tta_helpers.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-12-15 04:57:18.244565 clouds2mask-1.1.1/clouds2mask.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3989 2023-12-15 04:57:18.000000 clouds2mask-1.1.1/clouds2mask.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      617 2023-12-15 04:57:18.000000 clouds2mask-1.1.1/clouds2mask.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-12-15 04:57:18.000000 clouds2mask-1.1.1/clouds2mask.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       46 2023-12-15 04:57:18.000000 clouds2mask-1.1.1/clouds2mask.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       12 2023-12-15 04:57:18.000000 clouds2mask-1.1.1/clouds2mask.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-12-15 04:57:18.248565 clouds2mask-1.1.1/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)      916 2023-12-15 04:52:56.000000 clouds2mask-1.1.1/setup.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2024-04-05 00:31:55.822768 clouds2mask-1.1.2/
+-rw-r--r--   0 NickW      (503) staff       (20)     1066 2023-08-08 04:47:38.000000 clouds2mask-1.1.2/LICENSE
+-rw-r--r--   0 NickW      (503) staff       (20)     3989 2024-04-05 00:31:55.822399 clouds2mask-1.1.2/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)     3412 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/README.md
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2024-04-05 00:31:55.818250 clouds2mask-1.1.2/clouds2mask/
+-rw-r--r--   0 NickW      (503) staff       (20)      146 2024-04-05 00:29:00.000000 clouds2mask-1.1.2/clouds2mask/__init__.py
+-rw-r--r--   0 NickW      (503) staff       (20)     6608 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/build_vrt.py
+-rw-r--r--   0 NickW      (503) staff       (20)     7159 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/cloud_mask.py
+-rw-r--r--   0 NickW      (503) staff       (20)     4780 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/cloud_mask_linear.py
+-rw-r--r--   0 NickW      (503) staff       (20)     1865 2024-04-05 00:29:09.000000 clouds2mask-1.1.2/clouds2mask/download_model_weights.py
+-rw-r--r--   0 NickW      (503) staff       (20)     9020 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/inference.py
+-rw-r--r--   0 NickW      (503) staff       (20)     5788 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/make_qml_files.py
+-rw-r--r--   0 NickW      (503) staff       (20)      306 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/model_download_links.csv
+-rw-r--r--   0 NickW      (503) staff       (20)     4257 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/model_helpers.py
+-rw-r--r--   0 NickW      (503) staff       (20)     5715 2023-08-02 11:38:51.000000 clouds2mask-1.1.2/clouds2mask/model_settings.py
+-rw-r--r--   0 NickW      (503) staff       (20)    10999 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/patch_generator.py
+-rw-r--r--   0 NickW      (503) staff       (20)     6012 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/pred_joiner.py
+-rw-r--r--   0 NickW      (503) staff       (20)    14346 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/processing_settings.py
+-rw-r--r--   0 NickW      (503) staff       (20)     5448 2024-04-04 23:28:16.000000 clouds2mask-1.1.2/clouds2mask/tta_helpers.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2024-04-05 00:31:55.821560 clouds2mask-1.1.2/clouds2mask.egg-info/
+-rw-r--r--   0 NickW      (503) staff       (20)     3989 2024-04-05 00:31:55.000000 clouds2mask-1.1.2/clouds2mask.egg-info/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)      617 2024-04-05 00:31:55.000000 clouds2mask-1.1.2/clouds2mask.egg-info/SOURCES.txt
+-rw-r--r--   0 NickW      (503) staff       (20)        1 2024-04-05 00:31:55.000000 clouds2mask-1.1.2/clouds2mask.egg-info/dependency_links.txt
+-rw-r--r--   0 NickW      (503) staff       (20)       59 2024-04-05 00:31:55.000000 clouds2mask-1.1.2/clouds2mask.egg-info/requires.txt
+-rw-r--r--   0 NickW      (503) staff       (20)       12 2024-04-05 00:31:55.000000 clouds2mask-1.1.2/clouds2mask.egg-info/top_level.txt
+-rw-r--r--   0 NickW      (503) staff       (20)       38 2024-04-05 00:31:55.822893 clouds2mask-1.1.2/setup.cfg
+-rw-r--r--   0 NickW      (503) staff       (20)      979 2024-04-05 00:28:51.000000 clouds2mask-1.1.2/setup.py
```

### Comparing `clouds2mask-1.1.1/LICENSE` & `clouds2mask-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/PKG-INFO` & `clouds2mask-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clouds2mask
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for cloud and cloud shadow segmentation in Sentinel-2
 Home-page: https://github.com/DPIRD-DMA/CloudS2Mask
 Author: Nick Wright
 Author-email: nicholas.wright@dpird.wa.gov.au
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clouds2mask-1.1.1/README.md` & `clouds2mask-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/build_vrt.py` & `clouds2mask-1.1.2/clouds2mask/build_vrt.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/cloud_mask.py` & `clouds2mask-1.1.2/clouds2mask/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/cloud_mask_linear.py` & `clouds2mask-1.1.2/clouds2mask/cloud_mask_linear.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/inference.py` & `clouds2mask-1.1.2/clouds2mask/inference.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/make_qml_files.py` & `clouds2mask-1.1.2/clouds2mask/make_qml_files.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/model_helpers.py` & `clouds2mask-1.1.2/clouds2mask/model_helpers.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/model_settings.py` & `clouds2mask-1.1.2/clouds2mask/model_settings.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/patch_generator.py` & `clouds2mask-1.1.2/clouds2mask/patch_generator.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/pred_joiner.py` & `clouds2mask-1.1.2/clouds2mask/pred_joiner.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/processing_settings.py` & `clouds2mask-1.1.2/clouds2mask/processing_settings.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask/tta_helpers.py` & `clouds2mask-1.1.2/clouds2mask/tta_helpers.py`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/clouds2mask.egg-info/PKG-INFO` & `clouds2mask-1.1.2/clouds2mask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clouds2mask
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for cloud and cloud shadow segmentation in Sentinel-2
 Home-page: https://github.com/DPIRD-DMA/CloudS2Mask
 Author: Nick Wright
 Author-email: nicholas.wright@dpird.wa.gov.au
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clouds2mask-1.1.1/clouds2mask.egg-info/SOURCES.txt` & `clouds2mask-1.1.2/clouds2mask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clouds2mask-1.1.1/setup.py` & `clouds2mask-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import find_packages, setup
 
 setup(
     name="clouds2mask",
-    version="1.1.1",
+    version="1.1.2",
     description="""Python library for cloud and cloud shadow segmentation in Sentinel-2
     L1C imagery""",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Nick Wright",
     author_email="nicholas.wright@dpird.wa.gov.au",
     url="https://github.com/DPIRD-DMA/CloudS2Mask",
     python_requires=">=3.7",
     packages=find_packages(),
-    install_requires=["fastai>=2.7", "timm>=0.9", "tqdm>=4.0", "rasterio>=1.3"],
+    install_requires=[
+        "fastai>=2.7",
+        "timm>=0.9",
+        "tqdm>=4.0",
+        "rasterio>=1.3",
+        "gdown>=5.1.0",
+    ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
```

