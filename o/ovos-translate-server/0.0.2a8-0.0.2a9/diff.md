# Comparing `tmp/ovos_translate_server-0.0.2a8-py3-none-any.whl.zip` & `tmp/ovos_translate_server-0.0.2a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8609 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3147 b- defN 24-Feb-23 20:49 ovos_translate_server/__init__.py
--rw-r--r--  2.0 unx     1136 b- defN 24-Feb-23 20:49 ovos_translate_server/__main__.py
--rw-r--r--  2.0 unx      177 b- defN 24-Feb-23 20:49 ovos_translate_server/version.py
--rw-r--r--  2.0 unx    11347 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      980 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      950 b- defN 24-Feb-23 20:49 ovos_translate_server-0.0.2a8.dist-info/RECORD
-10 files, 17931 bytes uncompressed, 6939 bytes compressed:  61.3%
+Zip file size: 8594 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3147 b- defN 24-Apr-05 21:20 ovos_translate_server/__init__.py
+-rw-r--r--  2.0 unx     1136 b- defN 24-Apr-05 21:20 ovos_translate_server/__main__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-Apr-05 21:20 ovos_translate_server/version.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      930 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      950 b- defN 24-Apr-05 21:20 ovos_translate_server-0.0.2a9.dist-info/RECORD
+10 files, 17881 bytes uncompressed, 6924 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: ovos_translate_server/__main__.py
 Comment: 
 
 Filename: ovos_translate_server/version.py
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/LICENSE.md
+Filename: ovos_translate_server-0.0.2a9.dist-info/LICENSE.md
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/METADATA
+Filename: ovos_translate_server-0.0.2a9.dist-info/METADATA
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/WHEEL
+Filename: ovos_translate_server-0.0.2a9.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/entry_points.txt
+Filename: ovos_translate_server-0.0.2a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/top_level.txt
+Filename: ovos_translate_server-0.0.2a9.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/zip-safe
+Filename: ovos_translate_server-0.0.2a9.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_translate_server-0.0.2a8.dist-info/RECORD
+Filename: ovos_translate_server-0.0.2a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_translate_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 8
+VERSION_ALPHA = 9
 # END_VERSION_BLOCK
```

## Comparing `ovos_translate_server-0.0.2a8.dist-info/LICENSE.md` & `ovos_translate_server-0.0.2a9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ovos_translate_server-0.0.2a8.dist-info/METADATA` & `ovos_translate_server-0.0.2a9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-translate-server
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: simple flask server to host OpenVoiceOS translate plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-translate-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin lang detect translate OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -16,12 +16,11 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask
 Requires-Dist: ovos-plugin-manager
-Requires-Dist: ovos-lang-detector-classics-plugin
 
 UNKNOWN
```

## Comparing `ovos_translate_server-0.0.2a8.dist-info/RECORD` & `ovos_translate_server-0.0.2a9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ovos_translate_server/__init__.py,sha256=Y8TwYfxJqlUHA1J7_gXGOkCvJRtcR2hYqp0wwo6r_ms,3147
 ovos_translate_server/__main__.py,sha256=Q7MJsG_UBzaul0W9blfwJHDLCwGG3ZbrSlQFhOGb5Io,1136
-ovos_translate_server/version.py,sha256=BxBs80aIwaz2UIXDBGX93tZQuju6kfN8fRVjwIeNlhc,177
-ovos_translate_server-0.0.2a8.dist-info/LICENSE.md,sha256=diMg1nN8U1k1xwt21iM4oy1f-blxps2DUYh1zTOdpdI,11347
-ovos_translate_server-0.0.2a8.dist-info/METADATA,sha256=E-c8yhU8LjNwrocPQqOfP_nahMvoJnPmRj9Xg7t1kZY,980
-ovos_translate_server-0.0.2a8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ovos_translate_server-0.0.2a8.dist-info/entry_points.txt,sha256=SGE6jU6f01akw534GcpvBtCf5XZAtO0MNrT_3i09Q84,79
-ovos_translate_server-0.0.2a8.dist-info/top_level.txt,sha256=FxZjEsa5QA2U254ImugnyDpWC0Fu-iKQDignmZN_n1c,22
-ovos_translate_server-0.0.2a8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_translate_server-0.0.2a8.dist-info/RECORD,,
+ovos_translate_server/version.py,sha256=JbiDiI7BFf4c5rAPl_HfEUiHmGSt-ZALNV986MrjQk4,177
+ovos_translate_server-0.0.2a9.dist-info/LICENSE.md,sha256=diMg1nN8U1k1xwt21iM4oy1f-blxps2DUYh1zTOdpdI,11347
+ovos_translate_server-0.0.2a9.dist-info/METADATA,sha256=bu8pFRudKNTbpAsa-PcCEolZcQTfVWmFP3uoH-V60yg,930
+ovos_translate_server-0.0.2a9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_translate_server-0.0.2a9.dist-info/entry_points.txt,sha256=SGE6jU6f01akw534GcpvBtCf5XZAtO0MNrT_3i09Q84,79
+ovos_translate_server-0.0.2a9.dist-info/top_level.txt,sha256=FxZjEsa5QA2U254ImugnyDpWC0Fu-iKQDignmZN_n1c,22
+ovos_translate_server-0.0.2a9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_translate_server-0.0.2a9.dist-info/RECORD,,
```

