# Comparing `tmp/faust_avro_model_codegen-0.1.0.tar.gz` & `tmp/faust_avro_model_codegen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faust_avro_model_codegen-0.1.0.tar", max compression
+gzip compressed data, was "faust_avro_model_codegen-0.1.1.tar", max compression
```

## Comparing `faust_avro_model_codegen-0.1.0.tar` & `faust_avro_model_codegen-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.0/LICENSE
--rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-04 01:40:41.210165 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-05 15:54:00.157058 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/__main__.py
--rw-r--r--   0        0        0     2137 2024-04-04 21:10:41.978931 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/models_generator.py
--rw-r--r--   0        0        0     1642 2024-04-05 15:54:00.498726 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/schema_verifier.py
--rw-r--r--   0        0        0     1121 2024-04-04 20:55:02.367295 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/settings.py
--rw-r--r--   0        0        0     1939 2024-04-04 17:22:14.465653 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/template_renderer.py
--rw-r--r--   0        0        0      124 2024-04-02 16:52:58.713549 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/templates/enum.py.jinja2
--rw-r--r--   0        0        0     1426 2024-04-02 16:52:58.714573 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/templates/faust_record.jinja2
--rw-r--r--   0        0        0      368 2024-04-02 16:52:58.738340 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/templates/models.py.jinja2
--rw-r--r--   0        0        0     6258 2024-04-04 18:33:47.365894 faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/types.py
--rw-r--r--   0        0        0     1255 2024-04-05 15:49:42.699602 faust_avro_model_codegen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 16:19:21.530744 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-05 16:23:55.252305 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/__main__.py
+-rw-r--r--   0        0        0     2137 2024-04-05 16:19:21.533095 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/models_generator.py
+-rw-r--r--   0        0        0     1642 2024-04-05 16:23:55.267358 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/schema_verifier.py
+-rw-r--r--   0        0        0     1121 2024-04-05 16:19:21.536000 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/settings.py
+-rw-r--r--   0        0        0     1939 2024-04-05 16:19:21.536657 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/template_renderer.py
+-rw-r--r--   0        0        0      124 2024-04-05 16:19:21.537712 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/templates/enum.py.jinja2
+-rw-r--r--   0        0        0     1426 2024-04-05 16:19:21.538478 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/templates/faust_record.jinja2
+-rw-r--r--   0        0        0      368 2024-04-05 16:19:21.538931 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/templates/models.py.jinja2
+-rw-r--r--   0        0        0     6258 2024-04-05 16:19:21.539608 faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/types.py
+-rw-r--r--   0        0        0     1334 2024-04-05 16:22:37.458702 faust_avro_model_codegen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.1/PKG-INFO
```

### Comparing `faust_avro_model_codegen-0.1.0/LICENSE` & `faust_avro_model_codegen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/README.md` & `faust_avro_model_codegen-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/__main__.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/models_generator.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/models_generator.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/schema_verifier.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/schema_verifier.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/settings.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/template_renderer.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/template_renderer.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/templates/faust_record.jinja2` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/templates/faust_record.jinja2`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/faust_avro_model_codegen/types.py` & `faust_avro_model_codegen-0.1.1/faust_avro_model_codegen/types.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.0/pyproject.toml` & `faust_avro_model_codegen-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "faust-avro-model-codegen"
-version = "0.1.0"
+version = "0.1.1"
 description = "Generate Faust Avro Models from Avro Schema files."
 authors = ["Sean Zicari <szicari@streambit.software, Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/bboggs-streambit/faust-avro-model-codegen"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-typer = "^0.12.0"
-autoflake = "^2.3.1"
+python = ">=3.10"
+typer = ">0.10.0"
+autoflake = ">2.0.0"
 jinja2 = "^3.1.3"
-black = "^24.3.0"
+black = ">23.0.0"
 isort = "^5.13.2"
 rich = "^13.7.1"
 httpx = "^0.27.0"
-dataclasses-avroschema = {extras = ["faust"], version = "^0.58.0"}
+dataclasses-avroschema = {extras = ["faust"], version = ">=0.58.0"}
 mode-streaming = "<0.4.0"
-pydantic = "^2.6.4"
+pydantic = ">1.0.0"
 plumbum = "^1.8.2"
-tomlkit = "^0.12.4"
+tomlkit = ">=0.12.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pydevd-pycharm = ">=232.9559.11,<232.9560.0"
```

### Comparing `faust_avro_model_codegen-0.1.0/PKG-INFO` & `faust_avro_model_codegen-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: faust-avro-model-codegen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate Faust Avro Models from Avro Schema files.
+Home-page: https://github.com/bboggs-streambit/faust-avro-model-codegen
 License: MIT
 Author: Sean Zicari
 Author-email: szicari@streambit.software, Brad Boggs <bboggs@streambit.software
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: autoflake (>=2.3.1,<3.0.0)
-Requires-Dist: black (>=24.3.0,<25.0.0)
-Requires-Dist: dataclasses-avroschema[faust] (>=0.58.0,<0.59.0)
+Requires-Dist: autoflake (>2.0.0)
+Requires-Dist: black (>23.0.0)
+Requires-Dist: dataclasses-avroschema[faust] (>=0.58.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: mode-streaming (<0.4.0)
 Requires-Dist: plumbum (>=1.8.2,<2.0.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>1.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
-Requires-Dist: typer (>=0.12.0,<0.13.0)
+Requires-Dist: tomlkit (>=0.12.0)
+Requires-Dist: typer (>0.10.0)
+Project-URL: Repository, https://github.com/bboggs-streambit/faust-avro-model-codegen
 Description-Content-Type: text/markdown
 
 # Faust Avro Code Generator
 
 This is a Python library that generates Faust models from Avro schemas.
 
 ## Installation
```

