# Comparing `tmp/flowkit_jwt_generator-1.24.0.post0.dev15-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.24.0.post0.dev5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8538 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-05 16:05 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 24-Apr-05 16:05 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Apr-05 16:05 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Apr-05 16:05 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-Apr-05 16:05 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-05 16:05 flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 16:05 flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-05 16:05 flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-05 16:05 flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 24-Apr-05 16:05 flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/RECORD
-10 files, 17781 bytes uncompressed, 6840 bytes compressed:  61.5%
+Zip file size: 8523 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1333 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      962 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD
+10 files, 17774 bytes uncompressed, 6835 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-05T17:02:42+0100",
+ "date": "2024-04-03T17:21:49+0000",
  "dirty": false,
  "error": null,
- "full-revisionid": "2d6f9d5284e92d3254991e2e840da800f8ea245a",
- "version": "1.24.0.post0.dev15"
+ "full-revisionid": "c66bdfecb07382c6b69d6f73153359b4c5f1bb22",
+ "version": "1.24.0.post0.dev5"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.24.0.post0.dev15.dist-info/METADATA` & `flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flowkit_jwt_generator
-Version: 1.24.0.post0.dev15
+Name: flowkit-jwt-generator
+Version: 1.24.0.post0.dev5
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

