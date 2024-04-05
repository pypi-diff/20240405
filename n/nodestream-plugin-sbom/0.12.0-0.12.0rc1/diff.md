# Comparing `tmp/nodestream_plugin_sbom-0.12.0.tar.gz` & `tmp/nodestream_plugin_sbom-0.12.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_sbom-0.12.0.tar", max compression
+gzip compressed data, was "nodestream_plugin_sbom-0.12.0rc1.tar", max compression
```

## Comparing `nodestream_plugin_sbom-0.12.0.tar` & `nodestream_plugin_sbom-0.12.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-03 14:32:26.788760 nodestream_plugin_sbom-0.12.0/LICENSE
--rw-r--r--   0        0        0     7717 2024-04-03 14:32:26.788932 nodestream_plugin_sbom-0.12.0/README.md
--rw-r--r--   0        0        0      279 2024-04-03 14:32:26.789503 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/__init__.py
--rw-r--r--   0        0        0      109 2024-04-03 14:32:26.789747 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/amazon_inspector/__init__.py
--rw-r--r--   0        0        0     5991 2024-04-03 14:32:26.789906 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/amazon_inspector/amazon_inspector_sbom.py
--rw-r--r--   0        0        0       81 2024-04-03 14:32:26.790107 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/github/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-03 14:32:26.790255 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/github/github_sbom.py
--rw-r--r--   0        0        0      265 2024-04-03 14:32:26.790392 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/plugin.py
--rw-r--r--   0        0        0       62 2024-04-03 14:32:26.790706 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom/__init__.py
--rw-r--r--   0        0        0     2436 2024-04-03 14:32:26.790840 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom/sbom.py
--rw-r--r--   0        0        0     2980 2024-04-03 14:32:26.790517 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom.yaml
--rw-r--r--   0        0        0     3040 2024-04-03 14:32:26.790953 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom_amazon_inspector.yaml
--rw-r--r--   0        0        0     2982 2024-04-03 14:32:26.791059 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom_github.yaml
--rw-r--r--   0        0        0        0 2024-04-03 14:32:26.791212 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/__init__.py
--rw-r--r--   0        0        0     9602 2024-04-03 14:32:26.791383 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/cyclonedx_writer.py
--rw-r--r--   0        0        0      831 2024-04-03 14:32:26.791539 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/sbom_writer.py
--rw-r--r--   0        0        0     8793 2024-04-03 14:32:26.791668 nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/spdx_writer.py
--rw-r--r--   0        0        0      601 2024-04-05 14:48:06.953964 nodestream_plugin_sbom-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     8512 1970-01-01 00:00:00.000000 nodestream_plugin_sbom-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 14:32:26.788760 nodestream_plugin_sbom-0.12.0rc1/LICENSE
+-rw-r--r--   0        0        0     7717 2024-04-03 14:32:26.788932 nodestream_plugin_sbom-0.12.0rc1/README.md
+-rw-r--r--   0        0        0      279 2024-04-03 14:32:26.789503 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-03 14:32:26.789747 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/amazon_inspector/__init__.py
+-rw-r--r--   0        0        0     5991 2024-04-03 14:32:26.789906 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/amazon_inspector/amazon_inspector_sbom.py
+-rw-r--r--   0        0        0       81 2024-04-03 14:32:26.790107 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/github/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-03 14:32:26.790255 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/github/github_sbom.py
+-rw-r--r--   0        0        0      265 2024-04-03 14:32:26.790392 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/plugin.py
+-rw-r--r--   0        0        0       62 2024-04-03 14:32:26.790706 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom/__init__.py
+-rw-r--r--   0        0        0     2436 2024-04-03 14:32:26.790840 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom/sbom.py
+-rw-r--r--   0        0        0     2980 2024-04-03 14:32:26.790517 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom.yaml
+-rw-r--r--   0        0        0     3040 2024-04-03 14:32:26.790953 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom_amazon_inspector.yaml
+-rw-r--r--   0        0        0     2982 2024-04-03 14:32:26.791059 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom_github.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 14:32:26.791212 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/__init__.py
+-rw-r--r--   0        0        0     9602 2024-04-03 14:32:26.791383 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/cyclonedx_writer.py
+-rw-r--r--   0        0        0      831 2024-04-03 14:32:26.791539 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/sbom_writer.py
+-rw-r--r--   0        0        0     8793 2024-04-03 14:32:26.791668 nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/spdx_writer.py
+-rw-r--r--   0        0        0      608 2024-04-03 14:33:15.626879 nodestream_plugin_sbom-0.12.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     8467 1970-01-01 00:00:00.000000 nodestream_plugin_sbom-0.12.0rc1/PKG-INFO
```

### Comparing `nodestream_plugin_sbom-0.12.0/LICENSE` & `nodestream_plugin_sbom-0.12.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/README.md` & `nodestream_plugin_sbom-0.12.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/amazon_inspector/amazon_inspector_sbom.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/amazon_inspector/amazon_inspector_sbom.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/github/github_sbom.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/github/github_sbom.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom/sbom.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom/sbom.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom.yaml` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom_amazon_inspector.yaml` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom_amazon_inspector.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/sbom_github.yaml` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/sbom_github.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/cyclonedx_writer.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/cyclonedx_writer.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/sbom_writer.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/sbom_writer.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/nodestream_plugin_sbom/utils/spdx_writer.py` & `nodestream_plugin_sbom-0.12.0rc1/nodestream_plugin_sbom/utils/spdx_writer.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_sbom-0.12.0/pyproject.toml` & `nodestream_plugin_sbom-0.12.0rc1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nodestream-plugin-sbom"
-version = "0.12.0"
+version = "0.12.0rc1"
 description = "A plugin for nodestream that allows for importing Software Bill of Materials"
 authors = ["Dave Bechberger <dbechbe@amazon.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-nodestream = "^0.12.0"
+nodestream = "^0.12.0rc2"
 boto3 = "^1.34.40"
 flatdict =  ">=4.0.1"
 black = "^24.3.0"
 pre-commit = "^3.7.0"
 autoflake = "^2.3.1"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."nodestream.plugins"]
 projects = "nodestream_plugin_sbom.plugin"
```

### Comparing `nodestream_plugin_sbom-0.12.0/PKG-INFO` & `nodestream_plugin_sbom-0.12.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-sbom
-Version: 0.12.0
+Version: 0.12.0rc1
 Summary: A plugin for nodestream that allows for importing Software Bill of Materials
 License: Apache 2.0
 Author: Dave Bechberger
 Author-email: dbechbe@amazon.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autoflake (>=2.3.1,<3.0.0)
 Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: boto3 (>=1.34.40,<2.0.0)
 Requires-Dist: flatdict (>=4.0.1)
-Requires-Dist: nodestream (>=0.12.0,<0.13.0)
+Requires-Dist: nodestream (>=0.12.0rc2,<0.13.0)
 Requires-Dist: pre-commit (>=3.7.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Nodestream Software Bill of Material (SBOM) Plugin
 
 This repo contains a Nodestream plugin to import SBOM files in JSON formatted [CycloneDX](https://cyclonedx.org/) and [SPDX](https://spdx.dev/) into an opinionated graph data model in a graph database. Nodestream is a developer friendly Python framework for materializing and working with graph databases.
```

