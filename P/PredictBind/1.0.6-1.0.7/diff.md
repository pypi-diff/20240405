# Comparing `tmp/PredictBind-1.0.6.tar.gz` & `tmp/PredictBind-1.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PredictBind-1.0.6.tar", last modified: Fri Apr  5 19:38:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

