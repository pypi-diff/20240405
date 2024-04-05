# Comparing `tmp/shipdataprocess-0.8.2.tar.gz` & `tmp/shipdataprocess-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shipdataprocess-0.8.2.tar", last modified: Mon Aug 21 11:12:44 2023, max compression
+gzip compressed data, was "dist/shipdataprocess-0.8.3.tar", last modified: Fri Apr  5 09:26:01 2024, max compression
```

## Comparing `shipdataprocess-0.8.2.tar` & `shipdataprocess-0.8.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/
--rw-r--r--   0 root         (0) root         (0)     3556 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/CHANGES.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess/
--rw-r--r--   0 root         (0) root         (0)      497 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess/_version.py
--rw-r--r--   0 root         (0) root         (0)    17757 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/shipdataprocess/shiptype.py
--rw-r--r--   0 root         (0) root         (0)    19311 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/shipdataprocess/standardize.py
--rw-r--r--   0 root         (0) root         (0)     9071 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/shipdataprocess/normalize.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/shipdataprocess/collapse.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/shipdataprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11357 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1414 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1801 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       90 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      277 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    83607 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/versioneer.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1801 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-21 11:12:44.000000 shipdataprocess-0.8.2/shipdataprocess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      879 2023-08-21 11:12:16.000000 shipdataprocess-0.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess/
+-rw-r--r--   0 root         (0) root         (0)     5154 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/collapse.py
+-rw-r--r--   0 root         (0) root         (0)    17757 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/shiptype.py
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/normalize.py
+-rw-r--r--   0 root         (0) root         (0)    19542 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/shipdataprocess/standardize.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/shipdataprocess/_version.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      277 2024-04-05 09:26:01.000000 shipdataprocess-0.8.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)    83607 2024-04-05 09:25:32.000000 shipdataprocess-0.8.3/versioneer.py
```

### Comparing `shipdataprocess-0.8.2/CHANGES.md` & `shipdataprocess-0.8.3/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,9 +38,10 @@
 v0.6.16, 2020-11-26 -- Make smart_upper() to capture multiple URLs not to capitalize them  
 v0.6.17, 2021-07-30 -- Add Indonesian prefix and Chinese HAO suffix to the list of prefix/suffix to be removed 
 v0.6.18, 2021-08-04 -- Fix a bug in normalize_callsign() regarding NULL/NONE  
 v0.7.0, 2022-01-26 -- Fix it to work only in Python 3.6 or above, codes are compliant with PEP8, dependencies are clearer (Django removed)   
 v0.7.1, 2022-01-27 -- Fix a bug related to the shift to Python 3.6 or above compatibility  
 v0.8.0, 2023-06-07 -- Improve normalize_shipname() to replace STA and STA. values to SANTA and fix discrepancy with the trailing 0s and suffix N
 v0.8.2, 2023-08-21 -- Fix a bug in normalize_shipname() regarding STA./STA replace feature.
+v0.8.3, 2024-04-04 -- Fix a bug in standardize_int_str(). Check if string is an integer before trying to cast.
```

### Comparing `shipdataprocess-0.8.2/shipdataprocess/shiptype.py` & `shipdataprocess-0.8.3/shipdataprocess/shiptype.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/shipdataprocess/standardize.py` & `shipdataprocess-0.8.3/shipdataprocess/standardize.py`

 * *Files 5% similar despite different names*

```diff
@@ -436,14 +436,28 @@
             return re.sub("FISHERY", "FISHERIES", elem)
         else:
             raise ValueError("Unknown type received")
     else:
         return None
 
 
+def clean_int_str(x):
+    return re.sub(r"[^\d.]", "", str(x))
+
+def clean_int_str_in_pd_element(x):
+    temporal_value = clean_int_str(x)
+    if temporal_value == "":
+        return None
+
+    temporal_value = str(int(float(temporal_value)))
+    if (not pd.isna(temporal_value)) & (temporal_value != ""):
+        return temporal_value
+    else:
+        return None
+
 def standardize_int_str(elem, check_field=True):
     """
     This module standardizes an integer in the form of string
     because Pandas Series or DataFrame considers a column of integers
     with Nulls as a column of float. Save it as a string column so that
     it can be uploaded as integer columns when uploading to BigQuery.
 
@@ -451,28 +465,26 @@
     that contains a string field
     :param check_field: Boolean, field that contains the given strings
     :return: Same as the input elem type
     """
     if check_field:
         if type(elem) == pd.core.series.Series:
             return elem.apply(
-                lambda x: str(int(float(re.sub(r"[^\d.]", "", str(x)))))
-                if (x == x) & (x is not None) & (x != "")
-                else None
-            )
+                lambda x: clean_int_str_in_pd_element(x)
+                if not pd.isna(x)
+                else None )
         elif type(elem) == pd.core.frame.DataFrame:
             return elem[check_field].apply(
-                lambda x: str(int(float(re.sub(r"[^\d.]", "", str(x)))))
-                if (x == x) & (x is not None) & (x != "")
-                else None
-            )
+                lambda x: clean_int_str_in_pd_element(x)
+                if not pd.isna(x)
+                else None )
         elif (elem != elem) | (elem is None) | (elem == ""):
             return None
         elif (type(elem) == str) | (type(elem) == int) | (type(elem) == float):
-            return str(int(float(re.sub(r"[^\d.]", "", str(elem)))))
+            return clean_int_str(elem)
         else:
             raise ValueError("Unknown type received")
     else:
         return None
 
 
 def standardize_time(elem, check_field=True):
```

### Comparing `shipdataprocess-0.8.2/shipdataprocess/normalize.py` & `shipdataprocess-0.8.3/shipdataprocess/normalize.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/shipdataprocess/collapse.py` & `shipdataprocess-0.8.3/shipdataprocess/collapse.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/shipdataprocess/__init__.py` & `shipdataprocess-0.8.3/shipdataprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/LICENSE` & `shipdataprocess-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/README.md` & `shipdataprocess-0.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# shipdataprocess (current latest version 0.8.2)
+# shipdataprocess (current latest version 0.8.3)
 
 shipdataprocess provides packages and modules that help users process raw ship data. The data may come from Automatic identification system (AIS) transmission or others. Ship data includes vessel's name, callsign, shiptype, geartype information etc. You might find the packages here useful for normalizing ship names and IRCS (International Radio Call Sign) and for dealing with various types of ships and fishing gears. Typical usage often looks like this:
 
     #!/usr/bin/env python
 
     from shipdataprocess.normalize import normalize_shipname, normalize_callsign
```

### Comparing `shipdataprocess-0.8.2/PKG-INFO` & `shipdataprocess-0.8.3/shipdataprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shipdataprocess
-Version: 0.8.2
+Version: 0.8.3
 Summary: Useful modules to process vessel data
 Home-page: https://github.com/GlobalFishingWatch/shipdataprocess
 Author: Jaeyoon Park
 Author-email: jaeyoon@globalfishingwatch.org
 License: Apache 2.0
 Keywords: ship,vessel,fishing,normalization
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
-# shipdataprocess (current latest version 0.8.2)
+# shipdataprocess (current latest version 0.8.3)
 
 shipdataprocess provides packages and modules that help users process raw ship data. The data may come from Automatic identification system (AIS) transmission or others. Ship data includes vessel's name, callsign, shiptype, geartype information etc. You might find the packages here useful for normalizing ship names and IRCS (International Radio Call Sign) and for dealing with various types of ships and fishing gears. Typical usage often looks like this:
 
     #!/usr/bin/env python
 
     from shipdataprocess.normalize import normalize_shipname, normalize_callsign
```

### Comparing `shipdataprocess-0.8.2/versioneer.py` & `shipdataprocess-0.8.3/versioneer.py`

 * *Files identical despite different names*

### Comparing `shipdataprocess-0.8.2/shipdataprocess.egg-info/PKG-INFO` & `shipdataprocess-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shipdataprocess
-Version: 0.8.2
+Version: 0.8.3
 Summary: Useful modules to process vessel data
 Home-page: https://github.com/GlobalFishingWatch/shipdataprocess
 Author: Jaeyoon Park
 Author-email: jaeyoon@globalfishingwatch.org
 License: Apache 2.0
 Keywords: ship,vessel,fishing,normalization
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
-# shipdataprocess (current latest version 0.8.2)
+# shipdataprocess (current latest version 0.8.3)
 
 shipdataprocess provides packages and modules that help users process raw ship data. The data may come from Automatic identification system (AIS) transmission or others. Ship data includes vessel's name, callsign, shiptype, geartype information etc. You might find the packages here useful for normalizing ship names and IRCS (International Radio Call Sign) and for dealing with various types of ships and fishing gears. Typical usage often looks like this:
 
     #!/usr/bin/env python
 
     from shipdataprocess.normalize import normalize_shipname, normalize_callsign
```

### Comparing `shipdataprocess-0.8.2/setup.py` & `shipdataprocess-0.8.3/setup.py`

 * *Files identical despite different names*

