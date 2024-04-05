# Comparing `tmp/asepyte-0.0.4-py3-none-any.whl.zip` & `tmp/asepyte-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4647 bytes, number of entries: 8
--rw-r--r--  2.0 unx      940 b- defN 24-Apr-05 05:50 asepyte/__init__.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-05 05:50 asepyte/aseprite.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-05 05:50 asepyte/header.py
--rw-r--r--  2.0 unx     1065 b- defN 24-Apr-05 05:51 asepyte-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1321 b- defN 24-Apr-05 05:51 asepyte-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 05:51 asepyte-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-05 05:51 asepyte-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      609 b- defN 24-Apr-05 05:51 asepyte-0.0.4.dist-info/RECORD
-8 files, 8701 bytes uncompressed, 3589 bytes compressed:  58.8%
+Zip file size: 4645 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      940 b- defN 24-Apr-05 05:59 asepyte/__init__.py
+-rw-r--r--  2.0 unx      424 b- defN 24-Apr-05 05:59 asepyte/aseprite.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-05 05:59 asepyte/header.py
+-rw-r--r--  2.0 unx     1065 b- defN 24-Apr-05 05:59 asepyte-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1321 b- defN 24-Apr-05 05:59 asepyte-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 05:59 asepyte-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-05 05:59 asepyte-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      609 b- defN 24-Apr-05 05:59 asepyte-0.0.5.dist-info/RECORD
+8 files, 8701 bytes uncompressed, 3587 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: asepyte/aseprite.py
 Comment: 
 
 Filename: asepyte/header.py
 Comment: 
 
-Filename: asepyte-0.0.4.dist-info/LICENSE
+Filename: asepyte-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: asepyte-0.0.4.dist-info/METADATA
+Filename: asepyte-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: asepyte-0.0.4.dist-info/WHEEL
+Filename: asepyte-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: asepyte-0.0.4.dist-info/top_level.txt
+Filename: asepyte-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: asepyte-0.0.4.dist-info/RECORD
+Filename: asepyte-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asepyte/__init__.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from os import PathLike
 from typing import Protocol
 
 from asepyte.aseprite import Aseprite
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 class _BinaryReadableFile(Protocol):
     def read(self, n: int = -1) -> bytes: ...
 
 
 class _BinaryWritableFile(Protocol):
```

## Comparing `asepyte-0.0.4.dist-info/LICENSE` & `asepyte-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asepyte-0.0.4.dist-info/METADATA` & `asepyte-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asepyte
-Version: 0.0.4
+Version: 0.0.5
 Summary: asepyte
 Home-page: https://github.com/osom8979/asepyte
 Author: zer0
 Author-email: osom8979@gmail.com
 Maintainer: zer0
 Maintainer-email: osom8979@gmail.com
 License: MIT License
```

