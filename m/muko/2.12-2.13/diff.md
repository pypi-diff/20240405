# Comparing `tmp/muko-2.12-py3-none-any.whl.zip` & `tmp/muko-2.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1587684 bytes, number of entries: 7
+Zip file size: 1587683 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       20 b- defN 80-Jan-01 00:00 muko/__init__.py
 -rw-r--r--  2.0 fat   355840 b- defN 80-Jan-01 00:00 muko/cmuko.cp38-win_amd64.pyd
 -rw-r--r--  2.0 fat  2082964 b- defN 80-Jan-01 00:00 muko/font/default.otf
--rw-r--r--  2.0 fat     1074 b- defN 80-Jan-01 00:00 muko-2.12.dist-info/LICENSE
--rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 muko-2.12.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 muko-2.12.dist-info/WHEEL
-?rw-r--r--  2.0 fat      518 b- defN 16-Jan-01 00:00 muko-2.12.dist-info/RECORD
-7 files, 2441562 bytes uncompressed, 1586786 bytes compressed:  35.0%
+-rw-r--r--  2.0 fat     1074 b- defN 80-Jan-01 00:00 muko-2.13.dist-info/LICENSE
+-rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 muko-2.13.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 muko-2.13.dist-info/WHEEL
+?rw-r--r--  2.0 fat      518 b- defN 16-Jan-01 00:00 muko-2.13.dist-info/RECORD
+7 files, 2441562 bytes uncompressed, 1586785 bytes compressed:  35.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: muko/cmuko.cp38-win_amd64.pyd
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.12.dist-info/LICENSE
+Filename: muko-2.13.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.12.dist-info/METADATA
+Filename: muko-2.13.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.12.dist-info/WHEEL
+Filename: muko-2.13.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.12.dist-info/RECORD
+Filename: muko-2.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.12.dist-info/LICENSE` & `muko-2.13.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.12.dist-info/METADATA` & `muko-2.13.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.12
+Version: 2.13
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 License: MIT
 Author: Milk
 Author-email: 719496375@qq.com
 Requires-Python: ==3.8.*
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `muko-2.12.dist-info/RECORD` & `muko-2.13.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=I3iXnIfJYOJMurS2lNqY8lAIs_VHKbQ2L18rSV1KVy8,355840
+muko/cmuko.cp38-win_amd64.pyd,sha256=ImdDLoIkGLpJskexMx17rmY1oNF4hqAQzjaXicpefPM,355840
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.12.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.12.dist-info/METADATA,sha256=QLohGN833ZrbryYDrsdqmeKPJ6FIOipf7hrNI_NZQrQ,1058
-muko-2.12.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-muko-2.12.dist-info/RECORD,,
+muko-2.13.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.13.dist-info/METADATA,sha256=e8ooq3ZD4jtxkvoie1vnRuMmiaYCCv5mHZSaZEZmj7I,1058
+muko-2.13.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+muko-2.13.dist-info/RECORD,,
```

