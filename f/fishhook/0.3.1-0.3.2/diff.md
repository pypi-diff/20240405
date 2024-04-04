# Comparing `tmp/fishhook-0.3.1.tar.gz` & `tmp/fishhook-0.3.2-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fishhook-0.3.1.tar", last modified: Wed Apr  3 19:50:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

