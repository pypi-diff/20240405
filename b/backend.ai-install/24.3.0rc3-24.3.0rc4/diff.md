# Comparing `tmp/backend.ai-install-24.3.0rc3.tar.gz` & `tmp/backend.ai_install-24.3.0rc4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-install-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

