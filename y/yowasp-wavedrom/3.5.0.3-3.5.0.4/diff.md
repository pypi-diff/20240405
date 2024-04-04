# Comparing `tmp/yowasp_wavedrom-3.5.0.3-py3-none-any.whl.zip` & `tmp/yowasp_wavedrom-3.5.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40660 bytes, number of entries: 7
--rw-r--r--  2.0 unx      843 b- defN 24-Apr-04 17:30 yowasp_wavedrom/__init__.py
--rw-r--r--  2.0 unx   392672 b- defN 24-Apr-04 17:30 yowasp_wavedrom/bundle.js
--rw-r--r--  2.0 unx     3125 b- defN 24-Apr-04 17:31 yowasp_wavedrom-3.5.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 17:31 yowasp_wavedrom-3.5.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 17:31 yowasp_wavedrom-3.5.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-04 17:31 yowasp_wavedrom-3.5.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      610 b- defN 24-Apr-04 17:31 yowasp_wavedrom-3.5.0.3.dist-info/RECORD
-7 files, 397420 bytes uncompressed, 39566 bytes compressed:  90.0%
+Zip file size: 40658 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      843 b- defN 24-Apr-04 23:00 yowasp_wavedrom/__init__.py
+-rw-r--r--  2.0 unx   392666 b- defN 24-Apr-04 23:00 yowasp_wavedrom/bundle.js
+-rw-r--r--  2.0 unx     3125 b- defN 24-Apr-04 23:00 yowasp_wavedrom-3.5.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 23:00 yowasp_wavedrom-3.5.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 23:00 yowasp_wavedrom-3.5.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-04 23:00 yowasp_wavedrom-3.5.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-04 23:00 yowasp_wavedrom-3.5.0.4.dist-info/RECORD
+7 files, 397414 bytes uncompressed, 39564 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yowasp_wavedrom/__init__.py
 Comment: 
 
 Filename: yowasp_wavedrom/bundle.js
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.3.dist-info/METADATA
+Filename: yowasp_wavedrom-3.5.0.4.dist-info/METADATA
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.3.dist-info/WHEEL
+Filename: yowasp_wavedrom-3.5.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.3.dist-info/entry_points.txt
+Filename: yowasp_wavedrom-3.5.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.3.dist-info/top_level.txt
+Filename: yowasp_wavedrom-3.5.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.3.dist-info/RECORD
+Filename: yowasp_wavedrom-3.5.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yowasp_wavedrom/bundle.js

### js-beautify {}

```diff
@@ -26721,15 +26721,15 @@
 };
 WaveSkin.default = JSON.parse(JSON.stringify(WaveSkin.light));
 WaveSkin.default[2][2] = `@media(prefers-color-scheme:light){${WaveSkin.light[2][2]}}@media(prefers-color-scheme:dark){${WaveSkin.dark[2][2]}}`;
 
 function renderSignal(source) {
     const rendered = (0, import_render_signal.default)(0, source, WaveSkin);
     delete rendered[1]["id"];
-    delete rendered[4][2][1]["style"];
+    rendered[4][2].splice(1, 1);
     return (0, import_stringify.default)(rendered);
 }
 
 function renderBitField(source) {
     const rendered = (0, import_render_reg.default)(0, source);
     rendered.splice(2, 0, ["style", {}, "@media(prefers-color-scheme:dark){:root{filter:invert(1)}}"]);
     return (0, import_stringify.default)(rendered);
```

## Comparing `yowasp_wavedrom-3.5.0.3.dist-info/METADATA` & `yowasp_wavedrom-3.5.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yowasp-wavedrom
-Version: 3.5.0.3
+Version: 3.5.0.4
 Summary: WaveDrom generates diagrams for digital waveforms, bit fields, and simple combinational circuits
 Author-email: Catherine <whitequark@whitequark.org>
 License: MIT
 Project-URL: Homepage, https://yowasp.org/
 Project-URL: Source Code, https://github.com/YoWASP/wavedrom
 Project-URL: Bug Tracker, https://github.com/YoWASP/wavedrom/issues
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `yowasp_wavedrom-3.5.0.3.dist-info/RECORD` & `yowasp_wavedrom-3.5.0.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 yowasp_wavedrom/__init__.py,sha256=ROOgQsV6z8snf-ZKQZX2KW6nZh4MUF47UOLfDQgYndk,843
-yowasp_wavedrom/bundle.js,sha256=mUTijLUykc-iz020AqiPa5NQJlfabkLkL6gFfnUOwNg,392672
-yowasp_wavedrom-3.5.0.3.dist-info/METADATA,sha256=jhbGdJF1RioYLKQ486XeV9QhCOT0N_RyG-Zk1Kv0k9g,3125
-yowasp_wavedrom-3.5.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-yowasp_wavedrom-3.5.0.3.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
-yowasp_wavedrom-3.5.0.3.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
-yowasp_wavedrom-3.5.0.3.dist-info/RECORD,,
+yowasp_wavedrom/bundle.js,sha256=rAsoqZhCJxhC2a3u5h3bnRnGvrpNRzTT38B5FMSPywc,392666
+yowasp_wavedrom-3.5.0.4.dist-info/METADATA,sha256=AgQnNTHgjaawPoU_Pm7SXgWxqGjuiB0NynqBN9ZI4nE,3125
+yowasp_wavedrom-3.5.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+yowasp_wavedrom-3.5.0.4.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
+yowasp_wavedrom-3.5.0.4.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
+yowasp_wavedrom-3.5.0.4.dist-info/RECORD,,
```

