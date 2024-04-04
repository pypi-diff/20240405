# Comparing `tmp/uf-toolkit-0.2.0.tar.gz` & `tmp/uf_toolkit-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uf-toolkit-0.2.0.tar", last modified: Wed Mar 27 23:11:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

