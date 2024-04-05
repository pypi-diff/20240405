# Comparing `tmp/TFCat-1.0.0rc2.tar.gz` & `tmp/TFCat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/baptiste/Projets/VOParis/MASER/Catalogues/git/tfcat/dist/tmpywmaqhed/TFCat-1.0.0rc2.tar", last modified: Sun Sep 18 10:13:25 2022, max compression
+gzip compressed data, was "TFCat-1.0.1.tar", last modified: Fri Apr  5 16:55:56 2024, max compression
```

## Comparing `TFCat-1.0.0rc2.tar` & `TFCat-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/
--rw-r--r--   0 baptiste   (501) admin       (80)     1075 2021-02-24 13:04:29.000000 TFCat-1.0.0rc2/LICENSE
--rw-r--r--   0 baptiste   (501) admin       (80)     2369 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/PKG-INFO
--rw-r--r--   0 baptiste   (501) admin       (80)      458 2022-09-14 17:02:46.000000 TFCat-1.0.0rc2/README.md
-drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/
--rw-r--r--   0 baptiste   (501) admin       (80)     2369 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/PKG-INFO
--rw-r--r--   0 baptiste   (501) admin       (80)      390 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/SOURCES.txt
--rw-r--r--   0 baptiste   (501) admin       (80)        1 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/dependency_links.txt
--rw-r--r--   0 baptiste   (501) admin       (80)       38 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/requires.txt
--rw-r--r--   0 baptiste   (501) admin       (80)        6 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/TFCat.egg-info/top_level.txt
--rw-r--r--   0 baptiste   (501) admin       (80)     1164 2022-09-18 10:12:37.000000 TFCat-1.0.0rc2/pyproject.toml
--rw-r--r--   0 baptiste   (501) admin       (80)       38 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/setup.cfg
-drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2022-09-18 10:13:25.000000 TFCat-1.0.0rc2/tfcat/
--rw-r--r--   0 baptiste   (501) admin       (80)      964 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/__init__.py
--rw-r--r--   0 baptiste   (501) admin       (80)       81 2022-09-14 17:02:46.000000 TFCat-1.0.0rc2/tfcat/_version.py
--rw-r--r--   0 baptiste   (501) admin       (80)     4372 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/base.py
--rw-r--r--   0 baptiste   (501) admin       (80)     1469 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/codec.py
--rw-r--r--   0 baptiste   (501) admin       (80)    12110 2022-09-18 10:05:29.000000 TFCat-1.0.0rc2/tfcat/crs.py
--rw-r--r--   0 baptiste   (501) admin       (80)      543 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/factory.py
--rw-r--r--   0 baptiste   (501) admin       (80)     6958 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/feature.py
--rw-r--r--   0 baptiste   (501) admin       (80)      316 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/field.py
--rw-r--r--   0 baptiste   (501) admin       (80)     4776 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/geometry.py
--rw-r--r--   0 baptiste   (501) admin       (80)     1847 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/observation.py
--rw-r--r--   0 baptiste   (501) admin       (80)    10045 2022-09-15 12:59:22.000000 TFCat-1.0.0rc2/tfcat/tfcat.py
--rw-r--r--   0 baptiste   (501) admin       (80)     8551 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/utils.py
--rw-r--r--   0 baptiste   (501) admin       (80)     1021 2022-09-14 16:55:52.000000 TFCat-1.0.0rc2/tfcat/validate.py
+drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2024-04-05 16:55:56.201362 TFCat-1.0.1/
+-rw-r--r--   0 baptiste   (501) admin       (80)     1141 2023-02-24 15:53:00.000000 TFCat-1.0.1/LICENSE
+-rw-r--r--   0 baptiste   (501) admin       (80)     2684 2024-04-05 16:55:56.201158 TFCat-1.0.1/PKG-INFO
+-rw-r--r--   0 baptiste   (501) admin       (80)      562 2023-02-24 16:09:28.000000 TFCat-1.0.1/README.md
+drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2024-04-05 16:55:56.200931 TFCat-1.0.1/TFCat.egg-info/
+-rw-r--r--   0 baptiste   (501) admin       (80)     2684 2024-04-05 16:55:56.000000 TFCat-1.0.1/TFCat.egg-info/PKG-INFO
+-rw-r--r--   0 baptiste   (501) admin       (80)      540 2024-04-05 16:55:56.000000 TFCat-1.0.1/TFCat.egg-info/SOURCES.txt
+-rw-r--r--   0 baptiste   (501) admin       (80)        1 2024-04-05 16:55:56.000000 TFCat-1.0.1/TFCat.egg-info/dependency_links.txt
+-rw-r--r--   0 baptiste   (501) admin       (80)       40 2024-04-05 16:55:56.000000 TFCat-1.0.1/TFCat.egg-info/requires.txt
+-rw-r--r--   0 baptiste   (501) admin       (80)        6 2024-04-05 16:55:56.000000 TFCat-1.0.1/TFCat.egg-info/top_level.txt
+-rw-r--r--   0 baptiste   (501) admin       (80)     1230 2023-02-24 16:10:19.000000 TFCat-1.0.1/pyproject.toml
+-rw-r--r--   0 baptiste   (501) admin       (80)       38 2024-04-05 16:55:56.201408 TFCat-1.0.1/setup.cfg
+drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2024-04-05 16:55:56.197135 TFCat-1.0.1/tests/
+-rw-r--r--   0 baptiste   (501) admin       (80)     2010 2021-07-11 15:47:45.000000 TFCat-1.0.1/tests/test_base.py
+-rw-r--r--   0 baptiste   (501) admin       (80)      890 2021-07-11 15:47:45.000000 TFCat-1.0.1/tests/test_codec.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     8685 2024-04-05 16:55:40.000000 TFCat-1.0.1/tests/test_crs.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     4026 2024-04-05 16:49:14.000000 TFCat-1.0.1/tests/test_feature.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     5103 2021-10-27 15:29:40.000000 TFCat-1.0.1/tests/test_geometry.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     4261 2022-09-15 07:29:24.000000 TFCat-1.0.1/tests/test_tfcat.py
+-rw-r--r--   0 baptiste   (501) admin       (80)      181 2021-07-11 15:47:45.000000 TFCat-1.0.1/tests/test_utils.py
+-rw-r--r--   0 baptiste   (501) admin       (80)      105 2022-05-17 15:44:07.000000 TFCat-1.0.1/tests/test_validate.py
+drwxr-xr-x   0 baptiste   (501) admin       (80)        0 2024-04-05 16:55:56.200593 TFCat-1.0.1/tfcat/
+-rw-r--r--   0 baptiste   (501) admin       (80)      964 2024-04-05 16:49:14.000000 TFCat-1.0.1/tfcat/__init__.py
+-rw-r--r--   0 baptiste   (501) admin       (80)       81 2023-02-24 16:09:28.000000 TFCat-1.0.1/tfcat/_version.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     4384 2023-02-24 15:53:00.000000 TFCat-1.0.1/tfcat/base.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     1695 2023-02-24 15:53:00.000000 TFCat-1.0.1/tfcat/codec.py
+-rw-r--r--   0 baptiste   (501) admin       (80)    12144 2022-09-18 12:27:32.000000 TFCat-1.0.1/tfcat/crs.py
+-rw-r--r--   0 baptiste   (501) admin       (80)      543 2022-09-14 16:55:52.000000 TFCat-1.0.1/tfcat/factory.py
+-rw-r--r--   0 baptiste   (501) admin       (80)    11361 2024-04-05 16:49:14.000000 TFCat-1.0.1/tfcat/feature.py
+-rw-r--r--   0 baptiste   (501) admin       (80)      714 2022-09-20 12:50:17.000000 TFCat-1.0.1/tfcat/field.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     4776 2022-09-14 16:55:52.000000 TFCat-1.0.1/tfcat/geometry.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     1847 2024-04-05 16:49:14.000000 TFCat-1.0.1/tfcat/observation.py
+-rw-r--r--   0 baptiste   (501) admin       (80)    10086 2024-04-05 16:55:40.000000 TFCat-1.0.1/tfcat/tfcat.py
+-rw-r--r--   0 baptiste   (501) admin       (80)     1021 2022-09-14 16:55:52.000000 TFCat-1.0.1/tfcat/validate.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TFCat-1.0.0rc2/LICENSE` & `TFCat-1.0.1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2021 MASER / Catalogues
+Copyright (c) 2021-2022, contributors from the MASER Team (B. Cecconi,
+X. Bonnin, A. Loh, M. B. Taylor)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `TFCat-1.0.0rc2/PKG-INFO` & `TFCat-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: TFCat
-Version: 1.0.0rc2
+Version: 1.0.1
 Summary: Time-Frequency Catalogue (TFCat) Python module.
-Author-email: Baptiste Cecconi <baptiste.cecconi@obspm.fr>, Xavier Bonnin <xavier.bonnin@obspm.fr>, Alan Loh <alan.loh@obspm.fr>
+Author-email: Baptiste Cecconi <baptiste.cecconi@obspm.fr>, Xavier Bonnin <xavier.bonnin@obspm.fr>, Alan Loh <alan.loh@obspm.fr>, Adam Boudouma <adam.boudouma@obspm.fr>
 License: MIT License
         
-        Copyright (c) 2021 MASER / Catalogues
+        Copyright (c) 2021-2022, contributors from the MASER Team (B. Cecconi,
+        X. Bonnin, A. Loh, M. B. Taylor)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -30,22 +31,35 @@
 Keywords: radio astronomy,catalogue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: astropy
+Requires-Dist: matplotlib
+Requires-Dist: shapely<2
+Requires-Dist: jsonschema
 
 #  Time-Frequency Catalogue (TFCat) Python Module
 
 This module implements an interface for loading TFCat JSON 
 data files. 
 
 TFCat JSON Specification: [TFcat](https://gitlab.obspm.fr/maser/catalogues/catalogue-format)
 
 TFCat JSON Schema: https://voparis-ns.obspm.fr/maser/tfcat/v1.0/schema#
 
-*This version 1.0.0-rc1*
+*This version 1.0.0*
+
+## Installation
+
+TFCat is available from PyPI: https://pypi.org/project/TFCat/
+
+```
+pip install TFCat
+```
+
 
 ## Acknowlegments
 - This TFCat library has been derived from the 
   [jazzband/geojson](https://github.com/jazzband/geojson) python library.
```

### Comparing `TFCat-1.0.0rc2/TFCat.egg-info/PKG-INFO` & `TFCat-1.0.1/TFCat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: TFCat
-Version: 1.0.0rc2
+Version: 1.0.1
 Summary: Time-Frequency Catalogue (TFCat) Python module.
-Author-email: Baptiste Cecconi <baptiste.cecconi@obspm.fr>, Xavier Bonnin <xavier.bonnin@obspm.fr>, Alan Loh <alan.loh@obspm.fr>
+Author-email: Baptiste Cecconi <baptiste.cecconi@obspm.fr>, Xavier Bonnin <xavier.bonnin@obspm.fr>, Alan Loh <alan.loh@obspm.fr>, Adam Boudouma <adam.boudouma@obspm.fr>
 License: MIT License
         
-        Copyright (c) 2021 MASER / Catalogues
+        Copyright (c) 2021-2022, contributors from the MASER Team (B. Cecconi,
+        X. Bonnin, A. Loh, M. B. Taylor)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -30,22 +31,35 @@
 Keywords: radio astronomy,catalogue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: astropy
+Requires-Dist: matplotlib
+Requires-Dist: shapely<2
+Requires-Dist: jsonschema
 
 #  Time-Frequency Catalogue (TFCat) Python Module
 
 This module implements an interface for loading TFCat JSON 
 data files. 
 
 TFCat JSON Specification: [TFcat](https://gitlab.obspm.fr/maser/catalogues/catalogue-format)
 
 TFCat JSON Schema: https://voparis-ns.obspm.fr/maser/tfcat/v1.0/schema#
 
-*This version 1.0.0-rc1*
+*This version 1.0.0*
+
+## Installation
+
+TFCat is available from PyPI: https://pypi.org/project/TFCat/
+
+```
+pip install TFCat
+```
+
 
 ## Acknowlegments
 - This TFCat library has been derived from the 
   [jazzband/geojson](https://github.com/jazzband/geojson) python library.
```

### Comparing `TFCat-1.0.0rc2/pyproject.toml` & `TFCat-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TFCat"
-version = "1.0.0-rc2"
+version = "1.0.1"
 authors = [
     { name = "Baptiste Cecconi", email = "baptiste.cecconi@obspm.fr" },
     { name = "Xavier Bonnin", email = "xavier.bonnin@obspm.fr" },
-    { name = "Alan Loh", email = "alan.loh@obspm.fr" }
+    { name = "Alan Loh", email = "alan.loh@obspm.fr" },
+    { name = "Adam Boudouma", email = "adam.boudouma@obspm.fr" }
 ]
 description = "Time-Frequency Catalogue (TFCat) Python module."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 keywords = ["radio astronomy", "catalogue"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "astropy",
     "matplotlib",
-    "shapely",
+    "shapely < 2",
     "jsonschema"
 ]
 
 [tool.setuptools.packages.find]
 "include" = ["tfcat"]
 "exclude" = ["tests", "htmlcov", "examples"]
```

### Comparing `TFCat-1.0.0rc2/tfcat/__init__.py` & `TFCat-1.0.1/tfcat/__init__.py`

 * *Files identical despite different names*

### Comparing `TFCat-1.0.0rc2/tfcat/base.py` & `TFCat-1.0.1/tfcat/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import tfcat.codec
 import tfcat.factory
 
 
 class Base(dict):
     """
     A class representing a TFCat base object.
     """
@@ -17,15 +17,15 @@
         :rtype: Base
         """
         super(Base, self).__init__(iterable)
         self["type"] = getattr(self, "type", type(self).__name__)
         self.update(extra)
 
     def __repr__(self):
-        return json.dumps(self, sort_keys=True)
+        return tfcat.codec.dumps(self, sort_keys=True)
 
     __str__ = __repr__
 
     def __getattr__(self, name):
         """
         Permit dictionary items to be retrieved like object attributes
 
@@ -57,15 +57,15 @@
         :type name: str
         """
 
         del self[name]
 
     @classmethod
     def to_instance(cls, ob, default=None, strict=False):
-        """Encode a Base dict into an Base object.
+        """Encode a Base dict into a Base object.
         Assumes the caller knows that the dict should satisfy a TFCat type.
 
         :param cls: Dict containing the elements to be encoded into a TFCat
         object.
         :type cls: dict
         :param ob: TFCat object into which to encode the dict provided in
         `cls`.
@@ -123,12 +123,12 @@
         return [err for err in results if err]
 
     def errors(self):
         """Return validation errors (if any).
         Implement in each subclass.
         """
 
-        # make sure that each subclass implements it's own validation function
+        # make sure that each subclass implements its own validation function
         if self.__class__ != Base:
             raise NotImplementedError(self.__class__)
```

### Comparing `TFCat-1.0.0rc2/tfcat/codec.py` & `TFCat-1.0.1/tfcat/codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import json
 import tfcat.factory
 import tfcat.base
+import numpy
 
 """
 This file is adapted from: https://github.com/jazzband/geojson/blob/master/geojson/codec.py
 """
 
 
 class TFCatEncoder(json.JSONEncoder):
 
     def default(self, obj):
-        return tfcat.factory.Base.to_instance(obj) # NOQA
-
+        if isinstance(obj, numpy.signedinteger) or isinstance(obj, numpy.unsignedinteger):
+            return int(obj)
+        elif isinstance(obj, numpy.floating):
+            return float(obj)
+        else:
+            return tfcat.factory.Base.to_instance(obj) # NOQA
 
 # Wrap the functions from json, providing encoder, decoders, and
 # object creation hooks.
 # Here the defaults are set to only permit valid JSON as per RFC 4267
 
+
 def _enforce_strict_numbers(obj):
     raise ValueError("Number %r is not JSON compliant" % obj)
 
 
 def dump(obj, fp, cls=TFCatEncoder, allow_nan=False, **kwargs):
     return json.dump(obj, fp, cls=cls, allow_nan=allow_nan, **kwargs)
```

### Comparing `TFCat-1.0.0rc2/tfcat/crs.py` & `TFCat-1.0.1/tfcat/crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,12 +293,13 @@
 REF_POSITION = [
     'GEOCENTER',
 ]
 
 DefaultCRS = CRS({
     "type": "local",
     "properties": {
+        "name": "Time-Frequency",
         "time_coords_id": 'unix',
         "spectral_coords": SPECTRAL_COORDS['Hz'],
         "ref_position_id": 'GEOCENTER',
     }
 })
```

### Comparing `TFCat-1.0.0rc2/tfcat/factory.py` & `TFCat-1.0.1/tfcat/factory.py`

 * *Files identical despite different names*

### Comparing `TFCat-1.0.0rc2/tfcat/geometry.py` & `TFCat-1.0.1/tfcat/geometry.py`

 * *Files identical despite different names*

### Comparing `TFCat-1.0.0rc2/tfcat/observation.py` & `TFCat-1.0.1/tfcat/observation.py`

 * *Files identical despite different names*

### Comparing `TFCat-1.0.0rc2/tfcat/tfcat.py` & `TFCat-1.0.1/tfcat/tfcat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tfcat.codec import load, loads
 from tfcat.geometry import Polygon, MultiPolygon, Point, MultiPoint, LineString, MultiLineString
 from tfcat.feature import Feature, FeatureCollection
 from tfcat.observation import Observation
+from tfcat.validate import validate
 from tfcat.crs import CRS
 from tfcat.field import Field
 import tfcat.utils
 from matplotlib import pyplot as plt
 from urllib.request import urlopen
 from pathlib import Path
 from typing import Union
@@ -15,52 +16,51 @@
     """Main TFCat object.
 
     This object has several constructor methods:
 
     * :func:`from_file()` to load a TFCat feature collection from a local file.
     * :func:`from_url()` to load a TFCat feature collection from a eremote URL.
     * :func:`__init__()` to directly load a TFCat feature collection object.
-
-    :param tfcat_data: TFCat feature collection object
-    :type tfcat_data: FeatureCollection
-    :param file_uri: TFCat file or URL
-    :type file_uri: Union[Path, str, None]
-    :return: A TFcat object
-    :rtype: TFCat
     """
 
-    def __init__(self, tfcat_data, file_uri=None):
+    def __init__(
+            self,
+            tfcat_data: FeatureCollection,
+            file_uri: Union[Path, str, None] = None,
+    ):
+        """
+        :param tfcat_data: TFCat feature collection object
+        :param file_uri: TFCat file or URL
+        """
+
         self.file = file_uri
         self.data = tfcat_data
 
     @property
-    def data(self):
+    def data(self) -> FeatureCollection:
         """Returns the internal TFCat data object.
 
         :return: A TFCat FeatureCollection object
         :rtype: FeatureCollection
         """
 
         return self._data
 
     @data.setter
-    def data(self, tfcat_data):
+    def data(self, tfcat_data: FeatureCollection):
         self._data = tfcat_data
 
     @property
-    def has_observations(self):
+    def has_observations(self) -> bool:
         """Informs if the TFCat object has an observation list
-
-        :return:
-        :rtype: bool
         """
         return 'observations' in self._data.keys()
 
     @property
-    def _lookup(self):
+    def _lookup(self) -> list:
         return list(item.properties['obs_id'] for item in self._data.features)
 
     @classmethod
     def from_file(cls, file_name: Union[Path, str]):
         """Loads the TFCat feature collection from a local file
 
         :param file_name: local file path
@@ -108,35 +108,31 @@
     @property
     def fields(self) -> list:
         """Returns the list of Fields objects.
 
         Fields objects are describing the feature property keywords.
 
         :return: A list of feature property descriptors
-        :rtype: list[Field]
         """
         return self._data.fields
 
     def __len__(self) -> int:
         """Returns the length of the feature collection.
 
         The length is the number of features in the TFCat object.
 
         :returns: number of features
-        :rtype: int
         """
         return len(self._data.features)
 
-    def observation(self, n) -> Observation:
+    def observation(self, n: int) -> Observation:
         """Returns the nth observation of the TFCat feature collection object.
 
         :param n: index
-        :type n: int
         :return: nth observation
-        :rtype: Observation
         """
         return self._data.observations[n]
 
     def feature(self, n) -> Feature:
         """Returns the nth feature of the TFCat feature collection object.
 
         :param n: index
@@ -144,45 +140,50 @@
         :return: nth feature
         :rtype: Feature
         """
         return self._data.features[n]
 
     @property
     def iter_features(self) -> Feature:
-        """
-        Generator on features
+        """Generator on features.
+
         :return: feature
         """
         n = 0
         while n < len(self):
             yield self.feature(n) #, self.observation(self._lookup[n]) if self.has_observations else None
             n += 1
 
     @property
     def iter_observations(self) -> Observation:
-        """
-        Generator observations
+        """Generator on observations.
+
         :returns: observation
         """
         n = 0
         while n < len(self._data.observations):
             yield self.observation(n)
 #            yield [self.feature(i) for i, x in enumerate(self._lookup) if x == n], self.observation(n)
             n += 1
 
     def iter_features_by_obs_id(self, obs_id: int) -> Feature:
-        """
-        Generator on features within a given obs_id
+        """Generator on features within a given obs_id.
+
         :param obs_id: Observation obs_id
         :returns: Feature
         """
         for i, x in enumerate(self._lookup):
             if x == obs_id:
                 yield self.feature(i)
 
+    def validate(self):
+        """Validation against the JSON Schema.
+        """
+        return validate(self._data)
+
     def _plot_observation(self, oid):
         obs = self.observation(oid)
         crs = self.crs
 
         bbox_times = [obs.tmin, obs.tmax, obs.tmax, obs.tmin, obs.tmin]
         bbox_times = crs.time_converter(bbox_times).datetime
         bbox_freqs = [obs.fmin, obs.fmin, obs.fmax, obs.fmax, obs.fmin]
@@ -246,15 +247,15 @@
                 TIME_COORDS[crs.properties['time_coords_id']]
             )
         else:
             raise NotImplemented()
 
         self._plot_feature(fid)
 
-        plt.xlabel(time_coords['name'])
+        plt.xlabel("Time")
         plt.ylabel(f"{crs.properties['spectral_coords']['type']} ({crs.properties['spectral_coords']['unit']})")
         plt.title(f'Feature #{fid}')
         plt.show()
 
     def to_votable(self, file_xml='votable_tfcat.xml'):
         """Exports the TFCat feature collection into VOTable.
```

### Comparing `TFCat-1.0.0rc2/tfcat/validate.py` & `TFCat-1.0.1/tfcat/validate.py`

 * *Files identical despite different names*

