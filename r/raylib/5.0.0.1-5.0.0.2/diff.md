# Comparing `tmp/raylib-5.0.0.1.tar.gz` & `tmp/raylib-5.0.0.2-cp39-cp39-macosx_14_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raylib-5.0.0.1.tar", last modified: Mon Jan 22 15:17:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

