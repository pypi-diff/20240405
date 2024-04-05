# Comparing `tmp/faust_avro_model_codegen-0.1.4.tar.gz` & `tmp/faust_avro_model_codegen-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faust_avro_model_codegen-0.1.4.tar", max compression
+gzip compressed data, was "faust_avro_model_codegen-0.1.5.tar", max compression
```

## Comparing `faust_avro_model_codegen-0.1.4.tar` & `faust_avro_model_codegen-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.4/LICENSE
--rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-05 16:36:51.354296 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-05 16:36:51.354932 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/__main__.py
--rw-r--r--   0        0        0     2137 2024-04-05 16:36:51.355329 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/models_generator.py
--rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/schema_verifier.py
--rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/settings.py
--rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/template_renderer.py
--rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/templates/enum.py.jinja2
--rw-r--r--   0        0        0     1522 2024-04-05 17:26:46.466878 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/templates/faust_record.jinja2
--rw-r--r--   0        0        0      465 2024-04-05 17:20:52.120279 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/templates/models.py.jinja2
--rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/types.py
--rw-r--r--   0        0        0     1334 2024-04-05 18:38:47.169848 faust_avro_model_codegen-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 16:36:51.354296 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-05 16:36:51.354932 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__main__.py
+-rw-r--r--   0        0        0     2137 2024-04-05 16:36:51.355329 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/models_generator.py
+-rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/schema_verifier.py
+-rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/settings.py
+-rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/template_renderer.py
+-rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/enum.py.jinja2
+-rw-r--r--   0        0        0     1432 2024-04-05 18:59:58.111934 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/faust_record.jinja2
+-rw-r--r--   0        0        0      376 2024-04-05 19:00:07.722063 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/models.py.jinja2
+-rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/types.py
+-rw-r--r--   0        0        0     1313 2024-04-05 19:11:05.513687 faust_avro_model_codegen-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.5/PKG-INFO
```

### Comparing `faust_avro_model_codegen-0.1.4/LICENSE` & `faust_avro_model_codegen-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/README.md` & `faust_avro_model_codegen-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/__main__.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/models_generator.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/models_generator.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/schema_verifier.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/schema_verifier.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/settings.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/template_renderer.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/template_renderer.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/templates/faust_record.jinja2` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/templates/faust_record.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import typing, enum, dataclasses, datetime
 
 from dataclasses import dataclass, field
-try:
-    from dataclasses_avroschema.avrodantic import CT
-except ModuleNotFoundError:
-    from dataclasses_avroschema.schema_generator import CT
+from dataclasses_avroschema.schema_generator import CT
 from dataclasses_avroschema.faust import AvroRecord
 
 
 @dataclass
 class {{ c.name }}(AvroRecord):
     def __post_init__(self) -> None:
         for _field in dataclasses.fields(self):
```

### Comparing `faust_avro_model_codegen-0.1.4/faust_avro_model_codegen/types.py` & `faust_avro_model_codegen-0.1.5/faust_avro_model_codegen/types.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.4/pyproject.toml` & `faust_avro_model_codegen-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faust-avro-model-codegen"
-version = "0.1.4"
+version = "0.1.5"
 description = "Generate Faust Avro Models from Avro Schema files."
 authors = ["Sean Zicari <szicari@streambit.software, Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bboggs-streambit/faust-avro-model-codegen"
 
 [tool.poetry.dependencies]
@@ -34,11 +34,11 @@
 
 [tool.coverage.run]
 omit = ["*/site-packages/*" ,"*/distutils/*" ,"*/tests/*" ,"*/__init__.py", "*/__main__.py"]
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING', 'case never', 'typing.assert_never']
 
 [tool.pytest.ini_options]
-addopts = "-v --cov=faust_avro_code_gen --cov-report=term-missing --cov-report=xml --cov-report=html --cov-fail-under=100"
+addopts = "-v --cov=faust_avro_code_gen --cov-report=term-missing --cov-report=xml --cov-report=html"
 testpaths = ["tests"]
 python_files = ["test_*.py", " *_tests.py", "*test*.py"]
 pythonpath = "."
```

### Comparing `faust_avro_model_codegen-0.1.4/PKG-INFO` & `faust_avro_model_codegen-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faust-avro-model-codegen
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate Faust Avro Models from Avro Schema files.
 Home-page: https://github.com/bboggs-streambit/faust-avro-model-codegen
 License: MIT
 Author: Sean Zicari
 Author-email: szicari@streambit.software, Brad Boggs <bboggs@streambit.software
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

