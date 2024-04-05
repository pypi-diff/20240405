# Comparing `tmp/spark_batch-2.5-py3-none-any.whl.zip` & `tmp/spark_batch-2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,36 +1,48 @@
-Zip file size: 187160 bytes, number of entries: 34
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 05:55 spark_batch/__init__.py
--rw-r--r--  2.0 unx     5508 b- defN 23-Nov-11 19:01 spark_batch/run.py
--rwxr-xr-x  2.0 unx     2562 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.dbf
--rwxr-xr-x  2.0 unx      422 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.prj
--rwxr-xr-x  2.0 unx      348 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.sbn
--rwxr-xr-x  2.0 unx      132 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.sbx
--rwxr-xr-x  2.0 unx   151044 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.shp
--rwxr-xr-x  2.0 unx     1055 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.shp.xml
--rwxr-xr-x  2.0 unx      292 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_BADM_AS.shx
--rwxr-xr-x  2.0 unx     1494 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.dbf
--rwxr-xr-x  2.0 unx      422 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.prj
--rwxr-xr-x  2.0 unx      236 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.sbn
--rwxr-xr-x  2.0 unx      132 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.sbx
--rwxr-xr-x  2.0 unx    91780 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.shp
--rwxr-xr-x  2.0 unx     8332 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.shp.xml
--rwxr-xr-x  2.0 unx      180 b- defN 23-Nov-21 23:58 spark_batch/data/shp/BML_HADM_AS.shx
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-11 19:01 spark_batch/lib/__init__.py
--rw-r--r--  2.0 unx     7885 b- defN 23-Dec-11 08:09 spark_batch/lib/csv_table_manager.py
--rw-r--r--  2.0 unx    16092 b- defN 23-Dec-19 01:11 spark_batch/lib/delta_table_manager.py
--rw-r--r--  2.0 unx    21988 b- defN 24-Feb-07 04:47 spark_batch/lib/elt_manager.py
--rw-r--r--  2.0 unx     5513 b- defN 24-Feb-07 05:08 spark_batch/lib/json_table_manager.py
--rw-r--r--  2.0 unx     5256 b- defN 23-Dec-15 10:22 spark_batch/lib/mariadb_table_manager.py
--rw-r--r--  2.0 unx     5525 b- defN 23-Dec-06 13:41 spark_batch/lib/oracle_table_manager.py
--rw-r--r--  2.0 unx    10391 b- defN 24-Jan-25 08:24 spark_batch/lib/postgresql_table_manager.py
--rw-r--r--  2.0 unx     2482 b- defN 24-Feb-07 05:52 spark_batch/lib/pxlogger.py
--rw-r--r--  2.0 unx     5219 b- defN 24-Jan-15 00:51 spark_batch/lib/resource_manager.py
--rw-r--r--  2.0 unx     2324 b- defN 23-Nov-12 19:08 spark_batch/lib/spark_session.py
--rw-r--r--  2.0 unx     1860 b- defN 23-Nov-21 18:30 spark_batch/lib/udf_aes_cipher.py
--rw-r--r--  2.0 unx     5709 b- defN 24-Feb-02 06:37 spark_batch/lib/udf_geo_converter.py
--rw-r--r--  2.0 unx     4335 b- defN 24-Jan-29 01:09 spark_batch/lib/util.py
--rw-r--r--  2.0 unx      388 b- defN 24-Feb-07 05:55 spark_batch-2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 05:55 spark_batch-2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Feb-07 05:55 spark_batch-2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3036 b- defN 24-Feb-07 05:55 spark_batch-2.5.dist-info/RECORD
-34 files, 362046 bytes uncompressed, 182224 bytes compressed:  49.7%
+Zip file size: 402328 bytes, number of entries: 46
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-25 06:07 spark_batch/__init__.py
+-rw-r--r--  2.0 unx     5508 b- defN 24-Feb-07 09:17 spark_batch/run.py
+-rwxr-xr-x  2.0 unx     2562 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.dbf
+-rwxr-xr-x  2.0 unx      422 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.prj
+-rwxr-xr-x  2.0 unx      348 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.sbn
+-rwxr-xr-x  2.0 unx      132 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.sbx
+-rwxr-xr-x  2.0 unx   151044 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.shp
+-rwxr-xr-x  2.0 unx     1055 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.shp.xml
+-rwxr-xr-x  2.0 unx      292 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_BADM_AS.shx
+-rwxr-xr-x  2.0 unx     1494 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.dbf
+-rwxr-xr-x  2.0 unx      422 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.prj
+-rwxr-xr-x  2.0 unx      236 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.sbn
+-rwxr-xr-x  2.0 unx      132 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.sbx
+-rwxr-xr-x  2.0 unx    91780 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.shp
+-rwxr-xr-x  2.0 unx     8332 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.shp.xml
+-rwxr-xr-x  2.0 unx      180 b- defN 24-Feb-07 09:17 spark_batch/data/shp/BML_HADM_AS.shx
+-rwxr-xr-x  2.0 unx     2562 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.dbf
+-rwxr-xr-x  2.0 unx      422 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.prj
+-rwxr-xr-x  2.0 unx      348 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.sbn
+-rwxr-xr-x  2.0 unx      132 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.sbx
+-rwxr-xr-x  2.0 unx   153964 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.shp
+-rwxr-xr-x  2.0 unx      292 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_BADM_AS.shx
+-rwxr-xr-x  2.0 unx     4170 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.dbf
+-rwxr-xr-x  2.0 unx      516 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.sbn
+-rwxr-xr-x  2.0 unx      164 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.sbx
+-rwxr-xr-x  2.0 unx   136876 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.shp
+-rwxr-xr-x  2.0 unx     7908 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.shp.xml
+-rwxr-xr-x  2.0 unx      396 b- defN 24-Feb-07 09:17 spark_batch/data/shp2024/BML_HADM_AS.shx
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 09:17 spark_batch/lib/__init__.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Feb-07 09:17 spark_batch/lib/csv_table_manager.py
+-rw-r--r--  2.0 unx    16092 b- defN 24-Feb-07 09:17 spark_batch/lib/delta_table_manager.py
+-rw-r--r--  2.0 unx    22383 b- defN 24-Mar-25 04:10 spark_batch/lib/elt_manager.py
+-rw-r--r--  2.0 unx     5521 b- defN 24-Mar-25 05:58 spark_batch/lib/json_table_manager.py
+-rw-r--r--  2.0 unx     5256 b- defN 24-Feb-07 09:17 spark_batch/lib/mariadb_table_manager.py
+-rw-r--r--  2.0 unx     5525 b- defN 24-Feb-07 09:17 spark_batch/lib/oracle_table_manager.py
+-rw-r--r--  2.0 unx    10391 b- defN 24-Feb-07 09:17 spark_batch/lib/postgresql_table_manager.py
+-rw-r--r--  2.0 unx     2483 b- defN 24-Feb-07 09:17 spark_batch/lib/pxlogger.py
+-rw-r--r--  2.0 unx     5269 b- defN 24-Feb-07 09:17 spark_batch/lib/resource_manager.py
+-rw-r--r--  2.0 unx     2324 b- defN 24-Feb-07 09:17 spark_batch/lib/spark_session.py
+-rw-r--r--  2.0 unx     1860 b- defN 24-Feb-07 09:17 spark_batch/lib/udf_aes_cipher.py
+-rw-r--r--  2.0 unx     5709 b- defN 24-Feb-07 09:17 spark_batch/lib/udf_geo_converter.py
+-rw-r--r--  2.0 unx     4335 b- defN 24-Feb-07 09:17 spark_batch/lib/util.py
+-rw-r--r--  2.0 unx      388 b- defN 24-Mar-25 06:07 spark_batch-2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-25 06:07 spark_batch-2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Mar-25 06:07 spark_batch-2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4201 b- defN 24-Mar-25 06:07 spark_batch-2.6.dist-info/RECORD
+46 files, 671415 bytes uncompressed, 395512 bytes compressed:  41.1%
```

## zipnote {}

```diff
@@ -42,14 +42,50 @@
 
 Filename: spark_batch/data/shp/BML_HADM_AS.shp.xml
 Comment: 
 
 Filename: spark_batch/data/shp/BML_HADM_AS.shx
 Comment: 
 
+Filename: spark_batch/data/shp2024/BML_BADM_AS.dbf
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_BADM_AS.prj
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_BADM_AS.sbn
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_BADM_AS.sbx
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_BADM_AS.shp
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_BADM_AS.shx
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.dbf
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.sbn
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.sbx
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.shp
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.shp.xml
+Comment: 
+
+Filename: spark_batch/data/shp2024/BML_HADM_AS.shx
+Comment: 
+
 Filename: spark_batch/lib/__init__.py
 Comment: 
 
 Filename: spark_batch/lib/csv_table_manager.py
 Comment: 
 
 Filename: spark_batch/lib/delta_table_manager.py
@@ -84,20 +120,20 @@
 
 Filename: spark_batch/lib/udf_geo_converter.py
 Comment: 
 
 Filename: spark_batch/lib/util.py
 Comment: 
 
-Filename: spark_batch-2.5.dist-info/METADATA
+Filename: spark_batch-2.6.dist-info/METADATA
 Comment: 
 
-Filename: spark_batch-2.5.dist-info/WHEEL
+Filename: spark_batch-2.6.dist-info/WHEEL
 Comment: 
 
-Filename: spark_batch-2.5.dist-info/top_level.txt
+Filename: spark_batch-2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_batch-2.5.dist-info/RECORD
+Filename: spark_batch-2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_batch/lib/elt_manager.py

```diff
@@ -12,14 +12,17 @@
 from datetime import datetime
 import time
 import math
 
 
 class EltManager:
 
+    # useage:
+    #   em = EltManager(spark, config_file="/conf/config.yaml", domain="bcdb", record_type="mart")
+    #   em = EltManager(spark, config_file="/conf/config.yaml", domain="bcdb", record_type="mart", record_prefix="opt")
     def __init__(self, spark, config_file="config.yaml", domain="",
             record_type=None, record_topic=None, record_dpath=None,
             skip_ingest_for_sucess_record=False, record_table="elt_manager_log", record_prefix=None): 
 
         self.spark = spark
         self.logger = CustomLogger("EltManager")
         #self.odm = OrderManager(spark)
@@ -283,15 +286,15 @@
     Returns:
     - source_df (DataFrame): The DataFrame representing the source data after incremental ingestion.
     - target_df (DataFrame): The DataFrame representing the target data after merging.
     - valid (bool): A boolean indicating the success of the incremental ingestion process. True if successful, False otherwise.
     """
     def ingest_increment(self, source_objects, target_object, source_inc_query, target_condition,  
             source_df=None, source_customSchema=None, target_customSchema=None, cleansing_conditions=None, rebase_datetime=False,
-            delemeter=None, charset=None, header=True) :    
+            delemeter=None, charset=None, header=True, source_df_cache=False) :    
 
         sourceInfo = self._getSourceInfo(source_objects)
         targetInfo = self._getTargetInfo(target_object)
         
         timer = Timer()
         self.logger.info(f"ETL/IC Started : [ {targetInfo} ({source_objects}) ]")
 
@@ -305,14 +308,17 @@
                 else:
                     source_df = self.source_tm.queryTable(source_inc_query, tableNames=source_objects, customSchemas=source_customSchema)
 
             # 데이터가 없으면 종료
             if source_df is None :
                 raise RuntimeError(f"Source not found: {sourceInfo} / {targetInfo}")
 
+            if source_df_cache :
+                source_df.cache()
+
             #source_df.cache()
 
             if target_customSchema:
                 for column_name, data_type in target_customSchema.items():
                     source_df = source_df.withColumn(column_name, source_df[column_name].cast(data_type))
 
             cleaned_source_df = source_df
@@ -346,14 +352,16 @@
             self.logger.error(f"ETL/IC Error : {e1}")
             self.logger.error(f"ETL/IC Done : [ {targetInfo} / False (-1, -1, -1) / {timer.elapsed():,.2f} ]")
             self._record(self.record_inc_header, source_objects, target_object, False, -1, -1, -1, str(e1)[:255], timer.elapsed())
             return (None, None, False)
         finally:
             if rebase_datetime:
                 self.spark.conf.set("spark.sql.parquet.int96RebaseModeInWrite", "CORRECTED")
+            if source_df_cache :
+                source_df.unpersist()
         
     # condition1 = ~col("aaa").like("%.%")
     # cleansing_condition = F.col("vehno").isNotNull()  # Null 아닌것만 저장
     # condition2 = col("bbb") != "xyz"
     def cleansing(self, target_df,  cleansing_conditions=None):
         if cleansing_conditions is None:
             return (0, target_df)
```

## spark_batch/lib/json_table_manager.py

```diff
@@ -121,17 +121,18 @@
             
         return tableName if dpath is None else f'{dpath}/{tableName}'
     
     def _getArchivePath(self, tableName, dpath=None) :
         # 아카이브 경로 초기화
         archive_path = ""
 
-        # dpath가 있으면 추가
-        if dpath:
-            archive_path += dpath + "/"
+        if dpath is None:
+            dpath = self.archive_dpath
+
+        archive_path += dpath + "/"
 
         # 현재 날짜 폴더 추가
         current_date = datetime.now().strftime("%Y%m%d")
         archive_path += current_date + "/"
 
         # tableName 추가
         archive_path += tableName
```

## spark_batch/lib/pxlogger.py

```diff
@@ -1,8 +1,8 @@
-from spark_common.abstract_logger import AbstractLogger
+#from spark_common.abstract_logger import AbstractLogger
 import logging
 import sys
 
 
 # Using the same class name to achieve consistency
 #class CustomLogger(AbstractLogger):
 #    pass
```

## spark_batch/lib/resource_manager.py

```diff
@@ -1,12 +1,13 @@
 # 소스 대상 초기화 
 from .oracle_table_manager import OracleTableManager
 from .mariadb_table_manager import MariadbTableManager
 from .delta_table_manager import DeltaTableManager
 from .csv_table_manager import CSVTableManager
+from .json_table_manager import JSONTableManager
 from .postgresql_table_manager import PostgreSQLTableManager
 from .pxlogger import CustomLogger
 
 import yaml
 
 class ResourceManager:
     def __init__(self, spark, config_file="config.yaml"):
@@ -39,15 +40,15 @@
                 s3_endpoint = source_config.get("s3_endpoint")
                 s3_access_key = source_config.get("s3_access_key")
                 s3_secret_key = source_config.get("s3_secret_key")
                 s3_ssl_verify = source_config.get("s3_ssl_verify", True)
                 archive_bucket = source_config.get("archive_bucket")
                 archive_dpath = source_config.get("archive_dpath")
                 dpath = kwargs.get("dpath", None)
-                return self._get_CSVTableManager(s3_endpoint, s3_access_key, s3_secret_key, s3_ssl_verify, archive_bucket, archive_dpath, topic, dpath) if source_type_name == "csv" else elf._get_JSONTableManager(s3_endpoint, s3_access_key, s3_secret_key, s3_ssl_verify, archive_bucket, archive_dpath, topic, dpath)
+                return self._get_CSVTableManager(s3_endpoint, s3_access_key, s3_secret_key, s3_ssl_verify, archive_bucket, archive_dpath, topic, dpath) if source_type_name == "csv" else self._get_JSONTableManager(s3_endpoint, s3_access_key, s3_secret_key, s3_ssl_verify, archive_bucket, archive_dpath, topic, dpath)
             elif source_type_name == "delta":
                 dpath = kwargs.get("dpath", None)
                 
                 self.logger.debug(("source_type_name = delata  :", topic, dpath))
                 return self._get_DeltaTableManager(topic, dpath)
             else:
                 raise ValueError("Unsupported source type: " + source_type)
```

## Comparing `spark_batch-2.5.dist-info/RECORD` & `spark_batch-2.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -10,25 +10,37 @@
 spark_batch/data/shp/BML_HADM_AS.dbf,sha256=pmo3I3ca5QxdGbuzWVUM2UEk3rNxk_TF_0kx2_9b0U0,1494
 spark_batch/data/shp/BML_HADM_AS.prj,sha256=3PpCz9OSQX2VSutQONEv2qMqMIebP11hHyB8cRXcnn4,422
 spark_batch/data/shp/BML_HADM_AS.sbn,sha256=18sLENFp8JAcybvOu6DsoWnL9NqsEWeTS7HTJFCr6k4,236
 spark_batch/data/shp/BML_HADM_AS.sbx,sha256=UTaUASh79uQ-EFCzT3s9nldjsUJSA8IQUe3D9PUE1kY,132
 spark_batch/data/shp/BML_HADM_AS.shp,sha256=kTJNZMdNRWI-xYSwbPVw9C_SA5lXO8sg3v8MVQmmKww,91780
 spark_batch/data/shp/BML_HADM_AS.shp.xml,sha256=h11hJLDtHTnSNIh4QiizIv7Vln3r72koSWuXv5QoEIs,8332
 spark_batch/data/shp/BML_HADM_AS.shx,sha256=CTdhu3XEdecwsHwnOdMQm9aM7l0uZYJIWaoIf5FH7uI,180
+spark_batch/data/shp2024/BML_BADM_AS.dbf,sha256=WbcEfMNr4iUHSSiOJ4iErZA_5dDFBF0PgiUUt6G39D8,2562
+spark_batch/data/shp2024/BML_BADM_AS.prj,sha256=3PpCz9OSQX2VSutQONEv2qMqMIebP11hHyB8cRXcnn4,422
+spark_batch/data/shp2024/BML_BADM_AS.sbn,sha256=6rCG77HsyFg_coczPMO-pWkrVk-DpZ_5mlLvpAHY2ik,348
+spark_batch/data/shp2024/BML_BADM_AS.sbx,sha256=Y0__cD87_CwBBAWofpgr0Q_0h-0TPYSP1hGsyFNbJK8,132
+spark_batch/data/shp2024/BML_BADM_AS.shp,sha256=DyhxExOUt3KRmsSD8AP-z9xVdMpPLGc0i48M7dXmJPI,153964
+spark_batch/data/shp2024/BML_BADM_AS.shx,sha256=RksOnkLs5sd3rqRaLZw0siYBFMBaJrRQkb-h9cGXnyw,292
+spark_batch/data/shp2024/BML_HADM_AS.dbf,sha256=axtEtnuA6e6OZMyw3gwawBQ3H_uTs9lYKeWJk6I752U,4170
+spark_batch/data/shp2024/BML_HADM_AS.sbn,sha256=x08C2Me5oA0JbqmE4bB-_D3Nstf_hBI2E_Wzh_Ryjho,516
+spark_batch/data/shp2024/BML_HADM_AS.sbx,sha256=qrnx1EymDl520IpEXjZJFpZEi470za-ezuHjvxoXXGo,164
+spark_batch/data/shp2024/BML_HADM_AS.shp,sha256=BmwmyOaT2W7XOCUbPwu0EGTcUIFLhuvkpMCLOImFGT0,136876
+spark_batch/data/shp2024/BML_HADM_AS.shp.xml,sha256=6Ef72zmvTgi2WI4CnsCYPBOIQcAjCNQ6egppFVxDHuA,7908
+spark_batch/data/shp2024/BML_HADM_AS.shx,sha256=XV3jn51r5xjUuOcC7NPDu4G6J_PqPaARso57dvzsiBg,396
 spark_batch/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_batch/lib/csv_table_manager.py,sha256=Wy-X0fgEeBTE5u66wT8qCZWNgFrjYfhv0WEN0TKly3g,7885
 spark_batch/lib/delta_table_manager.py,sha256=ZMmxhCOsspmONsu8cDHW4xD3nRBKDEiQPiSlSjngKxo,16092
-spark_batch/lib/elt_manager.py,sha256=hWZXdRqiYwyJNddpqvUX0YOJgsEpx4BYyM5P3SeWXOY,21988
-spark_batch/lib/json_table_manager.py,sha256=Y85GHLxoaeSOz-naQnjJhhPuCjrY-WCzxZlcdtZcQyM,5513
+spark_batch/lib/elt_manager.py,sha256=BTnoFy24k0kU5q6ihDLnbs2v-FQ6635SEM9x1gzkHxs,22383
+spark_batch/lib/json_table_manager.py,sha256=LMEXTToowrr5pJfdB3EkKhV_axQ-URNj_8cVOIoXdU0,5521
 spark_batch/lib/mariadb_table_manager.py,sha256=xTXi8yRKxlCv_i6gD-uvdF4b70rSbU1K6vigwpMgxwY,5256
 spark_batch/lib/oracle_table_manager.py,sha256=KbL8W1oqrGii1WrvF9qMUfUxvnvMArkL1mdDK8DgWQc,5525
 spark_batch/lib/postgresql_table_manager.py,sha256=3XlxvXT95sUmttO_Aiq4B7Q9XMWY0PnMKBubQKnf9Do,10391
-spark_batch/lib/pxlogger.py,sha256=81dC0weKxAGKgE-LawrNYCxayTeLX1K2YaXavS6Ov78,2482
-spark_batch/lib/resource_manager.py,sha256=w9MG-ghfMSweVyEwNDzPl2Set5v15Gkvh8bdyb158HI,5219
+spark_batch/lib/pxlogger.py,sha256=wlu-0LfxaayGW1y2Wy5i6cDBh4GX-IaV--1ajtvLOJ4,2483
+spark_batch/lib/resource_manager.py,sha256=AtvGna8yawgNaLCgM_r_PKbdDD-kswJKgkVv4W6DqWc,5269
 spark_batch/lib/spark_session.py,sha256=Gv1xnnGFMERxnKNuWfX9frmcZh5sNx4AWk9rRgkHg7U,2324
 spark_batch/lib/udf_aes_cipher.py,sha256=_Ua9wlX7WDrAEZWfK11EUwCa3HExApzj9tXM3rMuHAs,1860
 spark_batch/lib/udf_geo_converter.py,sha256=NIZFgvZuvPDRaqwNDoFK4FrykgK9hbnRuxY6D6XjZ_k,5709
 spark_batch/lib/util.py,sha256=gI4r7OCcFQ35KpTLIHFVw36e5d-Absc6ufA3pHXddI8,4335
-spark_batch-2.5.dist-info/METADATA,sha256=GMF_wq1PylrGd06Sa_i2IrZ3U3MCT4vAmmNPJtrf-Tc,388
-spark_batch-2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-spark_batch-2.5.dist-info/top_level.txt,sha256=4CXvktYZ-h_dAJ9jETz_09zaMrW0RBzckuDwWC4BGqM,12
-spark_batch-2.5.dist-info/RECORD,,
+spark_batch-2.6.dist-info/METADATA,sha256=g6sW7Qy3PYFfZKCxajwHhjNHZMgWHi7eaXZPiDCv4N0,388
+spark_batch-2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+spark_batch-2.6.dist-info/top_level.txt,sha256=4CXvktYZ-h_dAJ9jETz_09zaMrW0RBzckuDwWC4BGqM,12
+spark_batch-2.6.dist-info/RECORD,,
```

