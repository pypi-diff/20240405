# Comparing `tmp/cioblender-0.2.4b8-py2.py3-none-any.whl.zip` & `tmp/cioblender-0.2.4b9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 4769 bytes, number of entries: 4
--rw-r--r--  2.0 unx     9219 b- defN 24-Apr-04 16:47 cioblender-0.2.4b8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 16:47 cioblender-0.2.4b8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-04 16:47 cioblender-0.2.4b8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      319 b- defN 24-Apr-04 16:47 cioblender-0.2.4b8.dist-info/RECORD
-4 files, 9659 bytes uncompressed, 4147 bytes compressed:  57.1%
+-rw-r--r--  2.0 unx     9218 b- defN 24-Apr-04 17:25 cioblender-0.2.4b9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 17:25 cioblender-0.2.4b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-04 17:25 cioblender-0.2.4b9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      319 b- defN 24-Apr-04 17:25 cioblender-0.2.4b9.dist-info/RECORD
+4 files, 9658 bytes uncompressed, 4147 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: cioblender-0.2.4b8.dist-info/METADATA
+Filename: cioblender-0.2.4b9.dist-info/METADATA
 Comment: 
 
-Filename: cioblender-0.2.4b8.dist-info/WHEEL
+Filename: cioblender-0.2.4b9.dist-info/WHEEL
 Comment: 
 
-Filename: cioblender-0.2.4b8.dist-info/top_level.txt
+Filename: cioblender-0.2.4b9.dist-info/top_level.txt
 Comment: 
 
-Filename: cioblender-0.2.4b8.dist-info/RECORD
+Filename: cioblender-0.2.4b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cioblender-0.2.4b8.dist-info/METADATA` & `cioblender-0.2.4b9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cioblender
-Version: 0.2.4b8
+Version: 0.2.4b9
 Summary: Blender plugin for Conductor Cloud Rendering Platform.
 Home-page: https://github.com/ConductorTechnologies/cioblender
 Author: conductor
 Author-email: info@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
@@ -87,15 +87,15 @@
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit)
 
 ## Changelog
 
 ## Unreleased:
-* 0.2.4-beta.8 
+* 0.2.4-beta.9
   * Clearing Existing Blender Installation Prior to Upgrade
 * 0.2.4-beta.7
   * Adding support for Alembic and HDR assets
 * 0.2.4-beta.6
   * Introduced the Upload Daemon feature, enabling background asset uploads for uninterrupted Blender sessions. By selecting 'use_upload_daemon', the feature separates the upload process from active work, allowing for continuous productivity. The daemon efficiently coordinates with the server to identify and upload required assets post-job submission.
   * The Submission dialog has been updated to enable continued work in Blender following the submission process.
 * 0.2.4-beta.5
```

