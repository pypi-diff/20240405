# Comparing `tmp/xnattagger-0.6.7-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.6.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6852 bytes, number of entries: 10
+Zip file size: 6816 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    16622 b- defN 24-Apr-04 19:05 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 24-Apr-04 19:06 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      220 b- defN 24-Apr-04 19:41 xnattagger/__version__.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
 -rw-r--r--  2.0 unx     1448 b- defN 23-Aug-25 17:45 xnattagger/config/tagger.yaml
--rwxr-xr-x  2.0 unx     2297 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      834 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/RECORD
-10 files, 23553 bytes uncompressed, 5424 bytes compressed:  77.0%
+-rwxr-xr-x  2.0 unx     2253 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      834 b- defN 24-Apr-04 19:43 xnattagger-0.6.8.dist-info/RECORD
+10 files, 23509 bytes uncompressed, 5388 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.6.7.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.6.8.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.6.7.dist-info/LICENSE
+Filename: xnattagger-0.6.8.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.6.7.dist-info/METADATA
+Filename: xnattagger-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.6.7.dist-info/WHEEL
+Filename: xnattagger-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.6.7.dist-info/top_level.txt
+Filename: xnattagger-0.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.6.7.dist-info/RECORD
+Filename: xnattagger-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.6.7.data/scripts/xnat_tagger.py` & `xnattagger-0.6.8.data/scripts/xnat_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--config', required=True,
         help='Filters configuration file') 
-    parser.add_argument('--target-modality', choices=['t1', 't2', 'dwi', 'bold', 'all'], nargs='+', required=True, type=str.lower) # Require --target argument
+    parser.add_argument('--target-modality', nargs='+', required=True, type=str.lower) # Require --target argument
     parser.add_argument('--label', required=True,
         help='Label of XNAT MR Session')  # Require label argument
     args = parser.parse_args()
 
     with open(args.config) as fo:
         configs = yaml.load(fo, Loader=yaml.SafeLoader)
```

## Comparing `xnattagger-0.6.7.dist-info/LICENSE` & `xnattagger-0.6.8.dist-info/LICENSE`

 * *Files identical despite different names*

