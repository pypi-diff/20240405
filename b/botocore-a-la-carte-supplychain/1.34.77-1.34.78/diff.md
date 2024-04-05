# Comparing `tmp/botocore-a-la-carte-supplychain-1.34.77.tar.gz` & `tmp/botocore_a_la_carte_supplychain-1.34.78-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-supplychain-1.34.77.tar", last modified: Thu Apr  4 01:01:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

