# Comparing `tmp/arkindex-base-worker-0.3.7rc7.tar.gz` & `tmp/arkindex_base_worker-0.3.7rc8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.7rc7.tar", last modified: Thu Apr  4 13:32:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

