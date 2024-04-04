# Comparing `tmp/flowdapt-0.1.7-py3-none-any.whl.zip` & `tmp/flowdapt-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 181685 bytes, number of entries: 175
+Zip file size: 181687 bytes, number of entries: 175
 -rw-r--r--  2.0 unx      130 b- defN 80-Jan-01 00:00 flowdapt/__init__.py
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 flowdapt/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 flowdapt/builtins/__init__.py
 -rw-r--r--  2.0 unx     9361 b- defN 80-Jan-01 00:00 flowdapt/builtins/utils.py
 -rw-r--r--  2.0 unx      385 b- defN 80-Jan-01 00:00 flowdapt/cli/__init__.py
 -rw-r--r--  2.0 unx      749 b- defN 80-Jan-01 00:00 flowdapt/cli/_internal.py
 -rw-r--r--  2.0 unx     2597 b- defN 80-Jan-01 00:00 flowdapt/cli/config.py
@@ -165,13 +165,13 @@
 -rw-r--r--  2.0 unx      833 b- defN 80-Jan-01 00:00 flowdapt/triggers/resources/triggers/actions.py
 -rw-r--r--  2.0 unx     2160 b- defN 80-Jan-01 00:00 flowdapt/triggers/resources/triggers/conditions.py
 -rw-r--r--  2.0 unx     1583 b- defN 80-Jan-01 00:00 flowdapt/triggers/resources/triggers/cron.py
 -rw-r--r--  2.0 unx     5790 b- defN 80-Jan-01 00:00 flowdapt/triggers/resources/triggers/methods.py
 -rw-r--r--  2.0 unx      135 b- defN 80-Jan-01 00:00 flowdapt/triggers/rpc/__init__.py
 -rw-r--r--  2.0 unx     6850 b- defN 80-Jan-01 00:00 flowdapt/triggers/rpc/triggers.py
 -rw-r--r--  2.0 unx     1843 b- defN 80-Jan-01 00:00 flowdapt/triggers/service.py
--rw-r--r--  2.0 unx    11346 b- defN 80-Jan-01 00:00 flowdapt-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    10504 b- defN 80-Jan-01 00:00 flowdapt-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 flowdapt-0.1.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    16070 b- defN 16-Jan-01 00:00 flowdapt-0.1.7.dist-info/RECORD
-175 files, 553255 bytes uncompressed, 155819 bytes compressed:  71.8%
+-rw-r--r--  2.0 unx    11346 b- defN 80-Jan-01 00:00 flowdapt-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10504 b- defN 80-Jan-01 00:00 flowdapt-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 flowdapt-0.1.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    16070 b- defN 16-Jan-01 00:00 flowdapt-0.1.8.dist-info/RECORD
+175 files, 553255 bytes uncompressed, 155821 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -504,23 +504,23 @@
 
 Filename: flowdapt/triggers/rpc/triggers.py
 Comment: 
 
 Filename: flowdapt/triggers/service.py
 Comment: 
 
-Filename: flowdapt-0.1.7.dist-info/LICENSE
+Filename: flowdapt-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: flowdapt-0.1.7.dist-info/METADATA
+Filename: flowdapt-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: flowdapt-0.1.7.dist-info/WHEEL
+Filename: flowdapt-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: flowdapt-0.1.7.dist-info/entry_points.txt
+Filename: flowdapt-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowdapt-0.1.7.dist-info/RECORD
+Filename: flowdapt-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `flowdapt-0.1.7.dist-info/LICENSE` & `flowdapt-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flowdapt-0.1.7.dist-info/METADATA` & `flowdapt-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdapt
-Version: 0.1.7
+Version: 0.1.8
 Summary: A generalized framework for robust modular deployments of large-scale, real-time adaptive modeling on chaotic data.
 License: Apache-2.0
 Author: Emergent Methods, LLC
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Requires-Dist: opentelemetry-api (==1.18.0)
 Requires-Dist: opentelemetry-exporter-otlp (==1.18.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
 Requires-Dist: opentelemetry-instrumentation-asgi (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-instrumentation-system-metrics (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-sdk (==1.18.0)
-Requires-Dist: orjson (==3.9.10)
+Requires-Dist: orjson (==3.9.14)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pympler (>=1.0.1,<2.0.0)
 Requires-Dist: pynvml (>=11.5.0,<12.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-manifest (>=2.2.3,<3.0.0)
```

## Comparing `flowdapt-0.1.7.dist-info/RECORD` & `flowdapt-0.1.8.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -164,12 +164,12 @@
 flowdapt/triggers/resources/triggers/actions.py,sha256=11ZckVuVcp3kROmW0zqj0CVIMs-CMUaBaDKW0Fkva4Q,833
 flowdapt/triggers/resources/triggers/conditions.py,sha256=RWD-JlgmuSQ-arkqUYhkb5B3ge7VZESZ0iDwYcqIkLU,2160
 flowdapt/triggers/resources/triggers/cron.py,sha256=QT54dbTYSRuM22nvzd0yG4DyFSRwxJedh6cc4NRSiIo,1583
 flowdapt/triggers/resources/triggers/methods.py,sha256=TQwHF_1RF3a4DqogiU2VxyL9uVeCLwCPH141E4o4bS0,5790
 flowdapt/triggers/rpc/__init__.py,sha256=kS3sNq4PvAPN9Zri1gYbz4K3AOjbuDeszzSrXIb5aCk,135
 flowdapt/triggers/rpc/triggers.py,sha256=LeibgZ3H15ZJis1O_SfX29GYASlgW2Xx9crTn-3nb0c,6850
 flowdapt/triggers/service.py,sha256=ct1UmHSsD517A9_UYeYO6ryA6K24zazH45KnYFnSYRM,1843
-flowdapt-0.1.7.dist-info/LICENSE,sha256=BY49ytuIAu1ENssv_H-487qf-QI0MHjArhTL7dWZIic,11346
-flowdapt-0.1.7.dist-info/METADATA,sha256=q_mVSq5cEkgZiAOOTlxu-r3AMa4Ntr-8zM4KzaMerZI,10504
-flowdapt-0.1.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-flowdapt-0.1.7.dist-info/entry_points.txt,sha256=EEbmpD6pqMjObmJZmQjPUlz08reB0QohNSMCGaNIPcQ,45
-flowdapt-0.1.7.dist-info/RECORD,,
+flowdapt-0.1.8.dist-info/LICENSE,sha256=BY49ytuIAu1ENssv_H-487qf-QI0MHjArhTL7dWZIic,11346
+flowdapt-0.1.8.dist-info/METADATA,sha256=OQv_x85WzMIfXDogWZDHnfwn4Ui1ppOO-hCXJzJaQIs,10504
+flowdapt-0.1.8.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+flowdapt-0.1.8.dist-info/entry_points.txt,sha256=EEbmpD6pqMjObmJZmQjPUlz08reB0QohNSMCGaNIPcQ,45
+flowdapt-0.1.8.dist-info/RECORD,,
```

