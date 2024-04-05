# Comparing `tmp/faust_avro_model_codegen-0.1.5.tar.gz` & `tmp/faust_avro_model_codegen-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faust_avro_model_codegen-0.1.5.tar", max compression
+gzip compressed data, was "faust_avro_model_codegen-0.1.6.tar", max compression
```

## Comparing `faust_avro_model_codegen-0.1.5.tar` & `faust_avro_model_codegen-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.5/LICENSE
--rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-05 16:36:51.354296 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-05 16:36:51.354932 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__main__.py
--rw-r--r--   0        0        0     2137 2024-04-05 16:36:51.355329 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/models_generator.py
--rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/schema_verifier.py
--rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/settings.py
--rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/template_renderer.py
--rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/enum.py.jinja2
--rw-r--r--   0        0        0     1432 2024-04-05 18:59:58.111934 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/faust_record.jinja2
--rw-r--r--   0        0        0      376 2024-04-05 19:00:07.722063 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/models.py.jinja2
--rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/types.py
--rw-r--r--   0        0        0     1313 2024-04-05 19:11:05.513687 faust_avro_model_codegen-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 16:36:51.354296 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-05 16:36:51.354932 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__main__.py
+-rw-r--r--   0        0        0     2137 2024-04-05 16:36:51.355329 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/models_generator.py
+-rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/schema_verifier.py
+-rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/settings.py
+-rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/template_renderer.py
+-rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/enum.py.jinja2
+-rw-r--r--   0        0        0     1432 2024-04-05 19:17:54.836876 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/faust_record.jinja2
+-rw-r--r--   0        0        0      376 2024-04-05 19:17:54.843765 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/models.py.jinja2
+-rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/types.py
+-rw-r--r--   0        0        0     1314 2024-04-05 19:19:16.703948 faust_avro_model_codegen-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.6/PKG-INFO
```

### Comparing `faust_avro_model_codegen-0.1.5/LICENSE` & `faust_avro_model_codegen-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/README.md` & `faust_avro_model_codegen-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__main__.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/models_generator.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/models_generator.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/schema_verifier.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/schema_verifier.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/settings.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/template_renderer.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/template_renderer.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/faust_record.jinja2` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/faust_record.jinja2`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/types.py` & `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/types.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.5/pyproject.toml` & `faust_avro_model_codegen-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "faust-avro-model-codegen"
-version = "0.1.5"
+version = "0.1.6"
 description = "Generate Faust Avro Models from Avro Schema files."
 authors = ["Sean Zicari <szicari@streambit.software, Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bboggs-streambit/faust-avro-model-codegen"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 typer = ">=0.9.0"
 autoflake = ">2.0.0"
 jinja2 = "^3.1.3"
 black = ">23.0.0"
 isort = "^5.13.2"
 rich = "^13.7.1"
-httpx = "^0.27.0"
+httpx = ">=0.24.0"
 dataclasses-avroschema = {extras = ["faust"], version = ">=0.58.0"}
 mode-streaming = "<0.4.0"
 pydantic = ">1.0.0"
 plumbum = "^1.8.2"
 tomlkit = ">=0.12.0"
```

### Comparing `faust_avro_model_codegen-0.1.5/PKG-INFO` & `faust_avro_model_codegen-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: faust-avro-model-codegen
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate Faust Avro Models from Avro Schema files.
 Home-page: https://github.com/bboggs-streambit/faust-avro-model-codegen
 License: MIT
 Author: Sean Zicari
 Author-email: szicari@streambit.software, Brad Boggs <bboggs@streambit.software
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: autoflake (>2.0.0)
 Requires-Dist: black (>23.0.0)
 Requires-Dist: dataclasses-avroschema[faust] (>=0.58.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: mode-streaming (<0.4.0)
 Requires-Dist: plumbum (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic (>1.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tomlkit (>=0.12.0)
```

