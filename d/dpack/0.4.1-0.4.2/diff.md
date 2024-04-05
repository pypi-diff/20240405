# Comparing `tmp/dpack-0.4.1-py3-none-any.whl.zip` & `tmp/dpack-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11474 bytes, number of entries: 17
--rw-r--r--  2.0 unx      172 b- defN 22-Jun-21 15:01 dpack/__init__.py
+Zip file size: 11484 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      172 b- defN 22-Aug-05 13:49 dpack/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 21-Oct-21 15:51 dpack/__main__.py
--rw-r--r--  2.0 unx     8394 b- defN 22-Jun-21 14:58 dpack/base.py
--rw-r--r--  2.0 unx     1706 b- defN 22-Jun-14 19:59 dpack/cli.py
+-rw-r--r--  2.0 unx     8448 b- defN 22-Aug-05 13:47 dpack/base.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-Dec-16 00:34 dpack/cli.py
 -rw-r--r--  2.0 unx     2516 b- defN 22-Jun-14 20:00 dpack/finders.py
 -rw-r--r--  2.0 unx     1027 b- defN 21-Oct-21 15:51 dpack/serve.py
 -rw-r--r--  2.0 unx       68 b- defN 21-Oct-21 15:51 dpack/processors/__init__.py
 -rw-r--r--  2.0 unx       83 b- defN 21-Oct-21 15:51 dpack/processors/cssmin.py
 -rw-r--r--  2.0 unx       80 b- defN 21-Oct-21 15:51 dpack/processors/jsmin.py
 -rw-r--r--  2.0 unx     1686 b- defN 22-Jun-14 19:59 dpack/processors/rewrite.py
 -rw-r--r--  2.0 unx      141 b- defN 21-Oct-21 15:51 dpack/processors/sass.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5424 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1304 b- defN 22-Jun-21 15:03 dpack-0.4.1.dist-info/RECORD
-17 files, 23868 bytes uncompressed, 9348 bytes compressed:  60.8%
+-rw-r--r--  2.0 unx     1067 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5424 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1304 b- defN 24-Apr-05 13:41 dpack-0.4.2.dist-info/RECORD
+17 files, 23922 bytes uncompressed, 9358 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: dpack/processors/rewrite.py
 Comment: 
 
 Filename: dpack/processors/sass.py
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/LICENSE
+Filename: dpack-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/METADATA
+Filename: dpack-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/WHEEL
+Filename: dpack-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/entry_points.txt
+Filename: dpack-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/top_level.txt
+Filename: dpack-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dpack-0.4.1.dist-info/RECORD
+Filename: dpack-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dpack/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .base import DPack
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __version_info__ = tuple(int(num) for num in __version__.split("."))
 
 __all__ = ["DPack", "__version__", "__version_info__"]
```

## dpack/base.py

```diff
@@ -30,15 +30,15 @@
     def modified(self, mtime):
         for path in self.check_paths():
             if os.path.getmtime(path) > mtime:
                 return True
         return False
 
     def process(self, packer):
-        with open(self.path, "r") as f:
+        with open(self.path, "r", encoding="utf-8") as f:
             text = f.read()
         for proc in self.processors:
             module_name, method_name = proc.rsplit(".", 1)
             module = importlib.import_module(module_name)
             method = getattr(module, method_name)
             text = method(text, self, packer)
         return text
@@ -57,15 +57,15 @@
         path = str(path)
         if path.startswith("/") or not self.base_dir:
             return path
         return os.path.abspath(os.path.normpath(os.path.join(self.base_dir, path)))
 
     def load_config(self, config_file, raise_if_missing=False):
         try:
-            with open(self.resolve(config_file), "r") as f:
+            with open(self.resolve(config_file), "r", encoding="utf-8") as f:
                 return yaml.safe_load(f)
         except FileNotFoundError as e:
             if raise_if_missing:
                 raise e
         return {}
 
     def dump_config(self):
@@ -215,12 +215,12 @@
             if force or mtime == 0 or self.modified(inputs, mtime):
                 ext = os.path.splitext(name)[1].replace(".", "").lower()
                 sep = self.concat.get(ext, "\n")
                 os.makedirs(os.path.dirname(path), exist_ok=True)
                 logger.debug(
                     "Packing {} <<< {}".format(name, " | ".join(str(i) for i in inputs))
                 )
-                with open(path, "w") as output:
+                with open(path, "w", encoding="utf-8") as output:
                     for idx, i in enumerate(inputs):
                         if idx > 0:
                             output.write(sep)
                         output.write(i.process(self))
```

## Comparing `dpack-0.4.1.dist-info/LICENSE` & `dpack-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dpack-0.4.1.dist-info/METADATA` & `dpack-0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpack
-Version: 0.4.1
+Version: 0.4.2
 Summary: Asset packager for Django.
 Home-page: https://github.com/dcwatson/dpack
 Author: Dan Watson
 Author-email: dcwatson@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `dpack-0.4.1.dist-info/RECORD` & `dpack-0.4.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-dpack/__init__.py,sha256=vOiIOMA5QX0QvinWEiJUk2-YQF5H3LPVKVuz0j1hzU0,172
+dpack/__init__.py,sha256=6_-B56ArSbTDvA2Cyo2BDwwJXN7_QgDpj9JdDkCbsO0,172
 dpack/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
-dpack/base.py,sha256=QOQLej10TRU6VVqHm8QDnRSUiKs33ZRKnWpoIqYWhgQ,8394
+dpack/base.py,sha256=dOBiyntgQoGMpvDwimR2vPKpEpxUZ-bnxWG6aPhIPO8,8448
 dpack/cli.py,sha256=-hKssHpKAdNeHd6OvkG5qdMGP2TlK5itDolk0bLEZog,1706
 dpack/finders.py,sha256=H-uACaHtoODQM_7RMyjoJpplQ63HuoQ88hCktTIrwv0,2516
 dpack/serve.py,sha256=JFUGqXofO-L_RDcoEBOQv18BkKoIbu4bis-tuxUww8U,1027
 dpack/processors/__init__.py,sha256=mBzq3wdhGA-4AO27bX-nqXzqvayMq4xxiV2fw25Z8y4,68
 dpack/processors/cssmin.py,sha256=FZkLg04XyRzY-mLvzekpMYlf3aqMD1wV_3pTLo4GhW8,83
 dpack/processors/jsmin.py,sha256=9yMTaY_zxB2tFu-rRwrD-GWxsg7_CQQbc8RL0LczivI,80
 dpack/processors/rewrite.py,sha256=qP9MTN_6mffYD0_1er2vzN3T_-IAymy1ErbbzeUEnvE,1686
 dpack/processors/sass.py,sha256=6G10mWYU2ODtE1d44XBw1p5b7CiR7OrtSplh0p0fyeU,141
-dpack-0.4.1.dist-info/LICENSE,sha256=KjCadNFiCaHtKQ7tZCKJ5y-f0cyPcnWMR5OWqD9VaYU,1067
-dpack-0.4.1.dist-info/METADATA,sha256=GcoqFxaH-3TgN6qEp9Ufdzmreq32-EHV6W3dDQFk8Rw,5424
-dpack-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dpack-0.4.1.dist-info/entry_points.txt,sha256=UAsq9qmzp7KDwww9HGY3WxvyCJbM2aSAxvXiTEyknPU,41
-dpack-0.4.1.dist-info/top_level.txt,sha256=o1L7CWqAi50Wj1PUSXUOR76hNta97GUoXXC6PyX7jU4,6
-dpack-0.4.1.dist-info/RECORD,,
+dpack-0.4.2.dist-info/LICENSE,sha256=KjCadNFiCaHtKQ7tZCKJ5y-f0cyPcnWMR5OWqD9VaYU,1067
+dpack-0.4.2.dist-info/METADATA,sha256=MK2gqH5JOCNOysxpGo5fgAzJnML2RcoBH5-D0bOpmlw,5424
+dpack-0.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dpack-0.4.2.dist-info/entry_points.txt,sha256=UAsq9qmzp7KDwww9HGY3WxvyCJbM2aSAxvXiTEyknPU,41
+dpack-0.4.2.dist-info/top_level.txt,sha256=o1L7CWqAi50Wj1PUSXUOR76hNta97GUoXXC6PyX7jU4,6
+dpack-0.4.2.dist-info/RECORD,,
```

