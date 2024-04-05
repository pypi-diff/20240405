# Comparing `tmp/wiliot-api-4.7.1.tar.gz` & `tmp/wiliot-api-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.7.1.tar", last modified: Mon Jan 29 09:11:22 2024, max compression
+gzip compressed data, was "wiliot-api-4.8.0.tar", last modified: Fri Apr  5 05:17:05 2024, max compression
```

## Comparing `wiliot-api-4.7.1.tar` & `wiliot-api-4.8.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     9554 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9048 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9514 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.333693 wiliot-api-4.7.1/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12211 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.333693 wiliot-api-4.7.1/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20455 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.333693 wiliot-api-4.7.1/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    23403 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    38029 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7096 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.337693 wiliot-api-4.7.1/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2024-01-29 09:11:12.000000 wiliot-api-4.7.1/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:11:22.333693 wiliot-api-4.7.1/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     9554 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-01-29 09:11:22.000000 wiliot-api-4.7.1/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11137 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10631 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20455 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52224 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.944864 wiliot-api-4.8.0/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-05 05:16:49.000000 wiliot-api-4.8.0/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 05:17:05.940864 wiliot-api-4.8.0/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11137 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-05 05:17:05.000000 wiliot-api-4.8.0/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.7.1/LICENSE` & `wiliot-api-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/PKG-INFO` & `wiliot-api-4.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-api
-Version: 4.7.1
-Summary: A library for interacting with Wiliot's private Cloud API
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud APIs from Python
 
 ### Installing pyWiliot
 ````commandline
 pip install wiliot-api
@@ -38,21 +21,24 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.0:
+
+* Added support for new labels (key:value pairs for platform entities)
+
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
 * Added option to get a new and unique reel id for manufacturing
 * Added the option to get post process tables for manufacturing partners
 * Added the option to add temperature calibration point to a tag
-* Added assetSeenInLocation to the list of generateable events
 
 ### Version 4.6.4:
 
 * Changed get_asset() implementation to use dedicated endpoint instead of metadataFetch
 
 
 ### Version 4.6.3:
@@ -207,15 +193,46 @@
 # Get a list of zones in a location
 platform.get_zones(location_id="my-location-id")
 
 # Associate a bridge to a zone
 platform.create_zone_association(location_id="my-location-id", zone_id="my-zone-id",
                                  association_type=ZoneAssociationType.BRIDGE, association_value="my-bridge-id")
 
-
+# Labels (key:value pairs)
+# Get a list of key:value pairs for an asset
+platform.get_entity_keys_values(entity_type=EntityType.ASSET,
+                                entity_id="my-asset-id")
+# Supported entity types:
+# * ASSET
+# * LOCATION
+# * ZONE
+# * BRIDGE
+# * GATEWAY
+
+# Get a specific key:value for a zone
+platform.get_entity_keys_values(entity_type=EntityType.ZONE,
+                                entity_id="my-zone-id",
+                                key="special_zone")
+
+# Set one or more key:value pairs for one or more entities (of the same type)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"})
+
+# The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
+# To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"},
+                                      overwrite_existing=True)
+
+# Delete key:value from one or more entities
+platform.delete_entities_key_value(entity_type=EntityType.LOCATION,
+                                   entity_ids=["location-1-id", "location-2-id"],
+                                   key='special_zone')
 ```
 
 ### Edge API
 
 ```python
 # Import the library
 from wiliot_api.edge.edge import *
@@ -305,9 +322,7 @@
 # .....
 req = wiliot_manufacturing.change_pixel_owner_by_file("from_owner_id", "to_owner_id", "/path/to/file")
 
 # Each of the functions above returns a string representing a request ID. To check on the status of the request
 print(wiliot_manufacturing.get_pixel_change_request_status(req))
 
 ```
-
-
```

### Comparing `wiliot-api-4.7.1/README.md` & `wiliot-api-4.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-api
+Version: 4.8.0
+Summary: A library for interacting with Wiliot's private Cloud API
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud APIs from Python
 
 ### Installing pyWiliot
 ````commandline
 pip install wiliot-api
@@ -21,21 +38,24 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.0:
+
+* Added support for new labels (key:value pairs for platform entities)
+
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
 * Added option to get a new and unique reel id for manufacturing
 * Added the option to get post process tables for manufacturing partners
 * Added the option to add temperature calibration point to a tag
-* Added assetSeenInLocation to the list of generateable events
 
 ### Version 4.6.4:
 
 * Changed get_asset() implementation to use dedicated endpoint instead of metadataFetch
 
 
 ### Version 4.6.3:
@@ -190,15 +210,46 @@
 # Get a list of zones in a location
 platform.get_zones(location_id="my-location-id")
 
 # Associate a bridge to a zone
 platform.create_zone_association(location_id="my-location-id", zone_id="my-zone-id",
                                  association_type=ZoneAssociationType.BRIDGE, association_value="my-bridge-id")
 
-
+# Labels (key:value pairs)
+# Get a list of key:value pairs for an asset
+platform.get_entity_keys_values(entity_type=EntityType.ASSET,
+                                entity_id="my-asset-id")
+# Supported entity types:
+# * ASSET
+# * LOCATION
+# * ZONE
+# * BRIDGE
+# * GATEWAY
+
+# Get a specific key:value for a zone
+platform.get_entity_keys_values(entity_type=EntityType.ZONE,
+                                entity_id="my-zone-id",
+                                key="special_zone")
+
+# Set one or more key:value pairs for one or more entities (of the same type)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"})
+
+# The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
+# To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"},
+                                      overwrite_existing=True)
+
+# Delete key:value from one or more entities
+platform.delete_entities_key_value(entity_type=EntityType.LOCATION,
+                                   entity_ids=["location-1-id", "location-2-id"],
+                                   key='special_zone')
 ```
 
 ### Edge API
 
 ```python
 # Import the library
 from wiliot_api.edge.edge import *
@@ -288,7 +339,9 @@
 # .....
 req = wiliot_manufacturing.change_pixel_owner_by_file("from_owner_id", "to_owner_id", "/path/to/file")
 
 # Each of the functions above returns a string representing a request ID. To check on the status of the request
 print(wiliot_manufacturing.get_pixel_change_request_status(req))
 
 ```
+
+
```

### Comparing `wiliot-api-4.7.1/bitbucket-pipelines.yml` & `wiliot-api-4.8.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/setup.py` & `wiliot-api-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/__init__.py` & `wiliot-api-4.8.0/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/api_client.py` & `wiliot-api-4.8.0/wiliot_api/api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
         full_path = base_path_to_use + urllib.parse.quote(path)
         url_param_path = "" if url_params is None \
             else ("?" + "&".join([f"{urllib.parse.quote(k)}={urllib.parse.quote(v)}" for k, v in url_params.items()]))
         full_path += url_param_path
-        data = json.dumps(payload) if isinstance(payload, dict) else payload
+        data = json.dumps(payload) if isinstance(payload, dict) or isinstance(payload, list) else payload
         headers = self.headers if override_headers is None else override_headers
         response = requests.post(url=full_path, headers=headers, data=data, params=params)
         try:
             message = response.json()
         except:
             message = response.text
         if isinstance(message, str):
@@ -219,21 +219,48 @@
             message = response.text
         if isinstance(message, str):
             message = {"data": message}
         message.update({'status_code': response.status_code})
         if int(response.status_code/100) != 2:
             raise WiliotCloudError(message)
         return message
+
+    def _patch(self, path, payload, params=None, files=None, override_client_path=None, override_api_version=None,
+               override_headers=None, url_params=None, verbose=False):
+        self._renew_token()
+        base_path_to_use = self._get_base_url(override_client_path=override_client_path,
+                                              override_api_version=override_api_version)
+        full_path = base_path_to_use + urllib.parse.quote(path)
+        url_param_path = "" if url_params is None \
+            else ("?" + "&".join([f"{urllib.parse.quote(k)}={urllib.parse.quote(v)}" for k, v in url_params.items()]))
+        full_path += url_param_path
+        data = json.dumps(payload) if isinstance(payload, dict) or isinstance(payload, list) else payload
+        headers = self.headers if override_headers is None else override_headers
+        response = requests.patch(url=full_path, headers=headers, data=data, params=params)
+        try:
+            message = response.json()
+        except:
+            message = response.text
+        if isinstance(message, str):
+            message = {"data": message}
+        message.update({'status_code': response.status_code})
+        if int(response.status_code/100) != 2:
+            desc = f'path:{full_path}, headers:{self.headers}, data:{data}, params:{params}'
+            if verbose:
+                message['request_details'] = desc
+            raise WiliotCloudError(message)
+        return message
     
     def _delete(self, path, payload=None, override_client_path=None, override_api_version=None):
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
         response = requests.delete(base_path_to_use + urllib.parse.quote(path), headers=self.headers,
                                    data=json.dumps(payload) if payload is not None else None)
         if int(response.status_code/100) != 2:
             raise WiliotCloudError(response.text)
         try:
             message = response.json()
         except:
             message = response.text
+        message.update({'status_code': response.status_code})
         return message
```

### Comparing `wiliot-api-4.7.1/wiliot_api/edge/edge.py` & `wiliot-api-4.8.0/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.8.0/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.8.0/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.8.0/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.8.0/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/platform/platform.py` & `wiliot-api-4.8.0/wiliot_api/platform/platform.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,14 +75,21 @@
     pass
 
 
 class ZoneNotFound(Exception):
     pass
 
 
+class KeyNotFound(Exception):
+    pass
+
+class KeyValueNotFound(Exception):
+    pass
+
+
 class TagRole(Enum):
     DEFAULT = 'DEFAULT'
     REFERENCE = 'REFERENCE'
 
 
 class Event(Enum):
     LOCATION = 'location'
@@ -100,14 +107,23 @@
     BRIDGE = 'bridge'
     TAG = 'tag'
 
 
 class LocationAssociationType(Enum):
     BRIDGE = 'bridge'
 
+class EntityType(Enum):
+    GATEWAY = 'gateway'
+    BRIDGE = 'bridge'
+    ASSET = 'asset'
+    LOCATION = 'location'
+    ZONE = 'zone'
+    CATEGORY = 'category'
+
+
 
 class PlatformClient(Client):
     def __init__(self, api_key, owner_id, env='prod', region='us-east-2', cloud='', log_file=None, logger_=None):
         self.client_path = "traceability/owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
         super().__init__(api_key=api_key, env=env, region=region, cloud=cloud, log_file=log_file, logger_=logger_)
 
@@ -955,7 +971,287 @@
         :param start_time: Integer - timestamp in seconds to start counting from
         :param end_time: Integer - timestamp in seconds to end counting at
         """
         path = f"connection/{connection_id}/startTime/{start_time}/endTime/{end_time}/events"
         print(path)
         res = self._get(path, override_client_path=f"owner/{self.owner_id}/")
         return res
+
+    #### New Labels ##########
+    def _create_labels(self, entity_type: EntityType, keys: list):
+        """
+        Create a new label (more precisely, a label key)
+        :param entity_type: EntityType - The entity type (one of the EntityTypes) - required
+        :param keys: List: Required - list of strings to create labels from
+        """
+        path = "label"
+        payload = [
+            {
+                "entityType": entity_type.value,
+                "key": k
+            }
+            for k in keys
+        ]
+        res = self._post(path, payload)
+        return res
+
+    def _get_labels(self, entity_type: EntityType=None, key: str=None):
+        """
+        Get a list of labels
+        :param entity_type: EntityType: Optional -Only return labels for entities of this type
+        :param key: String: Optional - only return labels with this key in them
+        """
+        path = "label"
+        params = {}
+        if entity_type is not None:
+            params[ 'entityType'] = entity_type.value
+        if key is not None:
+            params[ 'key'] = key
+        res = self._get(path, params=params)
+        return res['data']
+
+    def _update_label(self, label_id: str, key: str):
+        """
+        Update a label's key
+        :param label_id: String - required - The label's ID
+        :param key: String: String - Required - The new key for the label
+        """
+        path = f"label/{label_id}"
+        payload = {
+            'key': key
+        }
+        try:
+            res = self._patch(path, payload)
+            if res['status_code'] == 200:
+                return True
+            else:
+                return False
+        except WiliotCloudError as wce:
+            print(f"Failed to updated label {label_id}")
+            raise wce
+
+    def _delete_label(self, label_id: str):
+        """
+        Delete a label - Will also delete all instantiated versions of this label
+        :param label_id: String - required - The label's ID
+        returns: True is label was successfully deleted
+        """
+        path = f"label/{label_id}"
+        try:
+            res = self._delete(path)
+            return res['status_code'] == 200
+        except WiliotCloudError as wce:
+            print(f"Failed to delete label {label_id}")
+            raise wce
+
+    def _associate_labels_to_entities(self, entity_type: EntityType, entity_ids: list, label_values: list):
+        """
+        Associate one or more existing labels to an entity
+        :param entity_type: EntityType - Required - The type of entity to associate with the label
+        :param entity_ids: List - Required - A list of entity IDs to associate with the label
+        :param label_values: List - Required - List of dictionaries representing labels to associate with the
+        entity and their values. Each element in the list should be a dictionary with the following fields:
+            labelId - The ID of the label to associate
+            value - The value to assign to this label
+            For example: {"labelId": "7820d54e-eb2c-40db-9bbd-e8271ec06f95", "value": "5G"}
+        :return: True is entity was successfully associated
+        """
+        path = f"entity/{entity_type.value}/label"
+        assert all([isinstance(e, dict) and 'labelId' in list(e.keys()) and 'value' in list(e.keys()) for e in label_values]), f"label_values must contain a list of dictionaries each with a labelId field and a value field each"
+        payload = [{
+            'entityId': entity_id,
+            'labels': label_values
+        } for entity_id in entity_ids]
+        res = self._post(path, payload)
+        return res
+
+    def _update_label_value_for_entities(self, entity_type: EntityType, entity_ids: list, label_values: list):
+        """
+        Update the association value for one ore more entities
+        :param entity_type: EntityType - Required - The type of entity to update the value for
+        :param entity_ids: List - Required - A list of entity IDs to update the value for
+        :param label_values: List - Required - List of dictionaries representing labels to update
+        Each element should be a discionary with the following fields
+            labelId - The ID of the label to associate
+            value - The value to update for this label
+            For example: {"labelId": "7820d54e-eb2c-40db-9bbd-e8271ec06f95", "value": "5G"}
+        """
+        path = f"entity/{entity_type.value}/label"
+        assert all([isinstance(e, dict) and 'labelId' in list(e.keys()) and 'value' in list(e.keys()) for e in label_values]), f"label_values must contain a list of dictionaries each with a labelId field and a value field each"
+        payload = [{
+            'entityId': entity_id,
+            'labels': label_values
+        } for entity_id in entity_ids]
+        res = self._patch(path, payload)
+        return res
+
+    def _disassociate_labels_from_entities(self, entity_type: EntityType, entity_ids: list, labels: list):
+        """
+        Disassociate one or more existing labels to an entity
+        :param entity_type: EntityType - Required - The type of entity to disassociate from the label
+        :param entity_ids: List - Required - A list of entity IDs to disassociate from the label
+        :param label_values: List - Required - List of label IDs to disassociate
+        :return: True is entities was successfully disassociated
+        """
+        path = f"entity/{entity_type.value}/label"
+        payload = [{
+            'entityId': entity_id,
+            'labelIds': labels
+        } for entity_id in entity_ids]
+        res = self._delete(path, payload)
+        return res['status_code'] == 200
+
+    def get_entity_labels(self, entity_type: EntityType, entity_id: str=None, key: str=None):
+        """
+        Get all labels and values either for a specific entity or for all entities of a certain type
+        :param entity_type: EntityType - required - the type of entity to return labels and values for
+        :param entity_id: String - Optional - If provided returns only label and value pairs for the entity with the
+        specified entity_id
+        :param key: String - optional - filter only labels with the specified key
+        """
+        if entity_type is None:
+            path = f"entity/{entity_type.value}/label"
+        else:
+            path = f"entity/{entity_type.value}/{entity_id}/label"
+        params = {}
+        if key is not None:
+            params['key'] = key
+        return self._get(path, params=params).get('data',[])
+
+    def get_label_values(self, entity_type: EntityType, label_id: str=None):
+        """
+        Get all values of a label for a specific entity type
+        :param entity_type: EntityType - Required - the type of entity to search for
+        :param label_id: String - Required - the label ID to search for
+        """
+        path = f"entity/{entity_type.value}/label/{label_id}/values"
+        return self._get(path)
+
+    def set_keys_values_for_entities(self, entity_type: EntityType, entity_ids: list, keys_values: dict, overwrite_existing: bool = False):
+        """
+        Create a new key value pair for a list of entities
+        :param entity_type: EntityType - Required - the entity type of the entity to add the key value pair to
+        :param entity_ids: List - Required - a list of entity IDs to add the key value pairs to
+        :param keys_values: Dictionary - Required - A dictionary of key and values to add to the specified entities
+        :param overwrite_existing: Boolean - Optional - If True any existing association to the requested labels will not be overwritten
+        :return: Boolean - True if successful, False otherwise
+        """
+        # For each key value pair in the keys_value dictionary - create the label if it doesn't already exist
+        for key, value in keys_values.items():
+            try:
+                res = self._create_labels(entity_type=entity_type, keys=[key])
+                # Since we're only trying to create a single label - a success means we were able to
+                label_id = res['data'][0]['id']
+            except WiliotCloudError as wce:
+                # Check if the error is that the label already exists
+                if wce.args[0].get('data', {}).get('failedLabels', [{}])[0].get('reason', '').find('exist') != -1:
+                    label_id = wce.args[0]['data']['failedLabels'][0].get('labelId', None)
+                else:
+                    print(f"Failed to create label {key} for entity type {entity_type} due to: {wce.args[0]}. Will not create a key-value pair")
+                    continue
+            # Once we have a label ID - new or existing - associate a new value for a specific entity
+            try:
+                res = self._associate_labels_to_entities(entity_type=entity_type,
+                                                         entity_ids=entity_ids,
+                                                         label_values=[{"labelId": label_id, "value": value}])
+                if res['status_code'] == 200:
+                    return True
+                elif res['status_code'] == 207:
+                    # Partial success
+                    if overwrite_existing:
+                        for entity in res['data']:
+                            if entity['status'].lower() != 'success':
+                                for label in entity['failedLabels']:
+                                    if label['reason'].find('exist') != -1:
+                                        # If there is already a value associated with this label for this entity - update it
+                                        self._update_label_value_for_entities(entity_type=entity_type,
+                                                                              entity_ids=[entity['entityId']],
+                                                                              label_values=[{'labelId': label['labelId'], 'value': value}])
+                                        return True
+                else:
+                    return False
+
+            except WiliotCloudError as wce:
+                # If asked to overwrite - examine the results
+                if overwrite_existing:
+                    for entity in wce.args[0]['data']:
+                        for label in entity.get('failedLabels'):
+                            if label.get('reason').find('exists') != -1:
+                                self._update_label_value_for_entities(entity_type=entity_type,
+                                                                      entity_ids=[entity['entityId']],
+                                                                      label_values=[{'labelId': label['labelId'], 'value': value}])
+                                return True
+                else:
+                    raise
+
+    def get_entity_keys_values(self, entity_type: EntityType, entity_id: str, key: str=None):
+        """
+        Get all key value pairs for an entity
+        :param entity_type: EntityType - Required - the entity type of the entity to add the key value pair to
+        :param entity_id: String - Required - the ID of the entity to query
+        :param key: String - Optional - filter only values for the provided key
+        :return: List of key value pairs for the provided entity
+        """
+        path = f"/entity/{entity_type.value}/{entity_id}/label"
+        params = {}
+        if key is not None:
+            params['key'] = key
+        entity_key_values = self._get(path=path, params=params)
+        return entity_key_values.get('data', [])
+
+    def delete_entities_key_value(self, entity_type: EntityType, entity_ids: list, key: str):
+        """
+        Delete a key value pair for the provided entity
+        :param entity_type: EntityType - Required - The entity type of the entity to delete the key value
+        :param entity_ids: List - Required - A list of the entity IDs of the entities to delete the key for
+        :param key: String - Required - A key to remove
+        """
+        path = f"/entity/{entity_type.value}/label"
+        try:
+            # Get all labels
+            label = self._get_labels(entity_type=entity_type, key=key)[0]
+            label_ids = [label['id']]
+        except IndexError:
+            raise KeyNotFound
+        payload = [{
+            'entityId': entity_id,
+            'labelIds': label_ids
+        } for entity_id in entity_ids]
+        try:
+            res = self._delete(path, payload)
+        except Exception as e:
+            res = json.loads(e.args[0])
+            if res.get('data', {})[0].get('failedLabels', [])[0].get('reason').lower().find('not found') != -1:
+                raise KeyValueNotFound
+            else:
+                raise e
+        return res['status_code'] == 200
+
+
+    # Generic events API
+    def generate_generic_event(self, asset_id:str, category_id:str, event_name:str, value:str,
+                               key_set:list, confidence:float=1.0, start:int=None, end:int=None):
+        """
+        Generate a generic event
+        :param asset_id: String - Required - The event's asset ID
+        :param category_id: String - required - The events category ID
+        """
+        path = "event-api-record"
+        payload = {
+            "assetId": asset_id,
+            "categoryId": category_id,
+            "eventName": event_name,
+            "value": value,
+            "keySet": [
+                {"key": ks["key"], "value": ks["value"]} for ks in key_set
+            ],
+            "confidence": confidence,
+        }
+        if start is not None:
+            payload["start"] = start
+        if end is not None:
+            payload["end"] = end
+        try:
+            res = self._post(path, payload, override_client_path="owner/{owner_id}/".format(owner_id=self.owner_id))
+            return res['status_code'] == 200
+        except WiliotCloudError as wce:
+            print(f"Failed to generate generic event due to: {wce.args[0]}")
```

### Comparing `wiliot-api-4.7.1/wiliot_api/platform/platform_models.py` & `wiliot-api-4.8.0/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/security/security.py` & `wiliot-api-4.8.0/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api/utils/get_version.py` & `wiliot-api-4.8.0/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.7.1/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.8.0/wiliot_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.7.1
+Version: 4.8.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,21 +38,24 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.0:
+
+* Added support for new labels (key:value pairs for platform entities)
+
 ### Version 4.7.1:
 
 * Added option to upload testers data to cloud
 * Added option to get a new and unique reel id for manufacturing
 * Added the option to get post process tables for manufacturing partners
 * Added the option to add temperature calibration point to a tag
-* Added assetSeenInLocation to the list of generateable events
 
 ### Version 4.6.4:
 
 * Changed get_asset() implementation to use dedicated endpoint instead of metadataFetch
 
 
 ### Version 4.6.3:
@@ -207,15 +210,46 @@
 # Get a list of zones in a location
 platform.get_zones(location_id="my-location-id")
 
 # Associate a bridge to a zone
 platform.create_zone_association(location_id="my-location-id", zone_id="my-zone-id",
                                  association_type=ZoneAssociationType.BRIDGE, association_value="my-bridge-id")
 
-
+# Labels (key:value pairs)
+# Get a list of key:value pairs for an asset
+platform.get_entity_keys_values(entity_type=EntityType.ASSET,
+                                entity_id="my-asset-id")
+# Supported entity types:
+# * ASSET
+# * LOCATION
+# * ZONE
+# * BRIDGE
+# * GATEWAY
+
+# Get a specific key:value for a zone
+platform.get_entity_keys_values(entity_type=EntityType.ZONE,
+                                entity_id="my-zone-id",
+                                key="special_zone")
+
+# Set one or more key:value pairs for one or more entities (of the same type)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"})
+
+# The previous call will fail if the provided gateways already have a value for a key called "special_gateway" set
+# To force an overwrite of existing key value, use the overwrite_existing argument (False by default)
+platform.set_keys_values_for_entities(entity_type=EntityType.GATEWAY,
+                                      entity_ids=["gateway-id-1", "gateway-id-2"],
+                                      keys_values={"special_gateway": "True"},
+                                      overwrite_existing=True)
+
+# Delete key:value from one or more entities
+platform.delete_entities_key_value(entity_type=EntityType.LOCATION,
+                                   entity_ids=["location-1-id", "location-2-id"],
+                                   key='special_zone')
 ```
 
 ### Edge API
 
 ```python
 # Import the library
 from wiliot_api.edge.edge import *
```

### Comparing `wiliot-api-4.7.1/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.8.0/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

