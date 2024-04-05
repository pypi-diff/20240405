# Comparing `tmp/fplab-0.0.1.2.tar.gz` & `tmp/fplab-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.1.2.tar", last modified: Sun Mar 31 13:50:26 2024, max compression
+gzip compressed data, was "fplab-0.0.1.3.tar", last modified: Fri Apr  5 04:03:04 2024, max compression
```

## Comparing `fplab-0.0.1.2.tar` & `fplab-0.0.1.3.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.976686 fplab-0.0.1.2/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-03-31 13:50:26.975597 fplab-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      807 2024-03-31 02:53:23.000000 fplab-0.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.944345 fplab-0.0.1.2/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.1.2/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.1.2/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.1.2/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.1.2/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.1.2/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.1.2/fplab/intrinsic/frequency/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/intrinsic/mask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.1.2/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     7036 2024-03-31 08:36:57.000000 fplab-0.0.1.2/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     7102 2024-03-31 08:46:45.000000 fplab-0.0.1.2/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     5106 2024-03-31 08:46:45.000000 fplab-0.0.1.2/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.1.2/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.1.2/fplab/matching/matching.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/minutiae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.959972 fplab-0.0.1.2/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.2/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13494 2024-03-25 14:10:10.000000 fplab-0.0.1.2/fplab/tools/array.py
--rw-rw-rw-   0        0        0     4651 2024-03-31 08:46:45.000000 fplab-0.0.1.2/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15079 2024-03-31 08:46:45.000000 fplab-0.0.1.2/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15550 2024-03-13 03:07:50.000000 fplab-0.0.1.2/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:50:26.944345 fplab-0.0.1.2/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-03-31 13:50:26.000000 fplab-0.0.1.2/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      809 2024-03-31 13:50:26.000000 fplab-0.0.1.2/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 13:50:26.000000 fplab-0.0.1.2/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 13:50:26.000000 fplab-0.0.1.2/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 13:50:26.976686 fplab-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-03-31 13:48:55.000000 fplab-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.311618 fplab-0.0.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-05 04:03:04.311618 fplab-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2024-03-31 02:53:23.000000 fplab-0.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.234901 fplab-0.0.1.3/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.1.3/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.1.3/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-02 15:55:02.000000 fplab-0.0.1.3/fplab/generation/distortion.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.1.3/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/mask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.1.3/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     7036 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     7102 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     5254 2024-04-01 02:18:24.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.1.3/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.1.3/fplab/matching/matching.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/minutiae/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.311618 fplab-0.0.1.3/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13494 2024-03-25 14:10:10.000000 fplab-0.0.1.3/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     4651 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15079 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15550 2024-03-13 03:07:50.000000 fplab-0.0.1.3/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.249055 fplab-0.0.1.3/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 04:03:04.311618 fplab-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-01 02:14:01.000000 fplab-0.0.1.3/setup.py
```

### Comparing `fplab-0.0.1.2/LICENSE.txt` & `fplab-0.0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/PKG-INFO` & `fplab-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.1.2/README.md` & `fplab-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/enhancement/frequency.py` & `fplab-0.0.1.3/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/enhancement/spatial.py` & `fplab-0.0.1.3/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.1.3/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.1.3/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.1.3/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.1.3/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.1.3/fplab/intrinsic/orientation/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 与指纹方向场有关的函数
 average_orientation_nd      计算方向场的局部角度平均值
-show_orientation            展示方向场
+display_orientation            展示方向场
 """
 import gc
 import torch
 import numpy as np
 import cv2
 from fplab.tools.image import type_as
 from fplab.tools.array import ima_pad_blk, ima_l2rgb, ima_pad_crop, ima_show, ima_save
@@ -103,7 +103,12 @@
     gc.collect()
     if "show" in flag:
         ima_show(out)
     if "save" in flag and save_path:
         ima_save(out, save_path)
     if "return" in flag:
         return type_as(out, im)
+
+
+def compare_orientation_nd(o1, o2, c):
+    """比较两个无向方向场的相似度"""
+    return ((np.cos(2*(o1-o2)))*c).sum()/c.sum()
```

### Comparing `fplab-0.0.1.2/fplab/matching/matching.py` & `fplab-0.0.1.3/fplab/matching/matching.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/tools/array.py` & `fplab-0.0.1.3/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/tools/image.py` & `fplab-0.0.1.3/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/tools/nbis.py` & `fplab-0.0.1.3/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab/tools/tensor.py` & `fplab-0.0.1.3/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.2/fplab.egg-info/PKG-INFO` & `fplab-0.0.1.3/fplab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.1.2/fplab.egg-info/SOURCES.txt` & `fplab-0.0.1.3/fplab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 fplab.egg-info/PKG-INFO
 fplab.egg-info/SOURCES.txt
 fplab.egg-info/dependency_links.txt
 fplab.egg-info/top_level.txt
 fplab/enhancement/__init__.py
 fplab/enhancement/frequency.py
 fplab/enhancement/spatial.py
+fplab/generation/__init__.py
+fplab/generation/distortion.py
 fplab/intrinsic/__init__.py
 fplab/intrinsic/frequency/__init__.py
 fplab/intrinsic/frequency/projection.py
 fplab/intrinsic/frequency/tools.py
 fplab/intrinsic/mask/__init__.py
 fplab/intrinsic/multiple/__init__.py
 fplab/intrinsic/multiple/transform.py
```

### Comparing `fplab-0.0.1.2/setup.py` & `fplab-0.0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1.2'
+VERSION = '0.0.1.3'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

