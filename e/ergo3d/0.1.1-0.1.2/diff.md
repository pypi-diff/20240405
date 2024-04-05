# Comparing `tmp/ergo3d-0.1.1.tar.gz` & `tmp/ergo3d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergo3d-0.1.1.tar", last modified: Tue Apr  2 22:57:38 2024, max compression
+gzip compressed data, was "ergo3d-0.1.2.tar", last modified: Fri Apr  5 19:17:50 2024, max compression
```

## Comparing `ergo3d-0.1.1.tar` & `ergo3d-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.392226 ergo3d-0.1.1/
--rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      467 2024-04-02 22:57:38.392226 ergo3d-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      993 2024-04-02 22:57:36.000000 ergo3d-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.372224 ergo3d-0.1.1/ergo3d/
--rw-rw-rw-   0        0        0       44 2024-04-02 22:51:33.000000 ergo3d-0.1.1/ergo3d/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.382236 ergo3d-0.1.1/ergo3d/camera/
--rw-rw-rw-   0        0        0     4249 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/Camera.py
--rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/FLIR_camera.py
--rw-rw-rw-   0        0        0       24 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.392226 ergo3d-0.1.1/ergo3d/geometry/
--rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/CoordinateSystem3D.py
--rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/JointAngles.py
--rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/Plane.py
--rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/Point.py
--rw-rw-rw-   0        0        0      101 2024-04-02 22:50:46.000000 ergo3d-0.1.1/ergo3d/geometry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.372224 ergo3d-0.1.1/ergo3d.egg-info/
--rw-rw-rw-   0        0        0      467 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 22:57:38.392226 ergo3d-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-02 22:57:08.000000 ergo3d-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:50.855082 ergo3d-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-04-05 19:17:50.855082 ergo3d-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2024-04-02 23:02:10.000000 ergo3d-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:50.832081 ergo3d-0.1.2/ergo3d/
+-rw-rw-rw-   0        0        0       46 2024-04-04 19:41:29.000000 ergo3d-0.1.2/ergo3d/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:50.843081 ergo3d-0.1.2/ergo3d/camera/
+-rw-rw-rw-   0        0        0     4249 2024-04-02 22:55:21.000000 ergo3d-0.1.2/ergo3d/camera/Camera.py
+-rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.2/ergo3d/camera/FLIR_camera.py
+-rw-rw-rw-   0        0        0       51 2024-04-04 19:41:29.000000 ergo3d-0.1.2/ergo3d/camera/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:50.853081 ergo3d-0.1.2/ergo3d/geometry/
+-rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.2/ergo3d/geometry/CoordinateSystem3D.py
+-rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.2/ergo3d/geometry/JointAngles.py
+-rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.2/ergo3d/geometry/Plane.py
+-rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.2/ergo3d/geometry/Point.py
+-rw-rw-rw-   0        0        0      105 2024-04-04 19:41:29.000000 ergo3d-0.1.2/ergo3d/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:50.837082 ergo3d-0.1.2/ergo3d.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-04-05 19:17:50.000000 ergo3d-0.1.2/ergo3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-04-05 19:17:50.000000 ergo3d-0.1.2/ergo3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:17:50.000000 ergo3d-0.1.2/ergo3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 19:17:50.000000 ergo3d-0.1.2/ergo3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 19:17:50.000000 ergo3d-0.1.2/ergo3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:17:50.856082 ergo3d-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-05 19:17:48.000000 ergo3d-0.1.2/setup.py
```

### Comparing `ergo3d-0.1.1/LICENSE` & `ergo3d-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/camera/Camera.py` & `ergo3d-0.1.2/ergo3d/camera/Camera.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/camera/FLIR_camera.py` & `ergo3d-0.1.2/ergo3d/camera/FLIR_camera.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/geometry/CoordinateSystem3D.py` & `ergo3d-0.1.2/ergo3d/geometry/CoordinateSystem3D.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/geometry/JointAngles.py` & `ergo3d-0.1.2/ergo3d/geometry/JointAngles.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/geometry/Plane.py` & `ergo3d-0.1.2/ergo3d/geometry/Plane.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/ergo3d/geometry/Point.py` & `ergo3d-0.1.2/ergo3d/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.1/setup.py` & `ergo3d-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ergo3d',  # Name of your package
-    version='0.1.1',  # Version number
+    version='0.1.2',  # Version number
     description='A Python package for 3D ergonomic calculations.',  # Short description of your package
     url='https://github.com/LeyangWen/ergo3d',  # URL for your package's homepage
     author='Leyang Wen',  # Your name
     author_email='wenleyan@umich.edu',  # Your email
     license='MIT',  # License type for your package
     packages=find_packages(),  # Automatically find all packages and subpackages
     install_requires=[  # List of dependencies
```

