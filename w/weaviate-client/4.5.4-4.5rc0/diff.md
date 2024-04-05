# Comparing `tmp/weaviate-client-4.5.4.tar.gz` & `tmp/weaviate-client-4.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate-client-4.5.4.tar", last modified: Sat Mar 16 05:30:47 2024, max compression
+gzip compressed data, was "weaviate-client-4.5rc0.tar", last modified: Fri Feb 23 14:54:14 2024, max compression
```

## Comparing `weaviate-client-4.5.4.tar` & `weaviate-client-4.5rc0.tar`

### file list

```diff
@@ -1,409 +1,405 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.264776 weaviate-client-4.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.208777 weaviate-client-4.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.208777 weaviate-client-4.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-16 05:30:47.264776 weaviate-client-4.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.208777 weaviate-client-4.5.4/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-proxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.208777 weaviate-client-4.5.4/ci/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/proxy/envoy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.216777 weaviate-client-4.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    55128 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.220777 weaviate-client-4.5.4/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    18427 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    77448 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26572 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    20956 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.224777 weaviate-client-4.5.4/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.224777 weaviate-client-4.5.4/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.224777 weaviate-client-4.5.4/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-16 05:30:47.264776 weaviate-client-4.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.228777 weaviate-client-4.5.4/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.232776 weaviate-client-4.5.4/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.232776 weaviate-client-4.5.4/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.232776 weaviate-client-4.5.4/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.232776 weaviate-client-4.5.4/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.232776 weaviate-client-4.5.4/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.236776 weaviate-client-4.5.4/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.236776 weaviate-client-4.5.4/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.236776 weaviate-client-4.5.4/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22007 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.236776 weaviate-client-4.5.4/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.240776 weaviate-client-4.5.4/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.240776 weaviate-client-4.5.4/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.240776 weaviate-client-4.5.4/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24333 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.244776 weaviate-client-4.5.4/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    63976 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    36933 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    37851 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.244776 weaviate-client-4.5.4/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26695 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.244776 weaviate-client-4.5.4/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.248777 weaviate-client-4.5.4/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/bm25/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.248777 weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.248777 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.248777 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.248777 weaviate-client-4.5.4/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    25856 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.252776 weaviate-client-4.5.4/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39101 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/gql/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.256776 weaviate-client-4.5.4/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.260776 weaviate-client-4.5.4/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.260776 weaviate-client-4.5.4/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.260776 weaviate-client-4.5.4/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28079 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-03-16 05:30:20.000000 weaviate-client-4.5.4/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:30:47.264776 weaviate-client-4.5.4/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-16 05:30:47.000000 weaviate-client-4.5.4/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-03-16 05:30:47.000000 weaviate-client-4.5.4/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 05:30:47.000000 weaviate-client-4.5.4/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 05:30:46.000000 weaviate-client-4.5.4/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 05:30:47.000000 weaviate-client-4.5.4/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-16 05:30:47.000000 weaviate-client-4.5.4/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.349352 weaviate-client-4.5rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.353352 weaviate-client-4.5rc0/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25941 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20956 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.357352 weaviate-client-4.5rc0/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.357352 weaviate-client-4.5rc0/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32370 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74355 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.377352 weaviate-client-4.5rc0/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.377352 weaviate-client-4.5rc0/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24333 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63226 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30800 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31703 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26191 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22611 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39101 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27997 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate-client-4.5.4/.github/workflows/main.yaml` & `weaviate-client-4.5rc0/.github/workflows/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - README.rst
       - LICENSE.md
       - publishing.md
   pull_request:
 
 env:
   OLD_WEAVIATE_VERSION: 1.23.10
-  NEW_WEAVIATE_VERSION: preview-improved-update-of-target-vector-configs-3688182
+  NEW_WEAVIATE_VERSION: 1.24.0-rc.1
 
 jobs:
   lint-and-format:
     name: Run Linter and Formatter
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
```

### Comparing `weaviate-client-4.5.4/.pre-commit-config.yaml` & `weaviate-client-4.5rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/.pylintrc` & `weaviate-client-4.5rc0/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/CONTRIBUTING.md` & `weaviate-client-4.5rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/LICENSE` & `weaviate-client-4.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/PKG-INFO` & `weaviate-client-4.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.5.4
+Version: 4.5rc0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate-client-4.5.4/README.rst` & `weaviate-client-4.5rc0/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-async.yml` & `weaviate-client-4.5rc0/ci/docker-compose-async.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-azure.yml` & `weaviate-client-4.5rc0/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-cluster.yml` & `weaviate-client-4.5rc0/ci/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-generative.yml` & `weaviate-client-4.5rc0/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-okta-cc.yml` & `weaviate-client-4.5rc0/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-okta-users.yml` & `weaviate-client-4.5rc0/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-proxy.yml` & `weaviate-client-4.5rc0/ci/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 ---
 version: '3.4'
 services:
-  weaviate-proxy:
+  weaviate:
     command:
       - --host
       - 0.0.0.0
       - --port
       - '8080'
       - --scheme
       - http
       - --write-timeout=600s
-    ports:
-      - 8075:8080
     image: semitechnologies/weaviate:${WEAVIATE_VERSION}
+    ports:
+      - "8080:8080"
+      - "50051:50051"
     restart: on-failure:0
     environment:
       CONTEXTIONARY_URL: contextionary:9999
       QUERY_DEFAULTS_LIMIT: 25
       AUTHENTICATION_ANONYMOUS_ACCESS_ENABLED: 'true'
       PERSISTENCE_DATA_PATH: '/var/lib/weaviate'
       DEFAULT_VECTORIZER_MODULE: 'text2vec-contextionary'
-      ENABLE_MODULES: text2vec-contextionary
+      ENABLE_MODULES: text2vec-contextionary,backup-filesystem,img2vec-neural
       BACKUP_FILESYSTEM_PATH: "/tmp/backups"
       CLUSTER_GOSSIP_BIND_PORT: "7100"
       CLUSTER_DATA_BIND_PORT: "7101"
       CLUSTER_HOSTNAME: "node1"
       AUTOSCHEMA_ENABLED: 'false'
+      IMAGE_INFERENCE_API: "http://i2v-neural:8080"
       DISABLE_TELEMETRY: 'true'
   contextionary:
     environment:
       OCCURRENCE_WEIGHT_LINEAR_FACTOR: 0.75
       EXTENSIONS_STORAGE_MODE: weaviate
-      EXTENSIONS_STORAGE_ORIGIN: http://weaviate-proxy:8080
+      EXTENSIONS_STORAGE_ORIGIN: http://weaviate:8080
       NEIGHBOR_OCCURRENCE_IGNORE_PERCENTILE: 5
       ENABLE_COMPOUND_SPLITTING: 'false'
     image: semitechnologies/contextionary:en0.16.0-v1.2.0
     ports:
       - 9999:9999
-  proxy:
-    image: envoyproxy/envoy:v1.29-latest
-    ports:
-      - 10000:10000
-    volumes:
-      - ./proxy:/etc/envoy
+  i2v-neural:
+    image: semitechnologies/img2vec-pytorch:resnet50
 ...
```

### Comparing `weaviate-client-4.5.4/ci/docker-compose-rerank.yml` & `weaviate-client-4.5rc0/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/docker-compose-wcs.yml` & `weaviate-client-4.5rc0/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/ci/start_weaviate.sh` & `weaviate-client-4.5rc0/ci/start_weaviate.sh`

 * *Files 14% similar despite different names*

```diff
@@ -10,8 +10,7 @@
 nohup docker-compose -f ci/docker-compose-azure.yml up -d
 nohup docker-compose -f ci/docker-compose-okta-cc.yml up -d
 nohup docker-compose -f ci/docker-compose-okta-users.yml up -d
 nohup docker-compose -f ci/docker-compose-wcs.yml up -d
 nohup docker-compose -f ci/docker-compose-generative.yml up -d
 nohup docker-compose -f ci/docker-compose-cluster.yml up -d
 nohup docker-compose -f ci/docker-compose-rerank.yml up -d
-nohup docker-compose -f ci/docker-compose-proxy.yml up -d
```

### Comparing `weaviate-client-4.5.4/ci/stop_weaviate.sh` & `weaviate-client-4.5rc0/ci/stop_weaviate.sh`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 docker-compose -f ci/docker-compose-azure.yml down --remove-orphans
 docker-compose -f ci/docker-compose-okta-cc.yml down --remove-orphans
 docker-compose -f ci/docker-compose-okta-users.yml down --remove-orphans
 docker-compose -f ci/docker-compose-wcs.yml down --remove-orphans
 docker-compose -f ci/docker-compose-generative.yml down --remove-orphans
 docker-compose -f ci/docker-compose-cluster.yml down --remove-orphans
 docker-compose -f ci/docker-compose-rerank.yml down --remove-orphans
-docker-compose -f ci/docker-compose-proxy.yml down --remove-orphans
```

### Comparing `weaviate-client-4.5.4/docs/Makefile` & `weaviate-client-4.5rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/README.rst` & `weaviate-client-4.5rc0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/changelog.rst` & `weaviate-client-4.5rc0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,10 @@
 Changelog
 =========
 
-Version 4.5.4
---------------
-This patch version includes:
-
-- Fix parsing of creation/update time from old weaviate versions that write them in ns instead of ms
-- Support ``video_fields`` in ``multi2vec-palm`` which was added in Weaviate 1.24.4:
-
-Version 4.5.3
---------------
-This patch version includes:
-
-- Fix bug with hybrid searches without vector.
-- Support for new modules in Weaviate 1.24.2:
-  - ``text2vec-voyageai``
-  - ``generative-mistral``
-  - Support new parameters for interference URLs in ``text2vec-transformers`` and ``multi2vec-clip``
-- Support for new modules in Weaviate 1.24.3:
-  - ``multi2vec-palm``
-
-Version 4.5.2
---------------
-This patch version includes:
-
-- Fixes endpoint parameter for ``text2vec-palm``
-- Adds support for GSE and TRIGRAM tokenizers
-
-Version 4.5.1
---------------
-This patch version includes:
-
-- Implements an extension to the filtering syntax allowing to pass lists of filters
-    - ``Filter.all_of([f1, f2]])`` is a shortcut for ``f1 & f2``
-    - ``Filter.any_of([f1, f2]])`` is a shortcut for ``f1 | f2``
-    - Can all be chained and mixed together to create dynamic and complex filters
-- Introduces ``weaviate.classes.init.Timeout`` class allowing to define the timeout used when performing client init checks, in addition to connect and query
-- Fixes a bug when performing ``contains_any/contains_all`` filtering using an empty list
-- Adds the ability to limit the ``top_occurences`` return when performing aggregation queries
-- Allows for defining gRPC proxying of the client and fixes the parsing of ``http`` and ``https`` proxies
-- Allow ``None`` as a query value in BM25 and hybrid queries
-- Fix missing named vectors support in ``data.update`` and ``data.replace``
-- Reimplement support for updating named vector configurations alongside the patched ``1.24.1`` server version
-
-Version 4.5.0
---------------
-This minor version includes:
-
-- Full support for the new named vectors feature available in the Weaviate ``1.24`` release.
-- Bugfixes to passing of Weaviate schema objects as collection configurations in certain edge cases.
-- Support use of Sagemaker when vectorizing with the ``text2vec-aws`` module.
-- Allow creation of collections that use the ``hnsw`` index with the ``bq`` quantizing strategy.
-- Allow specifying ``dimensions`` when vectorizing with the ``text2vec-openai`` module.
-- Python in-memory performance improvements when making queries .
-
 Version 4.4.4
 --------------
 This patch version includes:
 
 - A fix to the validation logic of the ``apiEndpoint`` field of ``GenerativePaLMConfig`` object.
 
 Version 4.4.3
```

### Comparing `weaviate-client-4.5.4/docs/conf.py` & `weaviate-client-4.5rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/index.rst` & `weaviate-client-4.5rc0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/make.bat` & `weaviate-client-4.5rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.classification.rst` & `weaviate-client-4.5rc0/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.aggregations.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.batch.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.classes.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.grpc.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.queries.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.collections.rst` & `weaviate-client-4.5rc0/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.connect.rst` & `weaviate-client-4.5rc0/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.gql.rst` & `weaviate-client-4.5rc0/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.proto.v1.rst` & `weaviate-client-4.5rc0/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/docs/weaviate.rst` & `weaviate-client-4.5rc0/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/1234.3gp` & `weaviate-client-4.5rc0/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/conftest.py` & `weaviate-client-4.5rc0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/constants.py` & `weaviate-client-4.5rc0/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/hobbits.mp4` & `weaviate-client-4.5rc0/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_auth.py` & `weaviate-client-4.5rc0/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_batch_v4.py` & `weaviate-client-4.5rc0/integration/test_batch_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_client.py` & `weaviate-client-4.5rc0/integration/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator, Tuple, Union
+from typing import Generator
 
 import pytest
 from _pytest.fixtures import SubRequest
 
 import weaviate
 from weaviate.collections import Collection
 from weaviate.collections.classes.config import (
@@ -10,19 +10,18 @@
     _CollectionConfig,
     DataType,
     GenerativeSearches,
     Property,
     ReferenceProperty,
     Vectorizers,
 )
+from weaviate.connect.base import _Timeout
 from weaviate.exceptions import WeaviateClosedClientError, WeaviateStartUpError
 import weaviate.classes as wvc
 
-from weaviate.config import Timeout
-
 WCS_HOST = "piblpmmdsiknacjnm1ltla.c1.europe-west3.gcp.weaviate.cloud"
 WCS_URL = f"https://{WCS_HOST}"
 WCS_GRPC_HOST = f"grpc-{WCS_HOST}"
 WCS_CREDS = wvc.init.Auth.api_key("cy4ua772mBlMdfw3YnclqAWzFhQt0RLIN0sl")
 
 
 @pytest.fixture(scope="module")
@@ -428,17 +427,16 @@
 
     col.data.insert(properties={"name": "Name"})
 
     obj = col.query.fetch_objects().objects[0]
     assert obj.properties["name"] == "Name"
 
 
-@pytest.mark.parametrize("timeout", [(1, 2), Timeout(query=1, insert=2, init=1)])
-def test_client_with_extra_options(timeout: Union[Tuple[int, int], Timeout]) -> None:
-    additional_config = wvc.init.AdditionalConfig(timeout=timeout, trust_env=True)
+def test_client_with_extra_options() -> None:
+    additional_config = wvc.init.AdditionalConfig(timeout=(1, 2), trust_env=True)
 
     for client in [
         weaviate.connect_to_wcs(
             cluster_url=WCS_URL, auth_credentials=WCS_CREDS, additional_config=additional_config
         ),
         weaviate.connect_to_local(additional_config=additional_config),
         weaviate.connect_to_custom(
@@ -451,15 +449,15 @@
             auth_credentials=WCS_CREDS,
             additional_config=additional_config,
         ),
         weaviate.connect_to_embedded(
             port=8070, grpc_port=50040, additional_config=additional_config
         ),
     ]:
-        assert client._connection.timeout_config == Timeout(query=1, insert=2, init=1)
+        assert client._connection.timeout_config == _Timeout(1, 2)
 
 
 def test_connect_and_close_to_embedded() -> None:
     # Can't use the default port values as they are already in use by the local instances
     client = weaviate.connect_to_embedded(port=8078, grpc_port=50151, version="1.23.7")
 
     client.connect()
@@ -535,25 +533,7 @@
     ).is_ready()
 
 
 def test_client_is_ready() -> None:
     assert weaviate.connect_to_wcs(
         cluster_url=WCS_URL, auth_credentials=WCS_CREDS, skip_init_checks=True
     ).is_ready()
-
-
-def test_local_proxies() -> None:
-    with weaviate.connect_to_local(
-        additional_config=wvc.init.AdditionalConfig(
-            proxies=wvc.init.Proxies(
-                http="http://localhost:8075",
-                grpc="http://localhost:10000",
-            )
-        )
-    ) as client:
-        client.collections.delete("TestLocalProxies")
-        collection = client.collections.create(
-            "TestLocalProxies",
-            properties=[wvc.config.Property(name="name", data_type=wvc.config.DataType.TEXT)],
-        )
-        collection.data.insert({"name": "Test"})
-        assert collection.query.fetch_objects().objects[0].properties["name"] == "Test"
```

### Comparing `weaviate-client-4.5.4/integration/test_collection.py` & `weaviate-client-4.5rc0/integration/test_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,46 +705,14 @@
         ]
     )
     assert res.has_errors is False
 
     assert len(collection.query.hybrid(query="test", alpha=0, offset=offset).objects) == expected
 
 
-def test_hybrid_alpha(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[Property(name="name", data_type=DataType.TEXT)],
-        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
-            vectorize_collection_name=False
-        ),
-    )
-
-    res = collection.data.insert_many(
-        [
-            {"name": "banana"},
-            {"name": "fruit"},
-            {"name": "car"},
-        ]
-    )
-    assert res.has_errors is False
-
-    hybrid_res = collection.query.hybrid(query="fruit", alpha=0)
-    bm25_res = collection.query.bm25(query="fruit")
-    assert all(
-        bm25_res.objects[i].uuid == hybrid_res.objects[i].uuid
-        for i in range(len(hybrid_res.objects))
-    )
-
-    hybrid_res = collection.query.hybrid(query="fruit", alpha=1)
-    text_res = collection.query.near_text(query="fruit")
-    assert all(
-        text_res.objects[i].uuid == hybrid_res.objects[i].uuid
-        for i in range(len(hybrid_res.objects))
-    )
-
-
 @pytest.mark.parametrize("limit", [1, 2])
 def test_bm25_limit(collection_factory: CollectionFactory, limit: int) -> None:
     collection = collection_factory(
         properties=[Property(name="Name", data_type=DataType.TEXT, tokenization=Tokenization.WORD)],
         vectorizer_config=Configure.Vectorizer.none(),
     )
 
@@ -2077,32 +2045,7 @@
 
     collection.data.insert({"a": "a1"})
     objs = collection.query.fetch_objects(return_properties=["a", "b"]).objects
     assert len(objs) == 1
     assert objs[0].properties["a"] == "a1"
     if "b" in objs[0].properties:  # change this when server version bumps to 1.24.0
         assert objs[0].properties["b"] is None
-
-
-def test_none_query_hybrid_bm25(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[
-            Property(name="text", data_type=DataType.TEXT),
-        ],
-        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
-            vectorize_collection_name=False
-        ),
-    )
-
-    collection.data.insert({"text": "banana"})
-    collection.data.insert({"text": "dog"})
-    collection.data.insert({"text": "different concept"})
-
-    hybrid_objs = collection.query.hybrid(
-        query=None, vector=None, return_metadata=MetadataQuery.full()
-    ).objects
-    assert len(hybrid_objs) == 3
-    assert all(obj.metadata.score is not None and obj.metadata.score == 0.0 for obj in hybrid_objs)
-
-    bm25_objs = collection.query.bm25(query=None, return_metadata=MetadataQuery.full()).objects
-    assert len(bm25_objs) == 3
-    assert all(obj.metadata.score is not None and obj.metadata.score == 0.0 for obj in bm25_objs)
```

### Comparing `weaviate-client-4.5.4/integration/test_collection_aggregate.py` & `weaviate-client-4.5rc0/integration/test_collection_aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,28 +67,15 @@
     collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
     collection.data.insert({"text": "some text"})
     res = collection.aggregate.over_all(return_metrics=[Metrics("text").text(count=True)])
     assert isinstance(res.properties["text"], AggregateText)
     assert res.properties["text"].count == 1
 
 
-def test_aggregation_top_occurence_with_limit(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
-    collection.data.insert({"text": "one"})
-    collection.data.insert({"text": "one"})
-    collection.data.insert({"text": "two"})
-    res = collection.aggregate.over_all(
-        return_metrics=[Metrics("text").text(min_occurrences=1)],
-    )
-    assert isinstance(res.properties["text"], AggregateText)
-    assert len(res.properties["text"].top_occurrences) == 1
-    assert res.properties["text"].top_occurrences[0].count == 2
-
-
-def test_aggregation_groupby_with_limit(collection_factory: CollectionFactory) -> None:
+def test_aggregation_with_limit(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
     collection.data.insert({"text": "one"})
     collection.data.insert({"text": "two"})
     collection.data.insert({"text": "three"})
     res = collection.aggregate.over_all(
         return_metrics=[Metrics("text").text(count=True)],
         group_by=GroupByAggregate(prop="text", limit=2),
```

### Comparing `weaviate-client-4.5.4/integration/test_collection_batch.py` & `weaviate-client-4.5rc0/integration/test_collection_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_batch_delete.py` & `weaviate-client-4.5rc0/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_config.py` & `weaviate-client-4.5rc0/integration/test_collection_config.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_filter.py` & `weaviate-client-4.5rc0/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_geo.py` & `weaviate-client-4.5rc0/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_get.py` & `weaviate-client-4.5rc0/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_model.py` & `weaviate-client-4.5rc0/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_multi_node.py` & `weaviate-client-4.5rc0/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_nested.py` & `weaviate-client-4.5rc0/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_openai.py` & `weaviate-client-4.5rc0/integration/test_collection_openai.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_references.py` & `weaviate-client-4.5rc0/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_collection_rerank.py` & `weaviate-client-4.5rc0/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_gql_raw_v4.py` & `weaviate-client-4.5rc0/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_iterator.py` & `weaviate-client-4.5rc0/integration/test_iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration/test_named_vectors.py` & `weaviate-client-4.5rc0/integration/test_named_vectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from integration.conftest import CollectionFactory, OpenAICollection
 import pytest
 import weaviate.classes as wvc
 
 from weaviate.collections.classes.data import DataObject
 
 from weaviate.collections.classes.config import (
-    PQConfig,
     _VectorIndexConfigFlat,
     Vectorizers,
 )
 
 from weaviate.collections.classes.aggregate import AggregateInteger
 
 from weaviate.exceptions import WeaviateInvalidInputError
@@ -130,85 +129,14 @@
     obj = collection.query.fetch_object_by_id(
         batch_return.uuids[0], include_vector=["title", "bringYourOwn"]
     )
     assert obj.vector["title"] is not None
     assert obj.vector["bringYourOwn"] == [0.5, 0.25, 0.75]
 
 
-def test_update(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory("dummy")
-    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
-        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
-
-    collection = collection_factory(
-        properties=[
-            wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
-            wvc.config.Property(name="content", data_type=wvc.config.DataType.TEXT),
-        ],
-        vectorizer_config=[
-            wvc.config.Configure.NamedVectors.none(name="bringYourOwn"),
-        ],
-    )
-
-    uuid = collection.data.insert(
-        properties={"title": "Hello", "content": "World"},
-        vector={
-            "bringYourOwn": [0.5, 0.25, 0.75],
-        },
-    )
-    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
-        "bringYourOwn"
-    ] == [0.5, 0.25, 0.75]
-    collection.data.update(
-        uuid,
-        vector={
-            "bringYourOwn": [0.375, 0.625, 0.875],
-        },
-    )
-    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
-        "bringYourOwn"
-    ] == [0.375, 0.625, 0.875]
-
-
-def test_replace(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory("dummy")
-    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
-        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
-
-    collection = collection_factory(
-        properties=[
-            wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
-            wvc.config.Property(name="content", data_type=wvc.config.DataType.TEXT),
-        ],
-        vectorizer_config=[
-            wvc.config.Configure.NamedVectors.none(name="bringYourOwn"),
-        ],
-    )
-
-    uuid = collection.data.insert(
-        properties={"title": "Hello", "content": "World"},
-        vector={
-            "bringYourOwn": [0.5, 0.25, 0.75],
-        },
-    )
-    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
-        "bringYourOwn"
-    ] == [0.5, 0.25, 0.75]
-    collection.data.replace(
-        uuid,
-        properties={"title": "Hello", "content": "World"},
-        vector={
-            "bringYourOwn": [0.375, 0.625, 0.875],
-        },
-    )
-    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
-        "bringYourOwn"
-    ] == [0.375, 0.625, 0.875]
-
-
 def test_query(collection_factory: CollectionFactory) -> None:
     collection = collection_factory("dummy")
     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
         pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
     collection = collection_factory(
         properties=[
             wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
@@ -442,61 +370,61 @@
         return_metrics=wvc.aggregate.Metrics("number").integer(),
     )
     assert isinstance(agg.properties["number"], AggregateInteger)
     assert agg.properties["number"].sum_ == 1
     assert agg.properties["number"].minimum == 1
 
 
-def test_update_to_enable_quantizer_on_specific_named_vector(
-    collection_factory: CollectionFactory,
-) -> None:
-    collection = collection_factory("dummy")
-    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
-        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
-    collection = collection_factory(
-        properties=[
-            wvc.config.Property(name="first", data_type=wvc.config.DataType.TEXT),
-            wvc.config.Property(name="second", data_type=wvc.config.DataType.TEXT),
-        ],
-        vectorizer_config=[
-            wvc.config.Configure.NamedVectors.text2vec_contextionary(
-                "first",
-                source_properties=["first"],
-                vectorize_collection_name=False,
-            ),
-            wvc.config.Configure.NamedVectors.text2vec_contextionary(
-                "second",
-                source_properties=["second"],
-                vectorize_collection_name=False,
-            ),
-        ],
-    )
-
-    config = collection.config.get()
-    assert config.vector_config is not None
-    assert config.vector_config["first"].vector_index_config is not None
-    assert config.vector_config["second"].vector_index_config is not None
-    assert config.vector_config["second"].vector_index_config.quantizer is None
-
-    collection.config.update(
-        vectorizer_config=[
-            wvc.config.Reconfigure.NamedVectors.update(
-                name="second",
-                vector_index_config=wvc.config.Reconfigure.VectorIndex.hnsw(
-                    quantizer=wvc.config.Reconfigure.VectorIndex.Quantizer.pq(bit_compression=True)
-                ),
-            )
-        ]
-    )
-    config = collection.config.get()
-    assert config.vector_config is not None
-    assert config.vector_config["first"].vector_index_config is not None
-    assert config.vector_config["second"].vector_index_config is not None
-    assert isinstance(config.vector_config["second"].vector_index_config.quantizer, PQConfig)
-    assert config.vector_config["second"].vector_index_config.quantizer.bit_compression is True
+# def test_update_to_enable_quantizer_on_specific_named_vector(
+#     collection_factory: CollectionFactory,
+# ) -> None:
+#     collection = collection_factory("dummy")
+#     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
+#         pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
+#     collection = collection_factory(
+#         properties=[
+#             wvc.config.Property(name="first", data_type=wvc.config.DataType.TEXT),
+#             wvc.config.Property(name="second", data_type=wvc.config.DataType.TEXT),
+#         ],
+#         vectorizer_config=[
+#             wvc.config.Configure.NamedVectors.text2vec_contextionary(
+#                 "first",
+#                 source_properties=["first"],
+#                 vectorize_collection_name=False,
+#             ),
+#             wvc.config.Configure.NamedVectors.text2vec_contextionary(
+#                 "second",
+#                 source_properties=["second"],
+#                 vectorize_collection_name=False,
+#             ),
+#         ],
+#     )
+
+#     config = collection.config.get()
+#     assert config.vector_config is not None
+#     assert config.vector_config["first"].vector_index_config is not None
+#     assert config.vector_config["second"].vector_index_config is not None
+#     assert config.vector_config["second"].vector_index_config.quantizer is None
+
+#     collection.config.update(
+#         vectorizer_config=[
+#             wvc.config.Reconfigure.NamedVectors.update(
+#                 name="second",
+#                 vector_index_config=wvc.config.Reconfigure.VectorIndex.hnsw(
+#                     quantizer=wvc.config.Reconfigure.VectorIndex.Quantizer.pq(bit_compression=True)
+#                 ),
+#             )
+#         ]
+#     )
+#     config = collection.config.get()
+#     assert config.vector_config is not None
+#     assert config.vector_config["first"].vector_index_config is not None
+#     assert config.vector_config["second"].vector_index_config is not None
+#     assert isinstance(config.vector_config["second"].vector_index_config.quantizer, PQConfig)
+#     assert config.vector_config["second"].vector_index_config.quantizer.bit_compression is True
 
 
 # def test_update_to_change_quantizer_from_pq_to_bq_on_specific_named_vector(
 #     collection_factory: CollectionFactory,
 # ) -> None:
 #     collection = collection_factory("dummy")
 #     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
```

### Comparing `weaviate-client-4.5.4/integration/weaviate-logo.png` & `weaviate-client-4.5rc0/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/people_schema.json` & `weaviate-client-4.5rc0/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_authentication.py` & `weaviate-client-4.5rc0/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_backup.py` & `weaviate-client-4.5rc0/integration_v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_backup_v4.py` & `weaviate-client-4.5rc0/integration_v3/test_backup_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_batch.py` & `weaviate-client-4.5rc0/integration_v3/test_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_classification.py` & `weaviate-client-4.5rc0/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_cluster.py` & `weaviate-client-4.5rc0/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_crud.py` & `weaviate-client-4.5rc0/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_graphql.py` & `weaviate-client-4.5rc0/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_grcp.py` & `weaviate-client-4.5rc0/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_schema.py` & `weaviate-client-4.5rc0/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_stress.py` & `weaviate-client-4.5rc0/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/integration_v3/test_timeout.py` & `weaviate-client-4.5rc0/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/conftest.py` & `weaviate-client-4.5rc0/mock_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_auth.py` & `weaviate-client-4.5rc0/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_automatic_retries.py` & `weaviate-client-4.5rc0/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_batching_manual.py` & `weaviate-client-4.5rc0/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_collection.py` & `weaviate-client-4.5rc0/mock_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_connection.py` & `weaviate-client-4.5rc0/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_exception.py` & `weaviate-client-4.5rc0/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_graphql.py` & `weaviate-client-4.5rc0/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_resend.py` & `weaviate-client-4.5rc0/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/mock_tests/test_schema.py` & `weaviate-client-4.5rc0/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/profiling/constants.py` & `weaviate-client-4.5rc0/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/profiling/test_import_and_query.py` & `weaviate-client-4.5rc0/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/profiling/test_profiling.py` & `weaviate-client-4.5rc0/profiling/test_profiling.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/profiling/test_refs.py` & `weaviate-client-4.5rc0/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/profiling/test_sphere.py` & `weaviate-client-4.5rc0/profiling/test_sphere.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/publishing.md` & `weaviate-client-4.5rc0/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/pyproject.toml` & `weaviate-client-4.5rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/requirements-devel.txt` & `weaviate-client-4.5rc0/requirements-devel.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 setuptools_scm
 Sphinx>=7.0.0
 sphinx-rtd-theme==2.0.0
 autodoc-pydantic==2.0.1
 
 grpcio-tools
 
-pytest==8.1.1
+pytest==8.0.1
 pytest-cov==4.1.0
 pytest-benchmark==4.0.0
 pytest-profiling==1.7.0
-coverage==7.4.4
+coverage==7.4.2
 pytest-xdist==3.5.0
 werkzeug>=2.3.7
 pytest-httpserver>=1.0.8
 
 mypy>=1.5.1<2.0.0
 mypy-extensions==1.0.0
 tomli>=2.0.1<3.0.0
```

### Comparing `weaviate-client-4.5.4/setup.cfg` & `weaviate-client-4.5rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/README.md` & `weaviate-client-4.5rc0/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/batch/test_requests.py` & `weaviate-client-4.5rc0/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/classification/test_classification.py` & `weaviate-client-4.5rc0/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/cluster/test_cluster.py` & `weaviate-client-4.5rc0/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/collection/test_aggregates.py` & `weaviate-client-4.5rc0/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/collection/test_classes.py` & `weaviate-client-4.5rc0/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/collection/test_client.py` & `weaviate-client-4.5rc0/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/collection/test_collection_model.py` & `weaviate-client-4.5rc0/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/collection/test_config.py` & `weaviate-client-4.5rc0/test/collection/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -232,22 +232,22 @@
                 "vectorizeClassName": True,
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_palm(
             project_id="project",
-            api_endpoint="api.google.com",
+            api_endpoint="https://api.google.com",
             model_id="model",
             vectorize_collection_name=False,
         ),
         {
             "text2vec-palm": {
                 "projectId": "project",
-                "apiEndpoint": "api.google.com",
+                "apiEndpoint": "https://api.google.com/",
                 "modelId": "model",
                 "vectorizeClassName": False,
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_transformers(),
@@ -258,37 +258,19 @@
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_transformers(
             pooling_strategy="cls",
             vectorize_collection_name=False,
-            inference_url="https://api.transformers.com",
         ),
         {
             "text2vec-transformers": {
                 "vectorizeClassName": False,
                 "poolingStrategy": "cls",
-                "inferenceUrl": "https://api.transformers.com",
-            }
-        },
-    ),
-    (
-        Configure.Vectorizer.text2vec_voyageai(
-            vectorize_collection_name=False,
-            model="voyage-large-2",
-            truncate=False,
-            base_url="https://voyage.made-up.com",
-        ),
-        {
-            "text2vec-voyageai": {
-                "vectorizeClassName": False,
-                "model": "voyage-large-2",
-                "baseURL": "https://voyage.made-up.com",
-                "truncate": False,
             }
         },
     ),
     (
         Configure.Vectorizer.img2vec_neural(
             image_fields=["test"],
         ),
@@ -308,35 +290,14 @@
                 "imageFields": ["image"],
                 "textFields": ["text"],
                 "vectorizeClassName": True,
             }
         },
     ),
     (
-        Configure.Vectorizer.multi2vec_palm(
-            image_fields=["image"],
-            text_fields=["text"],
-            video_fields=["video"],
-            project_id="project",
-            video_interval_seconds=1,
-            location="us-central1",
-        ),
-        {
-            "multi2vec-palm": {
-                "imageFields": ["image"],
-                "textFields": ["text"],
-                "videoFields": ["video"],
-                "projectId": "project",
-                "location": "us-central1",
-                "videoIntervalSeconds": 1,
-                "vectorizeClassName": True,
-            }
-        },
-    ),
-    (
         Configure.Vectorizer.multi2vec_clip(
             image_fields=[Multi2VecField(name="image")],
             text_fields=[Multi2VecField(name="text")],
         ),
         {
             "multi2vec-clip": {
                 "imageFields": ["image"],
@@ -571,18 +532,14 @@
         {"generative-openai": {}},
     ),
     (
         Configure.Generative.anyscale(),
         {"generative-anyscale": {}},
     ),
     (
-        Configure.Generative.mistral(temperature=0.5, max_tokens=100, model="model"),
-        {"generative-mistral": {"temperature": 0.5, "maxTokens": 100, "model": "model"}},
-    ),
-    (
         Configure.Generative.openai(
             model="gpt-4",
             frequency_penalty=0.5,
             max_tokens=100,
             presence_penalty=0.5,
             temperature=0.5,
             top_p=0.5,
@@ -739,25 +696,25 @@
 ]
 
 
 @pytest.mark.parametrize("reranker_config,expected_mc", TEST_CONFIG_WITH_RERANKER)
 def test_config_with_reranker(
     reranker_config: _RerankerConfigCreate,
     expected_mc: dict,
-) -> None:
+):
     config = _CollectionConfigCreate(name="test", reranker_config=reranker_config)
     assert config._to_dict() == {
         **DEFAULTS,
         "vectorizer": "none",
         "class": "Test",
         "moduleConfig": expected_mc,
     }
 
 
-def test_config_with_properties() -> None:
+def test_config_with_properties():
     config = _CollectionConfigCreate(
         name="test",
         description="test",
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[
             Property(
                 name="text",
@@ -1087,33 +1044,14 @@
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
     (
         [
-            Configure.NamedVectors.text2vec_voyageai(
-                name="test", source_properties=["prop"], truncate=True
-            )
-        ],
-        {
-            "test": {
-                "vectorizer": {
-                    "text2vec-voyageai": {
-                        "properties": ["prop"],
-                        "vectorizeClassName": True,
-                        "truncate": True,
-                    }
-                },
-                "vectorIndexType": "hnsw",
-            }
-        },
-    ),
-    (
-        [
             Configure.NamedVectors.img2vec_neural(
                 name="test",
                 image_fields=["test"],
             )
         ],
         {
             "test": {
@@ -1143,39 +1081,14 @@
                         "vectorizeClassName": True,
                     }
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
-    (
-        [
-            Configure.NamedVectors.multi2vec_palm(
-                name="test",
-                image_fields=["image"],
-                text_fields=["text"],
-                project_id="project",
-                location="us-central1",
-            )
-        ],
-        {
-            "test": {
-                "vectorizer": {
-                    "multi2vec-palm": {
-                        "imageFields": ["image"],
-                        "textFields": ["text"],
-                        "projectId": "project",
-                        "location": "us-central1",
-                        "vectorizeClassName": True,
-                    }
-                },
-                "vectorIndexType": "hnsw",
-            }
-        },
-    ),
     (
         [
             Configure.NamedVectors.multi2vec_bind(
                 name="test",
                 audio_fields=["audio"],
                 depth_fields=["depth"],
                 image_fields=["image"],
```

### Comparing `weaviate-client-4.5.4/test/collection/test_queries.py` & `weaviate-client-4.5rc0/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/connection/test_connection.py` & `weaviate-client-4.5rc0/test/connection/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,15 @@
     @patch("weaviate.connect.base.os")
     def test_get_proxies(self, os_mock):
         """
         Test the `_get_proxies` function.
         """
 
         error_msg = lambda dt: (
-            "If 'proxies' is not None, it must be of type dict, str, or wvc.init.Proxies. "
-            f"Given type: {dt}."
+            "If 'proxies' is not None, it must be of type dict or str. " f"Given type: {dt}."
         )
         with self.assertRaises(TypeError) as error:
             proxies = _get_proxies([], False)
         check_error_message(self, error, error_msg(list))
 
         proxies = _get_proxies({}, False)
         self.assertEqual(proxies, {})
@@ -76,23 +75,23 @@
         proxies = _get_proxies({"test": True}, False)
         self.assertEqual(proxies, {"test": True})
 
         proxies = _get_proxies({"test": True}, True)
         self.assertEqual(proxies, {"test": True})
 
         proxies = _get_proxies("test", True)
-        self.assertEqual(proxies, {"http": "test", "https": "test", "grpc": "test"})
+        self.assertEqual(proxies, {"http": "test", "https": "test"})
 
         os_mock.environ.get.return_value = None
         proxies = _get_proxies(None, True)
         self.assertEqual(proxies, {})
 
         os_mock.environ.get.return_value = "test"
         proxies = _get_proxies(None, True)
-        self.assertEqual(proxies, {"http": "test", "https": "test", "grpc": "test"})
+        self.assertEqual(proxies, {"http": "test", "https": "test"})
 
     def test__get_valid_timeout_config(self):
         """
         Test the `_get_valid_timeout_config` function.
         """
 
         # incalid calls
```

### Comparing `weaviate-client-4.5.4/test/contextionary/test_text2vec_contextionary.py` & `weaviate-client-4.5rc0/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/data/references/test_crud_references.py` & `weaviate-client-4.5rc0/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/data/test_crud_data.py` & `weaviate-client-4.5rc0/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/gql/test_aggregate.py` & `weaviate-client-4.5rc0/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/gql/test_filter.py` & `weaviate-client-4.5rc0/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/gql/test_get.py` & `weaviate-client-4.5rc0/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/gql/test_query.py` & `weaviate-client-4.5rc0/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/schema/properties/test_properties.py` & `weaviate-client-4.5rc0/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/schema/schema_company.json` & `weaviate-client-4.5rc0/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/schema/test_schema.py` & `weaviate-client-4.5rc0/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_auth.py` & `weaviate-client-4.5rc0/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_client.py` & `weaviate-client-4.5rc0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_embedded.py` & `weaviate-client-4.5rc0/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_exceptions.py` & `weaviate-client-4.5rc0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_server_version.py` & `weaviate-client-4.5rc0/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/test_util.py` & `weaviate-client-4.5rc0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/test/util.py` & `weaviate-client-4.5rc0/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/__init__.py` & `weaviate-client-4.5rc0/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/auth.py` & `weaviate-client-4.5rc0/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/backup/backup.py` & `weaviate-client-4.5rc0/weaviate/backup/backup.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/batch/crud_batch.py` & `weaviate-client-4.5rc0/weaviate/batch/crud_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,17 +964,15 @@
             self._objects_throughput_frame.append(
                 len(self._objects_batch) / response.elapsed.total_seconds()
             )
             obj_per_second = sum(self._objects_throughput_frame) / len(
                 self._objects_throughput_frame
             )
 
-            self._recommended_num_objects = max(
-                round(obj_per_second * float(self._creation_time)), 1
-            )
+            self._recommended_num_objects = max(round(obj_per_second * self._creation_time), 1)
 
             res = _decode_json_response_list(response, "batch add objects")
             assert res is not None
             return res
         return []
 
     def create_references(self) -> list:
@@ -1063,15 +1061,15 @@
             self._references_throughput_frame.append(
                 len(self._reference_batch) / response.elapsed.total_seconds()
             )
             ref_per_sec = sum(self._references_throughput_frame) / len(
                 self._references_throughput_frame
             )
 
-            self._recommended_num_references = round(ref_per_sec * float(self._creation_time))
+            self._recommended_num_references = round(ref_per_sec * self._creation_time)
 
             res = _decode_json_response_list(response, "Create references")
             assert res is not None
             return res
         return []
 
     def _flush_in_thread(
@@ -1170,15 +1168,15 @@
             and not self._new_dynamic_batching
         ):
             obj_per_second = (
                 sum(self._objects_throughput_frame) / len(self._objects_throughput_frame) * 0.75
             )
             self._recommended_num_objects = max(
                 min(
-                    round(obj_per_second * float(self._creation_time)),
+                    round(obj_per_second * self._creation_time),
                     self._recommended_num_objects + 250,
                 ),
                 1,
             )
 
         # Create references after all the objects have been created
         reference_future_pool = []
@@ -1208,15 +1206,15 @@
             len(self._references_throughput_frame) != 0
             and self._recommended_num_references is not None
         ):
             ref_per_sec = sum(self._references_throughput_frame) / len(
                 self._references_throughput_frame
             )
             self._recommended_num_references = min(
-                round(ref_per_sec * float(self._creation_time)),
+                round(ref_per_sec * self._creation_time),
                 self._recommended_num_references * 2,
             )
 
         self._future_pool = []
         self._reference_batch_queue = []
         return
 
@@ -1740,19 +1738,19 @@
         return self._creation_time
 
     @creation_time.setter
     def creation_time(self, value: Real) -> None:
         _check_positive_num(value, "creation_time", Real)
         if self._recommended_num_references is not None:
             self._recommended_num_references = round(
-                self._recommended_num_references * float(value) / float(self._creation_time)
+                self._recommended_num_references * value / self._creation_time
             )
         if self._recommended_num_objects is not None:
             self._recommended_num_objects = round(
-                self._recommended_num_objects * float(value) / float(self._creation_time)
+                self._recommended_num_objects * value / self._creation_time
             )
         self._creation_time = value
         if self._batching_type:
             self._auto_create()
 
     @property
     def timeout_retries(self) -> int:
```

### Comparing `weaviate-client-4.5.4/weaviate/batch/requests.py` & `weaviate-client-4.5rc0/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/classes/config.py` & `weaviate-client-4.5rc0/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/classes/query.py` & `weaviate-client-4.5rc0/weaviate/classes/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/classification/classification.py` & `weaviate-client-4.5rc0/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/classification/config_builder.py` & `weaviate-client-4.5rc0/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/client.py` & `weaviate-client-4.5rc0/weaviate/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         )
         config = additional_config or AdditionalConfig()
         self.__skip_init_checks = skip_init_checks
 
         self._connection = ConnectionV4(  # pyright: ignore reportIncompatibleVariableOverride
             connection_params=connection_params,
             auth_client_secret=auth_client_secret,
-            timeout_config=config.timeout,
+            timeout_config=_get_valid_timeout_config(config.timeout),
             additional_headers=additional_headers,
             embedded_db=embedded_db,
             connection_config=config.connection,
             proxies=config.proxies,
             trust_env=config.trust_env,
         )
```

### Comparing `weaviate-client-4.5.4/weaviate/cluster/cluster.py` & `weaviate-client-4.5rc0/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/base.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/near_image.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_image.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/near_object.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_object.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/near_text.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_text.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/near_vector.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_vector.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/aggregations/over_all.py` & `weaviate-client-4.5rc0/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/backups.py` & `weaviate-client-4.5rc0/weaviate/collections/backups.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/base.py` & `weaviate-client-4.5rc0/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/base.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/batch_wrapper.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/client.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/client.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/collection.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     consistency_level=self._consistency_level,
                     verbose=verbose,
                     dry_run=dry_run,
                     tenant=tenant,
                     filters=_FilterToGRPC.convert(filters),
                 ),
                 metadata=metadata,
-                timeout=self._connection.timeout_config.insert,
+                timeout=self._connection.timeout_config.connect,
             )
 
             if verbose:
                 objects: List[DeleteManyObject] = [
                     DeleteManyObject(
                         uuid=_WeaviateUUIDInt(int.from_bytes(obj.uuid, byteorder="big")),
                         successful=obj.successful,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/batch/rest.py` & `weaviate-client-4.5rc0/weaviate/collections/batch/rest.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/aggregate.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,23 +134,21 @@
     property_name: str
     count: bool
 
 
 class _MetricsText(_MetricsBase):
     top_occurrences_count: bool
     top_occurrences_value: bool
-    min_occurrences: Optional[int]
 
     def to_gql(self) -> str:
-        limit = f"(limit: {self.min_occurrences})" if self.min_occurrences is not None else ""
         body = " ".join(
             [
                 "count" if self.count else "",
                 (
-                    "topOccurrences" + limit + " {"
+                    "topOccurrences {"
                     if self.top_occurrences_count or self.top_occurrences_value
                     else ""
                 ),
                 "occurs" if self.top_occurrences_count else "",
                 "value" if self.top_occurrences_value else "",
                 "}" if self.top_occurrences_count or self.top_occurrences_value else "",
             ]
@@ -273,43 +271,39 @@
         self.__property = property_
 
     def text(
         self,
         count: bool = False,
         top_occurrences_count: bool = False,
         top_occurrences_value: bool = False,
-        min_occurrences: Optional[int] = None,
     ) -> _MetricsText:
         """Define the metrics to be returned for a TEXT or TEXT_ARRAY property when aggregating over a collection.
 
         If none of the arguments are provided then all metrics will be returned.
 
         Arguments:
             `count`
                 Whether to include the number of objects that contain this property.
             `top_occurrences_count`
                 Whether to include the number of the top occurrences of a property's value.
             `top_occurrences_value`
                 Whether to include the value of the top occurrences of a property's value.
-            `min_occurrences`
-                Only include entries with more occurrences than the given limit.
 
         Returns:
             A `_MetricsStr` object that includes the metrics to be returned.
         """
         if not any([count, top_occurrences_count, top_occurrences_value]):
             count = True
             top_occurrences_count = True
             top_occurrences_value = True
         return _MetricsText(
             property_name=self.__property,
             count=count,
             top_occurrences_count=top_occurrences_count,
             top_occurrences_value=top_occurrences_value,
-            min_occurrences=min_occurrences,
         )
 
     def integer(
         self,
         count: bool = False,
         maximum: bool = False,
         mean: bool = False,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/batch.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/cluster.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,26 +124,20 @@
             Tokenize by word.
         `WHITESPACE`
             Tokenize by whitespace.
         `LOWERCASE`
             Tokenize by lowercase.
         `FIELD`
             Tokenize by field.
-        `GSE`
-            Tokenize using GSE (for Chinese and Japanese).
-        `TRIGRAM`
-            Tokenize into trigrams.
     """
 
     WORD = "word"
     WHITESPACE = "whitespace"
     LOWERCASE = "lowercase"
     FIELD = "field"
-    GSE = "gse"
-    TRIGRAM = "trigram"
 
 
 class GenerativeSearches(str, Enum):
     """The available generative search modules in Weaviate.
 
     These modules generate text from text-based inputs.
     See the [docs](https://weaviate.io/developers/weaviate/modules/reader-generator-modules) for more details.
@@ -160,15 +154,14 @@
     """
 
     OPENAI = "generative-openai"
     COHERE = "generative-cohere"
     PALM = "generative-palm"
     AWS = "generative-aws"
     ANYSCALE = "generative-anyscale"
-    MISTRAL = "generative-mistral"
 
 
 class Rerankers(str, Enum):
     """The available reranker modules in Weaviate.
 
     These modules rerank the results of a search query.
     See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules#re-ranking) for more details.
@@ -364,23 +357,14 @@
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.ANYSCALE, frozen=True, exclude=True
     )
     temperature: Optional[float]
     model: Optional[str]
 
 
-class _GenerativeMistral(_GenerativeConfigCreate):
-    generative: GenerativeSearches = Field(
-        default=GenerativeSearches.MISTRAL, frozen=True, exclude=True
-    )
-    temperature: Optional[float]
-    model: Optional[str]
-    maxTokens: Optional[int]
-
-
 class _GenerativeOpenAIConfigBase(_GenerativeConfigCreate):
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.OPENAI, frozen=True, exclude=True
     )
     baseURL: Optional[AnyHttpUrl]
     frequencyPenaltyProperty: Optional[float]
     presencePenaltyProperty: Optional[float]
@@ -471,22 +455,14 @@
     def anyscale(
         model: Optional[str] = None,
         temperature: Optional[float] = None,
     ) -> _GenerativeConfigCreate:
         return _GenerativeAnyscale(model=model, temperature=temperature)
 
     @staticmethod
-    def mistral(
-        model: Optional[str] = None,
-        temperature: Optional[float] = None,
-        max_tokens: Optional[int] = None,
-    ) -> _GenerativeConfigCreate:
-        return _GenerativeMistral(model=model, temperature=temperature, maxTokens=max_tokens)
-
-    @staticmethod
     def openai(
         model: Optional[str] = None,
         frequency_penalty: Optional[float] = None,
         max_tokens: Optional[int] = None,
         presence_penalty: Optional[float] = None,
         temperature: Optional[float] = None,
         top_p: Optional[float] = None,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config_base.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config_methods.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config_methods.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config_named_vectors.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config_named_vectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 from typing import Any, Dict, List, Literal, Optional, Union
-
 from pydantic import AnyHttpUrl, Field
-
 from weaviate.collections.classes.config_base import (
     _ConfigCreateModel,
     _ConfigUpdateModel,
 )
-from weaviate.collections.classes.config_vector_index import (
-    _VectorIndexConfigCreate,
-    _VectorIndexConfigHNSWUpdate,
-    _VectorIndexConfigFlatUpdate,
-    _VectorIndexConfigUpdate,
-    VectorIndexType,
-)
 from weaviate.collections.classes.config_vectorizers import (
     _Img2VecNeuralConfigCreate,
     _Multi2VecBindConfigCreate,
     _Multi2VecClipConfigCreate,
-    _Multi2VecPalmConfig,
     _Ref2VecCentroidConfigCreate,
     _Text2VecAWSConfigCreate,
     _Text2VecAzureOpenAIConfigCreate,
     _Text2VecCohereConfigCreate,
     _Text2VecContextionaryConfigCreate,
     _Text2VecGPT4AllConfigCreate,
     _Text2VecHuggingFaceConfigCreate,
     _Text2VecJinaConfigCreate,
     _Text2VecOpenAIConfigCreate,
     _Text2VecPalmConfigCreate,
     _Text2VecTransformersConfigCreate,
-    _Text2VecVoyageConfigCreate,
     _VectorizerConfigCreate,
     AWSModel,
     AWSService,
     CohereModel,
     CohereTruncation,
     JinaModel,
     Multi2VecField,
     OpenAIModel,
     OpenAIType,
     Vectorizers,
-    VoyageModel,
     _map_multi2vec_fields,
 )
+from weaviate.collections.classes.config_vector_index import (
+    _VectorIndexConfigCreate,
+    _VectorIndexConfigHNSWUpdate,
+    _VectorIndexConfigFlatUpdate,
+    _VectorIndexConfigUpdate,
+    VectorIndexType,
+)
 
 
 class _NamedVectorizerConfigCreate(_ConfigCreateModel):
     vectorizer: Vectorizers
     properties: Optional[List[str]] = Field(default=None, min_length=1, alias="source_properties")
 
     def _to_dict(self) -> Dict[str, Any]:
@@ -318,105 +313,39 @@
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def multi2vec_clip(
         name: str,
         *,
-        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
-        vectorize_collection_name: bool = True,
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        interference_url: Optional[str] = None,
-    ) -> _NamedVectorConfigCreate:
-        """Create a named vector using the `multi2vec_clip` model.
-
-        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
-        for detailed usage.
-
-        Arguments:
-            `name`
-                The name of the named vector.
-            `vector_index_config`
-                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
-            `vectorize_collection_name`
-                Whether to vectorize the collection name. Defaults to `True`.
-            `image_fields`
-                The image fields to use in vectorization.
-            `text_fields`
-                The text fields to use in vectorization.
-            `inference_url`
-                The inference url to use where API requests should go. Defaults to `None`, which uses the server-defined default.
-        """
-        return _NamedVectorConfigCreate(
-            name=name,
-            vectorizer=_Multi2VecClipConfigCreate(
-                imageFields=_map_multi2vec_fields(image_fields),
-                textFields=_map_multi2vec_fields(text_fields),
-                vectorizeClassName=vectorize_collection_name,
-                inferenceUrl=interference_url,
-            ),
-            vector_index_config=vector_index_config,
-        )
-
-    @staticmethod
-    def multi2vec_palm(
-        name: str,
-        *,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
-        location: str,
-        project_id: str,
-        image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        video_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        dimensions: Optional[int] = None,
-        video_interval_seconds: Optional[int] = None,
-        model_id: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `multi2vec_clip` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
-            `location`
-                Where the model runs. REQUIRED.
-            `project_id`
-                The project ID to use, REQUIRED.
-            `image_fields`
-                The image fields to use in vectorization.
-            `text_fields`
-                The text fields to use in vectorization.
-            `video_fields`
-                The video fields to use in vectorization.
-            `dimensions`
-                The number of dimensions to use. Defaults to `None`, which uses the server-defined default.
-            `video_interval_seconds`
-                Length of a video interval. Defaults to `None`, which uses the server-defined default.
-            `model_id`
-                The model ID to use. Defaults to `None`, which uses the server-defined default.
         """
         return _NamedVectorConfigCreate(
             name=name,
-            vectorizer=_Multi2VecPalmConfig(
-                projectId=project_id,
-                location=location,
+            vectorizer=_Multi2VecClipConfigCreate(
                 imageFields=_map_multi2vec_fields(image_fields),
                 textFields=_map_multi2vec_fields(text_fields),
-                videoFields=_map_multi2vec_fields(video_fields),
-                dimensions=dimensions,
-                modelId=model_id,
-                videoIntervalSeconds=video_interval_seconds,
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def multi2vec_bind(
@@ -436,14 +365,16 @@
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _NamedVectorConfigCreate(
             name=name,
@@ -472,16 +403,16 @@
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
-            `reference_properties`
-                The reference properties to use in vectorization, REQUIRED.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _NamedVectorConfigCreate(
             name=name,
@@ -631,15 +562,15 @@
     def text2vec_palm(
         name: str,
         project_id: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
-        api_endpoint: Optional[str] = None,
+        api_endpoint: Optional[AnyHttpUrl] = None,
         model_id: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `text2vec_palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
@@ -653,15 +584,15 @@
             `source_properties`
                 Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
             `api_endpoint`
-                The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
+                The API endpoint to use. Defaults to `None`, which uses the server-defined default.
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
         """
         return _NamedVectorConfigCreate(
@@ -680,17 +611,14 @@
     def text2vec_transformers(
         name: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
         pooling_strategy: Literal["masked_mean", "cls"] = "masked_mean",
-        inference_url: Optional[str] = None,
-        passage_inference_url: Optional[str] = None,
-        query_inference_url: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `text2vec_transformers` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-transformers)
         for detailed usage.
 
         Arguments:
@@ -700,30 +628,21 @@
                 Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
             `pooling_strategy`
                 The pooling strategy to use. Defaults to `masked_mean`.
-            `inference_url`
-                The inferenceUrl to use where API requests should go. You can use either this OR passage/query_inference_url. Defaults to `None`, which uses the server-defined default.
-            `passage_inference_url`
-                The inferenceUrl to use where passage API requests should go. You can use either this and query_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
-            `query_inference_url`
-                The inferenceUrl to use where query API requests should go. You can use either this and passage_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
         """
         return _NamedVectorConfigCreate(
             name=name,
             source_properties=source_properties,
             vectorizer=_Text2VecTransformersConfigCreate(
                 poolingStrategy=pooling_strategy,
                 vectorizeClassName=vectorize_collection_name,
-                inferenceUrl=inference_url,
-                passageInferenceUrl=passage_inference_url,
-                queryInferenceUrl=query_inference_url,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def text2vec_jinaai(
         name: str,
@@ -758,60 +677,14 @@
             vectorizer=_Text2VecJinaConfigCreate(
                 model=model,
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
-    @staticmethod
-    def text2vec_voyageai(
-        name: str,
-        *,
-        source_properties: Optional[List[str]] = None,
-        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
-        vectorize_collection_name: bool = True,
-        model: Optional[Union[VoyageModel, str]] = None,
-        base_url: Optional[str] = None,
-        truncate: Optional[bool] = None,
-    ) -> _NamedVectorConfigCreate:
-        """Create a named vector using the `text2vec-jinaai` model.
-
-        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-jinaai)
-        for detailed usage.
-
-        Arguments:
-            `name`
-                The name of the named vector.
-            `source_properties`
-                Which properties should be included when vectorizing. By default all text properties are included.
-            `vector_index_config`
-                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
-            `vectorize_collection_name`
-                Whether to vectorize the collection name. Defaults to `True`.
-            `model`
-                The model to use. Defaults to `None`, which uses the server-defined default.
-                See the
-                [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai#available-models) for more details.
-            `base_url`
-                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
-            `truncate`
-                Whether to truncate the input texts to fit within the context length. Defaults to `None`, which uses the server-defined default.
-        """
-        return _NamedVectorConfigCreate(
-            name=name,
-            source_properties=source_properties,
-            vectorizer=_Text2VecVoyageConfigCreate(
-                model=model,
-                vectorizeClassName=vectorize_collection_name,
-                baseURL=base_url,
-                truncate=truncate,
-            ),
-            vector_index_config=vector_index_config,
-        )
-
 
 class _NamedVectorsUpdate:
     @staticmethod
     def update(
         name: str,
         *,
         vector_index_config: Union[_VectorIndexConfigHNSWUpdate, _VectorIndexConfigFlatUpdate],
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config_vector_index.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config_vector_index.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/config_vectorizers.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/config_vectorizers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Union, cast
+from typing_extensions import TypeAlias
 
 from pydantic import AnyHttpUrl, BaseModel, Field, field_validator
-from typing_extensions import TypeAlias
 
 from weaviate.collections.classes.config_base import _ConfigCreateModel
 
+
 CohereModel: TypeAlias = Literal[
     "embed-multilingual-v2.0",
     "embed-multilingual-v3.0",
     "embed-multilingual-light-v3.0",
     "small",
     "medium",
     "large",
@@ -20,15 +21,14 @@
     "embed-english-light-v3.0",
 ]
 CohereTruncation: TypeAlias = Literal["NONE", "START", "END", "LEFT", "RIGHT"]
 OpenAIModel: TypeAlias = Literal[
     "text-embedding-3-small", "text-embedding-3-large", "text-embedding-ada-002"
 ]
 JinaModel: TypeAlias = Literal["jina-embeddings-v2-base-en", "jina-embeddings-v2-small-en"]
-VoyageModel: TypeAlias = Literal["voyage-large-2, voyage-code-2, voyage-2"]
 AWSModel: TypeAlias = Literal[
     "amazon.titan-embed-text-v1",
     "cohere.embed-english-v3",
     "cohere.embed-multilingual-v3",
 ]
 AWSService: TypeAlias = Literal[
     "bedrock",
@@ -59,22 +59,18 @@
             Weaviate module backed by OpenAI and Azure-OpenAI text-based embedding models.
         `TEXT2VEC_PALM`
             Weaviate module backed by PaLM text-based embedding models.
         `TEXT2VEC_TRANSFORMERS`
             Weaviate module backed by Transformers text-based embedding models.
         `TEXT2VEC_JINAAI`
             Weaviate module backed by Jina AI text-based embedding models.
-        `TEXT2VEC_VOYAGEAI`
-            Weaviate module backed by Voyage AI text-based embedding models.
         `IMG2VEC_NEURAL`
             Weaviate module backed by a ResNet-50 neural network for images.
         `MULTI2VEC_CLIP`
             Weaviate module backed by a Sentence-BERT CLIP model for images and text.
-        `MULTI2VEC_PALM`
-            Weaviate module backed by a palm model for images and text.
         `MULTI2VEC_BIND`
             Weaviate module backed by the ImageBind model for images, text, audio, depth, IMU, thermal, and video.
         `REF2VEC_CENTROID`
             Weaviate module backed by a centroid-based model that calculates an object's vectors from its referenced vectors.
     """
 
     NONE = "none"
@@ -83,19 +79,17 @@
     TEXT2VEC_CONTEXTIONARY = "text2vec-contextionary"
     TEXT2VEC_GPT4ALL = "text2vec-gpt4all"
     TEXT2VEC_HUGGINGFACE = "text2vec-huggingface"
     TEXT2VEC_OPENAI = "text2vec-openai"
     TEXT2VEC_PALM = "text2vec-palm"
     TEXT2VEC_TRANSFORMERS = "text2vec-transformers"
     TEXT2VEC_JINAAI = "text2vec-jinaai"
-    TEXT2VEC_VOYAGEAI = "text2vec-voyageai"
     IMG2VEC_NEURAL = "img2vec-neural"
     MULTI2VEC_CLIP = "multi2vec-clip"
     MULTI2VEC_BIND = "multi2vec-bind"
-    MULTI2VEC_PALM = "multi2vec-palm"
     REF2VEC_CENTROID = "ref2vec-centroid"
 
 
 class VectorDistances(str, Enum):
     """Vector similarity distance metric to be used in the `VectorIndexConfig` class.
 
     To ensure optimal search results, we recommend reviewing whether your model provider advises a
@@ -248,32 +242,35 @@
 class _Text2VecCohereConfigCreate(_Text2VecCohereConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecPalmConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_PALM, frozen=True, exclude=True)
     projectId: str
-    apiEndpoint: Optional[str]
+    apiEndpoint: Optional[AnyHttpUrl]
     modelId: Optional[str]
     vectorizeClassName: bool
 
+    def _to_dict(self) -> Dict[str, Any]:
+        ret_dict = super()._to_dict()
+        if self.apiEndpoint is not None:
+            ret_dict["apiEndpoint"] = self.apiEndpoint.unicode_string()
+        return ret_dict
+
 
 class _Text2VecPalmConfigCreate(_Text2VecPalmConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecTransformersConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(
         default=Vectorizers.TEXT2VEC_TRANSFORMERS, frozen=True, exclude=True
     )
     poolingStrategy: Literal["masked_mean", "cls"]
     vectorizeClassName: bool
-    inferenceUrl: Optional[str]
-    passageInferenceUrl: Optional[str]
-    queryInferenceUrl: Optional[str]
 
 
 class _Text2VecTransformersConfigCreate(_Text2VecTransformersConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecGPT4AllConfig(_ConfigCreateModel):
@@ -291,28 +288,14 @@
     vectorizeClassName: bool
 
 
 class _Text2VecJinaConfigCreate(_Text2VecJinaConfig, _VectorizerConfigCreate):
     pass
 
 
-class _Text2VecVoyageConfig(_ConfigCreateModel):
-    vectorizer: Vectorizers = Field(
-        default=Vectorizers.TEXT2VEC_VOYAGEAI, frozen=True, exclude=True
-    )
-    model: Optional[str]
-    baseURL: Optional[str]
-    truncate: Optional[bool]
-    vectorizeClassName: bool
-
-
-class _Text2VecVoyageConfigCreate(_Text2VecVoyageConfig, _VectorizerConfigCreate):
-    pass
-
-
 class _Img2VecNeuralConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.IMG2VEC_NEURAL, frozen=True, exclude=True)
     imageFields: List[str]
 
 
 class _Img2VecNeuralConfigCreate(_Img2VecNeuralConfig, _VectorizerConfigCreate):
     pass
@@ -344,32 +327,20 @@
         if len(ret_dict["weights"]) == 0:
             del ret_dict["weights"]
         return ret_dict
 
 
 class _Multi2VecClipConfig(_Multi2VecBase):
     vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_CLIP, frozen=True, exclude=True)
-    inferenceUrl: Optional[str]
 
 
 class _Multi2VecClipConfigCreate(_Multi2VecClipConfig, _VectorizerConfigCreate):
     pass
 
 
-class _Multi2VecPalmConfig(_Multi2VecBase, _VectorizerConfigCreate):
-    vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_PALM, frozen=True, exclude=True)
-    videoFields: Optional[List[Multi2VecField]]
-    projectId: str
-    location: Optional[str]
-    modelId: Optional[str]
-    dimensions: Optional[int]
-    videoIntervalSeconds: Optional[int]
-    vectorizeClassName: bool
-
-
 class _Multi2VecBindConfig(_Multi2VecBase):
     vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_BIND, frozen=True, exclude=True)
     audioFields: Optional[List[Multi2VecField]]
     depthFields: Optional[List[Multi2VecField]]
     IMUFields: Optional[List[Multi2VecField]]
     thermalFields: Optional[List[Multi2VecField]]
     videoFields: Optional[List[Multi2VecField]]
@@ -428,40 +399,36 @@
         """
         return _Img2VecNeuralConfigCreate(imageFields=image_fields)
 
     @staticmethod
     def multi2vec_clip(
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        interference_url: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
         """Create a `_Multi2VecClipConfigCreate` object for use when vectorizing using the `multi2vec-clip` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-clip)
         for detailed usage.
 
         Arguments:
             `image_fields`
                 The image fields to use in vectorization.
             `text_fields`
                 The text fields to use in vectorization.
-            `inference_url`
-                The inference url to use where API requests should go. Defaults to `None`, which uses the server-defined default.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
 
         Raises:
             `pydantic.ValidationError` if `image_fields` or `text_fields` are not `None` or a `list`.
         """
         return _Multi2VecClipConfigCreate(
             imageFields=_map_multi2vec_fields(image_fields),
             textFields=_map_multi2vec_fields(text_fields),
             vectorizeClassName=vectorize_collection_name,
-            inferenceUrl=interference_url,
         )
 
     @staticmethod
     def multi2vec_bind(
         audio_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         depth_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
@@ -752,28 +719,28 @@
             vectorizeClassName=vectorize_collection_name,
             dimensions=dimensions,
         )
 
     @staticmethod
     def text2vec_palm(
         project_id: str,
-        api_endpoint: Optional[str] = None,
+        api_endpoint: Optional[AnyHttpUrl] = None,
         model_id: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
         """Create a `_Text2VecPalmConfigCreate` object for use when vectorizing using the `text2vec-palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
         Arguments:
             `project_id`
                 The project ID to use, REQUIRED.
             `api_endpoint`
-                The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
+                The API endpoint to use. Defaults to `None`, which uses the server-defined default.
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
@@ -782,100 +749,35 @@
             projectId=project_id,
             apiEndpoint=api_endpoint,
             modelId=model_id,
             vectorizeClassName=vectorize_collection_name,
         )
 
     @staticmethod
-    def multi2vec_palm(
-        *,
-        location: str,
-        project_id: str,
-        image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        video_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
-        dimensions: Optional[int] = None,
-        model_id: Optional[str] = None,
-        video_interval_seconds: Optional[int] = None,
-        vectorize_collection_name: bool = True,
-    ) -> _VectorizerConfigCreate:
-        """Create a `_Multi2VecPalmConfig` object for use when vectorizing using the `text2vec-palm` model.
-
-        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
-        for detailed usage.
-
-        Arguments:
-            `location`
-                Where the model runs. REQUIRED.
-            `project_id`
-                The project ID to use, REQUIRED.
-            `image_fields`
-                The image fields to use in vectorization.
-            `text_fields`
-                The text fields to use in vectorization.
-            `video_fields`
-                The video fields to use in vectorization.
-            `dimensions`
-                The number of dimensions to use. Defaults to `None`, which uses the server-defined default.
-            `model_id`
-                The model ID to use. Defaults to `None`, which uses the server-defined default.
-            `video_interval_seconds`
-                Length of a video interval. Defaults to `None`, which uses the server-defined default.
-            `vectorize_collection_name`
-                Whether to vectorize the collection name. Defaults to `True`.
-
-        Raises:
-            `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
-        """
-        return _Multi2VecPalmConfig(
-            projectId=project_id,
-            location=location,
-            imageFields=_map_multi2vec_fields(image_fields),
-            textFields=_map_multi2vec_fields(text_fields),
-            videoFields=_map_multi2vec_fields(video_fields),
-            dimensions=dimensions,
-            modelId=model_id,
-            videoIntervalSeconds=video_interval_seconds,
-            vectorizeClassName=vectorize_collection_name,
-        )
-
-    @staticmethod
     def text2vec_transformers(
         pooling_strategy: Literal["masked_mean", "cls"] = "masked_mean",
         vectorize_collection_name: bool = True,
-        inference_url: Optional[str] = None,
-        passage_inference_url: Optional[str] = None,
-        query_inference_url: Optional[str] = None,
     ) -> _VectorizerConfigCreate:
         """Create a `_Text2VecTransformersConfigCreate` object for use when vectorizing using the `text2vec-transformers` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-transformers)
         for detailed usage.
 
         Arguments:
             `pooling_strategy`
                 The pooling strategy to use. Defaults to `masked_mean`.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
-            `inference_url`
-                The inference url to use where API requests should go. You can use either this OR passage/query_inference_url. Defaults to `None`, which uses the server-defined default.
-            `passage_inference_url`
-                The inference url to use where passage API requests should go. You can use either this and query_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
-            `query_inference_url`
-                The inference url to use where query API requests should go. You can use either this and passage_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
 
         Raises:
             `pydantic.ValidationError` if `pooling_strategy` is not a valid value from the `PoolingStrategy` type.
         """
         return _Text2VecTransformersConfigCreate(
             poolingStrategy=pooling_strategy,
             vectorizeClassName=vectorize_collection_name,
-            inferenceUrl=inference_url,
-            passageInferenceUrl=passage_inference_url,
-            queryInferenceUrl=query_inference_url,
         )
 
     @staticmethod
     def text2vec_jinaai(
         model: Optional[Union[JinaModel, str]] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
@@ -889,39 +791,7 @@
                 The model to use. Defaults to `None`, which uses the server-defined default.
                 See the
                 [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-jinaai#available-models) for more details.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _Text2VecJinaConfigCreate(model=model, vectorizeClassName=vectorize_collection_name)
-
-    @staticmethod
-    def text2vec_voyageai(
-        *,
-        model: Optional[Union[VoyageModel, str]] = None,
-        base_url: Optional[str] = None,
-        truncate: Optional[bool] = None,
-        vectorize_collection_name: bool = True,
-    ) -> _VectorizerConfigCreate:
-        """Create a `_Text2VecVoyageConfigCreate` object for use when vectorizing using the `text2vec-voyageai` model.
-
-        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai)
-        for detailed usage.
-
-        Arguments:
-            `model`
-                The model to use. Defaults to `None`, which uses the server-defined default.
-                See the
-                [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai#available-models) for more details.
-            `base_url`
-                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
-            `truncate`
-                Whether to truncate the input texts to fit within the context length. Defaults to `None`, which uses the server-defined default.
-            `vectorize_collection_name`
-                Whether to vectorize the collection name. Defaults to `True`.
-        """
-        return _Text2VecVoyageConfigCreate(
-            model=model,
-            baseURL=base_url,
-            truncate=truncate,
-            vectorizeClassName=vectorize_collection_name,
-        )
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/data.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/filters.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 
 from weaviate.collections.classes.types import _WeaviateInput
 from weaviate.types import UUID
 from weaviate.proto.v1 import base_pb2
 from weaviate.util import get_valid_uuid
 
-from weaviate.exceptions import WeaviateInvalidInputError
-
 
 class _Operator(str, Enum):
     EQUAL = "Equal"
     NOT_EQUAL = "NotEqual"
     LESS_THAN = "LessThan"
     LESS_THAN_EQUAL = "LessThanEqual"
     GREATER_THAN = "GreaterThan"
@@ -59,34 +57,34 @@
         else:
             assert self == _Operator.OR
             return base_pb2.Filters.OPERATOR_OR
 
 
 class _Filters:
     def __and__(self, other: "_Filters") -> "_FilterAnd":
-        return _FilterAnd([self, other])
+        return _FilterAnd(self, other)
 
     def __or__(self, other: "_Filters") -> "_FilterOr":
-        return _FilterOr([self, other])
+        return _FilterOr(self, other)
 
 
 class _FilterAnd(_Filters):
-    def __init__(self, filters: List[_Filters]):
-        self.filters: List[_Filters] = filters
+    def __init__(self, *args: _Filters):
+        self.filters: List[_Filters] = list(args)
 
     # replace with the following once 3.11 is the minimum version
     #     Operator: weaviate_pb2.Filters.OperatorType = weaviate_pb2.Filters.OperatorAnd
     @property
     def operator(self) -> _Operator:
         return _Operator.AND
 
 
 class _FilterOr(_Filters):
-    def __init__(self, filters: List[_Filters]):
-        self.filters: List[_Filters] = filters
+    def __init__(self, *args: _Filters):
+        self.filters: List[_Filters] = list(args)
 
     # replace with the following once 3.11 is the minimum version
     #     Operator: weaviate_pb2.Filters.OperatorType = weaviate_pb2.Filters.OperatorOr
     @property
     def operator(self) -> _Operator:
         return _Operator.OR
 
@@ -162,27 +160,22 @@
             target=self._target_path(),
             value=val,
             operator=_Operator.IS_NULL,
         )
 
     def contains_any(self, val: FilterValuesList) -> _FilterValue:
         """Filter on whether the property contains any of the given values."""
-        if len(val) == 0:
-            raise WeaviateInvalidInputError("Filter contains_any must have at least one value")
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.CONTAINS_ANY,
         )
 
     def contains_all(self, val: FilterValuesList) -> _FilterValue:
         """Filter on whether the property contains all of the given values."""
-        if len(val) == 0:
-            raise WeaviateInvalidInputError("Filter contains_all must have at least one value")
-
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.CONTAINS_ALL,
         )
 
     def equal(self, val: FilterValues) -> _FilterValue:
@@ -362,16 +355,14 @@
 class _FilterById(_FilterBase):
     def __init__(self, target: Optional[_TargetRefs] = None) -> None:
         self._target = target
         self._property = "_id"
 
     def contains_any(self, uuids: List[UUID]) -> _FilterValue:
         """Filter for objects that has one of the given ID."""
-        if len(uuids) == 0:
-            raise WeaviateInvalidInputError("Filter contains_any must have at least one value")
         return _FilterValue(
             target=self._target_path(),
             value=[get_valid_uuid(val) for val in uuids],
             operator=_Operator.CONTAINS_ANY,
         )
 
     def equal(self, uuid: UUID) -> _FilterValue:
@@ -557,32 +548,14 @@
         return _FilterByUpdateTime(target=None)
 
     @staticmethod
     def by_property(name: str, length: bool = False) -> _FilterByProperty:
         """Define a filter based on a property to be used when querying and deleting from a collection."""
         return _FilterByProperty(prop=name, length=length, target=None)
 
-    @staticmethod
-    def all_of(filters: List[_Filters]) -> _Filters:
-        """Combine all filters in the input list with an AND operator."""
-        if len(filters) == 1:
-            return filters[0]
-        elif len(filters) == 0:
-            raise WeaviateInvalidInputError("Filter.all_of must have at least one filter")
-        return _FilterAnd(filters)
-
-    @staticmethod
-    def any_of(filters: List[_Filters]) -> _Filters:
-        """Combine all filters in the input list with an OR operator."""
-        if len(filters) == 1:
-            return filters[0]
-        elif len(filters) == 0:
-            raise WeaviateInvalidInputError("Filter.any_of must have at least one filter")
-        return _FilterOr(filters)
-
 
 # type aliases for return classes
 FilterByProperty: TypeAlias = _FilterByProperty
 FilterById: TypeAlias = _FilterById
 FilterByCreationTime: TypeAlias = _FilterByCreationTime
 FilterByUpdateTime: TypeAlias = _FilterByUpdateTime
 FilterByRef: TypeAlias = _FilterByRef
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/grpc.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/internal.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/internal.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/orm.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/tenants.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/classes/types.py` & `weaviate-client-4.5rc0/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/cluster.py` & `weaviate-client-4.5rc0/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/collection.py` & `weaviate-client-4.5rc0/weaviate/collections/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/collections.py` & `weaviate-client-4.5rc0/weaviate/collections/collections.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/config.py` & `weaviate-client-4.5rc0/weaviate/collections/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,25 @@
     CollectionConfig,
     CollectionConfigSimple,
     _Property,
     _ReferenceProperty,
     ShardStatus,
     _ShardStatus,
     ShardTypes,
-    _NamedVectorConfigUpdate,
 )
 from weaviate.collections.classes.config_methods import (
     _collection_config_from_json,
     _collection_config_simple_from_json,
 )
 from weaviate.validator import _validate_input, _ValidateArgument
 from weaviate.connect import ConnectionV4
 from weaviate.exceptions import (
     WeaviateInvalidInputError,
 )
 from weaviate.util import _decode_json_response_dict, _decode_json_response_list
-from weaviate.warnings import _Warnings
 
 from weaviate.connect.v4 import _ExpectedStatusCodes
 
 
 class _ConfigBase:
     def __init__(self, connection: ConnectionV4, name: str, tenant: Optional[str]) -> None:
         self.__connection = connection
@@ -89,15 +87,14 @@
         vector_index_config: Optional[
             Union[_VectorIndexConfigHNSWUpdate, _VectorIndexConfigFlatUpdate]
         ] = None,
         vectorizer_config: Optional[
             Union[
                 _VectorIndexConfigHNSWUpdate,
                 _VectorIndexConfigFlatUpdate,
-                List[_NamedVectorConfigUpdate],
             ]
         ] = None,
     ) -> None:
         """Update the configuration for this collection in Weaviate.
 
         Use the `weaviate.classes.Reconfigure` class to generate the necessary configuration objects for this method.
 
@@ -107,32 +104,29 @@
             `inverted_index_config`
                 Configuration for the inverted index. Use `Reconfigure.inverted_index` to generate one.
             `replication_config`
                 Configuration for the replication. Use `Reconfigure.replication` to generate one.
             `vector_index_config` DEPRECATED USE `vectorizer_config` INSTEAD
                 Configuration for the vector index of the default single vector. Use `Reconfigure.vector_index` to generate one.
             `vectorizer_config`
-                Configurations for the vector index (or indices) of your collection.
-                Use `Reconfigure.vector_index` if there is only one vectorizer and `Reconfigure.NamedVectors` if you have many named vectors to generate them.
+                Configuration for the vector index of the default single vector. Use `Reconfigure.vector_index` to generate one.
 
         Raises:
             `weaviate.WeaviateInvalidInputError`:
                 If the input parameters are invalid.
             `weaviate.WeaviateConnectionError`:
                 If the network connection to Weaviate fails.
             `weaviate.UnexpectedStatusCodeError`:
                 If Weaviate reports a non-OK status.
 
         NOTE:
             - If you wish to update a specific option within the configuration and cannot find it in `CollectionConfigUpdate` then it is an immutable option.
             - To change it, you will have to delete the collection and recreate it with the desired options.
             - This is not the case of adding properties, which can be done with `collection.config.add_property()`.
         """
-        if vector_index_config is not None:
-            _Warnings.vector_index_config_in_config_update()
         try:
             config = _CollectionConfigUpdate(
                 description=description,
                 inverted_index_config=inverted_index_config,
                 replication_config=replication_config,
                 vector_index_config=vector_index_config,
                 vectorizer_config=vectorizer_config,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/data.py` & `weaviate-client-4.5rc0/weaviate/collections/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,21 +325,14 @@
             self.name,
             self._consistency_level,
             self._tenant,
             self._validate_arguments,
             data_model,
         )
 
-    def __parse_vector(self, obj: Dict[str, Any], vector: VECTORS) -> Dict[str, Any]:
-        if isinstance(vector, dict):
-            obj["vectors"] = {key: _get_vector_v4(val) for key, val in vector.items()}
-        else:
-            obj["vector"] = _get_vector_v4(vector)
-        return obj
-
     def insert(
         self,
         properties: Properties,
         references: Optional[ReferenceInputs] = None,
         uuid: Optional[UUID] = None,
         vector: Optional[VECTORS] = None,
     ) -> uuid_package.UUID:
@@ -349,17 +342,17 @@
             `properties`
                 The properties of the object, REQUIRED.
             `references`
                 Any references to other objects in Weaviate.
             `uuid`
                 The UUID of the object. If not provided, a random UUID will be generated.
             `vector`
-                The vector(s) of the object.
+                The vector of the object.
                 Supported types are
-                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
+                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor` and `tf.Tensor`, by default None.
                 - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
 
         Returns:
             `uuid.UUID`, the UUID of the inserted object.
 
         Raises:
             `weaviate.exceptions.UnexpectedStatusCodeError`:
@@ -381,16 +374,22 @@
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
             "id": str(uuid if uuid is not None else uuid_package.uuid4()),
         }
+
         if vector is not None:
-            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
+            if isinstance(vector, dict):
+                for key, val in vector.items():
+                    vector[key] = _get_vector_v4(val)
+                weaviate_obj["vectors"] = vector
+            else:
+                weaviate_obj["vector"] = _get_vector_v4(vector)
 
         return self._insert(weaviate_obj)
 
     def insert_many(
         self,
         objects: Sequence[Union[Properties, DataObject[Properties, Optional[ReferenceInputs]]]],
     ) -> BatchObjectReturn:
@@ -429,40 +428,37 @@
                         properties=cast(dict, obj),
                         tenant=self._tenant,
                         references=None,
                     )
                 )
                 for obj in objects
             ],
-            timeout=self._connection.timeout_config.insert,
+            timeout=self._connection.timeout_config.connect,
         )
 
     def replace(
         self,
         uuid: UUID,
         properties: Properties,
         references: Optional[ReferenceInputs] = None,
-        vector: Optional[VECTORS] = None,
+        vector: Optional[Sequence[float]] = None,
     ) -> None:
         """Replace an object in the collection.
 
         This is equivalent to a PUT operation.
 
         Arguments:
             `uuid`
                 The UUID of the object, REQUIRED.
             `properties`
                 The properties of the object, REQUIRED.
             `references`
                 Any references to other objects in Weaviate, REQUIRED.
             `vector`
-                The vector(s) of the object.
-                Supported types are
-                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
-                - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
+                The vector of the object.
 
         Raises:
             `weaviate.WeaviateConnectionError`:
                 If the network connection to Weaviate fails.
             `weaviate.exceptions.WeaviateInvalidInputError`:
                 If any of the arguments are invalid.
             `weaviate.UnexpectedStatusCodeError`:
@@ -474,36 +470,34 @@
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(expected=[Mapping], name="properties", value=properties),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
-                    _ValidateArgument(
-                        expected=[Sequence, None, Mapping], name="vector", value=vector
-                    ),
+                    _ValidateArgument(expected=[Sequence, None], name="vector", value=vector),
                 ]
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
         }
         if vector is not None:
-            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
+            weaviate_obj["vector"] = _get_vector_v4(vector)
 
         self._replace(weaviate_obj, uuid=uuid)
 
     def update(
         self,
         uuid: UUID,
         properties: Optional[Properties] = None,
         references: Optional[ReferenceInputs] = None,
-        vector: Optional[VECTORS] = None,
+        vector: Optional[List[float]] = None,
     ) -> None:
         """Update an object in the collection.
 
         This is equivalent to a PATCH operation.
 
         If the object does not exist yet, it will be created.
 
@@ -511,39 +505,34 @@
             `uuid`
                 The UUID of the object, REQUIRED.
             `properties`
                 The properties of the object.
             `references`
                 Any references to other objects in Weaviate.
             `vector`
-                The vector(s) of the object.
-                Supported types are
-                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
-                - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
+                The vector of the object.
         """
         if self._validate_arguments:
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(
                         expected=[Mapping, None], name="properties", value=properties
                     ),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
-                    _ValidateArgument(
-                        expected=[Sequence, None, Mapping], name="vector", value=vector
-                    ),
+                    _ValidateArgument(expected=[Sequence, None], name="vector", value=vector),
                 ],
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {"class": self.name, "properties": {**props, **refs}}
         if vector is not None:
-            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
+            weaviate_obj["vector"] = _get_vector_v4(vector)
 
         self._update(weaviate_obj, uuid=uuid)
 
     def reference_add(self, from_uuid: UUID, from_property: str, to: SingleReferenceInput) -> None:
         """Create a reference between an object in this collection and any other object in Weaviate.
 
         Arguments:
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/filters.py` & `weaviate-client-4.5rc0/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/grpc/query.py` & `weaviate-client-4.5rc0/weaviate/collections/grpc/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             sort_by=sort_by,
         )
 
         return self.__call(request)
 
     def hybrid(
         self,
-        query: Optional[str],
+        query: str,
         alpha: Optional[float] = None,
         vector: Optional[List[float]] = None,
         properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
@@ -152,47 +152,39 @@
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
-                    _ValidateArgument([None, str], "query", query),
+                    _ValidateArgument([str], "query", query),
                     _ValidateArgument([float, int, None], "alpha", alpha),
                     _ValidateArgument([List, None], "vector", vector),
                     _ValidateArgument([List, None], "properties", properties),
                     _ValidateArgument([HybridFusion, None], "fusion_type", fusion_type),
                     _ValidateArgument([str, None], "target_vector", target_vector),
                 ]
             )
 
-        # Set hybrid search to only query the other search-type if one of the two is not set
-        if query is None:
-            alpha = 1
-
-        hybrid_search = (
-            search_get_pb2.Hybrid(
-                properties=properties,
-                query=query,
-                alpha=float(alpha) if alpha is not None else None,
-                vector_bytes=(
-                    struct.pack("{}f".format(len(vector)), *vector) if vector is not None else None
-                ),
-                fusion_type=(
-                    cast(
-                        search_get_pb2.Hybrid.FusionType,
-                        search_get_pb2.Hybrid.FusionType.Value(fusion_type.value),
-                    )
-                    if fusion_type is not None
-                    else None
-                ),
-                target_vectors=[target_vector] if target_vector is not None else None,
-            )
-            if query is not None or vector is not None
-            else None
+        hybrid_search = search_get_pb2.Hybrid(
+            properties=properties,
+            query=query,
+            alpha=float(alpha) if alpha is not None else None,
+            vector_bytes=(
+                struct.pack("{}f".format(len(vector)), *vector) if vector is not None else None
+            ),
+            fusion_type=(
+                cast(
+                    search_get_pb2.Hybrid.FusionType,
+                    search_get_pb2.Hybrid.FusionType.Value(fusion_type.value),
+                )
+                if fusion_type is not None
+                else None
+            ),
+            target_vectors=[target_vector] if target_vector is not None else None,
         )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
             metadata=return_metadata,
@@ -204,30 +196,30 @@
             hybrid_search=hybrid_search,
         )
 
         return self.__call(request)
 
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
-                    _ValidateArgument([None, str], "query", query),
+                    _ValidateArgument([str], "query", query),
                     _ValidateArgument([List, None], "properties", properties),
                 ]
             )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
@@ -236,17 +228,15 @@
             return_properties=return_properties,
             return_references=return_references,
             generative=generative,
             rerank=rerank,
             autocut=autocut,
             bm25=search_get_pb2.BM25(
                 query=query, properties=properties if properties is not None else []
-            )
-            if query is not None
-            else None,
+            ),
         )
         return self.__call(request)
 
     def near_vector(
         self,
         near_vector: List[float],
         certainty: Optional[NUMBER] = None,
@@ -377,32 +367,28 @@
         certainty, distance = self.__parse_near_options(certainty, distance)
 
         near_text_req = search_get_pb2.NearTextSearch(
             query=near_text,
             certainty=certainty,
             distance=distance,
             target_vectors=[target_vector] if target_vector is not None else None,
-            move_away=(
-                search_get_pb2.NearTextSearch.Move(
-                    force=move_away.force,
-                    concepts=move_away._concepts_list,
-                    uuids=move_away._objects_list,
-                )
-                if move_away is not None
-                else None
-            ),
-            move_to=(
-                search_get_pb2.NearTextSearch.Move(
-                    force=move_to.force,
-                    concepts=move_to._concepts_list,
-                    uuids=move_to._objects_list,
-                )
-                if move_to is not None
-                else None
-            ),
+            move_away=search_get_pb2.NearTextSearch.Move(
+                force=move_away.force,
+                concepts=move_away._concepts_list,
+                uuids=move_away._objects_list,
+            )
+            if move_away is not None
+            else None,
+            move_to=search_get_pb2.NearTextSearch.Move(
+                force=move_to.force,
+                concepts=move_to._concepts_list,
+                uuids=move_to._objects_list,
+            )
+            if move_to is not None
+            else None,
         )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
             metadata=return_metadata,
@@ -605,15 +591,15 @@
     def __call(self, request: search_get_pb2.SearchRequest) -> search_get_pb2.SearchReply:
         try:
             assert self._connection.grpc_stub is not None
             res: search_get_pb2.SearchReply  # According to PEP-0526
             res, _ = self._connection.grpc_stub.Search.with_call(
                 request,
                 metadata=self._connection.grpc_headers(),
-                timeout=self._connection.timeout_config.query,
+                timeout=self._connection.timeout_config.connect,
             )
 
             return res
 
         except grpc.RpcError as e:
             raise WeaviateQueryError(e.details(), "GRPC search")  # pyright: ignore
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/grpc/shared.py` & `weaviate-client-4.5rc0/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/iterator.py` & `weaviate-client-4.5rc0/weaviate/collections/iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/orm.py` & `weaviate-client-4.5rc0/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/base.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,38 +90,32 @@
             self.__connection,
             self._name,
             self.__tenant,
             self.__consistency_level,
             validate_arguments=self._validate_arguments,
         )
 
-    def __retrieve_timestamp(
-        self,
-        timestamp: int,
-    ) -> datetime.datetime:
-        # Handle the case in which last_update_time_unix is in nanoseconds or milliseconds, issue #958
-        if len(str(timestamp)) <= 13:
-            return datetime.datetime.fromtimestamp(timestamp / 1000, tz=datetime.timezone.utc)
-        else:
-            return datetime.datetime.fromtimestamp(timestamp / 1e9, tz=datetime.timezone.utc)
-
     def __extract_metadata_for_object(
         self,
         add_props: "search_get_pb2.MetadataResult",
     ) -> MetadataReturn:
         meta = MetadataReturn(
             distance=add_props.distance if add_props.distance_present else None,
             certainty=add_props.certainty if add_props.certainty_present else None,
             creation_time=(
-                self.__retrieve_timestamp(add_props.creation_time_unix)
+                datetime.datetime.fromtimestamp(
+                    add_props.creation_time_unix / 1000, tz=datetime.timezone.utc
+                )
                 if add_props.creation_time_unix_present
                 else None
             ),
             last_update_time=(
-                self.__retrieve_timestamp(add_props.last_update_time_unix)
+                datetime.datetime.fromtimestamp(
+                    add_props.last_update_time_unix / 1000, tz=datetime.timezone.utc
+                )
                 if add_props.last_update_time_unix_present
                 else None
             ),
             score=add_props.score if add_props.score_present else None,
             explain_score=add_props.explain_score if add_props.explain_score_present else None,
             is_consistent=add_props.is_consistent if add_props.is_consistent_present else None,
             rerank_score=add_props.rerank_score if add_props.rerank_score_present else None,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/bm25/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from weaviate.types import INCLUDE_VECTOR
 
 
 class _BM25Generate(Generic[Properties, References], _BaseQuery[Properties, References]):
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -38,15 +38,15 @@
     ) -> GenerativeReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a keyword-based BM25 search of objects in this collection.
 
         See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
 
         Arguments:
             `query`
-                The keyword-based query to search for, REQUIRED. If None, a normal search will be performed.
+                The keyword-based query to search for, REQUIRED.
             `single_prompt`
                 The prompt to use for RaG on each object individually.
             `grouped_task`
                 The prompt to use for RaG on the entire result set.
             `grouped_properties`
                 The properties to use in the RaG on the entire result set.
             `query_properties`
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/bm25/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import INCLUDE_VECTOR
 
 class _BM25Generate(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -32,15 +32,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -52,15 +52,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -72,15 +72,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -92,15 +92,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -112,15 +112,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/bm25/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import INCLUDE_VECTOR
 
 
 class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -33,15 +33,15 @@
     ) -> QueryReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects in this collection using the keyword-based BM25 algorithm.
 
         See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
 
         Arguments:
             `query`
-                The keyword-based query to search for, REQUIRED. If None, a normal search will be performed.
+                The keyword-based query to search for, REQUIRED.
             `query_properties`
                 The properties to search in. If not specified, all properties are searched.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/bm25/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import INCLUDE_VECTOR
 
 class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -29,15 +29,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -46,15 +46,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -63,15 +63,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -80,15 +80,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
@@ -97,15 +97,15 @@
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
     def bm25(
         self,
-        query: Optional[str],
+        query: str,
         *,
         query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         rerank: Optional[Rerank] = None,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/fetch_objects/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/hybrid/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ) -> GenerativeReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of an object search in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
 
         See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
 
         Arguments:
             `query`
-                The keyword-based query to search for, REQUIRED. If query and vector are both None, a normal search will be performed.
+                The keyword-based query to search for, REQUIRED.
             `single_prompt`
                 The prompt to use for RaG on each object individually.
             `grouped_task`
                 The prompt to use for RaG on the entire result set.
             `grouped_properties`
                 The properties to use in the RaG on the entire result set.
             `alpha`
@@ -88,15 +88,15 @@
             A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the network connection to Weaviate fails.
         """
         res = self._query.hybrid(
-            query=query,
+            query=query or "",
             alpha=alpha,
             vector=vector,
             properties=query_properties,
             fusion_type=fusion_type,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/hybrid/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ) -> QueryReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
 
         See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
 
         Arguments:
             `query`
-                The keyword-based query to search for, REQUIRED. If query and vector are both None, a normal search will be performed.
+                The keyword-based query to search for, REQUIRED.
             `alpha`
                 The weight of the BM25 score. If not specified, the default weight specified by the server is used.
             `vector`
                 The specific vector to search for. If not specified, the query is vectorized and used in the similarity search.
             `query_properties`
                 The properties to search in. If not specified, all properties are searched.
             `fusion_type`
@@ -78,15 +78,15 @@
             A `QueryReturn` object that includes the searched objects.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the network connection to Weaviate fails.
         """
         res = self._query.hybrid(
-            query=query,
+            query=query or "",
             alpha=alpha,
             vector=vector,
             properties=query_properties,
             fusion_type=fusion_type,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
```

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/hybrid/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_image/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_image/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_image/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_image/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_media/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_media/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_media/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_media/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_object/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_object/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_object/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_object/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_text/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_text/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_text/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_text/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_vector/generate.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_vector/query.py` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/queries/near_vector/query.pyi` & `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/query.py` & `weaviate-client-4.5rc0/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/collections/tenants.py` & `weaviate-client-4.5rc0/weaviate/collections/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/connect/authentication.py` & `weaviate-client-4.5rc0/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/connect/base.py` & `weaviate-client-4.5rc0/weaviate/connect/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 import datetime
 import os
 import time
 from abc import ABC, abstractmethod
-from typing import Dict, Literal, Tuple, TypeVar, Union, cast, overload
+from dataclasses import dataclass
+from typing import Literal, Tuple, TypeVar, Union, cast, overload
 from urllib.parse import urlparse
 
 import grpc  # type: ignore
 from grpc import Channel, ssl_channel_credentials
 from grpc.aio import Channel as AsyncChannel  # type: ignore
 
 from pydantic import BaseModel, field_validator, model_validator
 
-from weaviate.config import Proxies
 from weaviate.types import NUMBER
 
 
 JSONPayload = Union[dict, list]
 TIMEOUT_TYPE_RETURN = Tuple[NUMBER, NUMBER]
+PYPI_TIMEOUT = 0.1
 MAX_GRPC_MESSAGE_LENGTH = 104858000  # 10mb, needs to be synchronized with GRPC server
-GRPC_DEFAULT_OPTIONS = [
+GRPC_OPTIONS = [
     ("grpc.max_send_message_length", MAX_GRPC_MESSAGE_LENGTH),
     ("grpc.max_receive_message_length", MAX_GRPC_MESSAGE_LENGTH),
 ]
 
 
+@dataclass
+class _Timeout:
+    connect: int
+    read: int
+
+    @classmethod
+    def from_timeout_config(cls, timeout: TIMEOUT_TYPE_RETURN) -> "_Timeout":
+        return cls(
+            connect=int(timeout[0]),
+            read=int(timeout[1]),
+        )
+
+
 class ProtocolParams(BaseModel):
     host: str
     port: int
     secure: bool
 
     @field_validator("host")
     def _check_host(cls, v: str) -> str:
@@ -106,43 +120,37 @@
         return (self.grpc.host, self.grpc.port)
 
     @property
     def _grpc_target(self) -> str:
         return f"{self.grpc.host}:{self.grpc.port}"
 
     @overload
-    def _grpc_channel(self, async_channel: Literal[False], proxies: Dict[str, str]) -> Channel:
+    def _grpc_channel(self, async_channel: Literal[False]) -> Channel:
         ...
 
     @overload
-    def _grpc_channel(self, async_channel: Literal[True], proxies: Dict[str, str]) -> AsyncChannel:
+    def _grpc_channel(self, async_channel: Literal[True]) -> AsyncChannel:
         ...
 
-    def _grpc_channel(
-        self, async_channel: bool, proxies: Dict[str, str]
-    ) -> Union[Channel, AsyncChannel]:
+    def _grpc_channel(self, async_channel: bool) -> Union[Channel, AsyncChannel]:
         if async_channel:
             import_path = grpc.aio
         else:
             import_path = grpc
 
-        if (p := proxies.get("grpc")) is not None:
-            options: list = [*GRPC_DEFAULT_OPTIONS, ("grpc.http_proxy", p)]
-        else:
-            options = GRPC_DEFAULT_OPTIONS
         if self.grpc.secure:
             return import_path.secure_channel(
                 target=self._grpc_target,
                 credentials=ssl_channel_credentials(),
-                options=options,
+                options=GRPC_OPTIONS,
             )
         else:
             return import_path.insecure_channel(
                 target=self._grpc_target,
-                options=options,
+                options=GRPC_OPTIONS,
             )
 
     @property
     def _http_scheme(self) -> str:
         return "https" if self.http.secure else "http"
 
     @property
@@ -156,15 +164,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def get_proxies(self) -> dict:
         raise NotImplementedError
 
 
-def _get_proxies(proxies: Union[dict, str, Proxies, None], trust_env: bool) -> dict:
+def _get_proxies(proxies: Union[dict, str, None], trust_env: bool) -> dict:
     """
     Get proxies as dict, compatible with 'requests' library.
     NOTE: 'proxies' has priority over 'trust_env', i.e. if 'proxies' is NOT None, 'trust_env'
     is ignored.
 
     Parameters
     ----------
@@ -185,42 +193,36 @@
     """
 
     if proxies is not None:
         if isinstance(proxies, str):
             return {
                 "http": proxies,
                 "https": proxies,
-                "grpc": proxies,
             }
         if isinstance(proxies, dict):
             return proxies
-        if isinstance(proxies, Proxies):
-            return proxies.model_dump(exclude_none=True)
         raise TypeError(
-            "If 'proxies' is not None, it must be of type dict, str, or wvc.init.Proxies. "
+            "If 'proxies' is not None, it must be of type dict or str. "
             f"Given type: {type(proxies)}."
         )
 
     if not trust_env:
         return {}
 
     http_proxy = (os.environ.get("HTTP_PROXY"), os.environ.get("http_proxy"))
     https_proxy = (os.environ.get("HTTPS_PROXY"), os.environ.get("https_proxy"))
-    grpc_proxy = (os.environ.get("GRPC_PROXY"), os.environ.get("grpc_proxy"))
 
-    if not any(http_proxy + https_proxy + grpc_proxy):
+    if not any(http_proxy + https_proxy):
         return {}
 
     proxies = {}
     if any(http_proxy):
         proxies["http"] = http_proxy[0] if http_proxy[0] else http_proxy[1]
     if any(https_proxy):
         proxies["https"] = https_proxy[0] if https_proxy[0] else https_proxy[1]
-    if any(grpc_proxy):
-        proxies["grpc"] = grpc_proxy[0] if grpc_proxy[0] else grpc_proxy[1]
 
     return proxies
 
 
 def _get_epoch_time() -> int:
     """
     Get the current epoch time as an integer.
```

### Comparing `weaviate-client-4.5.4/weaviate/connect/helpers.py` & `weaviate-client-4.5rc0/weaviate/connect/helpers.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/connect/v3.py` & `weaviate-client-4.5rc0/weaviate/connect/v3.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/connect/v4.py` & `weaviate-client-4.5rc0/weaviate/connect/v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,32 +17,35 @@
     ConnectError,
     HTTPError,
     Limits,
     ReadError,
     RemoteProtocolError,
     RequestError,
     Response,
+    Timeout,
     HTTPTransport,
     get,
-    Timeout,
 )
 
 from weaviate import __version__ as client_version
 from weaviate.auth import (
     AuthCredentials,
     AuthApiKey,
     AuthClientCredentials,
 )
-from weaviate.config import ConnectionConfig, Proxies, Timeout as TimeoutConfig
+from weaviate.config import ConnectionConfig
 from weaviate.connect.authentication import _Auth
 from weaviate.connect.base import (
     _ConnectionBase,
     ConnectionParams,
+    _Timeout,
     JSONPayload,
     _get_proxies,
+    PYPI_TIMEOUT,
+    TIMEOUT_TYPE_RETURN,
 )
 from weaviate.embedded import EmbeddedV4
 from weaviate.exceptions import (
     AuthenticationFailedError,
     UnexpectedStatusCodeError,
     WeaviateGRPCUnavailableError,
     WeaviateStartUpError,
@@ -82,16 +85,16 @@
     Connection class used to communicate to a weaviate instance.
     """
 
     def __init__(
         self,
         connection_params: ConnectionParams,
         auth_client_secret: Optional[AuthCredentials],
-        timeout_config: TimeoutConfig,
-        proxies: Union[str, Proxies, None],
+        timeout_config: Tuple[float, float],
+        proxies: Union[dict, str, None],
         trust_env: bool,
         additional_headers: Optional[Dict[str, Any]],
         connection_config: ConnectionConfig,
         embedded_db: Optional[EmbeddedV4] = None,
     ):
         self.url = connection_params._http_url
         self.embedded_db = embedded_db
@@ -101,28 +104,28 @@
         self.__additional_headers = {}
         self._auth = auth_client_secret
         self._connection_params = connection_params
         self._grpc_stub: Optional[weaviate_pb2_grpc.WeaviateStub] = None
         self._grpc_stub_async: Optional[weaviate_pb2_grpc.WeaviateStub] = None
         self._grpc_channel: Optional[Channel] = None
         self._grpc_channel_async: Optional[AsyncChannel] = None
-        self.timeout_config = timeout_config
+        self.timeout_config = _Timeout.from_timeout_config(timeout_config)
         self.__connection_config = connection_config
         self.__trust_env = trust_env
         self._weaviate_version = _ServerVersion.from_string("")
         self.__connected = False
 
         self._headers = {"content-type": "application/json"}
         if additional_headers is not None:
             _validate_input(_ValidateArgument([dict], "additional_headers", additional_headers))
             self.__additional_headers = additional_headers
             for key, value in additional_headers.items():
                 self._headers[key.lower()] = value
 
-        self._proxies: Dict[str, str] = _get_proxies(proxies, trust_env)
+        self._proxies = _get_proxies(proxies, trust_env)
 
         # auth secrets can contain more information than a header (refresh tokens and lifetime) and therefore take
         # precedent over headers
         if "authorization" in self._headers and auth_client_secret is not None:
             _Warnings.auth_header_and_auth_secret()
             self._headers.pop("authorization")
 
@@ -140,15 +143,15 @@
         try:
             self._weaviate_version = _ServerVersion.from_string(self.get_meta()["version"])
         except (WeaviateConnectionError, ReadError, RemoteProtocolError) as e:
             raise WeaviateStartUpError(f"Could not connect to Weaviate:{e}.") from e
 
         if not skip_init_checks:
             try:
-                pkg_info = get(PYPI_PACKAGE_URL, timeout=self.timeout_config.init).json()
+                pkg_info = get(PYPI_PACKAGE_URL, timeout=PYPI_TIMEOUT).json()
                 pkg_info = pkg_info.get("info", {})
                 latest_version = pkg_info.get("version", "unknown version")
                 if is_weaviate_client_too_old(client_version, latest_version):
                     _Warnings.weaviate_client_too_old_vs_latest(client_version, latest_version)
             except RequestError:
                 pass  # ignore any errors related to requests, it is a best-effort warning
 
@@ -163,62 +166,58 @@
     def __make_mounts(self, type_: Literal["async"]) -> Dict[str, AsyncHTTPTransport]:
         ...
 
     def __make_mounts(
         self, type_: Literal["sync", "async"]
     ) -> Union[Dict[str, HTTPTransport], Dict[str, AsyncHTTPTransport]]:
         if type_ == "async":
+            atransport = AsyncHTTPTransport(
+                limits=Limits(
+                    max_connections=self.__connection_config.session_pool_maxsize,
+                    max_keepalive_connections=self.__connection_config.session_pool_connections,
+                ),
+                retries=self.__connection_config.session_pool_max_retries,
+                trust_env=self.__trust_env,
+            )
             return {
-                f"{key}://"
-                if key == "http" or key == "https"
-                else key: AsyncHTTPTransport(
-                    limits=Limits(
-                        max_connections=self.__connection_config.session_pool_maxsize,
-                        max_keepalive_connections=self.__connection_config.session_pool_connections,
-                    ),
-                    proxy=proxy,
-                    retries=self.__connection_config.session_pool_max_retries,
-                    trust_env=self.__trust_env,
-                )
-                for key, proxy in self._proxies.items()
-                if key != "grpc"
+                "http://": atransport,
+                "https://": atransport,
             }
         else:
             assert type_ == "sync"
+            transport = HTTPTransport(
+                limits=Limits(
+                    max_connections=self.__connection_config.session_pool_maxsize,
+                    max_keepalive_connections=self.__connection_config.session_pool_connections,
+                ),
+                retries=self.__connection_config.session_pool_max_retries,
+                trust_env=self.__trust_env,
+            )
             return {
-                f"{key}://"
-                if key == "http" or key == "https"
-                else key: HTTPTransport(
-                    limits=Limits(
-                        max_connections=self.__connection_config.session_pool_maxsize,
-                        max_keepalive_connections=self.__connection_config.session_pool_connections,
-                    ),
-                    proxy=proxy,
-                    retries=self.__connection_config.session_pool_max_retries,
-                    trust_env=self.__trust_env,
-                )
-                for key, proxy in self._proxies.items()
-                if key != "grpc"
+                "http://": transport,
+                "https://": transport,
             }
 
     def __make_sync_client(self) -> Client:
         return Client(
             headers=self._headers,
             timeout=Timeout(
-                None, connect=self.timeout_config.query, read=self.timeout_config.insert
+                None, connect=self.timeout_config.connect, read=self.timeout_config.read
             ),
+            proxies=self._proxies,
             mounts=self.__make_mounts("sync"),
         )
 
     def __make_async_client(self) -> AsyncClient:
         return AsyncClient(
             headers=self._headers,
             timeout=Timeout(
-                None, connect=self.timeout_config.query, read=self.timeout_config.insert
+                None, connect=self.timeout_config.connect, read=self.timeout_config.read
             ),
+            proxies=self._proxies,
             mounts=self.__make_mounts("async"),
         )
 
     def __make_clients(self) -> None:
         self._client = self.__make_sync_client()
 
     def _create_clients(
@@ -356,17 +355,15 @@
         )
         demon.start()
 
     async def aopen(self) -> None:
         if self._aclient is None:
             self._aclient = self.__make_async_client()
         if self._grpc_stub_async is None:
-            self._grpc_channel_async = self._connection_params._grpc_channel(
-                async_channel=True, proxies=self._proxies
-            )
+            self._grpc_channel_async = self._connection_params._grpc_channel(async_channel=True)
             assert self._grpc_channel_async is not None
             self._grpc_stub_async = weaviate_pb2_grpc.WeaviateStub(self._grpc_channel_async)
 
     async def aclose(self) -> None:
         if self._aclient is not None:
             await self._aclient.aclose()
             self._aclient = None
@@ -582,16 +579,16 @@
 
 
 class ConnectionV4(_Connection):
     def __init__(
         self,
         connection_params: ConnectionParams,
         auth_client_secret: Optional[AuthCredentials],
-        timeout_config: TimeoutConfig,
-        proxies: Union[str, Proxies, None],
+        timeout_config: TIMEOUT_TYPE_RETURN,
+        proxies: Union[dict, str, None],
         trust_env: bool,
         additional_headers: Optional[Dict[str, Any]],
         connection_config: ConnectionConfig,
         embedded_db: Optional[EmbeddedV4] = None,
     ):
         super().__init__(
             connection_params,
@@ -641,26 +638,24 @@
             raise WeaviateClosedClientError()
         assert self._grpc_channel is not None
         try:
             res: health_pb2.HealthCheckResponse = self._grpc_channel.unary_unary(
                 "/grpc.health.v1.Health/Check",
                 request_serializer=health_pb2.HealthCheckRequest.SerializeToString,
                 response_deserializer=health_pb2.HealthCheckResponse.FromString,
-            )(health_pb2.HealthCheckRequest(), timeout=self.timeout_config.init)
+            )(health_pb2.HealthCheckRequest(), timeout=1)
             if res.status != health_pb2.HealthCheckResponse.SERVING:
                 raise WeaviateGRPCUnavailableError(f"v{self.server_version}")
         except _channel._InactiveRpcError as e:
             raise WeaviateGRPCUnavailableError(f"v{self.server_version}") from e
 
     def connect(self, skip_init_checks: bool) -> None:
         super().connect(skip_init_checks)
         # create GRPC channel. If Weaviate does not support GRPC then error now.
-        self._grpc_channel = self._connection_params._grpc_channel(
-            async_channel=False, proxies=self._proxies
-        )
+        self._grpc_channel = self._connection_params._grpc_channel(async_channel=False)
         assert self._grpc_channel is not None
         self._grpc_stub = weaviate_pb2_grpc.WeaviateStub(self._grpc_channel)
         if not skip_init_checks:
             self._ping_grpc()
 
         # do it after all other init checks so as not to break all the tests
         if self._weaviate_version.is_lower_than(1, 23, 7):
```

### Comparing `weaviate-client-4.5.4/weaviate/contextionary/crud_contextionary.py` & `weaviate-client-4.5rc0/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/data/crud_data.py` & `weaviate-client-4.5rc0/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/data/references/crud_references.py` & `weaviate-client-4.5rc0/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/embedded.py` & `weaviate-client-4.5rc0/weaviate/embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/error_msgs.py` & `weaviate-client-4.5rc0/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/exceptions.py` & `weaviate-client-4.5rc0/weaviate/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,17 +271,15 @@
 
 class WeaviateGRPCUnavailableError(WeaviateBaseError):
     """Is raised when a gRPC-backed query is made with no gRPC connection present."""
 
     def __init__(self, weaviate_version: str = "") -> None:
         msg = f"""gRPC health check could not be completed. This could have several reasons:
         - gRPC is not enabled or incorrectly configured on the server with version {weaviate_version} or the client
-        - your connection is unstable or has a high latency. In this case you can:
-            - increase init-timeout in `weaviate.connect_to_local(additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=X)))`
-            - disable startup checks by connecting using `skip_init_checks=True`
+        - your connection is unstable or has a high latency. In this case you can disable startup checks by connecting using `skip_init_checks=True`
         """
         super().__init__(msg)
 
 
 WeaviateGrpcUnavailable = WeaviateGRPCUnavailableError
```

### Comparing `weaviate-client-4.5.4/weaviate/gql/aggregate.py` & `weaviate-client-4.5rc0/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/gql/filter.py` & `weaviate-client-4.5rc0/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/gql/get.py` & `weaviate-client-4.5rc0/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/gql/multi_get.py` & `weaviate-client-4.5rc0/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/gql/query.py` & `weaviate-client-4.5rc0/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/outputs/aggregate.py` & `weaviate-client-4.5rc0/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/outputs/config.py` & `weaviate-client-4.5rc0/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/outputs/query.py` & `weaviate-client-4.5rc0/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/base_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/base_pb2.pyi` & `weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/batch_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/batch_pb2.pyi` & `weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/properties_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/properties_pb2.pyi` & `weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/search_get_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/weaviate_pb2.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/schema/crud_schema.py` & `weaviate-client-4.5rc0/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/schema/properties/crud_properties.py` & `weaviate-client-4.5rc0/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/types.py` & `weaviate-client-4.5rc0/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/util.py` & `weaviate-client-4.5rc0/weaviate/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,17 +453,15 @@
     ) from None
 
 
 def _get_vector_v4(vector: Sequence) -> List[float]:
     try:
         return get_vector(vector)
     except TypeError as e:
-        raise WeaviateInvalidInputError(
-            f"The vector you supplied was malformatted! Vector:  {vector}"
-        ) from e
+        raise WeaviateInvalidInputError("") from e
 
 
 def get_domain_from_weaviate_url(url: str) -> str:
     """
     Get the domain from a weaviate URL.
 
     Parameters
```

### Comparing `weaviate-client-4.5.4/weaviate/validator.py` & `weaviate-client-4.5rc0/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate/warnings.py` & `weaviate-client-4.5rc0/weaviate/warnings.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5.4/weaviate_client.egg-info/PKG-INFO` & `weaviate-client-4.5rc0/weaviate_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.5.4
+Version: 4.5rc0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate-client-4.5.4/weaviate_client.egg-info/SOURCES.txt` & `weaviate-client-4.5rc0/weaviate_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 .github/workflows/main.yaml
 ci/docker-compose-async.yml
 ci/docker-compose-azure.yml
 ci/docker-compose-cluster.yml
 ci/docker-compose-generative.yml
 ci/docker-compose-okta-cc.yml
 ci/docker-compose-okta-users.yml
-ci/docker-compose-proxy.yml
 ci/docker-compose-rerank.yml
 ci/docker-compose-wcs.yml
 ci/docker-compose.yml
 ci/start_weaviate.sh
 ci/stop_weaviate.sh
-ci/proxy/envoy.yaml
 docs/Makefile
 docs/README.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
@@ -139,15 +137,14 @@
 test/collection/__init__.py
 test/collection/conftest.py
 test/collection/test_aggregates.py
 test/collection/test_classes.py
 test/collection/test_client.py
 test/collection/test_collection_model.py
 test/collection/test_config.py
-test/collection/test_filter.py
 test/collection/test_queries.py
 test/connection/__init__.py
 test/connection/test_connection.py
 test/contextionary/__init__.py
 test/contextionary/test_text2vec_contextionary.py
 test/data/__init__.py
 test/data/test_crud_data.py
```

