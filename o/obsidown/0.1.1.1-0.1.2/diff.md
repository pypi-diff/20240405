# Comparing `tmp/obsidown-0.1.1.1-py3-none-any.whl.zip` & `tmp/obsidown-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 22204 bytes, number of entries: 16
+Zip file size: 22186 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 obsidown/__init__.py
 -rw-r--r--  2.0 unx      338 b- defN 80-Jan-01 00:00 obsidown/__main__.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 obsidown/config.py
 -rw-r--r--  2.0 unx     4929 b- defN 80-Jan-01 00:00 obsidown/main.py
 -rw-r--r--  2.0 unx     1202 b- defN 80-Jan-01 00:00 obsidown/operations/base.py
 -rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 obsidown/operations/dispatch.py
 -rw-r--r--  2.0 unx     1043 b- defN 80-Jan-01 00:00 obsidown/operations/link_convert.py
 -rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 obsidown/operations/math_convert.py
 -rw-r--r--  2.0 unx      601 b- defN 80-Jan-01 00:00 obsidown/operations/remove_after_string.py
 -rw-r--r--  2.0 unx     1197 b- defN 80-Jan-01 00:00 obsidown/operations/update_frontmatter.py
 -rw-r--r--  2.0 unx      692 b- defN 80-Jan-01 00:00 obsidown/operations/write_file.py
 -rw-r--r--  2.0 unx     4244 b- defN 80-Jan-01 00:00 obsidown/utils.py
--rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 obsidown-0.1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2119 b- defN 80-Jan-01 00:00 obsidown-0.1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 obsidown-0.1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1320 b- defN 16-Jan-01 00:00 obsidown-0.1.1.1.dist-info/RECORD
-16 files, 55307 bytes uncompressed, 20028 bytes compressed:  63.8%
+-rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 obsidown-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2117 b- defN 80-Jan-01 00:00 obsidown-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 obsidown-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1312 b- defN 16-Jan-01 00:00 obsidown-0.1.2.dist-info/RECORD
+16 files, 55297 bytes uncompressed, 20026 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: obsidown/operations/write_file.py
 Comment: 
 
 Filename: obsidown/utils.py
 Comment: 
 
-Filename: obsidown-0.1.1.1.dist-info/LICENSE
+Filename: obsidown-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: obsidown-0.1.1.1.dist-info/METADATA
+Filename: obsidown-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: obsidown-0.1.1.1.dist-info/WHEEL
+Filename: obsidown-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: obsidown-0.1.1.1.dist-info/RECORD
+Filename: obsidown-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `obsidown-0.1.1.1.dist-info/LICENSE` & `obsidown-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `obsidown-0.1.1.1.dist-info/METADATA` & `obsidown-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsidown
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: A quick way to convert obsidian markdown docs to markdown static pages
 License: GPLv3
 Author: Angelo 'Flecart' Huang
 Author-email: xuanqiang.huang@studio.unibo.it
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `obsidown-0.1.1.1.dist-info/RECORD` & `obsidown-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 obsidown/operations/dispatch.py,sha256=nTQaVFkiT23GZWO9hBkaE56sAsQx06E3SwxaRcrpRPI,1092
 obsidown/operations/link_convert.py,sha256=pYA37_vCZpprbUPgRPWhEZOhgz-fno3TFsZ5-Y6e2Is,1043
 obsidown/operations/math_convert.py,sha256=7FycqHTYk8jkKhrE_GiDYVgaaHuiTAA0oqMcu2zNEj0,560
 obsidown/operations/remove_after_string.py,sha256=UXqE7PC7KefWXyNRsr_9XkktesMm7YBmyoig6QCNCaY,601
 obsidown/operations/update_frontmatter.py,sha256=DYWVoDLaAkcyCn3N6BL4WkreNO6AAPgNjextT8TN4_8,1197
 obsidown/operations/write_file.py,sha256=B-ZQynmUaJsXQ6bBjLMpu5alWBj5GAbg1bqdcJPlimM,692
 obsidown/utils.py,sha256=GAiy1Qhi6Uu_n-qwXhEWwaPsvXhALyqNWakdchqkG70,4244
-obsidown-0.1.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-obsidown-0.1.1.1.dist-info/METADATA,sha256=YmBTgvPH3ZA0-7Sk0DCzkcAYebUqnoSMZiF49_6KJ0I,2119
-obsidown-0.1.1.1.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-obsidown-0.1.1.1.dist-info/RECORD,,
+obsidown-0.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+obsidown-0.1.2.dist-info/METADATA,sha256=mD6ivI7O1GKJfjU5gafsgwN-Jv7T0Bjm-oTD3UfrxQI,2117
+obsidown-0.1.2.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+obsidown-0.1.2.dist-info/RECORD,,
```

