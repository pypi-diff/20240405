# Comparing `tmp/dialog-workflow-local-0.0.86.tar.gz` & `tmp/dialog_workflow_local-0.0.87-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.86.tar", last modified: Fri Mar 22 10:28:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

