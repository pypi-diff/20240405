# Comparing `tmp/linkml-1.7.7.tar.gz` & `tmp/linkml-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.7.7.tar", max compression
+gzip compressed data, was "linkml-1.7.8.tar", max compression
```

## Comparing `linkml-1.7.7.tar` & `linkml-1.7.8.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0      535 2024-03-27 02:11:12.165624 linkml-1.7.7/LICENSE
--rw-r--r--   0        0        0     1369 2024-03-27 02:11:12.165624 linkml-1.7.7/README.md
--rw-r--r--   0        0        0     3327 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/__init__.py
--rw-r--r--   0        0        0      310 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/_version.py
--rw-r--r--   0        0        0    51006 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     4438 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/README.md
--rw-r--r--   0        0        0     1517 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     1956 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     2956 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     3787 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2538 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1014 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1466 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     3226 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     2665 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    34347 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5013 2024-03-27 02:11:12.185624 linkml-1.7.7/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10153 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     7696 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     5811 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/golanggen.py
--rw-r--r--   0        0        0     3437 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2151 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1729 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5324 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8644 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7728 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    27455 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/legacy/__init__.py
--rw-r--r--   0        0        0     3471 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    32926 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6450 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     7774 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    54458 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/owlgen.py
--rw-r--r--   0        0        0    14895 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/plantumlgen.py
--rw-r--r--   0        0        0     4720 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9750 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2290 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/protogen.py
--rw-r--r--   0        0        0      629 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/__init__.py
--rw-r--r--   0        0        0    19045 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/array.py
--rw-r--r--   0        0        0      721 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/black.py
--rw-r--r--   0        0        0     2681 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/build.py
--rw-r--r--   0        0        0    29809 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/pydanticgen.py
--rw-r--r--   0        0        0    19911 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/template.py
--rw-r--r--   0        0        0      443 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/attribute.py.jinja
--rw-r--r--   0        0        0      834 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/base_model.py.jinja
--rw-r--r--   0        0        0      565 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/class.py.jinja
--rw-r--r--   0        0        0      240 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/conditional_import.py.jinja
--rw-r--r--   0        0        0      338 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/enum.py.jinja
--rw-r--r--   0        0        0      385 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/footer.py.jinja
--rw-r--r--   0        0        0      945 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/imports.py.jinja
--rw-r--r--   0        0        0      438 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/module.py.jinja
--rw-r--r--   0        0        0      532 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pydanticgen/templates/validator.py.jinja
--rw-r--r--   0        0        0    52805 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2656 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0      108 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/shacl/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/shacl/ifabsent_processor.py
--rw-r--r--   0        0        0     1827 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/shacl/shacl_data_type.py
--rw-r--r--   0        0        0     8324 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9874 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6138 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      249 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2542 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1622 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9268 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    11626 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     6879 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/string_template.md
--rw-r--r--   0        0        0     2887 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4627 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     8577 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1614 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    12196 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4494 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17202 2024-03-27 02:11:12.189624 linkml-1.7.7/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5113 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/linter.py
--rw-r--r--   0        0        0    11502 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/linter/rules.py
--rw-r--r--   0        0        0       92 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     8622 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    26522 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/transformers/logical_model_transformer.py
--rw-r--r--   0        0        0      678 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/transformers/model_transformer.py
--rw-r--r--   0        0        0    17704 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5275 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/__init__.py
--rw-r--r--   0        0        0      742 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/cli_utils.py
--rw-r--r--   0        0        0     6283 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/converter.py
--rw-r--r--   0        0        0     3742 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/datautils.py
--rw-r--r--   0        0        0      472 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6912 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    38363 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/generator.py
--rw-r--r--   0        0        0      447 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5843 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0    21184 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/logictools.py
--rw-r--r--   0        0        0     9044 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4329 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9937 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    16761 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    46062 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    18447 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    17071 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2232 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1438 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/utils/validation.py
--rw-r--r--   0        0        0     5002 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/__init__.py
--rw-r--r--   0        0        0     7261 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/cli.py
--rw-r--r--   0        0        0     1165 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/__init__.py
--rw-r--r--   0        0        0     2616 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/delimited_file_loader.py
--rw-r--r--   0        0        0      809 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/json_loader.py
--rw-r--r--   0        0        0      559 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/loader.py
--rw-r--r--   0        0        0      525 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/passthrough_loader.py
--rw-r--r--   0        0        0      914 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/loaders/yaml_loader.py
--rw-r--r--   0        0        0      702 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/__init__.py
--rw-r--r--   0        0        0     2528 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/jsonschema_validation_plugin.py
--rw-r--r--   0        0        0     1985 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/pydantic_validation_plugin.py
--rw-r--r--   0        0        0     2308 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/recommended_slots_plugin.py
--rw-r--r--   0        0        0     3624 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/shacl_validation_plugin.py
--rw-r--r--   0        0        0     1548 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/plugins/validation_plugin.py
--rw-r--r--   0        0        0      870 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/report.py
--rw-r--r--   0        0        0     2732 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/validation_context.py
--rw-r--r--   0        0        0     5649 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validator/validator.py
--rw-r--r--   0        0        0      202 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validators/__init__.py
--rw-r--r--   0        0        0     7951 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4612 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    14905 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11611 2024-03-27 02:11:12.193624 linkml-1.7.7/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     7035 2024-03-27 02:11:37.645561 linkml-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     6707 1970-01-01 00:00:00.000000 linkml-1.7.7/setup.py
--rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 linkml-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0      535 2024-04-05 19:33:24.282387 linkml-1.7.8/LICENSE
+-rw-r--r--   0        0        0     1369 2024-04-05 19:33:24.282387 linkml-1.7.8/README.md
+-rw-r--r--   0        0        0     3663 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/_version.py
+-rw-r--r--   0        0        0    51006 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4438 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/README.md
+-rw-r--r--   0        0        0     1517 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     1956 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     2956 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     3787 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2538 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1014 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1466 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     3226 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     2705 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    34347 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5013 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10153 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     7696 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     5811 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3437 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2151 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1729 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5324 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8644 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7728 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    27455 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/legacy/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    32926 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6450 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7774 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    54458 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0    14895 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/plantumlgen.py
+-rw-r--r--   0        0        0     4720 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9750 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2290 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/protogen.py
+-rw-r--r--   0        0        0      629 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/pydanticgen/__init__.py
+-rw-r--r--   0        0        0    19506 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/pydanticgen/array.py
+-rw-r--r--   0        0        0      721 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/black.py
+-rw-r--r--   0        0        0     2681 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/build.py
+-rw-r--r--   0        0        0    29863 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/pydanticgen.py
+-rw-r--r--   0        0        0    19990 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/template.py
+-rw-r--r--   0        0        0      443 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/attribute.py.jinja
+-rw-r--r--   0        0        0      834 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/base_model.py.jinja
+-rw-r--r--   0        0        0      565 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/class.py.jinja
+-rw-r--r--   0        0        0      240 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/conditional_import.py.jinja
+-rw-r--r--   0        0        0      338 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/enum.py.jinja
+-rw-r--r--   0        0        0      385 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/footer.py.jinja
+-rw-r--r--   0        0        0      945 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/imports.py.jinja
+-rw-r--r--   0        0        0      438 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/module.py.jinja
+-rw-r--r--   0        0        0      532 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/validator.py.jinja
+-rw-r--r--   0        0        0    52915 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2973 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0      108 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/ifabsent_processor.py
+-rw-r--r--   0        0        0     1827 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/shacl_data_type.py
+-rw-r--r--   0        0        0     8771 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9874 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6138 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      249 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2542 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1622 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9320 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    12343 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     6879 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     2887 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4627 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     8577 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1614 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    12196 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4494 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17202 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5113 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11502 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/rules.py
+-rw-r--r--   0        0        0       92 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     8622 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    26522 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/logical_model_transformer.py
+-rw-r--r--   0        0        0      678 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/model_transformer.py
+-rw-r--r--   0        0        0    18857 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5275 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/__init__.py
+-rw-r--r--   0        0        0      742 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/cli_utils.py
+-rw-r--r--   0        0        0     6283 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/converter.py
+-rw-r--r--   0        0        0     3742 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      472 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6912 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    38394 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/generator.py
+-rw-r--r--   0        0        0      447 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5843 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0    21184 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/logictools.py
+-rw-r--r--   0        0        0     9044 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4417 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9937 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    16761 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    46093 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    18447 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    17071 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2232 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1438 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/validation.py
+-rw-r--r--   0        0        0     5002 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/__init__.py
+-rw-r--r--   0        0        0     7261 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/cli.py
+-rw-r--r--   0        0        0     1165 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/__init__.py
+-rw-r--r--   0        0        0     2616 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/delimited_file_loader.py
+-rw-r--r--   0        0        0      809 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/json_loader.py
+-rw-r--r--   0        0        0      559 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/loader.py
+-rw-r--r--   0        0        0      525 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/passthrough_loader.py
+-rw-r--r--   0        0        0      914 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/yaml_loader.py
+-rw-r--r--   0        0        0      702 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/__init__.py
+-rw-r--r--   0        0        0     2528 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/jsonschema_validation_plugin.py
+-rw-r--r--   0        0        0     1985 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/pydantic_validation_plugin.py
+-rw-r--r--   0        0        0     2308 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/recommended_slots_plugin.py
+-rw-r--r--   0        0        0     3888 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/shacl_validation_plugin.py
+-rw-r--r--   0        0        0     1548 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/validation_plugin.py
+-rw-r--r--   0        0        0      870 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/report.py
+-rw-r--r--   0        0        0     2732 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/validation_context.py
+-rw-r--r--   0        0        0     5649 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/validator.py
+-rw-r--r--   0        0        0      202 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     7951 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4612 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    14905 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11611 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     7421 2024-04-05 19:33:54.086785 linkml-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 linkml-1.7.8/setup.py
+-rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 linkml-1.7.8/PKG-INFO
```

### Comparing `linkml-1.7.7/LICENSE` & `linkml-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/README.md` & `linkml-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/__init__.py` & `linkml-1.7.8/linkml/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 
 # Local location of yaml files
 LOCAL_METAMODEL_YAML_FILE = linkml_files.LOCAL_PATH_FOR(Source.META, Format.YAML)
 LOCAL_TYPES_YAML_FILE = linkml_files.LOCAL_PATH_FOR(Source.TYPES, Format.YAML)
 LOCAL_MAPPINGS_YAML_FILE = linkml_files.LOCAL_PATH_FOR(Source.MAPPINGS, Format.YAML)
 LOCAL_ANNOTATIONS_YAML_FILE = linkml_files.LOCAL_PATH_FOR(Source.ANNOTATIONS, Format.YAML)
 LOCAL_EXTENSIONS_YAML_FILE = linkml_files.LOCAL_PATH_FOR(Source.EXTENSIONS, Format.YAML)
+LOCAL_MODEL_YAML_FILES = (
+    LOCAL_METAMODEL_YAML_FILE,
+    LOCAL_TYPES_YAML_FILE,
+    LOCAL_MAPPINGS_YAML_FILE,
+    LOCAL_ANNOTATIONS_YAML_FILE,
+    LOCAL_EXTENSIONS_YAML_FILE,
+)
 
 # Local location of jsonld and context.jsonld files
 LOCAL_METAMODEL_LDCONTEXT_FILE = linkml_files.LOCAL_PATH_FOR(Source.META, Format.JSONLD)
 LOCAL_METAMODEL_JSONLD_FILE = linkml_files.LOCAL_PATH_FOR(Source.META, Format.JSON)
 LOCAL_TYPES_LDCONTEXT_FILE = linkml_files.LOCAL_PATH_FOR(Source.TYPES, Format.JSONLD)
 LOCAL_TYPES_JSONLD_FILE = linkml_files.LOCAL_PATH_FOR(Source.TYPES, Format.JSON)
 LOCAL_MAPPINGS_LDCONTEXT_FILE = linkml_files.LOCAL_PATH_FOR(Source.MAPPINGS, Format.JSONLD)
@@ -51,14 +58,21 @@
 # Namespace for metamodel elements
 META_BASE_URI = linkml_files.LINKML_NAMESPACE
 METAMODEL_NAMESPACE = META_BASE_URI
 METATYPE_NAMESPACE = METAMODEL_NAMESPACE
 METAMAPPING_NAMESPACE = METAMODEL_NAMESPACE
 METAANNOTATIONS_NAMESPACE = METAMODEL_NAMESPACE
 METAEXTENSIONS_NAMESPACE = METAMODEL_NAMESPACE
+NAMESPACES = (
+    METAMODEL_NAMESPACE,
+    METATYPE_NAMESPACE,
+    METAMAPPING_NAMESPACE,
+    METAANNOTATIONS_NAMESPACE,
+    METAEXTENSIONS_NAMESPACE,
+)
 
 # Metamodel Context URI
 METAMODEL_CONTEXT_URI = linkml_files.URL_FOR(Source.META, Format.JSONLD)
 
 # Metamodel ShEx URI
 METAMODEL_SHEXJ_URI = linkml_files.URL_FOR(Source.META, Format.SHEXJ)
 METAMODEL_SHEXC_URI = linkml_files.URL_FOR(Source.META, Format.SHEXC)
```

### Comparing `linkml-1.7.7/linkml/generators/PythonGenNotes.md` & `linkml-1.7.8/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/README.md` & `linkml-1.7.8/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/__init__.py` & `linkml-1.7.8/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/common/type_designators.py` & `linkml-1.7.8/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/csvgen.py` & `linkml-1.7.8/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/class.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/index.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/subset.md.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -39,39 +39,39 @@
 {% endfor %}
 
 {% if classes_in_subset %}
 ## Classes in subset
 
 | Class | Description |
 | --- | --- |
-{% for c in gen.all_class_objects()|sort(attribute=sort_by) -%}
+{% for c in classes_in_subset -%}
 {%- if element.name in c.in_subset -%}
 | {{gen.link(c)}} | {{c.description|enshorten}} |
 {% endif -%}
 {% endfor %}
 
-{% for c in gen.all_class_objects()|sort(attribute=sort_by) -%}
+{% for c in classes_in_subset -%}
 {%- if element.name in c.in_subset -%}
-### {{ gen.name(c) }}
 
-{{c.description}}
+{% set induced_slots = gen.class_induced_slots(c.name)|sort(attribute=sort_by) %}
 
 {%- set filtered_slots = [] -%}
-
 {%- for s in induced_slots|sort(attribute=sort_by) -%}
     {%- if element.name in s.in_subset or element.name in schemaview.get_slot(s.name).in_subset -%}
         {% set _ = filtered_slots.append(s) %}
     {%- endif -%}
 {%- endfor %}
 
 {%- if filtered_slots|length > 0 -%}
-| Name | Cardinality and Range  | Description  |
+### Slots from {{ gen.link(c) }} also in _{{ element.name }}_
+
+| Name | Cardinality and Range | Description |
 | ---  | ---  | --- |
 {% for s in filtered_slots -%}
-| {{gen.link(s)}} | {{ gen.cardinality(s) }} <br/> {{gen.link(s.range)}}  | {{s.description|enshorten}} {% if s.identifier %}**identifier**{% endif %}  |
+| {{gen.link(s)}} | {{ gen.cardinality(s) }} <br/> {{gen.link(s.range)}} | {{s.description|enshorten}} {% if s.identifier %}**identifier**{% endif %} |
 {% endfor %}
 {%- endif %}
 
 
 {%- endif %}
 {% endfor %}
```

### Comparing `linkml-1.7.7/linkml/generators/docgen/type.md.jinja2` & `linkml-1.7.8/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/docgen.py` & `linkml-1.7.8/linkml/generators/docgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/dotgen.py` & `linkml-1.7.8/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/erdiagramgen.py` & `linkml-1.7.8/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/excelgen.py` & `linkml-1.7.8/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/golanggen.py` & `linkml-1.7.8/linkml/generators/golanggen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/golrgen.py` & `linkml-1.7.8/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/graphqlgen.py` & `linkml-1.7.8/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.7.8/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/javagen.py` & `linkml-1.7.8/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/jsonldcontextgen.py` & `linkml-1.7.8/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/jsonldgen.py` & `linkml-1.7.8/linkml/generators/jsonldgen.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     original_schema: SchemaDefinition = None
     """See https://github.com/linkml/linkml/issues/871"""
 
     context: str = None
     """Path to a JSONLD context file"""
 
     def __post_init__(self) -> None:
-        super().__post_init__()
         self.original_schema = deepcopy(self.schema)
+        super().__post_init__()
 
     def _add_type(self, node: YAMLRoot) -> dict:
         if self.format == "jsonld":
             typ = node.__class__.__name__
             node = node.__dict__
             node["@type"] = typ
         return node
```

### Comparing `linkml-1.7.7/linkml/generators/jsonschemagen.py` & `linkml-1.7.8/linkml/generators/jsonschemagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/linkmlgen.py` & `linkml-1.7.8/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/markdowngen.py` & `linkml-1.7.8/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/namespacegen.py` & `linkml-1.7.8/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/oocodegen.py` & `linkml-1.7.8/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/owlgen.py` & `linkml-1.7.8/linkml/generators/owlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/plantumlgen.py` & `linkml-1.7.8/linkml/generators/plantumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/prefixmapgen.py` & `linkml-1.7.8/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/projectgen.py` & `linkml-1.7.8/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/protogen.py` & `linkml-1.7.8/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/__init__.py` & `linkml-1.7.8/linkml/generators/pydanticgen/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/array.py` & `linkml-1.7.8/linkml/generators/pydanticgen/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 if sys.version_info.minor <= 8:
     from typing_extensions import Annotated
 else:
     from typing import Annotated
 
 from linkml.generators.pydanticgen.build import SlotResult
-from linkml.generators.pydanticgen.template import Import, Imports, ObjectImport
+from linkml.generators.pydanticgen.template import ConditionalImport, Import, Imports, ObjectImport
 
 
 class ArrayRepresentation(Enum):
     LIST = "list"
     NPARRAY = "nparray"  # numpy and nptyping must be installed to use this
 
 
@@ -50,15 +50,22 @@
             # double-nested parameterized types here
             # source_type: List[Union[T,List[...]]]
             item_type = Any if get_args(get_args(source_type)[0])[0] is _T else get_args(get_args(source_type)[0])[0]
 
             item_schema = handler.generate_schema(item_type)
             if item_schema.get("type", "any") != "any":
                 item_schema["strict"] = True
-            array_ref = f"any-shape-array-{item_type.__name__}"
+
+            if item_type is Any:
+                # Before python 3.11, `Any` type was a special object without a __name__
+                item_name = "Any"
+            else:
+                item_name = item_type.__name__
+
+            array_ref = f"any-shape-array-{item_name}"
 
             schema = core_schema.definitions_schema(
                 core_schema.list_schema(core_schema.definition_reference_schema(array_ref)),
                 [
                     core_schema.union_schema(
                         [
                             core_schema.list_schema(core_schema.definition_reference_schema(array_ref)),
@@ -74,22 +81,27 @@
     AnyShapeArray = Annotated[_RecursiveListType, AnyShapeArrayType]
 
     _AnyShapeArrayImports = (
         Imports()
         + Import(
             module="typing",
             objects=[
-                ObjectImport(name="Annotated"),
                 ObjectImport(name="Generic"),
                 ObjectImport(name="Iterable"),
                 ObjectImport(name="TypeVar"),
                 ObjectImport(name="Union"),
                 ObjectImport(name="get_args"),
             ],
         )
+        + ConditionalImport(
+            condition="sys.version_info.minor > 8",
+            module="typing",
+            objects=[ObjectImport(name="Annotated")],
+            alternative=Import(module="typing_extensions", objects=[ObjectImport(name="Annotated")]),
+        )
         + Import(module="pydantic", objects=[ObjectImport(name="GetCoreSchemaHandler")])
         + Import(module="pydantic_core", objects=[ObjectImport(name="CoreSchema"), ObjectImport(name="core_schema")])
     )
 
     # annotated types are special and inspect.getsource() can't stringify them
     _AnyShapeArrayInjects = [
         '_T = TypeVar("_T")',
```

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/black.py` & `linkml-1.7.8/linkml/generators/pydanticgen/black.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/build.py` & `linkml-1.7.8/linkml/generators/pydanticgen/build.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/pydanticgen.py` & `linkml-1.7.8/linkml/generators/pydanticgen/pydanticgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 DEFAULT_IMPORTS = (
     Imports()
     + Import(module="__future__", objects=[ObjectImport(name="annotations")])
     + Import(module="datetime", objects=[ObjectImport(name="datetime"), ObjectImport(name="date")])
     + Import(module="decimal", objects=[ObjectImport(name="Decimal")])
     + Import(module="enum", objects=[ObjectImport(name="Enum")])
     + Import(module="re")
+    + Import(module="sys")
     + Import(
         module="typing",
         objects=[
             ObjectImport(name="Any"),
             ObjectImport(name="List"),
             ObjectImport(name="Literal"),
             ObjectImport(name="Dict"),
@@ -640,18 +641,19 @@
 
         classes = {}
         predefined = self.get_predefined_slot_values()
         bases = self.get_class_isa_plus_mixins()
         for k, c in pyschema.classes.items():
             attrs = {}
             for attr_name, src_attr in c.attributes.items():
+                src_attr = src_attr._as_dict
                 new_fields = {
-                    k: src_attr._as_dict.get(k, None)
+                    k: src_attr.get(k, None)
                     for k in PydanticAttribute.model_fields.keys()
-                    if src_attr._as_dict.get(k, None) is not None
+                    if src_attr.get(k, None) is not None
                 }
                 predef_slot = predefined.get(k, {}).get(attr_name, None)
                 if predef_slot is not None:
                     predef_slot = str(predef_slot)
                 new_fields["predefined"] = predef_slot
                 new_fields["name"] = attr_name
                 attrs[attr_name] = PydanticAttribute(**new_fields, pydantic_ver=self.pydantic_version)
```

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/template.py` & `linkml-1.7.8/linkml/generators/pydanticgen/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import copy
 from importlib.util import find_spec
 from typing import Any, ClassVar, Dict, Generator, List, Literal, Optional, Union, overload
 
 from jinja2 import Environment, PackageLoader
 from pydantic import BaseModel, Field
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
@@ -50,14 +51,18 @@
         or with poetry::
 
             poetry install -E black
 
     """
 
     template: ClassVar[str]
+    _environment: ClassVar[Environment] = Environment(
+        loader=PackageLoader("linkml.generators.pydanticgen", "templates"), trim_blocks=True, lstrip_blocks=True
+    )
+
     pydantic_ver: int = int(PYDANTIC_VERSION[0])
 
     def render(self, environment: Optional[Environment] = None, black: bool = False) -> str:
         """
         Recursively render a template model to a string.
 
         For each field in the model, recurse through, rendering each :class:`.TemplateModel`
@@ -91,22 +96,19 @@
         else:
             return rendered
 
     @classmethod
     def environment(cls) -> Environment:
         """
         Default environment for Template models.
-
         uses a :class:`jinja2.PackageLoader` for the templates directory within this module
         with the ``trim_blocks`` and ``lstrip_blocks`` parameters set to ``True`` so that the
         default templates could be written in a more readable way.
         """
-        return Environment(
-            loader=PackageLoader("linkml.generators.pydanticgen", "templates"), trim_blocks=True, lstrip_blocks=True
-        )
+        return copy(cls._environment)
 
     if int(PYDANTIC_VERSION[0]) < 2:
         # simulate pydantic 2's model_fields behavior
         # without using classmethod + property decorators
         # see:
         # - https://docs.python.org/3/whatsnew/3.11.html#language-builtins
         # - https://github.com/python/cpython/issues/89519
```

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/templates/base_model.py.jinja` & `linkml-1.7.8/linkml/generators/pydanticgen/templates/base_model.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/templates/class.py.jinja` & `linkml-1.7.8/linkml/generators/pydanticgen/templates/class.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/templates/imports.py.jinja` & `linkml-1.7.8/linkml/generators/pydanticgen/templates/imports.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pydanticgen/templates/validator.py.jinja` & `linkml-1.7.8/linkml/generators/pydanticgen/templates/validator.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/pythongen.py` & `linkml-1.7.8/linkml/generators/pythongen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import keyword
 import logging
 import os
 import re
 from copy import copy
 from dataclasses import dataclass
+from pathlib import Path
 from types import ModuleType
 from typing import Callable, Dict, Iterator, List, Optional, Set, Tuple, Union
 
 import click
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import linkml_files
 from linkml_runtime.linkml_model.meta import (
@@ -58,14 +59,16 @@
     # ObjectVars
     gen_classvars: bool = True
     gen_slots: bool = True
     genmeta: bool = False
     emit_metadata: bool = True
 
     def __post_init__(self) -> None:
+        if isinstance(self.schema, Path):
+            self.schema = str(self.schema)
         self.sourcefile = self.schema
         self.schemaview = SchemaView(self.schema, base_dir=self.base_dir)
         super().__post_init__()
         if self.format is None:
             self.format = self.valid_formats[0]
         if self.schema.default_prefix == "linkml" and not self.genmeta:
             logging.error("Generating metamodel without --genmeta is highly inadvisable!")
```

### Comparing `linkml-1.7.7/linkml/generators/rdfgen.py` & `linkml-1.7.8/linkml/generators/rdfgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 Generate a JSON LD representation of the model
 
 """
 
 import os
 import urllib.parse as urlparse
+from copy import deepcopy
 from dataclasses import dataclass
 from typing import List, Optional
 
 import click
+from linkml_runtime.linkml_model import SchemaDefinition
 from rdflib import Graph
 from rdflib.plugin import Parser as rdflib_Parser
 from rdflib.plugin import plugins as rdflib_plugins
 
 from linkml import METAMODEL_CONTEXT_URI
 from linkml._version import __version__
 from linkml.generators.jsonldgen import JSONLDGenerator
@@ -31,21 +33,27 @@
     valid_formats = ["ttl"] + sorted([x.name for x in rdflib_plugins(None, rdflib_Parser) if "/" not in str(x.name)])
     visit_all_class_slots = False
     uses_schemaloader = True
 
     # ObjectVars
     emit_metadata: bool = False
     context: List[str] = None
+    original_schema: SchemaDefinition = None
+    """See https://github.com/linkml/linkml/issues/871"""
+
+    def __post_init__(self):
+        self.original_schema = deepcopy(self.schema)
+        super().__post_init__()
 
     def _data(self, g: Graph) -> str:
         return g.serialize(format="turtle" if self.format == "ttl" else self.format)
 
     def end_schema(self, output: Optional[str] = None, context: str = None, **_) -> None:
         gen = JSONLDGenerator(
-            self,
+            self.original_schema,
             format=JSONLDGenerator.valid_formats[0],
             metadata=self.emit_metadata,
             importmap=self.importmap,
         )
         # Iterate over permissible text strings making them URI compatible
         for e in gen.schema.enums.values():
             for pv in e.permissible_values.values():
```

### Comparing `linkml-1.7.7/linkml/generators/shacl/ifabsent_processor.py` & `linkml-1.7.8/linkml/generators/shacl/ifabsent_processor.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/shacl/shacl_data_type.py` & `linkml-1.7.8/linkml/generators/shacl/shacl_data_type.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/shaclgen.py` & `linkml-1.7.8/linkml/generators/shaclgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 
 @dataclass
 class ShaclGenerator(Generator):
     # ClassVars
     closed: bool = True
     """True means add 'sh:closed=true' to all shapes, except of mixin shapes and shapes, that have parents"""
-
+    suffix: str = None
+    """parameterized suffix to be appended. No suffix per default."""
     generatorname = os.path.basename(__file__)
     generatorversion = "0.0.1"
     valid_formats = ["ttl"]
     file_extension = "shacl.ttl"
     visit_all_class_slots = False
     uses_schemaloader = True
 
@@ -55,17 +56,20 @@
         for pfx in self.schema.prefixes.values():
             g.bind(str(pfx.prefix_prefix), pfx.prefix_reference)
 
         for c in sv.all_classes().values():
 
             def shape_pv(p, v):
                 if v is not None:
-                    g.add((class_uri, p, v))
+                    g.add((class_uri_with_suffix, p, v))
 
             class_uri = URIRef(sv.get_uri(c, expand=True))
+            class_uri_with_suffix = class_uri
+            if self.suffix is not None:
+                class_uri_with_suffix += self.suffix
             shape_pv(RDF.type, SH.NodeShape)
             shape_pv(SH.targetClass, class_uri)  # TODO
             if self.closed:
                 if c.mixin or c.abstract:
                     shape_pv(SH.closed, Literal(False))
                 else:
                     shape_pv(SH.closed, Literal(True))
@@ -207,22 +211,29 @@
 def add_simple_data_type(func: Callable, r: ElementName) -> None:
     for datatype in list(ShaclDataType):
         if datatype.linkml_type == r:
             func(SH.datatype, datatype.uri_ref)
 
 
 @shared_arguments(ShaclGenerator)
+@click.command()
 @click.option(
     "--closed/--non-closed",
     default=True,
     show_default=True,
     help="Use '--closed' to generate closed SHACL shapes. Use '--non-closed' to generate open SHACL shapes.",
 )
+@click.option(
+    "-s",
+    "--suffix",
+    default=None,
+    show_default=True,
+    help="Use --suffix to append given string to SHACL class name (e. g. --suffix Shape: Person becomes PersonShape).",
+)
 @click.version_option(__version__, "-V", "--version")
-@click.command()
 def cli(yamlfile, **args):
     """Generate SHACL turtle from a LinkML model"""
     gen = ShaclGenerator(yamlfile, **args)
     print(gen.serialize())
 
 
 if __name__ == "__main__":
```

### Comparing `linkml-1.7.7/linkml/generators/shexgen.py` & `linkml-1.7.8/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/sparqlgen.py` & `linkml-1.7.8/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/sqlalchemygen.py` & `linkml-1.7.8/linkml/generators/sqlalchemygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
             mappings=tr_result.mappings,
             backrefs=backrefs,
             classname=camelcase,
             no_model_import=no_model_import,
             is_join_table=lambda c: any(tag for tag in c.annotations.keys() if tag == "linkml:derived_from"),
             classes=rel_schema_classes_ordered,
         )
+        logging.debug(f"# Generated code:\n{code}")
         return code
 
     def serialize(self, **kwargs) -> str:
         return self.generate_sqla(**kwargs)
 
     def compile_sqla(
         self,
```

### Comparing `linkml-1.7.7/linkml/generators/sqltablegen.py` & `linkml-1.7.8/linkml/generators/sqltablegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,30 @@
                     )
                     if include_comments:
                         ddl_str += f"--     * Slot: {sn} Description: {strip_newlines(s.description)}\n"
                     if s.description:
                         col.comment = s.description
                     cols.append(col)
                 for uc_name, uc in c.unique_keys.items():
-                    sql_uc = UniqueConstraint(*[sql_name(sn) for sn in uc.unique_key_slots])
+
+                    def _sql_name(sn: str):
+                        if sn in c.attributes:
+                            return sql_name(sn)
+                        else:
+                            # for candidate in c.attributes.values():
+                            #    if "original_slot" in candidate.annotations:
+                            #        original = candidate.annotations["original_slot"]
+                            #        if original.value == sn:
+                            #            return sql_name(candidate.name)
+                            return None
+
+                    sql_names = [_sql_name(sn) for sn in uc.unique_key_slots]
+                    if any(sn is None for sn in sql_names):
+                        continue
+                    sql_uc = UniqueConstraint(*sql_names)
                     cols.append(sql_uc)
                 Table(sql_name(cn), schema_metadata, *cols, comment=str(c.description))
         schema_metadata.create_all(engine)
         return ddl_str
 
     def get_sql_range(self, slot: SlotDefinition, schema: SchemaDefinition = None):
         """
```

### Comparing `linkml-1.7.7/linkml/generators/sssomgen.py` & `linkml-1.7.8/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/string_template.md` & `linkml-1.7.8/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/summarygen.py` & `linkml-1.7.8/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/terminusdbgen.py` & `linkml-1.7.8/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/typescriptgen.py` & `linkml-1.7.8/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/yamlgen.py` & `linkml-1.7.8/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/generators/yumlgen.py` & `linkml-1.7.8/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/cli.py` & `linkml-1.7.8/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/config/datamodel/config.py` & `linkml-1.7.8/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/config/datamodel/config.yaml` & `linkml-1.7.8/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/config/default.yaml` & `linkml-1.7.8/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/formatters/formatter.py` & `linkml-1.7.8/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/formatters/json_formatter.py` & `linkml-1.7.8/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.7.8/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.7.8/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.7.8/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/linter.py` & `linkml-1.7.8/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/linter/rules.py` & `linkml-1.7.8/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/reporting/model.py` & `linkml-1.7.8/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/transformers/logical_model_transformer.py` & `linkml-1.7.8/linkml/transformers/logical_model_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/transformers/model_transformer.py` & `linkml-1.7.8/linkml/transformers/model_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/transformers/relmodel_transformer.py` & `linkml-1.7.8/linkml/transformers/relmodel_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,15 @@
                     logging.info(f"Added primary key {cn}.{pk.name}")
                 for link in links:
                     if link.target_class == cn:
                         link.target_slot = pk.name
 
         # TODO: separate out the logic into separate testable methods
         target_sv.set_modified()
+        multivalued_slots_original = []
         # post-process target schema
         for cn, c in target_sv.all_classes().items():
             if self.foreign_key_policy == ForeignKeyPolicy.NO_FOREIGN_KEYS:
                 continue
             pk_slot = self.get_direct_identifier_attribute(target_sv, cn)
             # if self.is_skip(c) and len(incoming_links) == 0:
             #    logging.info(f'Skipping class: {c.name}')
@@ -239,14 +240,15 @@
                 slot = copy(src_slot)
                 slot_range = slot.range
                 slot_range_is_class = slot_range in target_sv.all_classes()
                 is_shared = slot_range_is_class and (
                     slot.inlined or slot.inlined_as_list or "shared" in slot.annotations
                 )
                 if slot.multivalued:
+                    multivalued_slots_original.append(slot.name)
                     slot.multivalued = False
                     slot_name = slot.name
                     sn_singular = slot.singular_name if slot.singular_name else slot.name
                     if pk_slot is None:
                         pk_slot = self.add_primary_key(c.name, target_sv)
                     backref_slot = SlotDefinition(
                         name=f"{c.name}_{pk_slot.name}",
@@ -328,14 +330,15 @@
                     del c.attributes[slot_name]
                     target_sv.set_modified()
             target.classes[c.name] = c
 
         # add PK and FK anns
         target_sv.set_modified()
         fk_policy = self.foreign_key_policy
+        forward_map = {}
         for c in target.classes.values():
             if self.foreign_key_policy == ForeignKeyPolicy.NO_FOREIGN_KEYS:
                 continue
             pk_slot = target_sv.get_identifier_slot(c.name)
             for a in list(c.attributes.values()):
                 if pk_slot is None or a.name == pk_slot.name:
                     ann = Annotation("primary_key", "true")
@@ -352,22 +355,39 @@
                     is_inlined = a.inlined or not source_sv.get_identifier_slot(tc.name)
                     if (fk_policy == ForeignKeyPolicy.INJECT_FK_FOR_NESTED and is_inlined and not a.multivalued) or (
                         fk_policy == ForeignKeyPolicy.INJECT_FK_FOR_ALL_REFS
                     ):
                         # if it is already an injected backref, no need to re-inject
                         if "backref" not in a.annotations:
                             del c.attributes[a.name]
+                            original_name = a.name
                             if "forwardref" not in a.annotations:
-                                add_annotation(a, "original_slot", a.name)
+                                add_annotation(a, "original_slot", original_name)
                             a.alias = f"{a.name}_{tc_pk_slot.name}"
                             a.name = a.alias
                             c.attributes[a.name] = a
+                            forward_map[original_name] = a.name
                     ann = Annotation("foreign_key", f"{tc.name}.{tc_pk_slot.name}")
                     a.annotations[ann.tag] = ann
                     target_sv.set_modified()
+            # Rewrite unique key constraints
+            # - if a slot has a range of object, it may be renamed, e.g. person => person_id
+            # - if a slot is multivalued then it is translated to backref and the UC must be dropped
+            removed_ucs = []
+            for uc_name, uc in c.unique_keys.items():
+                if any(sn in multivalued_slots_original for sn in uc.unique_key_slots):
+                    logging.warning(
+                        f"Cannot represent uniqueness constraint {uc_name}. "
+                        f"one of the slots {uc.unique_key_slots} is multivalued"
+                    )
+                    removed_ucs.append(uc_name)
+                new_slot_names = [forward_map.get(sn, sn) for sn in uc.unique_key_slots]
+                uc.unique_key_slots = new_slot_names
+            for uc_name in removed_ucs:
+                del c.unique_keys[uc_name]
 
         result = TransformationResult(target, mappings=mappings)
         return result
 
     @staticmethod
     def get_direct_identifier_attribute(sv: SchemaView, cn: ClassDefinitionName) -> Optional[SlotDefinition]:
         c = sv.get_class(cn)
```

### Comparing `linkml-1.7.7/linkml/transformers/schema_renamer.py` & `linkml-1.7.8/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/cli_utils.py` & `linkml-1.7.8/linkml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/converter.py` & `linkml-1.7.8/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/datautils.py` & `linkml-1.7.8/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/execute_tutorial.py` & `linkml-1.7.8/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/generator.py` & `linkml-1.7.8/linkml/utils/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from io import StringIO
 from pathlib import Path
 from typing import Callable, ClassVar, Dict, List, Mapping, Optional, Set, TextIO, Type, Union, cast
 
 import click
 from click import Argument, Command, Option
 from linkml_runtime import SchemaView
-from linkml_runtime.dumpers import yaml_dumper
 from linkml_runtime.linkml_model.meta import (
     ClassDefinition,
     ClassDefinitionName,
     Definition,
     Element,
     ElementName,
     EnumDefinition,
@@ -79,15 +78,15 @@
 class Generator(metaclass=abc.ABCMeta):
     """
     Base class for generators
 
     For usage `Generator Docs <https://linkml.io/linkml/generators/>`_
     """
 
-    schema: Union[str, TextIO, SchemaDefinition, "Generator"]
+    schema: Union[str, TextIO, SchemaDefinition, "Generator", Path]
     """metamodel compliant schema.  Can be URI, file name, actual schema, another generator, an
         open file or a pre-parsed schema"""
 
     # ClassVars
     generatorname: ClassVar[str] = None
     """ Name of the generator. Override with os.path.basename(__file__)"""
 
@@ -126,15 +125,15 @@
 
     metadata: bool = True
     """True means include date, generator, etc. information in source header if appropriate"""
 
     useuris: Optional[bool] = None
     """True means declared class slot uri's are used.  False means use model uris"""
 
-    log_level: int = DEFAULT_LOG_LEVEL_INT
+    log_level: Optional[int] = DEFAULT_LOG_LEVEL_INT
     """Logging level, 0 is minimum"""
 
     mergeimports: Optional[bool] = True
     """True means merge non-linkml sources into importing package.  False means separate packages"""
 
     source_file_date: Optional[str] = None
     """Modification date of input source file"""
@@ -176,26 +175,32 @@
 
     stacktrace: bool = False
     """True means print stack trace, false just error message"""
 
     def __post_init__(self) -> None:
         if not self.logger:
             self.logger = logging.getLogger()
+        if self.log_level is not None:
+            self.logger.setLevel(self.log_level)
         if self.format is None:
             self.format = self.valid_formats[0]
         if self.format not in self.valid_formats:
             raise ValueError(f"Unrecognized format: {format}; known={self.valid_formats}")
         # legacy: all generators should use "mergeimports"
         # self.merge_imports = self.mergeimports
         if not self.metadata:
             self.source_file_date = None
             self.source_file_size = None
         if self.requires_metamodel:
             self.metamodel = _resolved_metamodel(self.mergeimports)
+
         schema = self.schema
+        if isinstance(schema, Path):
+            schema = str(schema)
+
         # TODO: remove aliasing
         self.emit_metadata = self.metadata
         if self.uses_schemaloader:
             self._initialize_using_schemaloader(schema)
         else:
             logging.info(f"Using SchemaView with im={self.importmap} // base_dir={self.base_dir}")
             self.schemaview = SchemaView(schema, importmap=self.importmap, base_dir=self.base_dir)
@@ -221,16 +226,15 @@
             self.schema_defaults = gen.schema_defaults
             self.logger = gen.logger
         else:
             if isinstance(schema, SchemaDefinition):
                 # schemaloader based methods require schemas to have been created via SchemaLoader,
                 # which prepopulates some fields (e.g. definition_url). If the schema has not been processed through the
                 # loader, then roundtrip
-                if any(c for c in schema.classes.values() if not c.definition_uri):
-                    schema = yaml_dumper.dumps(schema)
+                schema = schema._as_dict
             loader = SchemaLoader(
                 schema,
                 self.base_dir,
                 useuris=self.useuris,
                 importmap=self.importmap,
                 logger=self.logger,
                 mergeimports=self.mergeimports,
```

### Comparing `linkml-1.7.7/linkml/utils/ifabsent_functions.py` & `linkml-1.7.8/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/logictools.py` & `linkml-1.7.8/linkml/utils/logictools.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/mergeutils.py` & `linkml-1.7.8/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/rawloader.py` & `linkml-1.7.8/linkml/utils/rawloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 from datetime import datetime
+from pathlib import Path
 from typing import Optional, TextIO, Union
 from urllib.parse import urlparse
 
 import yaml
 from dateutil.parser import ParserError, parse
 from hbreader import FileInfo, HBType, detect_type
 from linkml_runtime.linkml_model.meta import SchemaDefinition, metamodel_version
@@ -25,15 +26,15 @@
         YAMLRoot.MissingRequiredField(self, f"{type(self).__name__}.{field_name}")
 
 
 SchemaDefinition.MissingRequiredField = mrf
 
 
 def load_raw_schema(
-    data: Union[str, dict, TextIO],
+    data: Union[str, dict, TextIO, Path],
     source_file: Optional[str] = None,
     source_file_date: Optional[str] = None,
     source_file_size: Optional[int] = None,
     base_dir: Optional[str] = None,
     merge_modules: Optional[bool] = True,
     emit_metadata: Optional[bool] = True,
 ) -> SchemaDefinition:
@@ -54,14 +55,17 @@
 
     # Passing a URL or file name
     if detect_type(data, base_dir) not in (HBType.STRING, HBType.STRINGABLE):
         assert source_file is None, "source_file parameter not allowed if data is a file or URL"
         assert source_file_date is None, "source_file_date parameter not allowed if data is a file or URL"
         assert source_file_size is None, "source_file_size parameter not allowed if data is a file or URL"
 
+    if isinstance(data, Path):
+        data = str(data)
+
     # Convert the input into a valid SchemaDefinition
     if isinstance(data, (str, dict, TextIO)):
         # TODO: Build a generic loader that detects type from suffix or content and invokes the appropriate loader
         schema_metadata = FileInfo()
         schema_metadata.source_file = source_file
         schema_metadata.source_file_date = source_file_date
         schema_metadata.source_file_size = source_file_size
```

### Comparing `linkml-1.7.7/linkml/utils/schema_builder.py` & `linkml-1.7.8/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/schema_fixer.py` & `linkml-1.7.8/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/schemaloader.py` & `linkml-1.7.8/linkml/utils/schemaloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 from collections import OrderedDict
 from copy import deepcopy
+from pathlib import Path
 from typing import Dict, Iterator, List, Mapping, Optional, Set, TextIO, Tuple, Union, cast
 from urllib.parse import urlparse
 
 from jsonasobj2 import values
 from linkml_runtime.linkml_model.meta import (
     ClassDefinition,
     ClassDefinitionName,
@@ -28,15 +29,15 @@
 from linkml.utils.rawloader import load_raw_schema
 from linkml.utils.schemasynopsis import SchemaSynopsis
 
 
 class SchemaLoader:
     def __init__(
         self,
-        data: Union[str, TextIO, SchemaDefinition, dict],
+        data: Union[str, TextIO, SchemaDefinition, dict, Path],
         base_dir: Optional[str] = None,
         namespaces: Optional[Namespaces] = None,
         useuris: Optional[bool] = None,
         importmap: Optional[Mapping[str, str]] = None,
         logger: Optional[logging.Logger] = None,
         mergeimports: Optional[bool] = True,
         emit_metadata: Optional[bool] = True,
```

### Comparing `linkml-1.7.7/linkml/utils/schemasynopsis.py` & `linkml-1.7.8/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/sqlutils.py` & `linkml-1.7.8/linkml/utils/sqlutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,24 +54,30 @@
     The wrapper transparently will take care of:
 
     - mapping your LinkML schema into SQL Tables
     - creating a SQL Alchemy ORM layer
     - mapping your data/objects in any LinkML compliant data format (json. yaml, rdf) into ORM objects
     """
 
-    schema: Union[str, SchemaDefinition] = None
-    schemaview: SchemaView = None
-    engine: Engine = None
-    database_path: str = None
+    schema: Optional[Union[str, Path, SchemaDefinition]] = None
+    schemaview: Optional[SchemaView] = None
+    engine: Optional[Engine] = None
+    database_path: Union[str, Path] = None
     use_memory: bool = False
     """https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#using-a-memory-database-in-multiple-threads"""
 
-    module: ModuleType = None
-    native_module: ModuleType = None
-    include_schema_in_database: bool = None
+    module: Optional[ModuleType] = None
+    native_module: Optional[ModuleType] = None
+    include_schema_in_database: bool = False
+
+    def __post_init__(self):
+        if self.database_path is None and not self.use_memory:
+            raise ValueError("Must have database path or use_memory must be True")
+        if self.schema is not None and self.schemaview is None:
+            self.schemaview = SchemaView(self.schema)
 
     def db_exists(self, create=True, force=False) -> Optional[str]:
         """
         check if database exists, optionally create if not present
 
         :param create: create if does not exist
         :param force: recreate database, destroying any content if previously present
@@ -113,16 +119,14 @@
 
         Note that the SQLA model is different from the native dataclass model
 
         :return: compiled module
         """
         gen = SQLAlchemyGenerator(self.schema)
         self.module = gen.compile_sqla(template=TemplateEnum.DECLARATIVE)
-        if self.schemaview is None:
-            self.schemaview = SchemaView(self.schema)
         return self.module
 
     def compile_native(self) -> ModuleType:
         """
         Compile native python object model
 
         :return: compiled module
@@ -219,30 +223,27 @@
             for k, v in vars(obj).items():
                 v2 = self.to_sqla(v)
                 if v2 is not None:
                     inst_args[k] = v2
             for n, nu_typ in inspect.getmembers(self.module):
                 # TODO: make more efficient
                 if n == typ.__name__:
-                    # print(f'Creating {nu_typ} from: {inst_args}')
                     nu_obj = nu_typ(**inst_args)
                     return nu_obj
             raise ValueError(f"Cannot find {typ.__name__} in {self.module}")
         else:
             return obj
 
     def from_sqla(self, obj: Any) -> Optional[Union[YAMLRoot, List[YAMLRoot]]]:
         """
         Translate from SQLAlchemy declarative module to native LinkML
 
         :param obj: sqla object
         :return: native dataclass object
         """
-        if self.schemaview is None:
-            self.schemaview = SchemaView(self.schema)
         typ = type(obj)
         nm = self.schemaview.class_name_mappings()
         if typ.__name__ in nm:
             cls = nm[typ.__name__]
         else:
             cls = None
         if isinstance(obj, list) or isinstance(obj, _AssociationCollection):
@@ -258,17 +259,15 @@
                 v = getattr(obj, sn, None)
                 v2 = self.from_sqla(v)
                 if v2 is not None and v2 != [] and v2 != {}:
                     inst_args[sn] = v2
             for n, nu_typ in inspect.getmembers(self.native_module):
                 # TODO: make more efficient
                 if n == typ.__name__:
-                    # print(f'CREATING {nu_typ} FROM {inst_args}')
                     nu_obj = nu_typ(**inst_args)
-                    # print(f'CREATED {nu_obj}')
                     return nu_obj
             raise ValueError(f"Cannot find {typ.__name__} in {self.native_module}")
         else:
             return obj
 
 
 @click.group()
```

### Comparing `linkml-1.7.7/linkml/utils/typereferences.py` & `linkml-1.7.8/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/utils/validation.py` & `linkml-1.7.8/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/__init__.py` & `linkml-1.7.8/linkml/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/cli.py` & `linkml-1.7.8/linkml/validator/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/__init__.py` & `linkml-1.7.8/linkml/validator/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/delimited_file_loader.py` & `linkml-1.7.8/linkml/validator/loaders/delimited_file_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/json_loader.py` & `linkml-1.7.8/linkml/validator/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/loader.py` & `linkml-1.7.8/linkml/validator/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/passthrough_loader.py` & `linkml-1.7.8/linkml/validator/loaders/passthrough_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/loaders/yaml_loader.py` & `linkml-1.7.8/linkml/validator/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/plugins/__init__.py` & `linkml-1.7.8/linkml/validator/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/plugins/jsonschema_validation_plugin.py` & `linkml-1.7.8/linkml/validator/plugins/jsonschema_validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/plugins/pydantic_validation_plugin.py` & `linkml-1.7.8/linkml/validator/plugins/pydantic_validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/plugins/recommended_slots_plugin.py` & `linkml-1.7.8/linkml/validator/plugins/recommended_slots_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/plugins/shacl_validation_plugin.py` & `linkml-1.7.8/linkml/validator/plugins/shacl_validation_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,29 +30,35 @@
         closed: bool = False,
         shacl_path: Optional[os.PathLike] = None,
         raise_on_conversion_error: bool = False,
     ) -> None:
         self.closed = closed
         self.shacl_path = shacl_path
         self.raise_on_conversion_error = raise_on_conversion_error
+        self._loaded_graphs = {}
 
     def _shacl_graph(self, context: ValidationContext) -> Optional[rdflib.Graph]:
         g = rdflib.Graph()
         if self.shacl_path:
             g.parse(str(self.shacl_path))
         else:
-            gen = ShaclGenerator(context._schema)
-            g = gen.as_graph()
+            schema_hash = hash(str(context._schema))
+            if schema_hash in self._loaded_graphs:
+                g = self._loaded_graphs[schema_hash]
+            else:
+                gen = ShaclGenerator(context._schema)
+                g = gen.as_graph()
+                self._loaded_graphs[schema_hash] = g
         return g
 
     def process(self, instance: Any, context: ValidationContext) -> Iterator[ValidationResult]:
-        """Perform JSON Schema validation on the provided instance
+        """Perform SHACL Schema validation on the provided instance
 
         :param instance: The instance to validate
-        :param context: The validation context which provides a JSON Schema artifact
+        :param context: The validation context which provides a SHACL artifact
         :return: Iterator over validation results
         :rtype: Iterator[ValidationResult]
         """
         import pyshacl
 
         shacl_graph = self._shacl_graph(context)
         if isinstance(instance, dict):
```

### Comparing `linkml-1.7.7/linkml/validator/plugins/validation_plugin.py` & `linkml-1.7.8/linkml/validator/plugins/validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/report.py` & `linkml-1.7.8/linkml/validator/report.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/validation_context.py` & `linkml-1.7.8/linkml/validator/validation_context.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validator/validator.py` & `linkml-1.7.8/linkml/validator/validator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validators/jsonschemavalidator.py` & `linkml-1.7.8/linkml/validators/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/validators/sparqlvalidator.py` & `linkml-1.7.8/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.7.8/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.7.8/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/linkml/workspaces/example_runner.py` & `linkml-1.7.8/linkml/workspaces/example_runner.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.7/pyproject.toml` & `linkml-1.7.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.7.7"
+version = "1.7.8"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -120,29 +120,24 @@
 pyyaml = "*"
 rdflib = ">=6.0.0"
 requests = ">=2.22"
 sqlalchemy = ">=1.4.31"
 watchdog = ">=0.9.0"
 pyshacl = { version = "^0.25.0", optional = true }
 black = { version=">=24.0.0", optional = true }
+typing-extensions = { version=">=4.4.0", python="<3.9" }
 
 [tool.poetry.group.dev.dependencies]
 chardet = "*"
 ipykernel = "*"
 ipython-genutils = "*"
 nbconvert = "*"
 nbformat = "*"
 coverage = "^6.4.1"
 tox = "^4"
-furo = {version = "^2023.03.27", extras = ["docs"]}
-sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
-sphinx = "*"
-sphinx-click = "*"
-sphinx-rtd-theme = "*"
-myst-parser = "*"
 requests-cache = "^1.2.0"
 myst-nb = {version=">=1.0.0", python=">=3.9"}
 sphinx-design = "^0.5.0"
 rich = "^13.7.1"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.4.0"
@@ -153,14 +148,25 @@
 ]
 
 [tool.poetry.extras]
 black = ["black"]
 shacl = ["pyshacl"]
 tests = ["black", "pyshacl"]
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+furo = {version = "^2023.03.27", extras = ["docs"]}
+sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
+sphinx = "*"
+sphinx-click = "*"
+sphinx-rtd-theme = "*"
+myst-parser = "*"
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.codespell]
 # TODO: bring in tests in too
 skip = '.git,*.pdf,*.svg,./tests,pyproject.toml,*.dill,poetry.lock'
@@ -189,15 +195,17 @@
 [tool.pytest.ini_options]
 filterwarnings = [
   # https://github.com/RDFLib/rdflib/issues/1830
   "ignore:.*_pytestfixturefunction is not defined in namespace:UserWarning"
 ]
 markers = [
   "network: mark tests that make external network requests",
-  "slow: mark test as slow to run"
+  "slow: mark test as slow to run",
+  "no_asserts: tests that don't have meaningful asserts, but are only snapshot comparisons, or historically had print statements, or other non-erroring behavior",
+  "strcmp: tests that compare stringified values rather than the values themselves"
 ]
 
 [tool.ruff]
 extend-exclude = [
     "tests/output",
     "tests/**/output",
     "tests/**/__snapshots__",
```

### Comparing `linkml-1.7.7/setup.py` & `linkml-1.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,16 @@
  'pyyaml',
  'rdflib>=6.0.0',
  'requests>=2.22',
  'sqlalchemy>=1.4.31',
  'watchdog>=0.9.0']
 
 extras_require = \
-{'black': ['black>=24.0.0'],
+{':python_version < "3.9"': ['typing-extensions>=4.4.0'],
+ 'black': ['black>=24.0.0'],
  'shacl': ['pyshacl>=0.25.0,<0.26.0'],
  'tests': ['pyshacl>=0.25.0,<0.26.0', 'black>=24.0.0']}
 
 entry_points = \
 {'console_scripts': ['gen-csv = linkml.generators.csvgen:cli',
                      'gen-doc = linkml.generators.docgen:cli',
                      'gen-erdiagram = linkml.generators.erdiagramgen:cli',
@@ -109,15 +110,15 @@
                      'linkml.validators.sparqlvalidator:cli',
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = linkml.validator.cli:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.7.7',
+    'version': '1.7.8',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.7.7/PKG-INFO` & `linkml-1.7.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.7.7
+Version: 1.7.8
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,15 @@
 Requires-Dist: pyshex (>=0.7.20)
 Requires-Dist: pyshexc (>=0.8.3)
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 Requires-Dist: rdflib (>=6.0.0)
 Requires-Dist: requests (>=2.22)
 Requires-Dist: sqlalchemy (>=1.4.31)
+Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.9"
 Requires-Dist: watchdog (>=0.9.0)
 Project-URL: Documentation, https://linkml.io/linkml/
 Project-URL: Repository, https://github.com/linkml/linkml
 Description-Content-Type: text/markdown
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)
 ![](https://github.com/linkml/linkml/workflows/Build/badge.svg)
```

