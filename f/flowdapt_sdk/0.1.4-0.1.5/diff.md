# Comparing `tmp/flowdapt_sdk-0.1.4-py3-none-any.whl.zip` & `tmp/flowdapt_sdk-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21388 bytes, number of entries: 31
+Zip file size: 21397 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      227 b- defN 80-Jan-01 00:00 flowdapt_sdk/__init__.py
 -rw-r--r--  2.0 unx     1885 b- defN 80-Jan-01 00:00 flowdapt_sdk/_compat.py
 -rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/__init__.py
 -rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/base.py
 -rw-r--r--  2.0 unx     6298 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/configs.py
 -rw-r--r--  2.0 unx     2162 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/metrics.py
 -rw-r--r--  2.0 unx     4194 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/plugins.py
@@ -16,18 +16,18 @@
 -rw-r--r--  2.0 unx     2180 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/configs.py
 -rw-r--r--  2.0 unx      610 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1365 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/metrics.py
 -rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/plugin.py
 -rw-r--r--  2.0 unx      601 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/resource.py
 -rw-r--r--  2.0 unx     1493 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/system.py
 -rw-r--r--  2.0 unx     2336 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/triggers.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/workflows.py
+-rw-r--r--  2.0 unx     3152 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/workflows.py
 -rw-r--r--  2.0 unx     1249 b- defN 80-Jan-01 00:00 flowdapt_sdk/errors.py
 -rw-r--r--  2.0 unx     1842 b- defN 80-Jan-01 00:00 flowdapt_sdk/sdk.py
 -rw-r--r--  2.0 unx      172 b- defN 80-Jan-01 00:00 flowdapt_sdk/serialize.py
 -rw-r--r--  2.0 unx     2400 b- defN 80-Jan-01 00:00 flowdapt_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 flowdapt_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/RECORD
-31 files, 70650 bytes uncompressed, 17350 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.5.dist-info/RECORD
+31 files, 70714 bytes uncompressed, 17359 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: flowdapt_sdk/utils.py
 Comment: 
 
 Filename: flowdapt_sdk/version.py
 Comment: 
 
-Filename: flowdapt_sdk-0.1.4.dist-info/LICENSE
+Filename: flowdapt_sdk-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: flowdapt_sdk-0.1.4.dist-info/METADATA
+Filename: flowdapt_sdk-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: flowdapt_sdk-0.1.4.dist-info/WHEEL
+Filename: flowdapt_sdk-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: flowdapt_sdk-0.1.4.dist-info/RECORD
+Filename: flowdapt_sdk-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowdapt_sdk/dto/workflows.py

```diff
@@ -77,7 +77,8 @@
     uid: Annotated[UUID, Field(title='Uid')]
     name: Annotated[str, Field(title='Name')]
     workflow: Annotated[str, Field(title='Workflow')]
     started_at: Annotated[datetime, Field(title='Started At')]
     finished_at: Annotated[datetime | None, Field(title='Finished At')] = None
     result: Annotated[Any | None, Field(title='Result')] = None
     state: Annotated[str, Field(title='State')]
+    source: Annotated[str | None, Field(title='Source')] = None
```

## Comparing `flowdapt_sdk-0.1.4.dist-info/LICENSE` & `flowdapt_sdk-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flowdapt_sdk-0.1.4.dist-info/METADATA` & `flowdapt_sdk-0.1.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdapt_sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for Flowdapt
 Home-page: https://gitlab.com/emergentmethods/flowdapt-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `flowdapt_sdk-0.1.4.dist-info/RECORD` & `flowdapt_sdk-0.1.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 flowdapt_sdk/dto/configs.py,sha256=8zNXF14tOc_keQm8PZOwLdRsJBhqQ5eUSulQsRFlkZc,2180
 flowdapt_sdk/dto/error.py,sha256=FS3L_gu8CiKkuOxmxN-VIhV9r0aN6mps-1GSD0qXDO4,610
 flowdapt_sdk/dto/metrics.py,sha256=IeCosyosfaFHmBiCUe9LW5FjJZZWQDyBBpiIBDmVmms,1365
 flowdapt_sdk/dto/plugin.py,sha256=YP1I1nd7F1gQ-il-j4f987jsmxLx-82CQEr3APJX5vM,1030
 flowdapt_sdk/dto/resource.py,sha256=geCuTDSu-vNmh3JSs5iRMuRh6_voKqaUKvpoUnlzaPI,601
 flowdapt_sdk/dto/system.py,sha256=CqZMgpP_6ga_uwRCGouXhBySpAZWZQsIvmTXmDGc-uA,1493
 flowdapt_sdk/dto/triggers.py,sha256=nn8daHjEFLFJqhOfwtkdrhWR1RLWN8KVACt8uJ6YVQ4,2336
-flowdapt_sdk/dto/workflows.py,sha256=p2az4NptrlHqMjW9kbn3QNZVl_XLZaok-9A6M2rLa4w,3088
+flowdapt_sdk/dto/workflows.py,sha256=N4lkbyWv438fWKQy1fncU6e4l_cJkLNwxdzWAk6IPuE,3152
 flowdapt_sdk/errors.py,sha256=yTNgjfQNIZXBvt2MCBoGQSqdqud39pcnLgl6deFf6Dc,1249
 flowdapt_sdk/sdk.py,sha256=Adh-UwqykMIMZFiGc5xT5i8wPNMjRe8JHYdVcHpTbHo,1842
 flowdapt_sdk/serialize.py,sha256=KKc4AbAz_Bc9f_qzBcbJqU3HWnZidSK3-M-n7JHXEpo,172
 flowdapt_sdk/utils.py,sha256=7DMBCN63DoBK76auaTN_XUNprxrwd2NGUcNY0DGXpgk,2400
 flowdapt_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-flowdapt_sdk-0.1.4.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-flowdapt_sdk-0.1.4.dist-info/METADATA,sha256=Nm1UwzqL59K7nsE1A3YORACrc9HQyMrUB4DehBL5PvQ,2028
-flowdapt_sdk-0.1.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-flowdapt_sdk-0.1.4.dist-info/RECORD,,
+flowdapt_sdk-0.1.5.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+flowdapt_sdk-0.1.5.dist-info/METADATA,sha256=JkumhG7vcrCp2j8RUyR-Fr_k-d9ZDhXH74JXS58g2KU,2028
+flowdapt_sdk-0.1.5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+flowdapt_sdk-0.1.5.dist-info/RECORD,,
```

