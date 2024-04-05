# Comparing `tmp/faust_avro_model_codegen-0.1.6.tar.gz` & `tmp/faust_avro_model_codegen-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faust_avro_model_codegen-0.1.6.tar", max compression
+gzip compressed data, was "faust_avro_model_codegen-0.1.7.tar", max compression
```

## Comparing `faust_avro_model_codegen-0.1.6.tar` & `faust_avro_model_codegen-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.6/LICENSE
--rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-05 16:36:51.354296 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-05 16:36:51.354932 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__main__.py
--rw-r--r--   0        0        0     2137 2024-04-05 16:36:51.355329 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/models_generator.py
--rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/schema_verifier.py
--rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/settings.py
--rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/template_renderer.py
--rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/enum.py.jinja2
--rw-r--r--   0        0        0     1432 2024-04-05 19:17:54.836876 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/faust_record.jinja2
--rw-r--r--   0        0        0      376 2024-04-05 19:17:54.843765 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/models.py.jinja2
--rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/types.py
--rw-r--r--   0        0        0     1314 2024-04-05 19:19:16.703948 faust_avro_model_codegen-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-04-05 15:50:29.658466 faust_avro_model_codegen-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1343 2024-04-05 15:01:42.339435 faust_avro_model_codegen-0.1.7/README.md
+-rw-r--r--   0        0        0      101 2024-04-05 20:38:10.161980 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/__init__.py
+-rw-r--r--   0        0        0     1224 2024-04-05 20:38:10.163631 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/__main__.py
+-rw-r--r--   0        0        0     1563 2024-04-05 20:38:10.172370 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/models_generator.py
+-rw-r--r--   0        0        0      380 2024-04-05 20:38:10.177078 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/schema_dir_parser.py
+-rw-r--r--   0        0        0     1642 2024-04-05 16:36:51.355983 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/schema_verifier.py
+-rw-r--r--   0        0        0     1121 2024-04-05 16:36:51.356228 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/settings.py
+-rw-r--r--   0        0        0     1939 2024-04-05 16:36:51.356479 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/template_renderer.py
+-rw-r--r--   0        0        0      996 2024-04-05 20:38:10.202752 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/template_writer.py
+-rw-r--r--   0        0        0      124 2024-04-05 16:36:51.356971 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/templates/enum.py.jinja2
+-rw-r--r--   0        0        0     1432 2024-04-05 19:17:54.836876 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/templates/faust_record.jinja2
+-rw-r--r--   0        0        0      376 2024-04-05 19:17:54.843765 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/templates/models.py.jinja2
+-rw-r--r--   0        0        0     6258 2024-04-05 16:36:51.358395 faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/types.py
+-rw-r--r--   0        0        0     1314 2024-04-05 20:38:10.203734 faust_avro_model_codegen-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 faust_avro_model_codegen-0.1.7/PKG-INFO
```

### Comparing `faust_avro_model_codegen-0.1.6/LICENSE` & `faust_avro_model_codegen-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/README.md` & `faust_avro_model_codegen-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/__main__.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 
 import httpx
 import typer
 
+from faust_avro_model_codegen import TemplateWriter
 from faust_avro_model_codegen.models_generator import FaustAvroModelGen
+from faust_avro_model_codegen.schema_dir_parser import AvroSchemaDirectoryParser
 from faust_avro_model_codegen.schema_verifier import SchemaVerifier
 from faust_avro_model_codegen.settings import Settings
 from faust_avro_model_codegen.template_renderer import TemplateRenderer
 from faust_avro_model_codegen.types import SchemaData
 
 
 def main(
@@ -16,25 +18,22 @@
         "--verify",
         "-v",
         help="Verify schemas against Schema Registry",
         is_flag=True,
     )
 ):
     config = Settings.from_toml()
-    schemas = [
-        SchemaData.from_file(schema_file.stem, schema_file.read_text())
-        for schema_file in Path(config.schema_dir).glob("*.avsc")
-    ]
-
+    schemas = AvroSchemaDirectoryParser.parse_dir(config.schema_dir)
     app = FaustAvroModelGen(
         renderer=TemplateRenderer.from_current_directory(),
         verifier=SchemaVerifier(
             schema_registry_url=config.schema_registry_url,
             client=lambda: httpx.Client(),
         ),
+        writer=TemplateWriter(),
     )
     app.generate_module(schemas, outfile=config.outfile)
 
     if verify:
         app.verify_schemas(schemas, config.faust_app_models_module)
```

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/models_generator.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/models_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,67 +4,48 @@
 from functools import reduce
 
 import isort
 from plumbum.cmd import autoflake, black  # type: ignore
 
 from .schema_verifier import SchemaVerifier
 from .template_renderer import TemplateRenderer, RenderedTemplate
+from .template_writer import TemplateWriter
 from .types import (
     CodeGenResultData,
     SchemaData,
 )
 
 
 class FaustAvroModelGen:
 
     def __init__(
         self,
         renderer: TemplateRenderer,
         verifier: SchemaVerifier,
+        writer: TemplateWriter,
     ):
         self.renderer = renderer
         self.verifier = verifier
+        self.writer = writer
 
     def generate_module(
         self, schemas: typing.Iterable[SchemaData], outfile: pathlib.Path
     ) -> None:
         codegen_results_from_schemas = (
             CodeGenResultData.from_schema_data(s) for s in schemas
         )
         accum_codegen_data = reduce(
             lambda s, t: s + t,
             codegen_results_from_schemas,
             CodeGenResultData.empty(),
         )
         self.write(outfile, self.renderer.render(accum_codegen_data))
 
-    @classmethod
-    def write(cls, filepath: pathlib.Path, rendered_text: RenderedTemplate) -> None:
-        if not filepath.parent.exists():
-            filepath.parent.mkdir(parents=True)
-
-        filepath.write_text(rendered_text)
-
-        cls._post_process_output_file(filepath)
-
-    @staticmethod
-    def _post_process_output_file(file: pathlib.Path) -> None:
-        isort.file(
-            file,
-            overwrite_in_place=True,
-            remove_redundant_aliases=True,
-            include_trailing_comma=True,
-            group_by_package=True,
-            float_to_top=True,
-            dedup_headings=True,
-            force_sort_within_sections=True,
-            quiet=True,
-        )
-        autoflake(file.absolute(), "--in-place", "--remove-all-unused-imports")
-        black(file.absolute())
+    def write(self, outfile: pathlib.Path, rendered_text: RenderedTemplate) -> None:
+        self.writer.write(outfile, rendered_text)
 
     def verify_schemas(
         self, schemas: typing.Iterable[SchemaData], module_name: str
     ) -> None:
         module = importlib.import_module(module_name)
         generated_classes = {
             schema.name: getattr(module, schema.schema["name"]) for schema in schemas
```

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/schema_verifier.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/schema_verifier.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/settings.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/template_renderer.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/template_renderer.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/templates/faust_record.jinja2` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/templates/faust_record.jinja2`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/faust_avro_model_codegen/types.py` & `faust_avro_model_codegen-0.1.7/faust_avro_model_codegen/types.py`

 * *Files identical despite different names*

### Comparing `faust_avro_model_codegen-0.1.6/pyproject.toml` & `faust_avro_model_codegen-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faust-avro-model-codegen"
-version = "0.1.6"
+version = "0.1.7"
 description = "Generate Faust Avro Models from Avro Schema files."
 authors = ["Sean Zicari <szicari@streambit.software, Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bboggs-streambit/faust-avro-model-codegen"
 
 [tool.poetry.dependencies]
```

### Comparing `faust_avro_model_codegen-0.1.6/PKG-INFO` & `faust_avro_model_codegen-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faust-avro-model-codegen
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate Faust Avro Models from Avro Schema files.
 Home-page: https://github.com/bboggs-streambit/faust-avro-model-codegen
 License: MIT
 Author: Sean Zicari
 Author-email: szicari@streambit.software, Brad Boggs <bboggs@streambit.software
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

