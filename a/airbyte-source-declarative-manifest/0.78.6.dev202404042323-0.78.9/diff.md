# Comparing `tmp/airbyte_source_declarative_manifest-0.78.6.dev202404042323.tar.gz` & `tmp/airbyte_source_declarative_manifest-0.78.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_declarative_manifest-0.78.6.dev202404042323.tar", max compression
+gzip compressed data, was "airbyte_source_declarative_manifest-0.78.9.tar", max compression
```

## Comparing `airbyte_source_declarative_manifest-0.78.6.dev202404042323.tar` & `airbyte_source_declarative_manifest-0.78.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4712 2024-04-04 23:20:32.818488 airbyte_source_declarative_manifest-0.78.6.dev202404042323/README.md
--rw-r--r--   0        0        0      833 2024-04-04 23:23:58.938899 airbyte_source_declarative_manifest-0.78.6.dev202404042323/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 23:20:32.818488 airbyte_source_declarative_manifest-0.78.6.dev202404042323/source_declarative_manifest/__init__.py
--rw-r--r--   0        0        0     2570 2024-04-04 23:20:32.818488 airbyte_source_declarative_manifest-0.78.6.dev202404042323/source_declarative_manifest/run.py
--rw-r--r--   0        0        0      554 2024-04-04 23:20:32.818488 airbyte_source_declarative_manifest-0.78.6.dev202404042323/source_declarative_manifest/spec.json
--rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.78.6.dev202404042323/PKG-INFO
+-rw-r--r--   0        0        0     3992 2024-04-05 16:33:09.000000 airbyte_source_declarative_manifest-0.78.9/README.md
+-rw-r--r--   0        0        0      817 2024-04-05 16:47:04.529701 airbyte_source_declarative_manifest-0.78.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 16:33:09.000000 airbyte_source_declarative_manifest-0.78.9/source_declarative_manifest/__init__.py
+-rw-r--r--   0        0        0     2180 2024-04-05 16:33:09.000000 airbyte_source_declarative_manifest-0.78.9/source_declarative_manifest/run.py
+-rw-r--r--   0        0        0      554 2024-04-05 16:33:09.000000 airbyte_source_declarative_manifest-0.78.9/source_declarative_manifest/spec.json
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.78.9/PKG-INFO
```

### Comparing `airbyte_source_declarative_manifest-0.78.6.dev202404042323/pyproject.toml` & `airbyte_source_declarative_manifest-0.78.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.78.6.dev202404042323"
+version = "0.78.9"
 name = "airbyte-source-declarative-manifest"
 description = "Base source implementation for low-code sources."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_declarative_manifest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.78.6"
+airbyte-cdk = "0.78.9"
 
 [tool.poetry.scripts]
 source-declarative-manifest = "source_declarative_manifest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
 pytest = "^6.2"
```

### Comparing `airbyte_source_declarative_manifest-0.78.6.dev202404042323/source_declarative_manifest/spec.json` & `airbyte_source_declarative_manifest-0.78.9/source_declarative_manifest/spec.json`

 * *Files identical despite different names*

