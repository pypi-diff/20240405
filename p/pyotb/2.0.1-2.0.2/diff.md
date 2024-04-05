# Comparing `tmp/pyotb-2.0.1.tar.gz` & `tmp/pyotb-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotb-2.0.1.tar", last modified: Mon Dec 18 08:41:14 2023, max compression
+gzip compressed data, was "pyotb-2.0.2.tar", last modified: Fri Apr  5 12:30:33 2024, max compression
```

## Comparing `pyotb-2.0.1.tar` & `pyotb-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 08:41:14.272702 pyotb-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-12-01 00:00:18.000000 pyotb-2.0.1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-12-01 00:00:18.000000 pyotb-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3319 2023-12-18 08:41:14.272702 pyotb-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-12-01 00:00:18.000000 pyotb-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 08:41:14.268702 pyotb-2.0.1/pyotb/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-12-18 08:23:19.000000 pyotb-2.0.1/pyotb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    71944 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/depreciation.py
--rw-rw-rw-   0 root         (0) root         (0)    21545 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/functions.py
--rw-rw-rw-   0 root         (0) root         (0)    13006 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7826 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyotb/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 08:41:14.272702 pyotb-2.0.1/pyotb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3319 2023-12-18 08:41:14.000000 pyotb-2.0.1/pyotb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2023-12-18 08:41:14.000000 pyotb-2.0.1/pyotb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-18 08:41:14.000000 pyotb-2.0.1/pyotb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-12-18 08:41:14.000000 pyotb-2.0.1/pyotb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-18 08:41:14.000000 pyotb-2.0.1/pyotb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-12-01 00:00:18.000000 pyotb-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-18 08:41:14.272702 pyotb-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 08:41:14.272702 pyotb-2.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    18354 2023-12-01 00:00:18.000000 pyotb-2.0.1/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     4705 2023-12-01 00:00:18.000000 pyotb-2.0.1/tests/test_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-12-01 00:00:18.000000 pyotb-2.0.1/tests/tests_data.py
+drwxr-xr-x   0 otbuser   (1000) otbuser   (1000)        0 2024-04-05 12:30:33.164884 pyotb-2.0.2/
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)      155 2024-04-05 12:00:33.000000 pyotb-2.0.2/AUTHORS.md
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)    11354 2024-04-05 12:00:33.000000 pyotb-2.0.2/LICENSE
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)     3315 2024-04-05 12:30:33.164884 pyotb-2.0.2/PKG-INFO
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     1872 2024-04-05 12:00:33.000000 pyotb-2.0.2/README.md
+drwxr-xr-x   0 otbuser   (1000) otbuser   (1000)        0 2024-04-05 12:30:33.160884 pyotb-2.0.2/pyotb/
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)      497 2024-04-05 12:25:19.000000 pyotb-2.0.2/pyotb/__init__.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     3142 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyotb/apps.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)    72188 2024-04-05 12:23:16.000000 pyotb-2.0.2/pyotb/core.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     2786 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyotb/depreciation.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)    21545 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyotb/functions.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)    13006 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyotb/helpers.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     7826 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyotb/install.py
+drwxr-xr-x   0 otbuser   (1000) otbuser   (1000)        0 2024-04-05 12:30:33.164884 pyotb-2.0.2/pyotb.egg-info/
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)     3315 2024-04-05 12:30:33.000000 pyotb-2.0.2/pyotb.egg-info/PKG-INFO
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)      370 2024-04-05 12:30:33.000000 pyotb-2.0.2/pyotb.egg-info/SOURCES.txt
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)        1 2024-04-05 12:30:33.000000 pyotb-2.0.2/pyotb.egg-info/dependency_links.txt
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)       80 2024-04-05 12:30:33.000000 pyotb-2.0.2/pyotb.egg-info/requires.txt
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)        6 2024-04-05 12:30:33.000000 pyotb-2.0.2/pyotb.egg-info/top_level.txt
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     1950 2024-04-05 12:00:34.000000 pyotb-2.0.2/pyproject.toml
+-rw-r--r--   0 otbuser   (1000) otbuser   (1000)       38 2024-04-05 12:30:33.164884 pyotb-2.0.2/setup.cfg
+drwxr-xr-x   0 otbuser   (1000) otbuser   (1000)        0 2024-04-05 12:30:33.164884 pyotb-2.0.2/tests/
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)    18354 2024-04-05 12:00:34.000000 pyotb-2.0.2/tests/test_core.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)     4705 2024-04-05 12:00:34.000000 pyotb-2.0.2/tests/test_pipeline.py
+-rw-rw-rw-   0 otbuser   (1000) otbuser   (1000)      769 2024-04-05 12:00:34.000000 pyotb-2.0.2/tests/tests_data.py
```

### Comparing `pyotb-2.0.1/LICENSE` & `pyotb-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/PKG-INFO` & `pyotb-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyotb
-Version: 2.0.1
+Version: 2.0.2
 Summary: Library to enable easy use of the Orfeo ToolBox (OTB) in Python
 Author: Nicolas Narçon, Vincent Delbar
 Author-email: Rémi Cresson <remi.cresson@inrae.fr>
 License: Apache-2.0
 Project-URL: documentation, https://pyotb.readthedocs.io
 Project-URL: homepage, https://github.com/orfeotoolbox/pyotb
-Project-URL: repository, https://gitlab.orfeo-toolbox.org/nicolasnn/pyotb
+Project-URL: repository, https://forgemia.inra.fr/orfeo-toolbox/pyotb
 Keywords: gis,remote sensing,otb,orfeotoolbox,orfeo toolbox
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyotb-2.0.1/README.md` & `pyotb-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb/apps.py` & `pyotb-2.0.2/pyotb/apps.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb/core.py` & `pyotb-2.0.2/pyotb/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,17 +661,16 @@
     def is_key_images_list(self, key: str) -> bool:
         """Check if a parameter key is an input parameter image list."""
         return self.app.GetParameterType(key) in self.INPUT_IMAGES_LIST_TYPES
 
     def get_first_key(self, param_types: list[int]) -> str:
         """Get the first param key for specific file types, try each list in args."""
         for param_type in param_types:
-            # Return the first key, from the alphabetically sorted keys of the
-            # application, which has the parameter type matching param_type.
-            for key, value in sorted(self._all_param_types.items()):
+            # Return the first key where type matches param_type.
+            for key, value in self._all_param_types.items():
                 if value == param_type:
                     return key
         raise TypeError(
             f"{self.name}: could not find any key matching the provided types"
         )
 
     @property
@@ -1015,17 +1014,23 @@
             self.app.ClearValue(key)
             return
         # Single-parameter cases
         if isinstance(obj, OTBObject):
             self.app.ConnectImage(key, obj.app, obj.output_image_key)
         elif isinstance(obj, otb.Application):
             self.app.ConnectImage(key, obj, get_out_images_param_keys(obj)[0])
+        # SetParameterValue in OTB<7.4 doesn't work for ram parameter (see OTB issue 2200)
         elif key == "ram":
-            # SetParameterValue in OTB<7.4 doesn't work for ram parameter cf OTB issue 2200
             self.app.SetParameterInt("ram", int(obj))
+        # SetParameterValue doesn't work with ParameterType_Field (see pyotb GitHub issue #1)
+        elif self.app.GetParameterType(key) == otb.ParameterType_Field:
+            if isinstance(obj, (list, tuple)):
+                self.app.SetParameterStringList(key, obj)
+            else:
+                self.app.SetParameterString(key, obj)
         # Any other parameters (str, int...)
         elif not isinstance(obj, (list, tuple)):
             self.app.SetParameterValue(key, obj)
         # Images list
         elif self.is_key_images_list(key):
             for inp in obj:
                 if isinstance(inp, OTBObject):
```

### Comparing `pyotb-2.0.1/pyotb/depreciation.py` & `pyotb-2.0.2/pyotb/depreciation.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb/functions.py` & `pyotb-2.0.2/pyotb/functions.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb/helpers.py` & `pyotb-2.0.2/pyotb/helpers.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb/install.py` & `pyotb-2.0.2/pyotb/install.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/pyotb.egg-info/PKG-INFO` & `pyotb-2.0.2/pyotb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyotb
-Version: 2.0.1
+Version: 2.0.2
 Summary: Library to enable easy use of the Orfeo ToolBox (OTB) in Python
 Author: Nicolas Narçon, Vincent Delbar
 Author-email: Rémi Cresson <remi.cresson@inrae.fr>
 License: Apache-2.0
 Project-URL: documentation, https://pyotb.readthedocs.io
 Project-URL: homepage, https://github.com/orfeotoolbox/pyotb
-Project-URL: repository, https://gitlab.orfeo-toolbox.org/nicolasnn/pyotb
+Project-URL: repository, https://forgemia.inra.fr/orfeo-toolbox/pyotb
 Keywords: gis,remote sensing,otb,orfeotoolbox,orfeo toolbox
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyotb-2.0.1/pyproject.toml` & `pyotb-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "tomli",
     "requests",
 ]
 
 [project.urls]
 documentation = "https://pyotb.readthedocs.io"
 homepage = "https://github.com/orfeotoolbox/pyotb"
-repository = "https://gitlab.orfeo-toolbox.org/nicolasnn/pyotb"
+repository = "https://forgemia.inra.fr/orfeo-toolbox/pyotb"
 
 [tool.setuptools]
 packages = ["pyotb"]
 
 [tool.setuptools.dynamic]
 version = { attr = "pyotb.__version__" }
```

### Comparing `pyotb-2.0.1/tests/test_core.py` & `pyotb-2.0.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/tests/test_pipeline.py` & `pyotb-2.0.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyotb-2.0.1/tests/tests_data.py` & `pyotb-2.0.2/tests/tests_data.py`

 * *Files identical despite different names*

