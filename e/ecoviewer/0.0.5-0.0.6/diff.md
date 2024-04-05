# Comparing `tmp/ecoviewer-0.0.5.tar.gz` & `tmp/ecoviewer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoviewer-0.0.5.tar", last modified: Fri Mar 29 18:50:59 2024, max compression
+gzip compressed data, was "ecoviewer-0.0.6.tar", last modified: Thu Apr  4 21:52:11 2024, max compression
```

## Comparing `ecoviewer-0.0.5.tar` & `ecoviewer-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/src/ecoviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/src/ecoviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/src/ecoviewer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/src/ecoviewer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/src/ecoviewer/config/configutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/src/ecoviewer/display/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/src/ecoviewer/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-03-29 18:50:32.000000 ecoviewer-0.0.5/src/ecoviewer/display/graphutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:50:59.559260 ecoviewer-0.0.5/src/ecoviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-29 18:50:59.000000 ecoviewer-0.0.5/src/ecoviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-29 18:50:59.000000 ecoviewer-0.0.5/src/ecoviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:50:59.000000 ecoviewer-0.0.5/src/ecoviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-29 18:50:59.000000 ecoviewer-0.0.5/src/ecoviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 18:50:59.000000 ecoviewer-0.0.5/src/ecoviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/src/ecoviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/src/ecoviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/src/ecoviewer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/src/ecoviewer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/src/ecoviewer/config/configutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/src/ecoviewer/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/src/ecoviewer/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-04-04 21:51:38.000000 ecoviewer-0.0.6/src/ecoviewer/display/graphutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:52:11.628040 ecoviewer-0.0.6/src/ecoviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-04 21:52:11.000000 ecoviewer-0.0.6/src/ecoviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 21:52:11.000000 ecoviewer-0.0.6/src/ecoviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:52:11.000000 ecoviewer-0.0.6/src/ecoviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 21:52:11.000000 ecoviewer-0.0.6/src/ecoviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 21:52:11.000000 ecoviewer-0.0.6/src/ecoviewer.egg-info/top_level.txt
```

### Comparing `ecoviewer-0.0.5/LICENSE` & `ecoviewer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.5/PKG-INFO` & `ecoviewer-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecoviewer-0.0.5/setup.cfg` & `ecoviewer-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoviewer
-version = 0.0.5
+version = 0.0.6
 authors = ["Ecotope"]
 description = Contains functions for use in HVAC Dash applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoviewer-0.0.5/src/ecoviewer/config/configutils.py` & `ecoviewer-0.0.6/src/ecoviewer/config/configutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,19 @@
         y2_fields = []
         for field_name, field_row in site_fields[site_fields['graph_id'] == index].iterrows():
             if field_name in df_columns:
                 column_details = {}
                 column_details["readable_name"] = field_row['pretty_name']
                 column_details["column_name"] = field_name
                 column_details["description"] = field_row["description"]
-                if not math.isnan(field_row["lower_bound"]):
-                # if not (field_row["lower_bound"] is None or not math.isnan(field_row["lower_bound"])):
+                # if not math.isnan(field_row["lower_bound"]):
+                if field_row["lower_bound"] is not None and not math.isnan(field_row["lower_bound"]):
                     column_details["lower_bound"] = field_row["lower_bound"]
-                if not math.isnan(field_row["upper_bound"]):
-                # if not (field_row["upper_bound"] is None or math.isnan(field_row["upper_bound"])):
+                # if not math.isnan(field_row["upper_bound"]):
+                if field_row["upper_bound"] is not None and math.isnan(field_row["upper_bound"]):
                     column_details["upper_bound"] = field_row["upper_bound"]
                 secondary_y = field_row['secondary_y']
                 if not secondary_y:
                     y1_fields.append(column_details)
                 else:
                     y2_fields.append(column_details)
         if len(y1_fields) == 0:
```

### Comparing `ecoviewer-0.0.5/src/ecoviewer/display/graphutils.py` & `ecoviewer-0.0.6/src/ecoviewer/display/graphutils.py`

 * *Files identical despite different names*

### Comparing `ecoviewer-0.0.5/src/ecoviewer.egg-info/PKG-INFO` & `ecoviewer-0.0.6/src/ecoviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoviewer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contains functions for use in HVAC Dash applications
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

