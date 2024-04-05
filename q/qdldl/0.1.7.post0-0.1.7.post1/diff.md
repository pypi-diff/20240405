# Comparing `tmp/qdldl-0.1.7.post0.tar.gz` & `tmp/qdldl-0.1.7.post1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/qdldl-0.1.7.post0.tar", last modified: Wed Jul  5 18:10:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

