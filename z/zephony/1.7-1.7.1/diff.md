# Comparing `tmp/zephony-1.7.tar.gz` & `tmp/zephony-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-1.7.tar", last modified: Wed Apr  3 20:33:54 2024, max compression
+gzip compressed data, was "zephony-1.7.1.tar", last modified: Thu Apr  4 23:08:07 2024, max compression
```

## Comparing `zephony-1.7.tar` & `zephony-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 20:33:54.755849 zephony-1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2024-04-03 20:33:36.000000 zephony-1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-03 20:33:54.755849 zephony-1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-03 20:33:36.000000 zephony-1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.751849 zephony-1.7/zephony/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 20:33:36.000000 zephony-1.7/zephony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2024-04-03 20:33:36.000000 zephony-1.7/zephony/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4145 2024-04-03 20:33:36.000000 zephony-1.7/zephony/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18046 2024-04-03 20:33:36.000000 zephony-1.7/zephony/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/zephony/models/
--rw-r--r--   0 root         (0) root         (0)    45030 2024-04-03 20:33:36.000000 zephony-1.7/zephony/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7377 2024-04-03 20:33:36.000000 zephony-1.7/zephony/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:33:54.755849 zephony-1.7/zephony.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 20:33:54.000000 zephony-1.7/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.940306 zephony-1.7.1/
+-rw-r--r--   0 root         (0) root         (0)      276 2024-04-04 23:08:07.940306 zephony-1.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-04 23:07:50.000000 zephony-1.7.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-04 23:08:07.940306 zephony-1.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      408 2024-04-04 23:07:50.000000 zephony-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.936306 zephony-1.7.1/zephony/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.936306 zephony-1.7.1/zephony/models/
+-rw-r--r--   0 root         (0) root         (0)    46626 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2024-04-04 23:07:50.000000 zephony-1.7.1/zephony/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:08:07.940306 zephony-1.7.1/zephony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      276 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 23:08:07.000000 zephony-1.7.1/zephony.egg-info/top_level.txt
```

### Comparing `zephony-1.7/zephony/decorators.py` & `zephony-1.7.1/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7/zephony/exceptions.py` & `zephony-1.7.1/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7/zephony/helpers.py` & `zephony-1.7.1/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-1.7/zephony/models/__init__.py` & `zephony-1.7.1/zephony/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -947,15 +947,16 @@
         #
         # and_(
         #     or_(a==b, c==d),
         #     or_(e==f, g==h),
         # )
 
         ors_list = []
-        for key in join['filters'].keys():
+        # if 'filters' is present in join
+        for key in join.get('filters', {}).keys():
             model_string, property_string = key.split('.')
             Model = model_string_alias_map[model_string]
 
             ands_list = []
             for allowed_value in join['filters'][key]:
                 ands_list.append(getattr(Model, property_string)==allowed_value)
 
@@ -1129,97 +1130,136 @@
             return results
 
         # Final list
         objects_details = []
 
         # To avoid row duplicates due to 1xN or NxN relationship
         primary_objects_map = {}
-        bridge_objects_maps = {}
-        for bridge_join_index, bridge_join in enumerate(bridge_joins):
-            bridge_objects_maps[bridge_join_index] = []
+        bridge_joins_maps = {
+            'bridge_objects_maps': {},
 
+            # This may not be needed if we want the same secondary objects
+            # connected through different bridge rows
+            'secondary_objects_maps': {},
+        }
+        for bridge_join in bridge_joins:
+            # bridge_objects_maps[bridge_join_index] = []
+            bridge_joins_maps['bridge_objects_maps'][bridge_join['details_list_key']] = []
+            bridge_joins_maps['secondary_objects_maps'][bridge_join['details_list_key']] = []
+
+        # Maps to avoid duplicates
+        list_joins_maps = {}
+        # bridge_joins_maps = {}
         for result in results:
             # If not joined, `result` represents the object else,
             # need to get the details via the attribute in the
             # result object
-
             if len(joins) > 0 or len(bridge_joins) > 0 or len(list_joins) > 0:
                 primary_object = getattr(result, cls.__name__)
             else:
                 primary_object = result
 
             if primary_object.id_ not in primary_objects_map:
                 primary_objects_map[primary_object.id_] = primary_object.get_details()
                 details = primary_objects_map[primary_object.id_]   # Helper variable
 
             for bridge_join_index, bridge_join in enumerate(bridge_joins):
+                # Initializing the final list
+                if bridge_join['details_list_key'] not in details:
+                    details[bridge_join['details_list_key']] = []
+
                 bridge_object_alias_name = (
                     f'{bridge_join["bridge_model"].__name__}'
                     # f'_{bridge_join["bridge_primary_id"]}'
                     f'_{bridge_join_index}'
                 )
                 bridge_object = getattr(
                     result,
                     # bridge_join['bridge_model'].__name__,
                     bridge_object_alias_name,
                 )
 
-                if bridge_object is not None:
-                    # Check if bridge object was already added
-                    if bridge_object.id_ in bridge_objects_maps[bridge_join_index]:
-                        continue
-                    else:
-                        bridge_objects_maps[bridge_join_index].append(bridge_object.id_)
+                # Skip if there's no bridge object
+                if bridge_object is None:
+                    continue
+
+                # Skip if bridge object was already part of the map
+                if bridge_object.id_ in bridge_joins_maps['bridge_objects_maps']\
+                        [bridge_join['details_list_key']]:
+                    continue
 
-                if bridge_join['details_list_key'] not in details:
-                    details[bridge_join['details_list_key']] = []
+                bridge_joins_maps['bridge_objects_maps']\
+                        [bridge_join['details_list_key']].append(bridge_object.id_)
 
                 # Secondary object was aliased in-case we were bridging
                 # between the same table
                 secondary_object_alias_name = (
                     f'{bridge_join["secondary_model"].__name__}'
                     # f'_{bridge_join["bridge_primary_id"]}'
                     f'_{bridge_join_index}'
                 )
                 secondary_object = getattr(
                     result,
                     # bridge_join['secondary_model'].__name__,
                     secondary_object_alias_name,
                 )
 
-                # Skip if there's no bridge entry
-                if secondary_object is not None:
-                    secondary_object_details = secondary_object.get_details()
-
-                    # If bridge table row details are requested
-                    if 'bridge_details_key' in bridge_join:
-                        secondary_object_details[
-                            bridge_join['bridge_details_key']
-                        ] = bridge_object.get_details()
+                # Skip if there's no secondary object
+                if secondary_object is None:
+                    continue
+
+                secondary_object_details = secondary_object.get_details()
+
+                # Skip if bridge object was already part of the map
+                if secondary_object.id_ in bridge_joins_maps['secondary_objects_maps']\
+                        [bridge_join['details_list_key']]:
+                    continue
+
+                bridge_joins_maps['secondary_objects_maps']\
+                        [bridge_join['details_list_key']].append(secondary_object.id_)
+
+                # If bridge table row details are requested
+                if 'bridge_details_key' in bridge_join:
+                    secondary_object_details[
+                        bridge_join['bridge_details_key']
+                    ] = bridge_object.get_details()
 
-                    details[bridge_join['details_list_key']].append(
-                        secondary_object_details
-                    )
+                details[bridge_join['details_list_key']].append(
+                    secondary_object_details
+                )
 
             for list_join_index, list_join in enumerate(list_joins):
+                # Initializing the map
+                if list_join['details_list_key'] not in list_joins_maps:
+                    list_joins_maps[list_join['details_list_key']] = []
+
+                # Initializing the final list
                 if list_join['details_list_key'] not in details:
                     details[list_join['details_list_key']] = []
 
                 secondary_object = getattr(
                     result,
                     list_join['secondary_model'].__name__,
                 )
 
-                # Skip if there's no list entry
-                if secondary_object is not None:
-                    secondary_object_details = secondary_object.get_details()
-
-                    details[list_join['details_list_key']].append(
-                        secondary_object_details
-                    )
+                # Skip if there's no object
+                if secondary_object is None:
+                    continue
+
+                # Skip if it's already part of the map
+                if secondary_object.id_ in list_joins_maps[list_join['details_list_key']]:
+                    continue
+
+                # Add to the map
+                list_joins_maps[list_join['details_list_key']].append(secondary_object.id_)
+
+                # Add to the final list
+                details[list_join['details_list_key']].append(
+                    secondary_object.get_details()
+                )
 
             for join in joins:
                 joined_object = getattr(result, f'{join[0].__name__}_{join[1]}')
 
                 if joined_object is not None:
                     details[join[2]] = joined_object.get_details()
                 else:
@@ -1234,10 +1274,9 @@
             return (objects_details, count)
 
         if first_item:
             if len(objects_details) == 0:
                 return None
             return objects_details[0]
 
-        ic('-----------------')
         return objects_details
```

### Comparing `zephony-1.7/zephony/validators.py` & `zephony-1.7.1/zephony/validators.py`

 * *Files identical despite different names*

