# Comparing `tmp/sirji-agents-0.0.4.tar.gz` & `tmp/sirji_agents-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.4.tar", last modified: Thu Apr  4 13:12:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

