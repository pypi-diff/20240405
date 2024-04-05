# Comparing `tmp/p4python-2023.2.2543803.tar.gz` & `tmp/p4python-2023.2.2581979-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\p4python-2023.2.2543803.tar", last modified: Fri Jan 19 01:44:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

