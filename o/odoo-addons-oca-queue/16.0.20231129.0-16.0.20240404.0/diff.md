# Comparing `tmp/odoo_addons_oca_queue-16.0.20231129.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_queue-16.0.20240404.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1372 bytes, number of entries: 4
--rw-r--r--  2.0 unx      861 b- defN 24-Jan-20 05:56 odoo_addons_oca_queue-16.0.20231129.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-20 05:56 odoo_addons_oca_queue-16.0.20231129.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Jan-20 05:56 odoo_addons_oca_queue-16.0.20231129.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      392 b- defN 24-Jan-20 05:56 odoo_addons_oca_queue-16.0.20231129.0.dist-info/RECORD
-4 files, 1346 bytes uncompressed, 598 bytes compressed:  55.6%
+Zip file size: 1378 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      927 b- defN 24-Apr-05 06:05 odoo_addons_oca_queue-16.0.20240404.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 06:05 odoo_addons_oca_queue-16.0.20240404.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-05 06:05 odoo_addons_oca_queue-16.0.20240404.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      392 b- defN 24-Apr-05 06:05 odoo_addons_oca_queue-16.0.20240404.0.dist-info/RECORD
+4 files, 1412 bytes uncompressed, 604 bytes compressed:  57.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_queue-16.0.20231129.0.dist-info/METADATA
+Filename: odoo_addons_oca_queue-16.0.20240404.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_queue-16.0.20231129.0.dist-info/WHEEL
+Filename: odoo_addons_oca_queue-16.0.20240404.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_queue-16.0.20231129.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_queue-16.0.20240404.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_queue-16.0.20231129.0.dist-info/RECORD
+Filename: odoo_addons_oca_queue-16.0.20240404.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_queue-16.0.20231129.0.dist-info/METADATA` & `odoo_addons_oca_queue-16.0.20240404.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-queue
-Version: 16.0.20231129.0
+Version: 16.0.20240404.0
 Summary: Meta package for oca-queue Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-base-export-async <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-import-async <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-queue-job <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-queue-job-batch <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-queue-job-cron <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-queue-job-cron-jobrunner <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-queue-job-subscribe <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-queue-job-web-notify <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-test-queue-job <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-test-queue-job-batch <16.1dev,>=16.0dev
 
 UNKNOWN
```

