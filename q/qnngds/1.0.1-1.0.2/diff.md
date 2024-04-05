# Comparing `tmp/qnngds-1.0.1.tar.gz` & `tmp/qnngds-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-1.0.1.tar", last modified: Thu Apr  4 21:36:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

