# Comparing `tmp/magenpy-0.0.9.tar.gz` & `tmp/magenpy-0.1.0-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/szabad/PycharmProjects/magenpy/dist/tmp_e27mdvg/magenpy-0.0.9.tar", last modified: Tue Aug  9 20:36:12 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

