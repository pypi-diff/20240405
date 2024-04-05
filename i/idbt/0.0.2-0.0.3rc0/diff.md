# Comparing `tmp/idbt-0.0.2.tar.gz` & `tmp/idbt-0.0.3rc0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbt-0.0.2.tar", last modified: Fri Apr  5 02:56:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

