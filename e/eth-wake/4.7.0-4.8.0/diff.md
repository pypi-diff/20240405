# Comparing `tmp/eth_wake-4.7.0.tar.gz` & `tmp/eth_wake-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_wake-4.7.0.tar", max compression
+gzip compressed data, was "eth_wake-4.8.0.tar", max compression
```

## Comparing `eth_wake-4.7.0.tar` & `eth_wake-4.8.0.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0      751 2024-03-16 09:49:50.662695 eth_wake-4.7.0/LICENSE
--rw-r--r--   0        0        0     9113 2024-03-16 09:49:50.662695 eth_wake-4.7.0/README.md
--rw-r--r--   0        0        0       61 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/.gitignore
--rw-r--r--   0        0        0      431 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/README.md
--rw-r--r--   0        0        0     1198 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/contracts/Counter.sol
--rw-r--r--   0        0        0      622 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/contracts/Gateway.sol
--rw-r--r--   0        0        0      307 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/contracts/Imports.sol
--rw-r--r--   0        0        0      215 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/hardhat.config.js
--rw-r--r--   0        0        0      813 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/package-lock.json
--rw-r--r--   0        0        0       97 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/package.json
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/scripts/__init__.py
--rw-r--r--   0        0        0      350 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/scripts/deploy.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/tests/__init__.py
--rw-r--r--   0        0        0     3559 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/tests/test_counter.py
--rw-r--r--   0        0        0     1815 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/tests/test_counter_fuzz.py
--rw-r--r--   0        0        0     1170 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/tests/test_counter_fuzz_failing.py
--rw-r--r--   0        0        0     3404 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/tests/test_crosschain.py
--rw-r--r--   0        0        0       24 2024-03-16 09:49:50.686695 eth_wake-4.7.0/examples/counter/wake.toml
--rw-r--r--   0        0        0     3404 2024-03-16 09:49:50.690696 eth_wake-4.7.0/pyproject.toml
--rw-r--r--   0        0        0      355 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/__init__.py
--rw-r--r--   0        0        0       25 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/__init__.py
--rw-r--r--   0        0        0    37717 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/cfg.py
--rw-r--r--   0        0        0     7500 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/expressions.py
--rw-r--r--   0        0        0     2353 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/graph.py
--rw-r--r--   0        0        0     1543 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/interface.py
--rw-r--r--   0        0        0    16505 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/ownable.py
--rw-r--r--   0        0        0     1093 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/proxy.py
--rw-r--r--   0        0        0     7416 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/analysis/utils.py
--rw-r--r--   0        0        0       38 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/__init__.py
--rw-r--r--   0        0        0     6239 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/__main__.py
--rw-r--r--   0        0        0     8068 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/accounts.py
--rw-r--r--   0        0        0     8674 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/compile.py
--rw-r--r--   0        0        0       54 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/console.py
--rw-r--r--   0        0        0    30671 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/detect.py
--rw-r--r--   0        0        0    24955 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/init.py
--rw-r--r--   0        0        0     1298 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/lsp.py
--rw-r--r--   0        0        0     8269 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/open.py
--rw-r--r--   0        0        0     5495 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/param_types.py
--rw-r--r--   0        0        0    23532 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/print.py
--rw-r--r--   0        0        0     3583 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/run.py
--rw-r--r--   0        0        0     5877 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/svm.py
--rw-r--r--   0        0        0     9541 2024-03-16 09:49:50.690696 eth_wake-4.7.0/wake/cli/test.py
--rw-r--r--   0        0        0      187 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/__init__.py
--rw-r--r--   0        0        0     4929 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/build_data_model.py
--rw-r--r--   0        0        0     3120 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/compilation_unit.py
--rw-r--r--   0        0        0    53031 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/compiler.py
--rw-r--r--   0        0        0       97 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8831 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     9163 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3597 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4912 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/config/__init__.py
--rw-r--r--   0        0        0    11941 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/config/data_model.py
--rw-r--r--   0        0        0    15443 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/config/wake_config.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/contracts/__init__.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/contracts/wake/__init__.py
--rw-r--r--   0        0        0    64087 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/contracts/wake/console.sol
--rw-r--r--   0        0        0       32 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/__init__.py
--rw-r--r--   0        0        0      408 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/enums.py
--rw-r--r--   0        0        0      640 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/logging.py
--rw-r--r--   0        0        0     3614 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/lsp_provider.py
--rw-r--r--   0        0        0    29888 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/solidity_version.py
--rw-r--r--   0        0        0    27317 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/visitor.py
--rw-r--r--   0        0        0     1793 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/core/wake_comments.py
--rw-r--r--   0        0        0      734 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/deployment/__init__.py
--rw-r--r--   0        0        0    14991 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/deployment/core.py
--rw-r--r--   0        0        0      141 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/detectors/__init__.py
--rw-r--r--   0        0        0    29429 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/detectors/api.py
--rw-r--r--   0        0        0      649 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/detectors/template.py
--rw-r--r--   0        0        0     7760 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/detectors/utils.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/__init__.py
--rw-r--r--   0        0        0     4552 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/blocks.py
--rw-r--r--   0        0        0    50133 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/call_trace.py
--rw-r--r--   0        0        0    29599 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/chain_interfaces.py
--rw-r--r--   0        0        0     1320 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/constants.py
--rw-r--r--   0        0        0   109991 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/core.py
--rw-r--r--   0        0        0     8429 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/globals.py
--rw-r--r--   0        0        0   161115 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/hardhat_console.py
--rw-r--r--   0        0        0     1267 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/internal.py
--rw-r--r--   0        0        0       39 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2092 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      825 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/http.py
--rw-r--r--   0        0        0     2912 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      668 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/json_rpc/websocket.py
--rw-r--r--   0        0        0    14876 2024-03-16 09:49:50.694696 eth_wake-4.7.0/wake/development/primitive_types.py
--rw-r--r--   0        0        0    96402 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/development/pytypes_generator.py
--rw-r--r--   0        0        0    29435 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/development/transactions.py
--rw-r--r--   0        0        0    45433 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/development/utils.py
--rw-r--r--   0        0        0     4197 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/__init__.py
--rw-r--r--   0        0        0     4947 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/abc.py
--rw-r--r--   0        0        0    39042 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/ast.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/__init__.py
--rw-r--r--   0        0        0     5827 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/abc.py
--rw-r--r--   0        0        0    19160 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/contract_definition.py
--rw-r--r--   0        0        0     4102 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/enum_definition.py
--rw-r--r--   0        0        0     2047 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/enum_value.py
--rw-r--r--   0        0        0     5380 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/error_definition.py
--rw-r--r--   0        0        0     6611 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/event_definition.py
--rw-r--r--   0        0        0    20351 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/function_definition.py
--rw-r--r--   0        0        0    14120 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/modifier_definition.py
--rw-r--r--   0        0        0     4401 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/struct_definition.py
--rw-r--r--   0        0        0     3662 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    20534 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/declarations/variable_declaration.py
--rw-r--r--   0        0        0    11238 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/enums.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/__init__.py
--rw-r--r--   0        0        0     8026 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/abc.py
--rw-r--r--   0        0        0     5988 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/assignment.py
--rw-r--r--   0        0        0     4316 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/binary_operation.py
--rw-r--r--   0        0        0     2627 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/conditional.py
--rw-r--r--   0        0        0     2001 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/elementary_type_name_expression.py
--rw-r--r--   0        0        0    11941 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/function_call.py
--rw-r--r--   0        0        0     3383 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/function_call_options.py
--rw-r--r--   0        0        0     9399 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/identifier.py
--rw-r--r--   0        0        0     2612 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/index_access.py
--rw-r--r--   0        0        0     3662 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/index_range_access.py
--rw-r--r--   0        0        0     2850 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/literal.py
--rw-r--r--   0        0        0    20305 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/member_access.py
--rw-r--r--   0        0        0     2372 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/new_expression.py
--rw-r--r--   0        0        0     3325 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/tuple_expression.py
--rw-r--r--   0        0        0     4515 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/expressions/unary_operation.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/__init__.py
--rw-r--r--   0        0        0    10622 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     9570 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3751 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     6082 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3449 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4305 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1553 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0    12331 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2539 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4686 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5668 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     9999 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/__init__.py
--rw-r--r--   0        0        0     6652 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/abc.py
--rw-r--r--   0        0        0     3254 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/block.py
--rw-r--r--   0        0        0     1722 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/break_statement.py
--rw-r--r--   0        0        0     1746 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/continue_statement.py
--rw-r--r--   0        0        0     2628 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/do_while_statement.py
--rw-r--r--   0        0        0     2545 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/emit_statement.py
--rw-r--r--   0        0        0     4836 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/expression_statement.py
--rw-r--r--   0        0        0     5797 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/for_statement.py
--rw-r--r--   0        0        0     3488 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/if_statement.py
--rw-r--r--   0        0        0    11028 2024-03-16 09:49:50.698696 eth_wake-4.7.0/wake/ir/statements/inline_assembly.py
--rw-r--r--   0        0        0     1694 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/placeholder_statement.py
--rw-r--r--   0        0        0     3423 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/return_statement.py
--rw-r--r--   0        0        0     2717 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/revert_statement.py
--rw-r--r--   0        0        0     3243 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/try_statement.py
--rw-r--r--   0        0        0     2571 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/unchecked_block.py
--rw-r--r--   0        0        0     4389 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/variable_declaration_statement.py
--rw-r--r--   0        0        0     2661 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/statements/while_statement.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/__init__.py
--rw-r--r--   0        0        0     5137 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/abc.py
--rw-r--r--   0        0        0     4062 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/array_type_name.py
--rw-r--r--   0        0        0     5924 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/elementary_type_name.py
--rw-r--r--   0        0        0     3961 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/function_type_name.py
--rw-r--r--   0        0        0     6502 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/mapping.py
--rw-r--r--   0        0        0    11357 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/type_names/user_defined_type_name.py
--rw-r--r--   0        0        0    61318 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/types.py
--rw-r--r--   0        0        0      822 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/utils.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/__init__.py
--rw-r--r--   0        0        0     1718 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/abc.py
--rw-r--r--   0        0        0     3025 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/assignment.py
--rw-r--r--   0        0        0     4701 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/block.py
--rw-r--r--   0        0        0     1007 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/break_statement.py
--rw-r--r--   0        0        0     2453 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/case_.py
--rw-r--r--   0        0        0     1064 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1860 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     3256 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/for_loop.py
--rw-r--r--   0        0        0     6392 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/function_call.py
--rw-r--r--   0        0        0     3516 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/function_definition.py
--rw-r--r--   0        0        0     2828 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/identifier.py
--rw-r--r--   0        0        0     2731 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/if_statement.py
--rw-r--r--   0        0        0     1266 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/leave.py
--rw-r--r--   0        0        0     3619 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/literal.py
--rw-r--r--   0        0        0     3147 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/switch.py
--rw-r--r--   0        0        0     2198 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/typed_name.py
--rw-r--r--   0        0        0     3235 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0       47 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/__init__.py
--rw-r--r--   0        0        0      310 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/__init__.py
--rw-r--r--   0        0        0     3842 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0     1123 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4303 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2291 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0     4128 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/commands/init.py
--rw-r--r--   0        0        0    31620 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/common_structures.py
--rw-r--r--   0        0        0     2533 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/context.py
--rw-r--r--   0        0        0     2574 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/enums.py
--rw-r--r--   0        0        0      471 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/__init__.py
--rw-r--r--   0        0        0     6969 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/code_action.py
--rw-r--r--   0        0        0    11343 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/code_lens.py
--rw-r--r--   0        0        0    19894 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/completion.py
--rw-r--r--   0        0        0    10194 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/definition.py
--rw-r--r--   0        0        0     1472 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     4331 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/document_link.py
--rw-r--r--   0        0        0     8062 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    18513 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/hover.py
--rw-r--r--   0        0        0     3927 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/implementation.py
--rw-r--r--   0        0        0     2914 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/inlay_hint.py
--rw-r--r--   0        0        0     5115 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/references.py
--rw-r--r--   0        0        0     8941 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/rename.py
--rw-r--r--   0        0        0     9389 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11131 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0      750 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/logging_handler.py
--rw-r--r--   0        0        0    64915 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     8941 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/lsp_parser.py
--rw-r--r--   0        0        0     5551 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/methods.py
--rw-r--r--   0        0        0     1897 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2024-03-16 09:49:50.702696 eth_wake-4.7.0/wake/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    53084 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/lsp/server.py
--rw-r--r--   0        0        0     6793 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/lsp/utils/uri.py
--rw-r--r--   0        0        0      102 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/migrations/__init__.py
--rw-r--r--   0        0        0     9091 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/migrations/woke_wake_migration.py
--rw-r--r--   0        0        0     3307 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/migrations/xdg_migration.py
--rw-r--r--   0        0        0       74 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/printers/__init__.py
--rw-r--r--   0        0        0    14954 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/printers/api.py
--rw-r--r--   0        0        0      412 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/printers/template.py
--rw-r--r--   0        0        0       50 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/regex_parser/solidity_import.py
--rw-r--r--   0        0        0    10611 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/svm/__init__.py
--rw-r--r--   0        0        0     1815 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/svm/abc.py
--rw-r--r--   0        0        0      270 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/svm/exceptions.py
--rw-r--r--   0        0        0    12254 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/svm/svm.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/templates/tests/__init__.py
--rw-r--r--   0        0        0      253 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/templates/tests/test_default.py
--rw-r--r--   0        0        0      838 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/__init__.py
--rw-r--r--   0        0        0    11116 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/core.py
--rw-r--r--   0        0        0    23995 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/coverage.py
--rw-r--r--   0        0        0      187 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     5028 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10577 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5407 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/fuzzing/generators.py
--rw-r--r--   0        0        0     8042 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/pytest_plugin_multiprocess.py
--rw-r--r--   0        0        0    12613 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/pytest_plugin_multiprocess_server.py
--rw-r--r--   0        0        0     2855 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/testing/pytest_plugin_single.py
--rw-r--r--   0        0        0      288 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/__init__.py
--rw-r--r--   0        0        0      654 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/context_managers.py
--rw-r--r--   0        0        0      975 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/decorators.py
--rw-r--r--   0        0        0      158 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/enums.py
--rw-r--r--   0        0        0     1699 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/file_utils.py
--rw-r--r--   0        0        0      518 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/formatters.py
--rw-r--r--   0        0        0      875 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/general.py
--rw-r--r--   0        0        0      384 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/networking.py
--rw-r--r--   0        0        0     1569 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/null_file.py
--rw-r--r--   0        0        0     1017 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/string.py
--rw-r--r--   0        0        0     1747 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/tee.py
--rw-r--r--   0        0        0     3792 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      424 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake/utils/version.py
--rw-r--r--   0        0        0     1296 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/__init__.py
--rw-r--r--   0        0        0     3726 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/abi_encode_with_signature.py
--rw-r--r--   0        0        0    15179 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/axelar_proxy_contract_id.py
--rw-r--r--   0        0        0     5656 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/balance_relied_on.py
--rw-r--r--   0        0        0     3197 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/call_options_not_called.py
--rw-r--r--   0        0        0     9968 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py
--rw-r--r--   0        0        0     2525 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/complex_struct_getter.py
--rw-r--r--   0        0        0     3434 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/empty_byte_array_copy_bug.py
--rw-r--r--   0        0        0    18811 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/incorrect_interface.py
--rw-r--r--   0        0        0     4318 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/missing_return.py
--rw-r--r--   0        0        0     4082 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0    11049 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/reentrancy.py
--rw-r--r--   0        0        0     2364 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/struct_mapping_deletion.py
--rw-r--r--   0        0        0     3590 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/tx_origin.py
--rw-r--r--   0        0        0     4019 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     1681 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unprotected_selfdestruct.py
--rw-r--r--   0        0        0     6655 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     2198 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unsafe_erc20_call.py
--rw-r--r--   0        0        0     2225 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unused_contract.py
--rw-r--r--   0        0        0     1790 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unused_function.py
--rw-r--r--   0        0        0     2781 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unused_import.py
--rw-r--r--   0        0        0     1520 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/unused_modifier.py
--rw-r--r--   0        0        0      229 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_detectors/utils.py
--rw-r--r--   0        0        0      462 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_printers/__init__.py
--rw-r--r--   0        0        0     3487 2024-03-16 09:49:50.706696 eth_wake-4.7.0/wake_printers/abi.py
--rw-r--r--   0        0        0     3223 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/c3_linearization.py
--rw-r--r--   0        0        0     4260 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/control_flow_graph.py
--rw-r--r--   0        0        0     5435 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/imports_graph.py
--rw-r--r--   0        0        0     6127 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/inheritance_graph.py
--rw-r--r--   0        0        0     1574 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/inheritance_tree.py
--rw-r--r--   0        0        0     5805 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/modifiers.py
--rw-r--r--   0        0        0     5748 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/state_changes.py
--rw-r--r--   0        0        0     3600 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/storage_layout.py
--rw-r--r--   0        0        0     8131 2024-03-16 09:49:50.710696 eth_wake-4.7.0/wake_printers/tokens.py
--rw-r--r--   0        0        0    12327 1970-01-01 00:00:00.000000 eth_wake-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2024-04-05 10:35:38.715089 eth_wake-4.8.0/LICENSE
+-rw-r--r--   0        0        0     9113 2024-04-05 10:35:38.715089 eth_wake-4.8.0/README.md
+-rw-r--r--   0        0        0       61 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/.gitignore
+-rw-r--r--   0        0        0      431 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/README.md
+-rw-r--r--   0        0        0     1198 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Counter.sol
+-rw-r--r--   0        0        0      622 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Gateway.sol
+-rw-r--r--   0        0        0      307 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Imports.sol
+-rw-r--r--   0        0        0      215 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/hardhat.config.js
+-rw-r--r--   0        0        0      813 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/package-lock.json
+-rw-r--r--   0        0        0       97 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/package.json
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/scripts/__init__.py
+-rw-r--r--   0        0        0      350 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/__init__.py
+-rw-r--r--   0        0        0     3559 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter.py
+-rw-r--r--   0        0        0     1815 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz.py
+-rw-r--r--   0        0        0     1170 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz_failing.py
+-rw-r--r--   0        0        0     3404 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_crosschain.py
+-rw-r--r--   0        0        0       24 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/wake.toml
+-rw-r--r--   0        0        0     3404 2024-04-05 10:35:38.743090 eth_wake-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0      355 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/__init__.py
+-rw-r--r--   0        0        0    37717 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/cfg.py
+-rw-r--r--   0        0        0     7584 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/expressions.py
+-rw-r--r--   0        0        0     2353 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/graph.py
+-rw-r--r--   0        0        0     1543 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/interface.py
+-rw-r--r--   0        0        0    16505 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/ownable.py
+-rw-r--r--   0        0        0     1093 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/proxy.py
+-rw-r--r--   0        0        0     7416 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/utils.py
+-rw-r--r--   0        0        0       38 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/__init__.py
+-rw-r--r--   0        0        0     7310 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/__main__.py
+-rw-r--r--   0        0        0     8068 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/accounts.py
+-rw-r--r--   0        0        0     8674 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/compile.py
+-rw-r--r--   0        0        0       54 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/console.py
+-rw-r--r--   0        0        0    30671 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/detect.py
+-rw-r--r--   0        0        0    24955 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/init.py
+-rw-r--r--   0        0        0     1298 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/lsp.py
+-rw-r--r--   0        0        0     8269 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/open.py
+-rw-r--r--   0        0        0     5495 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/param_types.py
+-rw-r--r--   0        0        0    23532 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/print.py
+-rw-r--r--   0        0        0     3583 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/run.py
+-rw-r--r--   0        0        0     5877 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/svm.py
+-rw-r--r--   0        0        0     9541 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/test.py
+-rw-r--r--   0        0        0      187 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/__init__.py
+-rw-r--r--   0        0        0     4929 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3120 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    53031 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8831 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     9163 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3597 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4912 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/__init__.py
+-rw-r--r--   0        0        0    11941 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/data_model.py
+-rw-r--r--   0        0        0    15443 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/wake_config.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/wake/__init__.py
+-rw-r--r--   0        0        0    64087 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/wake/console.sol
+-rw-r--r--   0        0        0       32 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/enums.py
+-rw-r--r--   0        0        0      640 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/logging.py
+-rw-r--r--   0        0        0    11342 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/lsp_provider.py
+-rw-r--r--   0        0        0    29888 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/solidity_version.py
+-rw-r--r--   0        0        0    27317 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/visitor.py
+-rw-r--r--   0        0        0     1793 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/wake_comments.py
+-rw-r--r--   0        0        0      734 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/deployment/__init__.py
+-rw-r--r--   0        0        0    14991 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/deployment/core.py
+-rw-r--r--   0        0        0      141 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/__init__.py
+-rw-r--r--   0        0        0    29661 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/api.py
+-rw-r--r--   0        0        0      649 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/template.py
+-rw-r--r--   0        0        0     7760 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/blocks.py
+-rw-r--r--   0        0        0    50133 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/call_trace.py
+-rw-r--r--   0        0        0    29599 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1320 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/constants.py
+-rw-r--r--   0        0        0   111039 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/core.py
+-rw-r--r--   0        0        0     8429 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/globals.py
+-rw-r--r--   0        0        0   161115 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/hardhat_console.py
+-rw-r--r--   0        0        0     1267 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/internal.py
+-rw-r--r--   0        0        0       39 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2092 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      825 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2912 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      668 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0    17584 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/primitive_types.py
+-rw-r--r--   0        0        0    96402 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/pytypes_generator.py
+-rw-r--r--   0        0        0    29435 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/transactions.py
+-rw-r--r--   0        0        0    45923 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/utils.py
+-rw-r--r--   0        0        0     4197 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/__init__.py
+-rw-r--r--   0        0        0     4947 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/abc.py
+-rw-r--r--   0        0        0    39042 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/ast.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/__init__.py
+-rw-r--r--   0        0        0     5827 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/abc.py
+-rw-r--r--   0        0        0    19160 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/contract_definition.py
+-rw-r--r--   0        0        0     4102 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/enum_definition.py
+-rw-r--r--   0        0        0     2047 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/enum_value.py
+-rw-r--r--   0        0        0     5380 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/error_definition.py
+-rw-r--r--   0        0        0     6611 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/event_definition.py
+-rw-r--r--   0        0        0    20351 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/function_definition.py
+-rw-r--r--   0        0        0    14120 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/modifier_definition.py
+-rw-r--r--   0        0        0     4401 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/struct_definition.py
+-rw-r--r--   0        0        0     3662 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    20534 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/variable_declaration.py
+-rw-r--r--   0        0        0    11238 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/enums.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/__init__.py
+-rw-r--r--   0        0        0     8026 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/abc.py
+-rw-r--r--   0        0        0     5988 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/assignment.py
+-rw-r--r--   0        0        0     4316 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/binary_operation.py
+-rw-r--r--   0        0        0     2627 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/conditional.py
+-rw-r--r--   0        0        0     2001 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/elementary_type_name_expression.py
+-rw-r--r--   0        0        0    11941 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/function_call.py
+-rw-r--r--   0        0        0     3383 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/function_call_options.py
+-rw-r--r--   0        0        0     9399 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/identifier.py
+-rw-r--r--   0        0        0     2612 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/index_access.py
+-rw-r--r--   0        0        0     3662 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/index_range_access.py
+-rw-r--r--   0        0        0     2850 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/literal.py
+-rw-r--r--   0        0        0    20305 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/member_access.py
+-rw-r--r--   0        0        0     2372 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/new_expression.py
+-rw-r--r--   0        0        0     3325 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/tuple_expression.py
+-rw-r--r--   0        0        0     4515 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/unary_operation.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/__init__.py
+-rw-r--r--   0        0        0    10622 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     9570 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3751 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     6082 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3449 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4305 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1553 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0    12331 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2539 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4686 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5668 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     9999 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/__init__.py
+-rw-r--r--   0        0        0     6652 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/abc.py
+-rw-r--r--   0        0        0     3254 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/block.py
+-rw-r--r--   0        0        0     1722 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/break_statement.py
+-rw-r--r--   0        0        0     1746 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/continue_statement.py
+-rw-r--r--   0        0        0     2628 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/do_while_statement.py
+-rw-r--r--   0        0        0     2545 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/emit_statement.py
+-rw-r--r--   0        0        0     4836 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/expression_statement.py
+-rw-r--r--   0        0        0     5797 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/for_statement.py
+-rw-r--r--   0        0        0     3488 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/if_statement.py
+-rw-r--r--   0        0        0    11028 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/inline_assembly.py
+-rw-r--r--   0        0        0     1694 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/placeholder_statement.py
+-rw-r--r--   0        0        0     3423 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/return_statement.py
+-rw-r--r--   0        0        0     2717 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/revert_statement.py
+-rw-r--r--   0        0        0     3243 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/try_statement.py
+-rw-r--r--   0        0        0     2571 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/unchecked_block.py
+-rw-r--r--   0        0        0     4389 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2661 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/while_statement.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/__init__.py
+-rw-r--r--   0        0        0     5137 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/abc.py
+-rw-r--r--   0        0        0     4062 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/array_type_name.py
+-rw-r--r--   0        0        0     5924 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/elementary_type_name.py
+-rw-r--r--   0        0        0     3961 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/function_type_name.py
+-rw-r--r--   0        0        0     6502 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/mapping.py
+-rw-r--r--   0        0        0    11357 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/user_defined_type_name.py
+-rw-r--r--   0        0        0    61318 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/types.py
+-rw-r--r--   0        0        0      822 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/__init__.py
+-rw-r--r--   0        0        0     1718 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/abc.py
+-rw-r--r--   0        0        0     3025 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4701 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/block.py
+-rw-r--r--   0        0        0     1007 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     2453 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/case_.py
+-rw-r--r--   0        0        0     1064 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1860 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     3256 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     6392 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/function_call.py
+-rw-r--r--   0        0        0     3516 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     2828 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/identifier.py
+-rw-r--r--   0        0        0     2731 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/if_statement.py
+-rw-r--r--   0        0        0     1266 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/leave.py
+-rw-r--r--   0        0        0     3619 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/literal.py
+-rw-r--r--   0        0        0     3147 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/switch.py
+-rw-r--r--   0        0        0     2198 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     3235 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0       47 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     3842 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0     1123 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4303 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2291 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0     4128 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/init.py
+-rw-r--r--   0        0        0    31620 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/common_structures.py
+-rw-r--r--   0        0        0     2552 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/context.py
+-rw-r--r--   0        0        0     2574 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/enums.py
+-rw-r--r--   0        0        0      471 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/code_action.py
+-rw-r--r--   0        0        0    11750 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    20068 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/completion.py
+-rw-r--r--   0        0        0    10194 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/definition.py
+-rw-r--r--   0        0        0     1472 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     4331 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8062 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    18513 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/hover.py
+-rw-r--r--   0        0        0     3927 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/implementation.py
+-rw-r--r--   0        0        0     3525 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/inlay_hint.py
+-rw-r--r--   0        0        0     5115 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/references.py
+-rw-r--r--   0        0        0     8941 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/rename.py
+-rw-r--r--   0        0        0     9389 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11131 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0      750 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/logging_handler.py
+-rw-r--r--   0        0        0    66467 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     8941 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_parser.py
+-rw-r--r--   0        0        0     5551 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    55986 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/server.py
+-rw-r--r--   0        0        0     6793 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/uri.py
+-rw-r--r--   0        0        0      102 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/__init__.py
+-rw-r--r--   0        0        0     9091 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/woke_wake_migration.py
+-rw-r--r--   0        0        0     3307 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/xdg_migration.py
+-rw-r--r--   0        0        0       74 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/__init__.py
+-rw-r--r--   0        0        0    14954 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/api.py
+-rw-r--r--   0        0        0      412 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/template.py
+-rw-r--r--   0        0        0       50 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0    10611 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/abc.py
+-rw-r--r--   0        0        0      270 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/exceptions.py
+-rw-r--r--   0        0        0    12254 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/svm.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/tests/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/tests/test_default.py
+-rw-r--r--   0        0        0      838 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/__init__.py
+-rw-r--r--   0        0        0    11116 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/core.py
+-rw-r--r--   0        0        0    23995 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/coverage.py
+-rw-r--r--   0        0        0      187 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     5028 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10577 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5407 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0     8240 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess.py
+-rw-r--r--   0        0        0    12854 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess_server.py
+-rw-r--r--   0        0        0     3057 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_single.py
+-rw-r--r--   0        0        0      288 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/context_managers.py
+-rw-r--r--   0        0        0      975 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/decorators.py
+-rw-r--r--   0        0        0      158 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/enums.py
+-rw-r--r--   0        0        0     1699 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/file_utils.py
+-rw-r--r--   0        0        0      518 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/formatters.py
+-rw-r--r--   0        0        0      875 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/general.py
+-rw-r--r--   0        0        0      384 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/networking.py
+-rw-r--r--   0        0        0     1569 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/null_file.py
+-rw-r--r--   0        0        0     1017 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/string.py
+-rw-r--r--   0        0        0     1747 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/tee.py
+-rw-r--r--   0        0        0     3792 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      424 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/version.py
+-rw-r--r--   0        0        0     1296 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/__init__.py
+-rw-r--r--   0        0        0     3726 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/abi_encode_with_signature.py
+-rw-r--r--   0        0        0    15179 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/axelar_proxy_contract_id.py
+-rw-r--r--   0        0        0     5656 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/balance_relied_on.py
+-rw-r--r--   0        0        0     3197 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     9968 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py
+-rw-r--r--   0        0        0     2525 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/complex_struct_getter.py
+-rw-r--r--   0        0        0     3434 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/empty_byte_array_copy_bug.py
+-rw-r--r--   0        0        0    18811 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/incorrect_interface.py
+-rw-r--r--   0        0        0     4318 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/missing_return.py
+-rw-r--r--   0        0        0     4082 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0    11049 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/reentrancy.py
+-rw-r--r--   0        0        0     2364 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/struct_mapping_deletion.py
+-rw-r--r--   0        0        0     3590 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/tx_origin.py
+-rw-r--r--   0        0        0     4019 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     1681 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unprotected_selfdestruct.py
+-rw-r--r--   0        0        0     6655 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     2198 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unsafe_erc20_call.py
+-rw-r--r--   0        0        0     2225 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_contract.py
+-rw-r--r--   0        0        0     1790 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_function.py
+-rw-r--r--   0        0        0     2781 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_import.py
+-rw-r--r--   0        0        0     1520 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_modifier.py
+-rw-r--r--   0        0        0      229 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/utils.py
+-rw-r--r--   0        0        0      462 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/abi.py
+-rw-r--r--   0        0        0     3223 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/c3_linearization.py
+-rw-r--r--   0        0        0     4260 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/control_flow_graph.py
+-rw-r--r--   0        0        0     5435 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/imports_graph.py
+-rw-r--r--   0        0        0     6127 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/inheritance_graph.py
+-rw-r--r--   0        0        0     1574 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/inheritance_tree.py
+-rw-r--r--   0        0        0     5805 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/modifiers.py
+-rw-r--r--   0        0        0     5748 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/state_changes.py
+-rw-r--r--   0        0        0     3600 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/storage_layout.py
+-rw-r--r--   0        0        0     8131 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/tokens.py
+-rw-r--r--   0        0        0    12327 1970-01-01 00:00:00.000000 eth_wake-4.8.0/PKG-INFO
```

### Comparing `eth_wake-4.7.0/LICENSE` & `eth_wake-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/README.md` & `eth_wake-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/contracts/Counter.sol` & `eth_wake-4.8.0/examples/counter/contracts/Counter.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/contracts/Gateway.sol` & `eth_wake-4.8.0/examples/counter/contracts/Gateway.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/package-lock.json` & `eth_wake-4.8.0/examples/counter/package-lock.json`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/tests/test_counter.py` & `eth_wake-4.8.0/examples/counter/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/tests/test_counter_fuzz.py` & `eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/tests/test_counter_fuzz_failing.py` & `eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz_failing.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/examples/counter/tests/test_crosschain.py` & `eth_wake-4.8.0/examples/counter/tests/test_crosschain.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/pyproject.toml` & `eth_wake-4.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eth-wake"
-version = "4.7.0"
+version = "4.8.0"
 description = "Wake is a Python-based Solidity development and testing framework with built-in vulnerability detectors."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://getwake.io"
 repository = "https://github.com/Ackee-Blockchain/wake"
 documentation = "https://ackeeblockchain.com/wake/docs/latest"
```

### Comparing `eth_wake-4.7.0/wake/analysis/cfg.py` & `eth_wake-4.8.0/wake/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/analysis/expressions.py` & `eth_wake-4.8.0/wake/analysis/expressions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Tuple, Union
 
 import wake.ir as ir
 import wake.ir.types as types
 from wake.core.logging import get_logger
+from wake.utils.decorators import return_on_recursion
 
 from .utils import get_function_implementations
 
 logger = get_logger(__name__)
 
 
 def expression_is_global_symbol(
@@ -48,14 +49,15 @@
                 logger.debug(f"Expression is {global_symbol}: {expr.source}")
                 return True
 
     logger.debug(f"Expression is NOT {global_symbol}: {expr.source}")
     return False
 
 
+@return_on_recursion((None,))
 def get_variable_declarations_from_expression(
     expr: ir.ExpressionAbc,
 ) -> Tuple[Optional[ir.VariableDeclaration], ...]:
     from wake.analysis.utils import get_all_base_and_child_declarations
 
     if isinstance(expr, ir.Identifier):
         ref = expr.referenced_declaration
```

### Comparing `eth_wake-4.7.0/wake/analysis/graph.py` & `eth_wake-4.8.0/wake/analysis/graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/analysis/interface.py` & `eth_wake-4.8.0/wake/analysis/interface.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/analysis/ownable.py` & `eth_wake-4.8.0/wake/analysis/ownable.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/analysis/proxy.py` & `eth_wake-4.8.0/wake/analysis/proxy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/analysis/utils.py` & `eth_wake-4.8.0/wake/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/__main__.py` & `eth_wake-4.8.0/wake/cli/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 import os
 import platform
 import sys
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, List, Optional, Sequence
 
 import rich_click as click
 from click.core import Context
 from rich.logging import RichHandler
 
 from .accounts import run_accounts
 from .compile import run_compile
@@ -72,14 +72,46 @@
         if cmd_name == "init":
             cmd_name = "up"
         return super().get_command(ctx, cmd_name)
 
     def list_commands(self, ctx: Context) -> List[str]:
         return sorted(["up"] + super().list_commands(ctx))
 
+    def main(
+        self,
+        args: Optional[Sequence[str]] = None,
+        prog_name: Optional[str] = None,
+        complete_var: Optional[str] = None,
+        standalone_mode: bool = True,
+        windows_expand_args: bool = True,
+        **extra: Any,
+    ) -> Any:
+        if "_WAKE_COMPLETE" in os.environ:
+            import warnings
+
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                return super().main(
+                    args=args,
+                    prog_name=prog_name,
+                    complete_var=complete_var,
+                    standalone_mode=standalone_mode,
+                    windows_expand_args=windows_expand_args,
+                    **extra,
+                )
+        else:
+            return super().main(
+                args=args,
+                prog_name=prog_name,
+                complete_var=complete_var,
+                standalone_mode=standalone_mode,
+                windows_expand_args=windows_expand_args,
+                **extra,
+            )
+
 
 @click.group(cls=AliasedGroup, context_settings={"help_option_names": ["-h", "--help"]})
 @click.option(
     "--debug",
     "-d",
     is_flag=True,
     default=False,
```

### Comparing `eth_wake-4.7.0/wake/cli/accounts.py` & `eth_wake-4.8.0/wake/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/compile.py` & `eth_wake-4.8.0/wake/cli/compile.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/detect.py` & `eth_wake-4.8.0/wake/cli/detect.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/init.py` & `eth_wake-4.8.0/wake/cli/init.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/lsp.py` & `eth_wake-4.8.0/wake/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/open.py` & `eth_wake-4.8.0/wake/cli/open.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/param_types.py` & `eth_wake-4.8.0/wake/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/print.py` & `eth_wake-4.8.0/wake/cli/print.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/run.py` & `eth_wake-4.8.0/wake/cli/run.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/svm.py` & `eth_wake-4.8.0/wake/cli/svm.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/cli/test.py` & `eth_wake-4.8.0/wake/cli/test.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/build_data_model.py` & `eth_wake-4.8.0/wake/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/compilation_unit.py` & `eth_wake-4.8.0/wake/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/compiler.py` & `eth_wake-4.8.0/wake/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/solc_frontend/input_data_model.py` & `eth_wake-4.8.0/wake/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/solc_frontend/output_data_model.py` & `eth_wake-4.8.0/wake/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/solc_frontend/solc_runner.py` & `eth_wake-4.8.0/wake/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/source_path_resolver.py` & `eth_wake-4.8.0/wake/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/compiler/source_unit_name_resolver.py` & `eth_wake-4.8.0/wake/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/config/__init__.py` & `eth_wake-4.8.0/wake/config/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/config/data_model.py` & `eth_wake-4.8.0/wake/config/data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/config/wake_config.py` & `eth_wake-4.8.0/wake/config/wake_config.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/contracts/wake/console.sol` & `eth_wake-4.8.0/wake/contracts/wake/console.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/core/logging.py` & `eth_wake-4.8.0/wake/core/logging.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/core/solidity_version.py` & `eth_wake-4.8.0/wake/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/core/visitor.py` & `eth_wake-4.8.0/wake/core/visitor.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/core/wake_comments.py` & `eth_wake-4.8.0/wake/core/wake_comments.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/deployment/__init__.py` & `eth_wake-4.8.0/wake/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/deployment/core.py` & `eth_wake-4.8.0/wake/deployment/core.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/detectors/api.py` & `eth_wake-4.8.0/wake/detectors/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import partial, total_ordering
+from itertools import chain
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     DefaultDict,
@@ -209,19 +210,21 @@
     """
     Strip all subdetections that are located in excluded paths and their parents are also in excluded paths.
     In other words, remove all subdetection branches that whole end up in excluded paths.
     """
     if len(detection.subdetections) == 0:
         return detection
 
+    wake_contracts_path = Path(__file__).parent.parent / "contracts"
+
     subdetections = []
     for d in detection.subdetections:
         if not any(
             is_relative_to(d.ir_node.source_unit.file, p)
-            for p in config.detectors.exclude_paths
+            for p in chain(config.detectors.exclude_paths, [wake_contracts_path])
         ):
             subdetections.append(d)
             continue
 
         d = _strip_excluded_subdetections(d, config)
         if len(d.subdetections) != 0:
             subdetections.append(d)
@@ -316,17 +319,19 @@
         if (
             len(detection.detection.subdetections) == 0
             and l > 0
             and detection.detection.subdetections_mandatory
         ):
             continue
 
+        wake_contracts_path = Path(__file__).parent.parent / "contracts"
+
         if any(
             is_relative_to(detection.detection.ir_node.source_unit.file, p)
-            for p in config.detectors.exclude_paths
+            for p in chain(config.detectors.exclude_paths, [wake_contracts_path])
         ):
             detection = DetectorResult(
                 _strip_excluded_subdetections(detection.detection, config),
                 detection.impact,
                 detection.confidence,
                 detection.uri,
             )
```

### Comparing `eth_wake-4.7.0/wake/detectors/template.py` & `eth_wake-4.8.0/wake/detectors/template.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/detectors/utils.py` & `eth_wake-4.8.0/wake/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/blocks.py` & `eth_wake-4.8.0/wake/development/blocks.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/call_trace.py` & `eth_wake-4.8.0/wake/development/call_trace.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/chain_interfaces.py` & `eth_wake-4.8.0/wake/development/chain_interfaces.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/constants.py` & `eth_wake-4.8.0/wake/development/constants.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/core.py` & `eth_wake-4.8.0/wake/development/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,23 @@
     chain_interfaces_manager,
     get_config,
     get_coverage_handler,
     get_exception_handler,
 )
 from .internal import UnknownEvent, read_from_memory
 from .json_rpc.communicator import JsonRpcError
-from .primitive_types import FixedSizeBytes, Integer
+from .primitive_types import (
+    FixedSizeBytes,
+    FixedSizeList,
+    Integer,
+    fixed_bytes_map,
+    fixed_list_map,
+    int_map,
+    uint_map,
+)
 
 if TYPE_CHECKING:
     from .transactions import (
         ChainTransactions,
         TransactionAbc,
         TransactionRevertedError,
     )
@@ -253,14 +261,17 @@
             raise ValueError(f"Unsupported type {t}")
 
     @classmethod
     def _types_from_args(cls, args: Iterable) -> str:
         if isinstance(args, tuple):
             return f"({','.join(cls._types_from_args(arg) for arg in args)})"
         elif isinstance(args, list):
+            if len(args) == 0:
+                return "uint256[]"  # should not matter what type is used
+
             for arg in args:
                 try:
                     arg_type = cls._types_from_args(arg)
                     if hasattr(args, "length"):
                         return f"{arg_type}[{getattr(args, 'length')}]"
                     else:
                         return f"{arg_type}[]"
@@ -390,30 +401,52 @@
                 ret.append(arg)
         return ret
 
     @staticmethod
     def _normalize_output(types: Sequence[str], arguments: Sequence) -> Tuple:
         ret = []
         assert len(types) == len(arguments)
-        for type, arg in zip(types, arguments):
-            type = type.strip()
-            if type == "address":
+        for t, arg in zip(types, arguments):
+            t = t.strip()
+            if t == "address":
                 ret.append(Address(arg))
-            elif type.endswith("]"):
-                args_type = type[: type.rfind("[")]
+            elif t.endswith("]"):
+                args_type = t[: t.rfind("[")]
+
+                if t[-2] == "[":
+                    target_type = list
+                else:
+                    length = int(t[t.rfind("[") + 1 : -1])
+                    target_type = (
+                        fixed_list_map[length]
+                        if length <= 32
+                        else type(f"List{length}", (FixedSizeList,), {"length": length})
+                    )
                 assert isinstance(arg, (list, tuple))
-                ret.append(Abi._normalize_output([args_type] * len(arg), arg))
-            elif type.startswith("(") and type.endswith(")"):
-                abi_type = eth_abi.grammar.parse(type)
+                ret.append(
+                    target_type(Abi._normalize_output([args_type] * len(arg), arg))
+                )
+            elif t.startswith("(") and t.endswith(")"):
+                abi_type = eth_abi.grammar.parse(t)
                 assert isinstance(abi_type, eth_abi.grammar.TupleType)
                 ret.append(
                     Abi._normalize_output(
                         [c.to_type_str() for c in abi_type.components], arg
                     )
                 )
+            elif t.startswith("int"):
+                length = int(t[3:])
+                ret.append(int_map[length](arg))
+            elif t.startswith("uint"):
+                length = int(t[4:])
+                ret.append(uint_map[length](arg))
+            elif t.startswith("bytes") and t != "bytes":
+                # bytes1 - bytes32
+                length = int(t[5:])
+                ret.append(fixed_bytes_map[length](arg))
             else:
                 ret.append(arg)
         return tuple(ret)
 
     @classmethod
     def encode(cls, types: Iterable, arguments: Iterable) -> bytes:
         return eth_abi.abi.encode(types, cls._normalize_input(arguments))
```

### Comparing `eth_wake-4.7.0/wake/development/globals.py` & `eth_wake-4.8.0/wake/development/globals.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/hardhat_console.py` & `eth_wake-4.8.0/wake/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/internal.py` & `eth_wake-4.8.0/wake/development/internal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/json_rpc/communicator.py` & `eth_wake-4.8.0/wake/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/json_rpc/http.py` & `eth_wake-4.8.0/wake/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/json_rpc/ipc.py` & `eth_wake-4.8.0/wake/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/json_rpc/websocket.py` & `eth_wake-4.8.0/wake/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/primitive_types.py` & `eth_wake-4.8.0/wake/development/primitive_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -343,14 +343,49 @@
         pass
 
     uint256.min = uint256(0)
     uint256.max = uint256(2**256 - 1)
 
     uint = uint256
 
+    uint_map = {
+        8: uint8,
+        16: uint16,
+        24: uint24,
+        32: uint32,
+        40: uint40,
+        48: uint48,
+        56: uint56,
+        64: uint64,
+        72: uint72,
+        80: uint80,
+        88: uint88,
+        96: uint96,
+        104: uint104,
+        112: uint112,
+        120: uint120,
+        128: uint128,
+        136: uint136,
+        144: uint144,
+        152: uint152,
+        160: uint160,
+        168: uint168,
+        176: uint176,
+        184: uint184,
+        192: uint192,
+        200: uint200,
+        208: uint208,
+        216: uint216,
+        224: uint224,
+        232: uint232,
+        240: uint240,
+        248: uint248,
+        256: uint256,
+    }
+
     class int8(Integer):
         pass
 
     int8.min = int8(-(2**7))
     int8.max = int8(2**7 - 1)
 
     class int16(Integer):
@@ -535,14 +570,49 @@
 
     class int256(Integer):
         pass
 
     int256.min = int256(-(2**255))
     int256.max = int256(2**255 - 1)
 
+    int_map = {
+        8: int8,
+        16: int16,
+        24: int24,
+        32: int32,
+        40: int40,
+        48: int48,
+        56: int56,
+        64: int64,
+        72: int72,
+        80: int80,
+        88: int88,
+        96: int96,
+        104: int104,
+        112: int112,
+        120: int120,
+        128: int128,
+        136: int136,
+        144: int144,
+        152: int152,
+        160: int160,
+        168: int168,
+        176: int176,
+        184: int184,
+        192: int192,
+        200: int200,
+        208: int208,
+        216: int216,
+        224: int224,
+        232: int232,
+        240: int240,
+        248: int248,
+        256: int256,
+    }
+
     class FixedSizeBytes(bytes, abc.ABC):
         length: uint8
 
         def __new__(cls, value):
             ret = super().__new__(cls, value)
             if len(ret) > cls.length:
                 raise ValueError(
@@ -645,14 +715,49 @@
 
     class bytes31(FixedSizeBytes):
         length = uint8(31)
 
     class bytes32(FixedSizeBytes):
         length = uint8(32)
 
+    fixed_bytes_map = {
+        1: bytes1,
+        2: bytes2,
+        3: bytes3,
+        4: bytes4,
+        5: bytes5,
+        6: bytes6,
+        7: bytes7,
+        8: bytes8,
+        9: bytes9,
+        10: bytes10,
+        11: bytes11,
+        12: bytes12,
+        13: bytes13,
+        14: bytes14,
+        15: bytes15,
+        16: bytes16,
+        17: bytes17,
+        18: bytes18,
+        19: bytes19,
+        20: bytes20,
+        21: bytes21,
+        22: bytes22,
+        23: bytes23,
+        24: bytes24,
+        25: bytes25,
+        26: bytes26,
+        27: bytes27,
+        28: bytes28,
+        29: bytes29,
+        30: bytes30,
+        31: bytes31,
+        32: bytes32,
+    }
+
     T = TypeVar("T")
 
     class FixedSizeList(List[T], abc.ABC):
         length: uint256
 
         def __init__(self, items: Iterable[T]):
             super().__init__(items)
@@ -752,7 +857,42 @@
         length = uint256(30)
 
     class List31(FixedSizeList[T]):
         length = uint256(31)
 
     class List32(FixedSizeList[T]):
         length = uint256(32)
+
+    fixed_list_map = {
+        1: List1,
+        2: List2,
+        3: List3,
+        4: List4,
+        5: List5,
+        6: List6,
+        7: List7,
+        8: List8,
+        9: List9,
+        10: List10,
+        11: List11,
+        12: List12,
+        13: List13,
+        14: List14,
+        15: List15,
+        16: List16,
+        17: List17,
+        18: List18,
+        19: List19,
+        20: List20,
+        21: List21,
+        22: List22,
+        23: List23,
+        24: List24,
+        25: List25,
+        26: List26,
+        27: List27,
+        28: List28,
+        29: List29,
+        30: List30,
+        31: List31,
+        32: List32,
+    }
```

### Comparing `eth_wake-4.7.0/wake/development/pytypes_generator.py` & `eth_wake-4.8.0/wake/development/pytypes_generator.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/transactions.py` & `eth_wake-4.8.0/wake/development/transactions.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/development/utils.py` & `eth_wake-4.8.0/wake/development/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     Contract,
     abi,
     get_contracts_by_fqn,
     get_fqn_from_address,
     get_user_defined_value_types_index,
 )
 from .globals import get_config
-from .primitive_types import uint256
+from .primitive_types import FixedSizeList, bytes32, fixed_list_map, uint256
 
 # pyright: reportGeneralTypeIssues=false, reportOptionalIterable=false, reportOptionalSubscript=false, reportOptionalMemberAccess=false
 
 
 @dataclass
 class ChainExplorer:
     url: str
@@ -224,17 +224,17 @@
         if predicate(el):
             p.append(el)
         else:
             not_p.append(el)
     return p, not_p
 
 
-def keccak256(b: bytes) -> bytes:
+def keccak256(b: bytes) -> bytes32:
     h = keccak.new(data=b, digest_bits=256)
-    return h.digest()
+    return bytes32(h.digest())
 
 
 def get_current_fn_name(back_count=1) -> str:
     frame = inspect.currentframe()
     assert frame is not None
     for _ in range(back_count):
         frame = frame.f_back
@@ -411,41 +411,51 @@
             base_type = types[type_info.base]
             items_per_slot = 32 // base_type.number_of_bytes
 
             # arrays always start a new slot
             if type_info.encoding == "dynamic_array":
                 slot = int.from_bytes(keccak256(slot.to_bytes(32, "big")), "big")
                 length = Abi.decode(["uint256"], slot_data)[0]
+                target_type = list
             else:
                 length = int(type_info.label.split("[")[-1][:-1])
+                target_type = (
+                    fixed_list_map[length]
+                    if length <= 32
+                    else type(f"List{length}", (FixedSizeList,), {"length": length})
+                )
 
             if len(keys) == 0:
                 # reading whole array
                 if items_per_slot > 0:
-                    return [
-                        _get_storage_value(
-                            slot + i // items_per_slot,
-                            (i % items_per_slot) * base_type.number_of_bytes,
-                            keys[1:],
-                            type_info.base,
-                            types,
-                        )
-                        for i in range(length)
-                    ]
+                    return target_type(
+                        [
+                            _get_storage_value(
+                                slot + i // items_per_slot,
+                                (i % items_per_slot) * base_type.number_of_bytes,
+                                keys[1:],
+                                type_info.base,
+                                types,
+                            )
+                            for i in range(length)
+                        ]
+                    )
                 else:
-                    return [
-                        _get_storage_value(
-                            slot + (base_type.number_of_bytes * i) // 32,
-                            0,
-                            keys[1:],
-                            type_info.base,
-                            types,
-                        )
-                        for i in range(length)
-                    ]
+                    return target_type(
+                        [
+                            _get_storage_value(
+                                slot + (base_type.number_of_bytes * i) // 32,
+                                0,
+                                keys[1:],
+                                type_info.base,
+                                types,
+                            )
+                            for i in range(length)
+                        ]
+                    )
             else:
                 if not isinstance(keys[0], int):
                     raise ValueError(
                         f"{type_info.label} requires integer index to be specified as key"
                     )
                 if keys[0] >= length:
                     raise ValueError(
```

### Comparing `eth_wake-4.7.0/wake/ir/__init__.py` & `eth_wake-4.8.0/wake/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/abc.py` & `eth_wake-4.8.0/wake/ir/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/ast.py` & `eth_wake-4.8.0/wake/ir/ast.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/abc.py` & `eth_wake-4.8.0/wake/ir/declarations/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/contract_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/contract_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/enum_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/enum_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/enum_value.py` & `eth_wake-4.8.0/wake/ir/declarations/enum_value.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/error_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/error_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/event_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/event_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/function_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/function_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/modifier_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/modifier_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/struct_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/struct_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/user_defined_value_type_definition.py` & `eth_wake-4.8.0/wake/ir/declarations/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/declarations/variable_declaration.py` & `eth_wake-4.8.0/wake/ir/declarations/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/enums.py` & `eth_wake-4.8.0/wake/ir/enums.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/abc.py` & `eth_wake-4.8.0/wake/ir/expressions/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/assignment.py` & `eth_wake-4.8.0/wake/ir/expressions/assignment.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/binary_operation.py` & `eth_wake-4.8.0/wake/ir/expressions/binary_operation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/conditional.py` & `eth_wake-4.8.0/wake/ir/expressions/conditional.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/elementary_type_name_expression.py` & `eth_wake-4.8.0/wake/ir/expressions/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/function_call.py` & `eth_wake-4.8.0/wake/ir/expressions/function_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/function_call_options.py` & `eth_wake-4.8.0/wake/ir/expressions/function_call_options.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/identifier.py` & `eth_wake-4.8.0/wake/ir/expressions/identifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/index_access.py` & `eth_wake-4.8.0/wake/ir/expressions/index_access.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/index_range_access.py` & `eth_wake-4.8.0/wake/ir/expressions/index_range_access.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/literal.py` & `eth_wake-4.8.0/wake/ir/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/member_access.py` & `eth_wake-4.8.0/wake/ir/expressions/member_access.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/new_expression.py` & `eth_wake-4.8.0/wake/ir/expressions/new_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/tuple_expression.py` & `eth_wake-4.8.0/wake/ir/expressions/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/expressions/unary_operation.py` & `eth_wake-4.8.0/wake/ir/expressions/unary_operation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/identifier_path.py` & `eth_wake-4.8.0/wake/ir/meta/identifier_path.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/import_directive.py` & `eth_wake-4.8.0/wake/ir/meta/import_directive.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/inheritance_specifier.py` & `eth_wake-4.8.0/wake/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/modifier_invocation.py` & `eth_wake-4.8.0/wake/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/override_specifier.py` & `eth_wake-4.8.0/wake/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/parameter_list.py` & `eth_wake-4.8.0/wake/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/pragma_directive.py` & `eth_wake-4.8.0/wake/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/source_unit.py` & `eth_wake-4.8.0/wake/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/structured_documentation.py` & `eth_wake-4.8.0/wake/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/try_catch_clause.py` & `eth_wake-4.8.0/wake/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/meta/using_for_directive.py` & `eth_wake-4.8.0/wake/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/reference_resolver.py` & `eth_wake-4.8.0/wake/ir/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/abc.py` & `eth_wake-4.8.0/wake/ir/statements/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/block.py` & `eth_wake-4.8.0/wake/ir/statements/block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/break_statement.py` & `eth_wake-4.8.0/wake/ir/statements/break_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/continue_statement.py` & `eth_wake-4.8.0/wake/ir/statements/continue_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/do_while_statement.py` & `eth_wake-4.8.0/wake/ir/statements/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/emit_statement.py` & `eth_wake-4.8.0/wake/ir/statements/emit_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/expression_statement.py` & `eth_wake-4.8.0/wake/ir/statements/expression_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/for_statement.py` & `eth_wake-4.8.0/wake/ir/statements/for_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/if_statement.py` & `eth_wake-4.8.0/wake/ir/statements/if_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/inline_assembly.py` & `eth_wake-4.8.0/wake/ir/statements/inline_assembly.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/placeholder_statement.py` & `eth_wake-4.8.0/wake/ir/statements/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/return_statement.py` & `eth_wake-4.8.0/wake/ir/statements/return_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/revert_statement.py` & `eth_wake-4.8.0/wake/ir/statements/revert_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/try_statement.py` & `eth_wake-4.8.0/wake/ir/statements/try_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/unchecked_block.py` & `eth_wake-4.8.0/wake/ir/statements/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/variable_declaration_statement.py` & `eth_wake-4.8.0/wake/ir/statements/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/statements/while_statement.py` & `eth_wake-4.8.0/wake/ir/statements/while_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/abc.py` & `eth_wake-4.8.0/wake/ir/type_names/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/array_type_name.py` & `eth_wake-4.8.0/wake/ir/type_names/array_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/elementary_type_name.py` & `eth_wake-4.8.0/wake/ir/type_names/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/function_type_name.py` & `eth_wake-4.8.0/wake/ir/type_names/function_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/mapping.py` & `eth_wake-4.8.0/wake/ir/type_names/mapping.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/type_names/user_defined_type_name.py` & `eth_wake-4.8.0/wake/ir/type_names/user_defined_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/types.py` & `eth_wake-4.8.0/wake/ir/types.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/utils.py` & `eth_wake-4.8.0/wake/ir/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/abc.py` & `eth_wake-4.8.0/wake/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/assignment.py` & `eth_wake-4.8.0/wake/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/block.py` & `eth_wake-4.8.0/wake/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/break_statement.py` & `eth_wake-4.8.0/wake/ir/yul/break_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/case_.py` & `eth_wake-4.8.0/wake/ir/yul/case_.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/continue_statement.py` & `eth_wake-4.8.0/wake/ir/yul/continue_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/expression_statement.py` & `eth_wake-4.8.0/wake/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/for_loop.py` & `eth_wake-4.8.0/wake/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/function_call.py` & `eth_wake-4.8.0/wake/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/function_definition.py` & `eth_wake-4.8.0/wake/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/identifier.py` & `eth_wake-4.8.0/wake/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/if_statement.py` & `eth_wake-4.8.0/wake/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/leave.py` & `eth_wake-4.8.0/wake/ir/yul/leave.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/literal.py` & `eth_wake-4.8.0/wake/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/switch.py` & `eth_wake-4.8.0/wake/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/typed_name.py` & `eth_wake-4.8.0/wake/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/ir/yul/variable_declaration.py` & `eth_wake-4.8.0/wake/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/commands/generate_control_flow_graph.py` & `eth_wake-4.8.0/wake/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/commands/generate_imports_graph.py` & `eth_wake-4.8.0/wake/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/commands/generate_inheritance_graph.py` & `eth_wake-4.8.0/wake/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/commands/generate_linearized_inheritance_graph.py` & `eth_wake-4.8.0/wake/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/commands/init.py` & `eth_wake-4.8.0/wake/lsp/commands/init.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/common_structures.py` & `eth_wake-4.8.0/wake/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/context.py` & `eth_wake-4.8.0/wake/lsp/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
     def __init__(
         self, server: LspServer, config: WakeConfig, perform_files_discovery: bool
     ) -> None:
         self.__server = server
         self.__workspace_config = config
         self.__diagnostics_queue = asyncio.Queue()
-        self.__detectors_lsp_provider = LspProvider()
-        self.__printers_lsp_provider = LspProvider()
+        self.__detectors_lsp_provider = LspProvider("detector")
+        self.__printers_lsp_provider = LspProvider("printer")
         self.__compiler = LspCompiler(
             server,
             self.__diagnostics_queue,
             self.__detectors_lsp_provider,
             self.__printers_lsp_provider,
             perform_files_discovery,
         )
```

### Comparing `eth_wake-4.7.0/wake/lsp/document_sync.py` & `eth_wake-4.8.0/wake/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/code_action.py` & `eth_wake-4.8.0/wake/lsp/features/code_action.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/code_lens.py` & `eth_wake-4.8.0/wake/lsp/features/code_lens.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,23 +183,30 @@
     _code_lens_cache[path] = []
 
     for offsets, code_lens_items in chain(
         context.detectors_lsp_provider.get_code_lenses(path).items(),
         context.printers_lsp_provider.get_code_lenses(path).items(),
     ):
         for code_lens_options in code_lens_items:
-            code_lens.append(
-                CodeLens(
-                    range=context.compiler.get_range_from_byte_offsets(path, offsets),
-                    command=Command(
-                        title=code_lens_options.title,
-                        command="",
-                    ),
-                )
+            lens = CodeLens(
+                range=context.compiler.get_range_from_byte_offsets(path, offsets),
+                command=Command(
+                    title=code_lens_options.title,
+                    command="Tools-for-Solidity.wake_callback"
+                    if code_lens_options.callback_id is not None
+                    else "",
+                ),
             )
+            if code_lens_options.callback_id is not None:
+                lens.command.arguments = [  # pyright: ignore reportGeneralTypeIssues
+                    params.text_document.uri,
+                    code_lens_options.callback_kind,
+                    code_lens_options.callback_id,
+                ]
+            code_lens.append(lens)
 
     for node in source_unit:
         if isinstance(node, DeclarationAbc):
             refs = list(node.get_all_references(include_declarations=True))
             refs_count = len(
                 [ref for ref in refs if not isinstance(ref, DeclarationAbc)]
             )
```

### Comparing `eth_wake-4.7.0/wake/lsp/features/completion.py` & `eth_wake-4.8.0/wake/lsp/features/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import enum
 import logging
 from itertools import chain
+from pathlib import Path
 from typing import Any, List, Optional, Union
 
 from wake.core import get_logger
 
 from ...compiler.source_unit_name_resolver import SourceUnitNameResolver
 from ..common_structures import (
     Command,
@@ -532,17 +533,20 @@
         if node.type == "import_directive":
             break
         node = node.parent
 
     if node is None:
         return None
 
+    wake_contracts_path = Path(__file__).parent.parent.parent / "contracts"
+
     this_source_unit_name = None
     for include_path in chain(
-        context.config.compiler.solc.include_paths, [context.config.project_root_path]
+        context.config.compiler.solc.include_paths,
+        [context.config.project_root_path, wake_contracts_path],
     ):
         try:
             rel_path = str(path.relative_to(include_path).as_posix())
             if this_source_unit_name is None or len(this_source_unit_name) > len(
                 rel_path
             ):
                 this_source_unit_name = rel_path
@@ -568,15 +572,15 @@
             if p.is_dir():
                 completions.add(("./" + p.name + "/", CompletionItemKind.FOLDER))
             elif p.is_file() and p.suffix == ".sol" and p != path:
                 completions.add(("./" + p.name, CompletionItemKind.FILE))
 
         for include_path in chain(
             context.config.compiler.solc.include_paths,
-            [context.config.project_root_path],
+            [context.config.project_root_path, wake_contracts_path],
         ):
             if include_path.is_dir():
                 for p in include_path.iterdir():
                     if p.is_dir():
                         completions.add((p.name + "/", CompletionItemKind.FOLDER))
                     elif p.is_file() and p.suffix == ".sol":
                         completions.add((p.name, CompletionItemKind.FILE))
@@ -594,15 +598,15 @@
                 if p.is_dir():
                     completions.add((p.name + "/", CompletionItemKind.FOLDER))
                 elif p.is_file() and p.suffix == ".sol" and p != path:
                     completions.add((p.name, CompletionItemKind.FILE))
     else:
         for include_path in chain(
             context.config.compiler.solc.include_paths,
-            [context.config.project_root_path],
+            [context.config.project_root_path, wake_contracts_path],
         ):
             if include_path.is_dir():
                 dir = include_path / parent
                 if dir.is_dir():
                     for p in dir.iterdir():
                         if p.is_dir():
                             completions.add((p.name + "/", CompletionItemKind.FOLDER))
```

### Comparing `eth_wake-4.7.0/wake/lsp/features/definition.py` & `eth_wake-4.8.0/wake/lsp/features/definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/diagnostic.py` & `eth_wake-4.8.0/wake/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/document_link.py` & `eth_wake-4.8.0/wake/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/document_symbol.py` & `eth_wake-4.8.0/wake/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/hover.py` & `eth_wake-4.8.0/wake/lsp/features/hover.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/implementation.py` & `eth_wake-4.8.0/wake/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/inlay_hint.py` & `eth_wake-4.8.0/wake/lsp/features/inlay_hint.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,20 +78,38 @@
     inlay_hints = []
     for offset, inlay_hint_items in chain(
         context.detectors_lsp_provider.get_inlay_hints(path, (start, end)).items(),
         context.printers_lsp_provider.get_inlay_hints(path, (start, end)).items(),
     ):
         for inlay_hint_options in inlay_hint_items:
             line, col = context.compiler.get_line_pos_from_byte_offset(path, offset)
+
+            parts = []
+            for label, tooltip, callback_id in zip(
+                inlay_hint_options.label,
+                inlay_hint_options.tooltip,
+                inlay_hint_options.callback_id,
+            ):
+                part = InlayHintLabelPart(value=label)
+                if tooltip is not None:
+                    part.tooltip = tooltip
+                if callback_id is not None:
+                    part.command = Command(
+                        title=label,
+                        command="Tools-for-Solidity.wake_callback",
+                        arguments=[
+                            params.text_document.uri,
+                            inlay_hint_options.callback_kind,
+                            callback_id,
+                        ],
+                    )
+                parts.append(part)
+
             inlay_hint = InlayHint(
                 position=Position(line=line, character=col),
-                label=inlay_hint_options.label,
+                label=parts,
                 padding_left=inlay_hint_options.padding_left,
                 padding_right=inlay_hint_options.padding_right,
             )
-            if inlay_hint_options.tooltip is not None:
-                inlay_hint.tooltip = MarkupContent(
-                    kind=MarkupKind.MARKDOWN, value=inlay_hint_options.tooltip
-                )
             inlay_hints.append(inlay_hint)
 
     return inlay_hints
```

### Comparing `eth_wake-4.7.0/wake/lsp/features/references.py` & `eth_wake-4.8.0/wake/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/rename.py` & `eth_wake-4.8.0/wake/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/type_definition.py` & `eth_wake-4.8.0/wake/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/features/type_hierarchy.py` & `eth_wake-4.8.0/wake/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/logging_handler.py` & `eth_wake-4.8.0/wake/lsp/logging_handler.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/lsp_compiler.py` & `eth_wake-4.8.0/wake/lsp/lsp_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import platform
 import re
 import threading
 import time
 import traceback
 from collections import deque
 from copy import deepcopy
+from dataclasses import dataclass
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Deque,
@@ -144,14 +145,21 @@
 
 class CustomFileChangeCommand(StrEnum):
     FORCE_RECOMPILE = "force_recompile"
     FORCE_RERUN_DETECTORS = "force_rerun_detectors"
     FORCE_RERUN_PRINTERS = "force_rerun_printers"
 
 
+@dataclass
+class ConfigUpdate:
+    update: Dict
+    removed_options: Set
+    local_config_path: Path
+
+
 class DetectionAdditionalInfo(LspModel):
     impact: DetectorImpact
     confidence: DetectorConfidence
     ignored: bool
     source_unit_name: str
 
     def __members(self) -> Tuple:
@@ -405,14 +413,21 @@
             RenameFilesParams,
             DeleteFilesParams,
         ],
     ) -> None:
         self.output_ready.clear()
         await self.__file_changes_queue.put(change)
 
+    async def update_config(
+        self, update: Dict, removed_options: Set, local_config_path: Path
+    ):
+        await self.__file_changes_queue.put(
+            ConfigUpdate(update, removed_options, local_config_path)
+        )
+
     async def force_recompile(self) -> None:
         self.__output_ready.clear()
         await self.__file_changes_queue.put(CustomFileChangeCommand.FORCE_RECOMPILE)
 
     async def force_rerun_detectors(self) -> None:
         await self.__file_changes_queue.put(
             CustomFileChangeCommand.FORCE_RERUN_DETECTORS
@@ -468,14 +483,16 @@
 
     async def _handle_change(
         self,
         change: Union[
             DidOpenTextDocumentParams,
             DidCloseTextDocumentParams,
             DidChangeTextDocumentParams,
+            CustomFileChangeCommand,
+            ConfigUpdate,
             None,
         ],
     ) -> None:
         if isinstance(change, CustomFileChangeCommand):
             if change == CustomFileChangeCommand.FORCE_RECOMPILE:
                 for file in self.__discovered_files:
                     # clear diagnostics
@@ -493,14 +510,17 @@
                         self.__discovered_files.add(file)
 
                 self.__force_compile_files.update(self.__discovered_files)
             elif change == CustomFileChangeCommand.FORCE_RERUN_DETECTORS:
                 self.__force_run_detectors = True
             elif change == CustomFileChangeCommand.FORCE_RERUN_PRINTERS:
                 self.__force_run_printers = True
+        elif isinstance(change, ConfigUpdate):
+            self.__config.local_config_path = change.local_config_path
+            self.__config.update(change.update, change.removed_options)
         elif isinstance(change, CreateFilesParams):
             for file in change.files:
                 path = uri_to_path(file.uri)
                 if (
                     path not in self.__discovered_files
                     and not self.__file_excluded(path)
                     and path.suffix == ".sol"
@@ -628,22 +648,29 @@
             self.__interval_trees.clear()
             self.__source_units.clear()
             self.__ir_reference_resolver.clear_all_indexed_nodes()
             return
 
         try:
             if full_compile:
-                graph, _ = self.__compiler.build_graph(
+                graph, source_units_to_paths = self.__compiler.build_graph(
                     self.__discovered_files,
                     {
                         path: info.text.encode("utf-8")
                         for path, info in self.__opened_files.items()
                     },
                     True,
                 )
+
+                # add to deleted files previously compiled files that are now excluded from build
+                # will trigger post-destroy callbacks and remove them from source units
+                for p in self.__source_units:
+                    # use graph.nodes - i.e. discovered files + their dependencies from exclude paths
+                    if p not in source_units_to_paths.values():
+                        self.__deleted_files.add(p)
                 self.__last_graph = graph
             else:
                 graph, _ = self.__compiler.build_graph(
                     files_to_compile,
                     {
                         path: info.text.encode("utf-8")
                         for path, info in self.__opened_files.items()
@@ -693,24 +720,28 @@
             for cu in compilation_units:
                 if versions & cu.versions:
                     source_unit_names |= cu.source_unit_names
                     versions &= cu.versions
                 else:
                     merged_compilation_units.append(
                         CompilationUnit(
-                            graph.subgraph(source_unit_names).copy(),
+                            graph.subgraph(
+                                source_unit_names
+                            ).copy(),  # pyright: ignore reportArgumentType
                             versions,
                         )
                     )
                     source_unit_names = set(cu.source_unit_names)
                     versions = cu.versions
 
             merged_compilation_units.append(
                 CompilationUnit(
-                    graph.subgraph(source_unit_names).copy(),
+                    graph.subgraph(
+                        source_unit_names
+                    ).copy(),  # pyright: ignore reportArgumentType
                     versions,
                 )
             )
 
             compilation_units = merged_compilation_units
 
         target_versions = []
@@ -1161,14 +1192,21 @@
                 f"Exception occurred while running printers:\n{traceback.format_exc()}",
                 MessageType.ERROR,
             )
 
         if progress_token is not None:
             await self.__server.progress_end(progress_token)
 
+        commands = self.__printers_lsp_provider.get_commands()
+        if len(commands) > 0:
+            self.__printers_lsp_provider.clear_commands()
+            await self.__server.send_notification(
+                "wake/executeCommands", list(commands)
+            )
+
         # make sure that code lenses are refreshed
         try:
             await self.__server.send_request(
                 RequestMethodEnum.WORKSPACE_CODE_LENS_REFRESH, None
             )
         except LspError:
             pass
```

### Comparing `eth_wake-4.7.0/wake/lsp/lsp_parser.py` & `eth_wake-4.8.0/wake/lsp/lsp_parser.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/methods.py` & `eth_wake-4.8.0/wake/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/protocol_structures.py` & `eth_wake-4.8.0/wake/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/rpc_protocol.py` & `eth_wake-4.8.0/wake/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/server.py` & `eth_wake-4.8.0/wake/lsp/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     GENERATE_INHERITANCE_GRAPH = "wake.generate.inheritance_graph"
     GENERATE_INHERITANCE_GRAPH_FULL = "wake.generate.inheritance_graph_full"
     GENERATE_LINEARIZED_INHERITANCE_GRAPH = "wake.generate.linearized_inheritance_graph"
     LSP_FORCE_RECOMPILE = "wake.lsp.force_recompile"
     LSP_FORCE_RERUN_DETECTORS = "wake.lsp.force_rerun_detectors"
     INIT_DETECTOR = "wake.init.detector"
     INIT_PRINTER = "wake.init.printer"
+    CALLBACK = "wake.callback"
 
 
 def key_in_nested_dict(key: Tuple, d: Dict) -> bool:
     try:
         for k in key:
             d = d[k]
         return True
@@ -839,28 +840,34 @@
                     context.config.project_root_path
                     / raw_config["configuration"]["toml_path"]
                 )
             if "use_toml_if_present" in raw_config["configuration"]:
                 context.use_toml = raw_config["configuration"]["use_toml_if_present"]
             raw_config.pop("configuration")
 
+        config_clone = WakeConfig.fromdict(
+            context.config.todict(), project_root_path=context.config.project_root_path
+        )
+
         if context.use_toml and context.toml_path.exists():
             if (
                 original_toml_path != context.toml_path
                 or original_use_toml != context.use_toml
             ):
                 try:
                     config = WakeConfig(
                         local_config_path=context.toml_path,
                         project_root_path=context.config.project_root_path,
                     )
                     config.load_configs()
 
-                    context.config.local_config_path = context.toml_path
-                    changed = context.config.update(config.todict(), set())
+                    local_config_path = context.toml_path
+                    config_update = config.todict()
+                    removed_options = set()
+                    changed = config_clone.update(config_update, removed_options)
                 except tomli.TOMLDecodeError:
                     await self.log_message(
                         f"Failed to parse {context.toml_path}.",
                         MessageType.ERROR,
                     )
                     await self.show_message(
                         f"Failed to parse {context.toml_path}.",
@@ -869,37 +876,49 @@
                     return
                 except ValidationError as e:
                     message = f"TOML config file validation error:\n{e}"
                     await self.log_message(message, MessageType.ERROR)
                     await self.show_message(message, MessageType.ERROR)
                     return
             else:
+                local_config_path = context.config.local_config_path  # still the same
                 changed = {}
+                config_update = {}
+                removed_options = set()
         else:
             raw_config_copy = deepcopy(raw_config)
             (
                 raw_config_copy,
                 invalid_options,
                 removed_options,
             ) = await self._parse_config(
                 raw_config_copy, context.config.project_root_path
             )
 
-            changed = context.config.update(
-                raw_config_copy, invalid_options.union(removed_options)
-            )
+            config_update = raw_config_copy
+            local_config_path = context.config.local_config_path
+            removed_options = invalid_options.union(removed_options)
+            changed = config_clone.update(config_update, removed_options)
+
+        await context.compiler.update_config(
+            config_update, removed_options, local_config_path
+        )
 
         if key_in_nested_dict(("compiler", "solc"), changed):
             await context.compiler.force_recompile()
         if (
             key_in_nested_dict(("lsp", "detectors"), changed)
             or key_in_nested_dict(("detectors",), changed)
             or key_in_nested_dict(("detector",), changed)
         ):
             await context.compiler.force_rerun_detectors()
+        if key_in_nested_dict(("printers",), changed) or key_in_nested_dict(
+            ("printer",), changed
+        ):
+            await context.compiler.force_rerun_printers()
         if key_in_nested_dict(("lsp", "code_lens"), changed):
             try:
                 await self.send_request(
                     RequestMethodEnum.WORKSPACE_CODE_LENS_REFRESH, None
                 )
             except LspError:
                 pass
@@ -992,34 +1011,50 @@
 
     async def _workspace_did_change_watched_files(
         self, params: DidChangeWatchedFilesParams
     ) -> None:
         latest_configuration = None
 
         for context in self.__workspaces.values():
+            config_clone = WakeConfig.fromdict(
+                context.config.todict(),
+                project_root_path=context.config.project_root_path,
+            )
+
             if (
                 context.use_toml
                 and context.toml_path.exists()
                 and any(ch.uri.lower().endswith(".toml") for ch in params.changes)
             ):
                 try:
                     config = WakeConfig(
                         local_config_path=context.toml_path,
                         project_root_path=context.config.project_root_path,
                     )
                     config.load_configs()
 
-                    changed = context.config.update(config.todict(), set())
+                    config_update = config.todict()
+                    changed = config_clone.update(config_update, set())
+
+                    await context.compiler.update_config(
+                        config_update, set(), context.toml_path
+                    )
 
                     if key_in_nested_dict(("compiler", "solc"), changed):
                         await context.compiler.force_recompile()
-                    if key_in_nested_dict(
-                        ("lsp", "detectors"), changed
-                    ) or key_in_nested_dict(("detectors",), changed):
+                    if (
+                        key_in_nested_dict(("lsp", "detectors"), changed)
+                        or key_in_nested_dict(("detectors",), changed)
+                        or key_in_nested_dict(("detector",), changed)
+                    ):
                         await context.compiler.force_rerun_detectors()
+                    if key_in_nested_dict(("printers",), changed) or key_in_nested_dict(
+                        ("printer",), changed
+                    ):
+                        await context.compiler.force_rerun_printers()
                     if key_in_nested_dict(("lsp", "code_lens"), changed):
                         try:
                             await self.send_request(
                                 RequestMethodEnum.WORKSPACE_CODE_LENS_REFRESH, None
                             )
                         except LspError:
                             pass
@@ -1074,15 +1109,18 @@
         self, params: DidChangeConfigurationParams
     ) -> None:
         logger.debug(f"Received configuration change: {params}")
         if "wake" in params.settings:
             for context in self.__workspaces.values():
                 await self._handle_config_change(context, params.settings["wake"])
 
-    async def _get_workspace(self, uri: DocumentUri) -> LspContext:
+    async def _get_workspace(
+        self,
+        uri: DocumentUri,  # pyright: ignore reportInvalidTypeForm
+    ) -> LspContext:
         path = uri_to_path(uri)
         matching_workspaces = []
         for workspace in self.__workspaces.values():
             try:
                 matching_workspaces.append(
                     (workspace, path.relative_to(workspace.config.project_root_path))
                 )
@@ -1312,14 +1350,40 @@
                 global_ = bool(params.arguments[1])
                 return await init_printer_handler(self.__main_workspace, name, global_)
             else:
                 raise LspError(
                     ErrorCodes.InvalidParams,
                     f"Expected 2 arguments for `{CommandsEnum.INIT_PRINTER}` command",
                 )
+        elif command == CommandsEnum.CALLBACK:
+            if params.arguments is not None and len(params.arguments) == 3:
+                if params.arguments[1] not in {"detector", "printer"}:
+                    raise LspError(
+                        ErrorCodes.InvalidParams,
+                        f"Invalid callback type: {params.arguments[1]}",
+                    )
+                document_uri = DocumentUri(params.arguments[0])
+                context = await self._get_workspace(document_uri)
+                if params.arguments[1] == "detector":
+                    context.detectors_lsp_provider.get_callback(params.arguments[2])()
+                else:
+                    context.printers_lsp_provider.get_callback(params.arguments[2])()
+
+                commands = context.printers_lsp_provider.get_commands()
+                if len(commands) > 0:
+                    context.printers_lsp_provider.clear_commands()
+                    await self.send_notification(
+                        "wake/executeCommands", {"commands": commands}
+                    )
+                return ""  # TODO
+            else:
+                raise LspError(
+                    ErrorCodes.InvalidParams,
+                    f"Expected 3 arguments for `{CommandsEnum.CALLBACK}` command",
+                )
 
         raise LspError(ErrorCodes.InvalidRequest, f"Unknown command: {command}")
 
     async def get_configuration(self) -> None:
         params = ConfigurationParams(
             items=[
                 ConfigurationItem(
```

### Comparing `eth_wake-4.7.0/wake/lsp/server_capabilities.py` & `eth_wake-4.8.0/wake/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/lsp/utils/position.py` & `eth_wake-4.8.0/wake/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/migrations/woke_wake_migration.py` & `eth_wake-4.8.0/wake/migrations/woke_wake_migration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/migrations/xdg_migration.py` & `eth_wake-4.8.0/wake/migrations/xdg_migration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/printers/api.py` & `eth_wake-4.8.0/wake/printers/api.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/regex_parser/solidity_import.py` & `eth_wake-4.8.0/wake/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/regex_parser/solidity_parser.py` & `eth_wake-4.8.0/wake/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/svm/abc.py` & `eth_wake-4.8.0/wake/svm/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/svm/svm.py` & `eth_wake-4.8.0/wake/svm/svm.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/__init__.py` & `eth_wake-4.8.0/wake/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/core.py` & `eth_wake-4.8.0/wake/testing/core.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/coverage.py` & `eth_wake-4.8.0/wake/testing/coverage.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/fuzzing/fuzz_test.py` & `eth_wake-4.8.0/wake/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/fuzzing/fuzzer.py` & `eth_wake-4.8.0/wake/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/fuzzing/generators.py` & `eth_wake-4.8.0/wake/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/testing/pytest_plugin_multiprocess.py` & `eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,7 +238,11 @@
                 nodeid,
                 location,
             )
         )
 
     def pytest_sessionfinish(self, session: Session, exitstatus: int):
         self._queue.put(("pytest_sessionfinish", self._index, exitstatus))
+
+    def pytest_terminal_summary(self, terminalreporter, exitstatus, config):
+        terminalreporter.section("Wake")
+        terminalreporter.write_line("Random seed: " + self._random_seed.hex())
```

### Comparing `eth_wake-4.7.0/wake/testing/pytest_plugin_multiprocess_server.py` & `eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,18 @@
         finally:
             print("")
             for report in reports:
                 session.config.hook.pytest_runtest_logreport(report=report)
 
         return True
 
+    def pytest_terminal_summary(self, terminalreporter, exitstatus, config):
+        terminalreporter.section("Wake")
+        terminalreporter.write_line("Random seeds: " + ", ".join(s.hex() for s in self._random_seeds[:self._proc_count]))
+
     def _update_progress(
         self,
         progress: rich.progress.Progress,
         index: int,
         task_id: rich.progress.TaskID,
         current_test: Optional[str],
         test_reports: Dict[str, str],
```

### Comparing `eth_wake-4.7.0/wake/testing/pytest_plugin_single.py` & `eth_wake-4.8.0/wake/testing/pytest_plugin_single.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,7 +85,11 @@
                     [coverage_handler.get_contract_ide_coverage()]
                 )
                 write_coverage(c, self._config.project_root_path / "wake-coverage.cov")
 
             chain_interfaces_manager.close_all()
 
         return True
+
+    def pytest_terminal_summary(self, terminalreporter, exitstatus, config):
+        terminalreporter.section("Wake")
+        terminalreporter.write_line("Random seed: " + self._random_seeds[0].hex())
```

### Comparing `eth_wake-4.7.0/wake/utils/context_managers.py` & `eth_wake-4.8.0/wake/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/decorators.py` & `eth_wake-4.8.0/wake/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/file_utils.py` & `eth_wake-4.8.0/wake/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/formatters.py` & `eth_wake-4.8.0/wake/utils/formatters.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/general.py` & `eth_wake-4.8.0/wake/utils/general.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/null_file.py` & `eth_wake-4.8.0/wake/utils/null_file.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/openzeppelin.py` & `eth_wake-4.8.0/wake/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/string.py` & `eth_wake-4.8.0/wake/utils/string.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/tee.py` & `eth_wake-4.8.0/wake/utils/tee.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake/utils/threaded_child_watcher.py` & `eth_wake-4.8.0/wake/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/__init__.py` & `eth_wake-4.8.0/wake_detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/abi_encode_with_signature.py` & `eth_wake-4.8.0/wake_detectors/abi_encode_with_signature.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/axelar_proxy_contract_id.py` & `eth_wake-4.8.0/wake_detectors/axelar_proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/balance_relied_on.py` & `eth_wake-4.8.0/wake_detectors/balance_relied_on.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/call_options_not_called.py` & `eth_wake-4.8.0/wake_detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py` & `eth_wake-4.8.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/complex_struct_getter.py` & `eth_wake-4.8.0/wake_detectors/complex_struct_getter.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/empty_byte_array_copy_bug.py` & `eth_wake-4.8.0/wake_detectors/empty_byte_array_copy_bug.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/incorrect_interface.py` & `eth_wake-4.8.0/wake_detectors/incorrect_interface.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/missing_return.py` & `eth_wake-4.8.0/wake_detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/msg_value_nonpayable_function.py` & `eth_wake-4.8.0/wake_detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/reentrancy.py` & `eth_wake-4.8.0/wake_detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/struct_mapping_deletion.py` & `eth_wake-4.8.0/wake_detectors/struct_mapping_deletion.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/tx_origin.py` & `eth_wake-4.8.0/wake_detectors/tx_origin.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unchecked_return_value.py` & `eth_wake-4.8.0/wake_detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unprotected_selfdestruct.py` & `eth_wake-4.8.0/wake_detectors/unprotected_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unsafe_delegatecall.py` & `eth_wake-4.8.0/wake_detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unsafe_erc20_call.py` & `eth_wake-4.8.0/wake_detectors/unsafe_erc20_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unused_contract.py` & `eth_wake-4.8.0/wake_detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unused_function.py` & `eth_wake-4.8.0/wake_detectors/unused_function.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unused_import.py` & `eth_wake-4.8.0/wake_detectors/unused_import.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_detectors/unused_modifier.py` & `eth_wake-4.8.0/wake_detectors/unused_modifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/abi.py` & `eth_wake-4.8.0/wake_printers/abi.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/c3_linearization.py` & `eth_wake-4.8.0/wake_printers/c3_linearization.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/control_flow_graph.py` & `eth_wake-4.8.0/wake_printers/control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/imports_graph.py` & `eth_wake-4.8.0/wake_printers/imports_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/inheritance_graph.py` & `eth_wake-4.8.0/wake_printers/inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/inheritance_tree.py` & `eth_wake-4.8.0/wake_printers/inheritance_tree.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/modifiers.py` & `eth_wake-4.8.0/wake_printers/modifiers.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/state_changes.py` & `eth_wake-4.8.0/wake_printers/state_changes.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/storage_layout.py` & `eth_wake-4.8.0/wake_printers/storage_layout.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/wake_printers/tokens.py` & `eth_wake-4.8.0/wake_printers/tokens.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.7.0/PKG-INFO` & `eth_wake-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-wake
-Version: 4.7.0
+Version: 4.8.0
 Summary: Wake is a Python-based Solidity development and testing framework with built-in vulnerability detectors.
 Home-page: https://getwake.io
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,static analysis,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
```

