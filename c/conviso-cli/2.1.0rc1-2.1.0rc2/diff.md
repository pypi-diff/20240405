# Comparing `tmp/conviso-cli-2.1.0rc1.tar.gz` & `tmp/conviso-cli-2.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-cli-2.1.0rc1.tar", last modified: Mon Mar 25 17:36:18 2024, max compression
+gzip compressed data, was "conviso-cli-2.1.0rc2.tar", last modified: Tue Mar 26 16:15:32 2024, max compression
```

## Comparing `conviso-cli-2.1.0rc1.tar` & `conviso-cli-2.1.0rc2.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)      544 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/conviso_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      544 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5691 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-25 17:36:18.000000 conviso-cli-2.1.0rc1/conviso_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)      105 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/git_data_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/common/graphql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/graphql/error_handlers.py
--rw-r--r--   0 root         (0) root         (0)      247 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/graphql/errors.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/graphql/low_client.py
--rw-r--r--   0 root         (0) root         (0)      185 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/common/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12044 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
--rw-r--r--   0 root         (0) root         (0)     3614 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/asset.py
--rw-r--r--   0 root         (0) root         (0)      511 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/issues.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/project.py
--rw-r--r--   0 root         (0) root         (0)     6458 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)     1254 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)     2352 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4726 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/util/ci_provider.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)    14635 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/create.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/ls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/ast/
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/ast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9410 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/ast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5350 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/companies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      892 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/companies/ls.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.832069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     4681 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      344 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/import_sarif/
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/import_sarif/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/iac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/iac/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11198 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/iac/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/projects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/projects/ls.py
--rw-r--r--   0 root         (0) root         (0)     9438 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/requirements_verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    19208 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    10781 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4937 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      386 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/rules_schema.json
--rw-r--r--   0 root         (0) root         (0)    13962 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/run.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     9232 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       27 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.828069 conviso-cli-2.1.0rc1/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 17:36:18.836069 conviso-cli-2.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1882 2024-03-25 17:36:15.000000 conviso-cli-2.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)      544 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/conviso_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      544 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-03-26 16:15:32.000000 conviso-cli-2.1.0rc2/conviso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/common/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/box.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/docker.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/git_data_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/common/graphql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/graphql/error_handlers.py
+-rw-r--r--   0 root         (0) root         (0)      247 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/graphql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/graphql/low_client.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/common/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12044 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.152301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/issues.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/scc.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/util/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/util/ci_provider.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/util/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/util/source_code_compressor.py
+-rw-r--r--   0 root         (0) root         (0)    14635 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/version_control_system_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/
+-rw-r--r--   0 root         (0) root         (0)      294 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/version_searcher_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flow/versioning_style/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/versioning_style/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flow/versioning_style/semantic_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.156301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/create.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/ls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/ast/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/ast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/companies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      892 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/companies/ls.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/ls.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/show.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/with_/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/with_/version_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      344 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/import_sarif/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/import_sarif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/iac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/iac/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/iac/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.160301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/projects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/projects/ls.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/requirements_verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sast/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    19208 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sast/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sca/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sca/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/sca/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-r--r--   0 root         (0) root         (0)      386 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/rules_schema.json
+-rw-r--r--   0 root         (0) root         (0)    16094 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/run.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/convisoappsec/sast/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/sast/decision.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/sast/sastbox.py
+-rw-r--r--   0 root         (0) root         (0)       27 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/convisoappsec/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.148301 conviso-cli-2.1.0rc2/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/scripts/shell_completer/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/scripts/shell_completer/flow_bash_completer.sh
+-rw-r--r--   0 root         (0) root         (0)      147 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/scripts/shell_completer/flow_fish_completer.fish
+-rw-r--r--   0 root         (0) root         (0)      844 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/scripts/shell_completer/flow_zsh_completer.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 16:15:32.164301 conviso-cli-2.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-03-26 16:15:29.000000 conviso-cli-2.1.0rc2/setup.py
```

### Comparing `conviso-cli-2.1.0rc1/PKG-INFO` & `conviso-cli-2.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.0rc1
+Version: 2.1.0rc2
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.0rc1/conviso_cli.egg-info/PKG-INFO` & `conviso-cli-2.1.0rc2/conviso_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.0rc1
+Version: 2.1.0rc2
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.0rc1/conviso_cli.egg-info/SOURCES.txt` & `conviso-cli-2.1.0rc2/conviso_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/common/box.py` & `conviso-cli-2.1.0rc2/convisoappsec/common/box.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/common/docker.py` & `conviso-cli-2.1.0rc2/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/common/git_data_parser.py` & `conviso-cli-2.1.0rc2/convisoappsec/common/git_data_parser.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/common/graphql/error_handlers.py` & `conviso-cli-2.1.0rc2/convisoappsec/common/graphql/error_handlers.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/common/graphql/low_client.py` & `conviso-cli-2.1.0rc2/convisoappsec/common/graphql/low_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from convisoappsec.common.graphql.error_handlers import GraphQlErrorHandler, RequestErrorHandler
 
 
 class GraphQLClient:
     DEFAULT_HEADERS = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
+        "User-Agent": "AST",
     }
 
     def __init__(self, url, headers={}):
         self.url = url
         self.__session = requests.Session()
         self.__session.headers.update(
             **self.DEFAULT_HEADERS,
```

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/api.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/sast.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/sast.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/models/issues/sca.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/models/issues/sca.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/resources_api.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/client.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/client.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/models/project.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/models/project.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/resources_api.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/util/ci_provider.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/util/ci_provider.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/version_control_system_adapter.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/version_control_system_adapter.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-cli-2.1.0rc2/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/create.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/create.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/assets/ls.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/assets/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/ast/entrypoint.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/ast/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/common.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/common.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/companies/ls.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/companies/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/context.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/ls.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/deploy/show.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/deploy/show.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/entrypoint.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/create/with_/version_tracker.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/findings/import_sarif/entrypoint.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/findings/import_sarif/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/iac/run.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/iac/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,27 +175,28 @@
             )
 
             with open(compatible_report_filepath) as report_file:
                 report_content = json.load(report_file)
 
                 issues = report_content.get("issues", [])
                 for issue in issues:
+                    hash_issue = issue.get('hash_issue_v2', [])
                     issue_model = CreateIacFindingInput(
                         asset_id=asset_id,
                         file_name=issue.get("filename"),
                         vulnerable_line=issue.get("line"),
                         title=issue.get("title"),
                         description=issue.get("description"),
                         severity=issue.get("severity"),
                         deploy_id=deploy_id,
                         code_snippet=parse_code_snippet(issue.get("evidence")),
                         reference=parse_conviso_references(issue.get("references")),
                         first_line=parse_first_line_number(issue.get("evidence")),
                         commit_ref=commit_ref,
-                        original_issue_id_from_tool=None
+                        original_issue_id_from_tool=hash_issue,
                     )
 
                     try:
                         conviso_api.issues.create_iac(issue_model)
                     except ReponseError as error:
                         if error.code == 'RECORD_NOT_UNIQUE':
                             duplicated_issues += 1
```

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/projects/ls.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/projects/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/requirements_verifier.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/requirements_verifier.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/sast/run.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/sast/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/sca/run.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/sca/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/rules_schema.json` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/rules_schema.json`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/flowcli/vulnerability/run.py` & `conviso-cli-2.1.0rc2/convisoappsec/flowcli/vulnerability/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.sast.sastbox import SASTBox
 from convisoappsec.flowcli.common import (asset_id_option, project_code_option, on_http_error)
 from convisoappsec.flowcli.findings import import_sarif
 from convisoappsec.flowcli.requirements_verifier import RequirementsVerifier
 from convisoappsec.flow import GitAdapter
-from convisoappsec.common.box import ContainerWrapper
+from convisoappsec.common.box import ContainerWrapper, convert_sarif_to_sastbox1
 
 
 @click.command()
 @project_code_option(required=False)
 @asset_id_option(required=False)
 @click.option(
     "-s",
@@ -214,26 +214,23 @@
     sca_issues_with_fix_accepted = [item for item in merged_issues_sca if item['status'] == 'FIX_ACCEPTED']
     sca_issues_without_fix_accepted = [item for item in merged_issues_sca if item['status'] != 'FIX_ACCEPTED']
 
     if len(issues_from_cp) == 0:
         log_func("No vulnerabilities was founded on conviso platform!")
         return
 
-    sast_hash_issues = perform_sastbox_scan(
-        sastbox_registry,
-        sastbox_repository_name,
-        sastbox_tag,
-        sastbox_skip_login,
-        repository_dir,
-        end_commit,
-        start_commit,
-        log_func,
-    )
+    # Starting executing the ast again
+    sast_hash_issues = perform_sastbox_scan(sastbox_registry, sastbox_repository_name, sastbox_tag, repository_dir)
+
+    sca_hash_issues = perform_sca_scan(repository_dir=repository_dir)
+    iac_hash_issues = perform_iac_scan(repository_dir=repository_dir)
 
-    sca_hash_issues = perform_sca_scan(repository_dir = repository_dir)
+    # we need to append the two lists because at the moment this was made, iac and sast has sast as type on cp.
+    sast_hash_issues = sast_hash_issues + iac_hash_issues
+    # end ast execution
 
     if len(sast_hash_issues) == 0 and len(sca_hash_issues) == 0:
         log_func("No vulnerabilities was founded congrats !!!")
         return
 
     set_of_sast_hash_issues = set(sast_hash_issues)
     set_of_sca_hash_issues = set(sca_hash_issues)
@@ -323,25 +320,16 @@
         issue_id = issue['id']
         status = 'CREATED'
 
         conviso_api.issues.update_issue_status(issue_id = issue_id, status = status)
 
 
 @pass_flow_context
-def perform_sastbox_scan(
-        flow_context,
-        sastbox_registry,
-        sastbox_repository_name,
-        sastbox_tag,
-        sastbox_skip_login,
-        repository_dir,
-        end_commit,
-        start_commit,
-        logger,
-):
+def perform_sastbox_scan(flow_context, sastbox_registry, sastbox_repository_name, sastbox_tag, repository_dir,):
+
     sastbox = SASTBox(
         registry=sastbox_registry,
         repository_name=sastbox_repository_name,
         tag=sastbox_tag,
     )
 
     conviso_rest_api = flow_context.create_conviso_rest_api_client()
@@ -430,9 +418,67 @@
         return hash_issues
 
     except Exception as e:
         on_http_error(e)
         raise click.ClickException(str(e)) from e
 
 
+@pass_flow_context
+def perform_iac_scan(flow_context, repository_dir):
+    """ Perform an iac scan """
+    try:
+        REQUIRED_CODEBASE_PATH = '/code'
+        IAC_IMAGE_NAME = 'sastbox-iac-scanner-checkov'
+        IAC_SCAN_FILENAME = '/{}.sarif'.format(IAC_IMAGE_NAME)
+        containers_map = {
+            IAC_IMAGE_NAME: {
+                'repository_dir': repository_dir,
+                'repository_name': IAC_IMAGE_NAME,
+                'tag': 'latest',
+                'command': [
+                    '-v',
+                    '--codebase', REQUIRED_CODEBASE_PATH,
+                    '--output', IAC_SCAN_FILENAME
+                ],
+            },
+        }
+
+        conviso_rest_api = flow_context.create_conviso_rest_api_client()
+        token = conviso_rest_api.docker_registry.get_sast_token()
+        scanners_wrapper = ContainerWrapper(
+            token=token,
+            containers_map=containers_map,
+            logger=None,
+            timeout=7200
+        )
+
+        scanners_wrapper.run()
+
+        results_filepaths = []  # [str(r.results) for r in scanners_wrapper.scanners]
+        hash_issues = []
+
+        for r in scanners_wrapper.scanners:
+            report_filepath = r.results
+            if report_filepath:
+                results_filepaths.append(report_filepath)
+
+        for report_path in results_filepaths:
+            try:
+                compatible_report_filepath = convert_sarif_to_sastbox1(
+                    report_path, repository_dir, token, 1700
+                )
+
+                with open(compatible_report_filepath) as report_file:
+                    report_content = json.load(report_file)
+                    issues = report_content.get("issues", [])
+                    hash_issues.extend(issue.get("hash_issue_v2") for issue in issues)
+            except (FileNotFoundError, json.JSONDecodeError) as e:
+                print(f"Error processing {report_path}: {e}")
+
+        return hash_issues
+    except Exception as e:
+        on_http_error(e)
+        raise click.ClickException(str(e)) from e
+
+
 def log_func(msg, new_line=True):
     click.echo(click.style(msg, bold=True, fg='blue'), nl=new_line, err=True)
```

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/sast/decision.py` & `conviso-cli-2.1.0rc2/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/convisoappsec/sast/sastbox.py` & `conviso-cli-2.1.0rc2/convisoappsec/sast/sastbox.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/scripts/shell_completer/flow_bash_completer.sh` & `conviso-cli-2.1.0rc2/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-cli-2.1.0rc2/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.0rc1/setup.py` & `conviso-cli-2.1.0rc2/setup.py`

 * *Files identical despite different names*

