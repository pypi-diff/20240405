# Comparing `tmp/napari-3dtimereg-0.0.2.tar.gz` & `tmp/napari-3dtimereg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-3dtimereg-0.0.2.tar", last modified: Fri Apr  5 13:21:23 2024, max compression
+gzip compressed data, was "napari-3dtimereg-0.0.3.tar", last modified: Fri Apr  5 13:26:39 2024, max compression
```

## Comparing `napari-3dtimereg-0.0.2.tar` & `napari-3dtimereg-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:21:23.264616 napari-3dtimereg-0.0.2/
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1523 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/LICENSE
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       96 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/MANIFEST.in
--rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5710 2024-04-05 13:21:23.264616 napari-3dtimereg-0.0.2/PKG-INFO
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     4316 2024-04-05 13:02:23.000000 napari-3dtimereg-0.0.2/README.md
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1175 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/pyproject.toml
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1470 2024-04-05 13:21:23.264616 napari-3dtimereg-0.0.2/setup.cfg
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       37 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:21:23.260616 napari-3dtimereg-0.0.2/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:21:23.260616 napari-3dtimereg-0.0.2/src/napari_3dtimereg/
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     8152 2024-04-04 15:55:42.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg/Utils.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg/__init__.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)    19832 2024-04-05 12:21:26.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg/movieRegistration.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      350 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:21:23.264616 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/
--rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5710 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/PKG-INFO
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      467 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/SOURCES.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/dependency_links.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       66 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/entry_points.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      107 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/requires.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       17 2024-04-05 13:21:23.000000 napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:26:39.372375 napari-3dtimereg-0.0.3/
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1523 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/LICENSE
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       96 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/MANIFEST.in
+-rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5726 2024-04-05 13:26:39.372375 napari-3dtimereg-0.0.3/PKG-INFO
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     4332 2024-04-05 13:25:59.000000 napari-3dtimereg-0.0.3/README.md
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1175 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/pyproject.toml
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1470 2024-04-05 13:26:39.372375 napari-3dtimereg-0.0.3/setup.cfg
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       37 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:26:39.368375 napari-3dtimereg-0.0.3/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:26:39.368375 napari-3dtimereg-0.0.3/src/napari_3dtimereg/
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     8152 2024-04-04 15:55:42.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg/Utils.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg/__init__.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)    19832 2024-04-05 12:21:26.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg/movieRegistration.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      350 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:26:39.372375 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/
+-rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5726 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/PKG-INFO
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      467 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       66 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/entry_points.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      107 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/requires.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       17 2024-04-05 13:26:39.000000 napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/top_level.txt
```

### Comparing `napari-3dtimereg-0.0.2/LICENSE` & `napari-3dtimereg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.2/PKG-INFO` & `napari-3dtimereg-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3dtimereg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Registration of 3D movies applied to all channels
 Home-page: https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/napari-3dtimereg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/napari-3dtimereg#README.md
@@ -34,16 +34,16 @@
 Requires-Dist: itk-registration
 Requires-Dist: itk-elastix
 
 # napari-3dtimereg
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-3dtimereg.svg?color=green)](https://gitlab.pasteur.fr/gletort/napari-3dtimereg/-/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
-[![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/napari-3dtimereg)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
 
 ----------------------------------
 ## Installation
```

### Comparing `napari-3dtimereg-0.0.2/README.md` & `napari-3dtimereg-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # napari-3dtimereg
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-3dtimereg.svg?color=green)](https://gitlab.pasteur.fr/gletort/napari-3dtimereg/-/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
-[![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/napari-3dtimereg)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
 
 ----------------------------------
 ## Installation
```

### Comparing `napari-3dtimereg-0.0.2/pyproject.toml` & `napari-3dtimereg-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.2/setup.cfg` & `napari-3dtimereg-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-3dtimereg
-version = 0.0.2
+version = 0.0.3
 description = Registration of 3D movies applied to all channels
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 license = BSD-3-Clause
```

### Comparing `napari-3dtimereg-0.0.2/src/napari_3dtimereg/Utils.py` & `napari-3dtimereg-0.0.3/src/napari_3dtimereg/Utils.py`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.2/src/napari_3dtimereg/movieRegistration.py` & `napari-3dtimereg-0.0.3/src/napari_3dtimereg/movieRegistration.py`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.2/src/napari_3dtimereg.egg-info/PKG-INFO` & `napari-3dtimereg-0.0.3/src/napari_3dtimereg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3dtimereg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Registration of 3D movies applied to all channels
 Home-page: https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/napari-3dtimereg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/napari-3dtimereg#README.md
@@ -34,16 +34,16 @@
 Requires-Dist: itk-registration
 Requires-Dist: itk-elastix
 
 # napari-3dtimereg
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-3dtimereg.svg?color=green)](https://gitlab.pasteur.fr/gletort/napari-3dtimereg/-/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
-[![Python Version](https://img.shields.io/pypi/pyversions/multireg.svg?color=green)](https://python.org)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/multireg)](https://napari-hub.org/plugins/napari-3dtimereg)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
 
 ----------------------------------
 ## Installation
```

