# Comparing `tmp/tempsdb-0.6.4.tar.gz` & `tmp/tempsdb-0.6.5-cp39-cp39-manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempsdb-0.6.4.tar", last modified: Fri Jul  9 15:56:45 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

