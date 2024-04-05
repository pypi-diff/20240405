# Comparing `tmp/rustyrs-0.3.1.tar.gz` & `tmp/rustyrs-0.3.2-cp311-cp311-manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

