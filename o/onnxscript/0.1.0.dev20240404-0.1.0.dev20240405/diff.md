# Comparing `tmp/onnxscript-0.1.0.dev20240404.tar.gz` & `tmp/onnxscript-0.1.0.dev20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240404.tar", last modified: Thu Apr  4 00:01:08 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240405.tar", last modified: Fri Apr  5 00:00:48 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240404.tar` & `onnxscript-0.1.0.dev20240405.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.737373 onnxscript-0.1.0.dev20240404/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-04 00:01:08.737373 onnxscript-0.1.0.dev20240404/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.681373 onnxscript-0.1.0.dev20240404/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.681373 onnxscript-0.1.0.dev20240404/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.681373 onnxscript-0.1.0.dev20240404/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.681373 onnxscript-0.1.0.dev20240404/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.677372 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.681373 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.697373 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.677372 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.677372 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.697373 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.701372 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43786 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.705373 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.705373 onnxscript-0.1.0.dev20240404/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15508 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43700 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.705373 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.721373 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/onnx_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tensor.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11925 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/testing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.721373 onnxscript-0.1.0.dev20240404/onnxscript/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.721373 onnxscript-0.1.0.dev20240404/onnxscript/tests/common/
--rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12891 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/common/testutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.677372 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.725373 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/error_reproduction.py
--rw-r--r--   0 vsts      (1001) docker     (127)    79029 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23392 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   102066 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.725373 onnxscript-0.1.0.dev20240404/onnxscript/tests/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      993 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/functions/ort_custom_ops.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.737373 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/attrref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2349 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1140 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/eg1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4713 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/getitem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2025 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1569 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/identity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/m1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2907 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4969 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2564 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/renaming.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/sequences.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13534 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1432 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/tests/models/type_double.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/type_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 00:01:08.737373 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-04 00:01:08.000000 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7933 2024-04-04 00:01:08.000000 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 00:01:08.000000 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-04 00:01:08.000000 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-04 00:01:08.000000 onnxscript-0.1.0.dev20240404/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     5060 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-04 00:01:08.737373 onnxscript-0.1.0.dev20240404/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-04 00:00:49.000000 onnxscript-0.1.0.dev20240404/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43786 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15508 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tensor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11925 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/testing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/
+-rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12891 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/testutils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/error_reproduction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    79029 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23392 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   102066 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      993 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/ort_custom_ops.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2349 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1140 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4713 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2025 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1569 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/identity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/m1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2907 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4969 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2564 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13534 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1432 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/type_annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7933 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     5060 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240404/LICENSE` & `onnxscript-0.1.0.dev20240405/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/PKG-INFO` & `onnxscript-0.1.0.dev20240405/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240404
+Version: 0.1.0.dev20240405
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240404/README.md` & `onnxscript-0.1.0.dev20240405/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240405/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240405/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240405/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240405/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240405/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/main.py` & `onnxscript-0.1.0.dev20240405/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240405/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240405/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/testing.py` & `onnxscript-0.1.0.dev20240405/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/error_reproduction.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/error_reproduction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/attrref.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/cast_like.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/different_opset.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/dropout.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/eager_op.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/eg1.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/getitem.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/graph_attr.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/identity.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/if_statement.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/loops_break.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/loops_while.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns1.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/onnxfns2.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/opt_input.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/opt_output.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/renaming.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/sequences.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/signal_dft.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/subfunction.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/tests/models/type_double.py` & `onnxscript-0.1.0.dev20240405/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240405/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript/values.py` & `onnxscript-0.1.0.dev20240405/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240405/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240404
+Version: 0.1.0.dev20240405
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240404/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240405/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/pyproject.toml` & `onnxscript-0.1.0.dev20240405/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240404/setup.py` & `onnxscript-0.1.0.dev20240405/setup.py`

 * *Files identical despite different names*

