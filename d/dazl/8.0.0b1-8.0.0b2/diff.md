# Comparing `tmp/dazl-8.0.0b1.tar.gz` & `tmp/dazl-8.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dazl-8.0.0b1.tar", max compression
+gzip compressed data, was "dazl-8.0.0b2.tar", max compression
```

## Comparing `dazl-8.0.0b1.tar` & `dazl-8.0.0b2.tar`

### file list

```diff
@@ -1,553 +1,553 @@
--rw-r--r--   0        0        0    11393 2024-02-17 22:53:35.749987 dazl-8.0.0b1/LICENSE
--rw-r--r--   0        0        0     2725 2024-02-17 22:53:35.750514 dazl-8.0.0b1/README.md
--rw-r--r--   0        0        0     2673 2024-02-17 22:53:36.227267 dazl-8.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      333 2024-02-17 22:53:36.227347 dazl-8.0.0b1/python/_dazl/__init__.py
--rw-r--r--   0        0        0      887 2024-02-17 22:53:36.227408 dazl-8.0.0b1/python/_dazl/__main__.py
--rw-r--r--   0        0        0     1476 2024-02-17 22:53:36.227467 dazl-8.0.0b1/python/_dazl/_logging.py
--rw-r--r--   0        0        0      276 2024-02-17 22:53:36.227535 dazl-8.0.0b1/python/_dazl/codegen/__init__.py
--rw-r--r--   0        0        0     5483 2024-02-17 22:53:36.227613 dazl-8.0.0b1/python/_dazl/codegen/go.py
--rw-r--r--   0        0        0      347 2024-02-17 22:53:36.227677 dazl-8.0.0b1/python/_dazl/codegen/go_header.py
--rw-r--r--   0        0        0     1728 2024-02-17 22:53:36.227737 dazl-8.0.0b1/python/_dazl/codegen/python.py
--rw-r--r--   0        0        0     5092 2024-02-17 22:53:36.227814 dazl-8.0.0b1/python/_dazl/codegen/python_grpc_pyi.py
--rw-r--r--   0        0        0      339 2024-02-17 22:53:36.227873 dazl-8.0.0b1/python/_dazl/codegen/python_header.py
--rw-r--r--   0        0        0     2442 2024-02-17 22:53:36.227934 dazl-8.0.0b1/python/_dazl/codegen/python_init.py
--rw-r--r--   0        0        0      520 2024-02-17 22:53:36.227993 dazl-8.0.0b1/python/_dazl/codegen/util.py
--rw-r--r--   0        0        0      944 2024-04-03 22:04:33.683110 dazl-8.0.0b1/python/_dazl/collections.py
--rw-r--r--   0        0        0     4095 2024-02-17 22:53:36.228120 dazl-8.0.0b1/python/_dazl/download/__init__.py
--rw-r--r--   0        0        0     3147 2024-02-17 22:53:36.228186 dazl-8.0.0b1/python/_dazl/protoc/__init__.py
--rw-r--r--   0        0        0     2027 2024-04-03 22:04:33.695507 dazl-8.0.0b1/python/_dazl/protopack/__init__.py
--rw-r--r--   0        0        0     4306 2024-02-17 22:53:36.228348 dazl-8.0.0b1/python/_dazl/protopack/rename.py
--rw-r--r--   0        0        0     3180 2024-02-17 22:53:36.228419 dazl-8.0.0b1/python/_dazl/protopack/rewrite.py
--rw-r--r--   0        0        0      221 2024-02-17 22:53:36.228490 dazl-8.0.0b1/python/_dazl/syntax/__init__.py
--rw-r--r--   0        0        0      601 2024-02-17 22:53:36.228554 dazl-8.0.0b1/python/_dazl/syntax/python/__init__.py
--rw-r--r--   0        0        0      586 2024-02-17 22:53:36.228610 dazl-8.0.0b1/python/_dazl/syntax/python/_basic.py
--rw-r--r--   0        0        0     6389 2024-02-17 22:53:36.228696 dazl-8.0.0b1/python/_dazl/syntax/python/imports.py
--rw-r--r--   0        0        0     2683 2024-02-17 22:53:36.228762 dazl-8.0.0b1/python/_dazl/syntax/python/pb.py
--rw-r--r--   0        0        0     7328 2024-02-17 22:53:36.228847 dazl-8.0.0b1/python/_dazl/syntax/python/symbols.py
--rw-r--r--   0        0        0     2793 2024-02-17 22:53:36.228907 dazl-8.0.0b1/python/_dazl/syntax/python/types.py
--rw-r--r--   0        0        0     2188 2024-02-17 22:53:36.229013 dazl-8.0.0b1/python/_dazl/update.py
--rw-r--r--   0        0        0     1737 2024-02-17 22:53:35.796705 dazl-8.0.0b1/python/dazl/__init__.py
--rw-r--r--   0        0        0      311 2024-02-17 22:53:35.796859 dazl-8.0.0b1/python/dazl/__main__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797029 dazl-8.0.0b1/python/dazl/_gen/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797159 dazl-8.0.0b1/python/dazl/_gen/com/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797280 dazl-8.0.0b1/python/dazl/_gen/com/daml/__init__.py
--rw-r--r--   0        0        0     1525 2024-02-17 22:53:36.229174 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py
--rw-r--r--   0        0        0    52179 2024-02-17 22:53:35.797603 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py
--rw-r--r--   0        0        0    78370 2024-02-17 22:53:35.797866 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi
--rw-r--r--   0        0        0     2298 2024-02-17 22:53:35.798460 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py
--rw-r--r--   0        0        0     1486 2024-02-17 22:53:35.798607 dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798740 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798859 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/__init__.py
--rw-r--r--   0        0        0     6188 2024-02-17 22:53:36.229442 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py
--rw-r--r--   0        0        0     2961 2024-02-17 22:53:35.799137 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
--rw-r--r--   0        0        0     1801 2024-02-17 22:53:35.799270 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi
--rw-r--r--   0        0        0     4390 2024-02-17 22:53:35.799437 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
--rw-r--r--   0        0        0     2396 2024-02-17 22:53:35.799592 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4542 2024-02-17 22:53:36.229586 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
--rw-r--r--   0        0        0     3967 2024-02-17 22:53:35.799910 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
--rw-r--r--   0        0        0     2714 2024-02-17 22:53:35.800064 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi
--rw-r--r--   0        0        0     6347 2024-02-17 22:53:35.800242 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3579 2024-02-17 22:53:35.800388 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     6304 2024-02-17 22:53:35.800524 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py
--rw-r--r--   0        0        0     4309 2024-02-17 22:53:35.800651 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi
--rw-r--r--   0        0        0    17920 2024-02-17 22:53:35.800772 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py
--rw-r--r--   0        0        0     8410 2024-02-17 22:53:35.800952 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3043 2024-02-17 22:53:35.801100 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py
--rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.801369 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi
--rw-r--r--   0        0        0     3683 2024-02-17 22:53:35.801517 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py
--rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.801662 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2218 2024-02-17 22:53:35.801796 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py
--rw-r--r--   0        0        0     1145 2024-02-17 22:53:35.801924 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi
--rw-r--r--   0        0        0     3426 2024-02-17 22:53:35.802064 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
--rw-r--r--   0        0        0     2113 2024-02-17 22:53:35.802196 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi
--rw-r--r--   0        0        0     6681 2024-02-17 22:53:35.802377 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3660 2024-02-17 22:53:35.802530 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2325 2024-02-17 22:53:35.802674 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
--rw-r--r--   0        0        0      995 2024-02-17 22:53:35.802815 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi
--rw-r--r--   0        0        0     4791 2024-02-17 22:53:35.802976 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
--rw-r--r--   0        0        0     2225 2024-02-17 22:53:35.803122 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     6691 2024-02-17 22:53:35.803305 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
--rw-r--r--   0        0        0     5361 2024-02-17 22:53:35.803473 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi
--rw-r--r--   0        0        0    19490 2024-02-17 22:53:35.803626 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     9064 2024-02-17 22:53:35.803836 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     9901 2024-02-17 22:53:35.804032 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py
--rw-r--r--   0        0        0     8928 2024-02-17 22:53:35.804213 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi
--rw-r--r--   0        0        0    25223 2024-02-17 22:53:35.804374 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    12691 2024-02-17 22:53:35.804590 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3879 2024-02-17 22:53:35.804732 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
--rw-r--r--   0        0        0     2724 2024-02-17 22:53:35.804879 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi
--rw-r--r--   0        0        0     7734 2024-02-17 22:53:35.805059 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
--rw-r--r--   0        0        0     3690 2024-02-17 22:53:35.805215 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3899 2024-02-17 22:53:35.805363 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
--rw-r--r--   0        0        0     2096 2024-02-17 22:53:35.805498 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi
--rw-r--r--   0        0        0    10939 2024-02-17 22:53:35.805669 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
--rw-r--r--   0        0        0     6396 2024-02-17 22:53:35.805827 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2250 2024-02-17 22:53:35.805984 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
--rw-r--r--   0        0        0      764 2024-02-17 22:53:35.806133 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi
--rw-r--r--   0        0        0     5656 2024-02-17 22:53:35.806304 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
--rw-r--r--   0        0        0     2220 2024-02-17 22:53:35.806432 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     6717 2024-02-17 22:53:35.806618 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
--rw-r--r--   0        0        0     7479 2024-02-17 22:53:35.806802 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi
--rw-r--r--   0        0        0     2481 2024-02-17 22:53:35.806959 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
--rw-r--r--   0        0        0     1851 2024-02-17 22:53:35.807108 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi
--rw-r--r--   0        0        0     2007 2024-02-17 22:53:35.807250 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py
--rw-r--r--   0        0        0     1023 2024-02-17 22:53:35.807378 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi
--rw-r--r--   0        0        0     5333 2024-02-17 22:53:35.807559 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
--rw-r--r--   0        0        0     6277 2024-02-17 22:53:35.807737 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi
--rw-r--r--   0        0        0     3878 2024-02-17 22:53:35.807846 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py
--rw-r--r--   0        0        0     2869 2024-02-17 22:53:35.807954 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi
--rw-r--r--   0        0        0     5706 2024-02-17 22:53:35.808080 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py
--rw-r--r--   0        0        0     3753 2024-02-17 22:53:35.808181 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     7614 2024-02-17 22:53:35.808362 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py
--rw-r--r--   0        0        0     7919 2024-02-17 22:53:35.808535 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi
--rw-r--r--   0        0        0     2840 2024-02-17 22:53:35.808687 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
--rw-r--r--   0        0        0     1333 2024-02-17 22:53:35.808832 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi
--rw-r--r--   0        0        0     3789 2024-02-17 22:53:35.808969 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     2480 2024-02-17 22:53:35.809097 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2941 2024-02-17 22:53:35.809229 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
--rw-r--r--   0        0        0      712 2024-02-17 22:53:35.809371 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi
--rw-r--r--   0        0        0     4024 2024-02-17 22:53:35.809532 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
--rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.809685 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2039 2024-02-17 22:53:35.809821 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
--rw-r--r--   0        0        0     1158 2024-02-17 22:53:35.809960 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi
--rw-r--r--   0        0        0     3815 2024-02-17 22:53:35.810109 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
--rw-r--r--   0        0        0     2815 2024-02-17 22:53:35.810258 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi
--rw-r--r--   0        0        0     6970 2024-02-17 22:53:35.810436 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
--rw-r--r--   0        0        0     4809 2024-02-17 22:53:35.810602 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      406 2024-02-17 22:53:35.810747 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
--rw-r--r--   0        0        0     2913 2024-02-17 22:53:35.810888 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
--rw-r--r--   0        0        0     1550 2024-02-17 22:53:35.811025 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi
--rw-r--r--   0        0        0     5129 2024-02-17 22:53:35.811190 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
--rw-r--r--   0        0        0     3379 2024-02-17 22:53:35.811324 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3327 2024-02-17 22:53:35.811469 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
--rw-r--r--   0        0        0     2554 2024-02-17 22:53:35.811605 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi
--rw-r--r--   0        0        0     3685 2024-02-17 22:53:35.811740 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
--rw-r--r--   0        0        0     3347 2024-02-17 22:53:35.811873 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi
--rw-r--r--   0        0        0     6625 2024-02-17 22:53:35.812036 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
--rw-r--r--   0        0        0     5153 2024-02-17 22:53:35.812194 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi
--rw-r--r--   0        0        0    18252 2024-02-17 22:53:35.812341 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
--rw-r--r--   0        0        0    11776 2024-02-17 22:53:35.812536 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5817 2024-02-17 22:53:35.812698 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
--rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.812851 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi
--rw-r--r--   0        0        0     3221 2024-02-17 22:53:35.812983 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
--rw-r--r--   0        0        0     2064 2024-02-17 22:53:35.813118 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi
--rw-r--r--   0        0        0     3207 2024-02-17 22:53:35.813255 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
--rw-r--r--   0        0        0     2293 2024-02-17 22:53:35.813390 dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813522 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813647 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813766 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.814533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/__init__.py
--rw-r--r--   0        0        0     1940 2024-02-17 22:53:35.814700 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/__init__.py
--rw-r--r--   0        0        0    11447 2024-02-17 22:53:36.229775 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.py
--rw-r--r--   0        0        0     9455 2024-02-17 22:53:35.814982 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.pyi
--rw-r--r--   0        0        0    29764 2024-02-17 22:53:35.815101 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.py
--rw-r--r--   0        0        0    16810 2024-02-17 22:53:35.815230 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     1030 2024-02-17 22:53:35.815381 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/__init__.py
--rw-r--r--   0        0        0     8612 2024-02-17 22:53:36.229948 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.py
--rw-r--r--   0        0        0     9794 2024-02-17 22:53:35.815639 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815757 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/__init__.py
--rw-r--r--   0        0        0     3128 2024-02-17 22:53:36.230077 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-17 22:53:36.230195 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.py
--rw-r--r--   0        0        0     1153 2024-02-17 22:53:35.816155 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.pyi
--rw-r--r--   0        0        0     3526 2024-02-17 22:53:35.816255 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     2257 2024-02-17 22:53:35.816350 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4279 2024-02-17 22:53:36.230361 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.py
--rw-r--r--   0        0        0     2594 2024-02-17 22:53:35.816602 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.pyi
--rw-r--r--   0        0        0     7501 2024-02-17 22:53:35.816727 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.py
--rw-r--r--   0        0        0     4941 2024-02-17 22:53:35.816854 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3638 2024-02-17 22:53:36.230477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.py
--rw-r--r--   0        0        0      858 2024-02-17 22:53:35.817036 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.pyi
--rw-r--r--   0        0        0    18541 2024-02-17 22:53:35.817152 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.py
--rw-r--r--   0        0        0    11361 2024-02-17 22:53:35.817304 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     7888 2024-02-17 22:53:36.230593 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.py
--rw-r--r--   0        0        0     4680 2024-02-17 22:53:35.817518 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.pyi
--rw-r--r--   0        0        0    25680 2024-02-17 22:53:35.817632 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.py
--rw-r--r--   0        0        0    15191 2024-02-17 22:53:35.817820 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.230708 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.py
--rw-r--r--   0        0        0     1904 2024-02-17 22:53:35.817978 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.pyi
--rw-r--r--   0        0        0     5932 2024-02-17 22:53:35.818106 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.py
--rw-r--r--   0        0        0     3678 2024-02-17 22:53:35.818203 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4424 2024-02-17 22:53:36.230855 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.py
--rw-r--r--   0        0        0     2976 2024-02-17 22:53:35.818423 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.pyi
--rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.818519 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.818618 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3800 2024-02-17 22:53:36.230977 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.py
--rw-r--r--   0        0        0     2706 2024-02-17 22:53:35.818787 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.pyi
--rw-r--r--   0        0        0     5644 2024-02-17 22:53:35.818916 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.py
--rw-r--r--   0        0        0     3720 2024-02-17 22:53:35.819018 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4972 2024-02-17 22:53:36.231102 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.py
--rw-r--r--   0        0        0     2651 2024-02-17 22:53:35.819215 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.pyi
--rw-r--r--   0        0        0    11631 2024-02-17 22:53:35.819360 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     6738 2024-02-17 22:53:36.231234 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.231353 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.py
--rw-r--r--   0        0        0     2174 2024-02-17 22:53:35.819629 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.pyi
--rw-r--r--   0        0        0     1916 2024-02-17 22:53:36.231467 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.py
--rw-r--r--   0        0        0      368 2024-02-17 22:53:35.819790 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.pyi
--rw-r--r--   0        0        0     3577 2024-02-17 22:53:35.819894 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.py
--rw-r--r--   0        0        0     2236 2024-02-17 22:53:35.819992 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      362 2024-02-17 22:53:35.820123 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/__init__.py
--rw-r--r--   0        0        0     2632 2024-02-17 22:53:36.231585 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.py
--rw-r--r--   0        0        0     1523 2024-02-17 22:53:35.820286 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.pyi
--rw-r--r--   0        0        0     5711 2024-02-17 22:53:36.231714 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.py
--rw-r--r--   0        0        0     5898 2024-02-17 22:53:35.820506 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.pyi
--rw-r--r--   0        0        0      825 2024-02-17 22:53:35.820637 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/__init__.py
--rw-r--r--   0        0        0     2930 2024-02-17 22:53:36.231843 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.py
--rw-r--r--   0        0        0     1682 2024-02-17 22:53:35.820805 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.pyi
--rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.820905 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.820999 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3392 2024-02-17 22:53:36.231947 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.py
--rw-r--r--   0        0        0     2186 2024-02-17 22:53:35.821159 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.pyi
--rw-r--r--   0        0        0     4358 2024-02-17 22:53:35.821284 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-02-17 22:53:35.821382 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.821508 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/__init__.py
--rw-r--r--   0        0        0     2030 2024-02-17 22:53:36.232068 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/__init__.py
--rw-r--r--   0        0        0     2000 2024-02-17 22:53:36.232185 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.py
--rw-r--r--   0        0        0      368 2024-02-17 22:53:35.821776 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.pyi
--rw-r--r--   0        0        0     3366 2024-02-17 22:53:35.821875 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2287 2024-02-17 22:53:35.822115 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.232290 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.py
--rw-r--r--   0        0        0     1796 2024-02-17 22:53:35.822288 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.pyi
--rw-r--r--   0        0        0     5273 2024-02-17 22:53:35.822416 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.py
--rw-r--r--   0        0        0     3430 2024-02-17 22:53:35.822515 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4927 2024-02-17 22:53:36.232409 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.py
--rw-r--r--   0        0        0     4070 2024-02-17 22:53:35.822715 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.pyi
--rw-r--r--   0        0        0     5949 2024-02-17 22:53:35.822844 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     3581 2024-02-17 22:53:35.822946 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5863 2024-02-17 22:53:36.232533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.py
--rw-r--r--   0        0        0     3374 2024-02-17 22:53:35.823157 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.pyi
--rw-r--r--   0        0        0    12411 2024-02-17 22:53:35.823336 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.py
--rw-r--r--   0        0        0     7875 2024-02-17 22:53:35.823465 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2409 2024-02-17 22:53:36.232649 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.py
--rw-r--r--   0        0        0     1790 2024-02-17 22:53:35.823639 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.pyi
--rw-r--r--   0        0        0     8931 2024-02-17 22:53:36.232813 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.py
--rw-r--r--   0        0        0     6904 2024-02-17 22:53:35.823888 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.pyi
--rw-r--r--   0        0        0    31573 2024-02-17 22:53:35.824004 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.py
--rw-r--r--   0        0        0    16744 2024-02-17 22:53:35.824127 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2015 2024-02-17 22:53:36.232930 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.py
--rw-r--r--   0        0        0      892 2024-02-17 22:53:35.824306 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.pyi
--rw-r--r--   0        0        0      274 2024-02-17 22:53:35.824436 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/__init__.py
--rw-r--r--   0        0        0     1978 2024-02-17 22:53:36.233033 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.py
--rw-r--r--   0        0        0     1150 2024-02-17 22:53:35.824596 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824718 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824840 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/__init__.py
--rw-r--r--   0        0        0      700 2024-02-17 22:53:35.824967 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/__init__.py
--rw-r--r--   0        0        0     7382 2024-02-17 22:53:36.233166 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.py
--rw-r--r--   0        0        0     7065 2024-02-17 22:53:35.825187 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.pyi
--rw-r--r--   0        0        0     5164 2024-02-17 22:53:35.825306 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.py
--rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.825398 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825518 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/__init__.py
--rw-r--r--   0        0        0     5756 2024-02-17 22:53:35.825809 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/__init__.py
--rw-r--r--   0        0        0    10342 2024-02-17 22:53:36.233353 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.py
--rw-r--r--   0        0        0     7925 2024-02-17 22:53:35.826054 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.pyi
--rw-r--r--   0        0        0    23356 2024-02-17 22:53:35.826172 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.py
--rw-r--r--   0        0        0    14253 2024-02-17 22:53:35.826358 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2258 2024-02-17 22:53:36.233483 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.py
--rw-r--r--   0        0        0      695 2024-02-17 22:53:35.826533 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.pyi
--rw-r--r--   0        0        0     3721 2024-02-17 22:53:35.826633 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2024-02-17 22:53:35.826853 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5241 2024-02-17 22:53:36.233620 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.py
--rw-r--r--   0        0        0     3208 2024-02-17 22:53:35.827057 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.pyi
--rw-r--r--   0        0        0    11122 2024-02-17 22:53:35.827192 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.py
--rw-r--r--   0        0        0     6364 2024-02-17 22:53:35.827314 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    11596 2024-02-17 22:53:36.233789 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.py
--rw-r--r--   0        0        0     9525 2024-02-17 22:53:35.827546 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.pyi
--rw-r--r--   0        0        0    33250 2024-02-17 22:53:35.827669 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.py
--rw-r--r--   0        0        0    21002 2024-02-17 22:53:35.827795 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5534 2024-02-17 22:53:36.233920 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.py
--rw-r--r--   0        0        0     4072 2024-02-17 22:53:35.828006 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.pyi
--rw-r--r--   0        0        0     9898 2024-02-17 22:53:35.828138 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.py
--rw-r--r--   0        0        0     6176 2024-02-17 22:53:35.828263 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2249 2024-02-17 22:53:36.234035 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.py
--rw-r--r--   0        0        0      832 2024-02-17 22:53:35.828433 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.pyi
--rw-r--r--   0        0        0     4589 2024-02-17 22:53:35.828559 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.py
--rw-r--r--   0        0        0     2395 2024-02-17 22:53:35.828662 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.pyi
--rw-r--r--   0        0        0     2960 2024-02-17 22:53:36.234150 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.py
--rw-r--r--   0        0        0     2330 2024-02-17 22:53:35.828823 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.pyi
--rw-r--r--   0        0        0     3234 2024-02-17 22:53:35.828919 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.py
--rw-r--r--   0        0        0     2091 2024-02-17 22:53:35.829017 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4466 2024-02-17 22:53:36.234278 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.py
--rw-r--r--   0        0        0     1906 2024-02-17 22:53:35.829213 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.pyi
--rw-r--r--   0        0        0    19105 2024-02-17 22:53:35.829321 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.py
--rw-r--r--   0        0        0    11105 2024-02-17 22:53:35.829485 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2309 2024-02-17 22:53:36.234404 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.py
--rw-r--r--   0        0        0      911 2024-02-17 22:53:35.829672 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.pyi
--rw-r--r--   0        0        0     5364 2024-02-17 22:53:35.829803 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3469 2024-02-17 22:53:35.829908 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2507 2024-02-17 22:53:36.234517 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.py
--rw-r--r--   0        0        0     1047 2024-02-17 22:53:35.830088 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.pyi
--rw-r--r--   0        0        0     3634 2024-02-17 22:53:35.830192 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.py
--rw-r--r--   0        0        0     2357 2024-02-17 22:53:35.830293 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5697 2024-02-17 22:53:36.234643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.py
--rw-r--r--   0        0        0     5622 2024-02-17 22:53:35.830510 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.pyi
--rw-r--r--   0        0        0     7628 2024-02-17 22:53:35.830634 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.py
--rw-r--r--   0        0        0     4909 2024-02-17 22:53:35.830760 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.830879 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/__init__.py
--rw-r--r--   0        0        0     1227 2024-02-17 22:53:35.831005 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/__init__.py
--rw-r--r--   0        0        0    16269 2024-02-17 22:53:36.234874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.py
--rw-r--r--   0        0        0    21287 2024-02-17 22:53:35.831279 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.pyi
--rw-r--r--   0        0        0     3318 2024-02-17 22:53:36.234997 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.py
--rw-r--r--   0        0        0     2205 2024-02-17 22:53:35.831462 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.831586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/__init__.py
--rw-r--r--   0        0        0     4582 2024-02-17 22:53:36.235225 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/__init__.py
--rw-r--r--   0        0        0     2069 2024-02-17 22:53:36.235360 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.py
--rw-r--r--   0        0        0     1456 2024-02-17 22:53:35.831874 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.pyi
--rw-r--r--   0        0        0     4351 2024-02-17 22:53:36.235489 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.py
--rw-r--r--   0        0        0     4153 2024-02-17 22:53:35.832097 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.pyi
--rw-r--r--   0        0        0     3340 2024-02-17 22:53:36.235615 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.py
--rw-r--r--   0        0        0     3275 2024-02-17 22:53:35.832262 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.pyi
--rw-r--r--   0        0        0     5709 2024-02-17 22:53:36.235748 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.py
--rw-r--r--   0        0        0     5991 2024-02-17 22:53:35.832480 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.pyi
--rw-r--r--   0        0        0     3817 2024-02-17 22:53:36.235861 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.py
--rw-r--r--   0        0        0     4555 2024-02-17 22:53:35.832670 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.pyi
--rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.235972 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.py
--rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.832840 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.pyi
--rw-r--r--   0        0        0    12436 2024-02-17 22:53:36.236180 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.py
--rw-r--r--   0        0        0    15054 2024-02-17 22:53:35.833159 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.pyi
--rw-r--r--   0        0        0     5560 2024-02-17 22:53:36.236308 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.py
--rw-r--r--   0        0        0     5503 2024-02-17 22:53:35.833382 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.pyi
--rw-r--r--   0        0        0     9990 2024-02-17 22:53:36.236477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.py
--rw-r--r--   0        0        0    12765 2024-02-17 22:53:35.833666 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.pyi
--rw-r--r--   0        0        0     1523 2024-02-17 22:53:36.236586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.py
--rw-r--r--   0        0        0      709 2024-02-17 22:53:35.833833 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.pyi
--rw-r--r--   0        0        0     5302 2024-02-17 22:53:36.236709 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.py
--rw-r--r--   0        0        0     5427 2024-02-17 22:53:35.834062 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.pyi
--rw-r--r--   0        0        0     2214 2024-02-17 22:53:36.236819 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.py
--rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.834226 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.pyi
--rw-r--r--   0        0        0    11115 2024-02-17 22:53:36.236972 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.py
--rw-r--r--   0        0        0    13925 2024-02-17 22:53:35.834499 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.pyi
--rw-r--r--   0        0        0     2787 2024-02-17 22:53:35.834625 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/__init__.py
--rw-r--r--   0        0        0     2404 2024-02-17 22:53:36.237090 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.py
--rw-r--r--   0        0        0     1515 2024-02-17 22:53:35.834780 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.pyi
--rw-r--r--   0        0        0     4869 2024-02-17 22:53:36.237227 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.py
--rw-r--r--   0        0        0     4409 2024-02-17 22:53:35.834991 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.pyi
--rw-r--r--   0        0        0     3035 2024-02-17 22:53:36.237347 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.py
--rw-r--r--   0        0        0     2788 2024-02-17 22:53:35.835144 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.pyi
--rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.237462 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.py
--rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.835281 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.pyi
--rw-r--r--   0        0        0     9401 2024-02-17 22:53:36.237635 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.py
--rw-r--r--   0        0        0    10568 2024-02-17 22:53:35.835548 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.pyi
--rw-r--r--   0        0        0     5513 2024-02-17 22:53:36.237766 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.py
--rw-r--r--   0        0        0     5720 2024-02-17 22:53:35.835760 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.pyi
--rw-r--r--   0        0        0     7000 2024-02-17 22:53:36.238013 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.py
--rw-r--r--   0        0        0     8939 2024-02-17 22:53:35.835987 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.pyi
--rw-r--r--   0        0        0     5100 2024-02-17 22:53:36.238150 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.py
--rw-r--r--   0        0        0     4441 2024-02-17 22:53:35.836194 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.pyi
--rw-r--r--   0        0        0     6336 2024-02-17 22:53:36.238289 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.py
--rw-r--r--   0        0        0     7245 2024-02-17 22:53:35.836409 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.pyi
--rw-r--r--   0        0        0     2342 2024-02-17 22:53:35.836543 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/__init__.py
--rw-r--r--   0        0        0     4494 2024-02-17 22:53:36.238432 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.py
--rw-r--r--   0        0        0     5711 2024-02-17 22:53:35.836833 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.pyi
--rw-r--r--   0        0        0     3405 2024-02-17 22:53:36.238565 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.py
--rw-r--r--   0        0        0     2687 2024-02-17 22:53:35.837015 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.pyi
--rw-r--r--   0        0        0     2797 2024-02-17 22:53:36.238686 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.py
--rw-r--r--   0        0        0     2318 2024-02-17 22:53:35.837236 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.pyi
--rw-r--r--   0        0        0     4570 2024-02-17 22:53:36.238816 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.py
--rw-r--r--   0        0        0     4998 2024-02-17 22:53:35.837489 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.pyi
--rw-r--r--   0        0        0     4089 2024-02-17 22:53:36.238938 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.py
--rw-r--r--   0        0        0     4314 2024-02-17 22:53:35.837659 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.pyi
--rw-r--r--   0        0        0     4288 2024-02-17 22:53:36.239072 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.py
--rw-r--r--   0        0        0     3511 2024-02-17 22:53:35.837971 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.pyi
--rw-r--r--   0        0        0    14188 2024-02-17 22:53:36.239292 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.py
--rw-r--r--   0        0        0    18723 2024-02-17 22:53:35.838244 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.pyi
--rw-r--r--   0        0        0      347 2024-02-17 22:53:35.838387 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/__init__.py
--rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.239423 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.py
--rw-r--r--   0        0        0     2681 2024-02-17 22:53:35.838556 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.pyi
--rw-r--r--   0        0        0     4895 2024-02-17 22:53:36.239540 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.py
--rw-r--r--   0        0        0     4326 2024-02-17 22:53:35.838746 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838864 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838999 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/__init__.py
--rw-r--r--   0        0        0      501 2024-02-17 22:53:35.839158 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/__init__.py
--rw-r--r--   0        0        0     5338 2024-02-17 22:53:36.239682 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.py
--rw-r--r--   0        0        0     4373 2024-02-17 22:53:35.839385 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839521 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839653 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/__init__.py
--rw-r--r--   0        0        0      333 2024-02-17 22:53:35.839777 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/__init__.py
--rw-r--r--   0        0        0     2582 2024-02-17 22:53:36.239829 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.py
--rw-r--r--   0        0        0     2054 2024-02-17 22:53:35.839944 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.pyi
--rw-r--r--   0        0        0      242 2024-02-17 22:53:35.840071 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/__init__.py
--rw-r--r--   0        0        0     1758 2024-02-17 22:53:36.239960 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.py
--rw-r--r--   0        0        0      759 2024-02-17 22:53:35.840231 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840341 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/__init__.py
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840467 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/__init__.py
--rw-r--r--   0        0        0     3459 2024-02-17 22:53:35.840596 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/__init__.py
--rw-r--r--   0        0        0     2985 2024-02-17 22:53:36.240102 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.py
--rw-r--r--   0        0        0     1696 2024-02-17 22:53:35.840769 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.pyi
--rw-r--r--   0        0        0     7338 2024-02-17 22:53:35.840894 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     4621 2024-02-17 22:53:35.841017 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     5607 2024-02-17 22:53:36.240240 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.py
--rw-r--r--   0        0        0     5171 2024-02-17 22:53:35.841241 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.pyi
--rw-r--r--   0        0        0     8037 2024-02-17 22:53:35.841367 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.py
--rw-r--r--   0        0        0     3606 2024-02-17 22:53:35.841477 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    19234 2024-02-17 22:53:36.240352 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.py
--rw-r--r--   0        0        0    17700 2024-02-17 22:53:35.841687 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.pyi
--rw-r--r--   0        0        0    26649 2024-02-17 22:53:35.841813 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.py
--rw-r--r--   0        0        0    16371 2024-02-17 22:53:35.842002 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     9552 2024-02-17 22:53:36.240545 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.py
--rw-r--r--   0        0        0     7723 2024-02-17 22:53:35.842226 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.pyi
--rw-r--r--   0        0        0    23014 2024-02-17 22:53:35.842330 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.py
--rw-r--r--   0        0        0    13350 2024-02-17 22:53:35.842512 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3466 2024-02-17 22:53:35.842643 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/__init__.py
--rw-r--r--   0        0        0     3630 2024-02-17 22:53:36.240688 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.py
--rw-r--r--   0        0        0     1729 2024-02-17 22:53:35.842800 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.pyi
--rw-r--r--   0        0        0     9812 2024-02-17 22:53:35.842944 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     6137 2024-02-17 22:53:35.843124 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.pyi
--rw-r--r--   0        0        0    24735 2024-02-17 22:53:36.240808 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.py
--rw-r--r--   0        0        0    22592 2024-02-17 22:53:35.843772 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.pyi
--rw-r--r--   0        0        0    40628 2024-02-17 22:53:35.843915 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.py
--rw-r--r--   0        0        0    24755 2024-02-17 22:53:35.844045 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3903 2024-02-17 22:53:36.240954 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.py
--rw-r--r--   0        0        0     2835 2024-02-17 22:53:35.844235 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.pyi
--rw-r--r--   0        0        0     6037 2024-02-17 22:53:35.844586 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.py
--rw-r--r--   0        0        0     3624 2024-02-17 22:53:35.844693 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      202 2024-02-17 22:53:35.844828 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/__init__.py
--rw-r--r--   0        0        0      273 2024-02-17 22:53:35.844970 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/__init__.py
--rw-r--r--   0        0        0     2657 2024-02-17 22:53:36.241074 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.py
--rw-r--r--   0        0        0     2008 2024-02-17 22:53:35.845143 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.pyi
--rw-r--r--   0        0        0      251 2024-02-17 22:53:35.845284 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/__init__.py
--rw-r--r--   0        0        0     1749 2024-02-17 22:53:36.241182 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.py
--rw-r--r--   0        0        0      917 2024-02-17 22:53:35.845466 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.pyi
--rw-r--r--   0        0        0      285 2024-02-17 22:53:35.845607 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/__init__.py
--rw-r--r--   0        0        0     1672 2024-02-17 22:53:36.241311 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.py
--rw-r--r--   0        0        0      672 2024-02-17 22:53:35.845773 dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.pyi
--rw-r--r--   0        0        0     5249 2024-02-17 22:53:35.846085 dazl-8.0.0b1/python/dazl/_logging.py
--rw-r--r--   0        0        0      990 2024-02-17 22:53:35.846274 dazl-8.0.0b1/python/dazl/_repr/__init__.py
--rw-r--r--   0        0        0     1722 2024-02-17 22:53:35.846434 dazl-8.0.0b1/python/dazl/cli/__init__.py
--rw-r--r--   0        0        0      602 2024-02-17 22:53:35.846572 dazl-8.0.0b1/python/dazl/cli/_base.py
--rw-r--r--   0        0        0     2102 2024-02-17 22:53:35.846711 dazl-8.0.0b1/python/dazl/cli/ls.py
--rw-r--r--   0        0        0     3273 2024-02-17 22:53:35.846854 dazl-8.0.0b1/python/dazl/cli/tail.py
--rw-r--r--   0        0        0     1233 2024-02-17 22:53:35.846993 dazl-8.0.0b1/python/dazl/cli/upload.py
--rw-r--r--   0        0        0      490 2024-02-17 22:53:35.847143 dazl-8.0.0b1/python/dazl/cli/version.py
--rw-r--r--   0        0        0     1036 2024-02-17 22:53:35.847287 dazl-8.0.0b1/python/dazl/client/__init__.py
--rw-r--r--   0        0        0     1339 2024-02-17 22:53:35.847416 dazl-8.0.0b1/python/dazl/client/_base_model.py
--rw-r--r--   0        0        0     3620 2024-02-17 22:53:35.847560 dazl-8.0.0b1/python/dazl/client/_conn_settings.py
--rw-r--r--   0        0        0     1419 2024-02-17 22:53:35.847692 dazl-8.0.0b1/python/dazl/client/_events.py
--rw-r--r--   0        0        0    24599 2024-02-17 22:53:35.847873 dazl-8.0.0b1/python/dazl/client/_network_client_impl.py
--rw-r--r--   0        0        0    33712 2024-02-17 22:53:35.848079 dazl-8.0.0b1/python/dazl/client/_party_client_impl.py
--rw-r--r--   0        0        0     4786 2024-02-17 22:53:35.848254 dazl-8.0.0b1/python/dazl/client/_reader_sync.py
--rw-r--r--   0        0        0      870 2024-02-17 22:53:35.848380 dazl-8.0.0b1/python/dazl/client/_run_level.py
--rw-r--r--   0        0        0     2150 2024-02-17 22:53:35.848512 dazl-8.0.0b1/python/dazl/client/_writer_verify.py
--rw-r--r--   0        0        0    68240 2024-02-17 22:53:35.848739 dazl-8.0.0b1/python/dazl/client/api.py
--rw-r--r--   0        0        0    19922 2024-04-03 22:04:34.042391 dazl-8.0.0b1/python/dazl/client/bots.py
--rw-r--r--   0        0        0    11197 2024-02-17 22:53:36.241744 dazl-8.0.0b1/python/dazl/client/commands.py
--rw-r--r--   0        0        0    18771 2024-02-17 22:53:35.849292 dazl-8.0.0b1/python/dazl/client/config.py
--rw-r--r--   0        0        0     1307 2024-02-17 22:53:35.849438 dazl-8.0.0b1/python/dazl/client/errors.py
--rw-r--r--   0        0        0     6863 2024-02-17 22:53:35.849586 dazl-8.0.0b1/python/dazl/client/events.py
--rw-r--r--   0        0        0     1070 2024-02-17 22:53:35.849718 dazl-8.0.0b1/python/dazl/client/ledger.py
--rw-r--r--   0        0        0      952 2024-02-17 22:53:35.849848 dazl-8.0.0b1/python/dazl/client/runner.py
--rw-r--r--   0        0        0     9113 2024-02-17 22:53:35.850034 dazl-8.0.0b1/python/dazl/client/state.py
--rw-r--r--   0        0        0     1533 2024-02-17 22:53:35.850173 dazl-8.0.0b1/python/dazl/damlast/__init__.py
--rw-r--r--   0        0        0      440 2024-02-17 22:53:35.850301 dazl-8.0.0b1/python/dazl/damlast/_base.py
--rw-r--r--   0        0        0     3251 2024-02-17 22:53:35.850563 dazl-8.0.0b1/python/dazl/damlast/_builtins_meta.py
--rw-r--r--   0        0        0     2394 2024-02-17 22:53:35.850708 dazl-8.0.0b1/python/dazl/damlast/builtins.py
--rw-r--r--   0        0        0    91575 2024-02-17 22:53:35.850968 dazl-8.0.0b1/python/dazl/damlast/daml_lf_1.py
--rw-r--r--   0        0        0     6316 2024-02-17 22:53:35.851133 dazl-8.0.0b1/python/dazl/damlast/daml_types.py
--rw-r--r--   0        0        0     1395 2024-02-17 22:53:35.851261 dazl-8.0.0b1/python/dazl/damlast/errors.py
--rw-r--r--   0        0        0    12557 2024-02-17 22:53:35.851482 dazl-8.0.0b1/python/dazl/damlast/expand.py
--rw-r--r--   0        0        0    20477 2024-02-17 22:53:35.851647 dazl-8.0.0b1/python/dazl/damlast/lookup.py
--rw-r--r--   0        0        0     2955 2024-02-17 22:53:35.851800 dazl-8.0.0b1/python/dazl/damlast/parse.py
--rw-r--r--   0        0        0    45323 2024-02-17 22:53:35.851985 dazl-8.0.0b1/python/dazl/damlast/pb_parse.py
--rw-r--r--   0        0        0     8997 2024-02-17 22:53:35.852177 dazl-8.0.0b1/python/dazl/damlast/pkgfile.py
--rw-r--r--   0        0        0     4855 2024-02-17 22:53:35.852319 dazl-8.0.0b1/python/dazl/damlast/protocols.py
--rw-r--r--   0        0        0     2938 2024-02-17 22:53:35.852452 dazl-8.0.0b1/python/dazl/damlast/types.py
--rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.852598 dazl-8.0.0b1/python/dazl/damlast/util.py
--rw-r--r--   0        0        0    14983 2024-02-17 22:53:35.852807 dazl-8.0.0b1/python/dazl/damlast/visitor.py
--rw-r--r--   0        0        0    27127 2024-02-17 22:53:35.852970 dazl-8.0.0b1/python/dazl/ledger/__init__.py
--rw-r--r--   0        0        0    11396 2024-02-17 22:53:36.241948 dazl-8.0.0b1/python/dazl/ledger/__init__.pyi
--rw-r--r--   0        0        0     2324 2024-02-17 22:53:35.853318 dazl-8.0.0b1/python/dazl/ledger/_offsets.py
--rw-r--r--   0        0        0     1652 2024-02-17 22:53:35.853444 dazl-8.0.0b1/python/dazl/ledger/_retry.py
--rw-r--r--   0        0        0     6622 2024-02-17 22:53:35.853593 dazl-8.0.0b1/python/dazl/ledger/aio/__init__.py
--rw-r--r--   0        0        0    11143 2024-02-17 22:53:36.242145 dazl-8.0.0b1/python/dazl/ledger/aio/__init__.pyi
--rw-r--r--   0        0        0     5890 2024-02-17 22:53:35.853898 dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader.py
--rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.854036 dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader_compat.py
--rw-r--r--   0        0        0    24190 2024-02-17 22:53:36.242330 dazl-8.0.0b1/python/dazl/ledger/api_types.py
--rw-r--r--   0        0        0     2117 2024-02-17 22:53:35.854345 dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.py
--rw-r--r--   0        0        0     7058 2024-02-17 22:53:36.242521 dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.pyi
--rw-r--r--   0        0        0     6846 2024-02-17 22:53:35.854636 dazl-8.0.0b1/python/dazl/ledger/blocking/_aiowrapper.py
--rw-r--r--   0        0        0     5937 2024-02-17 22:53:35.854781 dazl-8.0.0b1/python/dazl/ledger/blocking/pkgloader.py
--rw-r--r--   0        0        0    18153 2024-02-17 22:53:36.242680 dazl-8.0.0b1/python/dazl/ledger/config/__init__.py
--rw-r--r--   0        0        0    20662 2024-02-17 22:53:36.242858 dazl-8.0.0b1/python/dazl/ledger/config/access.py
--rw-r--r--   0        0        0    14197 2024-02-17 22:53:35.855738 dazl-8.0.0b1/python/dazl/ledger/config/argv.py
--rw-r--r--   0        0        0      304 2024-02-17 22:53:35.855868 dazl-8.0.0b1/python/dazl/ledger/config/exc.py
--rw-r--r--   0        0        0      343 2024-02-17 22:53:36.242964 dazl-8.0.0b1/python/dazl/ledger/config/log.py
--rw-r--r--   0        0        0     2881 2024-02-17 22:53:36.243096 dazl-8.0.0b1/python/dazl/ledger/config/ssl.py
--rw-r--r--   0        0        0    10455 2024-04-03 22:04:34.069311 dazl-8.0.0b1/python/dazl/ledger/config/url.py
--rw-r--r--   0        0        0     4761 2024-02-17 22:53:35.856335 dazl-8.0.0b1/python/dazl/ledger/errors.py
--rw-r--r--   0        0        0      475 2024-02-17 22:53:35.856470 dazl-8.0.0b1/python/dazl/ledger/grpc/__init__.py
--rw-r--r--   0        0        0     1188 2024-02-17 22:53:36.243409 dazl-8.0.0b1/python/dazl/ledger/grpc/__init__.pyi
--rw-r--r--   0        0        0     6459 2024-02-17 22:53:35.856863 dazl-8.0.0b1/python/dazl/ledger/grpc/channel.py
--rw-r--r--   0        0        0    18849 2024-02-17 22:53:35.857023 dazl-8.0.0b1/python/dazl/ledger/grpc/codec_aio.py
--rw-r--r--   0        0        0    47346 2024-02-17 22:53:36.243593 dazl-8.0.0b1/python/dazl/ledger/grpc/conn_aio.py
--rw-r--r--   0        0        0      313 2024-02-17 22:53:35.857372 dazl-8.0.0b1/python/dazl/ledger/pkgcache.py
--rw-r--r--   0        0        0      290 2024-02-17 22:53:35.857502 dazl-8.0.0b1/python/dazl/ledgerutil/__init__.py
--rw-r--r--   0        0        0    17303 2024-02-17 22:53:35.857651 dazl-8.0.0b1/python/dazl/ledgerutil/acs.py
--rw-r--r--   0        0        0     1883 2024-02-17 22:53:35.857792 dazl-8.0.0b1/python/dazl/ledgerutil/fetch.py
--rw-r--r--   0        0        0      208 2024-02-17 22:53:35.857969 dazl-8.0.0b1/python/dazl/metrics/__init__.py
--rw-r--r--   0        0        0      991 2024-02-17 22:53:35.858113 dazl-8.0.0b1/python/dazl/metrics/api.py
--rw-r--r--   0        0        0     1614 2024-02-17 22:53:35.858277 dazl-8.0.0b1/python/dazl/metrics/instrumenters.py
--rw-r--r--   0        0        0     1592 2024-02-17 22:53:35.858537 dazl-8.0.0b1/python/dazl/metrics/prometheus.py
--rw-r--r--   0        0        0      829 2024-02-17 22:53:35.858713 dazl-8.0.0b1/python/dazl/pretty/__init__.py
--rw-r--r--   0        0        0      877 2024-02-17 22:53:35.858915 dazl-8.0.0b1/python/dazl/pretty/pygments_daml_lexer.py
--rw-r--r--   0        0        0      252 2024-02-17 22:53:35.859109 dazl-8.0.0b1/python/dazl/pretty/table/__init__.py
--rw-r--r--   0        0        0      733 2024-02-17 22:53:35.859269 dazl-8.0.0b1/python/dazl/pretty/table/fmt_base.py
--rw-r--r--   0        0        0     1663 2024-02-17 22:53:35.859475 dazl-8.0.0b1/python/dazl/pretty/table/fmt_json.py
--rw-r--r--   0        0        0     5392 2024-02-17 22:53:35.859789 dazl-8.0.0b1/python/dazl/pretty/table/fmt_pretty.py
--rw-r--r--   0        0        0     3162 2024-02-17 22:53:35.860082 dazl-8.0.0b1/python/dazl/pretty/table/model.py
--rw-r--r--   0        0        0     1553 2024-02-17 22:53:35.860329 dazl-8.0.0b1/python/dazl/pretty/table/write.py
--rw-r--r--   0        0        0     3318 2024-02-17 22:53:35.860492 dazl-8.0.0b1/python/dazl/pretty/util.py
--rw-r--r--   0        0        0     1733 2024-02-17 22:53:36.243742 dazl-8.0.0b1/python/dazl/prim/__init__.py
--rw-r--r--   0        0        0     1635 2024-02-17 22:53:35.860901 dazl-8.0.0b1/python/dazl/prim/basic.py
--rw-r--r--   0        0        0     1645 2024-02-17 22:53:35.861044 dazl-8.0.0b1/python/dazl/prim/complex.py
--rw-r--r--   0        0        0     2421 2024-02-17 22:53:35.861220 dazl-8.0.0b1/python/dazl/prim/contracts.py
--rw-r--r--   0        0        0     7009 2024-02-17 22:53:35.861382 dazl-8.0.0b1/python/dazl/prim/datetime.py
--rw-r--r--   0        0        0     1155 2024-02-17 22:53:35.861521 dazl-8.0.0b1/python/dazl/prim/errors.py
--rw-r--r--   0        0        0     1521 2024-02-17 22:53:35.861669 dazl-8.0.0b1/python/dazl/prim/json.py
--rw-r--r--   0        0        0     1398 2024-02-17 22:53:35.861826 dazl-8.0.0b1/python/dazl/prim/map.py
--rw-r--r--   0        0        0     1476 2024-02-17 22:53:35.861995 dazl-8.0.0b1/python/dazl/prim/numbers.py
--rw-r--r--   0        0        0     1144 2024-04-03 22:04:34.052818 dazl-8.0.0b1/python/dazl/prim/party.py
--rw-r--r--   0        0        0      405 2024-02-17 22:53:35.862535 dazl-8.0.0b1/python/dazl/protocols/__init__.py
--rw-r--r--   0        0        0     6120 2024-02-17 22:53:35.862723 dazl-8.0.0b1/python/dazl/protocols/_base.py
--rw-r--r--   0        0        0     9246 2024-02-17 22:53:35.863100 dazl-8.0.0b1/python/dazl/protocols/autodetect.py
--rw-r--r--   0        0        0     2927 2024-02-17 22:53:35.863392 dazl-8.0.0b1/python/dazl/protocols/core.py
--rw-r--r--   0        0        0      891 2024-02-17 22:53:36.243999 dazl-8.0.0b1/python/dazl/protocols/errors.py
--rw-r--r--   0        0        0     6889 2024-02-17 22:53:35.863784 dazl-8.0.0b1/python/dazl/protocols/events.py
--rw-r--r--   0        0        0     2337 2024-02-17 22:53:35.864028 dazl-8.0.0b1/python/dazl/protocols/oauth.py
--rw-r--r--   0        0        0     4619 2024-02-17 22:53:35.864252 dazl-8.0.0b1/python/dazl/protocols/serializers.py
--rw-r--r--   0        0        0      141 2024-02-17 22:53:35.864476 dazl-8.0.0b1/python/dazl/protocols/v1/__init__.py
--rw-r--r--   0        0        0    17052 2024-02-17 22:53:35.864680 dazl-8.0.0b1/python/dazl/protocols/v1/grpc.py
--rw-r--r--   0        0        0    16229 2024-02-17 22:53:35.864920 dazl-8.0.0b1/python/dazl/protocols/v1/pb_parse_event.py
--rw-r--r--   0        0        0     4799 2024-02-17 22:53:35.865063 dazl-8.0.0b1/python/dazl/protocols/v1/pb_ser_command.py
--rw-r--r--   0        0        0      194 2024-02-17 22:53:35.865241 dazl-8.0.0b1/python/dazl/py.typed
--rw-r--r--   0        0        0     4796 2024-02-17 22:53:35.865561 dazl-8.0.0b1/python/dazl/query/__init__.py
--rw-r--r--   0        0        0      270 2024-02-17 22:53:35.865783 dazl-8.0.0b1/python/dazl/scheduler/__init__.py
--rw-r--r--   0        0        0     1318 2024-02-17 22:53:35.865997 dazl-8.0.0b1/python/dazl/scheduler/_base.py
--rw-r--r--   0        0        0     5076 2024-02-17 22:53:35.866174 dazl-8.0.0b1/python/dazl/scheduler/_invoker.py
--rw-r--r--   0        0        0     2062 2024-02-17 22:53:35.866302 dazl-8.0.0b1/python/dazl/scheduler/_invoker.pyi
--rw-r--r--   0        0        0      575 2024-02-17 22:53:35.866428 dazl-8.0.0b1/python/dazl/server/__init__.py
--rw-r--r--   0        0        0     3256 2024-02-17 22:53:35.866567 dazl-8.0.0b1/python/dazl/server/management.py
--rw-r--r--   0        0        0     1766 2024-02-17 22:53:35.866693 dazl-8.0.0b1/python/dazl/server/metrics.py
--rw-r--r--   0        0        0      355 2024-02-17 22:53:35.866819 dazl-8.0.0b1/python/dazl/testing/__init__.py
--rw-r--r--   0        0        0     2296 2024-02-17 22:53:35.866945 dazl-8.0.0b1/python/dazl/testing/_cert.py
--rw-r--r--   0        0        0    12650 2024-02-17 22:53:35.867157 dazl-8.0.0b1/python/dazl/testing/_sandbox.py
--rw-r--r--   0        0        0     7137 2024-02-17 22:53:36.244158 dazl-8.0.0b1/python/dazl/testing/connect.py
--rw-r--r--   0        0        0     3403 2024-02-17 22:53:36.244285 dazl-8.0.0b1/python/dazl/testing/connect.pyi
--rw-r--r--   0        0        0      488 2024-02-17 22:53:35.867581 dazl-8.0.0b1/python/dazl/util/__init__.py
--rw-r--r--   0        0        0    19677 2024-02-17 22:53:36.244448 dazl-8.0.0b1/python/dazl/util/asyncio_util.py
--rw-r--r--   0        0        0     4795 2024-04-03 22:04:34.110861 dazl-8.0.0b1/python/dazl/util/config_meta.py
--rw-r--r--   0        0        0      964 2024-02-17 22:53:35.868034 dazl-8.0.0b1/python/dazl/util/enum.py
--rw-r--r--   0        0        0     2657 2024-04-03 22:04:34.095373 dazl-8.0.0b1/python/dazl/util/io.py
--rw-r--r--   0        0        0      521 2024-02-17 22:53:36.244591 dazl-8.0.0b1/python/dazl/util/prim_natural.py
--rw-r--r--   0        0        0     3515 2024-02-17 22:53:36.244719 dazl-8.0.0b1/python/dazl/util/proc_util.py
--rw-r--r--   0        0        0     1391 2024-02-17 22:53:36.244841 dazl-8.0.0b1/python/dazl/util/termcap.py
--rw-r--r--   0        0        0     2347 2024-02-17 22:53:35.868846 dazl-8.0.0b1/python/dazl/util/tools.py
--rw-r--r--   0        0        0      890 2024-02-17 22:53:35.868988 dazl-8.0.0b1/python/dazl/util/typing.py
--rw-r--r--   0        0        0      612 2024-02-17 22:53:35.869136 dazl-8.0.0b1/python/dazl/values/__init__.py
--rw-r--r--   0        0        0     6068 2024-02-17 22:53:35.869300 dazl-8.0.0b1/python/dazl/values/canonical.py
--rw-r--r--   0        0        0    15792 2024-02-17 22:53:35.869533 dazl-8.0.0b1/python/dazl/values/context.py
--rw-r--r--   0        0        0     1881 2024-02-17 22:53:35.869663 dazl-8.0.0b1/python/dazl/values/json.py
--rw-r--r--   0        0        0     3359 2024-02-17 22:53:35.869788 dazl-8.0.0b1/python/dazl/values/mapper.py
--rw-r--r--   0        0        0     9955 2024-02-17 22:53:35.869972 dazl-8.0.0b1/python/dazl/values/protobuf.py
--rw-r--r--   0        0        0     2755 2024-02-17 22:53:35.870119 dazl-8.0.0b1/python/dazl/values/pysample_encoder.py
--rw-r--r--   0        0        0     5018 2024-02-17 22:53:35.870284 dazl-8.0.0b1/python/dazl/values/string.py
--rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 dazl-8.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11393 2024-02-17 22:53:35.749987 dazl-8.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2725 2024-02-17 22:53:35.750514 dazl-8.0.0b2/README.md
+-rw-r--r--   0        0        0     2673 2024-04-05 00:21:15.427502 dazl-8.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      333 2024-02-17 22:53:36.227347 dazl-8.0.0b2/python/_dazl/__init__.py
+-rw-r--r--   0        0        0      887 2024-02-17 22:53:36.227408 dazl-8.0.0b2/python/_dazl/__main__.py
+-rw-r--r--   0        0        0     1476 2024-02-17 22:53:36.227467 dazl-8.0.0b2/python/_dazl/_logging.py
+-rw-r--r--   0        0        0      276 2024-02-17 22:53:36.227535 dazl-8.0.0b2/python/_dazl/codegen/__init__.py
+-rw-r--r--   0        0        0     5483 2024-02-17 22:53:36.227613 dazl-8.0.0b2/python/_dazl/codegen/go.py
+-rw-r--r--   0        0        0      347 2024-02-17 22:53:36.227677 dazl-8.0.0b2/python/_dazl/codegen/go_header.py
+-rw-r--r--   0        0        0     1728 2024-02-17 22:53:36.227737 dazl-8.0.0b2/python/_dazl/codegen/python.py
+-rw-r--r--   0        0        0     5092 2024-02-17 22:53:36.227814 dazl-8.0.0b2/python/_dazl/codegen/python_grpc_pyi.py
+-rw-r--r--   0        0        0      339 2024-02-17 22:53:36.227873 dazl-8.0.0b2/python/_dazl/codegen/python_header.py
+-rw-r--r--   0        0        0     2442 2024-02-17 22:53:36.227934 dazl-8.0.0b2/python/_dazl/codegen/python_init.py
+-rw-r--r--   0        0        0      520 2024-02-17 22:53:36.227993 dazl-8.0.0b2/python/_dazl/codegen/util.py
+-rw-r--r--   0        0        0      944 2024-04-03 23:31:58.881356 dazl-8.0.0b2/python/_dazl/collections.py
+-rw-r--r--   0        0        0     4095 2024-02-17 22:53:36.228120 dazl-8.0.0b2/python/_dazl/download/__init__.py
+-rw-r--r--   0        0        0     3147 2024-02-17 22:53:36.228186 dazl-8.0.0b2/python/_dazl/protoc/__init__.py
+-rw-r--r--   0        0        0     2027 2024-04-03 23:31:58.881691 dazl-8.0.0b2/python/_dazl/protopack/__init__.py
+-rw-r--r--   0        0        0     4306 2024-02-17 22:53:36.228348 dazl-8.0.0b2/python/_dazl/protopack/rename.py
+-rw-r--r--   0        0        0     3180 2024-02-17 22:53:36.228419 dazl-8.0.0b2/python/_dazl/protopack/rewrite.py
+-rw-r--r--   0        0        0      221 2024-02-17 22:53:36.228490 dazl-8.0.0b2/python/_dazl/syntax/__init__.py
+-rw-r--r--   0        0        0      601 2024-02-17 22:53:36.228554 dazl-8.0.0b2/python/_dazl/syntax/python/__init__.py
+-rw-r--r--   0        0        0      586 2024-02-17 22:53:36.228610 dazl-8.0.0b2/python/_dazl/syntax/python/_basic.py
+-rw-r--r--   0        0        0     6389 2024-02-17 22:53:36.228696 dazl-8.0.0b2/python/_dazl/syntax/python/imports.py
+-rw-r--r--   0        0        0     2683 2024-02-17 22:53:36.228762 dazl-8.0.0b2/python/_dazl/syntax/python/pb.py
+-rw-r--r--   0        0        0     7328 2024-02-17 22:53:36.228847 dazl-8.0.0b2/python/_dazl/syntax/python/symbols.py
+-rw-r--r--   0        0        0     2793 2024-02-17 22:53:36.228907 dazl-8.0.0b2/python/_dazl/syntax/python/types.py
+-rw-r--r--   0        0        0     2188 2024-02-17 22:53:36.229013 dazl-8.0.0b2/python/_dazl/update.py
+-rw-r--r--   0        0        0     1737 2024-04-05 00:21:15.427830 dazl-8.0.0b2/python/dazl/__init__.py
+-rw-r--r--   0        0        0      311 2024-02-17 22:53:35.796859 dazl-8.0.0b2/python/dazl/__main__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797029 dazl-8.0.0b2/python/dazl/_gen/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797159 dazl-8.0.0b2/python/dazl/_gen/com/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.797280 dazl-8.0.0b2/python/dazl/_gen/com/daml/__init__.py
+-rw-r--r--   0        0        0     1525 2024-02-17 22:53:36.229174 dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py
+-rw-r--r--   0        0        0    52179 2024-02-17 22:53:35.797603 dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py
+-rw-r--r--   0        0        0    78370 2024-02-17 22:53:35.797866 dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi
+-rw-r--r--   0        0        0     2298 2024-02-17 22:53:35.798460 dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py
+-rw-r--r--   0        0        0     1486 2024-02-17 22:53:35.798607 dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798740 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.798859 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/__init__.py
+-rw-r--r--   0        0        0     6188 2024-02-17 22:53:36.229442 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py
+-rw-r--r--   0        0        0     2961 2024-02-17 22:53:35.799137 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
+-rw-r--r--   0        0        0     1801 2024-02-17 22:53:35.799270 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi
+-rw-r--r--   0        0        0     4390 2024-02-17 22:53:35.799437 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2396 2024-02-17 22:53:35.799592 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4542 2024-02-17 22:53:36.229586 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
+-rw-r--r--   0        0        0     3967 2024-02-17 22:53:35.799910 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
+-rw-r--r--   0        0        0     2714 2024-02-17 22:53:35.800064 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi
+-rw-r--r--   0        0        0     6347 2024-02-17 22:53:35.800242 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3579 2024-02-17 22:53:35.800388 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6304 2024-02-17 22:53:35.800524 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py
+-rw-r--r--   0        0        0     4309 2024-02-17 22:53:35.800651 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi
+-rw-r--r--   0        0        0    17920 2024-02-17 22:53:35.800772 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8410 2024-02-17 22:53:35.800952 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3043 2024-02-17 22:53:35.801100 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py
+-rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.801369 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi
+-rw-r--r--   0        0        0     3683 2024-02-17 22:53:35.801517 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.801662 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2218 2024-02-17 22:53:35.801796 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py
+-rw-r--r--   0        0        0     1145 2024-02-17 22:53:35.801924 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi
+-rw-r--r--   0        0        0     3426 2024-02-17 22:53:35.802064 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
+-rw-r--r--   0        0        0     2113 2024-02-17 22:53:35.802196 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi
+-rw-r--r--   0        0        0     6681 2024-02-17 22:53:35.802377 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3660 2024-02-17 22:53:35.802530 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2325 2024-02-17 22:53:35.802674 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
+-rw-r--r--   0        0        0      995 2024-02-17 22:53:35.802815 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi
+-rw-r--r--   0        0        0     4791 2024-02-17 22:53:35.802976 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2225 2024-02-17 22:53:35.803122 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6691 2024-02-17 22:53:35.803305 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
+-rw-r--r--   0        0        0     5361 2024-02-17 22:53:35.803473 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi
+-rw-r--r--   0        0        0    19490 2024-02-17 22:53:35.803626 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9064 2024-02-17 22:53:35.803836 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9901 2024-02-17 22:53:35.804032 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py
+-rw-r--r--   0        0        0     8928 2024-02-17 22:53:35.804213 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25223 2024-02-17 22:53:35.804374 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12691 2024-02-17 22:53:35.804590 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3879 2024-02-17 22:53:35.804732 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
+-rw-r--r--   0        0        0     2724 2024-02-17 22:53:35.804879 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi
+-rw-r--r--   0        0        0     7734 2024-02-17 22:53:35.805059 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3690 2024-02-17 22:53:35.805215 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3899 2024-02-17 22:53:35.805363 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
+-rw-r--r--   0        0        0     2096 2024-02-17 22:53:35.805498 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi
+-rw-r--r--   0        0        0    10939 2024-02-17 22:53:35.805669 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6396 2024-02-17 22:53:35.805827 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2250 2024-02-17 22:53:35.805984 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
+-rw-r--r--   0        0        0      764 2024-02-17 22:53:35.806133 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi
+-rw-r--r--   0        0        0     5656 2024-02-17 22:53:35.806304 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2220 2024-02-17 22:53:35.806432 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6717 2024-02-17 22:53:35.806618 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
+-rw-r--r--   0        0        0     7479 2024-02-17 22:53:35.806802 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi
+-rw-r--r--   0        0        0     2481 2024-02-17 22:53:35.806959 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
+-rw-r--r--   0        0        0     1851 2024-02-17 22:53:35.807108 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi
+-rw-r--r--   0        0        0     2007 2024-02-17 22:53:35.807250 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py
+-rw-r--r--   0        0        0     1023 2024-02-17 22:53:35.807378 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi
+-rw-r--r--   0        0        0     5333 2024-02-17 22:53:35.807559 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
+-rw-r--r--   0        0        0     6277 2024-02-17 22:53:35.807737 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi
+-rw-r--r--   0        0        0     3878 2024-02-17 22:53:35.807846 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py
+-rw-r--r--   0        0        0     2869 2024-02-17 22:53:35.807954 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi
+-rw-r--r--   0        0        0     5706 2024-02-17 22:53:35.808080 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3753 2024-02-17 22:53:35.808181 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7614 2024-02-17 22:53:35.808362 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py
+-rw-r--r--   0        0        0     7919 2024-02-17 22:53:35.808535 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi
+-rw-r--r--   0        0        0     2840 2024-02-17 22:53:35.808687 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
+-rw-r--r--   0        0        0     1333 2024-02-17 22:53:35.808832 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi
+-rw-r--r--   0        0        0     3789 2024-02-17 22:53:35.808969 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2480 2024-02-17 22:53:35.809097 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2941 2024-02-17 22:53:35.809229 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
+-rw-r--r--   0        0        0      712 2024-02-17 22:53:35.809371 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi
+-rw-r--r--   0        0        0     4024 2024-02-17 22:53:35.809532 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2333 2024-02-17 22:53:35.809685 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2039 2024-02-17 22:53:35.809821 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
+-rw-r--r--   0        0        0     1158 2024-02-17 22:53:35.809960 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi
+-rw-r--r--   0        0        0     3815 2024-02-17 22:53:35.810109 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
+-rw-r--r--   0        0        0     2815 2024-02-17 22:53:35.810258 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi
+-rw-r--r--   0        0        0     6970 2024-02-17 22:53:35.810436 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4809 2024-02-17 22:53:35.810602 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      406 2024-02-17 22:53:35.810747 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
+-rw-r--r--   0        0        0     2913 2024-02-17 22:53:35.810888 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
+-rw-r--r--   0        0        0     1550 2024-02-17 22:53:35.811025 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi
+-rw-r--r--   0        0        0     5129 2024-02-17 22:53:35.811190 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3379 2024-02-17 22:53:35.811324 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3327 2024-02-17 22:53:35.811469 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
+-rw-r--r--   0        0        0     2554 2024-02-17 22:53:35.811605 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi
+-rw-r--r--   0        0        0     3685 2024-02-17 22:53:35.811740 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
+-rw-r--r--   0        0        0     3347 2024-02-17 22:53:35.811873 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi
+-rw-r--r--   0        0        0     6625 2024-02-17 22:53:35.812036 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
+-rw-r--r--   0        0        0     5153 2024-02-17 22:53:35.812194 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi
+-rw-r--r--   0        0        0    18252 2024-02-17 22:53:35.812341 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11776 2024-02-17 22:53:35.812536 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5817 2024-02-17 22:53:35.812698 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
+-rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.812851 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi
+-rw-r--r--   0        0        0     3221 2024-02-17 22:53:35.812983 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
+-rw-r--r--   0        0        0     2064 2024-02-17 22:53:35.813118 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi
+-rw-r--r--   0        0        0     3207 2024-02-17 22:53:35.813255 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2293 2024-02-17 22:53:35.813390 dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813522 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813647 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.813766 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.814533 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/__init__.py
+-rw-r--r--   0        0        0     1940 2024-02-17 22:53:35.814700 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/__init__.py
+-rw-r--r--   0        0        0    11447 2024-02-17 22:53:36.229775 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.py
+-rw-r--r--   0        0        0     9455 2024-02-17 22:53:35.814982 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.pyi
+-rw-r--r--   0        0        0    29764 2024-02-17 22:53:35.815101 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16810 2024-02-17 22:53:35.815230 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1030 2024-02-17 22:53:35.815381 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/__init__.py
+-rw-r--r--   0        0        0     8612 2024-02-17 22:53:36.229948 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.py
+-rw-r--r--   0        0        0     9794 2024-02-17 22:53:35.815639 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815757 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.815874 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/__init__.py
+-rw-r--r--   0        0        0     3128 2024-02-17 22:53:36.230077 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-17 22:53:36.230195 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1153 2024-02-17 22:53:35.816155 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3526 2024-02-17 22:53:35.816255 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2257 2024-02-17 22:53:35.816350 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4279 2024-02-17 22:53:36.230361 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.py
+-rw-r--r--   0        0        0     2594 2024-02-17 22:53:35.816602 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.pyi
+-rw-r--r--   0        0        0     7501 2024-02-17 22:53:35.816727 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4941 2024-02-17 22:53:35.816854 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3638 2024-02-17 22:53:36.230477 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.py
+-rw-r--r--   0        0        0      858 2024-02-17 22:53:35.817036 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.pyi
+-rw-r--r--   0        0        0    18541 2024-02-17 22:53:35.817152 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11361 2024-02-17 22:53:35.817304 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7888 2024-02-17 22:53:36.230593 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.py
+-rw-r--r--   0        0        0     4680 2024-02-17 22:53:35.817518 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.pyi
+-rw-r--r--   0        0        0    25680 2024-02-17 22:53:35.817632 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0    15191 2024-02-17 22:53:35.817820 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.230708 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.py
+-rw-r--r--   0        0        0     1904 2024-02-17 22:53:35.817978 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.pyi
+-rw-r--r--   0        0        0     5932 2024-02-17 22:53:35.818106 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3678 2024-02-17 22:53:35.818203 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4424 2024-02-17 22:53:36.230855 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2976 2024-02-17 22:53:35.818423 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.818519 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.818618 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3800 2024-02-17 22:53:36.230977 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.py
+-rw-r--r--   0        0        0     2706 2024-02-17 22:53:35.818787 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.pyi
+-rw-r--r--   0        0        0     5644 2024-02-17 22:53:35.818916 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3720 2024-02-17 22:53:35.819018 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4972 2024-02-17 22:53:36.231102 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2651 2024-02-17 22:53:35.819215 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0    11631 2024-02-17 22:53:35.819360 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6738 2024-02-17 22:53:36.231234 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.231353 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.py
+-rw-r--r--   0        0        0     2174 2024-02-17 22:53:35.819629 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.pyi
+-rw-r--r--   0        0        0     1916 2024-02-17 22:53:36.231467 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.py
+-rw-r--r--   0        0        0      368 2024-02-17 22:53:35.819790 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.pyi
+-rw-r--r--   0        0        0     3577 2024-02-17 22:53:35.819894 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2236 2024-02-17 22:53:35.819992 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      362 2024-02-17 22:53:35.820123 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/__init__.py
+-rw-r--r--   0        0        0     2632 2024-02-17 22:53:36.231585 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1523 2024-02-17 22:53:35.820286 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     5711 2024-02-17 22:53:36.231714 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.py
+-rw-r--r--   0        0        0     5898 2024-02-17 22:53:35.820506 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.pyi
+-rw-r--r--   0        0        0      825 2024-02-17 22:53:35.820637 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/__init__.py
+-rw-r--r--   0        0        0     2930 2024-02-17 22:53:36.231843 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.py
+-rw-r--r--   0        0        0     1682 2024-02-17 22:53:35.820805 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     3811 2024-02-17 22:53:35.820905 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2393 2024-02-17 22:53:35.820999 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3392 2024-02-17 22:53:36.231947 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.py
+-rw-r--r--   0        0        0     2186 2024-02-17 22:53:35.821159 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     4358 2024-02-17 22:53:35.821284 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-02-17 22:53:35.821382 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.821508 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/__init__.py
+-rw-r--r--   0        0        0     2030 2024-02-17 22:53:36.232068 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/__init__.py
+-rw-r--r--   0        0        0     2000 2024-02-17 22:53:36.232185 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.py
+-rw-r--r--   0        0        0      368 2024-02-17 22:53:35.821776 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.pyi
+-rw-r--r--   0        0        0     3366 2024-02-17 22:53:35.821875 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2287 2024-02-17 22:53:35.822115 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3159 2024-02-17 22:53:36.232290 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.py
+-rw-r--r--   0        0        0     1796 2024-02-17 22:53:35.822288 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.pyi
+-rw-r--r--   0        0        0     5273 2024-02-17 22:53:35.822416 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3430 2024-02-17 22:53:35.822515 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4927 2024-02-17 22:53:36.232409 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.py
+-rw-r--r--   0        0        0     4070 2024-02-17 22:53:35.822715 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     5949 2024-02-17 22:53:35.822844 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3581 2024-02-17 22:53:35.822946 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5863 2024-02-17 22:53:36.232533 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.py
+-rw-r--r--   0        0        0     3374 2024-02-17 22:53:35.823157 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.pyi
+-rw-r--r--   0        0        0    12411 2024-02-17 22:53:35.823336 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7875 2024-02-17 22:53:35.823465 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2409 2024-02-17 22:53:36.232649 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.py
+-rw-r--r--   0        0        0     1790 2024-02-17 22:53:35.823639 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.pyi
+-rw-r--r--   0        0        0     8931 2024-02-17 22:53:36.232813 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.py
+-rw-r--r--   0        0        0     6904 2024-02-17 22:53:35.823888 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.pyi
+-rw-r--r--   0        0        0    31573 2024-02-17 22:53:35.824004 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16744 2024-02-17 22:53:35.824127 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2024-02-17 22:53:36.232930 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.py
+-rw-r--r--   0        0        0      892 2024-02-17 22:53:35.824306 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.pyi
+-rw-r--r--   0        0        0      274 2024-02-17 22:53:35.824436 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/__init__.py
+-rw-r--r--   0        0        0     1978 2024-02-17 22:53:36.233033 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.py
+-rw-r--r--   0        0        0     1150 2024-02-17 22:53:35.824596 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824718 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.824840 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/__init__.py
+-rw-r--r--   0        0        0      700 2024-02-17 22:53:35.824967 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/__init__.py
+-rw-r--r--   0        0        0     7382 2024-02-17 22:53:36.233166 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.py
+-rw-r--r--   0        0        0     7065 2024-02-17 22:53:35.825187 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.pyi
+-rw-r--r--   0        0        0     5164 2024-02-17 22:53:35.825306 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.825398 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825518 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.825643 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/__init__.py
+-rw-r--r--   0        0        0     5756 2024-02-17 22:53:35.825809 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/__init__.py
+-rw-r--r--   0        0        0    10342 2024-02-17 22:53:36.233353 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.py
+-rw-r--r--   0        0        0     7925 2024-02-17 22:53:35.826054 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.pyi
+-rw-r--r--   0        0        0    23356 2024-02-17 22:53:35.826172 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.py
+-rw-r--r--   0        0        0    14253 2024-02-17 22:53:35.826358 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2258 2024-02-17 22:53:36.233483 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.py
+-rw-r--r--   0        0        0      695 2024-02-17 22:53:35.826533 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.pyi
+-rw-r--r--   0        0        0     3721 2024-02-17 22:53:35.826633 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2024-02-17 22:53:35.826853 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5241 2024-02-17 22:53:36.233620 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.py
+-rw-r--r--   0        0        0     3208 2024-02-17 22:53:35.827057 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.pyi
+-rw-r--r--   0        0        0    11122 2024-02-17 22:53:35.827192 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6364 2024-02-17 22:53:35.827314 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11596 2024-02-17 22:53:36.233789 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.py
+-rw-r--r--   0        0        0     9525 2024-02-17 22:53:35.827546 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.pyi
+-rw-r--r--   0        0        0    33250 2024-02-17 22:53:35.827669 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.py
+-rw-r--r--   0        0        0    21002 2024-02-17 22:53:35.827795 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5534 2024-02-17 22:53:36.233920 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.py
+-rw-r--r--   0        0        0     4072 2024-02-17 22:53:35.828006 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.pyi
+-rw-r--r--   0        0        0     9898 2024-02-17 22:53:35.828138 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6176 2024-02-17 22:53:35.828263 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2249 2024-02-17 22:53:36.234035 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.py
+-rw-r--r--   0        0        0      832 2024-02-17 22:53:35.828433 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.pyi
+-rw-r--r--   0        0        0     4589 2024-02-17 22:53:35.828559 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.py
+-rw-r--r--   0        0        0     2395 2024-02-17 22:53:35.828662 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2960 2024-02-17 22:53:36.234150 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.py
+-rw-r--r--   0        0        0     2330 2024-02-17 22:53:35.828823 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.pyi
+-rw-r--r--   0        0        0     3234 2024-02-17 22:53:35.828919 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2091 2024-02-17 22:53:35.829017 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4466 2024-02-17 22:53:36.234278 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.py
+-rw-r--r--   0        0        0     1906 2024-02-17 22:53:35.829213 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.pyi
+-rw-r--r--   0        0        0    19105 2024-02-17 22:53:35.829321 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11105 2024-02-17 22:53:35.829485 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2309 2024-02-17 22:53:36.234404 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.py
+-rw-r--r--   0        0        0      911 2024-02-17 22:53:35.829672 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.pyi
+-rw-r--r--   0        0        0     5364 2024-02-17 22:53:35.829803 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3469 2024-02-17 22:53:35.829908 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2507 2024-02-17 22:53:36.234517 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.py
+-rw-r--r--   0        0        0     1047 2024-02-17 22:53:35.830088 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.pyi
+-rw-r--r--   0        0        0     3634 2024-02-17 22:53:35.830192 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2357 2024-02-17 22:53:35.830293 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5697 2024-02-17 22:53:36.234643 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.py
+-rw-r--r--   0        0        0     5622 2024-02-17 22:53:35.830510 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.pyi
+-rw-r--r--   0        0        0     7628 2024-02-17 22:53:35.830634 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4909 2024-02-17 22:53:35.830760 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.830879 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/__init__.py
+-rw-r--r--   0        0        0     1227 2024-02-17 22:53:35.831005 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/__init__.py
+-rw-r--r--   0        0        0    16269 2024-02-17 22:53:36.234874 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.py
+-rw-r--r--   0        0        0    21287 2024-02-17 22:53:35.831279 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.pyi
+-rw-r--r--   0        0        0     3318 2024-02-17 22:53:36.234997 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.py
+-rw-r--r--   0        0        0     2205 2024-02-17 22:53:35.831462 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.831586 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/__init__.py
+-rw-r--r--   0        0        0     4582 2024-02-17 22:53:36.235225 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/__init__.py
+-rw-r--r--   0        0        0     2069 2024-02-17 22:53:36.235360 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.py
+-rw-r--r--   0        0        0     1456 2024-02-17 22:53:35.831874 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.pyi
+-rw-r--r--   0        0        0     4351 2024-02-17 22:53:36.235489 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.py
+-rw-r--r--   0        0        0     4153 2024-02-17 22:53:35.832097 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.pyi
+-rw-r--r--   0        0        0     3340 2024-02-17 22:53:36.235615 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.py
+-rw-r--r--   0        0        0     3275 2024-02-17 22:53:35.832262 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.pyi
+-rw-r--r--   0        0        0     5709 2024-02-17 22:53:36.235748 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.py
+-rw-r--r--   0        0        0     5991 2024-02-17 22:53:35.832480 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.pyi
+-rw-r--r--   0        0        0     3817 2024-02-17 22:53:36.235861 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.py
+-rw-r--r--   0        0        0     4555 2024-02-17 22:53:35.832670 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.235972 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.py
+-rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.832840 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.pyi
+-rw-r--r--   0        0        0    12436 2024-02-17 22:53:36.236180 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.py
+-rw-r--r--   0        0        0    15054 2024-02-17 22:53:35.833159 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     5560 2024-02-17 22:53:36.236308 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     5503 2024-02-17 22:53:35.833382 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     9990 2024-02-17 22:53:36.236477 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.py
+-rw-r--r--   0        0        0    12765 2024-02-17 22:53:35.833666 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.pyi
+-rw-r--r--   0        0        0     1523 2024-02-17 22:53:36.236586 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.py
+-rw-r--r--   0        0        0      709 2024-02-17 22:53:35.833833 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.pyi
+-rw-r--r--   0        0        0     5302 2024-02-17 22:53:36.236709 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.py
+-rw-r--r--   0        0        0     5427 2024-02-17 22:53:35.834062 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.pyi
+-rw-r--r--   0        0        0     2214 2024-02-17 22:53:36.236819 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.py
+-rw-r--r--   0        0        0     1634 2024-02-17 22:53:35.834226 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.pyi
+-rw-r--r--   0        0        0    11115 2024-02-17 22:53:36.236972 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.py
+-rw-r--r--   0        0        0    13925 2024-02-17 22:53:35.834499 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.pyi
+-rw-r--r--   0        0        0     2787 2024-02-17 22:53:35.834625 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/__init__.py
+-rw-r--r--   0        0        0     2404 2024-02-17 22:53:36.237090 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.py
+-rw-r--r--   0        0        0     1515 2024-02-17 22:53:35.834780 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.pyi
+-rw-r--r--   0        0        0     4869 2024-02-17 22:53:36.237227 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.py
+-rw-r--r--   0        0        0     4409 2024-02-17 22:53:35.834991 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.pyi
+-rw-r--r--   0        0        0     3035 2024-02-17 22:53:36.237347 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.py
+-rw-r--r--   0        0        0     2788 2024-02-17 22:53:35.835144 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     2945 2024-02-17 22:53:36.237462 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.py
+-rw-r--r--   0        0        0     2263 2024-02-17 22:53:35.835281 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.pyi
+-rw-r--r--   0        0        0     9401 2024-02-17 22:53:36.237635 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.py
+-rw-r--r--   0        0        0    10568 2024-02-17 22:53:35.835548 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     5513 2024-02-17 22:53:36.237766 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     5720 2024-02-17 22:53:35.835760 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     7000 2024-02-17 22:53:36.238013 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.py
+-rw-r--r--   0        0        0     8939 2024-02-17 22:53:35.835987 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.pyi
+-rw-r--r--   0        0        0     5100 2024-02-17 22:53:36.238150 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.py
+-rw-r--r--   0        0        0     4441 2024-02-17 22:53:35.836194 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.pyi
+-rw-r--r--   0        0        0     6336 2024-02-17 22:53:36.238289 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.py
+-rw-r--r--   0        0        0     7245 2024-02-17 22:53:35.836409 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.pyi
+-rw-r--r--   0        0        0     2342 2024-02-17 22:53:35.836543 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/__init__.py
+-rw-r--r--   0        0        0     4494 2024-02-17 22:53:36.238432 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.py
+-rw-r--r--   0        0        0     5711 2024-02-17 22:53:35.836833 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.pyi
+-rw-r--r--   0        0        0     3405 2024-02-17 22:53:36.238565 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.py
+-rw-r--r--   0        0        0     2687 2024-02-17 22:53:35.837015 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.pyi
+-rw-r--r--   0        0        0     2797 2024-02-17 22:53:36.238686 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.py
+-rw-r--r--   0        0        0     2318 2024-02-17 22:53:35.837236 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.pyi
+-rw-r--r--   0        0        0     4570 2024-02-17 22:53:36.238816 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.py
+-rw-r--r--   0        0        0     4998 2024-02-17 22:53:35.837489 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     4089 2024-02-17 22:53:36.238938 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.py
+-rw-r--r--   0        0        0     4314 2024-02-17 22:53:35.837659 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.pyi
+-rw-r--r--   0        0        0     4288 2024-02-17 22:53:36.239072 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.py
+-rw-r--r--   0        0        0     3511 2024-02-17 22:53:35.837971 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.pyi
+-rw-r--r--   0        0        0    14188 2024-02-17 22:53:36.239292 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.py
+-rw-r--r--   0        0        0    18723 2024-02-17 22:53:35.838244 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.pyi
+-rw-r--r--   0        0        0      347 2024-02-17 22:53:35.838387 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/__init__.py
+-rw-r--r--   0        0        0     3179 2024-02-17 22:53:36.239423 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.py
+-rw-r--r--   0        0        0     2681 2024-02-17 22:53:35.838556 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.pyi
+-rw-r--r--   0        0        0     4895 2024-02-17 22:53:36.239540 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.py
+-rw-r--r--   0        0        0     4326 2024-02-17 22:53:35.838746 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838864 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.838999 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/__init__.py
+-rw-r--r--   0        0        0      501 2024-02-17 22:53:35.839158 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/__init__.py
+-rw-r--r--   0        0        0     5338 2024-02-17 22:53:36.239682 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.py
+-rw-r--r--   0        0        0     4373 2024-02-17 22:53:35.839385 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839521 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.839653 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/__init__.py
+-rw-r--r--   0        0        0      333 2024-02-17 22:53:35.839777 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2582 2024-02-17 22:53:36.239829 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.py
+-rw-r--r--   0        0        0     2054 2024-02-17 22:53:35.839944 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.pyi
+-rw-r--r--   0        0        0      242 2024-02-17 22:53:35.840071 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/v0/__init__.py
+-rw-r--r--   0        0        0     1758 2024-02-17 22:53:36.239960 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.py
+-rw-r--r--   0        0        0      759 2024-02-17 22:53:35.840231 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840341 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/__init__.py
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.840467 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/__init__.py
+-rw-r--r--   0        0        0     3459 2024-02-17 22:53:35.840596 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/__init__.py
+-rw-r--r--   0        0        0     2985 2024-02-17 22:53:36.240102 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.py
+-rw-r--r--   0        0        0     1696 2024-02-17 22:53:35.840769 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     7338 2024-02-17 22:53:35.840894 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4621 2024-02-17 22:53:35.841017 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5607 2024-02-17 22:53:36.240240 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.py
+-rw-r--r--   0        0        0     5171 2024-02-17 22:53:35.841241 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.pyi
+-rw-r--r--   0        0        0     8037 2024-02-17 22:53:35.841367 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3606 2024-02-17 22:53:35.841477 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19234 2024-02-17 22:53:36.240352 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.py
+-rw-r--r--   0        0        0    17700 2024-02-17 22:53:35.841687 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.pyi
+-rw-r--r--   0        0        0    26649 2024-02-17 22:53:35.841813 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16371 2024-02-17 22:53:35.842002 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9552 2024-02-17 22:53:36.240545 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.py
+-rw-r--r--   0        0        0     7723 2024-02-17 22:53:35.842226 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.pyi
+-rw-r--r--   0        0        0    23014 2024-02-17 22:53:35.842330 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.py
+-rw-r--r--   0        0        0    13350 2024-02-17 22:53:35.842512 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3466 2024-02-17 22:53:35.842643 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/__init__.py
+-rw-r--r--   0        0        0     3630 2024-02-17 22:53:36.240688 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.py
+-rw-r--r--   0        0        0     1729 2024-02-17 22:53:35.842800 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.pyi
+-rw-r--r--   0        0        0     9812 2024-02-17 22:53:35.842944 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6137 2024-02-17 22:53:35.843124 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24735 2024-02-17 22:53:36.240808 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.py
+-rw-r--r--   0        0        0    22592 2024-02-17 22:53:35.843772 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.pyi
+-rw-r--r--   0        0        0    40628 2024-02-17 22:53:35.843915 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24755 2024-02-17 22:53:35.844045 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3903 2024-02-17 22:53:36.240954 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.py
+-rw-r--r--   0        0        0     2835 2024-02-17 22:53:35.844235 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.pyi
+-rw-r--r--   0        0        0     6037 2024-02-17 22:53:35.844586 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3624 2024-02-17 22:53:35.844693 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      202 2024-02-17 22:53:35.844828 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/__init__.py
+-rw-r--r--   0        0        0      273 2024-02-17 22:53:35.844970 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/v0/__init__.py
+-rw-r--r--   0        0        0     2657 2024-02-17 22:53:36.241074 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.py
+-rw-r--r--   0        0        0     2008 2024-02-17 22:53:35.845143 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.pyi
+-rw-r--r--   0        0        0      251 2024-02-17 22:53:35.845284 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/v0/__init__.py
+-rw-r--r--   0        0        0     1749 2024-02-17 22:53:36.241182 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.py
+-rw-r--r--   0        0        0      917 2024-02-17 22:53:35.845466 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.pyi
+-rw-r--r--   0        0        0      285 2024-02-17 22:53:35.845607 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/version/__init__.py
+-rw-r--r--   0        0        0     1672 2024-02-17 22:53:36.241311 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.py
+-rw-r--r--   0        0        0      672 2024-02-17 22:53:35.845773 dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.pyi
+-rw-r--r--   0        0        0     5249 2024-02-17 22:53:35.846085 dazl-8.0.0b2/python/dazl/_logging.py
+-rw-r--r--   0        0        0      990 2024-02-17 22:53:35.846274 dazl-8.0.0b2/python/dazl/_repr/__init__.py
+-rw-r--r--   0        0        0     1722 2024-02-17 22:53:35.846434 dazl-8.0.0b2/python/dazl/cli/__init__.py
+-rw-r--r--   0        0        0      602 2024-02-17 22:53:35.846572 dazl-8.0.0b2/python/dazl/cli/_base.py
+-rw-r--r--   0        0        0     2102 2024-02-17 22:53:35.846711 dazl-8.0.0b2/python/dazl/cli/ls.py
+-rw-r--r--   0        0        0     3273 2024-02-17 22:53:35.846854 dazl-8.0.0b2/python/dazl/cli/tail.py
+-rw-r--r--   0        0        0     1233 2024-02-17 22:53:35.846993 dazl-8.0.0b2/python/dazl/cli/upload.py
+-rw-r--r--   0        0        0      490 2024-02-17 22:53:35.847143 dazl-8.0.0b2/python/dazl/cli/version.py
+-rw-r--r--   0        0        0     1036 2024-02-17 22:53:35.847287 dazl-8.0.0b2/python/dazl/client/__init__.py
+-rw-r--r--   0        0        0     1339 2024-02-17 22:53:35.847416 dazl-8.0.0b2/python/dazl/client/_base_model.py
+-rw-r--r--   0        0        0     3620 2024-02-17 22:53:35.847560 dazl-8.0.0b2/python/dazl/client/_conn_settings.py
+-rw-r--r--   0        0        0     1419 2024-02-17 22:53:35.847692 dazl-8.0.0b2/python/dazl/client/_events.py
+-rw-r--r--   0        0        0    24599 2024-02-17 22:53:35.847873 dazl-8.0.0b2/python/dazl/client/_network_client_impl.py
+-rw-r--r--   0        0        0    33712 2024-02-17 22:53:35.848079 dazl-8.0.0b2/python/dazl/client/_party_client_impl.py
+-rw-r--r--   0        0        0     4786 2024-02-17 22:53:35.848254 dazl-8.0.0b2/python/dazl/client/_reader_sync.py
+-rw-r--r--   0        0        0      870 2024-02-17 22:53:35.848380 dazl-8.0.0b2/python/dazl/client/_run_level.py
+-rw-r--r--   0        0        0     2150 2024-02-17 22:53:35.848512 dazl-8.0.0b2/python/dazl/client/_writer_verify.py
+-rw-r--r--   0        0        0    68240 2024-02-17 22:53:35.848739 dazl-8.0.0b2/python/dazl/client/api.py
+-rw-r--r--   0        0        0    19922 2024-04-03 23:31:58.882040 dazl-8.0.0b2/python/dazl/client/bots.py
+-rw-r--r--   0        0        0    11197 2024-02-17 22:53:36.241744 dazl-8.0.0b2/python/dazl/client/commands.py
+-rw-r--r--   0        0        0    18771 2024-02-17 22:53:35.849292 dazl-8.0.0b2/python/dazl/client/config.py
+-rw-r--r--   0        0        0     1307 2024-02-17 22:53:35.849438 dazl-8.0.0b2/python/dazl/client/errors.py
+-rw-r--r--   0        0        0     6863 2024-02-17 22:53:35.849586 dazl-8.0.0b2/python/dazl/client/events.py
+-rw-r--r--   0        0        0     1070 2024-02-17 22:53:35.849718 dazl-8.0.0b2/python/dazl/client/ledger.py
+-rw-r--r--   0        0        0      952 2024-02-17 22:53:35.849848 dazl-8.0.0b2/python/dazl/client/runner.py
+-rw-r--r--   0        0        0     9113 2024-02-17 22:53:35.850034 dazl-8.0.0b2/python/dazl/client/state.py
+-rw-r--r--   0        0        0     1533 2024-02-17 22:53:35.850173 dazl-8.0.0b2/python/dazl/damlast/__init__.py
+-rw-r--r--   0        0        0      440 2024-02-17 22:53:35.850301 dazl-8.0.0b2/python/dazl/damlast/_base.py
+-rw-r--r--   0        0        0     3251 2024-02-17 22:53:35.850563 dazl-8.0.0b2/python/dazl/damlast/_builtins_meta.py
+-rw-r--r--   0        0        0     2394 2024-02-17 22:53:35.850708 dazl-8.0.0b2/python/dazl/damlast/builtins.py
+-rw-r--r--   0        0        0    91575 2024-02-17 22:53:35.850968 dazl-8.0.0b2/python/dazl/damlast/daml_lf_1.py
+-rw-r--r--   0        0        0     6316 2024-02-17 22:53:35.851133 dazl-8.0.0b2/python/dazl/damlast/daml_types.py
+-rw-r--r--   0        0        0     1395 2024-02-17 22:53:35.851261 dazl-8.0.0b2/python/dazl/damlast/errors.py
+-rw-r--r--   0        0        0    12557 2024-02-17 22:53:35.851482 dazl-8.0.0b2/python/dazl/damlast/expand.py
+-rw-r--r--   0        0        0    20477 2024-02-17 22:53:35.851647 dazl-8.0.0b2/python/dazl/damlast/lookup.py
+-rw-r--r--   0        0        0     2955 2024-02-17 22:53:35.851800 dazl-8.0.0b2/python/dazl/damlast/parse.py
+-rw-r--r--   0        0        0    45323 2024-02-17 22:53:35.851985 dazl-8.0.0b2/python/dazl/damlast/pb_parse.py
+-rw-r--r--   0        0        0     8997 2024-02-17 22:53:35.852177 dazl-8.0.0b2/python/dazl/damlast/pkgfile.py
+-rw-r--r--   0        0        0     4855 2024-02-17 22:53:35.852319 dazl-8.0.0b2/python/dazl/damlast/protocols.py
+-rw-r--r--   0        0        0     2938 2024-02-17 22:53:35.852452 dazl-8.0.0b2/python/dazl/damlast/types.py
+-rw-r--r--   0        0        0     5978 2024-02-17 22:53:35.852598 dazl-8.0.0b2/python/dazl/damlast/util.py
+-rw-r--r--   0        0        0    14983 2024-02-17 22:53:35.852807 dazl-8.0.0b2/python/dazl/damlast/visitor.py
+-rw-r--r--   0        0        0    27127 2024-02-17 22:53:35.852970 dazl-8.0.0b2/python/dazl/ledger/__init__.py
+-rw-r--r--   0        0        0    11396 2024-02-17 22:53:36.241948 dazl-8.0.0b2/python/dazl/ledger/__init__.pyi
+-rw-r--r--   0        0        0     2324 2024-02-17 22:53:35.853318 dazl-8.0.0b2/python/dazl/ledger/_offsets.py
+-rw-r--r--   0        0        0     1652 2024-02-17 22:53:35.853444 dazl-8.0.0b2/python/dazl/ledger/_retry.py
+-rw-r--r--   0        0        0     6622 2024-02-17 22:53:35.853593 dazl-8.0.0b2/python/dazl/ledger/aio/__init__.py
+-rw-r--r--   0        0        0    11143 2024-02-17 22:53:36.242145 dazl-8.0.0b2/python/dazl/ledger/aio/__init__.pyi
+-rw-r--r--   0        0        0     5890 2024-02-17 22:53:35.853898 dazl-8.0.0b2/python/dazl/ledger/aio/pkgloader.py
+-rw-r--r--   0        0        0     3404 2024-02-17 22:53:35.854036 dazl-8.0.0b2/python/dazl/ledger/aio/pkgloader_compat.py
+-rw-r--r--   0        0        0    24190 2024-02-17 22:53:36.242330 dazl-8.0.0b2/python/dazl/ledger/api_types.py
+-rw-r--r--   0        0        0     2117 2024-02-17 22:53:35.854345 dazl-8.0.0b2/python/dazl/ledger/blocking/__init__.py
+-rw-r--r--   0        0        0     7058 2024-02-17 22:53:36.242521 dazl-8.0.0b2/python/dazl/ledger/blocking/__init__.pyi
+-rw-r--r--   0        0        0     6846 2024-02-17 22:53:35.854636 dazl-8.0.0b2/python/dazl/ledger/blocking/_aiowrapper.py
+-rw-r--r--   0        0        0     5937 2024-02-17 22:53:35.854781 dazl-8.0.0b2/python/dazl/ledger/blocking/pkgloader.py
+-rw-r--r--   0        0        0    18153 2024-02-17 22:53:36.242680 dazl-8.0.0b2/python/dazl/ledger/config/__init__.py
+-rw-r--r--   0        0        0    20662 2024-02-17 22:53:36.242858 dazl-8.0.0b2/python/dazl/ledger/config/access.py
+-rw-r--r--   0        0        0    14197 2024-02-17 22:53:35.855738 dazl-8.0.0b2/python/dazl/ledger/config/argv.py
+-rw-r--r--   0        0        0      304 2024-02-17 22:53:35.855868 dazl-8.0.0b2/python/dazl/ledger/config/exc.py
+-rw-r--r--   0        0        0      343 2024-02-17 22:53:36.242964 dazl-8.0.0b2/python/dazl/ledger/config/log.py
+-rw-r--r--   0        0        0     2881 2024-02-17 22:53:36.243096 dazl-8.0.0b2/python/dazl/ledger/config/ssl.py
+-rw-r--r--   0        0        0    10455 2024-04-03 23:31:58.882516 dazl-8.0.0b2/python/dazl/ledger/config/url.py
+-rw-r--r--   0        0        0     4761 2024-02-17 22:53:35.856335 dazl-8.0.0b2/python/dazl/ledger/errors.py
+-rw-r--r--   0        0        0      475 2024-02-17 22:53:35.856470 dazl-8.0.0b2/python/dazl/ledger/grpc/__init__.py
+-rw-r--r--   0        0        0     1188 2024-02-17 22:53:36.243409 dazl-8.0.0b2/python/dazl/ledger/grpc/__init__.pyi
+-rw-r--r--   0        0        0     6459 2024-02-17 22:53:35.856863 dazl-8.0.0b2/python/dazl/ledger/grpc/channel.py
+-rw-r--r--   0        0        0    18849 2024-02-17 22:53:35.857023 dazl-8.0.0b2/python/dazl/ledger/grpc/codec_aio.py
+-rw-r--r--   0        0        0    47784 2024-04-05 00:21:15.428279 dazl-8.0.0b2/python/dazl/ledger/grpc/conn_aio.py
+-rw-r--r--   0        0        0      313 2024-02-17 22:53:35.857372 dazl-8.0.0b2/python/dazl/ledger/pkgcache.py
+-rw-r--r--   0        0        0      290 2024-02-17 22:53:35.857502 dazl-8.0.0b2/python/dazl/ledgerutil/__init__.py
+-rw-r--r--   0        0        0    17303 2024-02-17 22:53:35.857651 dazl-8.0.0b2/python/dazl/ledgerutil/acs.py
+-rw-r--r--   0        0        0     1883 2024-02-17 22:53:35.857792 dazl-8.0.0b2/python/dazl/ledgerutil/fetch.py
+-rw-r--r--   0        0        0      208 2024-02-17 22:53:35.857969 dazl-8.0.0b2/python/dazl/metrics/__init__.py
+-rw-r--r--   0        0        0      991 2024-02-17 22:53:35.858113 dazl-8.0.0b2/python/dazl/metrics/api.py
+-rw-r--r--   0        0        0     1614 2024-02-17 22:53:35.858277 dazl-8.0.0b2/python/dazl/metrics/instrumenters.py
+-rw-r--r--   0        0        0     1592 2024-02-17 22:53:35.858537 dazl-8.0.0b2/python/dazl/metrics/prometheus.py
+-rw-r--r--   0        0        0      829 2024-02-17 22:53:35.858713 dazl-8.0.0b2/python/dazl/pretty/__init__.py
+-rw-r--r--   0        0        0      877 2024-02-17 22:53:35.858915 dazl-8.0.0b2/python/dazl/pretty/pygments_daml_lexer.py
+-rw-r--r--   0        0        0      252 2024-02-17 22:53:35.859109 dazl-8.0.0b2/python/dazl/pretty/table/__init__.py
+-rw-r--r--   0        0        0      733 2024-02-17 22:53:35.859269 dazl-8.0.0b2/python/dazl/pretty/table/fmt_base.py
+-rw-r--r--   0        0        0     1663 2024-02-17 22:53:35.859475 dazl-8.0.0b2/python/dazl/pretty/table/fmt_json.py
+-rw-r--r--   0        0        0     5392 2024-02-17 22:53:35.859789 dazl-8.0.0b2/python/dazl/pretty/table/fmt_pretty.py
+-rw-r--r--   0        0        0     3162 2024-02-17 22:53:35.860082 dazl-8.0.0b2/python/dazl/pretty/table/model.py
+-rw-r--r--   0        0        0     1553 2024-02-17 22:53:35.860329 dazl-8.0.0b2/python/dazl/pretty/table/write.py
+-rw-r--r--   0        0        0     3318 2024-02-17 22:53:35.860492 dazl-8.0.0b2/python/dazl/pretty/util.py
+-rw-r--r--   0        0        0     1733 2024-02-17 22:53:36.243742 dazl-8.0.0b2/python/dazl/prim/__init__.py
+-rw-r--r--   0        0        0     1635 2024-02-17 22:53:35.860901 dazl-8.0.0b2/python/dazl/prim/basic.py
+-rw-r--r--   0        0        0     1645 2024-02-17 22:53:35.861044 dazl-8.0.0b2/python/dazl/prim/complex.py
+-rw-r--r--   0        0        0     2421 2024-02-17 22:53:35.861220 dazl-8.0.0b2/python/dazl/prim/contracts.py
+-rw-r--r--   0        0        0     7009 2024-02-17 22:53:35.861382 dazl-8.0.0b2/python/dazl/prim/datetime.py
+-rw-r--r--   0        0        0     1155 2024-02-17 22:53:35.861521 dazl-8.0.0b2/python/dazl/prim/errors.py
+-rw-r--r--   0        0        0     1521 2024-02-17 22:53:35.861669 dazl-8.0.0b2/python/dazl/prim/json.py
+-rw-r--r--   0        0        0     1398 2024-02-17 22:53:35.861826 dazl-8.0.0b2/python/dazl/prim/map.py
+-rw-r--r--   0        0        0     1476 2024-02-17 22:53:35.861995 dazl-8.0.0b2/python/dazl/prim/numbers.py
+-rw-r--r--   0        0        0     1144 2024-04-03 23:31:58.882763 dazl-8.0.0b2/python/dazl/prim/party.py
+-rw-r--r--   0        0        0      405 2024-02-17 22:53:35.862535 dazl-8.0.0b2/python/dazl/protocols/__init__.py
+-rw-r--r--   0        0        0     6120 2024-02-17 22:53:35.862723 dazl-8.0.0b2/python/dazl/protocols/_base.py
+-rw-r--r--   0        0        0     9246 2024-02-17 22:53:35.863100 dazl-8.0.0b2/python/dazl/protocols/autodetect.py
+-rw-r--r--   0        0        0     2927 2024-02-17 22:53:35.863392 dazl-8.0.0b2/python/dazl/protocols/core.py
+-rw-r--r--   0        0        0      891 2024-02-17 22:53:36.243999 dazl-8.0.0b2/python/dazl/protocols/errors.py
+-rw-r--r--   0        0        0     6889 2024-02-17 22:53:35.863784 dazl-8.0.0b2/python/dazl/protocols/events.py
+-rw-r--r--   0        0        0     2337 2024-02-17 22:53:35.864028 dazl-8.0.0b2/python/dazl/protocols/oauth.py
+-rw-r--r--   0        0        0     4619 2024-02-17 22:53:35.864252 dazl-8.0.0b2/python/dazl/protocols/serializers.py
+-rw-r--r--   0        0        0      141 2024-02-17 22:53:35.864476 dazl-8.0.0b2/python/dazl/protocols/v1/__init__.py
+-rw-r--r--   0        0        0    17052 2024-02-17 22:53:35.864680 dazl-8.0.0b2/python/dazl/protocols/v1/grpc.py
+-rw-r--r--   0        0        0    16229 2024-02-17 22:53:35.864920 dazl-8.0.0b2/python/dazl/protocols/v1/pb_parse_event.py
+-rw-r--r--   0        0        0     4799 2024-02-17 22:53:35.865063 dazl-8.0.0b2/python/dazl/protocols/v1/pb_ser_command.py
+-rw-r--r--   0        0        0      194 2024-02-17 22:53:35.865241 dazl-8.0.0b2/python/dazl/py.typed
+-rw-r--r--   0        0        0     4796 2024-02-17 22:53:35.865561 dazl-8.0.0b2/python/dazl/query/__init__.py
+-rw-r--r--   0        0        0      270 2024-02-17 22:53:35.865783 dazl-8.0.0b2/python/dazl/scheduler/__init__.py
+-rw-r--r--   0        0        0     1318 2024-02-17 22:53:35.865997 dazl-8.0.0b2/python/dazl/scheduler/_base.py
+-rw-r--r--   0        0        0     5076 2024-02-17 22:53:35.866174 dazl-8.0.0b2/python/dazl/scheduler/_invoker.py
+-rw-r--r--   0        0        0     2062 2024-02-17 22:53:35.866302 dazl-8.0.0b2/python/dazl/scheduler/_invoker.pyi
+-rw-r--r--   0        0        0      575 2024-02-17 22:53:35.866428 dazl-8.0.0b2/python/dazl/server/__init__.py
+-rw-r--r--   0        0        0     3256 2024-02-17 22:53:35.866567 dazl-8.0.0b2/python/dazl/server/management.py
+-rw-r--r--   0        0        0     1766 2024-02-17 22:53:35.866693 dazl-8.0.0b2/python/dazl/server/metrics.py
+-rw-r--r--   0        0        0      355 2024-02-17 22:53:35.866819 dazl-8.0.0b2/python/dazl/testing/__init__.py
+-rw-r--r--   0        0        0     2296 2024-02-17 22:53:35.866945 dazl-8.0.0b2/python/dazl/testing/_cert.py
+-rw-r--r--   0        0        0    12650 2024-02-17 22:53:35.867157 dazl-8.0.0b2/python/dazl/testing/_sandbox.py
+-rw-r--r--   0        0        0     7137 2024-02-17 22:53:36.244158 dazl-8.0.0b2/python/dazl/testing/connect.py
+-rw-r--r--   0        0        0     3403 2024-02-17 22:53:36.244285 dazl-8.0.0b2/python/dazl/testing/connect.pyi
+-rw-r--r--   0        0        0      488 2024-02-17 22:53:35.867581 dazl-8.0.0b2/python/dazl/util/__init__.py
+-rw-r--r--   0        0        0    19677 2024-02-17 22:53:36.244448 dazl-8.0.0b2/python/dazl/util/asyncio_util.py
+-rw-r--r--   0        0        0     4795 2024-04-03 23:31:58.883054 dazl-8.0.0b2/python/dazl/util/config_meta.py
+-rw-r--r--   0        0        0      964 2024-02-17 22:53:35.868034 dazl-8.0.0b2/python/dazl/util/enum.py
+-rw-r--r--   0        0        0     2657 2024-04-03 23:31:58.883245 dazl-8.0.0b2/python/dazl/util/io.py
+-rw-r--r--   0        0        0      521 2024-02-17 22:53:36.244591 dazl-8.0.0b2/python/dazl/util/prim_natural.py
+-rw-r--r--   0        0        0     3515 2024-02-17 22:53:36.244719 dazl-8.0.0b2/python/dazl/util/proc_util.py
+-rw-r--r--   0        0        0     1391 2024-02-17 22:53:36.244841 dazl-8.0.0b2/python/dazl/util/termcap.py
+-rw-r--r--   0        0        0     2347 2024-02-17 22:53:35.868846 dazl-8.0.0b2/python/dazl/util/tools.py
+-rw-r--r--   0        0        0      890 2024-02-17 22:53:35.868988 dazl-8.0.0b2/python/dazl/util/typing.py
+-rw-r--r--   0        0        0      612 2024-02-17 22:53:35.869136 dazl-8.0.0b2/python/dazl/values/__init__.py
+-rw-r--r--   0        0        0     6068 2024-02-17 22:53:35.869300 dazl-8.0.0b2/python/dazl/values/canonical.py
+-rw-r--r--   0        0        0    15792 2024-02-17 22:53:35.869533 dazl-8.0.0b2/python/dazl/values/context.py
+-rw-r--r--   0        0        0     1881 2024-02-17 22:53:35.869663 dazl-8.0.0b2/python/dazl/values/json.py
+-rw-r--r--   0        0        0     3359 2024-02-17 22:53:35.869788 dazl-8.0.0b2/python/dazl/values/mapper.py
+-rw-r--r--   0        0        0     9955 2024-02-17 22:53:35.869972 dazl-8.0.0b2/python/dazl/values/protobuf.py
+-rw-r--r--   0        0        0     2755 2024-02-17 22:53:35.870119 dazl-8.0.0b2/python/dazl/values/pysample_encoder.py
+-rw-r--r--   0        0        0     5018 2024-02-17 22:53:35.870284 dazl-8.0.0b2/python/dazl/values/string.py
+-rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 dazl-8.0.0b2/PKG-INFO
```

### Comparing `dazl-8.0.0b1/LICENSE` & `dazl-8.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/README.md` & `dazl-8.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/pyproject.toml` & `dazl-8.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2017-2024 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "dazl"
-version = "8.0.0b1"
+version = "8.0.0b2"
 description = "high-level Ledger API client for Daml ledgers"
 license = "Apache-2.0"
 authors = ["Davin K. Tanabe <davin.tanabe@digitalasset.com>"]
 readme = 'README.md'
 repository = "https://github.com/digital-asset/dazl-client"
 homepage = "https://github.com/digital-asset/dazl-client"
 keywords = ["daml", "blockchain", "dlt", "distributed ledger", "digital asset"]
```

### Comparing `dazl-8.0.0b1/python/_dazl/__main__.py` & `dazl-8.0.0b2/python/_dazl/__main__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/_logging.py` & `dazl-8.0.0b2/python/_dazl/_logging.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/codegen/go.py` & `dazl-8.0.0b2/python/_dazl/codegen/go.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/codegen/python.py` & `dazl-8.0.0b2/python/_dazl/codegen/python.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/codegen/python_grpc_pyi.py` & `dazl-8.0.0b2/python/_dazl/codegen/python_grpc_pyi.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/codegen/python_init.py` & `dazl-8.0.0b2/python/_dazl/codegen/python_init.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/codegen/util.py` & `dazl-8.0.0b2/python/_dazl/codegen/util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/collections.py` & `dazl-8.0.0b2/python/_dazl/collections.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/download/__init__.py` & `dazl-8.0.0b2/python/_dazl/download/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/protoc/__init__.py` & `dazl-8.0.0b2/python/_dazl/protoc/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/protopack/__init__.py` & `dazl-8.0.0b2/python/_dazl/protopack/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/protopack/rename.py` & `dazl-8.0.0b2/python/_dazl/protopack/rename.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/protopack/rewrite.py` & `dazl-8.0.0b2/python/_dazl/protopack/rewrite.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/__init__.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/_basic.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/_basic.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/imports.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/imports.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/pb.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/pb.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/symbols.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/symbols.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/syntax/python/types.py` & `dazl-8.0.0b2/python/_dazl/syntax/python/types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/_dazl/update.py` & `dazl-8.0.0b2/python/_dazl/update.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/__init__.py` & `dazl-8.0.0b2/python/dazl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
     from google.protobuf.pyext import _message
 
     _message.SetAllowOversizeProtos(True)
 except ImportError:
     pass
 
 
-__version__ = "8.0.0b1"
+__version__ = "8.0.0b2"
```

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/daml_lf_1_15/daml_lf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/identity_provider_config_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/metering_report_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/object_meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/admin/user_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/contract_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/event_query_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/experimental_features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/admin/v0/vault_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/crypto/v0/crypto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/domain_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_mediator_administration_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_administration_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/enterprise_sequencer_connection_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/mediator_initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_administration_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_initialization_snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v0/sequencer_version_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v1/sequencer_initialization_snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/mediator_initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/admin/v2/sequencer_initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/domain_time_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_authentication_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connect_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/sequencer_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v0/service_agreement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/domain/api/v1/sequencer_connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/health/admin/v0/status_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/domain_connectivity_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/enterprise_participant_replication_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/inspection_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/package_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/participant_repair_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/party_name_management_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/ping_pong_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/pruning_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/resource_management_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/traffic_control_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/admin/v0/transfer_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/ledger_sync_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/participant/protocol/v0/submission_tracking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/acs_commitments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/causality_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/mediator_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/merkle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/participant_transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/sequencing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/storage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/synchronization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_ext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v0/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/mediator_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/merkle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/participant_transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/sequencing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/synchronization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v1/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/domain_params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/mediator_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/participant_transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/synchronization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v2/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/participant_transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/protocol/v3/synchronization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/pruning/admin/v0/pruning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/admin/v0/time_tracker_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/time/v0/time_proof_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_aggregation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_read_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v0/topology_manager_write_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/__init__.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/initialization_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_read_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/topology/admin/v1/topology_manager_write_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/traffic/v0/member_traffic_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/v0/trace_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.py` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.pyi` & `dazl-8.0.0b2/python/dazl/_gen/com/digitalasset/canton/version/untyped_versioned_message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_logging.py` & `dazl-8.0.0b2/python/dazl/_logging.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/_repr/__init__.py` & `dazl-8.0.0b2/python/dazl/_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/cli/__init__.py` & `dazl-8.0.0b2/python/dazl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/cli/_base.py` & `dazl-8.0.0b2/python/dazl/cli/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/cli/ls.py` & `dazl-8.0.0b2/python/dazl/cli/ls.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/cli/tail.py` & `dazl-8.0.0b2/python/dazl/cli/tail.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/cli/upload.py` & `dazl-8.0.0b2/python/dazl/cli/upload.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/__init__.py` & `dazl-8.0.0b2/python/dazl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_base_model.py` & `dazl-8.0.0b2/python/dazl/client/_base_model.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_conn_settings.py` & `dazl-8.0.0b2/python/dazl/client/_conn_settings.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_events.py` & `dazl-8.0.0b2/python/dazl/client/_events.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_network_client_impl.py` & `dazl-8.0.0b2/python/dazl/client/_network_client_impl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_party_client_impl.py` & `dazl-8.0.0b2/python/dazl/client/_party_client_impl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_reader_sync.py` & `dazl-8.0.0b2/python/dazl/client/_reader_sync.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_run_level.py` & `dazl-8.0.0b2/python/dazl/client/_run_level.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/_writer_verify.py` & `dazl-8.0.0b2/python/dazl/client/_writer_verify.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/api.py` & `dazl-8.0.0b2/python/dazl/client/api.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/bots.py` & `dazl-8.0.0b2/python/dazl/client/bots.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/commands.py` & `dazl-8.0.0b2/python/dazl/client/commands.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/config.py` & `dazl-8.0.0b2/python/dazl/client/config.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/errors.py` & `dazl-8.0.0b2/python/dazl/client/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/events.py` & `dazl-8.0.0b2/python/dazl/client/events.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/ledger.py` & `dazl-8.0.0b2/python/dazl/client/ledger.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/runner.py` & `dazl-8.0.0b2/python/dazl/client/runner.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/client/state.py` & `dazl-8.0.0b2/python/dazl/client/state.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/__init__.py` & `dazl-8.0.0b2/python/dazl/damlast/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/_builtins_meta.py` & `dazl-8.0.0b2/python/dazl/damlast/_builtins_meta.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/builtins.py` & `dazl-8.0.0b2/python/dazl/damlast/builtins.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/daml_lf_1.py` & `dazl-8.0.0b2/python/dazl/damlast/daml_lf_1.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/daml_types.py` & `dazl-8.0.0b2/python/dazl/damlast/daml_types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/errors.py` & `dazl-8.0.0b2/python/dazl/damlast/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/expand.py` & `dazl-8.0.0b2/python/dazl/damlast/expand.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/lookup.py` & `dazl-8.0.0b2/python/dazl/damlast/lookup.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/parse.py` & `dazl-8.0.0b2/python/dazl/damlast/parse.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/pb_parse.py` & `dazl-8.0.0b2/python/dazl/damlast/pb_parse.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/pkgfile.py` & `dazl-8.0.0b2/python/dazl/damlast/pkgfile.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/protocols.py` & `dazl-8.0.0b2/python/dazl/damlast/protocols.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/types.py` & `dazl-8.0.0b2/python/dazl/damlast/types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/util.py` & `dazl-8.0.0b2/python/dazl/damlast/util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/damlast/visitor.py` & `dazl-8.0.0b2/python/dazl/damlast/visitor.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/__init__.py` & `dazl-8.0.0b2/python/dazl/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/__init__.pyi` & `dazl-8.0.0b2/python/dazl/ledger/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/_offsets.py` & `dazl-8.0.0b2/python/dazl/ledger/_offsets.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/_retry.py` & `dazl-8.0.0b2/python/dazl/ledger/_retry.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/aio/__init__.py` & `dazl-8.0.0b2/python/dazl/ledger/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/aio/__init__.pyi` & `dazl-8.0.0b2/python/dazl/ledger/aio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader.py` & `dazl-8.0.0b2/python/dazl/ledger/aio/pkgloader.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/aio/pkgloader_compat.py` & `dazl-8.0.0b2/python/dazl/ledger/aio/pkgloader_compat.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/api_types.py` & `dazl-8.0.0b2/python/dazl/ledger/api_types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.py` & `dazl-8.0.0b2/python/dazl/ledger/blocking/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/blocking/__init__.pyi` & `dazl-8.0.0b2/python/dazl/ledger/blocking/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/blocking/_aiowrapper.py` & `dazl-8.0.0b2/python/dazl/ledger/blocking/_aiowrapper.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/blocking/pkgloader.py` & `dazl-8.0.0b2/python/dazl/ledger/blocking/pkgloader.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/config/__init__.py` & `dazl-8.0.0b2/python/dazl/ledger/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/config/access.py` & `dazl-8.0.0b2/python/dazl/ledger/config/access.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/config/argv.py` & `dazl-8.0.0b2/python/dazl/ledger/config/argv.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/config/ssl.py` & `dazl-8.0.0b2/python/dazl/ledger/config/ssl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/config/url.py` & `dazl-8.0.0b2/python/dazl/ledger/config/url.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/errors.py` & `dazl-8.0.0b2/python/dazl/ledger/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/grpc/__init__.pyi` & `dazl-8.0.0b2/python/dazl/ledger/grpc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/grpc/channel.py` & `dazl-8.0.0b2/python/dazl/ledger/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/grpc/codec_aio.py` & `dazl-8.0.0b2/python/dazl/ledger/grpc/codec_aio.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledger/grpc/conn_aio.py` & `dazl-8.0.0b2/python/dazl/ledger/grpc/conn_aio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1161,9 +1161,13 @@
 
         for name, f in self._filters.items():
             # for each filter, if this contract type could be interpreted as a match for the current
             # filter, then apply a client-side filter
             if is_match(name, event.contract_id.value_type):
                 return f.client_side is None or f.client_side(event.payload)
 
-        # we checked every name, but none of them matched
-        return False
+        # TODO: We checked every name, but none of them matched. This means we received an event for an
+        #  unexpected template name, and that could happen if the query was _interface_ based, as
+        #  opposed to _template_ based. For now, return True so that interface-based queries work at all,
+        #  but a better fix would be to check templates against a filter on the interface. This requires
+        #  us to have a bit more intelligence about the types coming over the wire.
+        return True
```

### Comparing `dazl-8.0.0b1/python/dazl/ledgerutil/acs.py` & `dazl-8.0.0b2/python/dazl/ledgerutil/acs.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/ledgerutil/fetch.py` & `dazl-8.0.0b2/python/dazl/ledgerutil/fetch.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/metrics/api.py` & `dazl-8.0.0b2/python/dazl/metrics/api.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/metrics/instrumenters.py` & `dazl-8.0.0b2/python/dazl/metrics/instrumenters.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/metrics/prometheus.py` & `dazl-8.0.0b2/python/dazl/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/__init__.py` & `dazl-8.0.0b2/python/dazl/pretty/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/pygments_daml_lexer.py` & `dazl-8.0.0b2/python/dazl/pretty/pygments_daml_lexer.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/table/fmt_base.py` & `dazl-8.0.0b2/python/dazl/pretty/table/fmt_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/table/fmt_json.py` & `dazl-8.0.0b2/python/dazl/pretty/table/fmt_json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/table/fmt_pretty.py` & `dazl-8.0.0b2/python/dazl/pretty/table/fmt_pretty.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/table/model.py` & `dazl-8.0.0b2/python/dazl/pretty/table/model.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/table/write.py` & `dazl-8.0.0b2/python/dazl/pretty/table/write.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/pretty/util.py` & `dazl-8.0.0b2/python/dazl/pretty/util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/__init__.py` & `dazl-8.0.0b2/python/dazl/prim/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/basic.py` & `dazl-8.0.0b2/python/dazl/prim/basic.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/complex.py` & `dazl-8.0.0b2/python/dazl/prim/complex.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/contracts.py` & `dazl-8.0.0b2/python/dazl/prim/contracts.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/datetime.py` & `dazl-8.0.0b2/python/dazl/prim/datetime.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/errors.py` & `dazl-8.0.0b2/python/dazl/prim/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/json.py` & `dazl-8.0.0b2/python/dazl/prim/json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/map.py` & `dazl-8.0.0b2/python/dazl/prim/map.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/numbers.py` & `dazl-8.0.0b2/python/dazl/prim/numbers.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/prim/party.py` & `dazl-8.0.0b2/python/dazl/prim/party.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/_base.py` & `dazl-8.0.0b2/python/dazl/protocols/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/autodetect.py` & `dazl-8.0.0b2/python/dazl/protocols/autodetect.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/core.py` & `dazl-8.0.0b2/python/dazl/protocols/core.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/errors.py` & `dazl-8.0.0b2/python/dazl/protocols/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/events.py` & `dazl-8.0.0b2/python/dazl/protocols/events.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/oauth.py` & `dazl-8.0.0b2/python/dazl/protocols/oauth.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/serializers.py` & `dazl-8.0.0b2/python/dazl/protocols/serializers.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/v1/grpc.py` & `dazl-8.0.0b2/python/dazl/protocols/v1/grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/v1/pb_parse_event.py` & `dazl-8.0.0b2/python/dazl/protocols/v1/pb_parse_event.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/protocols/v1/pb_ser_command.py` & `dazl-8.0.0b2/python/dazl/protocols/v1/pb_ser_command.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/query/__init__.py` & `dazl-8.0.0b2/python/dazl/query/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/scheduler/_base.py` & `dazl-8.0.0b2/python/dazl/scheduler/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/scheduler/_invoker.py` & `dazl-8.0.0b2/python/dazl/scheduler/_invoker.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/scheduler/_invoker.pyi` & `dazl-8.0.0b2/python/dazl/scheduler/_invoker.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/server/__init__.py` & `dazl-8.0.0b2/python/dazl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/server/management.py` & `dazl-8.0.0b2/python/dazl/server/management.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/server/metrics.py` & `dazl-8.0.0b2/python/dazl/server/metrics.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/testing/_cert.py` & `dazl-8.0.0b2/python/dazl/testing/_cert.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/testing/_sandbox.py` & `dazl-8.0.0b2/python/dazl/testing/_sandbox.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/testing/connect.py` & `dazl-8.0.0b2/python/dazl/testing/connect.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/testing/connect.pyi` & `dazl-8.0.0b2/python/dazl/testing/connect.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/asyncio_util.py` & `dazl-8.0.0b2/python/dazl/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/config_meta.py` & `dazl-8.0.0b2/python/dazl/util/config_meta.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/enum.py` & `dazl-8.0.0b2/python/dazl/util/enum.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/io.py` & `dazl-8.0.0b2/python/dazl/util/io.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/prim_natural.py` & `dazl-8.0.0b2/python/dazl/util/prim_natural.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/proc_util.py` & `dazl-8.0.0b2/python/dazl/util/proc_util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/termcap.py` & `dazl-8.0.0b2/python/dazl/util/termcap.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/tools.py` & `dazl-8.0.0b2/python/dazl/util/tools.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/util/typing.py` & `dazl-8.0.0b2/python/dazl/util/typing.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/__init__.py` & `dazl-8.0.0b2/python/dazl/values/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/canonical.py` & `dazl-8.0.0b2/python/dazl/values/canonical.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/context.py` & `dazl-8.0.0b2/python/dazl/values/context.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/json.py` & `dazl-8.0.0b2/python/dazl/values/json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/mapper.py` & `dazl-8.0.0b2/python/dazl/values/mapper.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/protobuf.py` & `dazl-8.0.0b2/python/dazl/values/protobuf.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/pysample_encoder.py` & `dazl-8.0.0b2/python/dazl/values/pysample_encoder.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/python/dazl/values/string.py` & `dazl-8.0.0b2/python/dazl/values/string.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0b1/PKG-INFO` & `dazl-8.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dazl
-Version: 8.0.0b1
+Version: 8.0.0b2
 Summary: high-level Ledger API client for Daml ledgers
 Home-page: https://github.com/digital-asset/dazl-client
 License: Apache-2.0
 Keywords: daml,blockchain,dlt,distributed ledger,digital asset
 Author: Davin K. Tanabe
 Author-email: davin.tanabe@digitalasset.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dazl Version: 8.0.0b1 Summary: high-level Ledger
+Metadata-Version: 2.1 Name: dazl Version: 8.0.0b2 Summary: high-level Ledger
 API client for Daml ledgers Home-page: https://github.com/digital-asset/dazl-
 client License: Apache-2.0 Keywords: daml,blockchain,dlt,distributed
 ledger,digital asset Author: Davin K. Tanabe Author-email:
 davin.tanabe@digitalasset.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

