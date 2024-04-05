# Comparing `tmp/pyazo_cli-0.3.6-py3-none-any.whl.zip` & `tmp/pyazo_cli-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5443 bytes, number of entries: 7
+Zip file size: 5462 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pyazo_cli/__init__.py
--rw-r--r--  2.0 unx     6081 b- defN 80-Jan-01 00:00 pyazo_cli/pyazo.py
--rw-r--r--  2.0 unx     1475 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3257 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      549 b- defN 16-Jan-01 00:00 pyazo_cli-0.3.6.dist-info/RECORD
-7 files, 11496 bytes uncompressed, 4467 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx     6138 b- defN 80-Jan-01 00:00 pyazo_cli/pyazo.py
+-rw-r--r--  2.0 unx     1475 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3257 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 pyazo_cli-0.3.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      549 b- defN 16-Jan-01 00:00 pyazo_cli-0.3.7.dist-info/RECORD
+7 files, 11553 bytes uncompressed, 4486 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyazo_cli/__init__.py
 Comment: 
 
 Filename: pyazo_cli/pyazo.py
 Comment: 
 
-Filename: pyazo_cli-0.3.6.dist-info/LICENSE
+Filename: pyazo_cli-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: pyazo_cli-0.3.6.dist-info/METADATA
+Filename: pyazo_cli-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: pyazo_cli-0.3.6.dist-info/WHEEL
+Filename: pyazo_cli-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyazo_cli-0.3.6.dist-info/entry_points.txt
+Filename: pyazo_cli-0.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyazo_cli-0.3.6.dist-info/RECORD
+Filename: pyazo_cli-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyazo_cli/pyazo.py

```diff
@@ -31,14 +31,15 @@
 
 backends = {
     'Linux': {
         'maim': ['-s', '-n', '0', tmp_file],
         'scrot': ['-s', tmp_file],
         'import': [tmp_file],  # ImageMagick
         'grimshot': ['save', 'area', tmp_file],
+        'spectacle': ['-b', '-r', '-n', '-o', tmp_file],
     },
     'Darwin': {
         'screencapture': ['-i', tmp_file],
     },
     'Windows': {
         'snippingtool': ['/clip'],  # '/clip' requires at least Win10 1703
     }
```

## Comparing `pyazo_cli-0.3.6.dist-info/LICENSE` & `pyazo_cli-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyazo_cli-0.3.6.dist-info/METADATA` & `pyazo_cli-0.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyazo_cli
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: https://github.com/pyazo-screenshot/cli
 License: BSD-3-Clause
 Author: Jelena Dokic
 Author-email: jrubics@hacke.rs
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `pyazo_cli-0.3.6.dist-info/RECORD` & `pyazo_cli-0.3.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pyazo_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyazo_cli/pyazo.py,sha256=bPSGvs9WzHmnGOnBuTo1g0x27NGtdR0QrcdBN1SeFOI,6081
-pyazo_cli-0.3.6.dist-info/LICENSE,sha256=tkn4MFg2fqRhPBD6-Gi0LBAL05izDcKH6kYbEtfjA54,1475
-pyazo_cli-0.3.6.dist-info/METADATA,sha256=7MpN681dEhETZ5j5hWhwEw9cvvBf05j25N9BQHQf4bY,3257
-pyazo_cli-0.3.6.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-pyazo_cli-0.3.6.dist-info/entry_points.txt,sha256=pztX2tl9UKG7i01MR57y-ha250I_pjnFyb__sqHeSy0,46
-pyazo_cli-0.3.6.dist-info/RECORD,,
+pyazo_cli/pyazo.py,sha256=k0dBhHkU1TCRZwqIIbvwkumsLy9L5h6qTSGSX6qbGBI,6138
+pyazo_cli-0.3.7.dist-info/LICENSE,sha256=tkn4MFg2fqRhPBD6-Gi0LBAL05izDcKH6kYbEtfjA54,1475
+pyazo_cli-0.3.7.dist-info/METADATA,sha256=mFPW6zoev7s7qNizAhWCE_8qw6LqsGFML31DhZdkr1w,3257
+pyazo_cli-0.3.7.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+pyazo_cli-0.3.7.dist-info/entry_points.txt,sha256=pztX2tl9UKG7i01MR57y-ha250I_pjnFyb__sqHeSy0,46
+pyazo_cli-0.3.7.dist-info/RECORD,,
```

